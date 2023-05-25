# Comparing `tmp/canvasapi-3.1.0.tar.gz` & `tmp/canvasapi-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canvasapi-3.1.0.tar", last modified: Fri Apr 21 23:07:46 2023, max compression
+gzip compressed data, was "canvasapi-3.2.0.tar", last modified: Thu May 25 14:45:51 2023, max compression
```

## Comparing `canvasapi-3.1.0.tar` & `canvasapi-3.2.0.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 23:07:46.250545 canvasapi-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-21 23:07:43.000000 canvasapi-3.1.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-21 23:07:43.000000 canvasapi-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-04-21 23:07:46.250545 canvasapi-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-04-21 23:07:43.000000 canvasapi-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 23:07:46.250545 canvasapi-3.1.0/canvasapi/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70346 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/account_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/appointment_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    23021 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/authentication_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/authentication_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/avatar.py
--rw-r--r--   0 runner    (1001) docker     (123)    10710 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/bookmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/calendar_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    50761 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/canvas_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/collaboration.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/comm_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/communication_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/content_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/content_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)    96214 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/course.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/course_epub_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/course_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/current_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/custom_gradebook_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)    22480 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/discussion_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/enrollment_term.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/eportfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/external_feed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/external_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/favorite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/grade_change_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/gradebook_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/grading_period.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/grading_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)    40859 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/license.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/module.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/notification_preference.py
--rw-r--r--   0 runner    (1001) docker     (123)    14174 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/outcome_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     8649 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/page.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/page_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/pairing_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/peer_review.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/poll_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/poll_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/poll_submission.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    32609 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/quiz.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/quiz_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/rubric.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/sis_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/submission.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/tab.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/todo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/usage_rights.py
--rw-r--r--   0 runner    (1001) docker     (123)    38451 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 23:07:46.250545 canvasapi-3.1.0/canvasapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-04-21 23:07:46.000000 canvasapi-3.1.0/canvasapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-21 23:07:46.000000 canvasapi-3.1.0/canvasapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 23:07:46.000000 canvasapi-3.1.0/canvasapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 23:07:46.000000 canvasapi-3.1.0/canvasapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-21 23:07:46.000000 canvasapi-3.1.0/canvasapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 23:07:46.000000 canvasapi-3.1.0/canvasapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-21 23:07:46.250545 canvasapi-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-21 23:07:43.000000 canvasapi-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:45:51.942722 canvasapi-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-25 14:45:50.000000 canvasapi-3.2.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-25 14:45:50.000000 canvasapi-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-25 14:45:51.942722 canvasapi-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-05-25 14:45:50.000000 canvasapi-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:45:51.942722 canvasapi-3.2.0/canvasapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70346 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/account_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/appointment_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23021 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/authentication_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/authentication_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/avatar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10710 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/calendar_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50761 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/canvas_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/collaboration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/comm_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/communication_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/content_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/content_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99485 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/course.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/course_epub_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/course_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/current_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/custom_gradebook_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22480 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/discussion_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/enrollment_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/eportfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/external_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/external_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/favorite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/grade_change_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/gradebook_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/grading_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/grading_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40859 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/new_quiz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/notification_preference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14174 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/outcome_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/page_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/pairing_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/peer_review.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/poll_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/poll_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/poll_submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32609 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/quiz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/quiz_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/rubric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/sis_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/todo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/usage_rights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38451 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-05-25 14:45:50.000000 canvasapi-3.2.0/canvasapi/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:45:51.942722 canvasapi-3.2.0/canvasapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-25 14:45:51.000000 canvasapi-3.2.0/canvasapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-25 14:45:51.000000 canvasapi-3.2.0/canvasapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:45:51.000000 canvasapi-3.2.0/canvasapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:45:51.000000 canvasapi-3.2.0/canvasapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 14:45:51.000000 canvasapi-3.2.0/canvasapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 14:45:51.000000 canvasapi-3.2.0/canvasapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-25 14:45:51.942722 canvasapi-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-25 14:45:50.000000 canvasapi-3.2.0/setup.py
```

### Comparing `canvasapi-3.1.0/AUTHORS.md` & `canvasapi-3.2.0/AUTHORS.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-Authors
-=======
+# Authors
 
-Development Lead
-----------------
+## Original Authors
 
 - Matthew Emond <me@ucf.edu> [@Thetwam](https://github.com/Thetwam)
 - Jesse McBride <jm@ucf.edu> [@jessemcbride](https://github.com/jessemcbride)
 
-Patches and Suggestions
------------------------
+## Maintainers
+
+- Matthew Emond [@Thetwam](https://github.com/Thetwam) (Lead)
+- Brian Bennett [@bennettscience](https://github.com/bennettscience)
+- Matthew Jones [@jonespm](https://github.com/jonespm)
+
+## Patches and Suggestions
 
 - Abrahan Nevarez [@zenith110](https://github.com/zenith110)
 - Adrian Goetz [@a-goetz](https://github.com/a-goetz)
 - Aileen Pongnon [@aileenpongnon](https://github.com/aileenpongnon)
 - Alyssa Davis [@allygator](https://github.com/allygator)
 - [@amorqiu](https://github.com/amorqiu)
 - Andrew Gardener [@andrew-gardener](https://github.com/andrew-gardener)
@@ -20,18 +23,18 @@
 - Ashutosh Saxena [@Xx-Ashutosh-xX](https://github.com/Xx-Ashutosh-xX)
 - Ben Liblit [@liblit](https://github.com/liblit)
 - Benjamin Reed [@breed](https://github.com/breed)
 - Bill Wrbican [@wjw27](https://github.com/wjw27)
 - [@Birdmaaan4](https://github.com/Birdmaaan4)
 - [@blepabyte](https://github.com/blepabyte)
 - Bradford Lynch [@bradfordlynch](https://github.com/bradfordlynch)
-- Brian Bennett [@bennettscience](https://github.com/bennettscience)
 - Bruce Spang [@brucespang](https://github.com/brucespang)
-- Catherine Abbruzzese [@cat0698](https://github.com/cat0698))
+- Caitlin Fabian [@Caitlin-Fabian](https://github.com/Caitlin-Fabian)
 - Cameron Cuff [@ctcuff](https://github.com/ctcuff)
+- Catherine Abbruzzese [@cat0698](https://github.com/cat0698)
 - Craig Thompson [@craigdsthompson](https://github.com/craigdsthompson)
 - Dalton Durst [@UniversalSuperBox](https://github.com/UniversalSuperBox)
 - Damian Sweeney [@damianfs](https://github.com/damianfs)
 - Daniel Brinkman [@DanBrink91](https://github.com/DanBrink91)
 - Daniel Grobani [@dgrobani](https://github.com/dgrobani)
 - Daniel Molares [@dmols](https://github.com/dmols)
 - David Warden [@dfwarden](https://github.com/dfwarden)
@@ -63,15 +66,14 @@
 - Lawrence Oks [@ljoks](https://github.com/ljoks)
 - Lee Fent [@lafent](https://github.com/lafent)
 - Leonard Camacho [@lcamacho](https://github.com/lcamacho)
 - Lucas Salas [@lucas-salas](https://github.com/lucas-salas)
 - Mark Lalor [@MarkLalor](https://github.com/MarkLalor)
 - Markus [@elec3647](https://github.com/elec3647)
 - Matthew Fedder [@matthewf-ucsd](https://github.com/matthewf-ucsd)
-- Matthew Jones [@jonespm](https://github.com/jonespm)
 - Michael Phelps [@nottheswimmer](https://github.com/nottheswimmer)
 - Mike Nahmias [@Mike-Nahmias](https://github.com/Mike-Nahmias)
 - Mike Suhan [@mikesuhan](https://github.com/mikesuhan)
 - Nathan Dabu [@nathaned](https://github.com/nathaned)
 - Petar Nikolovski [@petarGitNik](https://github.com/petarGitNik)
 - Philip Austin [@phaustin](https://github.com/phaustin)
 - Philip Carter [@phillyc](https://github.com/phillyc)
```

### Comparing `canvasapi-3.1.0/LICENSE` & `canvasapi-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/PKG-INFO` & `canvasapi-3.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvasapi
-Version: 3.1.0
+Version: 3.2.0
 Summary: API wrapper for the Canvas LMS
 Home-page: https://github.com/ucfopen/canvasapi
 Author: University of Central Florida - Center for Distributed Learning
 Author-email: techrangers@ucf.edu
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 [![CanvasAPI on PyPI](https://img.shields.io/pypi/v/canvasapi.svg)](https://pypi.python.org/pypi/canvasapi)
 [![License](https://img.shields.io/pypi/l/canvasapi.svg)](https://pypi.python.org/pypi/canvasapi)
@@ -33,27 +34,27 @@
 
 # CanvasAPI
 
 CanvasAPI is a Python library for accessing Instructure’s [Canvas LMS API](https://canvas.instructure.com/doc/api/index.html). The library enables developers to programmatically manage Canvas courses, users, gradebooks, and more.
 
 ## Table of Contents
 
-* [CanvasAPI](#canvasapi)
-    * [Table of Contents](#table-of-contents)
-    * [Installation](#installation)
-    * [Documentation](#documentation)
-    * [Contributing](#contributing)
-    * [Quickstart](#quickstart)
-        * [Working with Canvas Objects](#working-with-canvas-objects)
-            * [Course objects](#course-objects)
-            * [User objects](#user-objects)
-            * [Paginated Lists](#paginated-lists)
-            * [Keyword arguments](#keyword-arguments)
-    * [CanvasAPI Projects](#canvasapi-projects)
-    * [Contact Us](#contact-us)
+- [CanvasAPI](#canvasapi)
+  - [Table of Contents](#table-of-contents)
+  - [Installation](#installation)
+  - [Documentation](#documentation)
+  - [Contributing](#contributing)
+  - [Quickstart](#quickstart)
+    - [Working with Canvas Objects](#working-with-canvas-objects)
+      - [Course objects](#course-objects)
+      - [User objects](#user-objects)
+      - [Paginated Lists](#paginated-lists)
+      - [Keyword arguments](#keyword-arguments)
+  - [CanvasAPI Projects](#canvasapi-projects)
+  - [Contact Us](#contact-us)
 
 ## Installation
 
 You can install CanvasAPI with pip:
 
 `pip install canvasapi`
 
@@ -176,19 +177,19 @@
 
 For a more detailed description of how CanvasAPI handles more complex keyword arguments, check out the [Keyword Argument Documentation](http://canvasapi.readthedocs.io/en/stable/keyword-args.html).
 
 ## CanvasAPI Projects
 
 Since its initial release in June 2016, CanvasAPI has amassed over 100 [dependent repositories](https://github.com/ucfopen/canvasapi/network/dependents). Many of these include various tools used to enhance the Canvas experience for both instructors and students. Here are a few popular repositories that use CanvasAPI:
 
-* [Canvas Grab](https://github.com/skyzh/canvas_grab)
-    * Canvas Grab is the most popular project using CanvasAPI. This tool, with one click, copies all files from Canvas LMS to local directory. CanvasAPI is used in this project to connect to a course and grab its files.
-* [Clanvas](https://github.com/marklalor/clanvas)
-    * Clanvas is a command-line client for Canvas. It uses the already available bash commands plus some additional ones to interact with various features of Canvas from the commmand line.
-* [CS221Bot](https://github.com/Person314159/cs221bot)
-    * CS221Bot is a Discord bot for the CPCS 221 course at University of British Columbia. CanvasAPI is used in this project to connect to and synchronize with a course and get its data, such as announcements, new assignments, and more.
+- [Canvas Grab](https://github.com/skyzh/canvas_grab)
+  - Canvas Grab is the most popular project using CanvasAPI. This tool, with one click, copies all files from Canvas LMS to local directory. CanvasAPI is used in this project to connect to a course and grab its files.
+- [Clanvas](https://github.com/marklalor/clanvas)
+  - Clanvas is a command-line client for Canvas. It uses the already available bash commands plus some additional ones to interact with various features of Canvas from the commmand line.
+- [CS221Bot](https://github.com/Person314159/cs221bot)
+  - CS221Bot is a Discord bot for the CPCS 221 course at University of British Columbia. CanvasAPI is used in this project to connect to and synchronize with a course and get its data, such as announcements, new assignments, and more.
 
 If you have a project that uses CanvasAPI that you'd like to promote, please contact us!
 
 ## Contact Us
 
 Need help? Have an idea? Feel free to check out our [Discussions](https://github.com/ucfopen/canvasapi/discussions) board. Just want to say hi or get extended spport? Come join us on the [UCF Open Slack Channel](https://dl.ucf.edu/join-ucfopen) and join the `#canvasapi` channel!
```

### Comparing `canvasapi-3.1.0/README.md` & `canvasapi-3.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 
 # CanvasAPI
 
 CanvasAPI is a Python library for accessing Instructure’s [Canvas LMS API](https://canvas.instructure.com/doc/api/index.html). The library enables developers to programmatically manage Canvas courses, users, gradebooks, and more.
 
 ## Table of Contents
 
-* [CanvasAPI](#canvasapi)
-    * [Table of Contents](#table-of-contents)
-    * [Installation](#installation)
-    * [Documentation](#documentation)
-    * [Contributing](#contributing)
-    * [Quickstart](#quickstart)
-        * [Working with Canvas Objects](#working-with-canvas-objects)
-            * [Course objects](#course-objects)
-            * [User objects](#user-objects)
-            * [Paginated Lists](#paginated-lists)
-            * [Keyword arguments](#keyword-arguments)
-    * [CanvasAPI Projects](#canvasapi-projects)
-    * [Contact Us](#contact-us)
+- [CanvasAPI](#canvasapi)
+  - [Table of Contents](#table-of-contents)
+  - [Installation](#installation)
+  - [Documentation](#documentation)
+  - [Contributing](#contributing)
+  - [Quickstart](#quickstart)
+    - [Working with Canvas Objects](#working-with-canvas-objects)
+      - [Course objects](#course-objects)
+      - [User objects](#user-objects)
+      - [Paginated Lists](#paginated-lists)
+      - [Keyword arguments](#keyword-arguments)
+  - [CanvasAPI Projects](#canvasapi-projects)
+  - [Contact Us](#contact-us)
 
 ## Installation
 
 You can install CanvasAPI with pip:
 
 `pip install canvasapi`
 
@@ -152,19 +152,19 @@
 
 For a more detailed description of how CanvasAPI handles more complex keyword arguments, check out the [Keyword Argument Documentation](http://canvasapi.readthedocs.io/en/stable/keyword-args.html).
 
 ## CanvasAPI Projects
 
 Since its initial release in June 2016, CanvasAPI has amassed over 100 [dependent repositories](https://github.com/ucfopen/canvasapi/network/dependents). Many of these include various tools used to enhance the Canvas experience for both instructors and students. Here are a few popular repositories that use CanvasAPI:
 
-* [Canvas Grab](https://github.com/skyzh/canvas_grab)
-    * Canvas Grab is the most popular project using CanvasAPI. This tool, with one click, copies all files from Canvas LMS to local directory. CanvasAPI is used in this project to connect to a course and grab its files.
-* [Clanvas](https://github.com/marklalor/clanvas)
-    * Clanvas is a command-line client for Canvas. It uses the already available bash commands plus some additional ones to interact with various features of Canvas from the commmand line.
-* [CS221Bot](https://github.com/Person314159/cs221bot)
-    * CS221Bot is a Discord bot for the CPCS 221 course at University of British Columbia. CanvasAPI is used in this project to connect to and synchronize with a course and get its data, such as announcements, new assignments, and more.
+- [Canvas Grab](https://github.com/skyzh/canvas_grab)
+  - Canvas Grab is the most popular project using CanvasAPI. This tool, with one click, copies all files from Canvas LMS to local directory. CanvasAPI is used in this project to connect to a course and grab its files.
+- [Clanvas](https://github.com/marklalor/clanvas)
+  - Clanvas is a command-line client for Canvas. It uses the already available bash commands plus some additional ones to interact with various features of Canvas from the commmand line.
+- [CS221Bot](https://github.com/Person314159/cs221bot)
+  - CS221Bot is a Discord bot for the CPCS 221 course at University of British Columbia. CanvasAPI is used in this project to connect to and synchronize with a course and get its data, such as announcements, new assignments, and more.
 
 If you have a project that uses CanvasAPI that you'd like to promote, please contact us!
 
 ## Contact Us
 
 Need help? Have an idea? Feel free to check out our [Discussions](https://github.com/ucfopen/canvasapi/discussions) board. Just want to say hi or get extended spport? Come join us on the [UCF Open Slack Channel](https://dl.ucf.edu/join-ucfopen) and join the `#canvasapi` channel!
```

### Comparing `canvasapi-3.1.0/canvasapi/account.py` & `canvasapi-3.2.0/canvasapi/account.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/appointment_group.py` & `canvasapi-3.2.0/canvasapi/appointment_group.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/assignment.py` & `canvasapi-3.2.0/canvasapi/assignment.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/authentication_provider.py` & `canvasapi-3.2.0/canvasapi/authentication_provider.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/blueprint.py` & `canvasapi-3.2.0/canvasapi/blueprint.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/bookmark.py` & `canvasapi-3.2.0/canvasapi/bookmark.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/calendar_event.py` & `canvasapi-3.2.0/canvasapi/calendar_event.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/canvas.py` & `canvasapi-3.2.0/canvasapi/canvas.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/canvas_object.py` & `canvasapi-3.2.0/canvasapi/canvas_object.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/collaboration.py` & `canvasapi-3.2.0/canvasapi/collaboration.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/communication_channel.py` & `canvasapi-3.2.0/canvasapi/communication_channel.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/content_migration.py` & `canvasapi-3.2.0/canvasapi/content_migration.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/conversation.py` & `canvasapi-3.2.0/canvasapi/conversation.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/course.py` & `canvasapi-3.2.0/canvasapi/course.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     SubmissionHistory,
     SubmissionVersion,
 )
 from canvasapi.grading_period import GradingPeriod
 from canvasapi.grading_standard import GradingStandard
 from canvasapi.license import License
 from canvasapi.module import Module
+from canvasapi.new_quiz import NewQuiz
 from canvasapi.outcome_import import OutcomeImport
 from canvasapi.page import Page
 from canvasapi.paginated_list import PaginatedList
 from canvasapi.progress import Progress
 from canvasapi.quiz import QuizExtension
 from canvasapi.rubric import Rubric, RubricAssociation
 from canvasapi.submission import GroupedSubmission, Submission
@@ -274,33 +275,45 @@
             _kwargs=combine_kwargs(**kwargs),
         )
         column_json = response.json()
         column_json.update({"course_id": self.id})
 
         return CustomGradebookColumn(self._requester, column_json)
 
-    def create_discussion_topic(self, **kwargs):
+    def create_discussion_topic(self, attachment=None, **kwargs):
         """
         Creates a new discussion topic for the course or group.
 
         :calls: `POST /api/v1/courses/:course_id/discussion_topics \
         <https://canvas.instructure.com/doc/api/discussion_topics.html#method.discussion_topics.create>`_
 
+        :param attachment: (Optional) A file handler or path of the file to import.
+        :type attachment: file or str
+
         :rtype: :class:`canvasapi.discussion_topic.DiscussionTopic`
         """
-        response = self._requester.request(
-            "POST",
-            "courses/{}/discussion_topics".format(self.id),
-            _kwargs=combine_kwargs(**kwargs),
-        )
+        if attachment is not None:
+            attachment_file, is_path = file_or_path(attachment)
+            attachment = {"attachment": attachment_file}
+
+        try:
+            response = self._requester.request(
+                "POST",
+                "courses/{}/discussion_topics".format(self.id),
+                file=attachment,
+                _kwargs=combine_kwargs(**kwargs),
+            )
 
-        response_json = response.json()
-        response_json.update({"course_id": self.id})
+            response_json = response.json()
+            response_json.update({"course_id": self.id})
 
-        return DiscussionTopic(self._requester, response_json)
+            return DiscussionTopic(self._requester, response_json)
+        finally:
+            if attachment is not None and is_path:
+                attachment_file.close()
 
     def create_epub_export(self, **kwargs):
         """
         Create an ePub export for a course.
 
         :calls: `POST /api/v1/courses/:course_id/epub_exports/:id\
         <https://canvas.instructure.com/doc/api/e_pub_exports.html#method.epub_exports.create>`_
@@ -448,14 +461,37 @@
             _kwargs=combine_kwargs(**kwargs),
         )
         module_json = response.json()
         module_json.update({"course_id": self.id})
 
         return Module(self._requester, module_json)
 
+    def create_new_quiz(self, **kwargs):
+        """
+        Create a new quiz for the course.
+
+        :calls: `POST /api/quiz/v1/courses/:course_id/quizzes \
+        <https://canvas.instructure.com/doc/api/new_quizzes.html#method.new_quizzes/quizzes_api.create>`_
+
+        :returns: The newly-created New Quiz object
+        :rtype: :class:`canvasapi.new_quiz.NewQuiz`
+        """
+        endpoint = "courses/{}/quizzes".format(self.id)
+
+        response = self._requester.request(
+            "POST",
+            endpoint,
+            _url=self._requester.original_url + "/api/quiz/v1/" + endpoint,
+            _kwargs=combine_kwargs(**kwargs),
+        )
+        response_json = response.json()
+        response_json.update({"course_id": self.id})
+
+        return NewQuiz(self._requester, response_json)
+
     def create_page(self, wiki_page, **kwargs):
         """
         Create a new wiki page.
 
         :calls: `POST /api/v1/courses/:course_id/pages \
         <https://canvas.instructure.com/doc/api/pages.html#method.wiki_pages_api.create>`_
 
@@ -1697,14 +1733,64 @@
             self._requester,
             "GET",
             "courses/{}/students/submissions".format(self.id),
             {"course_id": self.id},
             _kwargs=combine_kwargs(**kwargs),
         )
 
+    def get_new_quiz(self, assignment, **kwargs):
+        """
+        Get details about a single new quiz.
+
+        :calls: `GET /api/quiz/v1/courses/:course_id/quizzes/:assignment_id \
+        <https://canvas.instructure.com/doc/api/new_quizzes.html#method.new_quizzes/quizzes_api.show>`_
+
+        :param assignment: The id of the assignment associated with the quiz.
+        :type assignment: :class:`canvasapi.assignment.Assignment`
+            or :class:`canvasapi.new_quiz.NewQuiz` or int
+
+        :returns: A New Quiz object.
+        :rtype: :class:`canvasapi.new_quiz.NewQuiz`
+        """
+
+        assignment_id = obj_or_id(assignment, "assignment", (Assignment, NewQuiz))
+        endpoint = "courses/{}/quizzes/{}".format(self.id, assignment_id)
+
+        response = self._requester.request(
+            "GET",
+            endpoint,
+            _url=self._requester.original_url + "/api/quiz/v1/" + endpoint,
+            _kwargs=combine_kwargs(**kwargs),
+        )
+        response_json = response.json()
+        response_json.update({"course_id": self.id})
+
+        return NewQuiz(self._requester, response_json)
+
+    def get_new_quizzes(self, **kwargs):
+        """
+        Get a list of new quizzes.
+
+        :calls: `GET /api/quiz/v1/courses/:course_id/quizzes \
+        <https://canvas.instructure.com/doc/api/new_quizzes.html#method.new_quizzes/quizzes_api.index>`_
+
+        :returns: A paginated list of New Quiz objects.
+        :rtype: :class:`canvasapi.paginated_list.PaginatedList`
+            of :class:`canvasapi.new_quiz.NewQuiz`
+        """
+        endpoint = "courses/{}/quizzes".format(self.id)
+        return PaginatedList(
+            NewQuiz,
+            self._requester,
+            "GET",
+            endpoint,
+            _url_override=self._requester.original_url + "/api/quiz/v1/" + endpoint,
+            _kwargs=combine_kwargs(**kwargs),
+        )
+
     def get_outcome_group(self, group, **kwargs):
         """
         Returns the details of the Outcome Group with the given id.
 
         :calls: `GET /api/v1/courses/:course_id/outcome_groups/:id \
             <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.show>`_
 
@@ -1715,15 +1801,17 @@
         :rtype: :class:`canvasapi.outcome.OutcomeGroup`
         """
         from canvasapi.outcome import OutcomeGroup
 
         outcome_group_id = obj_or_id(group, "group", (OutcomeGroup,))
 
         response = self._requester.request(
-            "GET", "courses/{}/outcome_groups/{}".format(self.id, outcome_group_id)
+            "GET",
+            "courses/{}/outcome_groups/{}".format(self.id, outcome_group_id),
+            _kwargs=combine_kwargs(**kwargs),
         )
 
         return OutcomeGroup(self._requester, response.json())
 
     def get_outcome_groups_in_context(self, **kwargs):
         """
         Get all outcome groups for context - BETA
```

### Comparing `canvasapi-3.1.0/canvasapi/current_user.py` & `canvasapi-3.2.0/canvasapi/current_user.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/custom_gradebook_columns.py` & `canvasapi-3.2.0/canvasapi/custom_gradebook_columns.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/discussion_topic.py` & `canvasapi-3.2.0/canvasapi/discussion_topic.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/enrollment.py` & `canvasapi-3.2.0/canvasapi/enrollment.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/enrollment_term.py` & `canvasapi-3.2.0/canvasapi/enrollment_term.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/eportfolio.py` & `canvasapi-3.2.0/canvasapi/eportfolio.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/exceptions.py` & `canvasapi-3.2.0/canvasapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/external_tool.py` & `canvasapi-3.2.0/canvasapi/external_tool.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/favorite.py` & `canvasapi-3.2.0/canvasapi/favorite.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/feature.py` & `canvasapi-3.2.0/canvasapi/feature.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/file.py` & `canvasapi-3.2.0/canvasapi/file.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/folder.py` & `canvasapi-3.2.0/canvasapi/folder.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/grading_period.py` & `canvasapi-3.2.0/canvasapi/grading_period.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/group.py` & `canvasapi-3.2.0/canvasapi/group.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/login.py` & `canvasapi-3.2.0/canvasapi/login.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/module.py` & `canvasapi-3.2.0/canvasapi/module.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/outcome.py` & `canvasapi-3.2.0/canvasapi/outcome.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/page.py` & `canvasapi-3.2.0/canvasapi/page.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,25 @@
         return "{} ({})".format(self.title, self.url)
 
     def delete(self, **kwargs):
         """
         Delete this page.
 
         :calls: `DELETE /api/v1/courses/:course_id/pages/:url \
-        <https://canvas.instructure.com/doc/api/pages.html#method.wiki_pages_api.destroy>`_
+            <https://canvas.instructure.com/doc/api/pages.html#method.wiki_pages_api.destroy>`_
+            or
+            `DELETE /api/v1/groups/:group_id/pages/:url \
+            <https://canvas.instructure.com/doc/api/pages.html#method.wiki_pages_api.destroy>`_
 
         :rtype: :class:`canvasapi.page.Page`
         """
+
         response = self._requester.request(
             "DELETE",
-            "courses/{}/pages/{}".format(self.course_id, self.url),
+            "{}s/{}/pages/{}".format(self.parent_type, self.parent_id, self.url),
             _kwargs=combine_kwargs(**kwargs),
         )
         return Page(self._requester, response.json())
 
     def edit(self, **kwargs):
         """
         Update the title or the contents of a specified wiki
@@ -47,15 +51,16 @@
 
     def get_parent(self, **kwargs):
         """
         Return the object that spawned this page.
 
         :calls: `GET /api/v1/groups/:group_id \
             <https://canvas.instructure.com/doc/api/groups.html#method.groups.show>`_
-            or :calls: `GET /api/v1/courses/:id \
+            or
+            `GET /api/v1/courses/:id \
             <https://canvas.instructure.com/doc/api/courses.html#method.courses.show>`_
 
         :rtype: :class:`canvasapi.group.Group` or :class:`canvasapi.course.Course`
         """
         from canvasapi.course import Course
         from canvasapi.group import Group
```

### Comparing `canvasapi-3.1.0/canvasapi/paginated_list.py` & `canvasapi-3.2.0/canvasapi/paginated_list.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,64 +21,84 @@
         self,
         content_class,
         requester,
         request_method,
         first_url,
         extra_attribs=None,
         _root=None,
+        _url_override=None,
         **kwargs
     ):
         self._elements = list()
 
         self._requester = requester
         self._content_class = content_class
         self._first_url = first_url
         self._first_params = kwargs or {}
         self._first_params["per_page"] = kwargs.get("per_page", 100)
         self._next_url = first_url
         self._next_params = self._first_params
         self._extra_attribs = extra_attribs or {}
         self._request_method = request_method
         self._root = _root
+        self._url_override = _url_override
 
     def __iter__(self):
         for element in self._elements:
             yield element
         while self._has_next():
             new_elements = self._grow()
             for element in new_elements:
                 yield element
 
     def __repr__(self):
         return "<PaginatedList of type {}>".format(self._content_class.__name__)
 
     def _get_next_page(self):
         response = self._requester.request(
-            self._request_method, self._next_url, **self._next_params
+            self._request_method,
+            self._next_url,
+            _url=self._url_override,
+            **self._next_params,
         )
         data = response.json()
         self._next_url = None
+        # Check the response headers first. This is the normal Canvas convention
+        # for pagination, but there are endpoints which return a `meta` property
+        # for pagination instead.
+        # See https://github.com/ucfopen/canvasapi/discussions/605
+        if response.links:
+            next_link = response.links.get("next")
+        elif isinstance(data, dict) and "meta" in data:
+            # requests parses headers into dicts, this returns the same
+            # structure so the regex will still work.
+            try:
+                next_link = {"url": data["meta"]["pagination"]["next"], "rel": "next"}
+            except KeyError:
+                next_link = None
+        else:
+            next_link = None
 
-        next_link = response.links.get("next")
         regex = r"{}(.*)".format(re.escape(self._requester.base_url))
 
         self._next_url = (
             re.search(regex, next_link["url"]).group(1) if next_link else None
         )
 
         self._next_params = {}
 
         content = []
 
         if self._root:
             try:
                 data = data[self._root]
             except KeyError:
-                # TODO: Fix this message to make more sense to an end user.
-                raise ValueError("Invalid root value specified.")
+                raise ValueError(
+                    "The key <{}> does not exist in the response.".format(self._root)
+                )
 
         for element in data:
             if element is not None:
                 element.update(self._extra_attribs)
                 content.append(self._content_class(self._requester, element))
 
         return content
```

### Comparing `canvasapi-3.1.0/canvasapi/planner.py` & `canvasapi-3.2.0/canvasapi/planner.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/poll.py` & `canvasapi-3.2.0/canvasapi/poll.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/poll_choice.py` & `canvasapi-3.2.0/canvasapi/poll_choice.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/poll_session.py` & `canvasapi-3.2.0/canvasapi/poll_session.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/progress.py` & `canvasapi-3.2.0/canvasapi/progress.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/quiz.py` & `canvasapi-3.2.0/canvasapi/quiz.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/quiz_group.py` & `canvasapi-3.2.0/canvasapi/quiz_group.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/requester.py` & `canvasapi-3.2.0/canvasapi/requester.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         if json:
             return self._session.post(url, headers=headers, json=dict(data))
 
         # Grab file from data.
         files = None
         for field, value in data:
             if field == "file":
-                if isinstance(value, dict):
+                if isinstance(value, dict) or value is None:
                     files = value
                 else:
                     files = {"file": value}
                 break
 
         # Remove file entry from data.
         data[:] = [tup for tup in data if tup[0] != "file"]
```

### Comparing `canvasapi-3.1.0/canvasapi/rubric.py` & `canvasapi-3.2.0/canvasapi/rubric.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/section.py` & `canvasapi-3.2.0/canvasapi/section.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/sis_import.py` & `canvasapi-3.2.0/canvasapi/sis_import.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/submission.py` & `canvasapi-3.2.0/canvasapi/submission.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/tab.py` & `canvasapi-3.2.0/canvasapi/tab.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/upload.py` & `canvasapi-3.2.0/canvasapi/upload.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/user.py` & `canvasapi-3.2.0/canvasapi/user.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi/util.py` & `canvasapi-3.2.0/canvasapi/util.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.1.0/canvasapi.egg-info/PKG-INFO` & `canvasapi-3.2.0/canvasapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvasapi
-Version: 3.1.0
+Version: 3.2.0
 Summary: API wrapper for the Canvas LMS
 Home-page: https://github.com/ucfopen/canvasapi
 Author: University of Central Florida - Center for Distributed Learning
 Author-email: techrangers@ucf.edu
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 [![CanvasAPI on PyPI](https://img.shields.io/pypi/v/canvasapi.svg)](https://pypi.python.org/pypi/canvasapi)
 [![License](https://img.shields.io/pypi/l/canvasapi.svg)](https://pypi.python.org/pypi/canvasapi)
@@ -33,27 +34,27 @@
 
 # CanvasAPI
 
 CanvasAPI is a Python library for accessing Instructure’s [Canvas LMS API](https://canvas.instructure.com/doc/api/index.html). The library enables developers to programmatically manage Canvas courses, users, gradebooks, and more.
 
 ## Table of Contents
 
-* [CanvasAPI](#canvasapi)
-    * [Table of Contents](#table-of-contents)
-    * [Installation](#installation)
-    * [Documentation](#documentation)
-    * [Contributing](#contributing)
-    * [Quickstart](#quickstart)
-        * [Working with Canvas Objects](#working-with-canvas-objects)
-            * [Course objects](#course-objects)
-            * [User objects](#user-objects)
-            * [Paginated Lists](#paginated-lists)
-            * [Keyword arguments](#keyword-arguments)
-    * [CanvasAPI Projects](#canvasapi-projects)
-    * [Contact Us](#contact-us)
+- [CanvasAPI](#canvasapi)
+  - [Table of Contents](#table-of-contents)
+  - [Installation](#installation)
+  - [Documentation](#documentation)
+  - [Contributing](#contributing)
+  - [Quickstart](#quickstart)
+    - [Working with Canvas Objects](#working-with-canvas-objects)
+      - [Course objects](#course-objects)
+      - [User objects](#user-objects)
+      - [Paginated Lists](#paginated-lists)
+      - [Keyword arguments](#keyword-arguments)
+  - [CanvasAPI Projects](#canvasapi-projects)
+  - [Contact Us](#contact-us)
 
 ## Installation
 
 You can install CanvasAPI with pip:
 
 `pip install canvasapi`
 
@@ -176,19 +177,19 @@
 
 For a more detailed description of how CanvasAPI handles more complex keyword arguments, check out the [Keyword Argument Documentation](http://canvasapi.readthedocs.io/en/stable/keyword-args.html).
 
 ## CanvasAPI Projects
 
 Since its initial release in June 2016, CanvasAPI has amassed over 100 [dependent repositories](https://github.com/ucfopen/canvasapi/network/dependents). Many of these include various tools used to enhance the Canvas experience for both instructors and students. Here are a few popular repositories that use CanvasAPI:
 
-* [Canvas Grab](https://github.com/skyzh/canvas_grab)
-    * Canvas Grab is the most popular project using CanvasAPI. This tool, with one click, copies all files from Canvas LMS to local directory. CanvasAPI is used in this project to connect to a course and grab its files.
-* [Clanvas](https://github.com/marklalor/clanvas)
-    * Clanvas is a command-line client for Canvas. It uses the already available bash commands plus some additional ones to interact with various features of Canvas from the commmand line.
-* [CS221Bot](https://github.com/Person314159/cs221bot)
-    * CS221Bot is a Discord bot for the CPCS 221 course at University of British Columbia. CanvasAPI is used in this project to connect to and synchronize with a course and get its data, such as announcements, new assignments, and more.
+- [Canvas Grab](https://github.com/skyzh/canvas_grab)
+  - Canvas Grab is the most popular project using CanvasAPI. This tool, with one click, copies all files from Canvas LMS to local directory. CanvasAPI is used in this project to connect to a course and grab its files.
+- [Clanvas](https://github.com/marklalor/clanvas)
+  - Clanvas is a command-line client for Canvas. It uses the already available bash commands plus some additional ones to interact with various features of Canvas from the commmand line.
+- [CS221Bot](https://github.com/Person314159/cs221bot)
+  - CS221Bot is a Discord bot for the CPCS 221 course at University of British Columbia. CanvasAPI is used in this project to connect to and synchronize with a course and get its data, such as announcements, new assignments, and more.
 
 If you have a project that uses CanvasAPI that you'd like to promote, please contact us!
 
 ## Contact Us
 
 Need help? Have an idea? Feel free to check out our [Discussions](https://github.com/ucfopen/canvasapi/discussions) board. Just want to say hi or get extended spport? Come join us on the [UCF Open Slack Channel](https://dl.ucf.edu/join-ucfopen) and join the `#canvasapi` channel!
```

### Comparing `canvasapi-3.1.0/canvasapi.egg-info/SOURCES.txt` & `canvasapi-3.2.0/canvasapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 canvasapi/grading_period.py
 canvasapi/grading_standard.py
 canvasapi/group.py
 canvasapi/jwt.py
 canvasapi/license.py
 canvasapi/login.py
 canvasapi/module.py
+canvasapi/new_quiz.py
 canvasapi/notification_preference.py
 canvasapi/outcome.py
 canvasapi/outcome_import.py
 canvasapi/page.py
 canvasapi/page_view.py
 canvasapi/paginated_list.py
 canvasapi/pairing_code.py
```

### Comparing `canvasapi-3.1.0/setup.py` & `canvasapi-3.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,10 +39,11 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries",
     ],
 )
```

