# Comparing `tmp/django-common-task-system-1.3.0.tar.gz` & `tmp/django-common-task-system-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-common-task-system-1.3.0.tar", last modified: Sat May 20 07:22:59 2023, max compression
+gzip compressed data, was "django-common-task-system-1.3.3.tar", last modified: Thu May 25 03:23:06 2023, max compression
```

## Comparing `django-common-task-system-1.3.0.tar` & `django-common-task-system-1.3.3.tar`

### file list

```diff
@@ -1,106 +1,120 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 07:22:59.069970 django-common-task-system-1.3.0/
--rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.3.0/LICENSE
--rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0      303 2023-05-20 07:22:59.069970 django-common-task-system-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 07:22:58.551720 django-common-task-system-1.3.0/django_common_task_system/
--rw-rw-rw-   0        0        0     3015 2023-05-04 05:28:57.000000 django-common-task-system-1.3.0/django_common_task_system/__init__.py
--rw-rw-rw-   0        0        0    11644 2023-05-17 06:20:23.000000 django-common-task-system-1.3.0/django_common_task_system/admin.py
--rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.3.0/django_common_task_system/apps.py
--rw-rw-rw-   0        0        0     1596 2023-04-17 06:43:49.000000 django-common-task-system-1.3.0/django_common_task_system/choices.py
--rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.3.0/django_common_task_system/fields.py
--rw-rw-rw-   0        0        0    18454 2023-05-18 06:23:57.000000 django-common-task-system-1.3.0/django_common_task_system/forms.py
-drwxrwxrwx   0        0        0        0 2023-05-20 07:22:58.647406 django-common-task-system-1.3.0/django_common_task_system/migrations/
--rw-rw-rw-   0        0        0     7688 2023-05-17 03:19:48.000000 django-common-task-system-1.3.0/django_common_task_system/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.3.0/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
--rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.3.0/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
--rw-rw-rw-   0        0        0     3283 2023-04-13 08:54:07.000000 django-common-task-system-1.3.0/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
--rw-rw-rw-   0        0        0      495 2023-04-17 01:38:40.000000 django-common-task-system-1.3.0/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
--rw-rw-rw-   0        0        0     1560 2023-04-17 08:33:41.000000 django-common-task-system-1.3.0/django_common_task_system/migrations/0006_consumerpermission.py
--rw-rw-rw-   0        0        0     1275 2023-04-21 07:23:00.000000 django-common-task-system-1.3.0/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py
--rw-rw-rw-   0        0        0      490 2023-05-09 02:37:58.000000 django-common-task-system-1.3.0/django_common_task_system/migrations/0008_taskschedule_strict_mode.py
--rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.3.0/django_common_task_system/migrations/__init__.py
--rw-rw-rw-   0        0        0     2679 2023-04-18 06:27:17.000000 django-common-task-system-1.3.0/django_common_task_system/mixin.py
--rw-rw-rw-   0        0        0    37039 2023-05-17 03:20:38.000000 django-common-task-system-1.3.0/django_common_task_system/models.py
--rw-rw-rw-   0        0        0     1010 2023-04-17 08:01:11.000000 django-common-task-system-1.3.0/django_common_task_system/permissions.py
--rw-rw-rw-   0        0        0     2475 2023-05-17 06:20:23.000000 django-common-task-system-1.3.0/django_common_task_system/serializers.py
-drwxrwxrwx   0        0        0        0 2023-05-20 07:22:58.442864 django-common-task-system-1.3.0/django_common_task_system/static/
-drwxrwxrwx   0        0        0        0 2023-05-20 07:22:58.443860 django-common-task-system-1.3.0/django_common_task_system/static/common_task_system/
-drwxrwxrwx   0        0        0        0 2023-05-20 07:22:58.658872 django-common-task-system-1.3.0/django_common_task_system/static/common_task_system/css/
--rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.3.0/django_common_task_system/static/common_task_system/css/calendar.css
--rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.3.0/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
-drwxrwxrwx   0        0        0        0 2023-05-20 07:22:58.702546 django-common-task-system-1.3.0/django_common_task_system/static/common_task_system/js/
--rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.3.0/django_common_task_system/static/common_task_system/js/calendar.js
--rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.3.0/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
--rw-rw-rw-   0        0        0     1558 2023-05-18 02:21:07.000000 django-common-task-system-1.3.0/django_common_task_system/static/common_task_system/js/task_type_admin.js
-drwxrwxrwx   0        0        0        0 2023-05-20 07:22:58.785274 django-common-task-system-1.3.0/django_common_task_system/system_task/
--rw-rw-rw-   0        0        0        0 2023-04-13 02:42:52.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/__init__.py
--rw-rw-rw-   0        0        0     5339 2023-05-18 02:04:00.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/admin.py
--rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/apps.py
--rw-rw-rw-   0        0        0    15577 2023-05-19 01:56:40.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/builtins.py
--rw-rw-rw-   0        0        0      629 2023-04-14 01:40:24.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/choices.py
--rw-rw-rw-   0        0        0     6929 2023-05-18 09:15:54.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/forms.py
-drwxrwxrwx   0        0        0        0 2023-05-20 07:22:58.849968 django-common-task-system-1.3.0/django_common_task_system/system_task/migrations/
--rw-rw-rw-   0        0        0    10476 2023-05-17 03:19:48.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
--rw-rw-rw-   0        0        0     2209 2023-04-13 05:28:04.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
--rw-rw-rw-   0        0        0     1007 2023-04-13 08:54:07.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
--rw-rw-rw-   0        0        0      467 2023-04-17 01:38:40.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
--rw-rw-rw-   0        0        0     1540 2023-04-17 08:33:41.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
--rw-rw-rw-   0        0        0     1062 2023-04-21 07:23:00.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py
--rw-rw-rw-   0        0        0      454 2023-05-09 02:37:58.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/migrations/0008_systemschedule_strict_mode.py
--rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/migrations/__init__.py
--rw-rw-rw-   0        0        0     4706 2023-05-15 05:40:55.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/models.py
--rw-rw-rw-   0        0        0     1132 2023-04-17 01:38:40.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/process.py
--rw-rw-rw-   0        0        0     2237 2023-04-13 07:08:11.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/queue.py
--rw-rw-rw-   0        0        0     1679 2023-04-21 07:11:39.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/serializers.py
--rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/tests.py
--rw-rw-rw-   0        0        0      877 2023-05-15 09:14:29.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/urls.py
--rw-rw-rw-   0        0        0     6405 2023-05-18 08:18:37.000000 django-common-task-system-1.3.0/django_common_task_system/system_task/views.py
-drwxrwxrwx   0        0        0        0 2023-05-20 07:22:58.859965 django-common-task-system-1.3.0/django_common_task_system/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.3.0/django_common_task_system/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     1674 2023-04-19 09:54:46.000000 django-common-task-system-1.3.0/django_common_task_system/system_task_execution/main.py
-drwxrwxrwx   0        0        0        0 2023-05-20 07:22:58.884958 django-common-task-system-1.3.0/django_common_task_system/system_task_execution/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.3.0/django_common_task_system/system_task_execution/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     2484 2023-05-15 07:47:12.000000 django-common-task-system-1.3.0/django_common_task_system/system_task_execution/system_task_execution/executor.py
-drwxrwxrwx   0        0        0        0 2023-05-20 07:22:58.944648 django-common-task-system-1.3.0/django_common_task_system/system_task_execution/system_task_execution/executors/
--rw-rw-rw-   0        0        0      669 2023-05-18 08:40:30.000000 django-common-task-system-1.3.0/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
--rw-rw-rw-   0        0        0     1332 2023-05-18 09:42:50.000000 django-common-task-system-1.3.0/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
--rw-rw-rw-   0        0        0     3283 2023-05-19 02:14:42.000000 django-common-task-system-1.3.0/django_common_task_system/system_task_execution/system_task_execution/executors/custom_program.py
--rw-rw-rw-   0        0        0     3859 2023-05-17 09:11:21.000000 django-common-task-system-1.3.0/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
--rw-rw-rw-   0        0        0      834 2023-05-15 07:46:24.000000 django-common-task-system-1.3.0/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
--rw-rw-rw-   0        0        0     1379 2023-05-17 06:57:02.000000 django-common-task-system-1.3.0/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
--rw-rw-rw-   0        0        0    11026 2023-05-17 09:31:21.000000 django-common-task-system-1.3.0/django_common_task_system/system_task_execution/system_task_execution/executors/strict_schedule.py
--rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.3.0/django_common_task_system/system_task_execution/system_task_execution/settings.py
--rw-rw-rw-   0        0        0     1258 2023-05-17 09:10:41.000000 django-common-task-system-1.3.0/django_common_task_system/system_task_execution/system_task_execution/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-20 07:22:58.445861 django-common-task-system-1.3.0/django_common_task_system/templates/
-drwxrwxrwx   0        0        0        0 2023-05-20 07:22:58.445861 django-common-task-system-1.3.0/django_common_task_system/templates/admin/
-drwxrwxrwx   0        0        0        0 2023-05-20 07:22:58.975834 django-common-task-system-1.3.0/django_common_task_system/templates/admin/system_schedule/
--rw-rw-rw-   0        0        0     8242 2023-04-19 07:36:00.000000 django-common-task-system-1.3.0/django_common_task_system/templates/admin/system_schedule/change_list.html
-drwxrwxrwx   0        0        0        0 2023-05-20 07:22:59.040076 django-common-task-system-1.3.0/django_common_task_system/templates/task_schedule/
--rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.3.0/django_common_task_system/templates/task_schedule/datetime_range.html
--rw-rw-rw-   0        0        0      279 2023-05-18 02:18:05.000000 django-common-task-system-1.3.0/django_common_task_system/templates/task_schedule/executable_file.html
--rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.3.0/django_common_task_system/templates/task_schedule/multi_day_select.html
--rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.3.0/django_common_task_system/templates/task_schedule/multi_month_day_select.html
--rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.3.0/django_common_task_system/templates/task_schedule/nlp_input.html
--rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.3.0/django_common_task_system/templates/task_schedule/period.html
--rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.3.0/django_common_task_system/templates/task_schedule/period_schedule.html
--rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.3.0/django_common_task_system/tests.py
--rw-rw-rw-   0        0        0     1089 2023-05-15 09:14:29.000000 django-common-task-system-1.3.0/django_common_task_system/urls.py
-drwxrwxrwx   0        0        0        0 2023-05-20 07:22:59.067965 django-common-task-system-1.3.0/django_common_task_system/utils/
--rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.3.0/django_common_task_system/utils/__init__.py
--rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.3.0/django_common_task_system/utils/algorithm.py
--rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.3.0/django_common_task_system/utils/cron_utils.py
--rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.3.0/django_common_task_system/utils/foreign_key.py
--rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.3.0/django_common_task_system/utils/schedule_time.py
--rw-rw-rw-   0        0        0    12233 2023-05-17 09:11:36.000000 django-common-task-system-1.3.0/django_common_task_system/views.py
-drwxrwxrwx   0        0        0        0 2023-05-20 07:22:58.580028 django-common-task-system-1.3.0/django_common_task_system.egg-info/
--rw-rw-rw-   0        0        0      303 2023-05-20 07:22:58.000000 django-common-task-system-1.3.0/django_common_task_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5048 2023-05-20 07:22:58.000000 django-common-task-system-1.3.0/django_common_task_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 07:22:58.000000 django-common-task-system-1.3.0/django_common_task_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-05-20 07:22:58.000000 django-common-task-system-1.3.0/django_common_task_system.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-05-20 07:22:58.000000 django-common-task-system-1.3.0/django_common_task_system.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 07:22:59.069970 django-common-task-system-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      611 2023-05-20 07:22:05.000000 django-common-task-system-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 07:22:59.068969 django-common-task-system-1.3.0/tests/
--rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.3.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.591874 django-common-task-system-1.3.3/
+-rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0      189 2023-05-20 07:32:40.000000 django-common-task-system-1.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      307 2023-05-25 03:23:06.590881 django-common-task-system-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.3.3/README.md
+-rw-rw-rw-   0        0        0        0 2023-05-24 09:43:33.000000 django-common-task-system-1.3.3/deploy.sh
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.143861 django-common-task-system-1.3.3/django_common_task_system/
+-rw-rw-rw-   0        0        0     3015 2023-05-24 09:35:14.000000 django-common-task-system-1.3.3/django_common_task_system/__init__.py
+-rw-rw-rw-   0        0        0    11644 2023-05-17 06:20:23.000000 django-common-task-system-1.3.3/django_common_task_system/admin.py
+-rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.3.3/django_common_task_system/apps.py
+-rw-rw-rw-   0        0        0     1596 2023-04-17 06:43:49.000000 django-common-task-system-1.3.3/django_common_task_system/choices.py
+-rw-rw-rw-   0        0        0    20540 2023-05-23 08:16:03.000000 django-common-task-system-1.3.3/django_common_task_system/forms.py
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.230222 django-common-task-system-1.3.3/django_common_task_system/migrations/
+-rw-rw-rw-   0        0        0     7635 2023-05-23 09:02:13.000000 django-common-task-system-1.3.3/django_common_task_system/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.3.3/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
+-rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.3.3/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
+-rw-rw-rw-   0        0        0     3283 2023-04-13 08:54:07.000000 django-common-task-system-1.3.3/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      495 2023-04-17 01:38:40.000000 django-common-task-system-1.3.3/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1560 2023-04-17 08:33:41.000000 django-common-task-system-1.3.3/django_common_task_system/migrations/0006_consumerpermission.py
+-rw-rw-rw-   0        0        0     1275 2023-04-21 07:23:00.000000 django-common-task-system-1.3.3/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py
+-rw-rw-rw-   0        0        0      490 2023-05-09 02:37:58.000000 django-common-task-system-1.3.3/django_common_task_system/migrations/0008_taskschedule_strict_mode.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.3.3/django_common_task_system/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2679 2023-04-18 06:27:17.000000 django-common-task-system-1.3.3/django_common_task_system/mixin.py
+-rw-rw-rw-   0        0        0    37016 2023-05-23 09:01:47.000000 django-common-task-system-1.3.3/django_common_task_system/models.py
+-rw-rw-rw-   0        0        0     1010 2023-04-17 08:01:11.000000 django-common-task-system-1.3.3/django_common_task_system/permissions.py
+-rw-rw-rw-   0        0        0     2756 2023-05-25 02:51:03.000000 django-common-task-system-1.3.3/django_common_task_system/serializers.py
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.050121 django-common-task-system-1.3.3/django_common_task_system/static/
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.050121 django-common-task-system-1.3.3/django_common_task_system/static/common_task_system/
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.240219 django-common-task-system-1.3.3/django_common_task_system/static/common_task_system/css/
+-rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.3.3/django_common_task_system/static/common_task_system/css/calendar.css
+-rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.3.3/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.281759 django-common-task-system-1.3.3/django_common_task_system/static/common_task_system/js/
+-rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.3.3/django_common_task_system/static/common_task_system/js/calendar.js
+-rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.3.3/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
+-rw-rw-rw-   0        0        0     1688 2023-05-23 08:07:41.000000 django-common-task-system-1.3.3/django_common_task_system/static/common_task_system/js/task_type_admin.js
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.306792 django-common-task-system-1.3.3/django_common_task_system/static/custom_programs/
+-rw-rw-rw-   0        0        0       29 2023-05-23 06:02:29.000000 django-common-task-system-1.3.3/django_common_task_system/static/custom_programs/python_test.py
+-rw-rw-rw-   0        0        0       19 2023-05-18 09:30:02.000000 django-common-task-system-1.3.3/django_common_task_system/static/custom_programs/shell_test.sh
+-rw-rw-rw-   0        0        0      317 2023-05-23 06:44:01.000000 django-common-task-system-1.3.3/django_common_task_system/static/custom_programs/zip_test.zip
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.369961 django-common-task-system-1.3.3/django_common_task_system/system_task/
+-rw-rw-rw-   0        0        0        0 2023-04-13 02:42:52.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/__init__.py
+-rw-rw-rw-   0        0        0     5370 2023-05-25 03:17:35.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/admin.py
+-rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/apps.py
+-rw-rw-rw-   0        0        0    15100 2023-05-25 02:25:35.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/builtins.py
+-rw-rw-rw-   0        0        0      629 2023-04-14 01:40:24.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/choices.py
+-rw-rw-rw-   0        0        0     8704 2023-05-23 08:21:17.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/forms.py
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.429176 django-common-task-system-1.3.3/django_common_task_system/system_task/migrations/
+-rw-rw-rw-   0        0        0    10423 2023-05-23 09:02:19.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
+-rw-rw-rw-   0        0        0     2209 2023-04-13 05:28:04.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
+-rw-rw-rw-   0        0        0     1007 2023-04-13 08:54:07.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      467 2023-04-17 01:38:40.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1540 2023-04-17 08:33:41.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
+-rw-rw-rw-   0        0        0     1062 2023-04-21 07:23:00.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py
+-rw-rw-rw-   0        0        0      454 2023-05-09 02:37:58.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/migrations/0008_systemschedule_strict_mode.py
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4706 2023-05-15 05:40:55.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/models.py
+-rw-rw-rw-   0        0        0     1132 2023-04-17 01:38:40.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/process.py
+-rw-rw-rw-   0        0        0     2237 2023-04-13 07:08:11.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/queue.py
+-rw-rw-rw-   0        0        0     1679 2023-04-21 07:11:39.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/serializers.py
+-rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/tests.py
+-rw-rw-rw-   0        0        0      877 2023-05-15 09:14:29.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/urls.py
+-rw-rw-rw-   0        0        0     6405 2023-05-18 08:18:37.000000 django-common-task-system-1.3.3/django_common_task_system/system_task/views.py
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.435690 django-common-task-system-1.3.3/django_common_task_system/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.3.3/django_common_task_system/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     1674 2023-04-19 09:54:46.000000 django-common-task-system-1.3.3/django_common_task_system/system_task_execution/main.py
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.453614 django-common-task-system-1.3.3/django_common_task_system/system_task_execution/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.3.3/django_common_task_system/system_task_execution/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     2542 2023-05-25 02:44:13.000000 django-common-task-system-1.3.3/django_common_task_system/system_task_execution/system_task_execution/executor.py
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.503434 django-common-task-system-1.3.3/django_common_task_system/system_task_execution/system_task_execution/executors/
+-rw-rw-rw-   0        0        0      669 2023-05-18 08:40:30.000000 django-common-task-system-1.3.3/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
+-rw-rw-rw-   0        0        0     1332 2023-05-18 09:42:50.000000 django-common-task-system-1.3.3/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
+-rw-rw-rw-   0        0        0     5738 2023-05-23 06:41:42.000000 django-common-task-system-1.3.3/django_common_task_system/system_task_execution/system_task_execution/executors/custom_program.py
+-rw-rw-rw-   0        0        0     3536 2023-05-25 03:17:35.000000 django-common-task-system-1.3.3/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
+-rw-rw-rw-   0        0        0      834 2023-05-15 07:46:24.000000 django-common-task-system-1.3.3/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
+-rw-rw-rw-   0        0        0     2170 2023-05-23 08:40:46.000000 django-common-task-system-1.3.3/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
+-rw-rw-rw-   0        0        0    11026 2023-05-17 09:31:21.000000 django-common-task-system-1.3.3/django_common_task_system/system_task_execution/system_task_execution/executors/strict_schedule.py
+-rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.3.3/django_common_task_system/system_task_execution/system_task_execution/settings.py
+-rw-rw-rw-   0        0        0     1258 2023-05-17 09:10:41.000000 django-common-task-system-1.3.3/django_common_task_system/system_task_execution/system_task_execution/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.052121 django-common-task-system-1.3.3/django_common_task_system/templates/
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.051123 django-common-task-system-1.3.3/django_common_task_system/templates/admin/
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.503434 django-common-task-system-1.3.3/django_common_task_system/templates/admin/system_schedule/
+-rw-rw-rw-   0        0        0     8242 2023-04-19 07:36:00.000000 django-common-task-system-1.3.3/django_common_task_system/templates/admin/system_schedule/change_list.html
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.528185 django-common-task-system-1.3.3/django_common_task_system/templates/task_schedule/
+-rw-rw-rw-   0        0        0      576 2023-05-22 09:21:21.000000 django-common-task-system-1.3.3/django_common_task_system/templates/task_schedule/custom_program.html
+-rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.3.3/django_common_task_system/templates/task_schedule/datetime_range.html
+-rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.3.3/django_common_task_system/templates/task_schedule/multi_day_select.html
+-rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.3.3/django_common_task_system/templates/task_schedule/multi_month_day_select.html
+-rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.3.3/django_common_task_system/templates/task_schedule/nlp_input.html
+-rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.3.3/django_common_task_system/templates/task_schedule/period.html
+-rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.3.3/django_common_task_system/templates/task_schedule/period_schedule.html
+-rw-rw-rw-   0        0        0      689 2023-05-23 08:02:57.000000 django-common-task-system-1.3.3/django_common_task_system/templates/task_schedule/sql_config.html
+-rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.3.3/django_common_task_system/tests.py
+-rw-rw-rw-   0        0        0     1089 2023-05-15 09:14:29.000000 django-common-task-system-1.3.3/django_common_task_system/urls.py
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.549194 django-common-task-system-1.3.3/django_common_task_system/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.3.3/django_common_task_system/utils/__init__.py
+-rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.3.3/django_common_task_system/utils/algorithm.py
+-rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.3.3/django_common_task_system/utils/cron_utils.py
+-rw-rw-rw-   0        0        0     1150 2023-05-25 02:36:14.000000 django-common-task-system-1.3.3/django_common_task_system/utils/foreign_key.py
+-rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.3.3/django_common_task_system/utils/schedule_time.py
+-rw-rw-rw-   0        0        0    12528 2023-05-25 03:11:40.000000 django-common-task-system-1.3.3/django_common_task_system/views.py
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.170635 django-common-task-system-1.3.3/django_common_task_system.egg-info/
+-rw-rw-rw-   0        0        0      307 2023-05-25 03:23:06.000000 django-common-task-system-1.3.3/django_common_task_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5612 2023-05-25 03:23:06.000000 django-common-task-system-1.3.3/django_common_task_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 03:23:06.000000 django-common-task-system-1.3.3/django_common_task_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-05-25 03:23:06.000000 django-common-task-system-1.3.3/django_common_task_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       59 2023-05-25 03:23:06.000000 django-common-task-system-1.3.3/django_common_task_system.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.555019 django-common-task-system-1.3.3/django_common_task_system_server/
+-rw-rw-rw-   0        0        0        0 2023-05-24 03:33:23.000000 django-common-task-system-1.3.3/django_common_task_system_server/__init__.py
+-rw-rw-rw-   0        0        0      684 2023-05-24 09:44:29.000000 django-common-task-system-1.3.3/django_common_task_system_server/manage.py
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.589868 django-common-task-system-1.3.3/django_common_task_system_server/server/
+-rw-rw-rw-   0        0        0        0 2023-05-24 02:04:52.000000 django-common-task-system-1.3.3/django_common_task_system_server/server/__init__.py
+-rw-rw-rw-   0        0        0      405 2023-05-24 02:04:52.000000 django-common-task-system-1.3.3/django_common_task_system_server/server/asgi.py
+-rw-rw-rw-   0        0        0     3537 2023-05-24 09:22:43.000000 django-common-task-system-1.3.3/django_common_task_system_server/server/settings.py
+-rw-rw-rw-   0        0        0      769 2023-05-24 02:04:52.000000 django-common-task-system-1.3.3/django_common_task_system_server/server/urls.py
+-rw-rw-rw-   0        0        0      405 2023-05-24 02:04:52.000000 django-common-task-system-1.3.3/django_common_task_system_server/server/wsgi.py
+-rw-rw-rw-   0        0        0       42 2023-05-25 03:23:06.591874 django-common-task-system-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      626 2023-05-25 03:22:47.000000 django-common-task-system-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 03:23:06.590881 django-common-task-system-1.3.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.3.3/tests/__init__.py
```

### Comparing `django-common-task-system-1.3.0/LICENSE` & `django-common-task-system-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/__init__.py` & `django-common-task-system-1.3.3/django_common_task_system/__init__.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/admin.py` & `django-common-task-system-1.3.3/django_common_task_system/admin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/choices.py` & `django-common-task-system-1.3.3/django_common_task_system/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/forms.py` & `django-common-task-system-1.3.3/django_common_task_system/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,62 +10,104 @@
 from . import get_task_schedule_model, get_task_model
 
 
 TaskModel = get_task_model()
 ScheduleModel = get_task_schedule_model()
 
 
-class ExecutableFileWidget(forms.MultiWidget):
-    template_name = 'task_schedule/executable_file.html'
+class CustomProgramWidget(forms.MultiWidget):
+    template_name = 'task_schedule/custom_program.html'
 
     def __init__(self, attrs=None):
         file = widgets.AdminFileWidget()
-        args = widgets.AdminTextInputWidget(attrs={'style': 'width: 60%; margin-top: 5px; margin-left: 170px;',
-                                                   'placeholder': '参数, 例如: -a 1 -b 2'})
-        super().__init__([file, args], attrs=attrs)
-
-    def get_context(self, name, value, attrs):
-        context = super().get_context(name, value, attrs)
-        return context
+        args = widgets.AdminTextInputWidget(attrs={'style': 'width: 60%; margin-top: 1px; ',
+                                                   'placeholder': '例如: -a 1 -b 2'})
+        docker_image = widgets.AdminTextInputWidget(attrs={'style': 'margin-top: 1px; ',
+                                                           'placeholder': 'common-task-system-client:latest'})
+        run_in_docker = forms.CheckboxInput()
+        super().__init__([file, args, docker_image, run_in_docker], attrs=attrs)
 
-    def format_value(self, value):
+    def decompress(self, value):
         if value:
             return value
-        return [None, None]
+        return [None, None, None, False]
+
+
+class CustomProgramField(forms.MultiValueField):
+    widget = CustomProgramWidget
+
+    def __init__(self, required=False, label="可执行文件", initial=None, **kwargs):
+        if initial is None:
+            initial = [None, None, None, False]
+        a, b, c, d = initial
+        fs = (
+            forms.FileField(help_text='仅支持zip、python、shell格式', required=False, initial=a),
+            forms.CharField(help_text='例如: -a 1 -b 2', required=False, initial=b),
+            forms.CharField(help_text='Docker镜像', required=False, initial=c),
+            forms.BooleanField(label="在Docker中运行", help_text='在Docker中运行', initial=d),
+        )
+        super(CustomProgramField, self).__init__(fs, required=required, label=label, **kwargs)
+
+    def compress(self, data_list):
+        return data_list
+
+    def validate(self, value):
+        super(CustomProgramField, self).validate(value)
+        file, args, *_ = value
+        if file:
+            ext = file.name.split('.')[-1]
+            if ext not in ['zip', 'py', 'sh']:
+                raise forms.ValidationError('仅支持zip、python、shell格式')
+
+
+class SqlConfigWidget(forms.MultiWidget):
+    template_name = 'task_schedule/sql_config.html'
+
+    def __init__(self, attrs=None):
+        host = widgets.AdminTextInputWidget()
+        port = widgets.AdminIntegerFieldWidget()
+        db = widgets.AdminTextInputWidget(attrs={'style': 'width: 120px'})
+        user = widgets.AdminTextInputWidget()
+        pwd = widgets.AdminTextInputWidget(attrs={'type': 'password'})
+        super().__init__([host, port, db, user, pwd], attrs=attrs)
 
     def decompress(self, value):
         if value:
             return value
-        return [None, None]
+        return [None, 3306, None, 'root', None]
 
 
-class ExecutableFileField(forms.MultiValueField):
-    widget = ExecutableFileWidget
+class SqlConfigField(forms.MultiValueField):
+    widget = SqlConfigWidget
 
-    def __init__(self, required=False, label="可执行文件", initial=None, **kwargs):
+    def __init__(self, required=False, label="SQL配置", initial=None, **kwargs):
         if initial is None:
-            initial = [None, None]
-        a, b = initial
+            initial = [None, 3306, None, 'root', None]
+        a, b, c, d, e = initial
         fs = (
-            forms.FileField(help_text='仅支持zip、python、shell格式', initial="dadsad"),
-            forms.CharField(help_text='参数, 例如: -a 1 -b 2', initial=b)
+            forms.CharField(help_text='仅支持zip、python、shell格式', required=False, initial=a),
+            forms.IntegerField(help_text='端口', required=False, initial=b),
+            forms.CharField(help_text='DB', required=False, initial=c),
+            forms.CharField(help_text='用户名', required=False, initial=d),
+            forms.CharField(help_text='在Docker中运行', initial=e),
         )
-        super(ExecutableFileField, self).__init__(fs, required=required, label=label, **kwargs)
+        super(SqlConfigField, self).__init__(fs, required=required, label=label, **kwargs)
 
     def compress(self, data_list):
         return data_list
 
     def validate(self, value):
-        super(ExecutableFileField, self).validate(value)
-        file, args = value
-        if not file:
-            raise forms.ValidationError('文件不能为空')
-        ext = file.name.split('.')[-1]
-        if ext not in ['zip', 'py', 'sh']:
-            raise forms.ValidationError('仅支持zip、python、shell格式')
+        super(SqlConfigField, self).validate(value)
+        host, port, db, user, pwd = value
+        if host:
+            import pymysql
+            try:
+                pymysql.connect(host=host, port=port, db=db, user=user, password=pwd)
+            except Exception as e:
+                raise forms.ValidationError('连接失败: {}'.format(e))
 
 
 class TaskForm(forms.ModelForm):
 
     def __init__(self, *args, **kwargs):
         super(TaskForm, self).__init__(*args, **kwargs)
         task: TaskModel = self.instance
```

### Comparing `django-common-task-system-1.3.0/django_common_task_system/migrations/0001_initial.py` & `django-common-task-system-1.3.3/django_common_task_system/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import datetime
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 import django.utils.timezone
 import django_common_objects.fields
 import django_common_objects.models
-import django_common_task_system.fields
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
@@ -48,15 +47,15 @@
             name='TaskSchedule',
             fields=[
                 ('id', models.AutoField(primary_key=True, serialize=False)),
                 ('priority', models.IntegerField(default=0, verbose_name='优先级')),
                 ('next_schedule_time', models.DateTimeField(db_index=True, default=django.utils.timezone.now, verbose_name='下次运行时间')),
                 ('schedule_start_time', models.DateTimeField(default=datetime.datetime(1, 1, 1, 0, 0), verbose_name='开始时间')),
                 ('schedule_end_time', models.DateTimeField(default=datetime.datetime(9999, 12, 31, 23, 59, 59, 999999), verbose_name='结束时间')),
-                ('config', django_common_task_system.fields.ScheduleConfigField(default=dict, verbose_name='参数')),
+                ('config', django_common_objects.fields.ConfigField(default=dict, verbose_name='参数')),
                 ('status', django_common_objects.fields.CharField(choices=[('O', '开启'), ('C', '关闭'), ('D', '已完成'), ('T', '测试'), ('E', '调度错误')], default='O', max_length=1, verbose_name='状态')),
                 ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
                 ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
             ],
             options={
                 'verbose_name': '任务计划',
                 'verbose_name_plural': '任务计划',
```

### Comparing `django-common-task-system-1.3.0/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py` & `django-common-task-system-1.3.3/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py` & `django-common-task-system-1.3.3/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/migrations/0006_consumerpermission.py` & `django-common-task-system-1.3.3/django_common_task_system/migrations/0006_consumerpermission.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py` & `django-common-task-system-1.3.3/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/mixin.py` & `django-common-task-system-1.3.3/django_common_task_system/mixin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/models.py` & `django-common-task-system-1.3.3/django_common_task_system/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from .choices import TaskStatus, TaskScheduleStatus, TaskScheduleType, TaskCallbackStatus, \
     TaskCallbackEvent, ScheduleTimingType, ScheduleQueueModule, ConsumerPermissionType
 from django_common_objects.models import CommonTag, CommonCategory
 from django_common_objects import fields as common_fields
 from .utils.cron_utils import get_next_cron_time
 from .utils import foreign_key
 from datetime import datetime, timedelta
-from . import fields
 from jionlp_time import parse_time
 from .utils.schedule_time import nlp_config_to_schedule_config
 from . import settings
 from . permissions import ConsumerPermissionValidator
 import re
 import os
 from django.core.validators import ValidationError
@@ -432,15 +431,15 @@
 class AbstractTaskSchedule(models.Model):
     id = models.AutoField(primary_key=True)
     task = models.ForeignKey(settings.TASK_MODEL, on_delete=models.CASCADE, db_constraint=False, verbose_name='任务')
     priority = models.IntegerField(default=0, verbose_name='优先级')
     next_schedule_time = models.DateTimeField(default=timezone.now, verbose_name='下次运行时间', db_index=True)
     schedule_start_time = models.DateTimeField(default=datetime.min, verbose_name='开始时间')
     schedule_end_time = models.DateTimeField(default=datetime.max, verbose_name='结束时间')
-    config = fields.ScheduleConfigField(default=dict, verbose_name='参数')
+    config = common_fields.ConfigField(default=dict, verbose_name='参数')
     status = common_fields.CharField(default=TaskScheduleStatus.OPENING.value, verbose_name='状态',
                                      choices=TaskScheduleStatus.choices)
     strict_mode = models.BooleanField(default=False, verbose_name='严格模式')
     callback = models.ForeignKey(TaskScheduleCallback, on_delete=models.CASCADE,
                                  null=True, blank=True, db_constraint=False, verbose_name='回调')
     user = models.ForeignKey(UserModel, on_delete=models.CASCADE, db_constraint=False, verbose_name='用户')
     create_time = models.DateTimeField(default=timezone.now, verbose_name='创建时间')
```

### Comparing `django-common-task-system-1.3.0/django_common_task_system/permissions.py` & `django-common-task-system-1.3.3/django_common_task_system/permissions.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/serializers.py` & `django-common-task-system-1.3.3/django_common_task_system/serializers.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,19 +49,29 @@
 
 
 class QueueScheduleSerializer(TaskScheduleSerializer):
     task = QueueTaskSerializer()
     callback = TaskCallbackSerializer()
     schedule_time = serializers.DateTimeField(source="next_schedule_time")
     generator = serializers.SerializerMethodField()
+    last_log = serializers.SerializerMethodField()
+    queue = serializers.SerializerMethodField()
+
+    @staticmethod
+    def get_last_log(obj):
+        return getattr(obj, 'last_log', None)
 
     @staticmethod
     def get_generator(obj):
         return getattr(obj, 'generator', 'auto')
 
+    @staticmethod
+    def get_queue(obj):
+        return getattr(obj, 'queue')
+
     class Meta:
         model = ScheduleModel
         # fields = ('id', 'task', 'schedule_time', 'update_time', 'callback', 'user')
         exclude = ('priority', 'create_time', 'next_schedule_time', 'schedule_start_time',
                    'schedule_end_time', 'status', 'config')
```

### Comparing `django-common-task-system-1.3.0/django_common_task_system/static/common_task_system/css/calendar.css` & `django-common-task-system-1.3.3/django_common_task_system/static/common_task_system/css/calendar.css`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/static/common_task_system/js/calendar.js` & `django-common-task-system-1.3.3/django_common_task_system/static/common_task_system/js/calendar.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/static/common_task_system/js/task_schedule_admin.js` & `django-common-task-system-1.3.3/django_common_task_system/static/common_task_system/js/task_schedule_admin.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/static/common_task_system/js/task_type_admin.js` & `django-common-task-system-1.3.3/django_common_task_system/static/common_task_system/js/task_type_admin.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,35 +1,39 @@
 $(document).ready(function() {
     const $taskParent = $('#id_parent');
     const $taskScriptField = $('.form-row.field-script');
     const $produceQueue = $('.fieldBox.field-queue');
     const $includeMeta = $('.fieldBox.field-include_meta');
     const $config = $('.form-row.field-config');
     const $taskScriptInput = $('#id_script');
-    const $executable = $('.form-row.field-executable_file');
+    const $customProgram = $('.form-row.field-custom_program');
+    const $sqlConfig = $('.form-row.field-sql_config');
 
     function show_hide_fields() {
         const parentTask = $taskParent.find("option:selected").text();
         console.log("parent task is ", parentTask);
         $config.hide();
         $taskScriptField.show();
-        $executable.hide();
+        $customProgram.hide();
+        $sqlConfig.hide();
         if (parentTask === "SQL执行") {
             $taskScriptInput.attr('placeholder', "请输入SQL语句, 多个语句用;分隔");
             $produceQueue.hide();
             $includeMeta.hide();
+            $sqlConfig.show();
         } else if (parentTask === "SQL生产") {
             $taskScriptInput.attr('placeholder', "请输入单条select语句");
             $produceQueue.show();
             $includeMeta.show();
+            $sqlConfig.show();
         } else if (parentTask === "Shell执行") {
             $produceQueue.hide();
             $taskScriptInput.attr('placeholder', "请输入shell命令，多个命令用;分隔");
-        } else if (parentTask === "自定义可执行任务") {
-            $executable.show();
+        } else if (parentTask === "自定义程序") {
+            $customProgram.show();
             $produceQueue.hide();
             $includeMeta.hide();
             $taskScriptField.hide();
         } else {
             $config.show();
             $taskScriptField.hide();
             $includeMeta.hide();
```

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task/admin.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,16 @@
     schedule_model = models.SystemSchedule
     list_display = ('id', 'admin_parent', 'name', 'category', 'admin_status', 'schedules', 'update_time')
 
     fields = (
         'category',
         ("name", "status",),
         ("parent", 'queue', 'include_meta'),
-        ('executable_file',),
+        ('custom_program', ),
+        'sql_config',
         "script",
         "config",
         'description',
     )
     filter_horizontal = []
     list_filter = ('category', 'parent')
 
@@ -76,15 +77,15 @@
 
 class SystemScheduleAdmin(base_admin.TaskScheduleAdmin):
 
     task_model = models.SystemTask
     schedule_log_model = models.SystemScheduleLog
     queues = builtins.queues
     schedule_put_name = 'system_schedule_put'
-    list_filter = ('task__category', )
+    list_filter = ('task__category', 'status')
 
     def has_delete_permission(self, request, obj=None):
         if obj and not request.user.is_superuser:
             return obj.task.category != builtins.categories.system_default_category
         return True
```

#### html2text {}

```diff
@@ -15,28 +15,28 @@
 instance: models.SystemProcess, **kwargs): ProcessManager.kill
 (instance.process_id) if os.path.isfile(instance.log_file) and not
 instance.log_file.endswith('system-process-default.log'): os.remove
 (instance.log_file) class SystemTaskAdmin(base_admin.TaskAdmin): form =
 forms.SystemTaskForm schedule_model = models.SystemSchedule list_display =
 ('id', 'admin_parent', 'name', 'category', 'admin_status', 'schedules',
 'update_time') fields = ( 'category', ("name", "status",), ("parent", 'queue',
-'include_meta'), ('executable_file',), "script", "config", 'description', )
-filter_horizontal = [] list_filter = ('category', 'parent') def
-has_delete_permission(self, request, obj=None): if obj and not
+'include_meta'), ('custom_program', ), 'sql_config', "script", "config",
+'description', ) filter_horizontal = [] list_filter = ('category', 'parent')
+def has_delete_permission(self, request, obj=None): if obj and not
 request.user.is_superuser: return obj.category !=
 builtins.categories.system_default_category return True class Media: js =
 ( 'https://cdn.bootcss.com/jquery/3.3.1/jquery.min.js', 'https://
 cdn.bootcss.com/popper.js/1.14.3/umd/popper.min.js', 'https://cdn.bootcss.com/
 bootstrap/4.1.3/js/bootstrap.min.js', 'common_task_system/js/
 task_type_admin.js', ) class SystemScheduleCallbackAdmin
 (base_admin.TaskScheduleCallbackAdmin): pass class SystemScheduleAdmin
 (base_admin.TaskScheduleAdmin): task_model = models.SystemTask
 schedule_log_model = models.SystemScheduleLog queues = builtins.queues
-schedule_put_name = 'system_schedule_put' list_filter = ('task__category', )
-def has_delete_permission(self, request, obj=None): if obj and not
+schedule_put_name = 'system_schedule_put' list_filter = ('task__category',
+'status') def has_delete_permission(self, request, obj=None): if obj and not
 request.user.is_superuser: return obj.task.category !=
 builtins.categories.system_default_category return True class
 SystemScheduleLogAdmin(base_admin.TaskScheduleLogAdmin): schedule_retry_name =
 'system_schedule_retry' class SystemProcessAdmin(admin.ModelAdmin):
 list_display = ('process_id', 'process_name', 'log_file', 'status',
 'stop_process', 'show_log', 'update_time') form = forms.SystemProcessForm
 fields = ( 'system_path', 'process_name', 'env', 'log_file', 'process_id',
```

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task/builtins.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task/builtins.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     BaseBuiltinQueues, BaseBuiltinProducers, BaseConsumerPermissions, BaseBuiltins, UserModel,
     BuiltinModels
 )
 from django_common_objects.models import CommonCategory
 from django_common_task_system.system_task.models import SystemTask, SystemScheduleProducer, SystemSchedule, \
     SystemConsumerPermission, SystemScheduleLog, SystemScheduleQueue
 from django_common_task_system import get_schedule_log_model, get_task_schedule_model
+from django_common_task_system.utils.foreign_key import get_model_related
 
 
 class BuiltinCategories(BuiltinModels):
     model = CommonCategory
     model_unique_kwargs = ('name',)
 
     def __init__(self, user):
@@ -119,19 +120,19 @@
             user=user,
             category=categories.system_base_category,
             config={
                 'required_fields': ['queue']
             }
         )
         self.custom_program_parent_task = self.model(
-            name='自定义可执行任务',
+            name='自定义程序',
             user=user,
             category=categories.system_base_category,
             config={
-                'required_fields': ['executable_file']
+                'required_fields': ['custom_program']
             }
         )
 
         interval = 1
         unit = 'month'
         self.system_log_cleaning = self.model(
             name='系统日志清理',
@@ -203,29 +204,14 @@
             category=categories.system_test_category,
             config={
                 'script': 'echo "hello world"'
             },
             user=user
         )
 
-        def get_model_related(model, parent='', excludes=None):
-            related = []
-            for field in model._meta.fields:
-                t = field.__class__.__name__
-                if t == 'ForeignKey' and parent.split("__")[-1] != field.name:
-                    if excludes and field.related_model in excludes:
-                        continue
-                    if parent:
-                        child = parent + "__" + field.name
-                    else:
-                        child = field.name
-                    related.append(child)
-                    related.extend(get_model_related(field.related_model, parent=child, excludes=excludes))
-            return related
-
         self.system_strict_schedule_process = self.model(
             name='系统严格模式任务处理',
             parent=self.strict_schedule_parent_task,
             category=categories.system_default_category,
             user=user,
             config={
                 'schedule_model': SystemSchedule.__module__ + "." + SystemSchedule.__name__,
@@ -243,40 +229,46 @@
             config={
                 'schedule_model': task_schedule.__module__ + "." + task_schedule.__name__,
                 'log_model': log_model.__module__ + "." + log_model.__name__,
                 'related': get_model_related(task_schedule, excludes=[UserModel, CommonCategory]),
             }
         )
         import os
-        executable_path = os.path.abspath(os.path.join(os.path.dirname(__file__), '../static/executable'))
+        executable_path = os.path.abspath(os.path.join(os.path.dirname(__file__), '../static/custom_programs'))
         self.test_custom_python_program = self.model(
             name='测试自定义Python程序执行任务',
             parent=self.custom_program_parent_task,
             category=categories.system_test_category,
             user=user,
             config={
-                'executable_file': os.path.join(executable_path, 'python_test.py')
+                'custom_program': {
+                    'executable': os.path.join(executable_path, 'python_test.py')
+                }
             }
         )
         self.test_custom_shell_program = self.model(
             name='测试自定义Shell程序执行任务',
             parent=self.custom_program_parent_task,
             category=categories.system_test_category,
             user=user,
             config={
-                'executable_file': os.path.join(executable_path, 'shell_test.sh')
+                'custom_program': {
+                    'executable': os.path.join(executable_path, 'shell_test.sh')
+                }
             }
         )
         self.test_execute_zip_program = self.model(
             name='测试自定义zip程序执行任务',
             parent=self.custom_program_parent_task,
             category=categories.system_test_category,
             user=user,
             config={
-                'executable_file': os.path.join(executable_path, 'zip_test.zip')
+                'custom_program': {
+                    'executable': os.path.join(executable_path, 'zip_test.zip')
+                }
             }
         )
         super(BuiltinTasks, self).__init__()
 
 
 class BuiltinSchedules(BuiltinModels):
     model_unique_kwargs = ['task', 'user']
```

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task/choices.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task/forms.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task/forms.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import time
 import hashlib
 from .process import ProcessManager
 from ..system_task_execution.main import start_system_client
 from django_common_objects.widgets import JSONWidget
 from django.conf import settings
 from django_common_task_system.forms import (
-    TaskScheduleProducerForm, TaskScheduleQueueForm, ExecutableFileField
+    TaskScheduleProducerForm, TaskScheduleQueueForm, CustomProgramField, SqlConfigField
 )
 
 
 class InitialFileStr(str):
 
     @property
     def url(self):
@@ -46,32 +46,45 @@
     )
 
     script = forms.CharField(
         label='脚本',
         widget=forms.Textarea(attrs={'style': 'width: 70%;'}),
         required=False
     )
+    sql_config = SqlConfigField(required=False, label="SQL源", help_text="仅支持MySQL, 默认当前数据库")
     # 不知道为什么这里使用validators时，在admin新增任务时如果validator没通过，第一次会报错，第二次就不会报错了
-    executable_file = ExecutableFileField(required=False, help_text='仅支持zip、python、shell格式')
+    custom_program = CustomProgramField(required=False, help_text='仅支持zip、python、shell格式')
 
     executable_path = os.path.join(settings.STATIC_ROOT or os.path.join(os.getcwd(), 'static'), 'executable')
 
     def __init__(self, *args, **kwargs):
         super(SystemTaskForm, self).__init__(*args, **kwargs)
         if self.instance.id:
-            queue = self.instance.config.get('queue')
+            config = self.instance.config
+            queue = config.get('queue')
             if queue:
                 self.initial['queue'] = models.SystemScheduleQueue.objects.get(code=queue)
-            self.initial['script'] = self.instance.config.get('script')
-            self.initial['include_meta'] = self.instance.config.get('include_meta')
-            executable_file = self.instance.config.get('executable_file')
-            if executable_file:
-                self.initial['executable_file'] = [
-                    InitialFileStr(executable_file.replace(self.executable_path, '')),
-                    self.instance.config.get('executable_args')
+            self.initial['script'] = config.get('script')
+            self.initial['include_meta'] = config.get('include_meta')
+            custom_program = config.get('custom_program')
+            if custom_program:
+                self.initial['custom_program'] = [
+                    InitialFileStr(custom_program.get('executable', '').replace(self.executable_path, '')),
+                    custom_program.get('args'),
+                    custom_program.get('docker_image'),
+                    custom_program.get('run_in_docker', False),
+                ]
+            sql_config = config.get('sql_config')
+            if sql_config:
+                self.initial['sql_config'] = [
+                    sql_config.get('host'),
+                    sql_config.get('port'),
+                    sql_config.get('database'),
+                    sql_config.get('user'),
+                    sql_config.get('password'),
                 ]
 
     def clean(self):
         cleaned_data = super(SystemTaskForm, self).clean()
         if self.errors:
             return None
         parent = cleaned_data.get('parent')
@@ -82,34 +95,58 @@
         for field in required_fields:
             value = cleaned_data.pop(field, None) or config.pop(field, None)
             if not value:
                 self.add_error('name', '%s不能为空' % field)
                 break
             if field == 'queue':
                 config[field] = value.code
-            elif field == 'executable_file':
-                if isinstance(value, str):
-                    config[field] = value
-                    continue
+            elif field == 'sql_config':
+                host, port, database, user, password = value
+                if host:
+                    config[field] = {
+                        'host': host,
+                        'port': port,
+                        'database': database,
+                        'user': user,
+                        'password': password,
+                    }
+            elif field == 'custom_program':
+                bytesio, args, docker_image, run_in_docker = value
+                if not bytesio:
+                    custom_program = config.pop(field, None)
+                    if not custom_program or not custom_program.get('executable'):
+                        self.add_error('custom_program', '自定义程序不能为空')
+                    else:
+                        config[field] = {
+                            'executable': custom_program.get('executable'),
+                            'args': args,
+                            'docker_image': docker_image,
+                            'run_in_docker': run_in_docker,
+                        }
+                    break
                 max_size = parent.config.get('max_size', 5 * 1024 * 1024)
-                bytesio, args = value
+                bytesio, args, docker_image, run_in_docker = value
                 if bytesio.size > max_size:
-                    self.add_error('name', '文件大小不能超过%sM' % round(max_size / 1024 / 1024))
+                    self.add_error('custom_program', '文件大小不能超过%sM' % round(max_size / 1024 / 1024))
                     break
                 path = os.path.join(self.executable_path, get_md5(cleaned_data['name']))
                 if not os.path.exists(path):
                     os.makedirs(path)
                 file = os.path.join(path, 'main%s' % os.path.splitext(bytesio.name)[-1])
                 with open(file, 'wb') as f:
                     trunk = bytesio.read(bytesio.DEFAULT_CHUNK_SIZE)
                     while trunk:
                         f.write(trunk)
                         trunk = bytesio.read(bytesio.DEFAULT_CHUNK_SIZE)
-                config['executable_file'] = file
-                config['executable_args'] = args
+                config[field] = {
+                    'executable': file,
+                    'args': args,
+                    'docker_image': docker_image,
+                    'run_in_docker': run_in_docker,
+                }
             else:
                 config[field] = value
         return cleaned_data
 
     class Meta:
         model = models.SystemTask
         fields = '__all__'
```

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task/migrations/0001_initial.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import datetime
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 import django.utils.timezone
 import django_common_objects.fields
 import django_common_objects.models
-import django_common_task_system.fields
 import django_common_task_system.system_task.models
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
@@ -43,15 +42,15 @@
             name='SystemSchedule',
             fields=[
                 ('id', models.AutoField(primary_key=True, serialize=False)),
                 ('priority', models.IntegerField(default=0, verbose_name='优先级')),
                 ('next_schedule_time', models.DateTimeField(db_index=True, default=django.utils.timezone.now, verbose_name='下次运行时间')),
                 ('schedule_start_time', models.DateTimeField(default=datetime.datetime(1, 1, 1, 0, 0), verbose_name='开始时间')),
                 ('schedule_end_time', models.DateTimeField(default=datetime.datetime(9999, 12, 31, 23, 59, 59, 999999), verbose_name='结束时间')),
-                ('config', django_common_task_system.fields.ScheduleConfigField(default=dict, verbose_name='参数')),
+                ('config', django_common_objects.fields.ConfigField(default=dict, verbose_name='参数')),
                 ('status', django_common_objects.fields.CharField(choices=[('O', '开启'), ('C', '关闭'), ('D', '已完成'), ('T', '测试'), ('E', '调度错误')], default='O', max_length=1, verbose_name='状态')),
                 ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
                 ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
             ],
             options={
                 'verbose_name': '系统计划',
                 'verbose_name_plural': '系统计划',
```

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task/models.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task/models.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task/process.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task/process.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task/queue.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task/queue.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task/serializers.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task/urls.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task/urls.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task/views.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task/views.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task_execution/main.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task_execution/main.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task_execution/system_task_execution/executor.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task_execution/system_task_execution/executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     response = requests.get(url)
     if response.status_code == 200:
         result = response.json()
         result['next_schedule_time'] = datetime.strptime(result.pop('schedule_time'), '%Y-%m-%d %H:%M:%S')
         schedule = to_model(result, SystemSchedule)
         schedule.queue = result.pop('queue', None)
         schedule.generator = result.pop('generator', None)
+        schedule.last_log = result.pop('last_log', None)
         return schedule
 
 
 def get_system_schedule(url):
     while True:
         schedule = request_system_schedule(url)
         if schedule:
```

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task_execution/system_task_execution/executors/base.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task_execution/system_task_execution/executors/base.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.urls import reverse
 import requests
-from .base import BaseExecutor, EmptyResult
+from .base import BaseExecutor, EmptyResult, NoRetryException
 from django.db import connection
 from django_common_task_system.system_task.models import SystemScheduleLog, SystemSchedule
 from django_common_task_system.system_task.builtins import builtins
 from django_common_task_system import get_task_schedule_model, get_schedule_log_model
 from django_common_task_system.models import ScheduleConfig
 from .. import settings
 
@@ -27,60 +27,50 @@
 
 
 class SystemExceptionExecutor(BaseExecutor):
     name = builtins.tasks.system_exception_handling.name
     schedule_id = builtins.schedules.system_exception_handling.id
     schedule_model = SystemSchedule
     schedule_log_model = SystemScheduleLog
-    handle_url = 'system_schedule_put'
+    handle_url = 'system_schedule_retry'
 
     def execute(self):
         max_retry_times = self.schedule.task.config.get('max_retry_times', 5)
         max_fetch_num = self.schedule.task.config.get('max_fetch_num', 1000)
         # columns = get_schedule_table_columns(table=self.schedule_model._meta.db_table)
         next_schedule_time = ScheduleConfig(config=self.schedule.config).get_next_time(
             self.schedule.next_schedule_time)
         last_schedule_time = self.schedule.next_schedule_time - (next_schedule_time - self.schedule.next_schedule_time)
         command = '''
-            select * from (
-            select queue, schedule_id, schedule_time, count(*) as times, max(create_time) as lastest_time 
-            from %s where create_time > CURDATE() and status = 'F' 
-            GROUP BY queue, schedule_id, schedule_time order by queue, schedule_id, schedule_time
-            ) a where a.times < %s and a.lastest_time > '%s' limit %s
+            select queue, schedule_id, schedule_time, count(*) as times, 
+                max(id) as log_id, max(create_time) as lastest_time 
+            from %s where create_time > CURDATE() and status in ('F', 'T') 
+            GROUP BY queue, schedule_id, schedule_time 
+            having times < %s and lastest_time > '%s' 
+            order by queue, schedule_id, schedule_time limit %s
         ''' % (self.schedule_log_model._meta.db_table, max_retry_times, last_schedule_time, max_fetch_num,)
         with connection.cursor() as cursor:
             cursor.execute(command)
-            rows = list(cursor.fetchall())
+            log_ids = [x[4] for x in cursor.fetchall()]
         batch_num = 1000
         i = 0
-        batch = rows[:batch_num]
+        batch = log_ids[:batch_num]
         result = {}
         error = None
         while batch:
             path = reverse(self.handle_url)
-            ids, queues, times = [], [], []
-            for q, i, t, *_ in batch:
-                if i == self.schedule_id:
-                    continue
-                ids.append(str(i))
-                queues.append(q)
-                times.append(t.strftime('%Y-%m-%d %H:%M:%S'))
             url = settings.HOST + path
-            batch_result = requests.post(url, data={
-                'i': ','.join(ids),
-                'q': ','.join(queues),
-                't': ','.join(times)
-            }).json()
+            batch_result = requests.post(url, data={'log-ids': ','.join(batch)}).json()
             result[i] = batch_result
             if 'error' in batch_result:
                 error = batch_result['error']
             i += 1
-            batch = rows[i * batch_num: (i + 1) * batch_num]
+            batch = log_ids[i * batch_num: (i + 1) * batch_num]
         if error:
-            raise Exception(error)
+            raise NoRetryException(error)
         if not result:
             raise EmptyResult('no task need to handle')
         return result
 
 
 class ScheduleExceptionExecutor(SystemExceptionExecutor):
     name = builtins.tasks.task_exception_handling.name
```

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task_execution/system_task_execution/executors/strict_schedule.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task_execution/system_task_execution/executors/strict_schedule.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/system_task_execution/system_task_execution/utils.py` & `django-common-task-system-1.3.3/django_common_task_system/system_task_execution/system_task_execution/utils.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/templates/admin/system_schedule/change_list.html` & `django-common-task-system-1.3.3/django_common_task_system/templates/admin/system_schedule/change_list.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/templates/task_schedule/multi_day_select.html` & `django-common-task-system-1.3.3/django_common_task_system/templates/task_schedule/multi_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/templates/task_schedule/multi_month_day_select.html` & `django-common-task-system-1.3.3/django_common_task_system/templates/task_schedule/multi_month_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/templates/task_schedule/nlp_input.html` & `django-common-task-system-1.3.3/django_common_task_system/templates/task_schedule/nlp_input.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/templates/task_schedule/period_schedule.html` & `django-common-task-system-1.3.3/django_common_task_system/templates/task_schedule/period_schedule.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/urls.py` & `django-common-task-system-1.3.3/django_common_task_system/urls.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/utils/algorithm.py` & `django-common-task-system-1.3.3/django_common_task_system/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/utils/schedule_time.py` & `django-common-task-system-1.3.3/django_common_task_system/utils/schedule_time.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.0/django_common_task_system/views.py` & `django-common-task-system-1.3.3/django_common_task_system/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from django.db.models.signals import post_delete, post_save
 from django.dispatch import receiver
 from rest_framework import status
-from rest_framework.decorators import api_view
 from rest_framework.generics import CreateAPIView
 from rest_framework.request import Request
 from rest_framework.response import Response
 from rest_framework.views import APIView
 from rest_framework.viewsets import ModelViewSet
 from django.http.response import JsonResponse
 from django.conf import settings
 from . import serializers, get_task_model, get_schedule_log_model, get_task_schedule_model, get_task_schedule_serializer
 from .choices import TaskScheduleStatus
 from .models import TaskSchedule, TaskScheduleProducer, TaskScheduleQueue, \
-    ConsumerPermission, ExceptionReport, builtins, ScheduleConfig
+    ConsumerPermission, ExceptionReport, builtins, ScheduleConfig, UserModel, CommonCategory
 from django_common_objects.rest_view import UserListAPIView, UserRetrieveAPIView
 from django.views.decorators.csrf import csrf_exempt
 from queue import Empty
 from datetime import datetime
 from jionlp_time import parse_time
 from .utils.schedule_time import nlp_config_to_schedule_config
+from .utils.foreign_key import get_model_related
 from .models import system_initialize_signal, system_schedule_event
 from threading import Thread
 import time
 import traceback
 
 
 TaskModel = get_task_model()
@@ -55,16 +55,16 @@
             queryset = self.schedule_model.objects.filter(**producer.filters)
             if producer.lte_now:
                 queryset = queryset.filter(next_schedule_time__lte=now)
             for schedule in queryset:
                 try:
                     # 限制队列长度, 防止内存溢出
                     while queue.qsize() < max_queue_size and schedule.next_schedule_time <= now:
+                        schedule.queue = queue_instance.code
                         data = self.serializer(schedule).data
-                        data['queue'] = queue_instance.code
                         queue.put(data)
                         schedule.next_schedule_time = ScheduleConfig(config=schedule.config
                                                                      ).get_next_time(schedule.next_schedule_time)
                     schedule.save(update_fields=('next_schedule_time', ))
                 except Exception as e:
                     schedule.status = TaskScheduleStatus.ERROR.value
                     schedule.save(update_fields=('status',))
@@ -175,31 +175,35 @@
             schedule = cls.schedule_model.objects.get(id=pk)
             return Response(cls.serializer(schedule).data)
         except TaskSchedule.DoesNotExist:
             return Response({'error': 'schedule not found'}, status=status.HTTP_404_NOT_FOUND)
 
     @classmethod
     def retry(cls, request):
-        log_ids = request.GET.get('log-ids', None)
+        log_ids = request.GET.get('log-ids', None) or request.data.get('log-ids', None)
         if not log_ids:
             return JsonResponse({'error': 'log-ids不能为空'}, status=status.HTTP_400_BAD_REQUEST)
         try:
             log_ids = [int(i) for i in log_ids.split(',')]
-            assert len(log_ids) < 1000, 'log-ids不能超过1000个'
+            if len(log_ids) > 1000:
+                raise Exception('log-ids不能超过1000个')
         except Exception as e:
             return JsonResponse({'error': 'logs_ids参数错误: %s' % e}, status=status.HTTP_400_BAD_REQUEST)
         try:
             result = {x: 'no such log' for x in log_ids}
-            logs = cls.log_model.objects.filter(id__in=log_ids)
+            related = get_model_related(cls.log_model, excludes=[UserModel, CommonCategory])
+            logs = cls.log_model.objects.filter(id__in=log_ids).select_related(*related)
             for log in logs:
+                schedule = log.schedule
                 queue = cls.queues[log.queue].queue
-                log.schedule.next_schedule_time = log.schedule_time
-                log.schedule.generator = 'retry'
-                data = cls.serializer(log.schedule).data
-                data['queue'] = log.queue
+                schedule.next_schedule_time = log.schedule_time
+                schedule.generator = 'retry'
+                schedule.last_log = log.result
+                schedule.queue = log.queue
+                data = cls.serializer(schedule).data
                 queue.put(data)
                 result[log.id] = log.queue
             return JsonResponse(result)
         except Exception as e:
             return JsonResponse({'error': '重试失败: %s' % e}, status=status.HTTP_400_BAD_REQUEST)
 
     @classmethod
@@ -241,16 +245,16 @@
                 schedule = schedule_mapping.get(i, None)
                 if schedule is None:
                     queue_result[i] = 'no such schedule: %s' % i
                     continue
                 schedule_result = queue_result.setdefault(i, [])
                 schedule.next_schedule_time = t
                 schedule.generator = 'put'
+                schedule.queue = q
                 data = cls.serializer(schedule).data
-                data['queue'] = q
                 queue_instance.queue.put(data)
                 schedule_result.append(t.strftime('%Y-%m-%d %H:%M:%S'))
             return JsonResponse(result)
         except Exception as e:
             return JsonResponse({'error': '添加到队列失败: %s' % e}, status=status.HTTP_400_BAD_REQUEST)
 
     @classmethod
```

### Comparing `django-common-task-system-1.3.0/django_common_task_system.egg-info/SOURCES.txt` & `django-common-task-system-1.3.3/django_common_task_system.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE
 MANIFEST.in
 README.md
+deploy.sh
 setup.py
 django_common_task_system/__init__.py
 django_common_task_system/admin.py
 django_common_task_system/apps.py
 django_common_task_system/choices.py
-django_common_task_system/fields.py
 django_common_task_system/forms.py
 django_common_task_system/mixin.py
 django_common_task_system/models.py
 django_common_task_system/permissions.py
 django_common_task_system/serializers.py
 django_common_task_system/tests.py
 django_common_task_system/urls.py
@@ -30,14 +30,17 @@
 django_common_task_system/migrations/0008_taskschedule_strict_mode.py
 django_common_task_system/migrations/__init__.py
 django_common_task_system/static/common_task_system/css/calendar.css
 django_common_task_system/static/common_task_system/css/task_schedule_admin.css
 django_common_task_system/static/common_task_system/js/calendar.js
 django_common_task_system/static/common_task_system/js/task_schedule_admin.js
 django_common_task_system/static/common_task_system/js/task_type_admin.js
+django_common_task_system/static/custom_programs/python_test.py
+django_common_task_system/static/custom_programs/shell_test.sh
+django_common_task_system/static/custom_programs/zip_test.zip
 django_common_task_system/system_task/__init__.py
 django_common_task_system/system_task/admin.py
 django_common_task_system/system_task/apps.py
 django_common_task_system/system_task/builtins.py
 django_common_task_system/system_task/choices.py
 django_common_task_system/system_task/forms.py
 django_common_task_system/system_task/models.py
@@ -66,20 +69,28 @@
 django_common_task_system/system_task_execution/system_task_execution/executors/base.py
 django_common_task_system/system_task_execution/system_task_execution/executors/custom_program.py
 django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
 django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
 django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
 django_common_task_system/system_task_execution/system_task_execution/executors/strict_schedule.py
 django_common_task_system/templates/admin/system_schedule/change_list.html
+django_common_task_system/templates/task_schedule/custom_program.html
 django_common_task_system/templates/task_schedule/datetime_range.html
-django_common_task_system/templates/task_schedule/executable_file.html
 django_common_task_system/templates/task_schedule/multi_day_select.html
 django_common_task_system/templates/task_schedule/multi_month_day_select.html
 django_common_task_system/templates/task_schedule/nlp_input.html
 django_common_task_system/templates/task_schedule/period.html
 django_common_task_system/templates/task_schedule/period_schedule.html
+django_common_task_system/templates/task_schedule/sql_config.html
 django_common_task_system/utils/__init__.py
 django_common_task_system/utils/algorithm.py
 django_common_task_system/utils/cron_utils.py
 django_common_task_system/utils/foreign_key.py
 django_common_task_system/utils/schedule_time.py
+django_common_task_system_server/__init__.py
+django_common_task_system_server/manage.py
+django_common_task_system_server/server/__init__.py
+django_common_task_system_server/server/asgi.py
+django_common_task_system_server/server/settings.py
+django_common_task_system_server/server/urls.py
+django_common_task_system_server/server/wsgi.py
 tests/__init__.py
```

### Comparing `django-common-task-system-1.3.0/setup.py` & `django-common-task-system-1.3.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-common-task-system',
-    packages=find_packages(exclude=['local_tests']),
-    version='1.3.0',
+    packages=find_packages(exclude=['local_tests', 'tests']),
+    version='1.3.3',
     install_requires=[
-        "django-common-objects>=1.0.6",
+        "django-common-objects>=1.0.7",
         "django>=3.2.18",
         "croniter>=1.3.8",
         "djangorestframework>=3.14.0",
         "PyMySQL>=1.0.2",
         "jionlp-time>=1.0.0",
     ],
     include_package_data=True,
     author='cone387',
     maintainer_email='1183008540@qq.com',
     license='MIT',
-    url='https://github.com/cone387/CommonTaskSystemServer',
+    url='https://github.com/cone387/DjangoCommonTaskSystem.git',
     python_requires='>=3.7, <4',
-)
+)
```

