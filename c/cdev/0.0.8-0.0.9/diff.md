# Comparing `tmp/cdev-0.0.8.tar.gz` & `tmp/cdev-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cdev-0.0.8.tar", last modified: Tue Apr  5 18:04:42 2022, max compression
+gzip compressed data, was "dist/cdev-0.0.9.tar", last modified: Tue Jun 21 00:32:47 2022, max compression
```

## Comparing `cdev-0.0.8.tar` & `cdev-0.0.9.tar`

### file list

```diff
@@ -1,238 +1,281 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      141 2022-03-09 16:24:04.000000 cdev-0.0.8/MANIFEST.in
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6203 2022-04-05 18:04:42.000000 cdev-0.0.8/PKG-INFO
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      577 2022-01-24 04:34:41.000000 cdev-0.0.8/cdev/__init__.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/cli/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       75 2022-01-24 04:34:41.000000 cdev-0.0.8/cdev/cli/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7975 2022-03-14 03:17:55.000000 cdev-0.0.8/cdev/cli/__main__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      237 2022-02-17 16:40:28.000000 cdev-0.0.8/cdev/cli/logger.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/commands/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2021-10-26 18:16:18.000000 cdev-0.0.8/cdev/commands/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      717 2022-03-14 03:17:55.000000 cdev-0.0.8/cdev/commands/cloud_output.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      560 2022-02-17 16:40:28.000000 cdev-0.0.8/cdev/commands/deploy.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1221 2022-02-17 19:53:39.000000 cdev-0.0.8/cdev/commands/destroy.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3868 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/commands/environment.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6149 2022-04-04 23:54:54.000000 cdev-0.0.8/cdev/commands/initializer.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7811 2022-02-17 16:40:28.000000 cdev-0.0.8/cdev/commands/local_development.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      727 2022-02-17 16:40:28.000000 cdev-0.0.8/cdev/commands/plan.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      563 2022-02-17 16:40:28.000000 cdev-0.0.8/cdev/commands/run.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/constructs/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      196 2022-01-24 04:34:41.000000 cdev-0.0.8/cdev/constructs/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1017 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/constructs/environment.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    14821 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/constructs/project.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/default/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       71 2022-01-24 04:34:41.000000 cdev-0.0.8/cdev/default/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      103 2022-01-26 01:54:28.000000 cdev-0.0.8/cdev/default/cloudmapper.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      102 2022-01-26 01:56:18.000000 cdev-0.0.8/cdev/default/components.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      952 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/default/environment.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      441 2022-02-17 16:40:28.000000 cdev-0.0.8/cdev/default/output_manager.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11194 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/default/project.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/packages/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       29 2022-02-17 16:40:28.000000 cdev-0.0.8/cdev/project_templates/packages/requirements.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/packages/src/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       20 2022-02-17 16:40:28.000000 cdev-0.0.8/cdev/project_templates/packages/src/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      415 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/project_templates/packages/src/cdev_project.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/packages/src/packages/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/project_templates/packages/src/packages/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1142 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/project_templates/packages/src/packages/resources.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       98 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/project_templates/packages/src/packages/utils.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/power_tools/
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/power_tools/src/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-03-21 20:02:06.000000 cdev-0.0.8/cdev/project_templates/power_tools/src/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      409 2022-03-21 20:02:06.000000 cdev-0.0.8/cdev/project_templates/power_tools/src/cdev_project.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/power_tools/src/examples/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      385 2022-03-21 20:02:06.000000 cdev-0.0.8/cdev/project_templates/power_tools/src/examples/config.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      649 2022-03-21 20:02:06.000000 cdev-0.0.8/cdev/project_templates/power_tools/src/examples/dataclass_example.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      464 2022-03-21 20:02:06.000000 cdev-0.0.8/cdev/project_templates/power_tools/src/examples/logging_example.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      494 2022-03-21 20:02:06.000000 cdev-0.0.8/cdev/project_templates/power_tools/src/examples/metrics_example.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      618 2022-03-21 20:02:06.000000 cdev-0.0.8/cdev/project_templates/power_tools/src/examples/middleware_example.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      560 2022-03-21 20:02:06.000000 cdev-0.0.8/cdev/project_templates/power_tools/src/examples/tracer_example.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/quick_start/
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/quick_start/src/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/project_templates/quick_start/src/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      417 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/project_templates/quick_start/src/cdev_project.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/quick_start/src/hello_world/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      704 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/project_templates/quick_start/src/hello_world/resources.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/quick_start_twilio/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       50 2022-04-04 23:54:54.000000 cdev-0.0.8/cdev/project_templates/quick_start_twilio/requirements.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/quick_start_twilio/src/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-04-04 23:54:54.000000 cdev-0.0.8/cdev/project_templates/quick_start_twilio/src/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      406 2022-04-04 23:54:54.000000 cdev-0.0.8/cdev/project_templates/quick_start_twilio/src/cdev_project.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/quick_start_twilio/src/link_bot/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      294 2022-04-04 23:54:54.000000 cdev-0.0.8/cdev/project_templates/quick_start_twilio/src/link_bot/api.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      561 2022-04-04 23:54:54.000000 cdev-0.0.8/cdev/project_templates/quick_start_twilio/src/link_bot/handlers.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/resources_test/
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/resources_test/src/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/project_templates/resources_test/src/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      419 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/project_templates/resources_test/src/cdev_project.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/resources_test/src/resource_test/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/project_templates/resources_test/src/resource_test/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1123 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/project_templates/resources_test/src/resource_test/resources.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/slack_bot/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        9 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/project_templates/slack_bot/requirements.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/slack_bot/src/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/project_templates/slack_bot/src/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      409 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/project_templates/slack_bot/src/cdev_project.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      144 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/project_templates/slack_bot/src/project_settings.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/slack_bot/src/slack_bot/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/project_templates/slack_bot/src/slack_bot/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1986 2022-03-09 15:51:31.000000 cdev-0.0.8/cdev/project_templates/slack_bot/src/slack_bot/resources.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/user_auth/
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/user_auth/src/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-03-17 02:52:01.000000 cdev-0.0.8/cdev/project_templates/user_auth/src/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      408 2022-03-17 02:52:39.000000 cdev-0.0.8/cdev/project_templates/user_auth/src/cdev_project.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/user_auth/src/content/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       76 2022-03-17 19:34:45.000000 cdev-0.0.8/cdev/project_templates/user_auth/src/content/auth_config.json
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/user_auth/src/content/css/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2022-03-17 19:34:24.000000 cdev-0.0.8/cdev/project_templates/user_auth/src/content/css/main.css
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1282 2022-03-17 19:34:24.000000 cdev-0.0.8/cdev/project_templates/user_auth/src/content/index.html
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/user_auth/src/content/js/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3106 2022-03-17 19:34:24.000000 cdev-0.0.8/cdev/project_templates/user_auth/src/content/js/app.js
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/project_templates/user_auth/src/user_auth/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      810 2022-03-17 19:43:01.000000 cdev-0.0.8/cdev/project_templates/user_auth/src/user_auth/resources.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/resources/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      147 2022-02-17 16:40:28.000000 cdev-0.0.8/cdev/resources/__init__.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/resources/simple/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2021-10-26 18:16:18.000000 cdev-0.0.8/cdev/resources/simple/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       48 2022-02-17 16:40:28.000000 cdev-0.0.8/cdev/resources/simple/api.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       48 2022-02-17 16:40:28.000000 cdev-0.0.8/cdev/resources/simple/iam.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       57 2022-02-17 16:40:28.000000 cdev-0.0.8/cdev/resources/simple/object_store.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       50 2022-02-17 16:40:28.000000 cdev-0.0.8/cdev/resources/simple/queue.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       58 2022-02-17 16:40:28.000000 cdev-0.0.8/cdev/resources/simple/relational_db.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       56 2022-02-17 16:40:28.000000 cdev-0.0.8/cdev/resources/simple/static_site.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       50 2022-02-17 16:40:28.000000 cdev-0.0.8/cdev/resources/simple/table.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       50 2022-02-17 16:40:28.000000 cdev-0.0.8/cdev/resources/simple/topic.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       52 2022-02-17 16:40:28.000000 cdev-0.0.8/cdev/resources/simple/xlambda.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev/scripts/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)      103 2021-08-23 04:54:04.000000 cdev-0.0.8/cdev/scripts/cdev
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6203 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7021 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      267 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       28 2022-04-05 18:04:42.000000 cdev-0.0.8/cdev.egg-info/top_level.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/core/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-01-24 04:34:41.000000 cdev-0.0.8/core/__init__.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/core/cli/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       76 2022-02-17 16:40:28.000000 cdev-0.0.8/core/cli/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4097 2022-02-17 16:40:28.000000 cdev-0.0.8/core/cli/__main__.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/core/commands/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       64 2022-02-17 16:40:28.000000 cdev-0.0.8/core/commands/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1288 2022-03-14 03:17:55.000000 cdev-0.0.8/core/commands/cloud_output.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      338 2022-02-17 16:40:28.000000 cdev-0.0.8/core/commands/create_resource_state.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1171 2022-02-17 16:40:28.000000 cdev-0.0.8/core/commands/create_workspace.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1024 2022-02-17 16:40:28.000000 cdev-0.0.8/core/commands/deploy_differences.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1654 2022-02-17 16:40:28.000000 cdev-0.0.8/core/commands/execute_frontend.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      678 2022-02-17 16:40:28.000000 cdev-0.0.8/core/commands/initialize_workspace.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      979 2022-02-17 16:40:28.000000 cdev-0.0.8/core/commands/run.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/core/constructs/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       58 2022-02-17 16:40:28.000000 cdev-0.0.8/core/constructs/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    19328 2022-02-17 16:40:28.000000 cdev-0.0.8/core/constructs/backend.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      701 2022-01-24 04:34:41.000000 cdev-0.0.8/core/constructs/backend_exceptions.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    43407 2022-02-17 16:40:28.000000 cdev-0.0.8/core/constructs/cloud_output.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7495 2022-02-17 16:40:28.000000 cdev-0.0.8/core/constructs/commands.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4472 2022-02-17 16:40:28.000000 cdev-0.0.8/core/constructs/components.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      981 2022-02-17 16:40:28.000000 cdev-0.0.8/core/constructs/mapper.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3771 2022-02-17 16:40:28.000000 cdev-0.0.8/core/constructs/models.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10530 2022-02-17 19:53:39.000000 cdev-0.0.8/core/constructs/output_manager.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10397 2022-02-23 21:07:42.000000 cdev-0.0.8/core/constructs/resource.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2234 2022-02-17 16:40:28.000000 cdev-0.0.8/core/constructs/resource_state.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2271 2022-03-09 15:51:31.000000 cdev-0.0.8/core/constructs/settings.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      411 2022-02-17 16:40:28.000000 cdev-0.0.8/core/constructs/types.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    30592 2022-02-17 16:40:28.000000 cdev-0.0.8/core/constructs/workspace.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/core/default/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-01-24 04:34:41.000000 cdev-0.0.8/core/default/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    46842 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/backend.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2497 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/cloudmapper.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/core/default/commands/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/commands/__init__.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/core/default/commands/bucket/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      331 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/commands/bucket/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5059 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/commands/bucket/cp.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2238 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/commands/bucket/sync.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1839 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/commands/bucket/utils.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/core/default/commands/function/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      319 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/commands/function/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2698 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/commands/function/execute.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4594 2022-03-30 18:55:56.000000 cdev-0.0.8/core/default/commands/function/logs.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      570 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/commands/function/utils.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/core/default/commands/relationaldb/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      249 2022-03-13 18:43:00.000000 cdev-0.0.8/core/default/commands/relationaldb/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3977 2022-03-13 18:43:00.000000 cdev-0.0.8/core/default/commands/relationaldb/shell.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1400 2022-03-14 18:13:10.000000 cdev-0.0.8/core/default/commands/relationaldb/utils.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/core/default/commands/static_site/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      271 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/commands/static_site/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3481 2022-03-17 14:53:51.000000 cdev-0.0.8/core/default/commands/static_site/sync.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1106 2022-03-17 02:28:25.000000 cdev-0.0.8/core/default/commands/static_site/utils.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/core/default/commands/table/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      283 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/commands/table/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2559 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/commands/table/clear_table.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3545 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/commands/table/put_items.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3174 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/commands/table/utils.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1385 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/components.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/core/default/mappers/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-01-24 04:34:41.000000 cdev-0.0.8/core/default/mappers/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3220 2022-02-23 21:08:09.000000 cdev-0.0.8/core/default/mappers/aws_client.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/core/default/mappers/simple/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-01-24 04:34:41.000000 cdev-0.0.8/core/default/mappers/simple/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    21059 2022-03-09 15:51:31.000000 cdev-0.0.8/core/default/mappers/simple/api_deployer.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7210 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/mappers/simple/bucket_deployer.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3542 2022-03-22 05:08:52.000000 cdev-0.0.8/core/default/mappers/simple/dynamodb_deployer.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11467 2022-03-29 17:00:08.000000 cdev-0.0.8/core/default/mappers/simple/event_deployer.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    21110 2022-03-09 15:51:31.000000 cdev-0.0.8/core/default/mappers/simple/lambda_deployer.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3385 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/mappers/simple/queue_deployer.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8245 2022-03-13 19:40:50.000000 cdev-0.0.8/core/default/mappers/simple/relational_db_deployer.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4258 2022-02-17 19:20:41.000000 cdev-0.0.8/core/default/mappers/simple/role_deployer.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11473 2022-03-17 02:21:02.000000 cdev-0.0.8/core/default/mappers/simple/static_site_deployer.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3411 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/mappers/simple/topic_deployer.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/core/default/resources/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       64 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/resources/__init__.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/core/default/resources/simple/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/resources/simple/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    12194 2022-03-29 17:00:08.000000 cdev-0.0.8/core/default/resources/simple/api.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      650 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/resources/simple/events.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2680 2022-03-13 02:04:13.000000 cdev-0.0.8/core/default/resources/simple/iam.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6116 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/resources/simple/object_store.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7124 2022-03-22 05:08:52.000000 cdev-0.0.8/core/default/resources/simple/queue.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8810 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/resources/simple/relational_db.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7660 2022-03-09 15:51:31.000000 cdev-0.0.8/core/default/resources/simple/static_site.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    14739 2022-03-22 05:08:52.000000 cdev-0.0.8/core/default/resources/simple/table.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5352 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/resources/simple/topic.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    12431 2022-02-17 16:40:28.000000 cdev-0.0.8/core/default/resources/simple/xlambda.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10658 2022-03-14 03:17:55.000000 cdev-0.0.8/core/default/workspace.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/core/scripts/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)      104 2022-01-24 04:34:41.000000 cdev-0.0.8/core/scripts/cdev_core
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/core/utils/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-01-24 04:34:41.000000 cdev-0.0.8/core/utils/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5767 2022-03-14 03:17:55.000000 cdev-0.0.8/core/utils/command_finder.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      962 2022-02-17 16:40:28.000000 cdev-0.0.8/core/utils/exceptions.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7678 2022-02-17 16:40:28.000000 cdev-0.0.8/core/utils/file_manager.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/core/utils/fs_manager/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       81 2022-01-24 04:34:41.000000 cdev-0.0.8/core/utils/fs_manager/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    13998 2022-02-17 16:40:28.000000 cdev-0.0.8/core/utils/fs_manager/docker_package_builder.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10836 2022-02-17 16:40:28.000000 cdev-0.0.8/core/utils/fs_manager/external_dependencies_index.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11136 2022-03-21 15:10:14.000000 cdev-0.0.8/core/utils/fs_manager/finder.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    27094 2022-03-13 02:04:13.000000 cdev-0.0.8/core/utils/fs_manager/package_mananger.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/core/utils/fs_manager/standard_library_names/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1663 2022-01-24 04:34:41.000000 cdev-0.0.8/core/utils/fs_manager/standard_library_names/python_3_6
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1668 2022-01-24 04:34:41.000000 cdev-0.0.8/core/utils/fs_manager/standard_library_names/python_3_7
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1672 2022-01-24 04:34:41.000000 cdev-0.0.8/core/utils/fs_manager/standard_library_names/python_3_8
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1672 2022-02-17 16:40:28.000000 cdev-0.0.8/core/utils/fs_manager/standard_library_names/python_3_9
--rw-r--r--   0 daniel    (1000) daniel    (1000)    17177 2022-02-17 16:40:28.000000 cdev-0.0.8/core/utils/fs_manager/utils.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    27699 2022-02-17 16:40:28.000000 cdev-0.0.8/core/utils/fs_manager/writer.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2700 2022-02-17 16:40:28.000000 cdev-0.0.8/core/utils/hasher.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8375 2022-02-17 16:40:28.000000 cdev-0.0.8/core/utils/logger.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2467 2022-02-17 16:40:28.000000 cdev-0.0.8/core/utils/module_loader.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5367 2022-03-17 02:19:07.000000 cdev-0.0.8/core/utils/paths.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1873 2022-03-09 15:51:27.000000 cdev-0.0.8/core/utils/platforms.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    15559 2022-02-17 16:40:28.000000 cdev-0.0.8/core/utils/topological_helper.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-04-05 18:04:42.000000 cdev-0.0.8/serverless_parser/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      535 2022-01-24 04:34:41.000000 cdev-0.0.8/serverless_parser/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1106 2022-01-24 04:34:41.000000 cdev-0.0.8/serverless_parser/parser.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      633 2022-01-24 04:34:41.000000 cdev-0.0.8/serverless_parser/parser_exceptions.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8829 2022-03-09 15:51:31.000000 cdev-0.0.8/serverless_parser/parser_objects.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    23492 2022-03-22 00:56:58.000000 cdev-0.0.8/serverless_parser/parser_utils.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2022-04-05 18:04:42.000000 cdev-0.0.8/setup.cfg
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1240 2022-04-05 18:04:08.000000 cdev-0.0.8/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      142 2022-06-04 19:48:48.000000 cdev-0.0.9/MANIFEST.in
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7563 2022-06-21 00:32:47.000000 cdev-0.0.9/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5943 2022-06-21 00:22:59.000000 cdev-0.0.9/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      575 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/__init__.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/cli/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       75 2022-01-24 04:34:41.000000 cdev-0.0.9/cdev/cli/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    10408 2022-06-21 00:22:59.000000 cdev-0.0.9/cdev/cli/__main__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      202 2022-06-21 00:22:59.000000 cdev-0.0.9/cdev/cli/logger.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/commands/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/commands/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      722 2022-06-21 00:22:59.000000 cdev-0.0.9/cdev/commands/cloud_output.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      575 2022-06-21 00:22:59.000000 cdev-0.0.9/cdev/commands/deploy.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1270 2022-06-21 00:22:59.000000 cdev-0.0.9/cdev/commands/destroy.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6411 2022-06-21 00:22:59.000000 cdev-0.0.9/cdev/commands/environment.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7616 2022-06-21 00:22:59.000000 cdev-0.0.9/cdev/commands/local_development.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      724 2022-06-21 00:22:59.000000 cdev-0.0.9/cdev/commands/plan.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7919 2022-06-21 00:22:59.000000 cdev-0.0.9/cdev/commands/project_initializer.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      574 2022-06-21 00:22:59.000000 cdev-0.0.9/cdev/commands/run.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      559 2022-06-21 00:22:59.000000 cdev-0.0.9/cdev/commands/sync.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/constructs/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      196 2022-01-24 04:34:41.000000 cdev-0.0.9/cdev/constructs/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1238 2022-06-21 00:22:59.000000 cdev-0.0.9/cdev/constructs/environment.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    13895 2022-06-21 00:22:59.000000 cdev-0.0.9/cdev/constructs/project.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/default/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       71 2022-01-24 04:34:41.000000 cdev-0.0.9/cdev/default/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      104 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/default/cloudmapper.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      103 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/default/components.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      740 2022-06-21 00:22:59.000000 cdev-0.0.9/cdev/default/environment.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      453 2022-06-21 00:22:59.000000 cdev-0.0.9/cdev/default/output_manager.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    11988 2022-06-21 00:22:59.000000 cdev-0.0.9/cdev/default/project.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/packages/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       30 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/packages/requirements.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/packages/src/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/packages/src/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      404 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/packages/src/cdev_project.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/packages/src/packages/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-03-09 15:51:31.000000 cdev-0.0.9/cdev/project_templates/packages/src/packages/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1054 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/packages/src/packages/resources.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       86 2022-06-21 00:22:59.000000 cdev-0.0.9/cdev/project_templates/packages/src/packages/utils.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/power_tools/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/power_tools/src/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-03-21 20:02:06.000000 cdev-0.0.9/cdev/project_templates/power_tools/src/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      402 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/power_tools/src/cdev_project.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/power_tools/src/examples/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      387 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/power_tools/src/examples/config.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      663 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/power_tools/src/examples/dataclass_example.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      452 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/power_tools/src/examples/logging_example.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      494 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/power_tools/src/examples/metrics_example.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      619 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/power_tools/src/examples/middleware_example.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      566 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/power_tools/src/examples/tracer_example.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/quick_start/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/quick_start/src/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-03-09 15:51:31.000000 cdev-0.0.9/cdev/project_templates/quick_start/src/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      410 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/quick_start/src/cdev_project.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/quick_start/src/hello_world/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:22:59.000000 cdev-0.0.9/cdev/project_templates/quick_start/src/hello_world/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      681 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/quick_start/src/hello_world/resources.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/quick_start_twilio/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       51 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/quick_start_twilio/requirements.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/quick_start_twilio/src/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-04-04 23:54:54.000000 cdev-0.0.9/cdev/project_templates/quick_start_twilio/src/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      399 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/quick_start_twilio/src/cdev_project.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/quick_start_twilio/src/link_bot/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      293 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/quick_start_twilio/src/link_bot/api.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      565 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/quick_start_twilio/src/link_bot/handlers.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/resources_test/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/resources_test/src/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-03-09 15:51:31.000000 cdev-0.0.9/cdev/project_templates/resources_test/src/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      407 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/resources_test/src/cdev_project.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/resources_test/src/resource_test/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-03-09 15:51:31.000000 cdev-0.0.9/cdev/project_templates/resources_test/src/resource_test/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1160 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/resources_test/src/resource_test/resources.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/slack_bot/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       10 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/slack_bot/requirements.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/slack_bot/src/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-03-09 15:51:31.000000 cdev-0.0.9/cdev/project_templates/slack_bot/src/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      401 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/slack_bot/src/cdev_project.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      145 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/slack_bot/src/project_settings.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/slack_bot/src/slack_bot/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-03-09 15:51:31.000000 cdev-0.0.9/cdev/project_templates/slack_bot/src/slack_bot/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1928 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/slack_bot/src/slack_bot/resources.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/user_auth/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/user_auth/src/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-03-17 02:52:01.000000 cdev-0.0.9/cdev/project_templates/user_auth/src/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      401 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/user_auth/src/cdev_project.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/user_auth/src/content/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       77 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/user_auth/src/content/auth_config.json
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/user_auth/src/content/css/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       33 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/user_auth/src/content/css/main.css
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1283 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/user_auth/src/content/index.html
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/user_auth/src/content/js/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3091 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/user_auth/src/content/js/app.js
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/project_templates/user_auth/src/user_auth/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      788 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/project_templates/user_auth/src/user_auth/resources.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/resources/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      147 2022-06-04 19:48:48.000000 cdev-0.0.9/cdev/resources/__init__.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/resources/simple/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2021-10-26 18:16:18.000000 cdev-0.0.9/cdev/resources/simple/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       48 2022-02-17 16:40:28.000000 cdev-0.0.9/cdev/resources/simple/api.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       48 2022-02-17 16:40:28.000000 cdev-0.0.9/cdev/resources/simple/iam.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       57 2022-02-17 16:40:28.000000 cdev-0.0.9/cdev/resources/simple/object_store.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       50 2022-02-17 16:40:28.000000 cdev-0.0.9/cdev/resources/simple/queue.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       58 2022-02-17 16:40:28.000000 cdev-0.0.9/cdev/resources/simple/relational_db.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       56 2022-02-17 16:40:28.000000 cdev-0.0.9/cdev/resources/simple/static_site.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       50 2022-02-17 16:40:28.000000 cdev-0.0.9/cdev/resources/simple/table.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       50 2022-02-17 16:40:28.000000 cdev-0.0.9/cdev/resources/simple/topic.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       52 2022-02-17 16:40:28.000000 cdev-0.0.9/cdev/resources/simple/xlambda.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev/scripts/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)      105 2022-06-21 00:22:59.000000 cdev-0.0.9/cdev/scripts/cdev
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7563 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8248 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      105 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       34 2022-06-21 00:32:47.000000 cdev-0.0.9/cdev.egg-info/top_level.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/core/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-01-24 04:34:41.000000 cdev-0.0.9/core/__init__.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/core/cli/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       76 2022-02-17 16:40:28.000000 cdev-0.0.9/core/cli/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4158 2022-06-21 00:22:59.000000 cdev-0.0.9/core/cli/__main__.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/core/commands/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       64 2022-02-17 16:40:28.000000 cdev-0.0.9/core/commands/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1784 2022-06-21 00:22:59.000000 cdev-0.0.9/core/commands/cloud_output.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      337 2022-06-21 00:22:59.000000 cdev-0.0.9/core/commands/create_resource_state.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1180 2022-06-21 00:22:59.000000 cdev-0.0.9/core/commands/create_workspace.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1473 2022-06-21 00:22:59.000000 cdev-0.0.9/core/commands/deploy_differences.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2291 2022-06-21 00:22:59.000000 cdev-0.0.9/core/commands/execute_frontend.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      551 2022-06-21 00:22:59.000000 cdev-0.0.9/core/commands/initialize_workspace.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1191 2022-06-21 00:22:59.000000 cdev-0.0.9/core/commands/run.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1069 2022-06-21 00:22:59.000000 cdev-0.0.9/core/commands/sync.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/core/constructs/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       58 2022-02-17 16:40:28.000000 cdev-0.0.9/core/constructs/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    19442 2022-06-21 00:22:59.000000 cdev-0.0.9/core/constructs/backend.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      701 2022-06-21 00:14:55.000000 cdev-0.0.9/core/constructs/backend_exceptions.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    39599 2022-06-21 00:22:59.000000 cdev-0.0.9/core/constructs/cloud_output.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8459 2022-06-21 00:22:59.000000 cdev-0.0.9/core/constructs/commands.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4461 2022-06-21 00:22:59.000000 cdev-0.0.9/core/constructs/components.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1939 2022-06-21 00:22:59.000000 cdev-0.0.9/core/constructs/mapper.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3935 2022-06-04 19:48:48.000000 cdev-0.0.9/core/constructs/models.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    14688 2022-06-21 00:22:59.000000 cdev-0.0.9/core/constructs/output_manager.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    10446 2022-06-21 00:22:59.000000 cdev-0.0.9/core/constructs/resource.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2223 2022-06-04 19:48:48.000000 cdev-0.0.9/core/constructs/resource_state.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2340 2022-06-21 00:22:59.000000 cdev-0.0.9/core/constructs/settings.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      486 2022-06-21 00:22:59.000000 cdev-0.0.9/core/constructs/types.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    37746 2022-06-21 00:22:59.000000 cdev-0.0.9/core/constructs/workspace.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3191 2022-06-21 00:22:59.000000 cdev-0.0.9/core/constructs/workspace_watcher.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/core/default/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-01-24 04:34:41.000000 cdev-0.0.9/core/default/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    48958 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/backend.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2662 2022-06-04 19:48:48.000000 cdev-0.0.9/core/default/cloudmapper.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/core/default/commands/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-02-17 16:40:28.000000 cdev-0.0.9/core/default/commands/__init__.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/core/default/commands/bucket/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      331 2022-02-17 16:40:28.000000 cdev-0.0.9/core/default/commands/bucket/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5074 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/commands/bucket/cp.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2174 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/commands/bucket/sync.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1785 2022-06-04 19:48:48.000000 cdev-0.0.9/core/default/commands/bucket/utils.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/core/default/commands/function/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      319 2022-02-17 16:40:28.000000 cdev-0.0.9/core/default/commands/function/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2773 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/commands/function/execute.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8231 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/commands/function/logs.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      611 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/commands/function/utils.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/core/default/commands/relationaldb/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      250 2022-06-04 19:48:48.000000 cdev-0.0.9/core/default/commands/relationaldb/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6453 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/commands/relationaldb/shell.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1437 2022-06-04 19:48:48.000000 cdev-0.0.9/core/default/commands/relationaldb/utils.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/core/default/commands/static_site/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      271 2022-02-17 16:40:28.000000 cdev-0.0.9/core/default/commands/static_site/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6234 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/commands/static_site/sync.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1085 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/commands/static_site/utils.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3007 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/commands/static_site/watcher.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/core/default/commands/table/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      283 2022-02-17 16:40:28.000000 cdev-0.0.9/core/default/commands/table/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2396 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/commands/table/clear_table.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3406 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/commands/table/put_items.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3135 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/commands/table/utils.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1331 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/components.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/core/default/mappers/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-01-24 04:34:41.000000 cdev-0.0.9/core/default/mappers/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2915 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/mappers/aws_client.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/core/default/mappers/simple/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-01-24 04:34:41.000000 cdev-0.0.9/core/default/mappers/simple/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    21472 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/mappers/simple/api_deployer.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8033 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/mappers/simple/bucket_deployer.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3480 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/mappers/simple/dynamodb_deployer.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    11151 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/mappers/simple/event_deployer.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    27138 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/mappers/simple/lambda_deployer.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3246 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/mappers/simple/queue_deployer.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8162 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/mappers/simple/relational_db_deployer.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4085 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/mappers/simple/role_deployer.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    11228 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/mappers/simple/static_site_deployer.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3342 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/mappers/simple/topic_deployer.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/core/default/resources/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       64 2022-02-17 16:40:28.000000 cdev-0.0.9/core/default/resources/__init__.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/core/default/resources/simple/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-02-17 16:40:28.000000 cdev-0.0.9/core/default/resources/simple/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    12271 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/resources/simple/api.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      656 2022-06-04 19:48:48.000000 cdev-0.0.9/core/default/resources/simple/events.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2726 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/resources/simple/iam.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6107 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/resources/simple/object_store.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7178 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/resources/simple/queue.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8884 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/resources/simple/relational_db.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7673 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/resources/simple/static_site.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    14713 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/resources/simple/table.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5379 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/resources/simple/topic.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    14951 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/resources/simple/xlambda.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    10064 2022-06-21 00:22:59.000000 cdev-0.0.9/core/default/workspace.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/core/scripts/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)      104 2022-05-29 03:30:14.000000 cdev-0.0.9/core/scripts/cdev_core
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/core/utils/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-01-24 04:34:41.000000 cdev-0.0.9/core/utils/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2638 2022-06-21 00:22:59.000000 cdev-0.0.9/core/utils/cache.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6764 2022-06-21 00:22:59.000000 cdev-0.0.9/core/utils/command_finder.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      961 2022-06-21 00:14:55.000000 cdev-0.0.9/core/utils/exceptions.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7918 2022-06-21 00:22:59.000000 cdev-0.0.9/core/utils/file_manager.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/core/utils/fs_manager/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:22:59.000000 cdev-0.0.9/core/utils/fs_manager/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    18034 2022-06-21 00:22:59.000000 cdev-0.0.9/core/utils/fs_manager/finder.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8040 2022-06-21 00:22:59.000000 cdev-0.0.9/core/utils/fs_manager/handler_optimizer.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      823 2022-06-21 00:22:59.000000 cdev-0.0.9/core/utils/fs_manager/module_types.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    25151 2022-06-21 00:22:59.000000 cdev-0.0.9/core/utils/fs_manager/package_manager.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    10041 2022-06-21 00:22:59.000000 cdev-0.0.9/core/utils/fs_manager/package_optimizer.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3999 2022-06-21 00:22:59.000000 cdev-0.0.9/core/utils/fs_manager/serverless_function_optimizer.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/core/utils/fs_manager/standard_library_names/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1668 2022-01-24 04:34:41.000000 cdev-0.0.9/core/utils/fs_manager/standard_library_names/python_3_7
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1672 2022-01-24 04:34:41.000000 cdev-0.0.9/core/utils/fs_manager/standard_library_names/python_3_8
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1672 2022-02-17 16:40:28.000000 cdev-0.0.9/core/utils/fs_manager/standard_library_names/python_3_9
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7903 2022-06-21 00:22:59.000000 cdev-0.0.9/core/utils/fs_manager/writer.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2713 2022-06-21 00:22:59.000000 cdev-0.0.9/core/utils/hasher.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8178 2022-06-21 00:22:59.000000 cdev-0.0.9/core/utils/logger.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2451 2022-06-21 00:22:59.000000 cdev-0.0.9/core/utils/module_loader.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      978 2022-06-21 00:22:59.000000 cdev-0.0.9/core/utils/operations.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6283 2022-06-21 00:22:59.000000 cdev-0.0.9/core/utils/paths.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3503 2022-06-21 00:22:59.000000 cdev-0.0.9/core/utils/platforms.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    17637 2022-06-21 00:22:59.000000 cdev-0.0.9/core/utils/topological_helper.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/serverless_parser/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      535 2022-01-24 04:34:41.000000 cdev-0.0.9/serverless_parser/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1086 2022-06-21 00:22:59.000000 cdev-0.0.9/serverless_parser/parser.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      633 2022-06-04 19:48:48.000000 cdev-0.0.9/serverless_parser/parser_exceptions.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8961 2022-06-21 00:22:59.000000 cdev-0.0.9/serverless_parser/parser_objects.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    24260 2022-06-21 00:22:59.000000 cdev-0.0.9/serverless_parser/parser_utils.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2022-06-21 00:32:47.000000 cdev-0.0.9/setup.cfg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1404 2022-06-21 00:27:07.000000 cdev-0.0.9/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/tests/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/__init__.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/tests/core/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/__init__.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/tests/core/constructs/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/constructs/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    15990 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/constructs/backend.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/constructs/mapper.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7466 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/constructs/test_output.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     9063 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/constructs/test_workspace.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/tests/core/default/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/default/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      385 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/default/conftest.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/tests/core/default/data/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/default/data/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/default/data/example_init.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3334 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/default/test_dependency_index.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/default/test_fs_manager.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1295 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/default/test_localbackend.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1619 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/default/test_localworkspace.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    15309 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/sample_data.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/tests/core/utils/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/utils/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      385 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/utils/conftest.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2632 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/utils/test_file_manager.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3279 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/utils/test_handler_optimizer.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      750 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/utils/test_hasher.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4818 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/utils/test_package_manager_api.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    18153 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/utils/test_package_manager_helpers.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      419 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/utils/test_package_optomizer_helpers.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1999 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/utils/test_paths.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3241 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/core/utils/test_topo_helper.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:32:47.000000 cdev-0.0.9/tests/visual/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/visual/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2501 2022-06-21 00:22:59.000000 cdev-0.0.9/tests/visual/output_manager.py
```

### Comparing `cdev-0.0.8/PKG-INFO` & `cdev-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,31 @@
-Metadata-Version: 2.1
-Name: cdev
-Version: 0.0.8
-Summary: CLI for cdev sdk
-Home-page: UNKNOWN
-Author: CDEV LLC
-Author-email: daniel@cdevframework.com
-License: Clear BSD
-Platform: UNKNOWN
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # Cdev - Serverless Development Framework
 
-The Cdev framework is designed to create a development environment that allows teams to harness the benefits of Serverless development by providing high level constructs and processes to reduce the friction of transitioning to Serverless development. By being built on a custom Infrastructure as Code framework, Cdev provides unique optimizations and flexibility that allows projects to start fast and scale naturally. 
+The Cdev framework is designed to create a development environment that allows teams to harness the benefits of Serverless development by providing high level constructs and processes to reduce the friction of transitioning to Serverless development. By being built on a custom Infrastructure as Code framework, Cdev provides unique optimizations and flexibility that allows projects to start fast and scale naturally.
 
 [![](https://cdevframework.io/images/github_banner.png)](https://cdevframework.io)
 
 
 [Website](https://cdevframework.io/) • [Docs](https://cdevframework.io/docs/) • [Slack](https://slack.com/)
 
 
 ## Features
 - [Serverless Function Parsing](https://cdevframework.io/docs/)
 - [Optimized Dependency Management](https://cdevframework.io/docs/)
 - [Custom Infrastructure as Code Framework](/src/core)
 - [Designed to feel as close as possible to writing regular Python](https://cdevframework.io/docs/)
 - [Extensible Plugin and Custom Functionality Capabilities](https://cdevframework.io/docs/)
 
-## Getting Started 
+## Getting Started
 - [An Aws account and credentials](https://aws.amazon.com/)
-    - Should have the `aws cli` and then run `aws configure` to set your credenentials. 
+    - Should have the `aws cli` and then run `aws configure` to set your credenentials.
 - Requires Python>=3.6 and pip
 - **Highly** encourage using a python virtual environment
 
-Starting from an empty directory. Set up your python virtual environment and install the Cdev cli. 
+Starting from an empty directory. Set up your python virtual environment and install the Cdev cli.
 ```
 $ python -m virtualenv .venv
 
 $ . ./.venv/bin/activate
 
 $ pip install cdev
 ```
@@ -94,34 +82,32 @@
 - Static Site Hosting
 
 For guides on how to deploy any of these resources, check out our [documentation](https://cdevframework.io/docs/)
 
 ## Early Alpha Notes
 The project is still in a pre-alpha state, so not all the features of the alpha are implemented. The main branch will be the most stable branch and should not have any breaking changes as work on the alpha continues. The alpha will be ready for a public launch by March 1st. Things left to do in alpha:
 - More unit and integration tests
-- General polish of output 
+- General polish of output
 - General work on documentation
 
 For testing parts of the early alpha, it helps to start from the `resources-test` project template as that will have a bunch of preconfigured resources.
 ```
 $ cdev init demo --template resources-test
 ```
 
 ## Post Alpha Road Map and Limitations
-We are currently in the **very very** early stage of creating a comprehensive framework that helps teams throughout the whole cloud development process. As with any tool, it is important to understand what it is capabale and **not** capable of doing. Here are a list of outstanding things that we are working (or thinking) on. 
+We are currently in the **very very** early stage of creating a comprehensive framework that helps teams throughout the whole cloud development process. As with any tool, it is important to understand what it is capabale and **not** capable of doing. Here are a list of outstanding things that we are working (or thinking) on.
 
 - Remote Backend
     - The current state of cloud resources are stored in json files. This is extremely limiting as it prevents multiple people from working on the same state at the same time. We are working on creating a DB that can used as a remote backend that will allow teams to collaborate more effectively.
 
 - Limited Resources and Options on Resources
-    - We are starting by focusing on a set of resource that we feel provide value while not being too complex. We have plans to add more resource and customization as time goes on. [Our custom Infrastructure as Code framework](/src/core) provides the flexibility to deploy any resource on any cloud, but we have to put in work to generate the configurations to talk to different clouds. In the future, we hope to support a large number of Aws and non Aws resources through standardized cloud API's like the [Aws Cloud Control API](https://aws.amazon.com/cloudcontrolapi/). 
+    - We are starting by focusing on a set of resource that we feel provide value while not being too complex. We have plans to add more resource and customization as time goes on. [Our custom Infrastructure as Code framework](/src/core) provides the flexibility to deploy any resource on any cloud, but we have to put in work to generate the configurations to talk to different clouds. In the future, we hope to support a large number of Aws and non Aws resources through standardized cloud API's like the [Aws Cloud Control API](https://aws.amazon.com/cloudcontrolapi/).
 
 - The Framework is Python Only
     - We started out with building the sdk in python first because that is the language we know best. We want the sdk to feel natural in whatever language is being used, which will require adding expertise to our team from other ecosystems. The underlying primitives that make up the framework are language agnostic, so we hope to one day support a wide range of languages.
 
 - Can I export my project to an industry standard tool like Aws Cloudformation or Terraform?
-    - We understand the benefits that come from avoiding lock-in by providing the ability to interpolate with the industry standard tools. We currently provision all resources with our custom [Infrastructure as Code Framework](/src/core) and store the state of the resources in local json files, which makes created projects not compatible with other tools. We felt that with building our own framework, we could explore new optimizations and ideas that could improve the developer experience. With some work, it is possible to make our framework work with and compatible with other Infrastructure as Code Frameworks, and we will be investigating this work as we move forward. 
+    - We understand the benefits that come from avoiding lock-in by providing the ability to interpolate with the industry standard tools. We currently provision all resources with our custom [Infrastructure as Code Framework](/src/core) and store the state of the resources in local json files, which makes created projects not compatible with other tools. We felt that with building our own framework, we could explore new optimizations and ideas that could improve the developer experience. With some work, it is possible to make our framework work with and compatible with other Infrastructure as Code Frameworks, and we will be investigating this work as we move forward.
 
 
 If you are interested in any of the challenges that we are working on or have expertise you think is missing in our project, please consider [applying for a job on our team](https://cdevframework.io/docs/).
-
-
```

### Comparing `cdev-0.0.8/cdev/__init__.py` & `cdev-0.0.9/cdev/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 
 
-This tool is designed to improve the developer experience for Serverless development. 
+This tool is designed to improve the developer experience for Serverless development.
 
 
 [![Demo](https://img.shields.io/badge/demo-holder-blue)](https://img.shields.io/badge/demo-holder-blue)
 
 """
 
 
@@ -19,8 +19,7 @@
 
 
 from . import constructs, resources
 
 
 # Ergonomic mapping so that the global project instance is in a more logical place for end developers.
 Project = constructs.project.Project
-
```

### Comparing `cdev-0.0.8/cdev/cli/__main__.py` & `cdev-0.0.9/cdev/cli/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,91 +1,116 @@
 import argparse
-from ast import parse
+import json
 import logging
+import os
 import traceback
 from typing import Callable, Any
 
-from ..commands import initializer, environment, plan, deploy, run, cloud_output, local_development, destroy
+from pydantic import FilePath
+
+from ..commands import (
+    cloud_output,
+    environment,
+    plan,
+    deploy,
+    destroy,
+    project_initializer,
+    run,
+    sync,
+)
+
+from cdev.constructs.project import CDEV_PROJECT_FILE, CDEV_FOLDER
+from cdev.default.project import local_project, local_project_info
 
 parser = argparse.ArgumentParser(description="cdev cli")
 subparsers = parser.add_subparsers(title="sub_command", description="valid subcommands")
 
-def wrap_load_project(command: Callable) -> Callable[[Any], Any]:
+
+def wrap_load_and_initialize_project(
+    command: Callable, initialize: bool = True
+) -> Callable[[Any], Any]:
+    """Helper annotation that makes sure that the global Project object is in the correct state before running a given command.
+
+    Args:
+        command (Callable): command to run
+        initialize (bool, optional): Initialize the Project. Defaults to True.
+
+    Returns:
+        Callable[[Any], Any]: Wrapped function
+    """
+
     def wrapped_caller(*args, **kwargs):
         try:
-            initializer.load_project(args)
+            load_and_initialize_project(initialize=initialize)
         except Exception as e:
-            print(f"Could not load the project to call {command}")
+            print(
+                f"Could not load (initialize={initialize}) the Cdev Project to call {command}"
+            )
             print(e)
             print(traceback.format_exc())
-
             return
 
         command(args)
 
     return wrapped_caller
 
 
-def wrap_load_and_initialize_project(command: Callable) -> Callable[[Any], Any]:
-    def wrapped_caller(*args, **kwargs):
-        try:
-            initializer.load_and_initialize_project(args)
-        except Exception as e:
-            print(f"Could not load and initialize the project to call {command}")
-            print(e)
-            print(traceback.format_exc())
-            return
+def load_and_initialize_project(initialize: bool = True) -> None:
+    """Create the global instance of the `Project` object as a `local_project` instance. If provided, also initialize the `Project`.
 
-        command(args)
+    Args:
+        initialize (bool, optional): Initialize the project. Defaults to True.
+    """
+    base_directory = os.getcwd()
 
-    return wrapped_caller
+    project_info_location = os.path.join(base_directory, CDEV_FOLDER, CDEV_PROJECT_FILE)
+    project_info = _load_local_project_information(project_info_location)
+
+    project = local_project(
+        project_info=project_info, project_info_filepath=project_info_location
+    )
+    if initialize:
+        project.initialize_project()
+
+
+def _load_local_project_information(
+    project_info_location: FilePath,
+) -> local_project_info:
+    """Help function to load the project info json file
+
+    Args:
+        project_info_location (FilePath): location of project info json
+
+    Returns:
+        local_project_info
+    """
+    with open(project_info_location, "r") as fh:
+        return local_project_info(**json.load(fh))
 
 
 CDEV_COMMANDS = [
     {
-        "name": "plan",
-        "help": "See the differences that have been made since the last deployment",
-        "default": wrap_load_and_initialize_project(plan.plan_command_cli),
-    },
-    {
         "name": "init",
         "help": "Create a new project",
-        "default": initializer.create_project_cli,
+        "default": project_initializer.create_project_cli,
         "args": [
             {"dest": "name", "type": str, "help": "Name of the new project"},
-            {"dest": "--template", "type": str, "help": "Name of the template for the new project"}
+            {
+                "dest": "--template",
+                "type": str,
+                "help": "Name of the template for the new project",
+            },
         ],
     },
     {
-        "name": "develop",
-        "help": "Open an interactive development environment",
-        "default": wrap_load_and_initialize_project(local_development.develop_command_cli),
-        "args": [
-            {"dest": "--complex", "help": "run a simple follower instead of full development environment", "action":"store_true"}
-        ]
-    },
-    {
-        "name": "destroy",
-        "help": "Destroy all the resources in the current environment",
-        "default": wrap_load_and_initialize_project(destroy.destroy_command_cli)
-    }, 
-
-    {
-        "name": "output",
-        "help": "See the generated cloud output",
-        "default": wrap_load_and_initialize_project(cloud_output.cloud_output_command_cli),
-        "args": [
-            {"dest": "cloud_output_id", "type": str, "help": "Id of the cloud output to display. ex: <component>.<ruuid>.<cdev_name>.<output_key>"},
-            {"dest": "--value", "help": "display only the value. Helpful for exporting values.", "action":"store_true"}
-        ]
-    }, 
-    {
         "name": "environment",
         "help": "Change and create environments for deployment",
-        "default": wrap_load_and_initialize_project(environment.environment_cli),
+        "default": wrap_load_and_initialize_project(
+            environment.environment_cli, initialize=False
+        ),
         "subcommands": [
             {
                 "command": "ls",
                 "help": "Show all available environments",
                 "args": [
                     {
                         "dest": "--all",
@@ -102,19 +127,19 @@
                         "dest": "env",
                         "type": str,
                         "help": "environment you want set as the new working environment",
                     }
                 ],
             },
             {
-                "command": "get",
+                "command": "info",
                 "help": "Get information about an environment",
                 "args": [
                     {
-                        "dest": "env",
+                        "dest": "--env",
                         "type": str,
                         "help": "environment you want info about",
                     }
                 ],
             },
             {
                 "command": "create",
@@ -141,65 +166,127 @@
                         "type": str,
                         "help": "New value of the variable. Must be used with --key.",
                     },
                     {
                         "dest": "--all",
                         "action": "store_true",
                         "help": "Set the value for all environments. Must be used with --new-value.",
-                    }
+                    },
                 ],
             },
         ],
     },
     {
+        "name": "plan",
+        "help": "See the differences that have been made since the last deployment",
+        "default": wrap_load_and_initialize_project(plan.plan_command_cli),
+    },
+    {
         "name": "deploy",
         "help": "Deploy a set of changes",
-        "default": wrap_load_and_initialize_project(deploy.deploy_command_cli)
+        "default": wrap_load_and_initialize_project(deploy.deploy_command_cli),
+    },
+    {
+        "name": "destroy",
+        "help": "Destroy all the resources in the current environment",
+        "default": wrap_load_and_initialize_project(destroy.destroy_command_cli),
+    },
+    {
+        "name": "output",
+        "help": "See the generated cloud output",
+        "default": wrap_load_and_initialize_project(
+            cloud_output.cloud_output_command_cli
+        ),
+        "args": [
+            {
+                "dest": "cloud_output_id",
+                "type": str,
+                "help": "Id of the cloud output to display. ex: <component>.<ruuid>.<cdev_name>.<output_key>",
+            },
+            {
+                "dest": "--value",
+                "help": "display only the value. Helpful for exporting values.",
+                "action": "store_true",
+            },
+        ],
     },
     {
         "name": "run",
         "help": "This command is used to run user defined and resource functions.",
         "default": wrap_load_and_initialize_project(run.run_command_cli),
         "args": [
             {"dest": "subcommand", "help": "the user defined command to call"},
             {"dest": "args", "nargs": argparse.REMAINDER},
         ],
     },
+    {
+        "name": "sync",
+        "help": "Watch for changes in the filesystem and perform a deploy automatically",
+        "default": wrap_load_and_initialize_project(sync.sync_command_cli),
+        "args": [
+            {
+                "dest": "--no-default",
+                "action": "store_true",
+                "help": "by default we ignore certain files and watch for some of them. If you want complete control on what is considered a change, turn this on and set your custom filters using --watch and --ignore",
+            },
+            {
+                "dest": "--disable-prompt",
+                "action": "store_true",
+                "help": "by default we ask for confirmation before deploying changes. Turn this on and perform deployments w/o requiring confirmation",
+            },
+            {
+                "dest": "--watch",
+                "type": str,
+                "help": "watch any file that matches the following pattern ['src/**/*.py','settings/*']",
+            },
+            {
+                "dest": "--ignore",
+                "type": str,
+                "help": "do not watch for any file that matches the following pattern ['.cdev/**','__pycache__/*']",
+            },
+        ],
+    },
 ]
 
 
 def subcommand_function_wrapper(name, func):
     # This wraps a function so that is can be used for subcommands by basing the subcommand as the first arg to the function
     # then the remaining args as the second arg
     def inner(args):
 
         return func(name, args)
 
     return inner
 
 
-def add_general_output_options(parser: argparse.ArgumentParser):
+def add_general_output_options(parser: argparse.ArgumentParser) -> None:
     parser.add_argument(
         "--output",
         type=str,
         choices=["json", "plain-text", "rich"],
         help="change the type of output generated",
     )
 
     parser.add_argument(
-        '-d', '--debug',
+        "-d",
+        "--debug",
         help="Print debug log statements. This is mostly for development use",
-        action="store_const", dest="loglevel", const=logging.DEBUG,
+        action="store_const",
+        dest="loglevel",
+        const=logging.DEBUG,
         default=logging.WARNING,
     )
 
     parser.add_argument(
-        '-v', '--verbose',
+        "-v",
+        "--verbose",
         help="Print info log message. Use this to get a more detailed understanding of what is executing.",
-        action="store_const", dest="loglevel", const=logging.INFO,
+        action="store_const",
+        dest="loglevel",
+        const=logging.INFO,
     )
 
 
 for command in CDEV_COMMANDS:
     tmp = subparsers.add_parser(command.get("name"), help=command.get("help"))
 
     if command.get("subcommands"):
@@ -215,24 +302,22 @@
             )
 
             for arg in subcommand.get("args"):
                 dest = arg.get("dest")
                 arg.pop("dest")
                 t2.add_argument(dest, **arg)
 
-           
             add_general_output_options(t2)
 
     else:
         if command.get("args"):
             for arg in command.get("args"):
-                dest = arg.get("dest")
-                arg.pop("dest")
+                dest = arg.pop("dest")
                 tmp.add_argument(dest, **arg)
 
         tmp.set_defaults(func=command.get("default"))
 
         add_general_output_options(tmp)
 
 
 args = parser.parse_args()
-args.func(args)
+args.func(args)
```

### Comparing `cdev-0.0.8/cdev/commands/cloud_output.py` & `cdev-0.0.9/cdev/commands/cloud_output.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,22 @@
 from cdev.default.output_manager import CdevOutputManager
 from cdev.cli.logger import set_global_logger_from_cli
 
 
 from core.commands.cloud_output import cloud_output_command as core_cloud_output_command
 
 
-def cloud_output_command_cli(args):
+def cloud_output_command_cli(args) -> None:
     config = args[0]
     set_global_logger_from_cli(config.loglevel)
     cloud_output_command(config.cloud_output_id, config.value)
 
 
-def cloud_output_command(cloud_output_id: str, only_value: bool):
+def cloud_output_command(cloud_output_id: str, only_value: bool) -> None:
 
     output_manager = CdevOutputManager()
 
     myProject = Project.instance()
-    
-    ws = myProject.get_current_environment().get_workspace()
 
+    ws = myProject.get_current_environment().get_workspace()
 
     core_cloud_output_command(ws, output_manager, cloud_output_id, only_value)
-    
-
```

### Comparing `cdev-0.0.8/cdev/commands/deploy.py` & `cdev-0.0.9/cdev/commands/deploy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from cdev.constructs.project import Project
 from cdev.default.output_manager import CdevOutputManager
 from cdev.cli.logger import set_global_logger_from_cli
 
 from core.commands.deploy_differences import execute_deployment
 
 
-
-def deploy_command_cli(args):
+def deploy_command_cli(args) -> None:
     config = args[0]
     set_global_logger_from_cli(config.loglevel)
     deploy_command(args)
 
 
-def deploy_command(args):
+def deploy_command(args) -> None:
 
     output_manager = CdevOutputManager()
     myProject = Project.instance()
 
     ws = myProject.get_current_environment().get_workspace()
 
     execute_deployment(ws, output_manager)
```

### Comparing `cdev-0.0.8/cdev/commands/destroy.py` & `cdev-0.0.9/cdev/commands/destroy.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,44 +2,45 @@
 from cdev.default.output_manager import CdevOutputManager
 from cdev.cli.logger import set_global_logger_from_cli
 from rich.prompt import Confirm
 
 
 from core.constructs.workspace import Workspace_State
 
-def destroy_command_cli(args):
+
+def destroy_command_cli(args) -> None:
     config = args[0]
     set_global_logger_from_cli(config.loglevel)
     destroy_command(args)
 
 
-def destroy_command(args):
+def destroy_command(args) -> None:
 
     output_manager = CdevOutputManager()
     myProject = Project.instance()
 
     ws = myProject.get_current_environment().get_workspace()
 
-
     ws.set_state(Workspace_State.EXECUTING_FRONTEND)
 
-    diff_previous_component_names = [x.name for x in ws.get_backend().get_resource_state(ws.get_resource_state_uuid()).components]
-
+    diff_previous_component_names = [
+        x.name
+        for x in ws.get_backend()
+        .get_resource_state(ws.get_resource_state_uuid())
+        .components
+    ]
 
     differences = ws.create_state_differences([], diff_previous_component_names)
 
     if any(x for x in differences):
         output_manager.print_state_differences(differences)
 
-
-    
-
     print("")
     do_deployment = Confirm.ask("Are you sure you want to Destroy the environment?")
 
     if not do_deployment:
         return
 
     differences_structured = ws.sort_differences(differences)
     ws.set_state(Workspace_State.EXECUTING_BACKEND)
 
-    ws.deploy_differences(differences_structured)
+    ws.deploy_differences(differences_structured)
```

### Comparing `cdev-0.0.8/cdev/commands/local_development.py` & `cdev-0.0.9/cdev/commands/local_development.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from cdev.constructs.project import Project
 from cdev.cli.logger import set_global_logger_from_cli
 
-from core.commands.deploy_differences import execute_deployment
 from cdev.default.output_manager import CdevOutputManager
 
 
-def develop_command_cli(args):
+def develop_command_cli(args) -> None:
     config = args[0]
     set_global_logger_from_cli(config.loglevel)
     develop_command(args)
 
 
-def develop_command(args):
+def develop_command(args) -> None:
 
     output_manager = CdevOutputManager()
     myProject = Project.instance()
 
     print(f"Live Development")
 
 
-
 """import os
 import sys
 from time import sleep
 from typing import Dict, List, Tuple
 
 from rich.console import Console
 from rich.layout import Layout
@@ -36,20 +34,20 @@
 from watchdog.observers import Observer
 from watchdog.events import PatternMatchingEventHandler
 from cdev.constructs import Cdev_Project
 
 from cdev.utils import hasher
 
 import threading
-    
+
 from ..utils import project
 from ..frontend import executer as frontend_executer
 from ..backend import executer as backend_executer
 from ..backend import resource_state_manager, cloud_mapper_manager
-    
+
 from cdev import output as cdev_output
 from cdev.settings import set_setting
 
 from . import deploy
 
 STD_OUT_HISTORY_BUFFER = []
 history = []
@@ -61,19 +59,19 @@
     "is_deploy_running": False
 }
 
 
 def make_develop_layout() -> Layout:
     layout = Layout("tmp")
     layout.split(
-        
+
         Layout(name="stdout"),
-        Layout(name="cloud_output"), 
-        Layout(name="commands"), 
-     
+        Layout(name="cloud_output"),
+        Layout(name="commands"),
+
     )
 
     layout['stdout'].ratio = 80
     layout['cloud_output'].ratio = 20
     layout['commands'].ratio = 1
     #layout['hidden'].visible = False
 
@@ -115,51 +113,51 @@
     else:
         my_event_handler.on_created = file_change_handler
         my_event_handler.on_deleted = file_change_handler
         my_event_handler.on_modified = file_change_handler
         my_event_handler.on_moved = file_change_handler
 
         my_observer.schedule(my_event_handler, path, recursive=go_recursively)
-    
 
-    
+
+
     cdev_output.create_buffer(CLOUD_OUTPUT_BUFFER)
     refresh_local_output({"buffer_name": CLOUD_OUTPUT_BUFFER, "reinitialize_project": True})
     my_observer.start()
     cdev_output.print(f"")
     cdev_output.print(f"[blink] *** waiting for changes ***[/blink]")
-    
+
     handle_std_in_thread = threading.Thread(target=handle_std_input, daemon=True)
     try:
-        
+
         if args.simple:
             # IF this is a simple develop session don't create live panels
             while True:
                 pass
 
-        
+
         with LIVE_OBJECT as l:
             refresh_output_buffer()
-            
+
             handle_std_in_thread.start()
             last_stdout_hash = 0
             while True:
                 messages, start_line_no, messages_hash = cdev_output.get_messages_from_buffer(-25,None)
-                
+
                 modified_messages = [f"({start_line_no+i}) {x}" for i,x in enumerate(messages,0)]
 
                 if messages_hash == last_stdout_hash:
                     pass
                 else:
-                    
+
                     messages_as_string = "\n".join(modified_messages)
                     last_stdout_hash = messages_hash
                     LAYOUT['stdout'].update(Panel(messages_as_string, title="STD OUT"))
                     update_screen()
-                    
+
                     sleep(.1)
 
 
     except KeyboardInterrupt:
         print("Development environment closed1")
         my_observer.stop()
         my_observer.join()
@@ -204,60 +202,60 @@
     CDEV_PROJECT = Cdev_Project()
     CDEV_PROJECT.clear_previous_state()
     cdev_output.print(f"File Change Detected. Starting Deploy Process")
     did_deploy = deploy.local_deploy_command({})
     if did_deploy:
         refresh_output_simple()
     cdev_output.print(f"[blink] *** waiting for changes ***[/blink]")
-    
+
     update_screen()
 
 
 
 
 def update_screen():
     LIVE_OBJECT.update(LAYOUT, refresh=True)
 
 
 def add_line_to_history(line):
     history.append(line)
 
-    
+
 
 def get_output_buffer() -> Tuple[str, str]:
     if not history:
         return None
 
     lines = '\n'.join(history)
     hash_val = hasher.hash_string(lines)
 
     #history.clear()
     return lines, hash_val
 
 
-def refresh_local_output(args: Dict):  
+def refresh_local_output(args: Dict):
 
     if not "buffer_name" in args:
         write_to_buffer = False
     else:
         write_to_buffer = True
 
     if args.get("reinitialize_project"):
         project.initialize_project()
         frontend_executer.execute_frontend()
 
 
     PROJECT = project.Cdev_Project()
-    
+
     desired_outputs = PROJECT.get_outputs()
 
     rendered_outputs = []
 
-    for label, output in desired_outputs.items(): 
-        
+    for label, output in desired_outputs.items():
+
         identifier = output.resource.split("::")[-1]
 
         if output.transformer:
             rendered_value = cloud_mapper_manager.get_output_value_by_hash(identifier, output.key, transformer=output.get("transformer"))
         else:
             rendered_value = cloud_mapper_manager.get_output_value_by_hash(identifier, output.key)
 
@@ -270,11 +268,11 @@
 
     for rendered_output in rendered_outputs:
         if not write_to_buffer:
             cdev_output.print(rendered_output)
         else:
             cdev_output.add_message_to_buffer(args.get("buffer_name"), str(rendered_output))
 
-    
+
 
 
 """
```

### Comparing `cdev-0.0.8/cdev/commands/plan.py` & `cdev-0.0.9/cdev/commands/plan.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,30 +2,25 @@
 from cdev.cli.logger import set_global_logger_from_cli
 from cdev.default.output_manager import CdevOutputManager
 
 from core.commands.execute_frontend import execute_frontend
 from core.utils.logger import log
 
 
-
-def plan_command_cli(args):
+def plan_command_cli(args) -> None:
     config = args[0]
     set_global_logger_from_cli(config.loglevel)
 
     plan_command({})
 
 
-def plan_command(args):
+def plan_command(args) -> None:
     log.info(msg="Starting Plan Command")
     output_manager = CdevOutputManager()
 
     myProject = Project.instance()
     log.debug("Loaded Project Global Instance")
-    
+
     ws = myProject.get_current_environment().get_workspace()
 
-    
-    
     execute_frontend(ws, output_manager)
     log.info("Finished Plan Command")
-
-
```

### Comparing `cdev-0.0.8/cdev/commands/run.py` & `cdev-0.0.9/cdev/commands/run.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from cdev.constructs.project import Project
 from cdev.cli.logger import set_global_logger_from_cli
 from cdev.default.output_manager import CdevOutputManager
 
 from core.commands.run import run_command as core_run_command
 
 
-def run_command_cli(args):
+def run_command_cli(args) -> None:
     config = args[0]
     set_global_logger_from_cli(config.loglevel)
 
     run_command(args[0])
 
 
-def run_command(args):
+def run_command(args) -> None:
     output_manager = CdevOutputManager()
 
-    myProject = Project.instance()
-    
-    ws = myProject.get_current_environment().get_workspace()
-    
-    core_run_command(ws, output_manager, args)
+    my_project = Project.instance()
+
+    ws = my_project.get_current_environment().get_workspace()
+
+    core_run_command(ws, output_manager, args)
```

### Comparing `cdev-0.0.8/cdev/constructs/environment.py` & `cdev-0.0.9/cdev/constructs/environment.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,49 @@
-from typing import List, Dict
-
 from pydantic import BaseModel
-from pydantic.types import FilePath
 
 from core.constructs.workspace import Workspace, Workspace_Info
 
 
-
-
 class environment_info(BaseModel):
     """
     Represents the information about an environment.
 
     Arguments:
         name (str): Name of this environment
         workspace_info (Workspace_Info): The information needed to load the Workspace for this environment
     """
 
     name: str
     workspace_info: Workspace_Info
 
-    def __init__(
-        __pydantic_self__,
-        name: str,
-        workspace_info: Workspace_Info
-        ) -> None:
-
-        super().__init__(
-            **{"name": name, "workspace_info": workspace_info}
-        )
+    def __init__(__pydantic_self__, name: str, workspace_info: Workspace_Info) -> None:
+
+        super().__init__(**{"name": name, "workspace_info": workspace_info})
 
 
 class Environment:
     """
     A logically isolated instance of a project.
     """
 
     def __init__(self, info: environment_info) -> None:
         pass
 
+    def get_name(self) -> str:
+        """Return the name of the Environment
+
+        Returns:
+            str: name of the Environment
+        """
+        raise NotImplementedError
+
     def get_workspace(self) -> Workspace:
+        """Get the Workspace associated with this Environment
+
+        Returns:
+            Workspace
+        """
         raise NotImplementedError
 
-    def initialize_environment(self):
+    def initialize_environment(self) -> None:
+        """Initialize the Environment"""
         raise NotImplementedError
```

### Comparing `cdev-0.0.8/cdev/constructs/project.py` & `cdev-0.0.9/cdev/constructs/project.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,68 +13,74 @@
 from core.constructs.cloud_output import Cloud_Output
 from core.constructs.settings import Settings, Settings_Info
 
 from .environment import environment_info, Environment
 
 _GLOBAL_PROJECT = None
 
+# Global definition that defines a cdev project as having a folder called `.cdev` with a valid `cdev_project.json`
+CDEV_FOLDER = ".cdev"
+CDEV_PROJECT_FILE = "cdev_project.json"
 
-class project_info(BaseModel):
-    project_name: str
-    environments: List[environment_info]
-    backend_info: Backend_Configuration
-    current_environment: Optional[str]
-
-    def __init__(
-        __pydantic_self__,
-        project_name: str,
-        environments: List[environment_info],
-        backend_info: Backend_Configuration,
-        current_environment: str = None,
-       
-    ) -> None:
-        """
-        Represents the data about a cdev project object:
 
-        Parameters:
-            project_name (str): Name of the project
-            environments (List[environment_info]): The environments that are currently part of the project
-            current_environment (str): The current environment
-            
-        """
-
-        super().__init__(
-            **{
-                "project_name": project_name,
-                "environments": environments,
-                "backend_info": backend_info,
-                "current_environment": current_environment,
-            }
-        )
+class Project_Info(BaseModel):
+    project_name: str
+    environment_infos: List[environment_info]
+    default_backend_configuration: Backend_Configuration
+    current_environment_name: Optional[str]
 
 
 class Project_State(str, Enum):
-    UNINITIALIZED = "UNINITIALIZED"
+    INFO_LOADED = "INFO_LOADED"
     INITIALIZING = "INITIALIZING"
     INITIALIZED = "INITIALIZED"
 
 
+###############################
+##### Exceptions
+###############################
+class ProjectError(Exception):
+    pass
+
+
+class NoGlobalProject(ProjectError):
+    pass
+
+
+class IncorrectPhase(ProjectError):
+    pass
+
+
+class EnvironmentDoesNotExist(ProjectError):
+    pass
+
+
+class NoCurrentEnvironment(ProjectError):
+    pass
+
+
+class BackendError(ProjectError):
+    pass
+
+
+class FilesystemError(ProjectError):
+    pass
+
 
 def wrap_phases(phases: List[Project_State]) -> Callable[[F], F]:
     """
-    Annotation that denotes when a function can be executed within the life cycle of a workspace. Throws excpetion if the workspace is not in the correct
+    Annotation that denotes when a function can be executed within the life cycle of a Project. Throws exception if the Project is not in the correct
     phase.
     """
 
     def inner_wrap(func: F) -> F:
         def wrapper_func(project: "Project", *func_posargs, **func_kwargs):
-
             current_state = project.get_state()
             if not current_state in phases:
-                raise Exception(
+                raise IncorrectPhase(
                     f"Trying to call {func} while in project state {current_state} but need to be in {phases}"
                 )
 
             else:
 
                 return func(project, *func_posargs, **func_kwargs)
 
@@ -89,359 +95,346 @@
     by Cdev to provide access to helpful API's for developers to use in their projects. The object is created and managed by
     the Cdev framework and follows a set of lifecycle rules (link to documentation).
 
     Developers can access the object in their projects by calling `Project.instance()`. When using the Project Object, developers
     should keep in mind the lifecycle rules around each API and how it fits into their project.
 
     """
+
     _settings: Settings
 
     @classmethod
-    def instance(cls):
-        """
-        Method to retrieve the global instance of the Project object.
+    def instance(cls) -> "Project":
+        """Method to retrieve the global instance of the Project object.
+
+        Raises:
+            NoGlobalProject
         """
         if not _GLOBAL_PROJECT:
-            raise Exception("Currently No GLOBAL PROJECT OBJECT")
+            raise NoGlobalProject
 
         return _GLOBAL_PROJECT
 
     @classmethod
-    def set_global_instance(cls, project: "Project"):
-        """
-        Method to set the global Project object. Should only be used to as defined in the lifecycle of the Cdev process. (documentation)
-        """
-        global _GLOBAL_PROJECT
-        _GLOBAL_PROJECT = project
-
-    @classmethod
-    def remove_global_instance(cls, caller: "Project"):
-        """
-        Method to reset the Global Project object. This should be the final cleanup step for a Cdev process.
-        """
-        global _GLOBAL_PROJECT
-
-        if not _GLOBAL_PROJECT:
-            raise Exception("Global Project is not set")
-
-        if not _GLOBAL_PROJECT == caller:
-            raise Exception("Only the current Project object can remove itself")
-
-        _GLOBAL_PROJECT = None
-
-
-    def set_name(self, name: str):
-        """
-        Set the name of this Project
+    def set_global_instance(cls, project: "Project") -> None:
+        """Method to set the global Project object. Should only be used by sub-classes to register themselves as the global `Project` within the
+        cdev execution steps.
 
         Args:
-            name (str): name of the Project
+            project (Project): Object to register as global Project
         """
-        raise NotImplementedError
+        global _GLOBAL_PROJECT
+        _GLOBAL_PROJECT = project
 
-
-    def get_name(self):
-        """
-        Get the name of this Project
+    def get_name(self) -> str:
+        """Get the name of this Project
 
         Returns:
             name (str)
+
+        Raises:
+            ProjectError
         """
         raise NotImplementedError
 
     def get_state(self) -> Project_State:
-        """
-        Get the current lifecycle state of the Project.
+        """Get the current lifecycle state of the Project.
 
         Returns:
             state (Project_State)
+
+        Raises:
+            ProjectError
         """
         raise NotImplementedError
 
-    def initialize_project(self):
-        """
-        Initialize the Project object so that it is ready to perform a given operation. Note that any configuration needed for the initialization
-        process should be defined during the creation of the object, and set such that this function needs no input.
+    def set_state(self, new_state: Project_State) -> None:
+        """Set the current lifecycle state of the Project
+
+        Args:
+            new_state (Project_State): new project state
         """
         raise NotImplementedError
 
-    def terminate_project(self):
-        """
-        Terminate the Project object as a cleanup operation after a given operation is complete. This should be the final step in the life cycle
-        of an operation that need to initialize the project.
+    def initialize_project(self) -> None:
+        """Initialize the Project object. This function can only be called when in the `LOAD_INFO` state. It will transition into the `INITIALIZING` phase
+        while the function is executing. Then it will transition to the `INITIALIZED` phase as the final action.
+
+        Raises:
+            ProjectError
         """
         raise NotImplementedError
 
-    def create_environment(self, environment_name: str, settings_files: List[str]):
-        """
-        Create a new environment for this project.
+    def create_environment(
+        self, environment_name: str, backend_configuration: Backend_Configuration = None
+    ) -> None:
+        """Create a new environment for this project.
+
+        Args:
+            environment_name (str): Name of the `Environment` to create
+            backend_configuration (Backend_Configuration, optional): Backend configuration to associate with the created `Environment`. Defaults to None.
+
+        Raises:
+            ProjectError
         """
         raise NotImplementedError
 
-    def destroy_environment(self, environment_name: str):
-        """
-        Destroy an environment. This function should only be called when the project is in the Initialized state, so that
-        any cloud resources in the environment will be destroyed.
+    def destroy_environment(self, environment_name: str) -> None:
+        """Destroy an environment. This function should only be used to delete the information about an environment. To delete actual cloud resources in an,
+        an environment you should use the `cdev destroy` command.
+
+        Args:
+            environment_name (str): Name of the `Environment` to destroy
+
+        Raises:
+            ProjectError
+            EnvironmentDoesNotExist
         """
         raise NotImplementedError
 
     def get_all_environment_names(self) -> List[str]:
-        """
-        Get all the available environments in the Project.
+        """Get all the available environments in the Project.
 
         Returns:
             environment_names (List[str]): environments
+
+        Raises:
+            ProjectError
         """
         raise NotImplementedError
 
     def get_current_environment_name(self) -> str:
-        """
-        Get the environment name that is currently active for this Project.
+        """Get the environment name that is currently active for this Project.
 
         Returns:
             environment_name (str)
+
+        Raises:
+            EnvironmentDoesNotExist
+            NoCurrentEnvironment
         """
         raise NotImplementedError
 
-    def set_current_environment(self, environment_name: str):
-        """
-        Change the currently active environment for this Project. This should only be called when the Project is
+    def set_current_environment(self, environment_name: str) -> None:
+        """Change the currently active environment for this Project. This should only be called when the Project is
         in the Uninitialized state to prevent it from being called during operations that modify an environment.
 
-        Arguments:
+        Args:
             environment_name (str): The environment name to switch to
 
         Raises:
             EnvironmentDoesNotExist
         """
         raise NotImplementedError
 
-    def get_environment(self, environment_name: str) -> Environment:
-        """
-        Get the environment object for a specified environment name. Note that the environment will be in a state
-        based on when this function is called within the Cdev lifecycle.
+    def get_environment_settings_info(
+        self, environment_name: str = None
+    ) -> Settings_Info:
+        """Get the information about an Environments Settings Modules
 
-        Arguments:
-            environment_name (str): The environment name to switch to
+        Args:
+            environment_name (str, optional): Name of the Environment. Defaults to None.
 
         Raises:
+            ProjectError
             EnvironmentDoesNotExist
+
+        Returns:
+            Settings_Info
         """
         raise NotImplementedError
 
-    def get_current_environment(self) -> Environment:
+    def update_environment_settings_info(
+        self, new_value: Settings_Info, environment_name: str = None
+    ):
+        """Update the information Settings Module Information for a given Environment
+
+        Args:
+            new_value (Settings_Info): New Settings Info for the Environment
+            environment_name (str, optional): Environment name to update. Defaults to None.
+
+        Raises:
+            ProjectError
+            EnvironmentDoesNotExist
         """
-        Get the environment object for the currently active Environment. Note that the Environment will be in a state
+        raise NotImplementedError
+
+    def get_environment(self, environment_name: str) -> Environment:
+        """Get the environment object for a specified environment name. Note that the environment will be in a state
         based on when this function is called within the Cdev lifecycle.
 
-        Arguments:
+        Args:
             environment_name (str): The environment name to switch to
 
         Raises:
             EnvironmentDoesNotExist
         """
         raise NotImplementedError
 
+    def get_current_environment(self) -> Environment:
+        """Get the environment object for the currently active Environment. Note that the Environment will be in a state
+        based on when this function is called within the Cdev lifecycle.
+
+        Raises:
+            EnvironmentDoesNotExist
+            NoCurrentEnvironment
+        """
+        raise NotImplementedError
 
     ############################
     ##### Settings
     ############################
     @property
     def settings(self) -> Settings:
         raise NotImplementedError
 
-    
     @settings.setter
     def settings(self, value: Settings):
         raise NotImplementedError
 
-
-    def get_settings_info(self, environment_name: str = None) -> Settings_Info:
-        raise NotImplementedError
-
-    
-    def update_settings_info(self, new_value: Settings_Info, environment_name: str = None):
-        raise NotImplementedError
-
-
     #######################
     ##### Display Output
     #######################
 
-    def display_output(self, tag: str, output: Cloud_Output):
-        """Display the output from a Resource or Reference after a process has completed
+    def display_output(self, tag: str, output: Cloud_Output) -> None:
+        """Display the output from a Resource or Reference after a `Deployment` process has completed
 
         Args:
             tag: A key value to display with the output
             output: The Cloud Output to render
         """
         raise NotImplementedError
 
-
-    def render_outputs(self) -> List[Tuple[str, Any]]:
-        """Render the output associated with the Workspace
-
-        Returns:
-            List[Tuple[str, Any]]: The List of outputs with their associated tag
-        
-        """
-        raise NotImplementedError
-
     #################
     ##### Mappers
     #################
     def add_mapper(self, mapper: CloudMapper) -> None:
-        """
-        Add a CloudMapper to the project. The order that the Mappers are added to the Project defines the precedence give when
+        """Add a CloudMapper to the project. The order that the Mappers are added to the Project defines the precedence give when
         determining which CloudMapper to use.
 
-        Note that this function should only be called during the `Project Initialization` part of the Cdev lifecycle.
-
-        Arguments:
+        Args:
             mapper (CloudMapper): The mapper to add
+
+        Raises:
+            ProjectError
         """
         raise NotImplementedError
 
     def add_mappers(self, mappers: List[CloudMapper]) -> None:
-        """
-        Add a List of CloudMappers to the project. The order that the Mappers are added to the Project defines the precedence
+        """Add a List of CloudMappers to the project. The order that the Mappers are added to the Project defines the precedence
         give when determining which CloudMapper to use.
 
-        Note that this function should only be called during the `Project Initialization` part of the Cdev lifecycle.
-
-        Arguments:
+        Args:
             mappers (List[CloudMapper]): The mapper to add
+
+        Raises:
+            ProjectError
         """
         raise NotImplementedError
 
     def get_mappers(self) -> List[CloudMapper]:
-        """
-        Return the List of CloudMappers for this Project.
-
-        Note that this function should only be called during the `Project Initialized` part of the Cdev lifecycle.
+        """Return the List of CloudMappers for this Project.
 
         Returns:
             mappers (List[CloudMapper]): mappers for this Project
+
+        Raises:
+            ProjectError
         """
         raise NotImplementedError
 
     def get_mapper_namespace(self) -> Dict[str, CloudMapper]:
-        """
-        Return the Dictionary that maps Resource ID's (ruuid) to the mapper that will be used to deploy the resource into the cloud.
-
-        Note that this function should only be called during the `Project Initialized` part of the Cdev lifecycle.
+        """Return the Dictionary that maps Resource ID's (ruuid) to the mapper that will be used to deploy the resource into the cloud.
 
         Returns:
             ruuid_to_mapper (Dict[str, CloudMapper]): Resource ID to CloudMapper
         """
         raise NotImplementedError
 
     #################
     ##### Commands
     #################
     def add_command(self, command_location: str):
-        """
-        Add a Command Location to the Project. The order that the Command is added to the Project defines the precedence
+        """Add a Command Location to the Project. The order that the Command is added to the Project defines the precedence
         give when searching for Commands. Command Locations should adhere to the defined form to ensure that they can be
         found within the Project.
 
-        Note that this function should only be called during the `Project Initialization` part of the Cdev lifecycle.
-
-        Arguments:
+        Args:
             command_location (Command): The command location to add
         """
         raise NotImplementedError
 
     def add_commands(self, command_locations: List[str]):
-        """
-        Add a List of Command Locations to the Project. The order that the Commands are added to the Project defines the precedence
+        """Add a List of Command Locations to the Project. The order that the Commands are added to the Project defines the precedence
         give when searching for a Command. Command Locations should adhere to the defined form to ensure that they can be
         found within the Project.
 
-        Note that this function should only be called during the `Project Initialization` part of the Cdev lifecycle.
-
-        Arguments:
-            command_locations (Command): The command location to add
+        Args:
+            command_locations (Command): The command locations to add
         """
         raise NotImplementedError
 
     def get_commands(self) -> List[str]:
-        """
-        Get the Command Locations for this Project.
-
-        Note that this function should only be called during the `Project Initialized` part of the Cdev lifecycle.
+        """Get the Command Locations for this Project.
 
         Returns:
             command_locations (List[str])
         """
         raise NotImplementedError
 
     #################
     ##### Components
     #################
-    def add_component(self, component: Component):
-        """
-        Add a Component to the Project. Components are used to determine the desired state of the Project. They should represent
+    def add_component(self, component: Component) -> None:
+        """Add a Component to the Project. Components are used to determine the desired state of the Project. They should represent
         a logical separation for the Resources in a project.
 
-        Note that this function should only be called during the `Project Initialization` part of the Cdev lifecycle.
-
-        Arguments:
+        Args:
             component (Component): Component to add
         """
         raise NotImplementedError
 
-    def add_components(self, components: List[Component]):
-        """
-        Add a List of Components to the Project. Components are used to determine the desired state of the Project. They
+    def add_components(self, components: List[Component]) -> None:
+        """Add a List of Components to the Project. Components are used to determine the desired state of the Project. They
         should represent a logical separation for the Resources in a project.
 
-        Note that this function should only be called during the `Project Initialization` part of the Cdev lifecycle.
-
-        Arguments:
-            component (Component): Component to add
+        Args:
+            components (Component): Components to add
         """
         raise NotImplementedError
 
     def get_components(self) -> List[Component]:
-        """
-        Return the Components for this Project.
-
-        Note that this function should only be called during the `Project Initialized` part of the Cdev lifecycle.
+        """Return the Components for this Project.
 
         Returns:
             components (List[Component])
         """
         raise NotImplementedError
 
 
 def check_if_project_exists(base_directory: DirectoryPath) -> bool:
     """
     This function checks for an existing Cdev project at the given directory. A Cdev project is defined by the existence of a valid
     'cdev_project.json' file (can be loaded as project_info) at the location of <base_directory>/.cdev/.
 
-    Arguments:
+    Args:
         base_directory: Directory to start search from
     """
-
-    CDEV_FOLDER = ".cdev"
-    CDEV_PROJECT_FILE = "cdev_project.json"
-
     if not os.path.isdir(base_directory):
         raise Exception(f"Given base directory is not a directory {base_directory}")
 
     if not os.path.isdir(os.path.join(base_directory, CDEV_FOLDER)):
         return False
 
     if not os.path.isfile(os.path.join(base_directory, CDEV_FOLDER, CDEV_PROJECT_FILE)):
         return False
 
     try:
         with open(
             os.path.join(base_directory, CDEV_FOLDER, CDEV_PROJECT_FILE), "r"
         ) as fh:
-            project_info(**json.load(fh))
+            Project_Info(**json.load(fh))
 
         return True
 
     except Exception as e:
         return False
```

### Comparing `cdev-0.0.8/cdev/default/project.py` & `cdev-0.0.9/cdev/default/project.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,340 +1,357 @@
 import json
 from pydantic.types import FilePath
-from typing import Dict, List, Callable, Any, TypeVar, Tuple
+import os
+from typing import Dict, List, Any
 
-
-from cdev.constructs.project import Project, Project_State, project_info, wrap_phases
+from cdev.constructs.project import (
+    BackendError,
+    Project,
+    Project_State,
+    Project_Info,
+    wrap_phases,
+    EnvironmentDoesNotExist,
+)
+from cdev.constructs.environment import environment_info, Environment
 from cdev.default.environment import local_environment
-from core.constructs.backend import Backend, load_backend
 
+from core.constructs.backend import load_backend, Backend_Configuration
 from core.constructs.mapper import CloudMapper
 from core.constructs.components import Component
-from core.constructs.workspace import Workspace_State
-
 from core.constructs.workspace import Workspace_Info
 from core.constructs.settings import Settings_Info, Settings
 from core.constructs.cloud_output import Cloud_Output
 
-from core.utils import file_manager
+from core.utils import file_manager, paths as paths_utils
+
 
-from ..constructs.environment import environment_info, Environment
+class local_project_info(Project_Info):
+    settings_directory: str
+    initialization_module: str
 
-WORKSPACE_STATE_TO_PROJECT_STATE = {
-    Workspace_State.UNINITIALIZED: Project_State.UNINITIALIZED,
-    Workspace_State.INITIALIZING: Project_State.INITIALIZING,
-    Workspace_State.INITIALIZED: Project_State.INITIALIZED,
-}
+    def __init__(__pydantic_self__, **data: Any) -> None:
+        """"""
+        super().__init__(**data)
 
 
 class local_project(Project):
     """
     An implementation of the Project API that works for simple local development.
 
     Arguments:
-        project_info_location (FilePath): Path the configuration json file
+        project_info (local_project_info): Info of the project
+        project_info_file (FilePath): Path to save configuration file
 
     """
 
+    # Note that the class methods should not include doc strings so that they inherit the doc string of the
+    # parent class.
+
     _instance = None
 
-    _current_environment: Environment = None
     _project_info_location: FilePath = None
+    _project_info: local_project_info = None
+    _current_state: Project_State = None
+    _loaded_environment: Environment = None
 
-    _central_state: project_info
-    _backend: Backend = None
-    _project_state: Project_State = None
-    _project_name: str = None
-
-    def __new__(cls, project_info_location: FilePath):
+    def __new__(cls, project_info: local_project_info, project_info_filepath: FilePath):
         if cls._instance is None:
             cls._instance = super(Project, cls).__new__(cls)
-            # Put any initialization here.
-            cls._instance._project_info_location = project_info_location
 
-            cls._instance._load_state()
+            cls._instance._project_info_location = project_info_filepath
+            cls._instance._project_info = project_info
 
-            cls._instance.set_name(cls._instance._central_state.project_name)
-
-            cls._instance._backend = load_backend(
-                cls._instance._central_state.backend_info
-            )
-
-            # Load the backend
-            cls._instance._current_environment = None
-            
-            cls._instance.set_state(Project_State.UNINITIALIZED)
+            cls._instance.set_state(Project_State.INFO_LOADED)
 
             Project.set_global_instance(cls._instance)
 
-
         return cls._instance
 
-    @classmethod
-    def terminate_singleton(cls):
-        cls._instance = None
-
-    def initialize_project(self):
+    @wrap_phases([Project_State.INFO_LOADED])
+    def initialize_project(self) -> None:
         self.set_state(Project_State.INITIALIZING)
         current_env = self.get_current_environment()
-        
-        if current_env:
-            current_env.initialize_environment()
+        current_env.initialize_environment()
         self.set_state(Project_State.INITIALIZED)
 
-    def terminate_project(self):
-        Project.remove_global_instance(self)
-
-
-    def set_name(self, name: str):
-        """
-        Set the name of this Project
-
-        Args:
-            name (str): name of the Project
-        """
-        self._project_name = name
+    def get_name(self) -> str:
+        return self._project_info.project_name
 
+    def get_state(self) -> Project_State:
+        return self._current_state
 
-    def get_name(self):
-        """
-        Get the name of this Project
+    def set_state(self, new_state: Project_State) -> None:
+        self._current_state = new_state
 
-        Returns:
-            name (str)
-        """
-        return self._project_name
+    @wrap_phases([Project_State.INFO_LOADED])
+    def create_environment(
+        self, environment_name: str, backend_configuration: Backend_Configuration = None
+    ) -> None:
+        self._load_info()
+
+        if not backend_configuration:
+            backend_configuration = self._create_default_backend_configuration()
+
+        try:
+            resource_state_id = load_backend(
+                backend_configuration
+            ).create_resource_state(environment_name)
+        except Exception as e:
+            raise BackendError
 
-    def get_state(self) -> Project_State:
-        return self._project_state
+        base_directory = os.path.dirname(self._project_info.settings_directory)
 
-    def set_state(self, new_state: Project_State):
-        self._project_state = new_state
+        _base_settings_file = os.path.join(
+            self._project_info.settings_directory, f"base_settings.py"
+        )
+        _environment_settings_file = os.path.join(
+            self._project_info.settings_directory, f"{environment_name}_settings.py"
+        )
 
-    # Note that the class methods should not include doc strings so that they inherit the doc string of the 
-    # parent class. 
+        settings_files = [_base_settings_file, _environment_settings_file]
 
-    @wrap_phases([Project_State.INITIALIZED, Project_State.UNINITIALIZED])
-    def create_environment(self, environment_name: str, settings_files: Dict[str,str] = None):
-        self._load_state()
-        resource_state_id = self._backend.create_resource_state(environment_name)
+        [paths_utils.touch_file(x) for x in settings_files]
 
-        workspace_config = {"backend_configuration": self._central_state.backend_info}
+        user_setting_modules = [
+            # set the settings modules as python modules
+            os.path.relpath(x, start=base_directory,)[
+                :-3
+            ].replace("/", ".")
+            for x in settings_files
+        ]
 
-        workspace_config["resource_state_uuid"] = resource_state_id
-        workspace_config["initialization_module"] = "src.cdev_project"
+        _abs_secrets_dir = os.path.join(
+            self._project_info.settings_directory, f"{environment_name}_secrets"
+        )
+        paths_utils.mkdir(_abs_secrets_dir)
+        relative_secret_dir = os.path.relpath(_abs_secrets_dir, start=base_directory)
 
-            
         settings = Settings_Info(
-            base_class = "core.constructs.settings.Settings"
-        ) if not settings_files else Settings_Info(
-            base_class = "core.constructs.settings.Settings",
-            user_setting_module=settings_files.get('user_setting_module'),
-            secret_dir=settings_files.get('secret_dir'),
+            base_class="core.constructs.settings.Settings",
+            user_setting_module=user_setting_modules,
+            secret_dir=relative_secret_dir,
         )
 
-        self._central_state.environments.append(
+        self._project_info.environment_infos.append(
             environment_info(
-                environment_name,
-                Workspace_Info(
-                    "core.default.workspace", 
-                    "local_workspace", 
-                    settings,
-                    workspace_config
+                name=environment_name,
+                workspace_info=Workspace_Info(
+                    python_module="core.default.workspace",
+                    python_class="local_workspace",
+                    settings_info=settings,
+                    backend_info=backend_configuration,
+                    resource_state_uuid=resource_state_id,
+                    initialization_modules=[self._project_info.initialization_module],
                 ),
             )
         )
 
-        self._write_state()
+        self._write_info()
 
-    @wrap_phases([Project_State.INITIALIZED, Project_State.UNINITIALIZED])
+    @wrap_phases([Project_State.INFO_LOADED])
     def destroy_environment(self, environment_name: str) -> None:
-        self._load_state()
+        self._load_info()
+
+        if environment_name not in self.get_all_environment_names():
+            raise EnvironmentDoesNotExist
 
-        self._central_state.environments = [
-            x for x in self._central_state.environments if x.name != environment_name
+        self._project_info.environment_infos = [
+            x
+            for x in self._project_info.environment_infos
+            if x.name != environment_name
         ]
 
-        self._write_state()
+        self._write_info()
 
-    @wrap_phases([Project_State.INITIALIZED, Project_State.UNINITIALIZED])
+    @wrap_phases([Project_State.INFO_LOADED])
     def get_all_environment_names(self) -> List[str]:
-        self._load_state()
+        self._load_info()
 
-        return [x.name for x in self._central_state.environments]
+        return [x.name for x in self._project_info.environment_infos]
 
-    @wrap_phases([Project_State.INITIALIZED, Project_State.UNINITIALIZED])
-    def set_current_environment(self, environment_name: str):
-        self._load_state()
+    @wrap_phases([Project_State.INFO_LOADED])
+    def set_current_environment(self, environment_name: str) -> None:
+        self._load_info()
 
-        if not environment_name in self.get_all_environment_names():
-            raise Exception
+        if environment_name not in self.get_all_environment_names():
+            raise EnvironmentDoesNotExist
 
-        self._central_state.current_environment = environment_name
+        self._project_info.current_environment_name = environment_name
 
-        self._write_state()
+        self._write_info()
 
-    def get_environment(self, environment_name: str) -> Environment:
-        self._load_state()
+    @wrap_phases([Project_State.INFO_LOADED])
+    def get_environment_settings_info(
+        self, environment_name: str = None
+    ) -> Settings_Info:
+        if not environment_name:
+            environment_name = self.get_current_environment_name()
 
-        environment_info = next(
-            x for x in self._central_state.environments if x.name == environment_name
-        )
+        self._load_info()
 
-        return local_environment(environment_info)
+        environment_info = self._get_environment_info(environment_name)
 
-    def get_current_environment_name(self) -> str:
-        self._load_state()
+        return environment_info.workspace_info.settings_info
 
-        return self._central_state.current_environment
+    @wrap_phases([Project_State.INFO_LOADED])
+    def update_environment_settings_info(
+        self, new_value: Settings_Info, environment_name: str = None
+    ) -> None:
+        if not environment_name:
+            environment_name = self.get_current_environment_name()
 
-    def get_current_environment(self) -> Environment:
-        self._load_state()
+        self._load_info()
+
+        # Remove the old environment
+        previous_environment_var = self._get_environment_info(environment_name)
+        previous_environment_var.workspace_info.settings_info = new_value
 
-        if not self._central_state.current_environment:
-            return None
+        self._project_info.environment_infos = [
+            x
+            for x in self._project_info.environment_infos
+            if not x.name == environment_name
+        ]
 
-        return self.get_environment(self._central_state.current_environment)
+        self._project_info.environment_infos.append(previous_environment_var)
 
-    def _get_environment_info(self, name: str) -> environment_info:
-        self._load_state()
+        self._write_info()
 
-        lookup_dict = {x.name: x for x in self._central_state.environments}
+    @wrap_phases(
+        [
+            Project_State.INFO_LOADED,
+            Project_State.INITIALIZING,
+            Project_State.INITIALIZED,
+        ]
+    )
+    def get_current_environment_name(self) -> str:
+        self._load_info()
 
-        if not name in lookup_dict:
-            raise Exception(f"No environment with name {name}")
+        return self._project_info.current_environment_name
 
-        return lookup_dict.get(name)
+    @wrap_phases([Project_State.INITIALIZING, Project_State.INITIALIZED])
+    def get_current_environment(self) -> Environment:
+        self._load_info()
+
+        current_environment_name = self.get_current_environment_name()
+
+        if (
+            not self._loaded_environment
+            or self._loaded_environment.get_name() != current_environment_name
+        ):
+            # If there is not a currently loaded environment or the currently loaded environment is not
+            # the current environment
+            environment_info = self._get_environment_info(current_environment_name)
+            self._loaded_environment = local_environment(environment_info)
+
+        return self._loaded_environment
 
     ############################
-    ##### Settings
+    ##### Runtime Settings
     ############################
     @property
+    @wrap_phases([Project_State.INITIALIZED])
     def settings(self) -> Settings:
         return self.get_current_environment().get_workspace().settings
 
-    
     @settings.setter
-    def settings(self, value: Settings):
-        self.get_current_environment().get_workspace().settings= value
-
-
-    def get_settings_info(self, environment_name: str =  None) -> Settings_Info:
-        if not environment_name:
-            environment_name = self.get_current_environment_name()
-
-
-        self._load_state()
-        
-        if not environment_name in [x.name for x in self._central_state.environments]:
-            raise Exception(f"No environment named {environment_name}")
-
-
-        return [x for x in self._central_state.environments if x.name == environment_name][0].workspace_info.settings_info
-    
-    def update_settings_info(self, new_value: Settings_Info, environment_name: str = None):
-        if not environment_name:
-            environment_name = self.get_current_environment_name()
-            
-        self._load_state()
-
-        # Remove the old environment
-        previous_environment_var = [x for x in self._central_state.environments if x.name == environment_name][0]
-        previous_environment_var.workspace_info.settings_info = new_value
-
-
-        self._central_state.environments = [x for x in self._central_state.environments if not x.name == environment_name]
-
-        self._central_state.environments.append(previous_environment_var)
-
-        self._write_state()
+    @wrap_phases([Project_State.INITIALIZING])
+    def settings(self, value: Settings) -> None:
+        self.get_current_environment().get_workspace().settings = value
 
     #######################
     ##### Display Output
     #######################
-    def display_output(self, tag: str, output: Cloud_Output):
-        """Display the output from a Resource or Reference after a process has completed
-
-        Args:
-            tag: A key value to display with the output
-            output: The Cloud Output to render
-        """
+    @wrap_phases([Project_State.INITIALIZED])
+    def display_output(self, tag: str, output: Cloud_Output) -> None:
         self.get_current_environment().get_workspace().display_output(tag, output)
 
-
-    def render_outputs(self) -> List[Tuple[str, Any]]:
-        """Render the output associated with the Workspace
-
-        Returns:
-            List[Tuple[str, Any]]: The List of outputs with their associated tag
-        
-        """
-        return self.get_current_environment().get_workspace().render_outputs()
-
-
     #################
     ##### Mappers
     #################
-    @wrap_phases([Workspace_State.INITIALIZING])
+    @wrap_phases([Project_State.INITIALIZING])
     def add_mapper(self, mapper: CloudMapper) -> None:
         ws = self.get_current_environment().get_workspace()
         ws.add_mapper(mapper)
 
-    @wrap_phases([Workspace_State.INITIALIZING])
+    @wrap_phases([Project_State.INITIALIZING])
     def add_mappers(self, mappers: List[CloudMapper]) -> None:
         ws = self.get_current_environment().get_workspace()
         ws.add_mappers(mappers)
 
-    @wrap_phases([Workspace_State.INITIALIZED])
+    @wrap_phases([Project_State.INITIALIZED])
     def get_mappers(self) -> List[CloudMapper]:
         ws = self.get_current_environment().get_workspace()
         return ws.get_mappers()
 
-    @wrap_phases([Workspace_State.INITIALIZED])
+    @wrap_phases([Project_State.INITIALIZED])
     def get_mapper_namespace(self) -> Dict:
         ws = self.get_current_environment().get_workspace()
         return ws.get_mapper_namespace()
 
     #################
     ##### Commands
     #################
-    @wrap_phases([Workspace_State.INITIALIZING])
-    def add_command(self, command_location: str):
+    @wrap_phases([Project_State.INITIALIZING])
+    def add_command(self, command_location: str) -> None:
         ws = self.get_current_environment().get_workspace()
         ws.add_command(command_location)
 
-    @wrap_phases([Workspace_State.INITIALIZING])
-    def add_commands(self, command_locations: List[str]):
+    @wrap_phases([Project_State.INITIALIZING])
+    def add_commands(self, command_locations: List[str]) -> None:
         ws = self.get_current_environment().get_workspace()
         ws.add_commands(command_locations)
 
-    @wrap_phases([Workspace_State.INITIALIZED])
+    @wrap_phases([Project_State.INITIALIZED])
     def get_commands(self) -> List[str]:
         ws = self.get_current_environment().get_workspace()
         return ws.get_commands()
 
     #################
     ##### Components
     #################
-    @wrap_phases([Workspace_State.INITIALIZING])
-    def add_component(self, component: Component):
+    @wrap_phases([Project_State.INITIALIZING])
+    def add_component(self, component: Component) -> None:
         ws = self.get_current_environment().get_workspace()
         ws.add_component(component)
 
-    @wrap_phases([Workspace_State.INITIALIZING])
-    def add_components(self, components: List[Component]):
+    @wrap_phases([Project_State.INITIALIZING])
+    def add_components(self, components: List[Component]) -> None:
         ws = self.get_current_environment().get_workspace()
         ws.add_components(components)
 
-    @wrap_phases([Workspace_State.INITIALIZED])
+    @wrap_phases([Project_State.INITIALIZED])
     def get_components(self) -> List[Component]:
         ws = self.get_current_environment().get_workspace()
         return ws.get_components()
 
-    def _write_state(self):
+    ##########################
+    ##### Internal Helpers
+    ##########################
+    def _write_info(self) -> None:
         file_manager.safe_json_write(
-            self._central_state.dict(), self._project_info_location
+            self._project_info.dict(), self._project_info_location
         )
 
-    def _load_state(self) -> project_info:
+    def _load_info(self):
         with open(self._project_info_location, "r") as fh:
-            self._central_state = project_info(**json.load(fh))
+            self._project_info = local_project_info(**json.load(fh))
+
+    def _create_default_backend_configuration(self) -> Backend_Configuration:
+        self._load_info()
+
+        return self._project_info.default_backend_configuration
+
+    def _get_environment_info(self, environment_name: str) -> environment_info:
+        self._load_info()
+
+        rv = next(
+            (
+                x
+                for x in self._project_info.environment_infos
+                if x.name == environment_name
+            )
+        )
+
+        if not rv:
+            raise EnvironmentDoesNotExist
+
+        return rv
```

### Comparing `cdev-0.0.8/cdev/project_templates/packages/src/packages/resources.py` & `cdev-0.0.9/cdev/project_templates/packages/src/packages/resources.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,39 @@
-# Generated as part of Quick Start project template 
+# Generated as part of Quick Start project template
 
 from cdev.resources.simple.xlambda import simple_function_annotation
 
 import aurora_data_api
 import pandas
 
 from .utils import helper_function
 
+
 @simple_function_annotation("hello_world_function")
 def hello_world(event, context):
-    print('Hello from inside your Function!')
+    print("Hello from inside your Function!")
     helper_function()
 
-    return {
-        "status_code": 200,
-        "message": "Hello Outside World!"
-    }
+    return {"status_code": 200, "message": "Hello Outside World!"}
 
 
 @simple_function_annotation("hello_world_function2")
 def hello_world2(event, context):
-    print('Hello from inside your Function!')
+    print("Hello from inside your Function!")
     print(aurora_data_api)
 
-    return {
-        "status_code": 200,
-        "message": "Hello Outside World!"
-    }
+    return {"status_code": 200, "message": "Hello Outside World!"}
 
 
 @simple_function_annotation("hello_world_function3")
 def hello_world3(event, context):
-    print('Hello from inside your Function!')
+    print("Hello from inside your Function!")
     print(aurora_data_api)
     print(pandas)
 
-    return {
-        "status_code": 200,
-        "message": "Hello Outside World!"
-    }
-
+    return {"status_code": 200, "message": "Hello Outside World!"}
 
 
 @simple_function_annotation("hello_world_function4")
 def hello_world4(event, context):
 
-    return {
-        "status_code": 200,
-        "message": "Hello Outside World!"
-    }
+    return {"status_code": 200, "message": "Hello Outside World!"}
```

### Comparing `cdev-0.0.8/cdev/project_templates/power_tools/src/examples/dataclass_example.py` & `cdev-0.0.9/cdev/project_templates/power_tools/src/examples/dataclass_example.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-from aws_lambda_powertools.utilities.data_classes import event_source, APIGatewayProxyEventV2
+from aws_lambda_powertools.utilities.data_classes import (
+    event_source,
+    APIGatewayProxyEventV2,
+)
 
 
 from cdev.resources.simple.api import Api
 from cdev.resources.simple.xlambda import simple_function_annotation
 
 from cdev import Project as cdev_project
 
 myProject = cdev_project.instance()
 
 DemoApi = Api("demoapi")
 
 hello_route = DemoApi.route("/helloworld", "GET")
 
+
 @simple_function_annotation("dataclass_example", events=[hello_route.event()])
 @event_source(data_class=APIGatewayProxyEventV2)
 def lambda_handler(event: APIGatewayProxyEventV2, context):
-    if 'helloworld' in event.path and event.http_method == 'GET':
+    if "helloworld" in event.path and event.http_method == "GET":
         print("Made it here!")
```

### Comparing `cdev-0.0.8/cdev/project_templates/power_tools/src/examples/tracer_example.py` & `cdev-0.0.9/cdev/project_templates/power_tools/src/examples/tracer_example.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from aws_lambda_powertools import Tracer
 
 from cdev.resources.simple.xlambda import simple_function_annotation
 
 from src.examples.config import powertool_vars, tracer_permissions
 
 
-tracer = Tracer() # Sets service via env var
+tracer = Tracer()  # Sets service via env var
 
 
 def collect_payment(charge_id: str):
     print(f"Collected charge: {charge_id}")
 
 
-@simple_function_annotation("tracer_example", environment=powertool_vars, permissions=[tracer_permissions])
+@simple_function_annotation(
+    "tracer_example", environment=powertool_vars, permissions=[tracer_permissions]
+)
 @tracer.capture_lambda_handler
 def handler(event, context):
-    charge_id = event.get('charge_id')
+    charge_id = event.get("charge_id")
     payment = collect_payment(charge_id)
-
```

### Comparing `cdev-0.0.8/cdev/project_templates/quick_start/src/hello_world/resources.py` & `cdev-0.0.9/cdev/project_templates/quick_start/src/hello_world/resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,23 @@
-# Generated as part of Quick Start project template 
+# Generated as part of Quick Start project template
 
 from cdev.resources.simple.api import Api
 from cdev.resources.simple.xlambda import simple_function_annotation
 
 from cdev import Project as cdev_project
 
 myProject = cdev_project.instance()
 
 DemoApi = Api("demoapi")
 
 hello_route = DemoApi.route("/hello_world", "GET")
 
+
 @simple_function_annotation("hello_world_function", events=[hello_route.event()])
 def hello_world(event, context):
-    print('Hello from inside your Function!')
-
-
-    return {
-        "status_code": 200,
-        "message": "Hello Outside World!"
-    }
+    print("Hello from inside your Function!")
 
+    return {"status_code": 200, "message": "Hello Outside World!"}
 
 
 myProject.display_output("Base API URL", DemoApi.output.endpoint)
-myProject.display_output("Routes", DemoApi.output.endpoints)
+myProject.display_output("Routes", DemoApi.output.endpoints)
```

### Comparing `cdev-0.0.8/cdev/project_templates/slack_bot/src/slack_bot/resources.py` & `cdev-0.0.9/cdev/project_templates/slack_bot/src/slack_bot/resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated as part of the Slack Events project template 
+# Generated as part of the Slack Events project template
 import json
 import os
 
 from slack_sdk import signature
 from slack_sdk import WebClient
 
 from cdev.resources.simple.api import Api, route_verb
@@ -10,64 +10,63 @@
 
 from cdev import Project as cdev_project
 
 from ..project_settings import SlackBotSettings
 
 myProject = cdev_project.instance()
 
-mySettings: SlackBotSettings =  myProject.settings
+mySettings: SlackBotSettings = myProject.settings
 
 DemoApi = Api("demoapi")
 
 webhook_route = DemoApi.route("/webhook", route_verb.POST)
 
 
 env_vars = {
-    "SLACK_SECRET": mySettings.SLACK_SECRET, 
+    "SLACK_SECRET": mySettings.SLACK_SECRET,
     "SLACK_BOT_OAUTH_TOKEN": mySettings.SLACK_BOT_OAUTH_TOKEN,
 }
 
 
-signature_verifier = signature.SignatureVerifier(signing_secret=os.environ.get('SLACK_SECRET'))
-client = WebClient(token=os.environ.get('SLACK_BOT_OAUTH_TOKEN'))
+signature_verifier = signature.SignatureVerifier(
+    signing_secret=os.environ.get("SLACK_SECRET")
+)
+client = WebClient(token=os.environ.get("SLACK_BOT_OAUTH_TOKEN"))
 
-@simple_function_annotation("webhook", events=[webhook_route.event()], environment=env_vars)
+
+@simple_function_annotation(
+    "webhook", events=[webhook_route.event()], environment=env_vars
+)
 def webhook(event, context):
     # Load the info to validate the request
-    body = event.get('body')
-    timestamp = event.get('headers').get("x-slack-request-timestamp")
-    slack_signature = event.get('headers').get("x-slack-signature")
+    body = event.get("body")
+    timestamp = event.get("headers").get("x-slack-request-timestamp")
+    slack_signature = event.get("headers").get("x-slack-signature")
 
     is_valid = signature_verifier.is_valid(body, timestamp, slack_signature)
 
     if not is_valid:
         # Not a valid request from our Slack App so return 401
         return {
             "status_code": 401,
         }
 
-
     data = json.loads(event.get("body"))
     print(data)
 
     if data.get("type") == "url_verification":
-        return {
-            "status_code": 200,
-            "message": {
-                "challenge": data.get('challenge')
-            }
-        }
+        return {"status_code": 200, "message": {"challenge": data.get("challenge")}}
 
-    response_channel = data.get('event').get('channel')
+    response_channel = data.get("event").get("channel")
 
     client.chat_meMessage(
         channel=response_channel,
         text="Hello from your app! :tada:",
     )
-    
+
     return {
         "status_code": 200,
     }
 
 
 myProject.display_output("Base API URL", DemoApi.output.endpoint)
-myProject.display_output("Routes", DemoApi.output.endpoints)
+myProject.display_output("Routes", DemoApi.output.endpoints)
```

### Comparing `cdev-0.0.8/cdev/project_templates/user_auth/src/content/index.html` & `cdev-0.0.9/cdev/project_templates/user_auth/src/content/index.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -31,8 +31,8 @@
         User profile:
         <pre id="ipt-user-profile"></pre>
       </label>
     </div>
     <script src="https://cdn.auth0.com/js/auth0-spa-js/1.13/auth0-spa-js.production.js"></script>
     <script src="js/app.js"></script>
   </body>
-</html>
+</html>
```

### Comparing `cdev-0.0.8/cdev/project_templates/user_auth/src/content/js/app.js` & `cdev-0.0.9/cdev/project_templates/user_auth/src/content/js/app.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -43,15 +43,15 @@
 };
 
 
 const updateUI = async () => {
 
     const isAuthenticated = await auth0.isAuthenticated();
 
-    // Update button states 
+    // Update button states
     document.getElementById("btn-logout").disabled = !isAuthenticated;
     document.getElementById("btn-api").disabled = !isAuthenticated;
     document.getElementById("btn-login").disabled = isAuthenticated;
 
     if (isAuthenticated) {
         // If the user is authenticated, display the authentication token and user settings from Auth0
         document.getElementById("gated-content").classList.remove("hidden");
```

### Comparing `cdev-0.0.8/cdev/project_templates/user_auth/src/user_auth/resources.py` & `cdev-0.0.9/cdev/project_templates/user_auth/src/user_auth/resources.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated as part of the User Auth project template 
+# Generated as part of the User Auth project template
 import json
 
 from cdev.resources.simple.api import Api
 from cdev.resources.simple.xlambda import simple_function_annotation
 
 from cdev import Project as cdev_project
 
@@ -10,20 +10,18 @@
 
 DemoApi = Api("demoapi")
 demo_route = DemoApi.route("/demo", "GET")
 
 
 @simple_function_annotation("demo_handler", events=[demo_route.event()])
 def hello_world(event, context):
-    print('Hello from inside your Function!')
+    print("Hello from inside your Function!")
 
     return {
         "status_code": 200,
         "body": json.dumps({"message": "Hello World From The Backend!"}),
-        "headers": {
-            "content-type": "application/json"
-        } 
+        "headers": {"content-type": "application/json"},
     }
 
 
 myProject.display_output("Base API URL", DemoApi.output.endpoint)
-myProject.display_output("Routes", DemoApi.output.endpoints)
+myProject.display_output("Routes", DemoApi.output.endpoints)
```

### Comparing `cdev-0.0.8/cdev.egg-info/PKG-INFO` & `cdev-0.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,127 +1,134 @@
 Metadata-Version: 2.1
 Name: cdev
-Version: 0.0.8
+Version: 0.0.9
 Summary: CLI for cdev sdk
 Home-page: UNKNOWN
 Author: CDEV LLC
 Author-email: daniel@cdevframework.com
 License: Clear BSD
+Description: # Cdev - Serverless Development Framework
+        
+        The Cdev framework is designed to create a development environment that allows teams to harness the benefits of Serverless development by providing high level constructs and processes to reduce the friction of transitioning to Serverless development. By being built on a custom Infrastructure as Code framework, Cdev provides unique optimizations and flexibility that allows projects to start fast and scale naturally.
+        
+        [![](https://cdevframework.io/images/github_banner.png)](https://cdevframework.io)
+        
+        
+        [Website](https://cdevframework.io/) • [Docs](https://cdevframework.io/docs/) • [Slack](https://slack.com/)
+        
+        
+        ## Features
+        - [Serverless Function Parsing](https://cdevframework.io/docs/)
+        - [Optimized Dependency Management](https://cdevframework.io/docs/)
+        - [Custom Infrastructure as Code Framework](/src/core)
+        - [Designed to feel as close as possible to writing regular Python](https://cdevframework.io/docs/)
+        - [Extensible Plugin and Custom Functionality Capabilities](https://cdevframework.io/docs/)
+        
+        ## Getting Started
+        - [An Aws account and credentials](https://aws.amazon.com/)
+            - Should have the `aws cli` and then run `aws configure` to set your credenentials.
+        - Requires Python>=3.6 and pip
+        - **Highly** encourage using a python virtual environment
+        
+        Starting from an empty directory. Set up your python virtual environment and install the Cdev cli.
+        ```
+        $ python -m virtualenv .venv
+        
+        $ . ./.venv/bin/activate
+        
+        $ pip install cdev
+        ```
+        
+        Create a new project, see the resources in the created project, and create the project.
+        
+        **When creating a new project, you will be prompted to link to a `S3 Bucket` for your deployment artifacts.**
+        
+        **You will need to provide a `S3 Bucket` in your Aws Account. If you do not already have one, you can create a bucket with the following command. This bucket can be used for managing the deployment artifacts for multiple projects.**
+        ```bash
+        aws s3 mb s3://<bucket-name>
+        ```
+        
+        ```
+        $ cdev
+        
+        $ cdev init demo-project --template quick-start
+        Name of bucket to store artifacts (): <bucket-name>
+        
+        $ cdev plan
+        
+        $ cdev deploy
+        ```
+        
+        Invoke the deployed function directly from the cli
+        ```
+        $ cdev run function.execute hello_world_comp.hello_world_function
+        ```
+        
+        You might have to wait a sec for the logs to process in the cloud
+        ```
+        $ cdev run function.logs hello_world_comp.hello_world_function
+        ```
+        
+        Invoke the deployed function via the created HTTP Api
+        ```
+        $ cdev output hello_world_comp.api.demoapi.endpoint
+        <url>
+        ```
+        
+        ```
+        $ curl <url>/hello_world
+        ```
+        
+        You can also visit `<url>/hello_world` in your favorite web browser!
+        
+        Delete the Resources in the Environment
+        ```
+        $ cdev destroy
+        ```
+        
+        For a more in depth information about the capabilities of Cdev, check out our [documentation](https://staging.cdevframework.io/docs/).
+        
+        
+        ## Supported Resources
+        - Serverless Functions
+        - HTTP Endpoints
+        - S3 Buckets
+        - Dynamodb
+        - Aurora DB (Mysql and Postgres)
+        - Sqs
+        - Sns
+        - Static Site Hosting
+        
+        For guides on how to deploy any of these resources, check out our [documentation](https://cdevframework.io/docs/)
+        
+        ## Early Alpha Notes
+        The project is still in a pre-alpha state, so not all the features of the alpha are implemented. The main branch will be the most stable branch and should not have any breaking changes as work on the alpha continues. Things left to do in alpha:
+        - More unit and integration tests
+        - General polish of output
+        - General work on documentation
+        
+        For testing parts of the early alpha, it helps to start from the `resources-test` project template as that will have a bunch of preconfigured resources.
+        ```
+        $ cdev init demo --template resources-test
+        ```
+        
+        ## Post Alpha Road Map and Limitations
+        We are currently in the **very very** early stage of creating a comprehensive framework that helps teams throughout the whole cloud development process. As with any tool, it is important to understand what it is capable and **not** capable of doing. Here are a list of outstanding things that we are working (or thinking) on.
+        
+        - Remote Backend
+            - The current state of cloud resources are stored in json files. This is extremely limiting as it prevents multiple people from working on the same state at the same time. We are working on creating a DB that can used as a remote backend that will allow teams to collaborate more effectively.
+        
+        - Limited Resources and Options on Resources
+            - We are starting by focusing on a set of resource that we feel provide value while not being too complex. We have plans to add more resource and customization as time goes on. [Our custom Infrastructure as Code framework](/src/core) provides the flexibility to deploy any resource on any cloud, but we have to put in work to generate the configurations to talk to different clouds. In the future, we hope to support a large number of Aws and non Aws resources through standardized cloud API's like the [Aws Cloud Control API](https://aws.amazon.com/cloudcontrolapi/).
+        
+        - The Framework is Python Only
+            - We started out with building the sdk in python first because that is the language we know best. We want the sdk to feel natural in whatever language is being used, which will require adding expertise to our team from other ecosystems. The underlying primitives that make up the framework are language agnostic, so we hope to one day support a wide range of languages.
+        
+        - Can I export my project to an industry standard tool like Aws Cloudformation or Terraform?
+            - We understand the benefits that come from avoiding lock-in by providing the ability to interpolate with the industry standard tools. We currently provision all resources with our custom [Infrastructure as Code Framework](/src/core) and store the state of the resources in local json files, which makes created projects not compatible with other tools. We felt that with building our own framework, we could explore new optimizations and ideas that could improve the developer experience. With some work, it is possible to make our framework work with and compatible with other Infrastructure as Code Frameworks, and we will be investigating this work as we move forward.
+        
+        
+        If you are interested in any of the challenges that we are working on or have expertise you think is missing in our project, please consider [applying for a job on our team](https://cdevframework.io/docs/).
+        
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-
-# Cdev - Serverless Development Framework
-
-The Cdev framework is designed to create a development environment that allows teams to harness the benefits of Serverless development by providing high level constructs and processes to reduce the friction of transitioning to Serverless development. By being built on a custom Infrastructure as Code framework, Cdev provides unique optimizations and flexibility that allows projects to start fast and scale naturally. 
-
-[![](https://cdevframework.io/images/github_banner.png)](https://cdevframework.io)
-
-
-[Website](https://cdevframework.io/) • [Docs](https://cdevframework.io/docs/) • [Slack](https://slack.com/)
-
-
-## Features
-- [Serverless Function Parsing](https://cdevframework.io/docs/)
-- [Optimized Dependency Management](https://cdevframework.io/docs/)
-- [Custom Infrastructure as Code Framework](/src/core)
-- [Designed to feel as close as possible to writing regular Python](https://cdevframework.io/docs/)
-- [Extensible Plugin and Custom Functionality Capabilities](https://cdevframework.io/docs/)
-
-## Getting Started 
-- [An Aws account and credentials](https://aws.amazon.com/)
-    - Should have the `aws cli` and then run `aws configure` to set your credenentials. 
-- Requires Python>=3.6 and pip
-- **Highly** encourage using a python virtual environment
-
-Starting from an empty directory. Set up your python virtual environment and install the Cdev cli. 
-```
-$ python -m virtualenv .venv
-
-$ . ./.venv/bin/activate
-
-$ pip install cdev
-```
-
-Create a new project, see the resources in the created project, and create the project
-```
-$ cdev
-
-$ cdev init demo-project --template quick-start
-
-$ cdev plan
-
-$ cdev deploy
-```
-
-Invoke the deployed function directly from the cli
-```
-$ cdev run function.execute hello_world_comp.hello_world_function
-```
-
-You might have to wait a sec for the logs to process in the cloud
-```
-$ cdev run function.logs hello_world_comp.hello_world_function
-```
-
-Invoke the deployed function via the created HTTP Api
-```
-$ cdev output hello_world_comp.api.demoapi.endpoint
-<url>
-```
-
-```
-$ curl <url>/hello_world
-```
-
-You can also visit `<url>/hello_world` in your favorite web browser!
-
-Delete the Resources in the Environment
-```
-$ cdev destroy
-```
-
-For a more in depth information about the capabilities of Cdev, check out our [documentation](https://staging.cdevframework.io/docs/).
-
-
-## Supported Resources
-- Serverless Functions
-- HTTP Endpoints
-- S3 Buckets
-- Dynamodb
-- Aurora DB (Mysql and Postgres)
-- Sqs
-- Sns
-- Static Site Hosting
-
-For guides on how to deploy any of these resources, check out our [documentation](https://cdevframework.io/docs/)
-
-## Early Alpha Notes
-The project is still in a pre-alpha state, so not all the features of the alpha are implemented. The main branch will be the most stable branch and should not have any breaking changes as work on the alpha continues. The alpha will be ready for a public launch by March 1st. Things left to do in alpha:
-- More unit and integration tests
-- General polish of output 
-- General work on documentation
-
-For testing parts of the early alpha, it helps to start from the `resources-test` project template as that will have a bunch of preconfigured resources.
-```
-$ cdev init demo --template resources-test
-```
-
-## Post Alpha Road Map and Limitations
-We are currently in the **very very** early stage of creating a comprehensive framework that helps teams throughout the whole cloud development process. As with any tool, it is important to understand what it is capabale and **not** capable of doing. Here are a list of outstanding things that we are working (or thinking) on. 
-
-- Remote Backend
-    - The current state of cloud resources are stored in json files. This is extremely limiting as it prevents multiple people from working on the same state at the same time. We are working on creating a DB that can used as a remote backend that will allow teams to collaborate more effectively.
-
-- Limited Resources and Options on Resources
-    - We are starting by focusing on a set of resource that we feel provide value while not being too complex. We have plans to add more resource and customization as time goes on. [Our custom Infrastructure as Code framework](/src/core) provides the flexibility to deploy any resource on any cloud, but we have to put in work to generate the configurations to talk to different clouds. In the future, we hope to support a large number of Aws and non Aws resources through standardized cloud API's like the [Aws Cloud Control API](https://aws.amazon.com/cloudcontrolapi/). 
-
-- The Framework is Python Only
-    - We started out with building the sdk in python first because that is the language we know best. We want the sdk to feel natural in whatever language is being used, which will require adding expertise to our team from other ecosystems. The underlying primitives that make up the framework are language agnostic, so we hope to one day support a wide range of languages.
-
-- Can I export my project to an industry standard tool like Aws Cloudformation or Terraform?
-    - We understand the benefits that come from avoiding lock-in by providing the ability to interpolate with the industry standard tools. We currently provision all resources with our custom [Infrastructure as Code Framework](/src/core) and store the state of the resources in local json files, which makes created projects not compatible with other tools. We felt that with building our own framework, we could explore new optimizations and ideas that could improve the developer experience. With some work, it is possible to make our framework work with and compatible with other Infrastructure as Code Frameworks, and we will be investigating this work as we move forward. 
-
-
-If you are interested in any of the challenges that we are working on or have expertise you think is missing in our project, please consider [applying for a job on our team](https://cdevframework.io/docs/).
-
-
```

### Comparing `cdev-0.0.8/cdev.egg-info/SOURCES.txt` & `cdev-0.0.9/cdev.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 MANIFEST.in
+README.md
 setup.py
 ./cdev/scripts/cdev
 ./core/scripts/cdev_core
 cdev/__init__.py
 cdev.egg-info/PKG-INFO
 cdev.egg-info/SOURCES.txt
 cdev.egg-info/dependency_links.txt
@@ -12,18 +13,19 @@
 cdev/cli/__main__.py
 cdev/cli/logger.py
 cdev/commands/__init__.py
 cdev/commands/cloud_output.py
 cdev/commands/deploy.py
 cdev/commands/destroy.py
 cdev/commands/environment.py
-cdev/commands/initializer.py
 cdev/commands/local_development.py
 cdev/commands/plan.py
+cdev/commands/project_initializer.py
 cdev/commands/run.py
+cdev/commands/sync.py
 cdev/constructs/__init__.py
 cdev/constructs/environment.py
 cdev/constructs/project.py
 cdev/default/__init__.py
 cdev/default/cloudmapper.py
 cdev/default/components.py
 cdev/default/environment.py
@@ -41,14 +43,15 @@
 cdev/project_templates/power_tools/src/examples/dataclass_example.py
 cdev/project_templates/power_tools/src/examples/logging_example.py
 cdev/project_templates/power_tools/src/examples/metrics_example.py
 cdev/project_templates/power_tools/src/examples/middleware_example.py
 cdev/project_templates/power_tools/src/examples/tracer_example.py
 cdev/project_templates/quick_start/src/__init__.py
 cdev/project_templates/quick_start/src/cdev_project.py
+cdev/project_templates/quick_start/src/hello_world/__init__.py
 cdev/project_templates/quick_start/src/hello_world/resources.py
 cdev/project_templates/quick_start_twilio/requirements.txt
 cdev/project_templates/quick_start_twilio/src/__init__.py
 cdev/project_templates/quick_start_twilio/src/cdev_project.py
 cdev/project_templates/quick_start_twilio/src/link_bot/api.py
 cdev/project_templates/quick_start_twilio/src/link_bot/handlers.py
 cdev/project_templates/resources_test/src/__init__.py
@@ -86,28 +89,30 @@
 core/commands/cloud_output.py
 core/commands/create_resource_state.py
 core/commands/create_workspace.py
 core/commands/deploy_differences.py
 core/commands/execute_frontend.py
 core/commands/initialize_workspace.py
 core/commands/run.py
+core/commands/sync.py
 core/constructs/__init__.py
 core/constructs/backend.py
 core/constructs/backend_exceptions.py
 core/constructs/cloud_output.py
 core/constructs/commands.py
 core/constructs/components.py
 core/constructs/mapper.py
 core/constructs/models.py
 core/constructs/output_manager.py
 core/constructs/resource.py
 core/constructs/resource_state.py
 core/constructs/settings.py
 core/constructs/types.py
 core/constructs/workspace.py
+core/constructs/workspace_watcher.py
 core/default/__init__.py
 core/default/backend.py
 core/default/cloudmapper.py
 core/default/components.py
 core/default/workspace.py
 core/default/commands/__init__.py
 core/default/commands/bucket/__init__.py
@@ -120,14 +125,15 @@
 core/default/commands/function/utils.py
 core/default/commands/relationaldb/__init__.py
 core/default/commands/relationaldb/shell.py
 core/default/commands/relationaldb/utils.py
 core/default/commands/static_site/__init__.py
 core/default/commands/static_site/sync.py
 core/default/commands/static_site/utils.py
+core/default/commands/static_site/watcher.py
 core/default/commands/table/__init__.py
 core/default/commands/table/clear_table.py
 core/default/commands/table/put_items.py
 core/default/commands/table/utils.py
 core/default/mappers/__init__.py
 core/default/mappers/aws_client.py
 core/default/mappers/simple/__init__.py
@@ -150,32 +156,62 @@
 core/default/resources/simple/queue.py
 core/default/resources/simple/relational_db.py
 core/default/resources/simple/static_site.py
 core/default/resources/simple/table.py
 core/default/resources/simple/topic.py
 core/default/resources/simple/xlambda.py
 core/utils/__init__.py
+core/utils/cache.py
 core/utils/command_finder.py
 core/utils/exceptions.py
 core/utils/file_manager.py
 core/utils/hasher.py
 core/utils/logger.py
 core/utils/module_loader.py
+core/utils/operations.py
 core/utils/paths.py
 core/utils/platforms.py
 core/utils/topological_helper.py
 core/utils/fs_manager/__init__.py
-core/utils/fs_manager/docker_package_builder.py
-core/utils/fs_manager/external_dependencies_index.py
 core/utils/fs_manager/finder.py
-core/utils/fs_manager/package_mananger.py
-core/utils/fs_manager/utils.py
+core/utils/fs_manager/handler_optimizer.py
+core/utils/fs_manager/module_types.py
+core/utils/fs_manager/package_manager.py
+core/utils/fs_manager/package_optimizer.py
+core/utils/fs_manager/serverless_function_optimizer.py
 core/utils/fs_manager/writer.py
-core/utils/fs_manager/standard_library_names/python_3_6
 core/utils/fs_manager/standard_library_names/python_3_7
 core/utils/fs_manager/standard_library_names/python_3_8
 core/utils/fs_manager/standard_library_names/python_3_9
 serverless_parser/__init__.py
 serverless_parser/parser.py
 serverless_parser/parser_exceptions.py
 serverless_parser/parser_objects.py
-serverless_parser/parser_utils.py
+serverless_parser/parser_utils.py
+tests/__init__.py
+tests/core/__init__.py
+tests/core/sample_data.py
+tests/core/constructs/__init__.py
+tests/core/constructs/backend.py
+tests/core/constructs/mapper.py
+tests/core/constructs/test_output.py
+tests/core/constructs/test_workspace.py
+tests/core/default/__init__.py
+tests/core/default/conftest.py
+tests/core/default/test_dependency_index.py
+tests/core/default/test_fs_manager.py
+tests/core/default/test_localbackend.py
+tests/core/default/test_localworkspace.py
+tests/core/default/data/__init__.py
+tests/core/default/data/example_init.py
+tests/core/utils/__init__.py
+tests/core/utils/conftest.py
+tests/core/utils/test_file_manager.py
+tests/core/utils/test_handler_optimizer.py
+tests/core/utils/test_hasher.py
+tests/core/utils/test_package_manager_api.py
+tests/core/utils/test_package_manager_helpers.py
+tests/core/utils/test_package_optomizer_helpers.py
+tests/core/utils/test_paths.py
+tests/core/utils/test_topo_helper.py
+tests/visual/__init__.py
+tests/visual/output_manager.py
```

### Comparing `cdev-0.0.8/core/cli/__main__.py` & `cdev-0.0.9/core/cli/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 from ..commands import (
     create_workspace,
     initialize_workspace,
     run,
     execute_frontend,
     create_resource_state,
-    cloud_output
+    cloud_output,
 )
 from ..constructs.workspace import Workspace
 
-parser = argparse.ArgumentParser(description="cdev cli")
+parser = argparse.ArgumentParser(description="cdev core cli")
 subparsers = parser.add_subparsers(title="sub_command", description="valid subcommands")
 
 
 def wrap_initialize_workspace(command: Callable) -> Callable[[Any], Any]:
     def wrapped_caller(args):
         try:
 
@@ -51,16 +51,16 @@
             create_resource_state.create_resource_state_cli
         ),
         "args": [],
     },
     {
         "name": "output",
         "help": "See the generated cloud output",
-        "default": wrap_initialize_workspace(cloud_output.cloud_output_command_cli)
-    }, 
+        "default": wrap_initialize_workspace(cloud_output.cloud_output_command_cli),
+    },
     {
         "name": "run",
         "help": "This command is used to run user defined and resource functions.",
         "default": wrap_initialize_workspace(run.run_command),
         "args": [
             {"dest": "subcommand", "help": "the user defined command to call"},
             {"dest": "args", "nargs": argparse.REMAINDER},
@@ -69,39 +69,44 @@
 ]
 
 
 def subcommand_function_wrapper(name, subcommand):
     # This wraps a function so that is can be used for subcommands by basing the subcommand as the first arg to the function
     # then the remaining args as the second arg
     def inner(args):
-
         return command(subcommand, args)
 
     return inner
 
 
-def add_general_output_options(parser: argparse.ArgumentParser):
+def add_general_output_options(parser: argparse.ArgumentParser) -> None:
     parser.add_argument(
         "--output",
         type=str,
         choices=["json", "plain-text", "rich"],
         help="change the type of output generated",
     )
 
     parser.add_argument(
-        '-d', '--debug',
+        "-d",
+        "--debug",
         help="Print debug log statements. This is mostly for development use",
-        action="store_const", dest="loglevel", const=logging.DEBUG,
+        action="store_const",
+        dest="loglevel",
+        const=logging.DEBUG,
         default=logging.WARNING,
     )
 
     parser.add_argument(
-        '-v', '--verbose',
+        "-v",
+        "--verbose",
         help="Print info log message. Use this to get a more detailed understanding of what is executing.",
-        action="store_const", dest="loglevel", const=logging.INFO,
+        action="store_const",
+        dest="loglevel",
+        const=logging.INFO,
     )
 
 
 for command in CDEV_COMMANDS:
     tmp = subparsers.add_parser(command.get("name"), help=command.get("help"))
 
     if command.get("subcommands"):
```

### Comparing `cdev-0.0.8/core/commands/cloud_output.py` & `cdev-0.0.9/core/commands/cloud_output.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,60 @@
-
-from ..constructs.workspace import Workspace
-from ..constructs.output_manager import OutputManager
+from core.constructs.workspace import Workspace
+from core.constructs.output_manager import OutputManager
 
 from core.utils.logger import log
 
-def cloud_output_command_cli(args):
+
+def cloud_output_command_cli(args) -> None:
     config = args[0]
     cloud_output_command(config)
 
 
-def cloud_output_command(workspace: Workspace, output: OutputManager, cloud_output_id: str, only_value: bool):
+def cloud_output_command(
+    workspace: Workspace,
+    output: OutputManager,
+    cloud_output_id: str,
+    only_value: bool = False,
+) -> None:
+    """Command to get the Cloud Output values from a given id.
+
+    Args:
+        workspace (Workspace): The Workspace that the command is executed within.
+        output (OutputManager): object to pass all output to.
+        cloud_output_id (str): Id of the output to get <component>.<ruuid>.<cdev_name>.<output_key>
+        only_value (bool): Output only the value. Helpful for shell scripting.
+
+    Raises:
+        Exception
+    """
     log.debug("Executing Frontend")
 
-   
-
-    split_names = cloud_output_id.split('.')
-
-    if not len(split_names) == 4:
-        raise Exception("Output not provided in correct structure. ex: <component>.<ruuid>.<cdev_name>.<output_key>")
+    split_names = cloud_output_id.split(".")
 
+    if len(split_names) != 4:
+        raise Exception(
+            "Output not provided in correct structure. ex: <component>.<ruuid>.<cdev_name>.<output_key>"
+        )
 
     component_name = split_names[0]
     resource_ruuid = f"cdev::simple::{split_names[1]}"
     resource_name = split_names[2]
     output_key = split_names[3]
 
-
     try:
         cloud_output = workspace.get_backend().get_cloud_output_by_name(
             workspace.get_resource_state_uuid(),
             component_name,
             resource_ruuid,
-            resource_name
+            resource_name,
         )
     except Exception as e:
         print(e)
         raise e
 
-
-    if not output_key in cloud_output:
+    if output_key not in cloud_output:
         raise Exception(f"Key {output_key} not in Cloud Output {cloud_output}")
 
-
     if not only_value:
         print(f"{output_key} -> {cloud_output.get(output_key)}")
     else:
-        print(cloud_output.get(output_key))
+        print(cloud_output.get(output_key))
```

### Comparing `cdev-0.0.8/core/commands/create_workspace.py` & `cdev-0.0.9/core/commands/create_workspace.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 """Utilities for creating a new resource state
 
 """
 import os
 
 from core.constructs import workspace as cdev_workspace
-from core.constructs.backend import Backend_Configuration
 from core.constructs.settings import Settings_Info
 
 from core.default.workspace import local_workspace_manager
 
 
-def create_workspace(args):
+def create_workspace() -> None:
+    """Create a workspace initialization info at the current working directory."""
     base_project_dir = os.getcwd()
     manager = local_workspace_manager(base_project_dir)
 
     if manager.check_if_workspace_exists():
         print("Workspace already initialized")
+        return
 
     workspace_info = cdev_workspace.Workspace_Info(
         "core.default.workspace",
         "local_workspace",
-        Settings_Info(
-            base_class="core.constructs.settings.Settings"
-        ),
+        Settings_Info(base_class="core.constructs.settings.Settings"),
         {
             "backend_configuration": {
                 "python_module": "core.default.backend",
                 "python_class": "LocalBackend",
                 "config": {
                     "base_folder": base_project_dir,
                     "central_state_file": "centralstate.json",
                 },
             },
             "initialization_file": "cdev_project",
-
         },
     )
 
     manager.create_new_workspace(workspace_info)
-
-    return
```

### Comparing `cdev-0.0.8/core/commands/deploy_differences.py` & `cdev-0.0.9/core/commands/deploy_differences.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-"""Utilities for creating a deploying a set of changes 
+"""Utilities for creating a deploying a set of changes
 
 """
+from typing import Optional
 
 from core.constructs.output_manager import OutputManager
-from ..constructs.workspace import Workspace, Workspace_State
+from core.constructs.workspace import Workspace, Workspace_State
 from rich.prompt import Confirm
 from .execute_frontend import execute_frontend
 
-import networkx as nx
 
+def execute_deployment_cli(args) -> None:
 
-def execute_deployment_cli(args):
+    workspace = Workspace.instance()
+    execute_deployment(workspace, OutputManager())
 
-    WORKSPACE = Workspace.instance()
 
-    execute_deployment(WORKSPACE, OutputManager())
+def execute_deployment(workspace: Workspace, output: OutputManager, no_prompt: Optional[bool] = False) -> None:
+    """Execute the process for a deployment. This includes generating the current frontend representation of the desired resources.
+    Then after confirmation, deploy any needed changes.
 
-
-
-def execute_deployment(workspace: Workspace, output: OutputManager):
+    Args:
+        workspace (Workspace): Workspace to execute the process within.
+        output (OutputManager): Output manager for sending messages to the console.
+    """
     unsorted_differences = execute_frontend(workspace, output)
 
     if not unsorted_differences:
         return
 
     differences_structured = workspace.sort_differences(unsorted_differences)
 
-    print("")
-    do_deployment = Confirm.ask("Do you want to deploy differences?")
+    if not no_prompt:
+        print("")
+        do_deployment = Confirm.ask("Do you want to deploy differences?")
 
-    if not do_deployment:
-        return
+        if not do_deployment:
+            return
 
     workspace.set_state(Workspace_State.EXECUTING_BACKEND)
-
     workspace.deploy_differences(differences_structured)
 
-
-    
-
     for tag, cloud_output in workspace.render_outputs():
         print(f"{tag} -> {cloud_output}")
```

### Comparing `cdev-0.0.8/core/commands/execute_frontend.py` & `cdev-0.0.9/core/commands/execute_frontend.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,48 +9,65 @@
 from ..constructs.output_manager import OutputManager
 
 from core.utils.logger import log
 
 
 def execute_frontend_cli(args):
 
-    WORKSPACE = Workspace.instance()
-
+    workspace = Workspace.instance()
     output_manager = OutputManager()
 
-
-    
-    execute_frontend(WORKSPACE, output_manager)
+    execute_frontend(workspace, output_manager)
 
 
-
-def execute_frontend(workspace: Workspace, output: OutputManager, previous_component_names: List[str]=None) -> Tuple[List[Component_Difference], List[Resource_Difference], List[Resource_Reference_Difference]]:
+def execute_frontend(
+    workspace: Workspace,
+    output: OutputManager,
+    previous_component_names: List[str] = None,
+) -> Tuple[
+    List[Component_Difference],
+    List[Resource_Difference],
+    List[Resource_Reference_Difference],
+]:
+    """Execute the Frontend process to generate the current set of differences between the desired resources and current deployed versions.
+
+    Args:
+        workspace (Workspace): Workspace to execute the process within.
+        output (OutputManager): Output manager for sending messages to the console.
+        previous_component_names (List[str], optional): components to diff against. Defaults to None.
+
+    Returns:
+        Tuple[ List[Component_Difference], List[Resource_Difference], List[Resource_Reference_Difference], ]: _description_
+    """
 
     log.debug("Executing Frontend")
 
     workspace.set_state(Workspace_State.EXECUTING_FRONTEND)
     current_state = workspace.generate_current_state()
 
-
     output.print_local_state(current_state)
 
     if not previous_component_names:
-        diff_previous_component_names = [x.name for x in workspace.get_backend().get_resource_state(workspace.get_resource_state_uuid()).components]
+        diff_previous_component_names = [
+            x.name
+            for x in workspace.get_backend()
+            .get_resource_state(workspace.get_resource_state_uuid())
+            .components
+        ]
     else:
         diff_previous_component_names = previous_component_names
 
-    
     output.print_components_to_diff_against(diff_previous_component_names)
 
-    differences = workspace.create_state_differences(current_state, diff_previous_component_names)
+    differences = workspace.create_state_differences(
+        current_state, diff_previous_component_names
+    )
 
-
-    if any(x for x in differences):
+    if any(differences):
         output.print_state_differences(differences)
-
     else:
+        differences = None
         print("No Differences")
-        return None
 
     log.debug("Finish Executing Frontend")
-    
+
     return differences
```

### Comparing `cdev-0.0.8/core/commands/initialize_workspace.py` & `cdev-0.0.9/core/commands/initialize_workspace.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,21 @@
 """Utilities for initializing the workspace
 
 """
 
 
 import os
 
-from ..constructs.workspace import Workspace_Info
+from core.constructs.workspace import Workspace_Info, load_and_initialize_workspace
+from core.default.workspace import local_workspace_manager
 
-from ..constructs.workspace import load_and_initialize_workspace
-from ..default.workspace import local_workspace_manager
 
-
-def initialize_workspace_cli(args):
+def initialize_workspace_cli(args) -> None:
 
     workspace_manager = local_workspace_manager(os.getcwd())
-
     workspace_config = workspace_manager.load_workspace_configuration()
+    initialize_workspace(workspace_config)
 
-    try:
-        initialize_workspace(workspace_config)
-    except Exception as e:
-        raise e
 
+def initialize_workspace(workspace_config: Workspace_Info) -> None:
 
-def initialize_workspace(workspace_config: Workspace_Info):
-
-    try:
-        load_and_initialize_workspace(workspace_config)
-    except Exception as e:
-        raise e
+    load_and_initialize_workspace(workspace_config)
```

### Comparing `cdev-0.0.8/core/commands/run.py` & `cdev-0.0.9/core/commands/run.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,43 @@
-"""Utilities for running custom scripts 
+"""Utilities for running custom scripts
 
 """
 
 
-from ..constructs.commands import BaseCommand, BaseCommandContainer
-from ..constructs.workspace import Workspace
-from ..constructs.output_manager import OutputManager
+from argparse import Namespace
+from core.constructs.workspace import Workspace
+from core.constructs.output_manager import OutputManager
 
 
-def execute_run_cli(args):
+def execute_run_cli(args) -> None:
     ws = Workspace.instance()
-    
+
     output_manager = OutputManager()
 
     run_command(ws, output_manager, args)
 
 
-def run_command(workspace: Workspace, output: OutputManager, cli_args):
-    """
-    Attempts to find and run a user defined command
+def run_command(
+    workspace: Workspace, output: OutputManager, cli_args: Namespace
+) -> None:
+    """Attempts to find and run a user defined command.
 
     format:
     cdev run <sub_command> <args>
+
+    Args:
+        workspace (Workspace): Workspace to execute the process within.
+        output (OutputManager): Output manager for sending messages to the console.
+        cli_args (Namespace): Arguments for the command.
     """
     # Convert namespace into dict
     params = vars(cli_args)
 
     # This is the command to run... It can be a single command or a path to the command where the path is '.' delimitated
     sub_command = params.get("subcommand")
     command_args = params.get("args") if params.get("args") else []
 
-    
     try:
         workspace.execute_command(sub_command, command_args)
     except Exception as e:
         print(e)
         return
```

### Comparing `cdev-0.0.8/core/constructs/backend.py` & `cdev-0.0.9/core/constructs/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 """Definition of the functionality of a Backend within the framework
 
 A Backend is designed to be the single central place for persistent storage within the framework. It is responsible
 for managing all changes within the state of a project. The backend touches almost all other primitives within
 the framework. To gain a better understanding of its larger role with the framework, refer to the documentation
 about the design of the framework (link).
 
-This file provides the definition of the functionality a backend should implement, but it does not provide 
-a concrete implementation. 
+This file provides the definition of the functionality a backend should implement, but it does not provide
+a concrete implementation.
 
-This file also contains the definition of how to configure and dynamically load a backend class. To denote a 
+This file also contains the definition of how to configure and dynamically load a backend class. To denote a
 concrete implementation, a python `module` and `class` must be provide. These should both be strings. They are
-used to load a class that inherits from the base `Backend` class. It also takes in a generic dictionary to be 
-passed as configuration into the dynamicall loaded class.
+used to load a class that inherits from the base `Backend` class. It also takes in a generic dictionary to be
+passed as configuration into the dynamically loaded class.
 
 """
 import inspect
-from typing import Dict, Tuple, Any, List
+from typing import Dict, Tuple, Any, List, Callable, Optional
 from pydantic import BaseModel
 
 from .components import Component_Difference, ComponentModel
 
 from .resource import Resource_Reference_Difference, ResourceModel, Resource_Difference
 from .resource_state import Resource_State
 
-from ..utils.module_loader import import_module
+from core.utils.module_loader import import_module
 
 
 class Backend_Configuration(BaseModel):
     python_module: str
     python_class: str
     config: Dict
 
@@ -72,15 +72,15 @@
 
         Raises:
             ResourceStateAlreadyExists
 
         """
         raise NotImplementedError
 
-    def delete_resource_state(self, resource_state_uuid: str):
+    def delete_resource_state(self, resource_state_uuid: str) -> None:
         """
         Delete a resource state within this store state.
 
         Args:
             resource_state_uuid (str): The uuid of the resource state to delete
 
         Raises:
@@ -110,15 +110,14 @@
 
         Raises:
             ResourceStateDoesNotExist
 
         """
         raise NotImplementedError
 
-
     def get_component(
         self, resource_state_uuid: str, component_name: str
     ) -> ComponentModel:
         """
         Get a component from the resource state.
 
         Args:
@@ -130,34 +129,32 @@
 
         Raises:
             ResourceStateDoesNotExist
             ComponentDoesNotExist
         """
         raise NotImplementedError
 
-
     def update_component(
         self, resource_state_uuid: str, component_difference: Component_Difference
-    ):
-        """Make an update to the component. 
+    ) -> None:
+        """Make an update to the component.
 
         Args:
             resource_state_uuid (str): The resource state that the change is in.
             component_difference (Component_Difference): The difference in the component to be made.
 
         Raises:
             ResourceStateDoesNotExist
             ComponentDoesNotExist
         """
         pass
 
-
     def get_component_uuid(self, resource_state_uuid: str, component_name: str) -> str:
         """
-        Get the unique namespace for this resource state and component. 
+        Get the unique namespace for this resource state and component.
 
         Args:
             resource_state_uuid (str): The resource state that this component will be in.
             component_name (str): Name of the component
 
         Raises:
             ResourceStateDoesNotExist
@@ -182,42 +179,42 @@
             resource_state_uuid (str): The resource state for this resource change.
             component_name (str): The component this resource change is occuring in.
             diff (Resource_Difference): The desired change in the resource.
 
         Returns:
             transaction_token (str): The transaction token to be used by the mapper when deploying the resource. This token can be used to give to a cloud
             provider as a idempotency token.
-            namespace_token (str): A suffix that can be added to deployed cloud resources that acts as a namespace for the resource within the cloud. 
+            namespace_token (str): A suffix that can be added to deployed cloud resources that acts as a namespace for the resource within the cloud.
 
         Raises:
             ResourceStateDoesNotExist
             ComponentDoesNotExist
         """
         raise NotImplementedError
 
     def complete_resource_change(
         self,
         resource_state_uuid: str,
         component_name: str,
         diff: Resource_Difference,
         transaction_token: str,
         cloud_output: Dict,
-        resolved_cloud_information: Dict={}
-    ):
+        resolved_cloud_information: Dict = {},
+    ) -> None:
         """
         Notify the resource state that all changes to a resource have completed successfully. This will cause the resource to
         update the state of the resource to the new state.
 
         Args:
             resource_state_uuid (str): The resource state for this resource change.
             component_name (str): The component this resource change is occuring in.
             diff (Resource_Difference): The desired change in the resource
             transaction_token (str): Identifying token representing what transaction is being completed
             cloud_output (Dict): Output information from the cloud provider
-            resolved_cloud_information (Dict): Information that was resolved from the cloud output of the component to deploy this change. 
+            resolved_cloud_information (Dict): Information that was resolved from the cloud output of the component to deploy this change.
 
 
         Raises:
             ResourceChangeTransactionDoesNotExist
             ComponentDoesNotExist
 
         """
@@ -226,15 +223,15 @@
     def fail_resource_change(
         self,
         resource_state_uuid: str,
         component_name: str,
         diff: Resource_Difference,
         transaction_token: str,
         failed_state: Dict,
-    ):
+    ) -> None:
         """
         Notify the resource state that an attempted change to a resource has failed. The provided failed state should encapsulate any needed information
         for a future mapper to recover the state of the resource back into a proper state.
 
         Args:
             resource_state_uuid (str): The resource state for this resource change.
             component_name (str): The component this resource change is occuring in.
@@ -251,15 +248,15 @@
     # Api for getting references from other components
     # Components can have references to resources that are managed in other components and it is the responsibility of the backend to resolve those references
     # The backend should be in charge of handling IAM to determine if resolving the reference is possible
     def resolve_reference_change(
         self,
         resource_state_uuid: str,
         diff: Resource_Reference_Difference,
-    ):
+    ) -> None:
         """
         Either reference or dereference a resource from a different component.
 
         Args:
             resource_state_uuid (str): The resource state for this resource change.
             component_name (str): The component this resource change is occuring in.
             diff (Resource_Difference): The desired change in the resource
@@ -271,15 +268,15 @@
 
     # Api for working with a resource states failed resource updates
     # We can either update the failed state by the mapper attempting to fix the underlying issue, or
     # We can recover the resource to either the new state or previous state by the mapper fixing the issues, or
     # We can just delete the failure from our failed state (not recommended unless you know what you are doing because it can leave resources in the cloud)
     def change_failed_state_of_resource_change(
         self, resource_state_uuid: str, transaction_token: str, new_failed_state: Dict
-    ):
+    ) -> None:
         """
         Update the failed state of a 'resource change'.
 
         Args:
             resource_state_uuid (str): The resource state that this transaction is in.
             transaction_token (str): Identifying token for the failed transaction.
             new_failed_state (Dict): The new failed state of the transaction.
@@ -292,15 +289,15 @@
         raise NotImplementedError
 
     def recover_failed_resource_change(
         self,
         resource_state_uuid: str,
         transaction_token: str,
         to_previous_state: bool = True,
-    ):
+    ) -> None:
         """
         Recover the state of the change back to the previous state or forward to the new state. Note this will result in the failed resource change being removed from the stored state.
 
         Args:
             resource_state_uuid (str): The resource state that this transaction is in.
             transaction_token (str): Identifying token for the failed transaction.
             to_previous_state (bool): Bool to decide if the resource should be transitioned to the previous state or new state.
@@ -310,15 +307,15 @@
             ComponentDoesNotExist
             ResourceChangeTransactionDoesNotExist
         """
         raise NotImplementedError
 
     def remove_failed_resource_change(
         self, resource_state_uuid: str, transaction_token: str
-    ):
+    ) -> None:
         """
         Completely remove the failed resource change from the stored state. Note that this should be used with caution as it can lead to hanging cloud resources.
 
         Args:
             resource_state_uuid (str): The resource state that this transaction is in.
             transaction_token (str): Identifying token for the failed transaction.
 
@@ -399,15 +396,14 @@
             ComponentDoesNotExist
             CloudOutputDoesNotExist
             KeyNotInCloudOutput
 
         """
         raise NotImplementedError
 
-
     def get_cloud_output_by_name(
         self,
         resource_state_uuid: str,
         component_name: str,
         resource_type: str,
         resource_name: str,
     ) -> Dict:
@@ -465,15 +461,17 @@
     # the actual cdev resources.
     def create_differences(
         self,
         resource_state_uuid: str,
         new_components: List[ComponentModel],
         old_components: List[str],
     ) -> Tuple[
-        Component_Difference,  Resource_Difference, Resource_Reference_Difference,
+        Component_Difference,
+        Resource_Difference,
+        Resource_Reference_Difference,
     ]:
         """
         Create the set of differences from a proposed set of components to a provided set of current components identified by their name. This allows the flexibility for working on a particular
         set of components within a resource state.
         """
         raise NotImplementedError
 
@@ -496,15 +494,15 @@
         backend_module = import_module(config.python_module)
     except Exception as e:
         print("Error loading backend module")
         print(f"Error > {e}")
 
         raise e
 
-    backend_class = None
+    backend_class: Optional[Callable] = None
     for item in dir(backend_module):
         potential_obj = getattr(backend_module, item)
         if (
             inspect.isclass(potential_obj)
             and issubclass(potential_obj, Backend)
             and item == config.python_class
         ):
@@ -513,13 +511,13 @@
 
     if not backend_class:
         print(f"Could not find {config.python_class} in {config.python_module}")
         raise Exception
 
     try:
         # initialize the backend obj with the provided configuration values
-        initialized_obj = potential_obj(**config.config)
+        initialized_obj = backend_class(**config.config)
     except Exception as e:
-        print(f"Could not initialize {potential_obj} Class from config {config.config}")
+        print(f"Could not initialize {backend_class} Class from config {config.config}")
         raise e
 
     return initialized_obj
```

### Comparing `cdev-0.0.8/core/constructs/backend_exceptions.py` & `cdev-0.0.9/core/constructs/backend_exceptions.py`

 * *Files identical despite different names*

### Comparing `cdev-0.0.8/core/constructs/cloud_output.py` & `cdev-0.0.9/core/constructs/cloud_output.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,61 @@
 """Structure that encapsulates the desire to capture and use output from deploying a resource on the cloud.
 
-Often, it is required to use the returned values provided by the cloud as input into another resource. For 
+Often, it is required to use the returned values provided by the cloud as input into another resource. For
 example, wanting to pass a created db name into the environment variables of a serverless function that will
 reference it. Therefor, it is important that these values are core primitives within the framework.
 
 The core framework has tried to make working with these types of values feel as natural as possible, but it
 is important to have an understanding of how they are designed to avoid confusion. A `Cloud Output` represents
 a future value that is not currently know at the execution time of the current code. They are designed to look
 and feel like the `types` they will evaluate to by providing methods that mirror common methods of the evaluated
 type.
 
 For example, a `Cloud Output String` contains methods such as `replace` that mirror `replace` on a regular string.
-These methods can be chained together to create more complex functionality. For a more in depth discussion on the 
+These methods can be chained together to create more complex functionality. For a more in depth discussion on the
 capabilities and limits of this system read out documentation at <link>.
 
 """
 
 from enum import Enum
-from typing import Any, List, Tuple, NewType, overload, Optional, Union, Iterable, Mapping, TypeVar, Generic
+from typing import (
+    Any,
+    Dict,
+    List,
+    Tuple,
+    NewType,
+    overload,
+    Optional,
+    Union,
+    Iterable,
+    Mapping,
+    TypeVar,
+    Generic,
+)
 from typing_extensions import Literal, SupportsIndex
 from collections.abc import Sequence
 
 from core.constructs.models import ImmutableModel, frozendict
 from core.utils import hasher
 
-CLOUD_OUTPUT_ID = 'cdev_cloud_output'
+CLOUD_OUTPUT_ID = "cdev_cloud_output"
 
 # Wrapper type to help keep annotations compact
-output_operation = NewType('output_operation', Tuple[str, Tuple, frozendict])
+output_operation = NewType("output_operation", Tuple[str, Tuple, frozendict])
+
 
 class OutputType(str, Enum):
-    """Type of Cloud Output 
-    
+    """Type of Cloud Output
+
     Since Cloud Output can be derived from resources and references, we need to denote where the Output is coming from.
     """
-    RESOURCE = 'resource'
-    REFERENCE = 'reference'
+
+    RESOURCE = "resource"
+    REFERENCE = "reference"
+
 
 ########################
 ##### Immutable Models
 ########################
 class cloud_output_model(ImmutableModel):
     """
     Often we want resources that depend on the value of output of other resources that is only known after a cloud resource is created. This serves
@@ -62,33 +78,34 @@
     """
 
     type: OutputType
     """
     Type of the underlying item we want to get the output of
     """
 
-    id: Literal['cdev_cloud_output']
+    id: Literal["cdev_cloud_output"]
     """
     Literal that allows a dict to be identified as a Cloud Output Model
     """
 
 
 class cloud_output_dynamic_model(cloud_output_model):
     """
     A cloud output model that has accompanying operations to be applied to the derived value
     """
 
-    output_operations: Tuple[output_operation,...]
+    output_operations: Tuple[output_operation, ...]
     """
     Tuple of all the operations to be applied to the derived value
     """
 
 
-
-def evaluate_dynamic_output(original_value: Any, cloud_output_dynamic: cloud_output_dynamic_model) -> Any:
+def evaluate_dynamic_output(
+    original_value: Any, cloud_output_dynamic: cloud_output_dynamic_model
+) -> Any:
     """Evaluate a set of operations on a starting value.
 
     Args:
         original_value (Any): The original value to operate on
         cloud_output_dynamic (cloud_output_dynamic_model): The model containing the operations to execute
 
     Raises:
@@ -101,15 +118,15 @@
 
     intermediate_value = original_value
     for x in operations:
         func_name = x[0]
         xargs = x[1]
         kwargs = x[2]
 
-        if func_name == '**not':
+        if func_name == "**not":
             # There is not hidden method that implements not, so we need to hard code this.
             new_rv = not intermediate_value
 
         elif func_name == "**and":
             new_rv = intermediate_value and xargs[0]
 
         elif func_name == "**or":
@@ -117,175 +134,186 @@
 
         elif func_name == "**xor":
             new_rv = intermediate_value ^ xargs[0]
 
         elif func_name == "join":
             new_rv = getattr(intermediate_value, func_name)(xargs)
 
-
         else:
-            object_methods = set([method_name for method_name in dir(str) if callable(getattr(str, method_name))])
-    
-    
-            if not func_name in object_methods:
+            object_methods = set(
+                [
+                    method_name
+                    for method_name in dir(str)
+                    if callable(getattr(str, method_name))
+                ]
+            )
+
+            if func_name not in object_methods:
                 print(object_methods)
-                raise Exception(f"'{func_name}' not in available methods for {intermediate_value} ({type(intermediate_value)})")
-    
+                raise Exception(
+                    f"'{func_name}' not in available methods for {intermediate_value} ({type(intermediate_value)})"
+                )
+
             if xargs and kwargs:
                 new_rv = getattr(intermediate_value, func_name)(**kwargs)
             elif (not xargs) and kwargs:
                 new_rv = getattr(intermediate_value, func_name)(**kwargs)
             elif xargs and (not kwargs):
                 new_rv = getattr(intermediate_value, func_name)(*xargs)
             elif (not xargs) and (not kwargs):
-                new_rv = getattr(intermediate_value, func_name)() 
-    
-    
+                new_rv = getattr(intermediate_value, func_name)()
+            else:
+                pass
         intermediate_value = new_rv
 
-
     return intermediate_value
 
 
 ########################
 ##### Helper Classes
 ########################
-class Cloud_Output():
+class Cloud_Output:
     """
     Mutable Class that can used during the creation phases to represent a desired cloud output model.
     """
 
-
     def __init__(self, name: str, ruuid: str, key: str, type: OutputType) -> None:
         self._name = name
         self._ruuid = ruuid
         self._key = key
         self._type = type
 
-
     def render(self) -> cloud_output_dynamic_model:
         return cloud_output_model(
             name=self._name,
             ruuid=self._ruuid,
             key=self._key,
             type=self._type,
-            id='cdev_cloud_output',
+            id="cdev_cloud_output",
         )
 
     def hash(self) -> str:
-        return hasher.hash_list([
-            self._name,
-            self._ruuid,
-            self._key,
-            self._type
-        ])
+        return hasher.hash_list([self._name, self._ruuid, self._key, self._type])
+
 
 class Cloud_Output_Dynamic(Cloud_Output):
     """
     Mutable Class that can used during the creation phases to represent a desired cloud output model. Allows the user to define
-    a list of operations that should be applied to the retrieved value. 
+    a list of operations that should be applied to the retrieved value.
     """
+
     def __init__(self, name: str, ruuid: str, key: str, type: OutputType) -> None:
         super().__init__(name, ruuid, key, type)
         self._operations: List[output_operation] = []
 
     def render(self) -> cloud_output_dynamic_model:
-        operations = tuple([(x[0], tuple(x[1]), frozendict(x[2])) for x in self._operations])
+        operations = tuple(
+            [(x[0], tuple(x[1]), frozendict(x[2])) for x in self._operations]
+        )
 
         return cloud_output_dynamic_model(
             name=self._name,
             ruuid=self._ruuid,
             key=self._key,
             type=self._type,
-            id='cdev_cloud_output',
-            output_operations=operations
+            id="cdev_cloud_output",
+            output_operations=operations,
         )
 
-
     def hash(self) -> str:
-        return hasher.hash_list([
-            super().hash(),
-            self.render().output_operations if self._operations else ""
-        ])
-
-   
+        return hasher.hash_list(
+            [
+                super().hash(),
+                self.render().output_operations if self._operations else "",
+            ]
+        )
 
 
 ########################
 ##### Types of Output
 ########################
-    
+
+
 class Cloud_Output_Bool(Cloud_Output_Dynamic):
     """
     Cloud Output that will resolve to a Boolean value after being retrieve or after all the operations have been executed
     """
 
     def __init__(self, name: str, ruuid: str, key: str, type: OutputType) -> None:
         super().__init__(name, ruuid, key, type)
 
-
-    def and_(self, x: bool) -> 'Cloud_Output_Bool':
+    def and_(self, x: bool) -> "Cloud_Output_Bool":
         """And against x
 
-        Returns a Cloud Output Bool on which further operations can be chained.
+        Args:
+            x (bool)
+
+        Returns:
+            Cloud_Output_Bool
         """
         self._operations.append(
             (
-                '**and', 
-                tuple([x]), 
+                "**and",
+                tuple([x]),
                 {},
             )
         )
 
         return self
 
-
-    def or_(self, x: bool) -> 'Cloud_Output_Bool':
+    def or_(self, x: bool) -> "Cloud_Output_Bool":
         """Or against x
 
-        Returns a Cloud Output Bool on which further operations can be chained.
+        Args:
+            x (bool)
+
+        Returns:
+            Cloud_Output_Bool
         """
         self._operations.append(
             (
-                '**or', 
-                tuple([x]), 
+                "**or",
+                tuple([x]),
                 {},
             )
         )
 
         return self
 
-
-    def xor_(self, x: bool) -> 'Cloud_Output_Bool':
+    def xor_(self, x: bool) -> "Cloud_Output_Bool":
         """Xor against x
 
-        Returns a Cloud Output Bool on which further operations can be chained.
+        Args:
+            x (bool)
+
+        Returns:
+            Cloud_Output_Bool
         """
         self._operations.append(
             (
-                '**xor', 
-                tuple([x]), 
+                "**xor",
+                tuple([x]),
                 {},
             )
         )
 
         return self
 
+    def not_(self) -> "Cloud_Output_Bool":
+        """Not against self
 
-    def not_(self) -> 'Cloud_Output_Bool':
-        """Not Current Value
-
-        Returns a Cloud Output Bool on which further operations can be chained.
+        Returns:
+            Cloud_Output_Bool
         """
-        # Special case because there is not underlying method to call for not so pass this hardcoded 
+        # Special case because there is not underlying method to call for not so pass this hardcoded
         # value and make sure that the operation interpreter respects this token as the 'not' operator.
         self._operations.append(
             (
-                '**not', 
-                (), 
+                "**not",
+                (),
                 {},
             )
         )
 
         return self
 
 
@@ -293,1223 +321,1207 @@
     """
     Cloud Output that will resolve to a Integer value after being retrieve or after all the operations have been executed
     """
 
     def __init__(self, name: str, ruuid: str, key: str, type: OutputType) -> None:
         super().__init__(name, ruuid, key, type)
 
+    def add(self, x: int) -> "Cloud_Output_Int":
+        """Add x
 
-    def add(self, x: int) -> 'Cloud_Output_Int':
-        """Add x 
+        Args:
+            x (int)
 
-        Returns a Cloud Output Int on which further operations can be chained.
+        Returns:
+            Cloud_Output_Int
         """
         self._operations.append(
             (
-                '__add__', 
-                tuple([x]), 
+                "__add__",
+                tuple([x]),
                 {},
             )
         )
 
         return self
 
-    
-    def subtract(self, x: int) -> 'Cloud_Output_Int':
-        """Substract x
+    def subtract(self, x: int) -> "Cloud_Output_Int":
+        """Subtract x
+
+        Args:
+            x (int)
 
-        Returns a Cloud Output Int on which further operations can be chained.
+        Returns:
+            Cloud_Output_Int
         """
         self._operations.append(
             (
-                '__add__', 
-                tuple([x*-1]), 
+                "__add__",
+                tuple([x * -1]),
                 {},
             )
         )
 
         return self
 
-
-    def multiply(self, x: int) -> 'Cloud_Output_Int':
+    def multiply(self, x: int) -> "Cloud_Output_Int":
         """Multiply x
 
-        Returns a Cloud Output Int on which further operations can be chained.
+        Args:
+            x (int)
+
+        Returns:
+            Cloud_Output_Int
         """
         self._operations.append(
             (
-                '__mul__', 
-                tuple([x]), 
+                "__mul__",
+                tuple([x]),
                 {},
             )
         )
 
         return self
 
-
-    def divide_mod(self, x: int) -> Tuple['Cloud_Output_Int', 'Cloud_Output_Int']:
+    def divide_mod(self, x: int) -> Tuple["Cloud_Output_Int", "Cloud_Output_Int"]:
         """Return the pair (i // x, i % x)
 
-        Returns a Cloud Output Int on which further operations can be chained.
+        Returns:
+            Tuple["Cloud_Output_Int", "Cloud_Output_Int"]
         """
         self._operations.append(
             (
-                '__divmod__', 
-                tuple([x]), 
+                "__divmod__",
+                tuple([x]),
                 {},
             )
         )
 
         return self
 
-    
+
 class Cloud_Output_Str(Sequence, Cloud_Output_Dynamic):
     """
     Cloud Output that will resolve to a String value after being retrieve or after all the operations have been executed
     """
 
-
     def __init__(self, name: str, ruuid: str, key: str, type: OutputType) -> None:
         super().__init__(name, ruuid, key, type)
 
     def __len__(self):
         raise Exception
 
-    def __getitem__(self, key) -> 'Cloud_Output_Str':
-        self._operations.append(
-            (
-                '__getitem__',
-                [key],
-                {}
-            )
-        )    
+    def __getitem__(self, key) -> "Cloud_Output_Str":
+        self._operations.append(("__getitem__", [key], {}))
 
         return self
 
     def __contains__(self, _o: str) -> Cloud_Output_Bool:
-        self._operations.append(
-            (
-                '__contains__',
-                [_o],
-                {}
-            )
-        )
+        self._operations.append(("__contains__", [_o], {}))
 
         return self
 
-    def capitalize(self) -> 'Cloud_Output_Str':
+    def capitalize(self) -> "Cloud_Output_Str":
         """Make the first character have upper case and the rest lower case.
 
-        Append the operation to the Cloud Output Object and return the same Object for 
-        any further operations.
-
+        Returns:
+            Cloud_Output_Str
         """
         self._operations.append(
             (
-                'capitalize', 
-                (), 
+                "capitalize",
+                (),
                 {},
             )
         )
         return self
 
-    def casefold(self) -> 'Cloud_Output_Str':
+    def casefold(self) -> "Cloud_Output_Str":
         """Make S suitable for caseless comparisons.
 
-        Append the operation to the Cloud Output Object and return the same Object for 
-        any further operations.
-        
+        Returns:
+            Cloud_Output_Str
         """
         self._operations.append(
             (
-                'casefold', 
-                (), 
+                "casefold",
+                (),
                 {},
             )
         )
         return self
 
-    def center(
-        self, 
-        width: SupportsIndex, 
-        fillchar: str = None) -> 'Cloud_Output_Str':
+    def center(self, width: SupportsIndex, fillchar: str = None) -> "Cloud_Output_Str":
         """S centered in a string of length width. Padding is done using the specified fill character (default is a space)
 
-        Append the operation to the Cloud Output Object and return the same Cloud Output String object for any further operations.
+        Args:
+            width (SupportsIndex)
+            fillchar (str, optional)
+
+        Returns:
+            Cloud_Output_Str
         """
 
-        
         if fillchar:
             args = (width, fillchar)
         else:
-            args = (width)
-
+            args = width
 
         self._operations.append(
             (
-                'center', 
-                args, 
+                "center",
+                args,
                 {},
             )
         )
         return self
 
-    def count(self, 
-        x: str, 
-        start: Optional[SupportsIndex] = None, 
-        end: Optional[SupportsIndex] = None) -> Cloud_Output_Int:
+    def count(
+        self,
+        x: str,
+        start: Optional[SupportsIndex] = None,
+        end: Optional[SupportsIndex] = None,
+    ) -> Cloud_Output_Int:
         """The number of non-overlapping occurrences of substring sub in string S[start:end].
-        
-        Returns a Cloud Output Int on which further operations can be chained. The created Cloud Output Int
-        will contain all previous operations of the current Cloud Output String that this is being called on.
 
-        Optional arguments start and end are interpreted as in slice notation.
+        Args:
+            x (str)
+            start (Optional[SupportsIndex], optional): Defaults to None.
+            end (Optional[SupportsIndex], optional): Defaults to None.
+
+        Returns:
+            Cloud_Output_Int
         """
 
-        
         if start and end:
             args = (x, start, end)
         elif start and (not end):
             args = (x, start, None)
 
         elif (not start) and end:
             args = (x, None, end)
 
         else:
             args = (x, None, None)
 
         self._operations.append(
             (
-                'count', 
-                args, 
+                "count",
+                args,
                 {},
             )
         )
 
-        rv = Cloud_Output_Int(
-            self._name, self._ruuid, self._key, self._type
-        )
+        rv = Cloud_Output_Int(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
     def endswith(
-        self, 
+        self,
         suffix: Union[str, Tuple[str, ...]],
-        start: Optional[SupportsIndex] = None, 
-        end: Optional[SupportsIndex] = None) -> Cloud_Output_Bool:
+        start: Optional[SupportsIndex] = None,
+        end: Optional[SupportsIndex] = None,
+    ) -> Cloud_Output_Bool:
         """Return True if S ends with the specified suffix, False otherwise.
-        
-        Returns a Cloud Output Boolean on which further operations can be chained. The created Cloud Output Boolean
-        will contain all previous operations of the current Cloud Output String that this is being called on.
-        
+
         With optional start, test S beginning at that position.
         With optional end, stop comparing S at that position.
         suffix can also be a tuple of strings to try.
+
+        Args:
+            suffix (Union[str, Tuple[str, ...]]):
+            start (Optional[SupportsIndex], optional): Defaults to None.
+            end (Optional[SupportsIndex], optional): Defaults to None.
+
+        Returns:
+            Cloud_Output_Bool
         """
 
         args = []
 
         if suffix:
             args.append(suffix)
 
         if start:
             args.append(start)
 
         if end:
             args.append(end)
 
-
         self._operations.append(
             (
-                'endswith', 
+                "endswith",
                 tuple(args),
                 {},
             )
         )
 
-        rv = Cloud_Output_Bool(
-            self._name, self._ruuid, self._key, self._type
-        )
+        rv = Cloud_Output_Bool(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
-    def expandtabs(self, tabsize=8) -> 'Cloud_Output_Str':
+    def expandtabs(self, tabsize=8) -> "Cloud_Output_Str":
         """S where all tab characters are expanded using spaces.
-        
-        Append the operation to the Cloud Output Object and return the same Cloud Output String object for any further operations.
-        
+
         If tabsize is not given, a tab size of 8 characters is assumed.
+
+        Args:
+            tabsize (int, optional): Defaults to 8.
+
+        Returns:
+            Cloud_Output_Str
         """
         self._operations.append(
             (
-                'expandtabs', 
-                (), 
-                {
-                    'tabsize': tabsize
-                },
+                "expandtabs",
+                (),
+                {"tabsize": tabsize},
             )
         )
         return self
 
     def find(
-        self, 
-        sub: str, 
-        start: Optional[SupportsIndex] = None, 
-        end: Optional[SupportsIndex] = None) -> Cloud_Output_Int:
-        """
-        Return the lowest index in S where substring sub is found, such that sub is contained within S[start:end].  
-        
-        Returns a Cloud Output Int on which further operations can be chained. The created Cloud Output Int
-        will contain all previous operations of the current Cloud Output String that this is being called on.
+        self,
+        sub: str,
+        start: Optional[SupportsIndex] = None,
+        end: Optional[SupportsIndex] = None,
+    ) -> Cloud_Output_Int:
+        """Return the lowest index in S where substring sub is found, such that sub is contained within S[start:end].
 
         Optional arguments start and end are interpreted as in slice notation.
+
+        Args:
+            sub (str)
+            start (Optional[SupportsIndex], optional): Defaults to None.
+            end (Optional[SupportsIndex], optional): Defaults to None.
+
+        Returns:
+            Cloud_Output_Int
         """
 
         args = [sub]
 
         if start:
             args.append(start)
 
         if end:
             args.append(end)
 
         self._operations.append(
             (
-                'find', 
-                tuple(args), 
+                "find",
+                tuple(args),
                 {},
             )
         )
 
-        rv = Cloud_Output_Int(
-            self._name, self._ruuid, self._key, self._type
-        )
+        rv = Cloud_Output_Int(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
-    def format(self, *args, **kwargs) -> 'Cloud_Output_Str':
+    def format(self, *args, **kwargs) -> "Cloud_Output_Str":
         """Format S, using substitutions from args and kwargs.
 
-        Append the operation to the Cloud Output Object and return the same Cloud Output String object for any further operations.
-
         The substitutions are identified by braces ('{' and '}').
+
+        Returns:
+            Cloud_Output_Str
         """
         self._operations.append(
             (
-                'format', 
-                args, 
+                "format",
+                args,
                 kwargs,
             )
         )
         return self
 
-    def format_map(self, mapping) -> 'Cloud_Output_Str':
+    def format_map(self, mapping: Dict) -> "Cloud_Output_Str":
         """Format S, using substitutions from mapping.
+
         The substitutions are identified by braces ('{' and '}').
 
-        Append the operation to the Cloud Output Object and return the same Cloud Output String object for any further operations.
+        Args:
+            mapping (Dict)
+
+        Returns:
+            Cloud_Output_Str
         """
         self._operations.append(
             (
-                'format_map', 
-                (), 
-                {
-                    'mapping': mapping
-                },
+                "format_map",
+                (),
+                {"mapping": mapping},
             )
         )
         return self
 
     def index(
-        self, 
-        sub: str, 
-        start: Optional[SupportsIndex] = None, 
-        end: Optional[SupportsIndex] = None) -> Cloud_Output_Int:
-        """Return the lowest index in S where substring sub is found, such that sub is contained within S[start:end].  
-
-        Returns a Cloud Output Int on which further operations can be chained. The created Cloud Output Int
-        will contain all previous operations of the current Cloud Output String that this is being called on.
-        
+        self,
+        sub: str,
+        start: Optional[SupportsIndex] = None,
+        end: Optional[SupportsIndex] = None,
+    ) -> Cloud_Output_Int:
+        """Return the lowest index in S where substring sub is found, such that sub is contained within S[start:end].
+
         Optional arguments start and end are interpreted as in slice notation.
 
-        Raises ValueError when the substring is not found.
+        When evaluating, raises ValueError if the substring is not found.
+
+        Args:
+            sub (str)
+            start (Optional[SupportsIndex], optional): Defaults to None.
+            end (Optional[SupportsIndex], optional): Defaults to None.
+
+        Returns:
+            Cloud_Output_Int
         """
 
         args = [sub]
 
         if start:
             args.append(start)
 
         if end:
             args.append(end)
 
         self._operations.append(
             (
-                'index', 
-                tuple(args), 
+                "index",
+                tuple(args),
                 {},
             )
         )
 
-        rv = Cloud_Output_Int(
-            self._name, self._ruuid, self._key, self._type
-        )
+        rv = Cloud_Output_Int(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
     def isalnum(self) -> Cloud_Output_Bool:
         """Return True if all characters in S are alphanumeric and there is at least one character in S, False otherwise.
 
-        Returns a Cloud Output Boolean on which further operations can be chained. The created Cloud Output Boolean
-        will contain all previous operations of the current Cloud Output String that this is being called on.
+        Returns:
+            Cloud_Output_Bool
         """
         self._operations.append(
             (
-                'isalnum', 
-                (), 
+                "isalnum",
+                (),
                 {},
             )
         )
 
-        rv = Cloud_Output_Bool(
-            self._name, self._ruuid, self._key, self._type
-        )
+        rv = Cloud_Output_Bool(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
-
     def isalpha(self) -> Cloud_Output_Bool:
         """Return True if all characters in S are alphabetic and there is at least one character in S, False otherwise.
 
-        Returns a Cloud Output Boolean on which further operations can be chained. The created Cloud Output Boolean
-        will contain all previous operations of the current Cloud Output String that this is being called on.
+        Returns:
+            Cloud_Output_Bool
         """
         self._operations.append(
             (
-                'isalpha',
+                "isalpha",
                 (),
                 {},
             )
         )
 
-        rv = Cloud_Output_Bool(
-            self._name, self._ruuid, self._key, self._type
-        )
+        rv = Cloud_Output_Bool(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
     def isdecimal(self) -> Cloud_Output_Bool:
         """Return True if there are only decimal characters in S, False otherwise.
 
-        Returns a Cloud Output Boolean on which further operations can be chained. The created Cloud Output Boolean
-        will contain all previous operations of the current Cloud Output String that this is being called on.
+        Returns:
+            Cloud_Output_Bool
         """
         self._operations.append(
             (
-                'isdecimal', 
+                "isdecimal",
                 (),
                 {},
             )
         )
 
-        rv = Cloud_Output_Bool(
-            self._name, self._ruuid, self._key, self._type
-        )
+        rv = Cloud_Output_Bool(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
     def isdigit(self) -> Cloud_Output_Bool:
         """Return True if all characters in S are digits and there is at least one character in S, False otherwise.
-        
-        Returns a Cloud Output Boolean on which further operations can be chained. The created Cloud Output Boolean
-        will contain all previous operations of the current Cloud Output String that this is being called on.
+
+        Returns:
+            Cloud_Output_Bool
         """
         self._operations.append(
             (
-                'isdigit',
+                "isdigit",
                 (),
                 {},
             )
         )
 
-        rv = Cloud_Output_Bool(
-            self._name, self._ruuid, self._key, self._type
-        )
+        rv = Cloud_Output_Bool(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
     def isidentifier(self) -> Cloud_Output_Bool:
         """Return True if S is a valid identifier according to the language definition.
 
-        Returns a Cloud Output Boolean on which further operations can be chained. The created Cloud Output Boolean
-        will contain all previous operations of the current Cloud Output String that this is being called on.
-
         Use keyword.iskeyword() to test for reserved identifiers
         such as "def" and "class".
 
+        Returns:
+            Cloud_Output_Bool
         """
         self._operations.append(
             (
-                'isidentifier',
+                "isidentifier",
                 (),
                 {},
             )
         )
 
-        rv = Cloud_Output_Bool(
-            self._name, self._ruuid, self._key, self._type
-        )
+        rv = Cloud_Output_Bool(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
     def islower(self) -> Cloud_Output_Bool:
         """Return True if all cased characters in S are lowercase and there is at least one cased character in S, False otherwise.
 
-        Returns a Cloud Output Boolean on which further operations can be chained. The created Cloud Output Boolean
-        will contain all previous operations of the current Cloud Output String that this is being called on.
+
+        Returns:
+            Cloud_Output_Bool
         """
         self._operations.append(
             (
-                'islower',
-                (), 
+                "islower",
+                (),
                 {},
             )
         )
 
-        rv = Cloud_Output_Bool(
-            self._name, self._ruuid, self._key, self._type
-        )
+        rv = Cloud_Output_Bool(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
     def isnumeric(self) -> Cloud_Output_Bool:
         """Return True if there are only numeric characters in S, False otherwise.
 
-        Returns a Cloud Output Boolean on which further operations can be chained. The created Cloud Output Boolean
-        will contain all previous operations of the current Cloud Output String that this is being called on.
+        Returns:
+            Cloud_Output_Bool
         """
         self._operations.append(
             (
-                'isnumeric',
+                "isnumeric",
                 (),
                 {},
             )
         )
 
-        rv = Cloud_Output_Bool(
-            self._name, self._ruuid, self._key, self._type
-        )
+        rv = Cloud_Output_Bool(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
     def isprintable(self) -> Cloud_Output_Bool:
         """Return True if all characters in S are considered printable in repr() or S is empty, False otherwise.
 
-        Returns a Cloud Output Boolean on which further operations can be chained. The created Cloud Output Boolean
-        will contain all previous operations of the current Cloud Output String that this is being called on.
+        Returns:
+            Cloud_Output_Bool
         """
         self._operations.append(
             (
-                'isprintable', 
+                "isprintable",
                 (),
                 {},
             )
         )
 
-        rv = Cloud_Output_Bool(
-            self._name, self._ruuid, self._key, self._type
-        )
+        rv = Cloud_Output_Bool(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
     def isspace(self) -> Cloud_Output_Bool:
         """Return True if all characters in S are whitespace and there is at least one character in S, False otherwise.
 
-        Returns a Cloud Output Boolean on which further operations can be chained. The created Cloud Output Boolean
-        will contain all previous operations of the current Cloud Output String that this is being called on.
+        Returns:
+            Cloud_Output_Bool
         """
         self._operations.append(
             (
-                'isspace', 
-                (), 
+                "isspace",
+                (),
                 {},
             )
         )
 
-        rv = Cloud_Output_Bool(
-            self._name, self._ruuid, self._key, self._type
-        )
+        rv = Cloud_Output_Bool(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
     def istitle(self) -> Cloud_Output_Bool:
         """Return True if S is a titlecased string and there is at least one
         character in S, i.e. upper- and titlecase characters may only
         follow uncased characters and lowercase characters only cased ones.
         Return False otherwise.
 
-        Returns a Cloud Output Boolean on which further operations can be chained. The created Cloud Output Boolean
-        will contain all previous operations of the current Cloud Output String that this is being called on.
+        Returns:
+            Cloud_Output_Bool
         """
         self._operations.append(
             (
-                'istitle', 
-                (), 
+                "istitle",
+                (),
                 {},
             )
         )
 
-        rv = Cloud_Output_Bool(
-            self._name, self._ruuid, self._key, self._type
-        )
+        rv = Cloud_Output_Bool(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
     def isupper(self) -> Cloud_Output_Bool:
         """Return True if all cased characters in S are uppercase and there is
         at least one cased character in S, False otherwise.
 
-        Returns a Cloud Output Boolean on which further operations can be chained. The created Cloud Output Boolean
-        will contain all previous operations of the current Cloud Output String that this is being called on.
+        Returns:
+            Cloud_Output_Bool
         """
         self._operations.append(
             (
-                'isupper', 
-                (), 
+                "isupper",
+                (),
                 {},
             )
         )
 
-        rv = Cloud_Output_Bool(
-            self._name, self._ruuid, self._key, self._type
-        )
+        rv = Cloud_Output_Bool(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
-    
+    def join(self, iterable: Iterable[str]) -> "Cloud_Output_Str":
+        """Return a string which is the concatenation of the strings in the iterable with S being the separator.
 
-    def join(self, iterable: Iterable[str]) -> 'Cloud_Output_Str':
-        """Return a string which is the concatenation of the strings in the iterable with S being the seperator.
+        Args:
+            iterable (Iterable[str])
 
-        Append the operation to the Cloud Output Object and return the same Cloud Output String object for any further operations.
+        Returns:
+            Cloud_Output_Str
         """
         self._operations.append(
             (
-                'join',
-                iterable, 
-                {
-                    
-                },
+                "join",
+                iterable,
+                {},
             )
         )
-        print(self._operations)
         return self
 
+    def ljust(self, width: SupportsIndex, __fillchar: str = "") -> "Cloud_Output_Str":
+        """Return S left-justified in a Unicode string of length __width.
 
-    def ljust(self, width: SupportsIndex, __fillchar: str = "") -> 'Cloud_Output_Str':
-        """Return S left-justified in a Unicode string of length __width. 
+        Padding is done using the specified fill character (default is a space).
 
-        Append the operation to the Cloud Output Object and return the same Cloud Output String object for any further operations.
+        Args:
+            width (SupportsIndex)
+            __fillchar (str, optional): Defaults to "".
 
-        Padding is done using the specified fill character (default is a space).
+        Returns:
+            Cloud_Output_Str
         """
 
         args = [width]
 
         if __fillchar:
             args.append(__fillchar)
 
         self._operations.append(
             (
-                'ljust',
+                "ljust",
                 tuple(args),
                 {},
             )
         )
         return self
 
-    def lower(self) -> 'Cloud_Output_Str':
+    def lower(self) -> "Cloud_Output_Str":
         """Return a copy of the string S converted to lowercase.
 
-        Append the operation to the Cloud Output Object and return the same Cloud Output String object for any further operations.
+        Returns:
+            Cloud_Output_Str
         """
         self._operations.append(
             (
-                'lower',
+                "lower",
                 (),
                 {},
             )
         )
         return self
 
-    def lstrip(self, chars: Optional[str] = None) -> 'Cloud_Output_Str':
+    def lstrip(self, chars: Optional[str] = None) -> "Cloud_Output_Str":
         """Return a copy of the string S with leading whitespace removed.
-        
-        Append the operation to the Cloud Output Object and return the same Cloud Output String object for any further operations.
-        
+
         If chars is given and not None, remove characters in chars instead.
+
+        Args:
+            chars (Optional[str], optional): Defaults to None.
+
+        Returns:
+            Cloud_Output_Str
         """
 
         args = []
 
         if chars:
             args.append(chars)
         self._operations.append(
             (
-                'lstrip', 
-                tuple(args), 
+                "lstrip",
+                tuple(args),
                 {},
             )
         )
 
         return self
 
-
-
     def replace(
-        self, 
-        old: str, 
-        new: str, 
-        count: SupportsIndex = None) -> 'Cloud_Output_Str':
-        """Change all occurrences of substring old replaced by new. 
+        self, old: str, new: str, count: SupportsIndex = None
+    ) -> "Cloud_Output_Str":
+        """Change all occurrences of substring old replaced by new.
 
-        Append the operation to the Cloud Output Object and return the same Cloud Output String object for any further operations.
-        
         If the optional argument count is given, only the first count occurrences are replaced.
+
+        Args:
+            old (str)
+            new (str)
+            count (SupportsIndex, optional): Defaults to None.
+
+        Returns:
+            Cloud_Output_Str
         """
 
         if count:
             args = (old, new, count)
         else:
             args = (old, new)
 
         self._operations.append(
             (
-                'replace',
+                "replace",
                 args,
-                {
-                
-                },
+                {},
             )
         )
 
         return self
 
     def rfind(
-        self, 
-        sub: str, 
-        start: Optional[SupportsIndex] = None, 
-        end: Optional[SupportsIndex] = None) -> Cloud_Output_Int:
-        """Return the highest index in S where substring sub is found, such that sub is contained within S[start:end].  
-        
-        Returns a Cloud Output Int on which further operations can be chained. The created Cloud Output Int
-        will contain all previous operations of the current Cloud Output String that this is being called on.
+        self,
+        sub: str,
+        start: Optional[SupportsIndex] = None,
+        end: Optional[SupportsIndex] = None,
+    ) -> Cloud_Output_Int:
+        """Return the highest index in S where substring sub is found, such that sub is contained within S[start:end].
 
         Optional arguments start and end are interpreted as in slice notation.
 
         Return -1 on failure.
-        """
 
+        Args:
+            sub (str)
+            start (Optional[SupportsIndex], optional): Defaults to None.
+            end (Optional[SupportsIndex], optional): Defaults to None.
+
+        Returns:
+            Cloud_Output_Int
+        """
         args = [sub]
 
         if start:
             args.append(start)
 
         if end:
             args.append(end)
 
         self._operations.append(
             (
-                'rfind',
+                "rfind",
                 tuple(args),
                 {},
             )
         )
 
-        rv = Cloud_Output_Int(
-            self._name, self._ruuid, self._key, self._type
-        )
+        rv = Cloud_Output_Int(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
     def rindex(
-        self, 
-        sub: str,  
-        start: Optional[SupportsIndex] = None, 
-        end: Optional[SupportsIndex] = None) -> Cloud_Output_Int:
-        """Return the highest index in S where substring sub is found, such that sub is contained within S[start:end].  
-        
-        Returns a Cloud Output Int on which further operations can be chained. The created Cloud Output Int
-        will contain all previous operations of the current Cloud Output String that this is being called on.
+        self,
+        sub: str,
+        start: Optional[SupportsIndex] = None,
+        end: Optional[SupportsIndex] = None,
+    ) -> Cloud_Output_Int:
+        """Return the highest index in S where substring sub is found, such that sub is contained within S[start:end].
 
         Optional arguments start and end are interpreted as in slice notation.
 
-        Raises ValueError when the substring is not found.
+        When evaluating, raises ValueError if the substring is not found.
+
+        Args:
+            sub (str)
+            start (Optional[SupportsIndex], optional): Defaults to None.
+            end (Optional[SupportsIndex], optional): Defaults to None.
+
+        Returns:
+            Cloud_Output_Int
         """
 
         args = [sub]
 
         if start:
             args.append(start)
 
         if end:
             args.append(end)
 
         self._operations.append(
             (
-                'rindex',
+                "rindex",
                 (),
                 {
                     "__sub": sub,
                     "__start": start,
-                    "__end": end,   
+                    "__end": end,
                 },
             )
         )
 
-        rv = Cloud_Output_Int(
-            self._name, self._ruuid, self._key, self._type
-        )
+        rv = Cloud_Output_Int(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
-
-    def rjust(
-        self, 
-        width: SupportsIndex, 
-        fillchar: str = None) -> 'Cloud_Output_Str':
+    def rjust(self, width: SupportsIndex, fillchar: str = None) -> "Cloud_Output_Str":
         """Right-justify S in a string of length width. Padding is
         done using the specified fill character (default is a space).
 
-        Append the operation to the Cloud Output Object and return the same Cloud Output String object for any further operations.
-        """
 
+        Args:
+            width (SupportsIndex):
+            fillchar (str, optional): Defaults to None.
+
+        Returns:
+            Cloud_Output_Str
+        """
         args = [width]
 
         if fillchar:
             args.append(fillchar)
 
         print(args)
         self._operations.append(
             (
-                'rjust',
+                "rjust",
                 tuple(args),
                 {},
             )
         )
 
         return self
 
-
-    #def rsplit(
-    #    self, 
-    #    sep: Optional[str] = None, 
+    # def rsplit(
+    #    self,
+    #    sep: Optional[str] = None,
     #    maxsplit: Optional[SupportsIndex] = None) -> List['Cloud_Output_Str']:
     #    """Return a list of the words in S, using sep as the
     #    delimiter string, starting at the end of the string and
-    #    working to the front.  
-#
+    #    working to the front.
+    #
     #    Append the operation to the Cloud Output Object and return the same Cloud Output String object for any further operations.
-    #    
-    #    If maxsplit is given, at most maxsplit splits are done. 
-    #    
+    #
+    #    If maxsplit is given, at most maxsplit splits are done.
+    #
     #    If sep is not specified, any whitespace string is a separator.
     #    """
     #    args = []
-#
+    #
     #    if sep:
     #        args.append(sep)
-#
+    #
     #    if maxsplit:
     #        args.append(maxsplit)
-#
-#
+    #
+    #
     #    self._operations.append(
     #        (
     #            'rsplit',
     #            tuple(args),
     #            {},
     #        )
     #    )
     #    return self
 
-    
-    def rstrip(
-        self, 
-        chars: Optional[str] = None)  -> 'Cloud_Output_Str':
+    def rstrip(self, chars: Optional[str] = None) -> "Cloud_Output_Str":
         """Return S with trailing whitespace removed.
-        
-        Append the operation to the Cloud Output Object and return the same Cloud Output String object for any further operations.
-        
+
         If chars is given and not None, remove characters in chars instead.
+
+        Args:
+            chars (Optional[str], optional): Defaults to None.
+
+        Returns:
+            Cloud_Output_Str
         """
         self._operations.append(
             (
-                'rstrip',
-                (chars), 
+                "rstrip",
+                (chars),
                 {},
             )
         )
 
-    #def split(
-    #    self, 
+    # def split(
+    #    self,
     #    sep=None,
     #    maxsplit=-1) -> List['Cloud_Output_Str']:
-    #    """Return a list of the words in S, using sep as the delimiter string.  
-#
+    #    """Return a list of the words in S, using sep as the delimiter string.
+    #
     #    ## TODO Sequence type
-    #    
+    #
     #    If maxsplit is given, at most maxsplit splits are done.
-    #    
+    #
     #    If sep is not specified or is None, any whitespace string is a separator and empty strings are
     #    removed from the result.
     #    """
     #    self._operations.append(
     #        (
-    #            'split', 
+    #            'split',
     #            (sep, maxsplit),
     #            {},
     #        )
     #    )
-#
-    #def splitlines(
-    #    self, 
+    #
+    # def splitlines(
+    #    self,
     #    keepends: bool = False) -> List['Cloud_Output_Str']:
     #    """
     #    Return a list of the lines in S, breaking at line boundaries.
-#
+    #
     #    ## TODO Sequence type
-    #    
+    #
     #    Line breaks are not included in the resulting list unless keepends is given and true.
     #    """
     #    self._operations.append(
     #        (
-    #            'splitlines', 
-    #            (keepends), 
+    #            'splitlines',
+    #            (keepends),
     #            {},
     #        )
     #    )
-#
+    #
     def startswith(
-        self, 
-        prefix: Union[str, Tuple[str, ...]], 
-        start: Optional[SupportsIndex] = None, 
-        end: Optional[SupportsIndex] = None) -> Cloud_Output_Int:
+        self,
+        prefix: Union[str, Tuple[str, ...]],
+        start: Optional[SupportsIndex] = None,
+        end: Optional[SupportsIndex] = None,
+    ) -> Cloud_Output_Int:
         """Return True if S starts with the specified prefix, False otherwise.
-        
-        Returns a Cloud Output Boolean on which further operations can be chained. The created Cloud Output Boolean
-        will contain all previous operations of the current Cloud Output String that this is being called on.
-        
+
         With optional start, test S beginning at that position.
         With optional end, stop comparing S at that position.
         prefix can also be a tuple of strings to try.
+
+        Args:
+            prefix (Union[str, Tuple[str, ...]]):
+            start (Optional[SupportsIndex], optional): Defaults to None.
+            end (Optional[SupportsIndex], optional): Defaults to None.
+
+        Returns:
+            Cloud_Output_Int
         """
 
         args = [prefix]
 
         if start:
             args.append(start)
 
         if end:
             args.append(end)
 
         self._operations.append(
             (
-                'startswith', 
-                tuple(args), 
+                "startswith",
+                tuple(args),
                 {},
             )
         )
 
-        rv = Cloud_Output_Int(
-            self._name, self._ruuid, self._key, self._type
-        )
+        rv = Cloud_Output_Int(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
-    def strip(
-        self, 
-        chars: Optional[str] = ...)  -> 'Cloud_Output_Str':
+    def strip(self, chars: Optional[str] = ...) -> "Cloud_Output_Str":
         """S with leading and trailing whitespace removed.
-        
-        Append the operation to the Cloud Output Object and return the same Cloud Output String object for any further operations.
-        
+
         If chars is given and not None, remove characters in chars instead.
+
+        Args:
+            chars (Optional[str], optional): Defaults to ....
+
+        Returns:
+            Cloud_Output_Str
         """
-        self._operations.append(
-            (
-                'strip',
-                (chars),
-                {}
-            )
-        )
+        self._operations.append(("strip", (chars), {}))
         return self
 
-    def swapcase(self) -> 'Cloud_Output_Str':
+    def swapcase(self) -> "Cloud_Output_Str":
         """S with uppercase characters converted to lowercase and vice versa.
 
-        Append the operation to the Cloud Output Object and return the same Cloud Output String object for any further operations.
+        Returns:
+            Cloud_Output_Str
         """
-        self._operations.append(
-            (
-                'swapcase', 
-                (), 
-                {}
-            )
-        )
+        self._operations.append(("swapcase", (), {}))
 
         return self
 
-
-    def title(self) -> 'Cloud_Output_Str':
+    def title(self) -> "Cloud_Output_Str":
         """Titlecased version of S
 
-        Append the operation to the Cloud Output Object and return the same Cloud Output String object for any further operations.
-        
         i.e. words start with title case characters, all remaining cased characters have lower case.
+
+        Returns:
+            Cloud_Output_Str
         """
-        self._operations.append(
-            (
-                'title',
-                (),
-                {}
-            )
-        )
+        self._operations.append(("title", (), {}))
         return self
 
     def translate(
         self,
-        table: Mapping[
-                int, 
-                Union[ 
-                    Union[int ,str,None], 
-                    List[ Union[int, str, None] ] 
-                ]
-            ]
-        ) -> 'Cloud_Output_Str':
-        """S in which each character has been mapped through the given translation table. 
-        
+        table: Mapping[int, Union[Union[int, str, None], List[Union[int, str, None]]]],
+    ) -> "Cloud_Output_Str":
+        """S in which each character has been mapped through the given translation table.
+
         The table must implement
         lookup/indexing via __getitem__, for instance a dictionary or list,
         mapping Unicode ordinals to Unicode ordinals, strings, or None. If
         this operation raises LookupError, the character is left untouched.
         Characters mapped to None are deleted.
-        """
-        self._operations.append(
-            (
-                'translate', 
-                (table),
-                {}
-            )
-        )
 
-    def upper(self) -> 'Cloud_Output_Str':
+        Args:
+            table (Mapping[int, Union[Union[int, str, None], List[Union[int, str, None]]]]):
+
+        Returns:
+            Cloud_Output_Str
         """
-        Return a copy of S converted to uppercase.
+        self._operations.append(("translate", (table), {}))
 
-        Append the operation to the Cloud Output Object and return the same Cloud Output String object for any further operations.
+    def upper(self) -> "Cloud_Output_Str":
+        """Return a copy of S converted to uppercase.
+
+        Returns:
+            Cloud_Output_Str
         """
-        self._operations.append(
-            (
-                'upper', 
-                (), 
-                {}
-            )
-        )
+        self._operations.append(("upper", (), {}))
 
         return self
 
+    def zfill(self, width: SupportsIndex) -> "Cloud_Output_Str":
+        """Pad a numeric string S with zeros on the left, to fill a field of the specified width.
 
-    def zfill(self, width: SupportsIndex) -> 'Cloud_Output_Str':
-        """Pad a numeric string S with zeros on the left, to fill a field of the specified width. 
-        
-        Append the operation to the Cloud Output Object and return the same Cloud Output String object for any further operations.
-        
         The string S is never truncated.
+
+        Args:
+            width (SupportsIndex)
+
+        Returns:
+            Cloud_Output_Str
         """
-        self._operations.append(
-            (
-                'zfill', 
-                tuple([width]), 
-                {}
-            )
-        )
+        self._operations.append(("zfill", tuple([width]), {}))
 
         return self
 
 
 # Wrapper type to denote all the possible single value outputs
-T = TypeVar('T', Cloud_Output_Dynamic, Cloud_Output_Str, Cloud_Output_Int, Cloud_Output_Bool)
+T = TypeVar(
+    "T", Cloud_Output_Dynamic, Cloud_Output_Str, Cloud_Output_Int, Cloud_Output_Bool
+)
+
 
 class Cloud_Output_Sequence(Sequence, Cloud_Output_Dynamic, Generic[T]):
     """
     Cloud Output that will resolve to a Sequence of values after being retrieve or after all the operations have been executed
     """
-    def __init__(self, name: str, ruuid: str, key: str, type: OutputType, _member_class) -> None:
+
+    def __init__(
+        self, name: str, ruuid: str, key: str, type: OutputType, _member_class
+    ) -> None:
         super().__init__(name, ruuid, key, type)
 
         self._member_class = _member_class
 
     def __len__(self):
         raise Exception
 
     # Use these stub methods to define the typing signature so that the output is correct based on the input given
     @overload
-    def __getitem__(self, key: slice) -> 'Cloud_Output_Sequence[T]': 
+    def __getitem__(self, key: slice) -> "Cloud_Output_Sequence[T]":
         pass
 
     @overload
-    def  __getitem__(self, key: int) ->  T: 
+    def __getitem__(self, key: int) -> T:
         pass
 
     # implementation
     def __getitem__(self, key):
-        self._operations.append(
-                (
-                    '__getitem__',
-                    [key],
-                    {}
-                )
-            )  
-        
+        """Provides API for lazy evaluating __getitem__
+
+        Args:
+            key (_type_)
+
+        Raises:
+            Exception
+
+        Returns:
+            _type_
+        """
+        self._operations.append(("__getitem__", [key], {}))
+
         if isinstance(key, slice):
             return self
 
         elif isinstance(key, int):
-            rv = self._member_class(
-                self._name, self._ruuid, self._key, self._type
-            )
+            rv = self._member_class(self._name, self._ruuid, self._key, self._type)
 
             rv._operations = self._operations.copy()
 
             return rv
 
         else:
             raise Exception
 
-
     def __contains__(self, o: Any) -> Cloud_Output_Bool:
-        self._operations.append(
-            (
-                '__contains__',
-                [o],
-                {}
-            )
-        )
+        """Provides API for lazy evaluating __contains__
 
-        rv = Cloud_Output_Bool(
-            self._name, self._ruuid, self._key, self._type
-        )
+        Args:
+            o (Any)
+
+        Returns:
+            Cloud_Output_Bool
+        """
+        self._operations.append(("__contains__", [o], {}))
+
+        rv = Cloud_Output_Bool(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
-
     def __len__(self) -> Cloud_Output_Int:
-        self._operations.append(
-            (
-                '__len__',
-                [],
-                {}
-            )
-        )
+        """Provides API for lazy evaluating __len__
 
-        rv = Cloud_Output_Int(
-            self._name, self._ruuid, self._key, self._type
-        )
+        Returns:
+            Cloud_Output_Int
+        """
+        self._operations.append(("__len__", [], {}))
+
+        rv = Cloud_Output_Int(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
 
-
 class Cloud_Output_Mapping(Sequence, Cloud_Output_Dynamic, Generic[T]):
     """
     Cloud Output that will resolve to a Mapping of string to values (after being retrieved or after all the operations have been executed).
     """
-    def __init__(self, name: str, ruuid: str, key: str, type: OutputType, _member_class) -> None:
+
+    def __init__(
+        self, name: str, ruuid: str, key: str, type: OutputType, _member_class
+    ) -> None:
         super().__init__(name, ruuid, key, type)
 
         self._member_class = _member_class
 
     def __len__(self):
         raise Exception
 
-
     # implementation
-    def __getitem__(self, key: str) -> T: 
+    def __getitem__(self, key: str) -> T:
+        """Provides API for lazy evaluating __getitem__
+
+        Args:
+            key (str)
+
+        Raises:
+            Exception
+
+        Returns:
+            T
+        """
         if not isinstance(key, str):
             raise Exception
 
+        self._operations.append(("__getitem__", [key], {}))
 
-        self._operations.append(
-                (
-                    '__getitem__',
-                    [key],
-                    {}
-                )
-            )  
-        
-
-        rv = self._member_class(
-            self._name, self._ruuid, self._key, self._type
-        )
+        rv = self._member_class(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
 
-
     def __contains__(self, _o: str) -> Cloud_Output_Bool:
-        self._operations.append(
-            (
-                '__contains__',
-                [_o],
-                {}
-            )
-        )
+        """Provides API for lazy evaluating __contains__
 
-        rv = Cloud_Output_Bool(
-            self._name, self._ruuid, self._key, self._type
-        )
+        Args:
+            _o (str)
+
+        Returns:
+            Cloud_Output_Bool
+        """
+        self._operations.append(("__contains__", [_o], {}))
+
+        rv = Cloud_Output_Bool(self._name, self._ruuid, self._key, self._type)
 
         rv._operations = self._operations.copy()
 
         return rv
```

### Comparing `cdev-0.0.8/core/constructs/commands.py` & `cdev-0.0.9/core/constructs/commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """Structures for user defined command system
 
 One of the goals of the Core Framework is to provide flexibility such that end users can easily
 create custom functionality for their projects. One way of providing this flexibility, is to provide
-an easy interface for executing code from within the context of the framework from the CLI. This 
-process is heavily modeled and inspired by the `Django Command Framework` 
+an easy interface for executing code from within the context of the framework from the CLI. This
+process is heavily modeled and inspired by the `Django Command Framework`
 (https://github.com/django/django/blob/b0ed619303d2fb723330ca9efa3acf23d49f1d19/django/core/management/base.py).
 
 The main primitive is the `BaseCommand` class. By deriving from this class, developers can create code
-that is easily accessible and discoverable from the command line. To see how these class are discovered 
+that is easily accessible and discoverable from the command line. To see how these class are discovered
 and execute see our more in depth documentation on the command system at <link>
 
 """
 
 import os
 from argparse import ArgumentParser, HelpFormatter
 import sys
 from io import TextIOBase
+from typing import Tuple
+
 from rich.console import Console
 
 
 class CdevCommandError(BaseException):
     """Base exception Class
 
     Exception class indicating a problem while executing a management
@@ -57,136 +59,141 @@
     }
 
     def _reordered_actions(self, actions):
         return sorted(
             actions, key=lambda a: set(a.option_strings) & self.show_last != set()
         )
 
-    def add_usage(self, usage, actions, *args, **kwargs):
+    def add_usage(self, usage, actions, *args, **kwargs) -> None:
         super().add_usage(usage, self._reordered_actions(actions), *args, **kwargs)
 
-    def add_arguments(self, actions):
+    def add_arguments(self, actions) -> None:
         super().add_arguments(self._reordered_actions(actions))
 
 
 class OutputWrapper(TextIOBase):
     """
     Wrapper around stdout/stderr
     """
 
     @property
     def style_func(self):
         return self._style_func
 
     @style_func.setter
-    def style_func(self, style_func):
+    def style_func(self, style_func) -> None:
         if style_func and self.isatty():
             self._style_func = style_func
         else:
             self._style_func = lambda x: x
 
-    def __init__(self, out, ending="\n"):
+    def __init__(self, out, ending="\n") -> None:
         self._out = out
         self.style_func = None
         self.ending = ending
 
     def __getattr__(self, name):
         return getattr(self._out, name)
 
-    def flush(self):
+    def flush(self) -> None:
         if hasattr(self._out, "flush"):
             self._out.flush()
 
-    def isatty(self):
+    def isatty(self) -> bool:
         return hasattr(self._out, "isatty") and self._out.isatty()
 
-    def write(self, msg="", style_func=None, ending=None):
+    def write(self, msg="", style_func=None, ending=None) -> None:
         ending = self.ending if ending is None else ending
         if ending and not msg.endswith(ending):
             msg += ending
         style_func = style_func or self.style_func
         self._out.write(style_func(msg))
 
 
 class ConsoleOutputWrapper(TextIOBase):
     """
-    Wrapper around a `rich` console. 
+    Wrapper around a `rich` console.
     """
 
     @property
     def style_func(self):
         return self._style_func
 
     @style_func.setter
-    def style_func(self, style_func):
+    def style_func(self, style_func) -> None:
         if style_func and self.isatty():
             self._style_func = style_func
         else:
             self._style_func = lambda x: x
 
-    def __init__(self, console: Console, ending="\n"):
+    def __init__(self, console: Console, ending="\n") -> None:
         self._out = console
         self.style_func = None
         self.ending = ending
 
     def __getattr__(self, name):
         return getattr(self._out, name)
 
-    def flush(self):
+    def flush(self) -> None:
         self._out.clear()
 
-    def isatty(self):
+    def isatty(self) -> bool:
         return self._out.is_terminal
 
-    def write(self, msg: str ="", style_func=None, ending=None):
+    def write(self, msg: str = "", style_func=None, ending=None) -> None:
         ending = self.ending if ending is None else ending
         if ending and not msg.endswith(ending):
             msg += ending
         style_func = style_func or self.style_func
         self._out.print(style_func(msg))
 
 
-
 class BaseCommand:
-    """Base Class for a user defined command
-    
-    """
+    """Base Class for a user defined command"""
 
     # Help message for this command
     help = ""
 
     # If this command requires the project to have been initialized
     requires_initialized_workspace = True
 
     # If the command should look to substitute args with cloud output values
     substitute_from_output = True
 
-    def __init__(self, stdout: Console = None, stderr: Console = None, no_color=False, force_color=False):
-        self.stdout = ConsoleOutputWrapper(stdout) if stdout else OutputWrapper(sys.stdout)
-        self.stderr = ConsoleOutputWrapper(stderr) if stderr else OutputWrapper(sys.stderr)
+    def __init__(
+        self,
+        stdout: Console = None,
+        stderr: Console = None,
+        no_color=False,
+        force_color=False,
+    ) -> None:
+        self.stdout = (
+            ConsoleOutputWrapper(stdout) if stdout else OutputWrapper(sys.stdout)
+        )
+        self.stderr = (
+            ConsoleOutputWrapper(stderr) if stderr else OutputWrapper(sys.stderr)
+        )
 
     def create_arg_parser(self, prog_name, subcommand, **kwargs) -> ArgumentParser:
         parser = ArgumentParser(
             prog="%s %s" % (os.path.basename(prog_name), subcommand),
             description=self.help or None,
             formatter_class=CdevHelpFormatter,
             **kwargs
         )
 
         self.add_arguments(parser)
 
         return parser
 
-    def add_arguments(self, parser: ArgumentParser):
-        """Add the cli arguments for the command
-        
-        """
+    def add_arguments(self, parser: ArgumentParser) -> None:
+        """Add the cli arguments for the command"""
         pass
 
-    def run_from_command_line(self, argv):
+    def run_from_command_line(self, argv) -> None:
         """
         Handles input from command line and builds arg parser and uses it to validate input.
 
         argv -> [program_name, command, *args]
 
         program_name: represents where to find the command
         command: command to run
@@ -202,35 +209,59 @@
 
         try:
             self.command(*args, **cmd_options)
         except CdevCommandError as e:
             self.stderr.write("%s: %s" % (e.__class__.__name__, e))
             sys.exit(e.returncode)
 
-    def command(self, *args, **kwargs):
+    def command(self, *args, **kwargs) -> None:
         """
         The actual logic of the command. Subclasses must implement
         this method.
         """
         raise NotImplementedError(
             "subclasses of BaseCommand must provide a command() method"
         )
 
+    def get_component_and_resource_from_qualified_name(self,
+                                                       full_name: str,
+                                                       ) -> Tuple[str, str]:
+        if full_name is None:
+            raise Exception("Invalid arguments provided to get resource detail")
+
+        component_and_function = full_name.split(".")
+        if len(component_and_function) != 2:
+            raise Exception(f"Could not get resource detail from {full_name}")
+
+        component_name = full_name.split(".")[0]
+        resource_name = full_name.split(".")[1]
+        return component_name, resource_name
+
 
 class BaseCommandContainer:
     """
     This is used to designate that the directory is a CommandContainer and should be searched for when looking for commands.
 
     This class should be initialized in the __init__.py file for the folder.
 
     The directory should contain valid Commands or other CommandContainers
     """
 
     # Help message for this container
     help = ""
 
-    def __init__(self, stdout: Console = None, stderr: Console = None, no_color=False, force_color=False):
-        self.stdout = ConsoleOutputWrapper(stdout) if stdout else OutputWrapper(sys.stdout)
-        self.stderr = ConsoleOutputWrapper(stderr) if stderr else OutputWrapper(sys.stderr)
+    def __init__(
+        self,
+        stdout: Console = None,
+        stderr: Console = None,
+        no_color=False,
+        force_color=False,
+    ) -> None:
+        self.stdout = (
+            ConsoleOutputWrapper(stdout) if stdout else OutputWrapper(sys.stdout)
+        )
+        self.stderr = (
+            ConsoleOutputWrapper(stderr) if stderr else OutputWrapper(sys.stderr)
+        )
 
-    def display_help_message(self) -> str:
+    def display_help_message(self) -> None:
         self.stdout.write(self.help)
```

### Comparing `cdev-0.0.8/core/constructs/components.py` & `cdev-0.0.9/core/constructs/components.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Structure that encapsulates a namespace of deploy resources
 
 Properties of a component:
 []
 """
 
 from enum import Enum
-from typing import Dict, Union, List, Optional, Set
+from typing import Dict, List, Optional
 
 
 from pydantic import BaseModel
 
 from .resource import ResourceReferenceModel, ResourceModel
 
 
@@ -26,26 +26,25 @@
                 it changes only if a change in the state is desired.
 
     - name  ->  a string that is the human readable name for this component
     """
 
     name: str
     """
-    A human readable logical name for the component. 
+    A human readable logical name for the component.
 
-    This value is important for allow human level refactoring of components. To update a component name once created, you must edit only the 
-    name and not change the hash. If you change both the hash and name in the same deployment, it will register this as a delete and create 
-    instead of update. 
+    This value is important for allow human level refactoring of components. To update a component name once created, you must edit only the
+    name and not change the hash. If you change both the hash and name in the same deployment, it will register this as a delete and create
+    instead of update.
     """
 
-
     hash: str
     """
     A hash that is used to identify if changes in the resources have occurred. It should have the property:
-    - This value changes only if a there is a change in the resource. 
+    - This value changes only if a there is a change in the resource.
     """
 
     resources: Optional[List[ResourceModel]]
     """
     List of Rendered Resources that make up the current state of this component
     """
 
@@ -72,27 +71,26 @@
     def __init__(
         __pydantic_self__,
         name: str,
         hash: str = "0",
         resources: List[ResourceModel] = [],
         references: List[ResourceReferenceModel] = [],
         cloud_output: Dict[str, Dict] = {},
-        previous_resolved_cloud_values: Dict[str, Dict]={},
+        previous_resolved_cloud_values: Dict[str, Dict] = {},
         external_references: Dict[str, Dict] = {},
     ) -> None:
         super().__init__(
             **{
                 "name": name,
                 "hash": hash,
                 "resources": list(resources),
                 "references": list(references),
                 "cloud_output": dict(cloud_output),
                 "previous_resolved_cloud_values": dict(previous_resolved_cloud_values),
                 "external_references": dict(external_references),
-
             }
         )
 
 
 class Component_Change_Type(str, Enum):
     CREATE = "CREATE"
     UPDATE_NAME = "UPDATE_NAME"
@@ -117,30 +115,29 @@
                 "previous_name": previous_name,
                 "new_name": new_name,
             }
         )
 
     class Config:
         use_enum_values = True
-        # Beta Feature but should be fine since this is simple data 
+        # Beta Feature but should be fine since this is simple data
         frozen = True
 
 
-
 class Component:
     """
     A component is a logical collection of resources. This simple definition is intended to allow flexibility for different
     styles of setup. It is up to the end user to decide on how they group the resources.
 
     A component must override the `render` method, which returns the desired resources with configuration as a component model.
     The `render` method does not take any input parameters, therefore all configuration for the component should be done via the `__init__`
     method or other defined methods.
     """
 
-    def __init__(self, name: str):
+    def __init__(self, name: str) -> None:
         self.name = name
 
     def render(self) -> ComponentModel:
         """Abstract Class that must be implemented by the descendant that returns a component model"""
         raise NotImplementedError
 
     def get_name(self) -> str:
```

### Comparing `cdev-0.0.8/core/constructs/models.py` & `cdev-0.0.9/core/constructs/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
     sequence_like,
 )
 
 from pydantic.typing import (
     is_namedtuple,
 )
 
-from typing import  Any
+from typing import Any
 
-class frozendict(Mapping):
 
+class frozendict(Mapping):
     def __init__(self, d: dict):
         self._d = d
 
     def __iter__(self):
         return iter(self._d)
 
     def __len__(self):
@@ -35,74 +35,78 @@
 
     @classmethod
     def __get_validators__(cls):
         yield cls.validate
 
     @classmethod
     def validate(cls, v):
-        
-        if not (isinstance(v, frozendict)) :
-            
-            raise TypeError(f'{v} Not Frozen Dict')
+
+        if not (isinstance(v, frozendict)):
+
+            raise TypeError(f"{v} Not Frozen Dict")
 
         return v
-    
+
     def __repr__(self) -> str:
         return f"FrozenDict({self._d})"
 
 
 class ImmutableModel(BaseModel):
     @classmethod
     def _get_value(
         cls,
         v: Any,
         to_dict: bool,
         by_alias: bool,
-        include ,
+        include,
         exclude,
         exclude_unset: bool,
         exclude_defaults: bool,
         exclude_none: bool,
     ) -> Any:
 
         if isinstance(v, BaseModel):
             if to_dict:
-                v_dict = frozendict( v.dict(
-                    by_alias=by_alias,
-                    exclude_unset=exclude_unset,
-                    exclude_defaults=exclude_defaults,
-                    include=include,
-                    exclude=exclude,
-                    exclude_none=exclude_none,
-                ))
+                v_dict = frozendict(
+                    v.dict(
+                        by_alias=by_alias,
+                        exclude_unset=exclude_unset,
+                        exclude_defaults=exclude_defaults,
+                        include=include,
+                        exclude=exclude,
+                        exclude_none=exclude_none,
+                    )
+                )
                 if ROOT_KEY in v_dict:
                     return v_dict[ROOT_KEY]
                 return v_dict
             else:
                 return v.copy(include=include, exclude=exclude)
 
         value_exclude = ValueItems(v, exclude) if exclude else None
         value_include = ValueItems(v, include) if include else None
 
         if isinstance(v, dict):
-            return frozendict( {
-                k_: cls._get_value(
-                    v_,
-                    to_dict=to_dict,
-                    by_alias=by_alias,
-                    exclude_unset=exclude_unset,
-                    exclude_defaults=exclude_defaults,
-                    include=value_include and value_include.for_element(k_),
-                    exclude=value_exclude and value_exclude.for_element(k_),
-                    exclude_none=exclude_none,
-                )
-                for k_, v_ in v.items()
-                if (not value_exclude or not value_exclude.is_excluded(k_))
-                and (not value_include or value_include.is_included(k_))
-            })
+            return frozendict(
+                {
+                    k_: cls._get_value(
+                        v_,
+                        to_dict=to_dict,
+                        by_alias=by_alias,
+                        exclude_unset=exclude_unset,
+                        exclude_defaults=exclude_defaults,
+                        include=value_include and value_include.for_element(k_),
+                        exclude=value_exclude and value_exclude.for_element(k_),
+                        exclude_none=exclude_none,
+                    )
+                    for k_, v_ in v.items()
+                    if (not value_exclude or not value_exclude.is_excluded(k_))
+                    and (not value_include or value_include.is_included(k_))
+                }
+            )
 
         elif sequence_like(v):
             seq_args = (
                 cls._get_value(
                     v_,
                     to_dict=to_dict,
                     by_alias=by_alias,
@@ -112,22 +116,23 @@
                     exclude=value_exclude and value_exclude.for_element(i),
                     exclude_none=exclude_none,
                 )
                 for i, v_ in enumerate(v)
                 if (not value_exclude or not value_exclude.is_excluded(i))
                 and (not value_include or value_include.is_included(i))
             )
-            
-            return v.__class__(*seq_args) if is_namedtuple(v.__class__) else v.__class__(seq_args)
 
-        elif isinstance(v, Enum) and getattr(cls.Config, 'use_enum_values', False):
+            return (
+                v.__class__(*seq_args)
+                if is_namedtuple(v.__class__)
+                else v.__class__(seq_args)
+            )
+
+        elif isinstance(v, Enum) and getattr(cls.Config, "use_enum_values", False):
             return v.value
 
         else:
             return v
 
     class Config:
         extra = "allow"
         frozen = True
-
-
-
```

### Comparing `cdev-0.0.8/core/constructs/output_manager.py` & `cdev-0.0.9/core/constructs/output_manager.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,143 +3,158 @@
 
 
 """
 
 from rich.console import Console
 from typing import Any, List, Tuple, Union
 
-from rich.progress import Progress, TaskID  
+from rich.progress import Progress, TaskID
 
-from core.constructs.components import Component_Change_Type, ComponentModel, Component_Difference
-from core.constructs.resource import Resource_Change_Type, Resource_Difference, Resource_Reference_Change_Type, Resource_Reference_Difference
+from core.constructs.components import (
+    Component_Change_Type,
+    ComponentModel,
+    Component_Difference,
+)
+from core.constructs.resource import (
+    Resource_Change_Type,
+    Resource_Difference,
+    Resource_Reference_Change_Type,
+    Resource_Reference_Difference,
+)
+
+
+class OutputManager:
+    def __init__(self, console: Console = None, progress: Progress = None) -> None:
+        """Initialize the Output Manager
 
-class OutputManager():
-    def __init__(self, console: Console=None, progress: Progress=None) -> None:
-
-        if console:
-            self._console = console
-        else:
-            self._console = Console()
-
-        if progress:
-            self._progress = progress
-        else:
-            self._progress = None
+        Args:
+            console (Console, optional): Defaults to None.
+            progress (Progress, optional): Defaults to None.
+        """
+        self._console = console or Console()
+        self._progress = progress
 
+    def print_header(self, resource_state_uuid: str) -> None:
+        """Print the header of the output
 
-    def print_header(self, resource_state_uuid: str):        
+        Args:
+            resource_state_uuid (str)
+        """
         print(f"Resource State: {resource_state_uuid}")
-
         print("")
 
+    def print_local_state(self, rendered_components: List[ComponentModel]) -> None:
+        """Print the current state
 
-    def print_local_state(self, rendered_components: List[ComponentModel]):
-
+        Args:
+            rendered_components (List[ComponentModel])
+        """
         rendered_components.sort(key=lambda x: x.name)
-        
+
         self._console.print(f"Current State:")
         for component in rendered_components:
             self._console.print(f"Component: [bold blue]{component.name}[/bold blue]")
-
-            if component.resources:
-                self._console.print(f"    Resources:")
-                for resource in component.resources:
-                    self._console.print(f"        [bold blue]{resource.name} ({resource.ruuid})[/bold blue]")
-
-
-            if component.references:
-                self._console.print(f"    References:")
-                for reference in component.references:
-                    self._console.print(f"        [bold blue]From {reference.component_name} reference {reference.name} ({reference.ruuid})[/bold blue]")
+            self._print_component_resources(component)
+            self._print_component_references(component)
 
         self._console.print("")
 
+    def print_components_to_diff_against(self, old_component_names: List[str]) -> None:
+        """Print the component names we are diffing against
 
-    def print_components_to_diff_against(self, old_component_names: List[str]):
+        Args:
+            old_component_names (List[str])
+        """
 
         self._console.print("Components to diff against:")
         for component_name in old_component_names:
             self._console.print(f"    {component_name}")
 
-
         self._console.print("")
 
+    def print_state_differences(
+        self,
+        differences: Tuple[
+            List[Component_Difference],
+            List[Resource_Difference],
+            List[Resource_Reference_Difference],
+        ],
+    ) -> None:
+        """Print the differences in a state
+
+        Args:
+            differences (Tuple[ List[Component_Difference], List[Resource_Difference], List[Resource_Reference_Difference], ])
+        """
+        if not any(differences):
+            return
 
-    def print_state_differences(self, differences: Tuple[List[Component_Difference], List[Resource_Difference], List[Resource_Reference_Difference]]):
         component_differences = differences[0]
         resource_differences = differences[1]
         reference_differences = differences[2]
 
-
         self._console.print(f"[bold white]Differences in State:[/bold white]")
 
         for component_diff in component_differences:
-            if component_diff.action_type == Component_Change_Type.UPDATE_NAME:
-                self._console.print(f"    [bold yellow]Update Name: [/bold yellow][bold blue]{component_diff.previous_name} to {component_diff.new_name} (component)[/bold blue]")
-                continue
-
-            elif component_diff.action_type == Component_Change_Type.UPDATE_IDENTITY:
-                self._console.print(f"    [bold yellow]Update Identity: [/bold yellow][bold blue]{component_diff.new_name} (component)[/bold blue]")
-
-            elif component_diff.action_type == Component_Change_Type.CREATE:
-                self._console.print(f"    [bold green]Create: [/bold green][bold blue]{component_diff.new_name} (component)[/bold blue]")
-
-            elif component_diff.action_type == Component_Change_Type.DELETE:
-                self._console.print(f"    [bold red]Delete: [/bold red] [bold blue]{component_diff.previous_name} (component)[/bold blue]")
-
-
-            resource_changes = [x for x in resource_differences if x.component_name == component_diff.new_name or x.component_name == component_diff.previous_name ]
-
-            if resource_changes:
-                for resource_diff in resource_changes:
-                    if resource_diff.action_type == Resource_Change_Type.CREATE:
-                        self._console.print(f"        [bold green]Create:[/bold green][bold blue] {resource_diff.new_resource.name} ({resource_diff.new_resource.ruuid})[/bold blue]")
-
-                    elif resource_diff.action_type == Resource_Change_Type.DELETE:
-                        self._console.print(f"        [bold red]Delete:[/bold red][bold blue] {resource_diff.previous_resource.name} ({resource_diff.previous_resource.ruuid})[/bold blue]")
-
-                    elif resource_diff.action_type == Resource_Change_Type.UPDATE_IDENTITY:
-                        self._console.print(f"        [bold yellow]Update:[/bold yellow][bold blue] {resource_diff.new_resource.name} ({resource_diff.new_resource.ruuid})[/bold blue]")
-
-                    elif resource_diff.action_type == Resource_Change_Type.UPDATE_NAME:
-                        self._console.print(f"        [bold yellow]Update Name:[/bold yellow][bold blue] from {resource_diff.previous_resource.name} to {resource_diff.new_resource.name} ({resource_diff.new_resource.ruuid})[/bold blue]")
-
-
-            reference_changes = [x for x in reference_differences if x.originating_component_name == component_diff.new_name]
-
-            if reference_changes:
-                for reference_diff in reference_changes:
-                    if reference_diff.action_type == Resource_Reference_Change_Type.CREATE:
-                        self._console.print(f"        [bold green]Create reference:[/bold green][bold blue] {reference_diff.resource_reference.name} ({reference_diff.resource_reference.ruuid}) from {reference_diff.originating_component_name}[/bold blue]")
-
-                    elif reference_diff.action_type == Resource_Reference_Change_Type.DELETE:
-                        self._console.print(f"        [bold red]Delete reference:[/bold red][bold blue] {reference_diff.resource_reference.name} ({reference_diff.resource_reference.ruuid}) from {reference_diff.originating_component_name}[/bold blue]")
-
-
-    def create_task(self, description: str, start: bool = True, total: int = 100, completed: int = 0, visible: bool = True, **fields: Any) -> 'OutputTask':
-        """Create a task for the progress object in this output manager. 
+            self._print_component_differences(component_diff)
+            self._print_component_resource_differences(
+                component_diff, resource_differences
+            )
+            self._print_component_reference_differences(
+                component_diff, reference_differences
+            )
+
+    def create_task(
+        self,
+        description: str,
+        start: bool = True,
+        total: int = 100,
+        completed: int = 0,
+        visible: bool = True,
+        **fields: Any,
+    ) -> "OutputTask":
+        """Create a task for the progress object in this output manager.
 
         Raises:
-            Exception: [description]
+            Exception
 
         Returns:
             OutputTask: Object to use to track the progress of the event
         """
 
-
         if not self._progress:
             raise Exception
 
-
-        task_id = self._progress.add_task(description=description, start=start, total=total, completed=completed, visible=visible, **fields)
+        task_id = self._progress.add_task(
+            description=description,
+            start=start,
+            total=total,
+            completed=completed,
+            visible=visible,
+            **fields,
+        )
 
         return OutputTask(self, task_id)
 
+    def create_output_description(
+        self,
+        node: Union[
+            Resource_Difference, Resource_Reference_Difference, Component_Difference
+        ],
+    ) -> str:
+        """Create a label for a given difference
 
-    def create_output_description(self, node: Union[Resource_Difference, Resource_Reference_Difference, Component_Difference]) -> str:
+        Args:
+            node (Union[ Resource_Difference, Resource_Reference_Difference, Component_Difference ])
+
+        Raises:
+            Exception
+
+        Returns:
+            str
+        """
         if isinstance(node, Resource_Difference):
             if node.action_type == Resource_Change_Type.CREATE:
                 return f"[bold green]Creating:[/bold green][bold blue] {node.new_resource.name} ({node.new_resource.ruuid})[/bold blue]"
 
             elif node.action_type == Resource_Change_Type.DELETE:
                 return f"[bold red]Deleting:[/bold red][bold blue] {node.previous_resource.name} ({node.previous_resource.ruuid})[/bold blue]"
 
@@ -166,49 +181,209 @@
             elif node.action_type == Component_Change_Type.CREATE:
                 return f"[bold green]Create: [/bold green][bold blue]{node.new_name} (component)[/bold blue]"
 
             elif node.action_type == Component_Change_Type.DELETE:
                 return f"[bold red]Delete: [/bold red] [bold blue]{node.previous_name} (component)[/bold blue]"
 
         else:
-            raise Exception(f"Trying to deploy node {node} but it is not a correct type ")
+            raise Exception(
+                f"Trying to deploy node {node} but it is not a correct type "
+            )
+
+
+    def _print_component_resources(self, component: ComponentModel) -> None:
+        """Print the resources in a component
+
+        Args:
+            component (ComponentModel)
+        """
+        if component.resources is None or not any(component.resources):
+            self._console.print(f"        [bold blue] No Resources")
+            return
+
+        for resource in component.resources:
+            self._console.print(
+                f"        [bold blue]{resource.name} ({resource.ruuid})[/bold blue]"
+            )
+
+
+    def _print_component_references(self, component: ComponentModel) -> None:
+        """Print the references in a component
+
+        Args:
+            component (ComponentModel)
+        """
+
+        if component.references is None or not any(component.references):
+            self._console.print(f"        [bold blue] No References")
+            return
+
+        for reference in component.references:
+            self._console.print(
+                f"        [bold blue]From {reference.component_name} reference {reference.name} ({reference.ruuid})[/bold blue]"
+            )
+
+    def _print_component_differences(
+        self, component_diff: Component_Difference
+    ) -> None:
+        """Print the details in a component difference
+
+        Args:
+            component_diff (Component_Difference)
+        """
+        if component_diff.action_type == Component_Change_Type.UPDATE_NAME:
+            self._console.print(
+                f"    [bold yellow]Update Name: [/bold yellow][bold blue]{component_diff.previous_name} to {component_diff.new_name} (component)[/bold blue]"
+            )
+            return
+
+        if component_diff.action_type == Component_Change_Type.UPDATE_IDENTITY:
+            self._console.print(
+                f"    [bold yellow]Update Identity: [/bold yellow][bold blue]{component_diff.new_name} (component)[/bold blue]"
+            )
+            return
+
+        if component_diff.action_type == Component_Change_Type.CREATE:
+            self._console.print(
+                f"    [bold green]Create: [/bold green][bold blue]{component_diff.new_name} (component)[/bold blue]"
+            )
+            return
+
+        if component_diff.action_type == Component_Change_Type.DELETE:
+            self._console.print(
+                f"    [bold red]Delete: [/bold red] [bold blue]{component_diff.previous_name} (component)[/bold blue]"
+            )
+        return
+
+    def _print_component_resource_differences(
+        self,
+        component_diff: Component_Difference,
+        resource_differences: List[Resource_Difference],
+    ) -> None:
+        """Print details of the resource differences in the component
+
+        Args:
+            component_diff (Component_Difference)
+            resource_differences (List[Resource_Difference])
+        """
+        resource_changes = [
+            x
+            for x in resource_differences
+            if x.component_name == component_diff.new_name
+            or x.component_name == component_diff.previous_name
+        ]
+
+        for resource_diff in resource_changes:
+            if resource_diff.action_type == Resource_Change_Type.CREATE:
+                self._console.print(
+                    f"        [bold green]Create:[/bold green][bold blue] {resource_diff.new_resource.name} ({resource_diff.new_resource.ruuid})[/bold blue]"
+                )
+
+            elif resource_diff.action_type == Resource_Change_Type.DELETE:
+                self._console.print(
+                    f"        [bold red]Delete:[/bold red][bold blue] {resource_diff.previous_resource.name} ({resource_diff.previous_resource.ruuid})[/bold blue]"
+                )
+
+            elif resource_diff.action_type == Resource_Change_Type.UPDATE_IDENTITY:
+                self._console.print(
+                    f"        [bold yellow]Update:[/bold yellow][bold blue] {resource_diff.new_resource.name} ({resource_diff.new_resource.ruuid})[/bold blue]"
+                )
+
+            elif resource_diff.action_type == Resource_Change_Type.UPDATE_NAME:
+                self._console.print(
+                    f"        [bold yellow]Update Name:[/bold yellow][bold blue] from {resource_diff.previous_resource.name} to {resource_diff.new_resource.name} ({resource_diff.new_resource.ruuid})[/bold blue]"
+                )
+
+    def _print_component_reference_differences(
+        self,
+        component_diff: Component_Difference,
+        reference_differences: List[Resource_Reference_Difference],
+    ) -> None:
+        """Print the details in the reference differences
+
+        Args:
+            component_diff (Component_Difference)
+            reference_differences (List[Resource_Reference_Difference])
+        """
+        reference_changes = [
+            x
+            for x in reference_differences
+            if x.originating_component_name == component_diff.new_name
+        ]
+
+        for reference_diff in reference_changes:
+            if reference_diff.action_type == Resource_Reference_Change_Type.CREATE:
+                self._console.print(
+                    f"        [bold green]Create reference:[/bold green][bold blue] {reference_diff.resource_reference.name} ({reference_diff.resource_reference.ruuid}) from {reference_diff.originating_component_name}[/bold blue]"
+                )
+
+            elif reference_diff.action_type == Resource_Reference_Change_Type.DELETE:
+                self._console.print(
+                    f"        [bold red]Delete reference:[/bold red][bold blue] {reference_diff.resource_reference.name} ({reference_diff.resource_reference.ruuid}) from {reference_diff.originating_component_name}[/bold blue]"
+                )
 
 
-class OutputTask():
+class OutputTask:
     """
     Wrapper around an output that can be used to track long running events. The implementation is as a wrapper around a 'progress task' from the
     rich library. Thus, the api for 'update' and 'start' follows the same pattern as that of a 'task' in the rich library. The print method provides
-    access for sending messages to the parent console of this task. 
-    """  
+    access for sending messages to the parent console of this task.
+    """
 
     def __init__(self, output_manager: OutputManager, task_id: TaskID) -> None:
         self._output_manager = output_manager
         self._task_id = task_id
 
-    
-    def print(self, msg: str):
+    def print(self, msg: str) -> None:
         """Print a message to the parent output context.
 
         Args:
             msg (str): message to print
         """
         self._output_manager._console.print(msg)
 
-
-    def print_error(self, msg: str):
+    def print_error(self, msg: str) -> None:
         """
         Print a message as an error
 
         Args:
             msg (str): error message
         """
         self.print(f"[bold red]{msg}[/bold red]")
 
+    def update(
+        self,
+        *args,
+        total: float = None,
+        completed: float = None,
+        advance: None = None,
+        description: str = None,
+        visible: bool = None,
+        refresh: bool = False,
+        **fields: Any,
+    ) -> None:
+        """Update the output tasks
 
+        Args:
+            total (float, optional): Defaults to None.
+            completed (float, optional): Defaults to None.
+            advance (None, optional): Defaults to None.
+            description (str, optional): Defaults to None.
+            visible (bool, optional): Defaults to None.
+            refresh (bool, optional): Defaults to False.
+        """
+        # self._output_manager._console.print(fields.get('comment'))
+        self._output_manager._progress.update(
+            self._task_id,
+            *args,
+            total=total,
+            completed=completed,
+            advance=advance,
+            description=description,
+            visible=visible,
+            refresh=refresh,
+            **fields,
+        )
 
-    def update(self, *args, total: float = None, completed: float = None, advance: None = None, description: str = None, visible: bool = None, refresh: bool = False, **fields: Any):
-        #self._output_manager._console.print(fields.get('comment'))
-        self._output_manager._progress.update(self._task_id, *args, total=total, completed=completed, advance=advance, description=description, visible=visible, refresh=refresh, **fields)
-
-
-    def start_task(self):
+    def start_task(self) -> None:
+        """Start the given task progress bar"""
         self._output_manager._progress.start_task(self._task_id)
```

### Comparing `cdev-0.0.8/core/constructs/resource.py` & `cdev-0.0.9/core/constructs/resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 """Structures for representing cloud resources and references within the framework
 
 """
 from functools import wraps
-from typing import Dict, TypeVar, Union, List, Optional, Set, Callable, Any
+from typing import List, Optional, Any
 
 from enum import Enum
 
 from core.constructs.models import ImmutableModel
 from core.constructs.cloud_output import OutputType, Cloud_Output_Str
 from core.constructs.types import F
+from core.utils.hasher import hash_list
 
-from ..utils.hasher import hash_list
 
-    
 ##################
 ##### Resource
 ##################
 class ResourceModel(ImmutableModel):
     """Base class with basic information about a defined resource.
-    
-    All classes derived from this should contain additional information about the state of a resource. 
+
+    All classes derived from this should contain additional information about the state of a resource.
     Within the life cycle of the Cdev Core framework,this is used to represent resources after any
     configuration; hence the need to make these immutable data
-    classes. 
+    classes.
 
     Attributes:
-        name: The name of the resource. Note that the combination of a name and ruuid should be unique 
+        name: The name of the resource. Note that the combination of a name and ruuid should be unique
           within a namespace
         ruuid: The identifier of this resource type.
-        hash: A string that is the hash of this object. This hash must be computed such that it changes 
+        hash: A string that is the hash of this object. This hash must be computed such that it changes
           only if a change in the state is desired.
     """
 
     name: str
     """
     This is a human readable logical name for the resource. This must be unique for the resource within the namespace and resource type
     (i.e. the concat value of <ruuid>:<name> must be unique)
 
-    This value is important for allow human level refactoring of resources. To update a resources name once created, you must edit only the 
-    name and not change the hash. If you change both the hash and name in the same deployment, it will register this as a delete and create 
-    instead of update. 
+    This value is important for allow human level refactoring of resources. To update a resources name once created, you must edit only the
+    name and not change the hash. If you change both the hash and name in the same deployment, it will register this as a delete and create
+    instead of update.
     """
 
     ruuid: str
     """
     Name space identifier that is used to pass this resource to a downstream mapper
 
     Form: (top-level-namespace)::(resource-type-id)
@@ -85,27 +84,28 @@
                 "previous_resource": previous_resource,
                 "new_resource": new_resource,
             }
         )
 
     class Config:
         use_enum_values = True
-        # Beta Feature but should be fine since this is simple data 
+        # Beta Feature but should be fine since this is simple data
         frozen = True
 
 
 def update_hash(func: F) -> F:
     """Wrap a function that modifies the state of a Resource so that the hash is properly updated when a change occurs.
 
     Args:
         func (F): State modifying method.
 
     Returns:
         F: Wrapped function to compute new hash after changes have been made
     """
+
     @wraps(func)
     def wrapped_func(resource: "Resource", *func_posargs, **func_kwargs):
         rv = func(resource, *func_posargs, **func_kwargs)
         resource.compute_hash()
         return rv
 
     return wrapped_func
@@ -118,94 +118,96 @@
         self._hash = None
         self._nonce = nonce
 
     def render(self) -> ResourceModel:
         raise NotImplementedError
 
     @property
-    def name(self):
+    def name(self) -> str:
         """The name of the created resource"""
         return self._name
 
     @name.setter
-    def name(self, value: str):
+    def name(self, value: str) -> None:
         raise Exception("The Name of a resource can only be set when initialized.")
 
     @property
-    def ruuid(self):
+    def ruuid(self) -> str:
         """The ruuid of the created resource"""
         return self._ruuid
 
     @ruuid.setter
-    def ruuid(self, value: str):
+    def ruuid(self, value: str) -> None:
         raise Exception("The Ruuid of a resource can only be set when initialized.")
 
     @property
-    def nonce(self):
+    def nonce(self) -> str:
         """The nonce of the created resource"""
         return self._nonce
 
     @nonce.setter
-    def nonce(self, value: str):
+    def nonce(self, value: str) -> None:
         raise Exception("The nonce of a resource can only be set when initialized.")
 
     @property
-    def hash(self):
+    def hash(self) -> str:
         """The cdev hash of the resource"""
         if self._hash is None:
             raise Exception
 
         return self._hash
 
     @hash.setter
-    def hash(self, value: str):
-        raise Exception("The `hash` of a Resource can only be set by the `compute_hash` method")
+    def hash(self, value: str) -> None:
+        raise Exception(
+            "The `hash` of a Resource can only be set by the `compute_hash` method"
+        )
 
     def compute_hash(self):
         raise NotImplementedError
 
 
-class ResourceOutputs():
+class ResourceOutputs:
     """Container object for the returned values from the cloud after the resource has been deployed."""
+
     OUTPUT_TYPE = OutputType.RESOURCE
 
     def __init__(self, name: str, ruuid: str) -> None:
         self._name = name
         self._ruuid = ruuid
 
     @property
-    def cloud_id(self) -> 'Cloud_Output_Str':
+    def cloud_id(self) -> "Cloud_Output_Str":
         return Cloud_Output_Str(
-            name=self._name,
-            ruuid=self._ruuid,
-            key='cloud_id',
-            type=self.OUTPUT_TYPE
+            name=self._name, ruuid=self._ruuid, key="cloud_id", type=self.OUTPUT_TYPE
         )
 
     @cloud_id.setter
     def cloud_id(self, value: Any):
         raise Exception
 
     @property
-    def cloud_region(self) -> 'Cloud_Output_Str':
+    def cloud_region(self) -> "Cloud_Output_Str":
         return Cloud_Output_Str(
             name=self._name,
             ruuid=self._ruuid,
-            key='cloud_region',
-            type=self.OUTPUT_TYPE
+            key="cloud_region",
+            type=self.OUTPUT_TYPE,
         )
 
     @cloud_region.setter
     def cloud_region(self, value: Any):
         raise Exception
 
+
 ##################
 ##### Reference
 ##################
 
+
 class ResourceReferenceModel(ImmutableModel):
     """
     This is the information needed to reference a resource that is defined outside this component
 
     --- Attributes ---
 
     - ruuid ->  a string that represents the resource identifier (provider::resource-type)
@@ -227,17 +229,17 @@
     """
 
     name: str
     """
     This is a human readable logical name for the resource. This must be unique for the resource within the namespace and resource type
     (i.e. the concat value of <ruuid>:<name> must be unique)
 
-    This value is important for allow human level refactoring of resources. To update a resources name once created, you must edit only the 
-    name and not change the hash. If you change both the hash and name in the same deployment, it will register this as a delete and create 
-    instead of update. 
+    This value is important for allow human level refactoring of resources. To update a resources name once created, you must edit only the
+    name and not change the hash. If you change both the hash and name in the same deployment, it will register this as a delete and create
+    instead of update.
     """
 
     is_in_parent_resource_state: Optional[bool]
     """
     Boolean to determine if the reference should be resolved in the same resource state or from the parent resource state.
     """
 
@@ -292,15 +294,15 @@
 
 
 class Resource_Reference:
     RUUID: str = None
 
     def __init__(
         self, component_name: str, name: str, is_in_parent_resource_state: bool = False
-    ):
+    ) -> None:
         self.component_name = component_name
         self.name = name
         self.is_in_parent_resource_state = is_in_parent_resource_state
 
     def render(self) -> ResourceReferenceModel:
         raise NotImplementedError
 
@@ -311,42 +313,40 @@
                 self.RUUID,
                 self.name,
                 str(self.is_in_parent_resource_state),
             ]
         )
 
 
-
 ####################
 ##### Mixins
 ####################
 class PermissionsAvailableMixin:
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)  # forwards all unused arguments
-        self._available_permissions = None # Needs to be set later in the calling subclass
+        self._available_permissions = (
+            None  # Needs to be set later in the calling subclass
+        )
 
     @property
     def available_permissions(self):
         """The available permissions of the created resource"""
         return self._available_permissions
 
     @available_permissions.setter
-    def available_permissions(self, permissions: Any):
+    def available_permissions(self, permissions: Any) -> None:
         self._available_permissions = permissions
 
 
-
 class PermissionsGrantableMixin:
-
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)  # forwards all unused arguments
-        self._granted_permissions = [] # Needs to be set later in the calling subclass
-
+        self._granted_permissions = []  # Needs to be set later in the calling subclass
 
     @property
     def granted_permissions(self):
         return self._granted_permissions
 
     @granted_permissions.setter
     @update_hash
-    def granted_permissions(self, value: List):
+    def granted_permissions(self, value: List) -> None:
         self._granted_permissions = value
```

### Comparing `cdev-0.0.8/core/constructs/resource_state.py` & `cdev-0.0.9/core/constructs/resource_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     Unique identifier for this state
     """
 
     components: Optional[List[ComponentModel]]
     """
     The list of components owned by this namespace
     """
-    
+
     component_name_to_uuid: Optional[Dict[str, str]]
     """
     A dictionary from the uuid of a component to the component name
     """
 
     parent_uuid: Optional[str]
     """
@@ -52,32 +52,30 @@
     """
 
     failed_changes: Optional[Dict[str, Tuple[str, Resource_Difference, Dict]]]
     """
     A dictionary of transaction tokens to a tuple of (component_name, diff, error_info) for the changes that failed
     """
 
-
     def __init__(
         __pydantic_self__,
         name: str,
         uuid: str,
         components: List[ComponentModel] = [],
-        component_name_to_uuid: Dict[str, str]={},
+        component_name_to_uuid: Dict[str, str] = {},
         parent_uuid: Optional[str] = None,
         children: List[str] = [],
         resource_changes: Dict[str, Tuple[str, Resource_Difference]] = {},
         failed_changes: Dict[str, Tuple[str, Resource_Difference, Dict]] = {},
-        
     ) -> None:
         super().__init__(
             **{
                 "name": name,
                 "uuid": uuid,
                 "components": components,
                 "component_name_to_uuid": component_name_to_uuid,
                 "parent_uuid": parent_uuid,
                 "children": children,
                 "resource_changes": resource_changes,
-                "failed_changes": failed_changes
+                "failed_changes": failed_changes,
             }
         )
```

### Comparing `cdev-0.0.8/core/constructs/settings.py` & `cdev-0.0.9/core/constructs/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,101 +1,92 @@
 """
-Basic available settings 
+Basic available settings
 """
 import os
 
-from typing import Any, Optional
-from rich.logging import RichHandler
-
-from rich.traceback import install
-
-from typing import List, Set
+from typing import Optional, List
 
 from pydantic import (
     BaseModel,
     BaseSettings,
 )
 
 from core.utils.module_loader import import_class, import_module
 
 
 class Settings_Info(BaseModel):
     base_class: str
     user_setting_module: Optional[List[str]]
     secret_dir: Optional[str]
-    
+
 
 class Settings(BaseSettings):
 
     # Starting Path for workspace
     BASE_PATH: str = os.path.abspath(os.getcwd())
 
-
     INTERNAL_FOLDER_NAME: str = ".cdev"
 
     # Configuration file for a workspace
     WORKSPACE_FILE: str = "workspace_info.json"
 
-
     INTERMEDIATE_FOLDER_LOCATION: str = os.path.join(
         BASE_PATH, INTERNAL_FOLDER_NAME, "intermediate"
     )
 
+    # Cache Directory
+    CACHE_DIRECTORY: str = os.path.join(INTERMEDIATE_FOLDER_LOCATION, "cache")
+
     # Bucket to use as a place to store resource artifacts in the cloud
-    S3_ARTIFACTS_BUCKET: str = "cdev-demo-project-artifacts"
+    S3_ARTIFACTS_BUCKET: Optional[str] = None
 
     # AWS account information
     AWS_REGION: str = "us-east-1"
-    
+
     # Base entry point file for the workspace
-    ENTRY_POINT_FILE: str = os.path.join(
-        BASE_PATH, "cdev_project.py"
-    )
+    ENTRY_POINT_FILE: str = os.path.join(BASE_PATH, "cdev_project.py")
 
     DEPLOYMENT_PLATFORM: str = "x86"
 
     USE_DOCKER: bool = False
 
-
     class Config:
-        env_prefix = 'cdev_'
+        env_prefix = "cdev_"
         validate_assignment = True
-        #extra = 'allow'
-
+        # extra = 'allow'
 
 
 def initialize_settings(info: Settings_Info) -> Settings:
-    class_name = info.base_class.split('.')[-1]
-    module_name = ".".join(info.base_class.split('.')[:-1])
+    """Initialize the Settings object from a given Setting Info
+
+    Args:
+        info (Settings_Info)
+
+    Returns:
+        Settings
+    """
+    class_name = info.base_class.split(".")[-1]
+    module_name = ".".join(info.base_class.split(".")[:-1])
 
     base_settings_class = import_class(module_name, class_name)
 
     kw_args = {}
 
     if info.secret_dir:
-        kw_args['_secrets_dir'] = info.secret_dir
-
+        kw_args["_secrets_dir"] = info.secret_dir
 
     # All the settings are stored as relative paths so they need to convert to full paths
-    t = {k:os.path.join(os.getcwd(),v) for k,v in kw_args.items()}
-    
+    t = {k: os.path.join(os.getcwd(), v) for k, v in kw_args.items()}
+
     base_setting_obj = base_settings_class(**t)
 
     if info.user_setting_module:
         for settings_module in info.user_setting_module:
-            
-
             module = import_module(settings_module)
 
             for setting in dir(module):
                 if setting.isupper():
                     setting_value = getattr(module, setting)
 
                     setattr(base_setting_obj, setting, setting_value)
 
-       
-
     return base_setting_obj
-
-    
-
-
```

### Comparing `cdev-0.0.8/core/constructs/workspace.py` & `cdev-0.0.9/core/constructs/workspace.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,109 @@
-"""Construct that represents the collection of other primitives 
+"""Construct that represents the collection of other primitives
 
 
 """
 
 from enum import Enum
 import inspect
 from rich.console import Console
-from rich.progress import Progress, BarColumn, TextColumn, TimeElapsedColumn, SpinnerColumn
-from typing import Callable, List, Dict, Any, Tuple, TypeVar
+from rich.progress import (
+    Progress,
+    BarColumn,
+    TextColumn,
+    TimeElapsedColumn,
+    SpinnerColumn,
+)
+from typing import Callable, List, Dict, Any, Tuple, TypeVar, Optional
+
 
 from networkx.algorithms.dag import topological_sort
 from networkx.classes.digraph import DiGraph
 from networkx.classes.graph import NodeView
 
 from pydantic import BaseModel
 
 from core.constructs.models import frozendict
 from core.constructs.output_manager import OutputManager, OutputTask
 
-from core.constructs.resource import Resource_Change_Type, Resource_Difference, Resource_Reference_Difference, Resource_Reference_Change_Type, ResourceModel
-from core.constructs.backend import Backend
+from core.constructs.resource import (
+    Resource_Change_Type,
+    Resource_Difference,
+    Resource_Reference_Difference,
+    Resource_Reference_Change_Type,
+    ResourceModel,
+)
+from core.constructs.backend import Backend, Backend_Configuration, load_backend
 from core.constructs.mapper import CloudMapper
-from core.constructs.components import Component, Component_Change_Type, Component_Difference, ComponentModel
+from core.constructs.components import (
+    Component,
+    Component_Change_Type,
+    Component_Difference,
+    ComponentModel,
+)
 from core.constructs.commands import BaseCommand, BaseCommandContainer
-from core.constructs.cloud_output import Cloud_Output, evaluate_dynamic_output, cloud_output_dynamic_model
+from core.constructs.cloud_output import (
+    Cloud_Output,
+    evaluate_dynamic_output,
+    cloud_output_dynamic_model,
+)
 from core.constructs.settings import Settings_Info, Settings, initialize_settings
 
 
 from core.utils.command_finder import find_specified_command
 from core.utils import module_loader, topological_helper
 from core.utils.logger import log
 
 from core.constructs.types import F
 
 
 _GLOBAL_WORKSPACE: "Workspace" = None
 
 
-
-
 class Workspace_Info(BaseModel):
     python_module: str
     python_class: str
     settings_info: Settings_Info
-    config: Dict
+    backend_info: Backend_Configuration
+    resource_state_uuid: str
+    initialization_modules: Optional[List[str]]
+    config: Optional[Dict]
 
     def __init__(
-        __pydantic_self__, python_module: str, python_class: str, settings_info: Settings_Info, config: Dict
+        __pydantic_self__,
+        python_module: str,
+        python_class: str,
+        settings_info: Settings_Info,
+        backend_info: Backend_Configuration,
+        resource_state_uuid: str,
+        initialization_modules: Optional[List[str]] = [],
+        config: Optional[Dict] = {},
     ) -> None:
         """
         Represents the data needed to create a new cdev workspace:
 
-        Parameters:
-            python_module: The name of the python module to load as the workspace
-            python_class: The name of the class in the python module to initialize
-            settings_info: Settings_Info
-            config: configuration option for the workspace
+        Args:
+            python_module (str): The name of the python module to load as the workspace
+            python_class (str): The name of the class in the python module to initialize
+            settings_info (Settings_Info): Information to load settings of the `Workspace`
+            backend_info (Backend_Configuration): Configuration information for the `Backend`
+            resource_state_uuid (str): The `Backend` resource state uuid this `Workspace` will execute against
+            initialization_modules (Optional[List[str]]): List of Python modules to dynamically import to initialize `Workspace`
+            config (Optional[Dict]): configuration option for the workspace
 
         """
 
         super().__init__(
             **{
                 "python_module": python_module,
                 "python_class": python_class,
                 "settings_info": settings_info,
+                "backend_info": backend_info,
+                "resource_state_uuid": resource_state_uuid,
+                "initialization_modules": initialization_modules,
                 "config": config,
             }
         )
 
 
 class Workspace_State(str, Enum):
     UNINITIALIZED = "UNINITIALIZED"
@@ -75,191 +111,249 @@
     INITIALIZED = "INITIALIZED"
     EXECUTING_FRONTEND = "EXECUTING_FRONTEND"
     EXECUTING_BACKEND = "EXECUTING_BACKEND"
 
 
 def wrap_phase(phases: List[Workspace_State]) -> Callable[[F], F]:
     """
-    Annotation that denotes when a function can be executed within the life cycle of a workspace. Throws excpetion if the workspace is not in the correct
-    phase.
+    Annotation that denotes when a function can be executed within the life cycle of a workspace.
+    Throws exception if the workspace is not in the correct phase.
     """
 
     def inner_wrap(func: F) -> F:
         def wrapper_func(workspace: "Workspace", *func_posargs, **func_kwargs):
 
             current_state = workspace.get_state()
-            if not current_state in phases:
+            if current_state not in phases:
                 raise Exception(
                     f"Trying to call {func} while in workspace state {current_state} but need to be in {phases}"
                 )
 
-            else:
-                rv = func(workspace, *func_posargs, **func_kwargs)
-                return rv
+            rv = func(workspace, *func_posargs, **func_kwargs)
+            return rv
 
         return wrapper_func
 
     return inner_wrap
 
 
 class Workspace:
     """
     A singleton that encapsulates the configuration and high level information needed to construct the project. This singleton
     can be used within the different components to gain information about the higher level project that it is within. Once constructed,
     the object should remain a read only object to prevent components from changing configuration beyond their scope.
     """
-    _settings: Settings
+
+    _settings: Settings = None
+    _resource_state_uuid: str = None
 
     @classmethod
-    def instance(cls) -> 'Workspace':
+    def instance(cls) -> "Workspace":
+        """Get the Global instance variable to a given Workspace
+
+        Returns:
+            Workspace
+        """
         if not _GLOBAL_WORKSPACE:
             raise Exception("Currently No Global Workspace")
 
         return _GLOBAL_WORKSPACE
 
     @classmethod
-    def set_global_instance(cls, workspace: "Workspace"):
+    def set_global_instance(cls, workspace: "Workspace") -> None:
+        """Set the Global instance variable to a given Workspace
+
+        Args:
+            caller (Workspace)
+        """
         global _GLOBAL_WORKSPACE
         _GLOBAL_WORKSPACE = workspace
 
     @classmethod
-    def remove_global_instance(cls, caller: "Workspace"):
-        """
-        Method to reset the Global Workspace object. This should be the final cleanup step for a Cdev process.
+    def remove_global_instance(cls, caller: "Workspace") -> None:
+        """Method to reset the Global Workspace object. This should be the final cleanup step for a Cdev process.
+
+        Args:
+            caller (Workspace)
         """
         global _GLOBAL_WORKSPACE
 
         if not _GLOBAL_WORKSPACE:
             raise Exception("Global Workspace is not set")
 
         if not _GLOBAL_WORKSPACE == caller:
             raise Exception("Only the current Workspace object can remove itself")
 
         _GLOBAL_WORKSPACE = None
 
-    def initialize_workspace(self, workspace_configuration: Workspace_Info):
-        """
-        Run the configuration needed to initialize a workspace. This should generally only be called by the Core framework itself to ensure that the
+    def initialize_workspace(
+        self,
+        settings_info: Settings_Info,
+        backend_info: Backend_Configuration,
+        resource_state_uuid: str,
+        initialization_modules: Optional[List[str]] = [],
+        configuration: Dict = {},
+    ) -> None:
+        """Run the configuration needed to initialize a workspace. This should generally only be called by the Core framework itself to ensure that the
         life cycle of a workspace is correctly handled.
-        """
-        raise NotImplementedError
 
-    def destroy_workspace(self):
+        Args:
+            settings_info (Settings_Info): Information to load the `Workspace` settings
+            backend_info (Backend_Configuration): information to connect to the `Backend`
+            resource_state_uuid (str): resource state to execute commands over
+            configuration (Dict): additional configuration
+        """
+        try:
+            initialized_backend = load_backend(backend_info)
+            self.set_backend(initialized_backend)
+        except Exception as e:
+            print(f"Could not load the load backend")
+            raise e
+
+        try:
+            top_level_resource_states = (
+                initialized_backend.get_top_level_resource_states()
+            )
+        except Exception as e:
+            raise e
+
+        if resource_state_uuid not in set([x.uuid for x in top_level_resource_states]):
+            raise Exception(
+                f"{resource_state_uuid} not in loaded backend resource states: ({top_level_resource_states})"
+            )
+
+        self.set_resource_state_uuid(resource_state_uuid)
+
+        try:
+            initialized_settings = initialize_settings(settings_info)
+            self.settings = initialized_settings
+        except Exception as e:
+            print(f"Could not load the load backend")
+            raise e
+
+        if initialization_modules:
+            for initialize_module in initialization_modules:
+                try:
+                    module_loader.import_module(initialize_module)
+                except Exception as e:
+                    raise e
+
+    def destroy_workspace(self) -> None:
+        """Tear down the current Workspace
+
+        Raises:
+            NotImplementedError
+        """
         raise NotImplementedError
 
     ############################
     ##### Settings
     ############################
 
-    
     @property
-    def settings(cls) -> Settings:
-        return Workspace._settings
+    def settings(self) -> Settings:
+        """Get settings object
 
-    
-    @settings.setter
-    def settings(cls, value: Settings):
-        Workspace._settings = value
+        Returns:
+            Settings
+        """
+        return self._settings
 
+    @settings.setter
+    def settings(self, value: Settings) -> None:
+        """Set settings object"""
+        self._settings = value
 
     ############################
     ##### Initialized
     ############################
     def get_state(self) -> Workspace_State:
-        """
-        Get the current lifecycle state of the Workspace.
+        """Get the current lifecycle state of the Workspace.
 
         Returns:
             state (Workspace_State)
         """
         raise NotImplementedError
 
-    def set_state(self, value: Workspace_State):
-        """
-        Set the current lifecycle state of the Workspace.
+    def set_state(self, value: Workspace_State) -> None:
+        """Set the current lifecycle state of the Workspace.
 
-        Arguments:
+        Args:
             value (Workspace_State)
         """
         raise NotImplementedError
 
     #################
     ##### Mappers
     #################
     def add_mapper(self, mapper: CloudMapper) -> None:
-        """
-        Add a CloudMapper to the project. The order that the Mappers are added to the Workspace defines the precedence give when
+        """Add a CloudMapper to the project. The order that the Mappers are added to the Workspace defines the precedence give when
         determining which CloudMapper to use.
 
         Note that this function should only be called during the `Workspace Initialization` part of the Cdev lifecycle.
 
-        Arguments:
+        Args:
             mapper (CloudMapper): The mapper to add
         """
         raise NotImplementedError
 
     def add_mappers(self, mappers: List[CloudMapper]) -> None:
-        """
-        Add a List of CloudMappers to the project. The order that the Mappers are added to the Workspace defines the precedence
+        """Add a List of CloudMappers to the project. The order that the Mappers are added to the Workspace defines the precedence
         give when determining which CloudMapper to use.
 
         Note that this function should only be called during the `Workspace Initialization` part of the Cdev lifecycle.
 
-        Arguments:
+        Args:
             mappers (List[CloudMapper]): The mapper to add
         """
         raise NotImplementedError
 
     def get_mappers(self) -> List[CloudMapper]:
-        """
-        Return the List of CloudMappers for this Workspace.
+        """Return the List of CloudMappers for this Workspace.
 
         Note that this function should only be called during the `Workspace Initialized` part of the Cdev lifecycle.
 
         Returns:
             mappers (List[CloudMapper]): mappers for this Workspace
         """
         raise NotImplementedError
 
     def get_mapper_namespace(self) -> Dict[str, CloudMapper]:
-        """
-        Return the Dictionary that maps Resource ID's (ruuid) to the mapper that will be used to deploy the resource into the cloud.
+        """Return the Dictionary that maps Resource ID's (ruuid) to the mapper that will be used to deploy the resource into the cloud.
 
         Note that this function should only be called during the `Workspace Initialized` part of the Cdev lifecycle.
 
         Returns:
             ruuid_to_mapper (Dict[str, CloudMapper]): Resource ID to CloudMapper
         """
         raise NotImplementedError
 
     #################
     ##### Commands
     #################
-    def add_command(self, command_location: str):
-        """
-        Add a Command Location to the Workspace. The order that the Command is added to the Workspace defines the precedence
+    def add_command(self, command_location: str) -> None:
+        """Add a Command Location to the Workspace. The order that the Command is added to the Workspace defines the precedence
         give when searching for Commands. Command Locations should adhere to the defined form to ensure that they can be
         found within the Workspace.
 
         Note that this function should only be called during the `Workspace Initialization` part of the Cdev lifecycle.
 
-        Arguments:
+        Args:
             command_location (Command): The command location to add
         """
         raise NotImplementedError
 
-    def add_commands(self, command_locations: List[str]):
-        """
-        Add a List of Command Locations to the Workspace. The order that the Commands are added to the Workspace defines the precedence
+    def add_commands(self, command_locations: List[str]) -> None:
+        """Add a List of Command Locations to the Workspace. The order that the Commands are added to the Workspace defines the precedence
         give when searching for a Command. Command Locations should adhere to the defined form to ensure that they can be
         found within the Workspace.
 
         Note that this function should only be called during the `Workspace Initialization` part of the Cdev lifecycle.
 
-        Arguments:
+        Args:
             command_locations (Command): The command location to add
         """
         raise NotImplementedError
 
     def get_commands(self) -> List[str]:
         """Get the Command Locations for this Workspace.
 
@@ -270,123 +364,111 @@
         """
         raise NotImplementedError
 
     #######################
     ##### Display Output
     #######################
 
-    def display_output(self, tag: str, output: Cloud_Output):
+    def display_output(self, tag: str, output: Cloud_Output) -> None:
         """Display the output from a Resource or Reference after a process has completed
 
         Args:
             tag: A key value to display with the output
             output: The Cloud Output to render
         """
         raise NotImplementedError
 
-
     def render_outputs(self) -> List[Tuple[str, Any]]:
         """Render the output associated with the Workspace
 
         Returns:
             List[Tuple[str, Any]]: The List of outputs with their associated tag
-        
         """
         raise NotImplementedError
 
+    def clear_output(self) -> None:
+        raise NotImplementedError
 
     #######################
     ##### Components
     #######################
-    def add_component(self, component: Component):
-        """
-        Add a Component to the Workspace. Components are used to determine the desired state of the Workspace. They should represent
+    def add_component(self, component: Component) -> None:
+        """Add a Component to the Workspace. Components are used to determine the desired state of the Workspace. They should represent
         a logical separation for the Resources in a project.
 
         Note that this function should only be called during the `Workspace Initialization` part of the Cdev lifecycle.
 
         Arguments:
             component (Component): Component to add
         """
         raise NotImplementedError
 
-    def add_components(self, components: List[Component]):
-        """
-        Add a List of Components to the Workspace. Components are used to determine the desired state of the Workspace. They
+    def add_components(self, components: List[Component]) -> None:
+        """Add a List of Components to the Workspace. Components are used to determine the desired state of the Workspace. They
         should represent a logical separation for the Resources in a project.
 
         Note that this function should only be called during the `Workspace Initialization` part of the Cdev lifecycle.
 
         Arguments:
             component (Component): Component to add
         """
         raise NotImplementedError
 
     def get_components(self) -> List[Component]:
-        """
-        Return the Components for this Workspace.
+        """Return the Components for this Workspace.
 
         Note that this function should only be called during the `Workspace Initialized` or `Executing Frontend` part of the Cdev lifecycle.
 
         Returns:
             components (List[Component])
         """
         raise NotImplementedError
 
     ################
     ##### Backend
     ################
     def get_backend(self) -> Backend:
-        """
-        Return the Backend that is associated with this Workspace.
+        """Return the Backend that is associated with this Workspace.
 
         Note that this function should only be called during the `Workspace Initialized` part of the Cdev lifecycle.
 
         Returns:
             backend (Backend): Initialized Backend for the Workspace
         """
         raise NotImplementedError
 
-    def set_backend(self, backend: Backend):
-        """
-        Set the Backend for the Workspace.
+    def set_backend(self, backend: Backend) -> None:
+        """Set the Backend for the Workspace.
 
         Note that this function should only be called during the `Workspace Initialization` part of the Cdev lifecycle.
 
         Arguments:
             backend (Backend):  Initialized Backend for the Workspace
         """
         raise NotImplementedError
 
-    def set_resource_state_uuid(self, resource_state_uuid: str):
-        """
-        Set the Resource State UUID to denote the Resource State that this Workspace will execute over.
-
+    def set_resource_state_uuid(self, resource_state_uuid: str) -> None:
+        """Set the Resource State UUID to denote the Resource State that this Workspace will execute over.
         Note that this function should only be called during the `Workspace Initialization` part of the Cdev lifecycle.
-
         Arguments:
             resource_state_uuid (str): Resource State UUID from the Backend
         """
         raise NotImplementedError
 
     def get_resource_state_uuid(self) -> str:
-        """
-        Get the Resource State UUID that this Workspace is executing over.
-
+        """Get the Resource State UUID that this Workspace is executing over.
         Note that this function should only be called during the `Workspace Initialized` part of the Cdev lifecycle.
-
         Returns:
             resource_state_uuid (str): Resource State UUID from the Backend
         """
         raise NotImplementedError
 
     @wrap_phase([Workspace_State.EXECUTING_FRONTEND])
     def generate_current_state(self) -> List[ComponentModel]:
-        """
-        Execute the components of this workspace to generate the current desired state of the resources.
+        """Execute the components of this workspace to generate the current desired state of the resources.
 
         Returns:
             Current State (List[ComponentModel]): The current state generated by the components.
         """
 
         rv = []
         components: List[Component] = self.get_components()
@@ -394,316 +476,435 @@
         for component in components:
             rv.append(component.render())
 
         return rv
 
     @wrap_phase([Workspace_State.EXECUTING_FRONTEND])
     def create_state_differences(
-        self, desired_state: List[ComponentModel], previous_state_component_names: List[str]
+        self,
+        desired_state: List[ComponentModel],
+        previous_state_component_names: List[str],
     ) -> Tuple[
-        Component_Difference, Resource_Difference, Resource_Reference_Difference,
+        Component_Difference,
+        Resource_Difference,
+        Resource_Reference_Difference,
     ]:
-        """
-        Produce the differences between the desired state of the components and the current saved state
+        """Produce the differences between the desired state of the components and the current saved state
 
-        Arguments:
+        Args:
             desired_state (List[ComponentModel]): The current state generated by the components.
             previous_state_component_names (List[str]): The names of the components to diff against.
 
         Returns:
             component_differences (List[Component_Difference]): The list of differences at the component level.
             reference_differences (List[Resource_Reference_Difference]): The list of differences for references within components.
             resource_differences (List[Resource_Difference]): The list of the difference for the resources within components.
-
         """
 
         backend = self.get_backend()
         resource_state_uuid = self.get_resource_state_uuid()
 
         return backend.create_differences(
             resource_state_uuid, desired_state, previous_state_component_names
         )
 
     @wrap_phase([Workspace_State.EXECUTING_FRONTEND])
-    def sort_differences(self, differences: Tuple[List[Component_Difference], List[Resource_Reference_Difference], List[Resource_Difference]]) -> DiGraph:
-        return topological_helper.generate_sorted_resources(differences)
+    def sort_differences(
+        self,
+        differences: Tuple[
+            List[Component_Difference],
+            List[Resource_Reference_Difference],
+            List[Resource_Difference],
+        ],
+    ) -> DiGraph:
+        """Given the sets of differences, sort them into a topological deployment order based on dependencies between resource outputs
+
+        Args:
+            differences (Tuple[ List[Component_Difference], List[Resource_Reference_Difference], List[Resource_Difference], ])
 
+        Returns:
+            DiGraph
+        """
+        return topological_helper.generate_sorted_resources(differences)
 
     @wrap_phase([Workspace_State.EXECUTING_BACKEND])
     def deploy_differences(self, differences_dag: DiGraph) -> None:
+        """Given the sets of differences, sort them into a topological deployment order based on dependencies between resource outputs
+
+        Args:
+            differences (Tuple[ List[Component_Difference], List[Resource_Reference_Difference], List[Resource_Difference], ])
 
+        Returns:
+            DiGraph
+        """
         console = Console()
         with Progress(
-                SpinnerColumn(),
-                "[progress.description]{task.description}",
-                BarColumn(finished_style='white'),
-                TimeElapsedColumn(),
-                TextColumn("{task.fields[comment]}"),
-                console=console
-            ) as progress:
+            SpinnerColumn(),
+            "[progress.description]{task.description}",
+            BarColumn(finished_style="white"),
+            TimeElapsedColumn(),
+            TextColumn("{task.fields[comment]}"),
+            console=console,
+        ) as progress:
             output_manager = OutputManager(console, progress)
 
-            all_nodes_sorted: List[NodeView] = [x for x in topological_sort(differences_dag)]
+            all_nodes_sorted: List[NodeView] = [
+                x for x in topological_sort(differences_dag)
+            ]
 
             # There seems to be some bug in Rich that causes a deadlock when creating a bunch of Tasks in a row.
             # The problem seems to be around it refreshing after creating each task, so to avoid this problem,
-            # we are disabling the console while the task are created. Then turn the console back on when they 
+            # we are disabling the console while the task are created. Then turn the console back on when they
             # are created.
             # TODO: Recreate problem in isolated environment, and submit bug report.
             output_manager._progress.disable = True
 
-            node_to_task= {x: output_manager.create_task(output_manager.create_output_description(x), start=False, total=10, comment='Waiting') for x in all_nodes_sorted}
+            node_to_task = {
+                x: output_manager.create_task(
+                    output_manager.create_output_description(x),
+                    start=False,
+                    total=10,
+                    comment="Waiting",
+                )
+                for x in all_nodes_sorted
+            }
 
             # Re-enable to console to update
             output_manager._progress.disable = False
 
-            topological_helper.topological_iteration(differences_dag, self.wrap_output_deploy_change(node_to_task), failed_parent_handler=self.wrap_output_failed_child(node_to_task))
-            
-
+            topological_helper.topological_iteration(
+                differences_dag,
+                self.wrap_output_deploy_change(node_to_task),
+                failed_parent_handler=self.wrap_output_failed_child(node_to_task),
+            )
 
     @wrap_phase([Workspace_State.EXECUTING_BACKEND])
     def wrap_output_failed_child(self, tasks: Dict[NodeView, OutputTask]):
+        """Wrapped function that fails any resource that has a failed parent
+
+        Args:
+            tasks (Dict[NodeView, OutputTask])
+        """
+
         def mark_failure_by_parent(change: NodeView) -> None:
             output_task = tasks.get(change)
-            output_task.update(advance=10, comment="Failed because parent resource failed to deploy :cross_mark:")
+            output_task.update(
+                advance=10,
+                comment="Failed because parent resource failed to deploy :cross_mark:",
+            )
 
         return mark_failure_by_parent
 
-
     @wrap_phase([Workspace_State.EXECUTING_BACKEND])
     def wrap_output_deploy_change(self, tasks: Dict[NodeView, OutputTask]):
+        """Wrapped function callers mapper and updates backend
+
+        Args:
+            tasks (Dict[NodeView, OutputTask])
+        """
 
         def deploy_change(change: NodeView) -> None:
             output_task = tasks.get(change)
             output_task.start_task()
 
             if isinstance(change, Resource_Difference):
                 # Step 1 is to register a transaction with the backend
 
                 try:
-                    transaction_token, namespace_token = self.get_backend().create_resource_change_transaction(self.get_resource_state_uuid(), change.component_name, change)
+                    (
+                        transaction_token,
+                        namespace_token,
+                    ) = self.get_backend().create_resource_change_transaction(
+                        self.get_resource_state_uuid(), change.component_name, change
+                    )
                 except Exception as e:
                     print(e)
                     print(f"Error Creating Transaction: {change}")
                     raise e
-                
 
-                ruuid = change.new_resource.ruuid if change.new_resource else change.previous_resource.ruuid
+                ruuid = (
+                    change.new_resource.ruuid
+                    if change.new_resource
+                    else change.previous_resource.ruuid
+                )
 
                 # The Previous output is used by the mappers to make changes to the underlying resources.
                 previous_output = (
-                    self.get_backend().get_cloud_output_by_name(self.get_resource_state_uuid(), change.component_name, ruuid, change.previous_resource.name)
-                    if not change.action_type == Resource_Change_Type.CREATE else
-                    {}
+                    self.get_backend().get_cloud_output_by_name(
+                        self.get_resource_state_uuid(),
+                        change.component_name,
+                        ruuid,
+                        change.previous_resource.name,
+                    )
+                    if not change.action_type == Resource_Change_Type.CREATE
+                    else {}
                 )
 
                 try:
                     # Substitute the model with a model that has the cloud outputs evaluated.
-                    new_evaluated_resource, evaluated_keys = self.evaluate_and_replace_cloud_output(change.component_name, change.new_resource)
-                    previous_evaluated_resource = self.evaluate_and_replace_previous_cloud_output(change.component_name, change.previous_resource)
+                    (
+                        new_evaluated_resource,
+                        evaluated_keys,
+                    ) = self.evaluate_and_replace_cloud_output(
+                        change.component_name, change.new_resource
+                    )
+                    previous_evaluated_resource = (
+                        self.evaluate_and_replace_previous_cloud_output(
+                            change.component_name, change.previous_resource
+                        )
+                    )
 
-                    
                     # If there was no cloud output in the resource, then the evaluated resources will equal the original resources
-                    # so using that value is safe. 
+                    # so using that value is safe.
                     _evaluated_change = Resource_Difference(
                         change.action_type,
                         change.component_name,
                         previous_evaluated_resource,
                         new_evaluated_resource,
                     )
 
-                    
                 except Exception as e:
                     print(e)
                     print(f"Error evaluating cloud output from change: {change}")
                     raise e
 
                 try:
                     log.debug("evaluated information %s", _evaluated_change)
                     output_task.update(advance=5, comment="Deploying on Cloud :cloud:")
                     mapper = self.get_mapper_namespace().get(ruuid)
-                    cloud_output = mapper.deploy_resource(transaction_token, namespace_token, _evaluated_change, previous_output, output_task)
-                    output_task.update(advance=3, comment="Completing transaction with Backend")
+                    cloud_output = mapper.deploy_resource(
+                        transaction_token,
+                        namespace_token,
+                        _evaluated_change,
+                        previous_output,
+                        output_task,
+                    )
+                    output_task.update(
+                        advance=3, comment="Completing transaction with Backend"
+                    )
 
                 except Exception as e:
-                    self.get_backend().fail_resource_change(self.get_resource_state_uuid(), change.component_name, change, transaction_token, {"message": "deployment error"})
-                    output_task.update(advance=10, comment="Failed because mapper raised error :cross_mark:")
+                    self.get_backend().fail_resource_change(
+                        self.get_resource_state_uuid(),
+                        change.component_name,
+                        change,
+                        transaction_token,
+                        {"message": "deployment error"},
+                    )
+                    output_task.update(
+                        advance=10,
+                        comment="Failed because mapper raised error :cross_mark:",
+                    )
                     print(e)
                     raise e
 
                 try:
                     if change.action_type == Resource_Change_Type.CREATE:
-                        cloud_output['cloud_region'] = Workspace.instance().settings.AWS_REGION
-
+                        cloud_output[
+                            "cloud_region"
+                        ] = Workspace.instance().settings.AWS_REGION
 
                     self.get_backend().complete_resource_change(
                         self.get_resource_state_uuid(),
                         change.component_name,
                         change,
                         transaction_token,
                         cloud_output,
-                        evaluated_keys
+                        evaluated_keys,
                     )
 
                 except Exception as e:
-                    self.get_backend().fail_resource_change(self.get_resource_state_uuid(), change.component_name, change, transaction_token, {"message": "backend error"})
-                    output_task.update(advance=10, comment="Failed because backend raised error :cross_mark:")
+                    self.get_backend().fail_resource_change(
+                        self.get_resource_state_uuid(),
+                        change.component_name,
+                        change,
+                        transaction_token,
+                        {"message": "backend error"},
+                    )
+                    output_task.update(
+                        advance=10,
+                        comment="Failed because backend raised error :cross_mark:",
+                    )
                     print(e)
                     raise e
 
             elif isinstance(change, Resource_Reference_Difference):
-                output_task.update(advance=5, comment=f'{"Creating" if change.action_type == Resource_Reference_Change_Type.CREATE else "Removing"} Reference')
-                self.get_backend().resolve_reference_change(self.get_resource_state_uuid(), change)
-
+                output_task.update(
+                    advance=5,
+                    comment=f'{"Creating" if change.action_type == Resource_Reference_Change_Type.CREATE else "Removing"} Reference',
+                )
+                self.get_backend().resolve_reference_change(
+                    self.get_resource_state_uuid(), change
+                )
 
             elif isinstance(change, Component_Difference):
-                output_task.update(advance=5, comment='Updating Component in Backend')
-                self.get_backend().update_component(self.get_resource_state_uuid(), change)
-
+                output_task.update(advance=5, comment="Updating Component in Backend")
+                self.get_backend().update_component(
+                    self.get_resource_state_uuid(), change
+                )
 
             else:
-                raise Exception(f"Trying to deploy node {change} but it is not a correct type ")
-
-
-            output_task.update(completed=10, comment='Completed :white_check_mark:')
+                raise Exception(
+                    f"Trying to deploy node {change} but it is not a correct type "
+                )
 
+            output_task.update(completed=10, comment="Completed :white_check_mark:")
 
         return deploy_change
 
     @wrap_phase([Workspace_State.EXECUTING_BACKEND])
-    def evaluate_and_replace_cloud_output(self, component_name: str, original_resource: ResourceModel) -> Tuple[ResourceModel, Dict]:
-        """[stuff]
+    def evaluate_and_replace_cloud_output(
+        self, component_name: str, original_resource: ResourceModel
+    ) -> Tuple[ResourceModel, Dict]:
+        """Replace the Cloud Output object in the given resource
 
         Args:
-            component_name (str): [description]
-            original_resource (ResourceModel): [description]
+            component_name (str)
+            original_resource (ResourceModel)
 
         Returns:
-            Tuple[ResourceModel, Dict]: [description]
+            Tuple[ResourceModel, Dict]
         """
         if not original_resource:
             return original_resource, None
-        
+
         original_resource_dict = frozendict(original_resource.dict())
-        
+
         def _resolver(ruuid, name, key) -> Any:
             return self.get_backend().get_cloud_output_value_by_name(
-                self.get_resource_state_uuid(),
-                component_name,
-                ruuid,
-                name,
-                key
+                self.get_resource_state_uuid(), component_name, ruuid, name, key
             )
-            
-        updated_resource, resolved_value = self._recursive_replace_output(_resolver, original_resource_dict, {})
-        
+
+        updated_resource, resolved_value = self._recursive_replace_output(
+            _resolver, original_resource_dict, {}
+        )
+
         evaluated_resource = original_resource.__class__(**updated_resource)
 
         return evaluated_resource, resolved_value
 
-
     @wrap_phase([Workspace_State.EXECUTING_BACKEND])
-    def evaluate_and_replace_previous_cloud_output(self, component_name: str, previous_resource: ResourceModel) -> ResourceModel:
-        """[stuff]
+    def evaluate_and_replace_previous_cloud_output(
+        self, component_name: str, previous_resource: ResourceModel
+    ) -> ResourceModel:
+        """Replace the Cloud Output object in the given resource based on the previous cloud output values
 
         Args:
-            component_name (str): [description]
-            original_resource (ResourceModel): [description]
+            component_name (str)
+            original_resource (ResourceModel)
 
         Returns:
-            Tuple[ResourceModel, Dict]: [description]
+            Tuple[ResourceModel, Dict]
         """
-        
+
         if not previous_resource:
             return previous_resource
-        
+
         original_resource_dict = frozendict(previous_resource.dict())
-        
 
         def wrap_resolver() -> Callable:
-            previous_resolved_values = self.get_backend().get_component(self.get_resource_state_uuid(), component_name).previous_resolved_cloud_values
+            previous_resolved_values = (
+                self.get_backend()
+                .get_component(self.get_resource_state_uuid(), component_name)
+                .previous_resolved_cloud_values
+            )
 
             if not previous_resolved_values:
                 raise Exception
 
-            previous_resource_resolved_values = previous_resolved_values.get(f'{previous_resource.ruuid};{previous_resource.name}')
+            previous_resource_resolved_values = previous_resolved_values.get(
+                f"{previous_resource.ruuid};{previous_resource.name}"
+            )
 
             def _resolver(ruuid, name, key) -> Any:
 
                 if not previous_resource_resolved_values:
                     raise Exception
 
-                key  = f"{ruuid};{name};{key}"
+                key = f"{ruuid};{name};{key}"
 
                 if not key in previous_resource_resolved_values:
                     raise Exception
 
                 return previous_resource_resolved_values.get(key)
 
             return _resolver
-            
-            
-        updated_resource, _ = self._recursive_replace_output(wrap_resolver(), original_resource_dict, {})
-        
+
+        updated_resource, _ = self._recursive_replace_output(
+            wrap_resolver(), original_resource_dict, {}
+        )
+
         evaluated_resource = previous_resource.__class__(**updated_resource)
 
         return evaluated_resource
 
+    def _recursive_replace_output(
+        self, resolver: Callable, original: Any, resolved_values: Dict = {}
+    ) -> Tuple[Any, Dict]:
+        """Recursively replace any output
 
-    def _recursive_replace_output(self, resolver: Callable, original: Any, resolved_values: Dict = {}) -> Tuple[Any, Dict]:
+        Args:
+            resolver (Callable)
+            original (Any)
+            resolved_values (Dict, optional): Defaults to {}.
+
+        Returns:
+            Tuple[Any, Dict]
+        """
         # This function works over ImmutableModel that were converted using the `.dict` method. Therefore,
         # the collections will be `frozendict` and `frozenset` instead of `dict` and `list`
-        
+
         if isinstance(original, frozendict):
-            if "id" in original and original.get("id") == 'cdev_cloud_output':
-                
+            if "id" in original and original.get("id") == "cdev_cloud_output":
+
                 _value = resolver(
-                    original.get('ruuid'),
-                    original.get('name'),
-                    original.get('key')
+                    original.get("ruuid"), original.get("name"), original.get("key")
                 )
-                
+
                 values_key = f"{original.get('ruuid')};{original.get('name')};{original.get('key')}"
                 resolved_values[values_key] = _value
 
-                if original.get('output_operations'):
-                    return (evaluate_dynamic_output(_value, cloud_output_dynamic_model(**original)), resolved_values)
+                if original.get("output_operations"):
+                    return (
+                        evaluate_dynamic_output(
+                            _value, cloud_output_dynamic_model(**original)
+                        ),
+                        resolved_values,
+                    )
 
                 return (_value, resolved_values)
 
             rv = {}
-            for k,v in original.items():
-                new_v, tmp_resolved_values = self._recursive_replace_output(resolver, v, resolved_values)
-                
+            for k, v in original.items():
+                new_v, tmp_resolved_values = self._recursive_replace_output(
+                    resolver, v, resolved_values
+                )
+
                 rv[k] = new_v
 
                 resolved_values.update(tmp_resolved_values)
 
-
             return (frozendict(rv), resolved_values)
 
-        elif isinstance(original, frozenset): 
+        elif isinstance(original, frozenset):
             rv = []
             for x in original:
                 new_v, tmp_resolved_values = self._recursive_replace_output(resolver, x)
-                
+
                 rv.append(new_v)
 
                 resolved_values.update(tmp_resolved_values)
 
             return frozenset(rv), resolved_values
 
-        
         return original, resolved_values
 
-
     @wrap_phase([Workspace_State.INITIALIZED])
-    def execute_command(self, command: str, args: List):
-        """
-        Find the desired command based on the search path and execute it with the given arguments.
+    def execute_command(self, command: str, args: List) -> None:
+        """Find the desired command based on the search path and execute it with the given arguments.
 
         Args:
             command (str): The full command to search for. can be '.' seperated to denote search path.
             args (List): The command lines arguments to pass to the command.
 
         Raises:
             KeyError: Raises an exception.
@@ -711,15 +912,14 @@
 
         # Command in list form
         command_list = command.split(".")
 
         # Create list of all directories to start searching in
         all_search_locations_list = self.get_commands()
 
-
         obj, program_name, command_name, is_command = find_specified_command(
             command_list, all_search_locations_list
         )
 
         if is_command:
             if not isinstance(obj, BaseCommand):
                 raise Exception
@@ -737,49 +937,84 @@
             try:
                 obj.display_help_message()
             except Exception as e:
                 raise e
 
 
 class WorkspaceManager:
-    def create_new_workspace(self, workspace_info: Workspace_Info, *posargs, **kwargs):
-        """
-        Create a new workspace based on the information provided.
+    def create_new_workspace(
+        self, workspace_info: Workspace_Info, *posargs, **kwargs
+    ) -> None:
+        """Create a new workspace based on the information provided.
 
         Args:
             workspace_info (Workspace_Info): information about the backend configuration
 
         Raises:
             WorkSpaceAlreadyCreated
         """
         raise NotImplementedError
 
     def check_if_workspace_exists(self, *posargs, **kwargs) -> bool:
+        """Check if a workspace exists
+
+        Raises:
+            NotImplementedError
+
+        Returns:
+            bool
+        """
         raise NotImplementedError
 
     def load_workspace_configuration(self, *posargs, **kwargs) -> Workspace_Info:
+        """Load the configuration of the workspace
+
+        Raises:
+            NotImplementedError
+
+        Returns:
+            Workspace_Info
+        """
         raise NotImplementedError
 
     def load_workspace(self, *posargs, **kwargs) -> Workspace:
+        """Load a workspace
+
+        Raises:
+            NotImplementedError
+
+        Returns:
+            Workspace
+        """
         raise NotImplementedError
 
 
-def load_and_initialize_workspace(config: Workspace_Info):
-    """
-    Load and initialize the workspace from the given configuration
+def load_and_initialize_workspace(config: Workspace_Info) -> None:
+    """Load and initialize the workspace from the given configuration
+
+    Args:
+        config (Workspace_Info)
     """
     ws = load_workspace(config)
     ws.set_state(Workspace_State.INITIALIZING)
     initialize_workspace(ws, config.settings_info, config.config)
     ws.set_state(Workspace_State.INITIALIZED)
 
 
 def load_workspace(config: Workspace_Info) -> Workspace:
-    """
-    Load and initialize the workspace from the given configuration
+    """Load the workspace from the given configuration
+
+    Args:
+        config (Workspace_Info)
+
+    Raises:
+        Exception
+
+    Returns:
+        Workspace
     """
     try:
         workspace_module = module_loader.import_module(config.python_module)
     except Exception as e:
         print("Error loading workspace module")
         print(f"Error > {e}")
 
@@ -797,34 +1032,43 @@
             break
 
     if not workspace_class:
         print(f"Could not find {config.python_class} in {config.python_module}")
         raise Exception
 
     try:
-        # initialize the backend obj with the provided configuration values
         return workspace_class()
 
     except Exception as e:
         print(
             f"Could not load {workspace_class} Class from config {config.config}; {e}"
         )
         raise e
 
 
-def initialize_workspace(workspace: Workspace, settings: Settings_Info , config: Dict):
+def initialize_workspace(workspace: Workspace, workspace_info: Workspace_Info) -> None:
+    """Initialize the given workspace
+
+    Args:
+        workspace (Workspace): _description_
+        workspace_info (Workspace_Info): _description_
+
+    Raises:
+        e: _description_
+    """
     try:
-        Workspace.settings = initialize_settings(settings)
-        
+        workspace.set_state(Workspace_State.INITIALIZING)
         # initialize the backend obj with the provided configuration values
-        workspace.initialize_workspace(config)
-        
+        workspace.initialize_workspace(
+            settings_info=workspace_info.settings_info,
+            backend_info=workspace_info.backend_info,
+            resource_state_uuid=workspace_info.resource_state_uuid,
+            initialization_modules=workspace_info.initialization_modules,
+            configuration=workspace_info.config,
+        )
+        workspace.set_state(Workspace_State.INITIALIZED)
 
     except Exception as e:
         print(
-            f"Could not initialize {workspace} Class from config {config}; {e}"
+            f"Could not initialize {workspace} Class from config {workspace_info}; {e}"
         )
         raise e
-
-
-
-
```

### Comparing `cdev-0.0.8/core/default/backend.py` & `cdev-0.0.9/core/default/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 import json
 import os
 
-from pathlib import PosixPath, WindowsPath
 from pydantic.main import BaseModel
 from pydantic.types import DirectoryPath, FilePath
 
 from typing import Dict, List, Any, Tuple
 import uuid
 
-from core.constructs.workspace import Workspace
 
+from core.constructs.backend import Backend_Configuration, Backend
+from core.constructs.backend_exceptions import *
 
-from ..constructs.backend import Backend_Configuration, Backend
-from ..constructs.backend_exceptions import *
-
-from ..constructs.components import (
+from core.constructs.components import (
     Component_Change_Type,
     ComponentModel,
     Component_Difference,
 )
-from ..constructs.resource import (
+from core.constructs.resource import (
     Resource_Change_Type,
     Resource_Difference,
     Resource_Reference_Change_Type,
     ResourceModel,
     Resource_Reference_Difference,
     ResourceReferenceModel,
 )
-from ..constructs.resource_state import Resource_State
+from core.constructs.resource_state import Resource_State
 from ..utils import file_manager, hasher as cdev_hasher
 
 
 class LocalBackendError(BackendError):
     pass
 
 
@@ -39,28 +36,26 @@
     pass
 
 
 class InvalidResourceStateData(LocalBackendError):
     pass
 
 
-
 class SetEncoder(json.JSONEncoder):
     def default(self, obj):
-       if isinstance(obj, set):
-          return list(obj)
-       return json.JSONEncoder.default(self, obj)
+        if isinstance(obj, set):
+            return list(obj)
+        return json.JSONEncoder.default(self, obj)
 
 
 class Local_Backend_Configuration(Backend_Configuration):
     def __init__(self, config: Dict) -> None:
-        """
-        Represents the data needed to create a new cdev workspace:
+        """Represents the data needed to create a new cdev workspace:
 
-        Parameters:
+        Args:
             python_module: The name of the python module to load as the backend
             config: configuration option for the backend
 
         """
 
         super().__init__(
             **{
@@ -93,30 +88,24 @@
 
 class LocalBackend(Backend):
     # Structurally, this implementation will have a central json that can be used as an index into more precise json files. For example, each resource state will be its own json file, but
     # the central file will keep track of each one.
     def __init__(
         self, base_folder: DirectoryPath, central_state_file: FilePath = None
     ) -> None:
-        """
-        Implementation of a Backend using locally stored json files as the peristent storage medium. This backend should only be used for small project as it does not provide any mechanisms
+        """Implementation of a Backend using locally stored json files as the persistent storage medium. This backend should only be used for small project as it does not provide any mechanisms
         to work well when multiple people edit the state. Also this is a single threaded implementation.
 
-        *** For now, we will not use any kind of WAL for make changes to underlying state files, so it can be bad if you kill the process unexpectedly. In the future, it will use some mechanism
-        to prevent this. ***
-
-        Arguments:
+        Args:
             base_folder (DirectoryPath): Path to a folder to use for storing local json files. Defaults to cdev setting if not provided.
             central_state_file (FilePath): Path to the central state file. Defaults to cdev setting if not provided.
         """
 
-        
         DEFAULT_CENTRAL_STATE_FILE = os.path.join(base_folder, "local_state.json")
 
-
         self.base_folder = base_folder
         self.central_state_file = (
             central_state_file if central_state_file else DEFAULT_CENTRAL_STATE_FILE
         )
 
         if not os.path.isdir(self.base_folder):
             print(f"ERROR HERE")
@@ -126,19 +115,27 @@
             self._central_state = LocalCentralFile({}, [], [])
 
         else:
             with open(self.central_state_file, "r") as fh:
                 self._central_state = LocalCentralFile(**json.load(fh))
 
     def _write_central_file(self):
-        file_manager.safe_json_write(self._central_state.dict(), self.central_state_file)
+        """Save the central state to disk"""
+        file_manager.safe_json_write(
+            self._central_state.dict(), self.central_state_file
+        )
 
     def _write_resource_state_file(self, resource_state: Resource_State, fp: FilePath):
+        """Save the resource state to disk
+
+        Args:
+            resource_state (Resource_State)
+            fp (FilePath)
+        """
         file_manager.safe_json_write(resource_state.dict(), fp)
-    
 
     # Api for working with Resource States
     def create_resource_state(
         self, name: str, parent_resource_state_uuid: str = None
     ) -> str:
         # Create the new resource state
         if name in set(self._central_state.resource_state_names):
@@ -166,15 +163,15 @@
         self._central_state.resource_state_names.append(new_resource_state.name)
 
         self._write_central_file()
         self._write_resource_state_file(new_resource_state, filename)
 
         return new_resource_state.uuid
 
-    def delete_resource_state(self, resource_state_uuid: str):
+    def delete_resource_state(self, resource_state_uuid: str) -> None:
         if not resource_state_uuid in self._central_state.resource_state_locations:
             raise ResourceStateDoesNotExist(
                 f"Resource state: {resource_state_uuid} does not exist"
             )
 
         resource_state_to_delete = self.get_resource_state(resource_state_uuid)
 
@@ -216,33 +213,39 @@
             raise CanNotFindResourceStateFile(
                 f"Can not find resource state file for {resource_state_uuid}"
             )
 
         try:
             return file_manager.load_resource_state(file_location)
 
-
         except Exception as e:
             raise InvalidResourceStateData(
-                f"Ivalid data for Resource State from file {file_location} for resource state {resource_state_uuid}; {e}"
+                f"Invalid data for Resource State from file {file_location} for resource state {resource_state_uuid}; {e}"
             )
 
     def get_top_level_resource_states(self) -> List[Resource_State]:
         rv = []
-        
+
         for resource_id in self._central_state.top_level_states:
             # Let any exception from loading a state pass up to caller
             rv.append(self.get_resource_state(resource_id))
 
-        
         return rv
 
     # Components
-    def _create_component(self, resource_state_uuid: str, component_name: str):
+    def _create_component(self, resource_state_uuid: str, component_name: str) -> None:
+        """Create a component with the provide name in provided the resource state
+
+        Args:
+            resource_state_uuid (str)
+            component_name (str)
 
+        Raises:
+            ComponentAlreadyExists
+        """
         resource_state = self.get_resource_state(resource_state_uuid)
         resource_state_file_location = self._get_resource_state_file_location(
             resource_state_uuid
         )
 
         if component_name in set(x.name for x in resource_state.components):
             # Cant not have two components of the same name in the same resource state
@@ -256,16 +259,25 @@
 
         # Create a uuid for the component
         component_uuid = str(uuid.uuid4())
         resource_state.component_name_to_uuid[component_name] = component_uuid
 
         self._write_resource_state_file(resource_state, resource_state_file_location)
 
-    def _delete_component(self, resource_state_uuid: str, component_name: str):
+    def _delete_component(self, resource_state_uuid: str, component_name: str) -> None:
+        """Delete the component by name in a provided resource state
 
+        Args:
+            resource_state_uuid (str)
+            component_name (str)
+
+        Raises:
+            ComponentDoesNotExist
+            ComponentNotEmpty
+        """
         resource_state = self.get_resource_state(resource_state_uuid)
         resource_state_file_location = self._get_resource_state_file_location(
             resource_state_uuid
         )
 
         if not component_name in set(x.name for x in resource_state.components):
             # Component of that name does not exists
@@ -282,181 +294,212 @@
                 f"Can not delete Component {component_name} in Resource State {resource_state_uuid} because the component is not empty"
             )
 
         resource_state.components = [
             x for x in resource_state.components if not x.name == component_name
         ]
 
-        
         resource_state.component_name_to_uuid.pop(component_name)
 
         self._write_resource_state_file(resource_state, resource_state_file_location)
 
+    def _update_component_name(
+        self,
+        resource_state_uuid: str,
+        previous_component_name: str,
+        new_component_name: str,
+    ) -> None:
+        """Update the component by name
 
-    def _update_component_name(self, resource_state_uuid: str, previous_component_name: str, new_component_name: str):
+        Args:
+            resource_state_uuid (str)
+            previous_component_name (str)
+            new_component_name (str)
+
+        Raises:
+            ComponentDoesNotExist
+            ComponentAlreadyExists
+        """
         resource_state = self.get_resource_state(resource_state_uuid)
         resource_state_file_location = self._get_resource_state_file_location(
             resource_state_uuid
         )
 
-        if not previous_component_name in set(x.name for x in resource_state.components) or not previous_component_name in resource_state.component_name_to_uuid:
+        if (
+            not previous_component_name
+            in set(x.name for x in resource_state.components)
+            or not previous_component_name in resource_state.component_name_to_uuid
+        ):
             # Component of that name does not exists
             raise ComponentDoesNotExist(
                 f"Could not find component {previous_component_name} in Resource State {resource_state_uuid}"
             )
 
-
-        if new_component_name in set(x.name for x in resource_state.components) or new_component_name in resource_state.component_name_to_uuid:
+        if (
+            new_component_name in set(x.name for x in resource_state.components)
+            or new_component_name in resource_state.component_name_to_uuid
+        ):
             # Cant not have two components of the same name in the same resource state
             raise ComponentAlreadyExists(
                 f"Component already exists with name {new_component_name} in Resource State {resource_state_uuid}"
             )
 
         # get the component to rename
         rename_component = next(
             x for x in resource_state.components if x.name == previous_component_name
         )
 
         # remove the component from the list of components
         resource_state.components = [
-            x for x in resource_state.components if not x.name == previous_component_name
+            x
+            for x in resource_state.components
+            if not x.name == previous_component_name
         ]
 
         # Since ComponentModels are frozen, we can just change the name
         # So we make a dict of the current ComponentModel then change the name and use the dict as input
         # for a new ComponentModel Obj. Then add the new Obj to the resource state
         component_as_dict = rename_component.dict()
-        component_as_dict['name'] = new_component_name
+        component_as_dict["name"] = new_component_name
         new_component = ComponentModel(**component_as_dict)
 
         resource_state.components.append(new_component)
 
         # Update the name to uuid dict
         resource_state.component_name_to_uuid.pop(previous_component_name)
         resource_state.component_name_to_uuid[new_component_name] = new_component
 
-
         self._write_resource_state_file(resource_state, resource_state_file_location)
 
-        
-
     def get_component(
         self, resource_state_uuid: str, component_name: str
     ) -> ComponentModel:
-
         resource_state = self.get_resource_state(resource_state_uuid)
 
         if not component_name in set(x.name for x in resource_state.components):
             # Component of that name does not exists
             raise ComponentDoesNotExist(
                 f"Can not find Component {component_name} in Resource State {resource_state_uuid}"
             )
 
         return next(x for x in resource_state.components if x.name == component_name)
 
-
     def get_component_uuid(self, resource_state_uuid: str, component_name: str) -> str:
         resource_state = self.get_resource_state(resource_state_uuid)
 
         if not component_name in resource_state.component_name_to_uuid:
             raise ComponentDoesNotExist(
                 f"Can not find Component {component_name} in Resource State {resource_state_uuid}"
             )
 
         component_uuid = resource_state.component_name_to_uuid.get(component_name)
 
         return cdev_hasher.hash_list([resource_state_uuid, component_uuid])
 
-
     def update_component(
         self, resource_state_uuid: str, component_difference: Component_Difference
-    ):
+    ) -> None:
         if component_difference.action_type == Component_Change_Type.CREATE:
-            self._create_component(resource_state_uuid , component_difference.new_name)
+            self._create_component(resource_state_uuid, component_difference.new_name)
             return
 
         elif component_difference.action_type == Component_Change_Type.DELETE:
-            self._delete_component(resource_state_uuid, component_difference.previous_name)
+            self._delete_component(
+                resource_state_uuid, component_difference.previous_name
+            )
             return
 
         elif component_difference.action_type == Component_Change_Type.UPDATE_IDENTITY:
             return
 
-        elif  component_difference.action_type == Component_Change_Type.UPDATE_NAME:
-            self._update_component_name(resource_state_uuid, component_difference.previous_name, component_difference.new_name)
+        elif component_difference.action_type == Component_Change_Type.UPDATE_NAME:
+            self._update_component_name(
+                resource_state_uuid,
+                component_difference.previous_name,
+                component_difference.new_name,
+            )
 
         else:
-            raise Exception(f"Component Action type not supported {component_difference.action_type}")
-
+            raise Exception(
+                f"Component Action type not supported {component_difference.action_type}"
+            )
 
     def create_resource_change_transaction(
         self, resource_state_uuid: str, component_name: str, diff: Resource_Difference
     ) -> Tuple[str, str]:
         resource_state = self.get_resource_state(resource_state_uuid)
         resource_state_file_location = self._get_resource_state_file_location(
             resource_state_uuid
         )
 
         transaction_token = str(uuid.uuid4())
 
-        ruuid = diff.new_resource.ruuid if diff.new_resource else diff.previous_resource.ruuid
+        ruuid = (
+            diff.new_resource.ruuid
+            if diff.new_resource
+            else diff.previous_resource.ruuid
+        )
 
-        namespace_token = cdev_hasher.hash_list([resource_state_uuid, self.get_component_uuid(resource_state_uuid, component_name), ruuid])
+        namespace_token = cdev_hasher.hash_list(
+            [
+                resource_state_uuid,
+                self.get_component_uuid(resource_state_uuid, component_name),
+                ruuid,
+            ]
+        )
 
         resource_state.resource_changes[transaction_token] = (component_name, diff)
 
         self._write_resource_state_file(resource_state, resource_state_file_location)
 
         return transaction_token, namespace_token
 
-
     def complete_resource_change(
         self,
         resource_state_uuid: str,
         component_name: str,
         diff: Resource_Difference,
         transaction_token: str,
         cloud_output: Dict = None,
-        resolved_cloud_information: Dict={}
-    ):
+        resolved_cloud_information: Dict = {},
+    ) -> None:
 
         resource_state = self.get_resource_state(resource_state_uuid)
         resource_state_file_location = self._get_resource_state_file_location(
             resource_state_uuid
         )
 
-        
         if not transaction_token in resource_state.resource_changes:
-            
+
             raise ResourceChangeTransactionDoesNotExist(
                 f"Transaction {transaction_token} does not exist in Resource State {resource_state_uuid}"
             )
 
         component = self.get_component(resource_state_uuid, component_name)
-        
-        new_component = self._update_component(component, diff, cloud_output, resolved_cloud_information)
-        
-        
+
+        new_component = self._update_component(
+            component, diff, cloud_output, resolved_cloud_information
+        )
+
         resource_state.components = [
             x for x in resource_state.components if not x.name == component.name
         ] + [new_component]
 
         resource_state.resource_changes.pop(transaction_token)
 
         self._write_resource_state_file(resource_state, resource_state_file_location)
-        
 
     def fail_resource_change(
         self,
         resource_state_uuid: str,
         component_name: str,
         diff: Resource_Difference,
         transaction_token: str,
         failed_state: Dict,
-    ):
+    ) -> None:
 
         resource_state = self.get_resource_state(resource_state_uuid)
         resource_state_file_location = self._get_resource_state_file_location(
             resource_state_uuid
         )
 
         if not transaction_token in resource_state.resource_changes:
@@ -471,15 +514,15 @@
             failed_state,
         )
 
         self._write_resource_state_file(resource_state, resource_state_file_location)
 
     def change_failed_state_of_resource_change(
         self, resource_state_uuid: str, transaction_token: str, new_failed_state: Dict
-    ):
+    ) -> None:
 
         resource_state = self.get_resource_state(resource_state_uuid)
         resource_state_file_location = self._get_resource_state_file_location(
             resource_state_uuid
         )
 
         if not transaction_token in resource_state.failed_changes:
@@ -501,15 +544,15 @@
 
     def recover_failed_resource_change(
         self,
         resource_state_uuid: str,
         transaction_token: str,
         to_previous_state: bool = True,
         cloud_output: Dict = None,
-    ):
+    ) -> None:
 
         resource_state = self.get_resource_state(resource_state_uuid)
         resource_state_file_location = self._get_resource_state_file_location(
             resource_state_uuid
         )
 
         if not transaction_token in resource_state.failed_changes:
@@ -528,15 +571,15 @@
                 x for x in resource_state.components if not x.name == component_name
             ] + [new_component]
 
         self._write_resource_state_file(resource_state, resource_state_file_location)
 
     def remove_failed_resource_change(
         self, resource_state_uuid: str, transaction_token: str
-    ):
+    ) -> None:
 
         resource_state = self.get_resource_state(resource_state_uuid)
         resource_state_file_location = self._get_resource_state_file_location(
             resource_state_uuid
         )
 
         if not transaction_token in resource_state.failed_changes:
@@ -548,21 +591,23 @@
 
         self._write_resource_state_file(resource_state, resource_state_file_location)
 
     def resolve_reference_change(
         self,
         resource_state_uuid: str,
         diff: Resource_Reference_Difference,
-    ):
+    ) -> None:
         resource_state = self.get_resource_state(resource_state_uuid)
         resource_state_file_location = self._get_resource_state_file_location(
             resource_state_uuid
         )
 
-        component = self.get_component(resource_state_uuid, diff.originating_component_name)
+        component = self.get_component(
+            resource_state_uuid, diff.originating_component_name
+        )
 
         _reference_resource_state = resource_state
         if diff.resource_reference.is_in_parent_resource_state:
             if not resource_state.parent_uuid:
                 raise ResourceReferenceError(
                     f"Current Resource State {resource_state_uuid} does not have a Parent Resource State to resolve {diff} to"
                 )
@@ -589,15 +634,15 @@
             in all_parent_resources
         ):
             raise ResourceReferenceError(
                 f"Could not find resource {diff.resource_reference.ruuid};{diff.resource_reference.name} in parent component"
             )
 
         if diff.action_type == Resource_Reference_Change_Type.CREATE:
-            
+
             reference_id = (
                 f"{diff.resource_reference.ruuid}{diff.resource_reference.name}"
             )
 
             # resolve the reference by adding a count to the reference counter in the referenced component
             if not reference_id in _referenced_component.external_references:
                 _referenced_component.external_references[reference_id] = {"cnt": 1}
@@ -610,15 +655,15 @@
                     "cnt": previous_cnt + 1
                 }
 
             # Add this to the references for this component
             component.references.append(diff.resource_reference)
 
         elif diff.action_type == Resource_Reference_Change_Type.DELETE:
-            
+
             reference_id = (
                 f"{diff.resource_reference.ruuid}{diff.resource_reference.name}"
             )
 
             # resolve the dereference by subtracting a count to the reference counter in the referenced component
             if not reference_id in _referenced_component.external_references:
                 raise ResourceReferenceError(
@@ -780,15 +825,14 @@
         if not key in cloud_output:
             raise KeyNotInCloudOutput(
                 f"Can not find Key {key} in Cloud Output for {resource_type}::{resource_hash} in Component {component_name} in Resource State {resource_state_uuid}"
             )
 
         return cloud_output.get(key)
 
-
     def get_cloud_output_by_name(
         self,
         resource_state_uuid: str,
         component_name: str,
         resource_type: str,
         resource_name: str,
     ) -> Any:
@@ -819,131 +863,144 @@
         Component_Difference, Resource_Reference_Difference, Resource_Difference
     ]:
         try:
             # Load the previous components
             previous_components: List[ComponentModel] = [
                 self.get_component(resource_state_uuid, x) for x in old_components
             ]
-           
+
         except Exception as e:
             raise e
 
         return _create_differences(new_components, previous_components)
 
     def _update_component(
         self,
         component: ComponentModel,
         diff: Resource_Difference,
         new_cloud_output: Dict = {},
-        resolved_cloud_information: Dict={}
+        resolved_cloud_information: Dict = {},
     ) -> ComponentModel:
-        """
-        Apply a resource difference over a component model and return the updated component model
+        """Apply a resource difference over a component model and return the updated component model
 
-        Arguments:
+        Args:
             component(ComponentModel): The component to update
             diff (Resource_Difference): The difference to apply
             new_cloud_output (Dict): The updated output if needed
             resolved_cloud_information (Dict): cloud output information used to deploy resource
 
         Returns:
-            new_component(ComponentModel): The update component model
-
+            new_component(ComponentModel)
         """
         if diff.action_type == Resource_Change_Type.DELETE:
-            
+
             component.resources = [
                 x
                 for x in component.resources
-                if not (x.ruuid == diff.previous_resource.ruuid and x.name == diff.previous_resource.name)
-            ] 
-            
+                if not (
+                    x.ruuid == diff.previous_resource.ruuid
+                    and x.name == diff.previous_resource.name
+                )
+            ]
+
             # remove the previous resource's cloud output
             previous_resource_cloud_output_id = self._get_cloud_output_id(
                 diff.previous_resource
             )
-            
+
             if previous_resource_cloud_output_id in component.cloud_output:
                 component.cloud_output.pop(previous_resource_cloud_output_id)
 
-
-            if previous_resource_cloud_output_id  in component.previous_resolved_cloud_values:
-                component.previous_resolved_cloud_values.pop(previous_resource_cloud_output_id)
-            
+            if (
+                previous_resource_cloud_output_id
+                in component.previous_resolved_cloud_values
+            ):
+                component.previous_resolved_cloud_values.pop(
+                    previous_resource_cloud_output_id
+                )
 
         elif (
             diff.action_type == Resource_Change_Type.UPDATE_IDENTITY
             or diff.action_type == Resource_Change_Type.UPDATE_NAME
         ):
-                   
+
             component.resources = [
                 x
                 for x in component.resources
-                if not (x.ruuid == diff.previous_resource.ruuid and x.name == diff.previous_resource.name)
-            ]  +  [diff.new_resource]
+                if not (
+                    x.ruuid == diff.previous_resource.ruuid
+                    and x.name == diff.previous_resource.name
+                )
+            ] + [diff.new_resource]
 
             # remove the previous resource's cloud output
             previous_resource_cloud_output_id = self._get_cloud_output_id(
                 diff.previous_resource
             )
 
             if previous_resource_cloud_output_id in component.cloud_output:
                 component.cloud_output.pop(previous_resource_cloud_output_id)
 
-            if previous_resource_cloud_output_id  in component.previous_resolved_cloud_values:
-                component.previous_resolved_cloud_values.pop(previous_resource_cloud_output_id)
-            
+            if (
+                previous_resource_cloud_output_id
+                in component.previous_resolved_cloud_values
+            ):
+                component.previous_resolved_cloud_values.pop(
+                    previous_resource_cloud_output_id
+                )
+
             cloud_output_id = self._get_cloud_output_id(diff.new_resource)
             component.cloud_output[cloud_output_id] = new_cloud_output
 
-            component.previous_resolved_cloud_values[cloud_output_id] = resolved_cloud_information
-        
+            component.previous_resolved_cloud_values[
+                cloud_output_id
+            ] = resolved_cloud_information
 
         elif diff.action_type == Resource_Change_Type.CREATE:
-            component.resources.append(diff.new_resource)            
+            component.resources.append(diff.new_resource)
 
             cloud_output_id = self._get_cloud_output_id(diff.new_resource)
 
             component.cloud_output[cloud_output_id] = new_cloud_output
-            component.previous_resolved_cloud_values[cloud_output_id] = resolved_cloud_information
+            component.previous_resolved_cloud_values[
+                cloud_output_id
+            ] = resolved_cloud_information
 
         # recompute hash
         component.hash = _compute_component_hash(component)
 
         return component
 
     def _get_cloud_output_id(self, resource: ResourceModel) -> str:
-        """
-        Uniform way of generating cloud mapping id's
+        """Uniform way of generating cloud mapping id's
 
-        Arguments:
+        Args:
             resource (ResourceModel): resource to get id of
 
         Returns:
             cloud_output_id (str): id for the resource
         """
         return f"{resource.ruuid};{resource.name}"
 
     def _get_resource_state_file_location(self, resource_state_uuid: str) -> FilePath:
         return self._central_state.resource_state_locations.get(resource_state_uuid)
 
 
 # Helper functions
 def _compute_component_hash(component: ComponentModel) -> str:
-    """
-    Uniform way of computing a component's identity hash
+    """Uniform way of computing a component's identity hash
 
-    Argument:
+    Args:
         component (ComponentModel): The component to compute the hash of
 
     Returns:
         hash (str): identity hash for the component
     """
     if component.resources:
-        
+
         resources = [x for x in component.resources]
         resources.sort(key=lambda x: x.hash)
 
         resource_hashes = [x.hash for x in resources]
     else:
         resource_hashes = []
 
@@ -962,29 +1019,37 @@
 
 
 def _create_resource_diffs(
     component_name: str,
     new_resources: List[ResourceModel],
     old_resource: List[ResourceModel],
 ) -> List[Resource_Difference]:
+    """Create the differences between differences in the resources
+
+    Args:
+        component_name (str)
+        new_resources (List[ResourceModel]
+        old_resource (List[ResourceModel])
 
+    Returns:
+        List[Resource_Difference]
+    """
     if old_resource:
         # build map<hash,resource>
         old_hash_to_resource: Dict[str, ResourceModel] = {
             x.hash: x for x in old_resource
         }
         # build map<name,resource>
         old_name_to_resource: Dict[str, ResourceModel] = {
             x.name: x for x in old_resource
         }
     else:
         old_hash_to_resource = {}
         old_name_to_resource = {}
 
-
     rv = []
     for resource in new_resources:
         if (
             resource.hash in old_hash_to_resource
             and resource.name in old_name_to_resource
         ):
 
@@ -1028,29 +1093,29 @@
             # POP the seen previous resources as we go so only remaining resources will be deletes
             old_resource.remove(old_name_to_resource.get(resource.name))
 
         elif (
             not resource.hash in old_hash_to_resource
             and not resource.name in old_name_to_resource
         ):
-            
+
             rv.append(
                 Resource_Difference(
                     **{
                         "action_type": Resource_Change_Type.CREATE,
                         "component_name": component_name,
                         "previous_resource": None,
                         "new_resource": resource,
                     }
                 )
             )
 
     if old_resource:
         for resource in old_resource:
-           
+
             rv.append(
                 Resource_Difference(
                     **{
                         "action_type": Resource_Change_Type.DELETE,
                         "component_name": component_name,
                         "previous_resource": resource,
                         "new_resource": None,
@@ -1060,17 +1125,26 @@
 
     return rv
 
 
 def _create_reference_diffs(
     new_references: List[ResourceReferenceModel],
     old_references: List[ResourceReferenceModel],
-    originating_component_name: str, 
+    originating_component_name: str,
 ) -> List[Resource_Reference_Difference]:
+    """Create the differences between components
+
+    Args:
+        new_references (List[ResourceReferenceModel])
+        old_references (List[ResourceReferenceModel])
+        originating_component_name (str)
 
+    Returns:
+        List[Resource_Reference_Difference]
+    """
     if old_references:
         # build map<name,resource>
         old_name_to_references: Dict[str, ResourceReferenceModel] = {
             f"{x.ruuid};;{x.name}": x for x in old_references
         }
     else:
         old_name_to_references = {}
@@ -1081,37 +1155,52 @@
         if _id in old_name_to_references:
             # POP the seen previous resources as we go so only remaining resources will be deletes
             old_references.remove(old_name_to_references.get(_id))
 
         else:
             rv.append(
                 Resource_Reference_Difference(
-                    Resource_Reference_Change_Type.CREATE, originating_component_name, reference
+                    Resource_Reference_Change_Type.CREATE,
+                    originating_component_name,
+                    reference,
                 )
             )
 
     for old_reference in old_references:
-        
+
         rv.append(
             Resource_Reference_Difference(
-                Resource_Reference_Change_Type.DELETE, originating_component_name, old_reference
+                Resource_Reference_Change_Type.DELETE,
+                originating_component_name,
+                old_reference,
             )
         )
 
     return rv
 
 
 def _create_differences(
     new_components: List[ComponentModel], previous_components: List[ComponentModel]
 ) -> Tuple[
     List[Component_Difference],
     List[Resource_Difference],
-    List[Resource_Reference_Difference]
+    List[Resource_Reference_Difference],
 ]:
+    """Create the differences between components
 
+    Args:
+        new_components (List[ComponentModel])
+        previous_components (List[ComponentModel])
+
+    Raises:
+        Exception
+
+    Returns:
+        Tuple[ List[Component_Difference], List[Resource_Difference], List[Resource_Reference_Difference], ]
+    """
     component_diffs = []
     resource_diffs = []
     reference_diffs = []
 
     if previous_components:
         # build map<hash,resource>
         previous_hash_to_component = {x.hash: x for x in previous_components}
@@ -1127,27 +1216,29 @@
         for component in new_components:
 
             if (
                 not component.hash in previous_hash_to_component
                 and not component.name in previous_name_to_component
             ):
                 # Create component and all resources and all references
-            
+
                 component_diffs.append(
                     Component_Difference(
                         Component_Change_Type.CREATE, new_name=component.name
                     )
                 )
 
                 tmp_resource_diff = _create_resource_diffs(
                     component.name, component.resources, []
                 )
                 resource_diffs.extend(tmp_resource_diff)
 
-                tmp_reference_diff = _create_reference_diffs(component.references, [], component.name)
+                tmp_reference_diff = _create_reference_diffs(
+                    component.references, [], component.name
+                )
                 reference_diffs.extend(tmp_reference_diff)
 
             elif (
                 component.hash in previous_hash_to_component
                 and component.name in previous_name_to_component
             ):
                 # Since the hash is the same we can infer all the resource hashes and reference hashes are the same
@@ -1247,11 +1338,13 @@
         )
 
         tmp_resource_diff = _create_resource_diffs(
             removed_component.name, [], removed_component.resources
         )
         resource_diffs.extend(tmp_resource_diff)
 
-        tmp_reference_diff = _create_reference_diffs([], removed_component.references, removed_component.name)
+        tmp_reference_diff = _create_reference_diffs(
+            [], removed_component.references, removed_component.name
+        )
         reference_diffs.extend(tmp_reference_diff)
 
     return component_diffs, resource_diffs, reference_diffs
```

### Comparing `cdev-0.0.8/core/default/cloudmapper.py` & `cdev-0.0.9/core/default/cloudmapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,83 @@
 from typing import Callable, Dict, List, Set
 
 
 from core.constructs.output_manager import OutputTask
 
-from ..constructs.resource import Resource_Change_Type, Resource_Reference_Difference, Resource_Difference
+from ..constructs.resource import (
+    Resource_Change_Type,
+    Resource_Reference_Difference,
+    Resource_Difference,
+)
 from ..constructs.mapper import CloudMapper
 
-#from .mappers.aws import aws_lambda, dynamodb, iam, s3, sqs, apigatewayv2, apigateway
+# from .mappers.aws import aws_lambda, dynamodb, iam, s3, sqs, apigatewayv2, apigateway
 
 from .mappers.simple import (
     api_deployer,
     bucket_deployer,
     lambda_deployer,
     dynamodb_deployer,
     queue_deployer,
     relational_db_deployer,
     static_site_deployer,
-    topic_deployer
+    topic_deployer,
 )
 
-class DefaultMapper(CloudMapper):   
-    
+
+class DefaultMapper(CloudMapper):
     def __init__(self) -> None:
         super().__init__(RESOURCE_TO_HANDLER_FUNCTION)
 
     def get_namespaces(self) -> List[str]:
         return [
             "cdev::simple::api",
             "cdev::simple::bucket",
             "cdev::simple::function",
             "cdev::simple::lambda_layer",
             "cdev::simple::table",
             "cdev::simple::queue",
             "cdev::simple::relationaldb",
             "cdev::simple::staticsite",
-            "cdev::simple::topic"
+            "cdev::simple::topic",
         ]
 
-    def deploy_resource(self, transaction_token: str, namespace_token: str, resource_diff: Resource_Difference, previous_output: Dict, output_task: OutputTask) -> Dict:
-        ruuid = resource_diff.new_resource.ruuid if resource_diff.new_resource else resource_diff.previous_resource.ruuid
-
-        return self.get_resource_to_handler()[ruuid](transaction_token, namespace_token, resource_diff, previous_output, output_task)
-    
+    def deploy_resource(
+        self,
+        transaction_token: str,
+        namespace_token: str,
+        resource_diff: Resource_Difference,
+        previous_output: Dict,
+        output_task: OutputTask,
+    ) -> Dict:
+        ruuid = (
+            resource_diff.new_resource.ruuid
+            if resource_diff.new_resource
+            else resource_diff.previous_resource.ruuid
+        )
+
+        return self.get_resource_to_handler()[ruuid](
+            transaction_token,
+            namespace_token,
+            resource_diff,
+            previous_output,
+            output_task,
+        )
 
     def get_available_resources(self) -> Set[str]:
         return set(self.get_namespaces())
 
     def get_resource_to_handler(self) -> Dict[str, Callable]:
         return self.resource_to_handler
-        
 
 
 RESOURCE_TO_HANDLER_FUNCTION = {
-   
     "cdev::simple::function": lambda_deployer.handle_simple_lambda_function_deployment,
     "cdev::simple::lambda_layer": lambda_deployer.handle_simple_layer_deployment,
     "cdev::simple::api": api_deployer.handle_simple_api_deployment,
     "cdev::simple::bucket": bucket_deployer.handle_simple_bucket_deployment,
     "cdev::simple::table": dynamodb_deployer.handle_simple_table_deployment,
     "cdev::simple::queue": queue_deployer.handle_simple_queue_deployment,
     "cdev::simple::relationaldb": relational_db_deployer.handle_simple_relational_db_deployment,
     "cdev::simple::staticsite": static_site_deployer.handle_simple_static_site_deployment,
-    "cdev::simple::topic": topic_deployer.handle_simple_topic_deployment
-    
+    "cdev::simple::topic": topic_deployer.handle_simple_topic_deployment,
 }
```

### Comparing `cdev-0.0.8/core/default/commands/bucket/cp.py` & `cdev-0.0.9/core/default/commands/bucket/cp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 """Command for uploading objects to a Bucket
 
 """
 from argparse import ArgumentParser
 from imp import source_from_cache
 import boto3
 import os
@@ -14,18 +13,17 @@
 
 from . import utils
 
 
 class cp(BaseCommand):
     help = """
     Command to mirror s3 `cp` command.
-    
-    """
 
-    def add_arguments(self, parser: ArgumentParser):
+    """
+    def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument(
             "source",
             type=str,
             help="The source of the file. Must either be a local path or bucket location (bucket://<component>.<name>/<path>)",
         )
         parser.add_argument(
             "destination",
@@ -35,122 +33,111 @@
 
         parser.add_argument(
             "--recursive",
             action="store_true",
             help="The destination of the file. Must either be a local path or bucket location (bucket://<component>.<name>/<path>)",
         )
 
-    def command(self, *args, **kwargs):
-        
+    def command(self, *args, **kwargs) -> None:
+
         source_raw = kwargs.get("source")
         destination_raw = kwargs.get("destination")
 
         is_recursive = kwargs.get("recursive")
 
-
         if utils.is_valid_remote(source_raw):
             is_source_remote = True
             source = utils.parse_remote_location(source_raw)
-            
+
         elif os.path.isfile(source_raw):
             is_source_remote = False
             source = source_raw
 
         elif os.path.isdir(source_raw) and is_recursive:
             is_source_remote = False
             source = source_raw
 
         else:
-            raise Exception(f"Source {source_raw} is neither a valid location on the file system or a valid remote location")
-
-
+            raise Exception(
+                f"Source {source_raw} is neither a valid location on the file system or a valid remote location"
+            )
 
         if utils.is_valid_remote(destination_raw):
             is_destination_remote = True
             destination = utils.parse_remote_location(destination_raw)
-        
+
         elif os.path.isdir(destination_raw):
             is_destination_remote = False
             destination = destination_raw
 
         elif os.path.isdir(os.path.dirname(destination_raw)):
             is_destination_remote = False
             destination = destination_raw
 
-        
-
         else:
-            raise Exception(f"Destination {destination_raw} is neither a valid location on the file system or a valid remote location")
-
+            raise Exception(
+                f"Destination {destination_raw} is neither a valid location on the file system or a valid remote location"
+            )
 
         if not is_destination_remote and not is_source_remote:
-            raise Exception(f"Both destination ({destination}) and source ({source}) are file system locations")
-
+            raise Exception(
+                f"Both destination ({destination}) and source ({source}) are file system locations"
+            )
 
         s3 = boto3.resource("s3")
-        
 
         if is_destination_remote and not is_source_remote:
-            # Remote destination and local file system. 
+            # Remote destination and local file system.
             # Copying up
-            cloud_output = utils.get_cloud_output_from_cdev_name(destination.component_name, destination.cdev_bucket_name)
-            bucket_name = cloud_output.get('bucket_name')
-            
+            cloud_output = utils.get_cloud_output_from_cdev_name(
+                destination.component_name, destination.cdev_bucket_name
+            )
+            bucket_name = cloud_output.get("bucket_name")
 
             bucket = s3.Bucket(bucket_name)
 
             if destination.path:
                 key_name = destination.path
             else:
                 key_name = source
 
             mimetype, _ = mimetypes.guess_type(source)
             if mimetype is None:
                 raise Exception("Failed to guess mimetype")
 
             self.stdout.write(f"Upload {source_raw} ->  {destination_raw}")
-            bucket.upload_file(
-                source, key_name, ExtraArgs={"ContentType": mimetype}
-            )
+            bucket.upload_file(source, key_name, ExtraArgs={"ContentType": mimetype})
 
         if not is_destination_remote and is_source_remote:
             # Local destination and remote source.
             # Pulling down
 
-            cloud_output = utils.get_cloud_output_from_cdev_name(source.component_name, source.cdev_bucket_name)
-            bucket_name = cloud_output.get('bucket_name')
-            
+            cloud_output = utils.get_cloud_output_from_cdev_name(
+                source.component_name, source.cdev_bucket_name
+            )
+            bucket_name = cloud_output.get("bucket_name")
 
             bucket = s3.Bucket(bucket_name)
 
             self.stdout.write(f"Download {source_raw} -> {destination_raw} ")
             bucket.download_file(source.path, destination)
 
-
         if is_destination_remote and is_source_remote:
             # Local destination and remote source.
             # Pulling down
 
-            source_cloud_output = utils.get_cloud_output_from_cdev_name(source.component_name, source.cdev_bucket_name)
-            source_bucket_name = source_cloud_output.get('bucket_name')
-
-            destination_cloud_output = utils.get_cloud_output_from_cdev_name(destination.component_name, destination.cdev_bucket_name)
-            destination_bucket_name = destination_cloud_output.get('bucket_name')
-            
-
+            source_cloud_output = utils.get_cloud_output_from_cdev_name(
+                source.component_name, source.cdev_bucket_name
+            )
+            source_bucket_name = source_cloud_output.get("bucket_name")
+            destination_cloud_output = utils.get_cloud_output_from_cdev_name(
+                destination.component_name, destination.cdev_bucket_name
+            )
+            destination_bucket_name = destination_cloud_output.get("bucket_name")
             destination_bucket = s3.Bucket(destination_bucket_name)
 
             destination_key = destination.path if destination.path else source.path
 
             self.stdout.write(f"Copy {source_raw} -> {destination_raw}")
             destination_bucket.copy(
-                {
-                    'Bucket': source_bucket_name,
-                    'Key': source.path
-                }, 
-                destination_key
+                {"Bucket": source_bucket_name, "Key": source.path}, destination_key
             )
-
-
-
-
-
```

### Comparing `cdev-0.0.8/core/default/commands/bucket/sync.py` & `cdev-0.0.9/core/default/commands/bucket/sync.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,61 @@
-
 """Command for syncing a set of resources to a static site
 """
 from argparse import ArgumentParser
 import boto3
 import os
 import mimetypes
 
-from core.constructs.commands import BaseCommand, OutputWrapper
-from core.default.resources.simple.object_store import Bucket, bucket_model
+from core.constructs.commands import BaseCommand
 from core.utils.paths import get_full_path_from_workspace_base
 
 from . import utils
 
 
 class sync_files(BaseCommand):
     help = """
     Command to sync a folder of content to a bucket
     """
 
-    def add_arguments(self, parser: ArgumentParser):
+    def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument(
             "resource_name", type=str, help="The bucket resource you want to sync."
         )
         parser.add_argument(
             "--dir",
             type=str,
             help="content folder to sync to the resource.",
         )
         parser.add_argument(
             "--clear",
             action="store_true",
             help="Clear the existing content of the bucket before syncing the new data.",
         )
 
-    def command(self, *args, **kwargs):
+    def command(self, *args, **kwargs) -> None:
         full_resource_name: str = kwargs.get("resource_name")
-        component_name = full_resource_name.split('.')[0]
-        bucket_cdev_name = full_resource_name.split('.')[1]
+        component_name = full_resource_name.split(".")[0]
+        bucket_cdev_name = full_resource_name.split(".")[1]
         content_directory = kwargs.get("dir")
         clear_bucket = kwargs.get("clear")
 
-        cloud_output = utils.get_cloud_output_from_cdev_name(component_name, bucket_cdev_name)
+        cloud_output = utils.get_cloud_output_from_cdev_name(
+            component_name, bucket_cdev_name
+        )
 
         final_dir = get_full_path_from_workspace_base(content_directory)
 
         bucket_name = cloud_output.get("bucket_name")
-        
 
         s3 = boto3.resource("s3")
         bucket = s3.Bucket(bucket_name)
 
         if clear_bucket:
             bucket.object_versions.delete()
 
-
         for subdir, dirs, files in os.walk(final_dir):
             for file in files:
                 full_path = os.path.join(subdir, file)
 
                 key_name = os.path.relpath(full_path, final_dir)
 
                 mimetype, _ = mimetypes.guess_type(full_path)
```

### Comparing `cdev-0.0.8/core/default/commands/bucket/utils.py` & `cdev-0.0.9/core/default/commands/bucket/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,73 +3,66 @@
 from tokenize import group
 
 from core.constructs.resource import ResourceModel
 from core.constructs.workspace import Workspace
 
 RUUID = "cdev::simple::bucket"
 
+
 def get_cloud_output_from_cdev_name(component_name: str, cdev_name: str) -> str:
     try:
         ws = Workspace.instance()
 
-
         cloud_output = ws.get_backend().get_cloud_output_by_name(
-            ws.get_resource_state_uuid(),
-            component_name,
-            RUUID, 
-            cdev_name
+            ws.get_resource_state_uuid(), component_name, RUUID, cdev_name
         )
 
         return cloud_output
     except Exception as e:
         print(f"Could not find resource {component_name}:{RUUID}:{cdev_name}")
         print(e)
         return None
 
 
-
 def get_resource_from_cdev_name(component_name: str, cdev_name: str) -> ResourceModel:
     try:
         ws = Workspace.instance()
 
-
         resource = ws.get_backend().get_resource_by_name(
-            ws.get_resource_state_uuid(),
-            component_name,
-            RUUID, 
-            cdev_name
+            ws.get_resource_state_uuid(), component_name, RUUID, cdev_name
         )
 
         return resource
     except Exception as e:
         print(f"Could not find resource {component_name}:{RUUID}:{cdev_name}")
         print(e)
         return None
 
 
 remote_name_regex = "bucket://([a-z,_]+).([a-z,_]+)/?(\S+)?"
 compiled_regex = re.compile(remote_name_regex)
 
+
 @dataclass
 class remote_location:
     component_name: str
     cdev_bucket_name: str
     path: str
 
+
 def is_valid_remote(name: str) -> bool:
     return True if compiled_regex.match(name) else False
 
 
 def parse_remote_location(name: str) -> remote_location:
     match = compiled_regex.match(name)
 
     if not match:
-        raise Exception("provided name {name} does not match regex for a remote bucket object")
+        raise Exception(
+            "provided name {name} does not match regex for a remote bucket object"
+        )
 
     return remote_location(
         component_name=match.group(1),
         cdev_bucket_name=match.group(2),
-        path=match.group(3)
+        path=match.group(3),
     )
-
-
-
```

### Comparing `cdev-0.0.8/core/default/commands/function/execute.py` & `cdev-0.0.9/core/default/commands/function/execute.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,92 +1,84 @@
-
-from argparse import ArgumentParser
 import json
 import os
-from typing import List, Dict
 
+from argparse import ArgumentParser
+from typing import Dict
 from boto3 import client
 
-from core.constructs.commands import BaseCommand, OutputWrapper
-from core.constructs.workspace import Workspace
-from core.utils import hasher
-
-
-
+from core.constructs.commands import BaseCommand
 from core.default.commands.function.utils import get_cloud_id_from_cdev_name
 
 RUUID = "cdev::simple::function"
 
 
 class execute(BaseCommand):
 
     help = """
         Execute a function in the cloud.
     """
 
-    def add_arguments(self, parser: ArgumentParser):
+    def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument(
-            "function_id", 
-            type=str, 
-            help="The id of the function to execute."
+            "function_id", type=str, help="The id of the function to execute."
         )
         parser.add_argument(
             "--event",
             type=str,
             help="File (json) location of event object to provide as input to the function. Can not be used with '--event-data` flag.",
         )
         parser.add_argument(
             "--event-data",
             type=str,
             help="Raw string form of event object to provide as input to the function. Can not be used with '--event' flag.",
         )
-        
-       
 
-    def command(self, *args, **kwargs):
+    def command(self, *args, **kwargs) -> None:
+
+        event_data = self._get_event_data(*args, **kwargs)
 
-        full_function_name: str = kwargs.get("function_id")
+        full_function_name = kwargs.get("function_id")
+        (
+            component_name,
+            function_name,
+        ) = self.get_component_and_resource_from_qualified_name(full_function_name)
+
+        cloud_name = get_cloud_id_from_cdev_name(component_name, function_name)
+
+        lambda_client = client("lambda")
+
+        self.stdout.write(f"executing {full_function_name}")
+        response = lambda_client.invoke(
+            FunctionName=cloud_name,
+            InvocationType="RequestResponse",
+            Payload=json.dumps(event_data),
+        )
 
+        self.stdout.write(str(response))
+
+    def _get_event_data(self, *args, **kwargs) -> Dict:
         event_file_location: str = kwargs.get("event")
         event_raw_data: str = kwargs.get("event_data")
 
         if event_file_location and event_raw_data:
             raise Exception("Can not provide both '--event-data' and '--event'")
 
-        event_data = {}
-
         if event_file_location:
             if not os.path.isfile(event_file_location):
                 raise Exception(f"{event_file_location} is not a valid file location")
 
             with open(event_file_location) as fh:
                 try:
                     event_data = json.load(fh)
+                    return event_data
                 except Exception as e:
                     print(e)
-                    raise Exception(f'Could not load {event_file_location} as json')
+                    raise Exception(f"Could not load {event_file_location} as json")
 
-                
         if event_raw_data:
             try:
                 event_data = json.loads(event_raw_data)
+                return event_data
             except Exception as e:
                 print(e)
-                raise Exception(f'Could not load {event_raw_data} as json')
-
-
-        component_name = full_function_name.split('.')[0]
-        function_name = full_function_name.split('.')[1]
-
-        cloud_name = get_cloud_id_from_cdev_name(component_name, function_name)
-
-        lambda_client = client('lambda')    
-
-        self.stdout.write(f'executing {full_function_name}')
-        response = lambda_client.invoke(
-            FunctionName=cloud_name,
-            InvocationType='RequestResponse',
-            Payload=json.dumps(event_data)
-        )
-
-
-        print(response)
+                raise Exception(f"Could not load {event_raw_data} as json")
+        return {}
```

### Comparing `cdev-0.0.8/core/default/commands/function/utils.py` & `cdev-0.0.9/core/default/commands/function/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+from typing import Tuple, Optional
+
 from core.constructs.workspace import Workspace
 
 
 RUUID = "cdev::simple::function"
 
-def get_cloud_id_from_cdev_name(component_name: str, cdev_function_name: str) -> str:
+
+def get_cloud_id_from_cdev_name(component_name: str, cdev_function_name: str) -> Optional[str]:
     try:
         ws = Workspace.instance()
 
-
         cloud_id = ws.get_backend().get_cloud_output_value_by_name(
             ws.get_resource_state_uuid(),
             component_name,
-            RUUID, 
-            cdev_function_name, 
-            "cloud_id"
+            RUUID,
+            cdev_function_name,
+            "cloud_id",
         )
 
         return cloud_id
     except Exception as e:
         print(f"Could not find cloud id")
         print(e)
-        return None
+    return None
```

### Comparing `cdev-0.0.8/core/default/commands/relationaldb/utils.py` & `cdev-0.0.9/core/default/commands/relationaldb/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-
 from typing import Tuple
 
 from core.constructs.workspace import Workspace
 from core.default.resources.simple.relational_db import simple_relational_db_model
 
 RUUID = "cdev::simple::relationaldb"
 
-def get_db_info_from_cdev_name(component_name: str, cdev_database_name: str) -> Tuple[str,str,str]:
+
+def get_db_info_from_cdev_name(
+    component_name: str, cdev_database_name: str
+) -> Tuple[str, str, str]:
     """_summary_
 
     Args:
         component_name (str): Name of the component that the resource is in
         cdev_database_name (str): Name of the resource
 
     Returns:
@@ -18,32 +20,32 @@
     """
     try:
         ws = Workspace.instance()
 
         cluster_arn = ws.get_backend().get_cloud_output_value_by_name(
             ws.get_resource_state_uuid(),
             component_name,
-            RUUID, 
-            cdev_database_name, 
-            "cluster_arn"
+            RUUID,
+            cdev_database_name,
+            "cluster_arn",
         )
 
-        
         secret_arn = ws.get_backend().get_cloud_output_value_by_name(
             ws.get_resource_state_uuid(),
             component_name,
-            RUUID, 
-            cdev_database_name, 
-            "secret_arn"
+            RUUID,
+            cdev_database_name,
+            "secret_arn",
         )
 
-        db_resource_model: simple_relational_db_model  = ws.get_backend().get_resource_by_name(
-            ws.get_resource_state_uuid(),
-            component_name,
-            RUUID, 
-            cdev_database_name, 
+        db_resource_model: simple_relational_db_model = (
+            ws.get_backend().get_resource_by_name(
+                ws.get_resource_state_uuid(),
+                component_name,
+                RUUID,
+                cdev_database_name,
+            )
         )
 
-
         return (cluster_arn, secret_arn, db_resource_model.DatabaseName)
     except Exception as e:
         print(e)
```

### Comparing `cdev-0.0.8/core/default/commands/static_site/utils.py` & `cdev-0.0.9/core/default/commands/static_site/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,36 @@
+from typing import Optional, Dict
+
 from core.constructs.resource import ResourceModel
 from core.constructs.workspace import Workspace
 
 RUUID = "cdev::simple::staticsite"
 
-def get_cloud_output_from_cdev_name(component_name: str, cdev_name: str) -> str:
+
+def get_cloud_output_from_cdev_name(component_name: str, cdev_name: str) -> Optional[Dict]:
     try:
         ws = Workspace.instance()
 
-
         cloud_output = ws.get_backend().get_cloud_output_by_name(
-            ws.get_resource_state_uuid(),
-            component_name,
-            RUUID, 
-            cdev_name
+            ws.get_resource_state_uuid(), component_name, RUUID, cdev_name
         )
 
         return cloud_output
     except Exception as e:
         print(f"Could not find resource {component_name}:{RUUID}:{cdev_name}")
         print(e)
         return None
 
 
-
-def get_resource_from_cdev_name(component_name: str, cdev_name: str) -> ResourceModel:
+def get_resource_from_cdev_name(component_name: str, cdev_name: str) -> Optional[ResourceModel]:
     try:
         ws = Workspace.instance()
 
-
         resource = ws.get_backend().get_resource_by_name(
-            ws.get_resource_state_uuid(),
-            component_name,
-            RUUID, 
-            cdev_name
+            ws.get_resource_state_uuid(), component_name, RUUID, cdev_name
         )
 
         return resource
     except Exception as e:
         print(f"Could not find resource {component_name}:{RUUID}:{cdev_name}")
         print(e)
         return None
-
```

### Comparing `cdev-0.0.8/core/default/commands/table/clear_table.py` & `cdev-0.0.9/core/default/commands/table/clear_table.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,43 @@
-from argparse import ArgumentParser
-from typing import Dict, List
 
 import boto3
 
+from argparse import ArgumentParser
 
 from core.constructs.commands import BaseCommand, OutputWrapper
-from core.default.resources.simple.table import Table
-from core.utils.paths import get_full_path_from_workspace_base
 
 
 from . import utils
 
 RUUID = "cdev::simple::table"
 
 
 class clear_table(BaseCommand):
 
     help = """
-Clear the current data from a given Table. This should only be used on development tables.   
+Clear the current data from a given Table. This should only be used on development tables.
 """
 
-    def add_arguments(self, parser: ArgumentParser):
+    def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument(
             "resource_name", type=str, help="The resource you want to sync data to"
         )
 
-    def command(self, *args, **kwargs):
+    def command(self, *args, **kwargs) -> None:
         """
         Clear all items for the table
         """
         # https://stackoverflow.com/questions/55169952/delete-all-items-dynamodb-using-python
 
-        full_resource_name = kwargs.get("resource_name")
-        component_name = full_resource_name.split('.')[0]
-        table_resource_name = full_resource_name.split('.')[1]
+        component_name, table_resource_name = self.get_component_and_resource_from_qualified_name(kwargs.get("resource_name"))
 
-        cloud_output = utils.get_cloud_output_from_cdev_name(component_name, table_resource_name)
-        table_cloud_name = cloud_output.get('table_name')
+        cloud_output = utils.get_cloud_output_from_cdev_name(
+            component_name, table_resource_name
+        )
+        table_cloud_name = cloud_output.get("table_name")
 
         dynamo = boto3.resource("dynamodb")
         table = dynamo.Table(table_cloud_name)
 
         # get the table keys
         tableKeyNames = [key.get("AttributeName") for key in table.key_schema]
```

### Comparing `cdev-0.0.8/core/default/commands/table/put_items.py` & `cdev-0.0.9/core/default/commands/table/put_items.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,113 +1,110 @@
 from argparse import ArgumentParser
 import json
 import os
-from tempfile import TemporaryFile
-from typing import Dict, List
 
 from core.constructs.commands import BaseCommand, OutputWrapper
 from core.default.resources.simple.table import Table, simple_table_model
-from core.utils.paths import get_full_path_from_workspace_base
 
 from core.default.mappers import aws_client
 
 
-from . import utils 
+from . import utils
 
 
 RUUID = "cdev::simple::table"
 
 
 class put_object(BaseCommand):
-    def add_arguments(self, parser: ArgumentParser):
+
+    def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument(
             "resource_name", type=str, help="The resource you want to sync data to"
         )
         parser.add_argument(
             "--file", type=str, help="The location of the json file containing data"
         )
         parser.add_argument(
             "--data", type=str, help="The json data you want to put in the db"
         )
 
-    def command(self, *args, **kwargs):
-        full_resource_name = kwargs.get("resource_name")
-        component_name = full_resource_name.split('.')[0]
-        table_resource_name = full_resource_name.split('.')[1]
+    def command(self, *args, **kwargs) -> None:
+
+        component_name, table_resource_name = self.get_component_and_resource_from_qualified_name(kwargs.get("resource_name"))
 
-        cloud_output = utils.get_cloud_output_from_cdev_name(component_name, table_resource_name)
-        resource: simple_table_model = utils.get_resource_from_cdev_name(component_name, table_resource_name)
+        cloud_output = utils.get_cloud_output_from_cdev_name(
+            component_name, table_resource_name
+        )
+        resource: simple_table_model = utils.get_resource_from_cdev_name(
+            component_name, table_resource_name
+        )
 
-        table_cloud_name = cloud_output.get('table_name')
+        table_cloud_name = cloud_output.get("table_name")
 
         data_string = kwargs.get("data")
         data_file = kwargs.get("file")
 
         if data_string and data_file:
             raise Exception(f"Can not provide both --data and --file arguments")
 
         if not (data_string or data_file):
             raise Exception(f"Must provide either --data or --file arguments")
 
-
-
         if data_string:
             try:
                 data = json.loads(data_string)
-                    
+
             except Exception as e:
                 self.stderr.write("Data provided was not a valid json string")
                 return
 
-
         if data_file:
             if not os.path.isfile(data_file):
                 raise Exception(f"{data_file} is not a valid data file")
 
             try:
                 with open(data_file) as fp:
                     data = json.load(fp)
-            
+
             except Exception as e:
                 print(e)
                 raise e
 
-
-            if not 'items' in data:
-                raise Exception(f"Loaded data from {data_file} does not contain the 'items' key")
-
+            if not "items" in data:
+                raise Exception(
+                    f"Loaded data from {data_file} does not contain the 'items' key"
+                )
 
         attributes_dict = {
-            x.get("attribute_name"): x.get("attribute_type") for x in resource.attributes
+            x.get("attribute_name"): x.get("attribute_type")
+            for x in resource.attributes
         }
 
-
-        for datum in data.get('items'):
-            is_data_valid, msg = utils.validate_data(datum, attributes_dict, resource.keys)
+        for datum in data.get("items"):
+            is_data_valid, msg = utils.validate_data(
+                datum, attributes_dict, resource.keys
+            )
 
             if not is_data_valid:
                 self.stderr.write(msg)
                 return
 
         try:
-            
-            translated_data = [utils.recursive_translate_data(x) for x in data.get('items')]
+
+            translated_data = [
+                utils.recursive_translate_data(x) for x in data.get("items")
+            ]
         except:
             self.stderr.write("Could not translate data to dynamodb put item form")
 
         try:
             for datum in translated_data:
                 aws_client.run_client_function(
                     "dynamodb",
                     "put_item",
-                    {
-                        "TableName": table_cloud_name, 
-                        "Item": datum
-                    },
+                    {"TableName": table_cloud_name, "Item": datum},
                 )
 
                 self.stdout.write(f"Wrote {datum} to {table_resource_name}")
         except Exception as e:
             self.stderr.write(f"Could not write data to table {table_resource_name}")
             return
-
-
```

### Comparing `cdev-0.0.8/core/default/commands/table/utils.py` & `cdev-0.0.9/core/default/commands/table/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,52 @@
-from typing import Dict, List
+from typing import Dict, List, Optional
 
 from core.constructs.resource import ResourceModel
 from core.constructs.workspace import Workspace
 
 RUUID = "cdev::simple::table"
 
-def get_cloud_output_from_cdev_name(component_name: str, cdev_name: str) -> str:
+
+def get_cloud_output_from_cdev_name(component_name: str, cdev_name: str) -> Optional[Dict]:
     try:
         ws = Workspace.instance()
 
-
         cloud_output = ws.get_backend().get_cloud_output_by_name(
-            ws.get_resource_state_uuid(),
-            component_name,
-            RUUID, 
-            cdev_name
+            ws.get_resource_state_uuid(), component_name, RUUID, cdev_name
         )
 
         return cloud_output
     except Exception as e:
         print(f"Could not find resource {component_name}:{RUUID}:{cdev_name}")
         print(e)
         return None
 
 
-
-def get_resource_from_cdev_name(component_name: str, cdev_name: str) -> ResourceModel:
+def get_resource_from_cdev_name(component_name: str, cdev_name: str) -> Optional[ResourceModel]:
     try:
         ws = Workspace.instance()
 
-
         resource = ws.get_backend().get_resource_by_name(
-            ws.get_resource_state_uuid(),
-            component_name,
-            RUUID, 
-            cdev_name
+            ws.get_resource_state_uuid(), component_name, RUUID, cdev_name
         )
 
         return resource
     except Exception as e:
         print(f"Could not find resource {component_name}:{RUUID}:{cdev_name}")
         print(e)
         return None
 
 
-
-
 _attribute_types_to_python_type = {"S": [str], "N": [int, float], "B": [bytes]}
 
 
-def validate_data(data: Dict, attributes: Dict, keys: List[Dict]) -> bool:
+def validate_data(data: Dict, attributes: Dict, keys: List[Dict]) -> Tuple[bool, str]:
     for key in keys:
         if not key.get("attribute_name") in data:
-            return (False, f"Table key {key.get('attribute_name')} not in data")
+            return False, f"Table key {key.get('attribute_name')} not in data"
 
         valid_types = _attribute_types_to_python_type.get(
             attributes.get(key.get("attribute_name"))
         )
 
         is_val_valid_type = False
         for attribute_type in valid_types:
@@ -66,15 +56,15 @@
 
         if not is_val_valid_type:
             return (
                 False,
                 f"Table key {key.get('attribute_name')} ({valid_types}) not correct type in data ({type(data.get(key.get('attribute_name')))})",
             )
 
-    return (True, "")
+    return True, ""
 
 
 def recursive_translate_data(value) -> Dict:
     if isinstance(value, str):
         transformed_val = {"S": value}
     elif isinstance(value, (int, float)):
         transformed_val = {"N": value}
```

### Comparing `cdev-0.0.8/core/default/components.py` & `cdev-0.0.9/core/default/components.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from core.utils.exceptions import Cdev_Error, Cdev_Warning
 from core.utils.fs_manager import finder
 
 
 from core.constructs.components import ComponentModel, Component
 from core.utils import hasher
 
 
@@ -15,25 +14,24 @@
     """
 
     def __init__(self, fp, name):
         super().__init__(name)
         self.fp = fp
 
     def render(self) -> ComponentModel:
+        """Render this component based on the information in the files at the provided folder path
+
+        Returns:
+            ComponentModel
         """
-        Render this component based on the information in the files at the provided folder path
-        """
-        resources_sorted, references_sorted = finder.parse_folder(
-            self.fp
-        )
+        resources_sorted, references_sorted = finder.parse_folder(self.fp)
         total_component_hash = hasher.hash_list(
             [x.hash for x in resources_sorted] + [x.hash for x in references_sorted]
         )
 
-        
         rv = ComponentModel(
             **{
                 "resources": list(resources_sorted),
                 "hash": total_component_hash,
                 "name": self.get_name(),
             }
         )
```

### Comparing `cdev-0.0.8/core/default/mappers/aws_client.py` & `cdev-0.0.9/core/default/mappers/aws_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,113 +1,94 @@
 from time import sleep
-from typing import Callable, List
+from typing import Callable, List, Optional, Any
 import boto3
 
-AVAILABLE_SERVICES = set(["lambda", "s3", "dynamodb", "iam", "apigatewayv2", "sqs", "apigateway"])
+AVAILABLE_SERVICES = {"lambda", "s3", "dynamodb", "iam", "apigatewayv2", "sqs", "apigateway"}
 
 
-
-def _get_boto_client(service_name, credentials=None, profile_name=None):
+def _get_boto_client(service_name, credentials=None, profile_name=None) -> boto3.session.Session:
 
     # TODO readd this check after development is finished and we have the full list of services
-    #if not service_name in AVAILABLE_SERVICES:
+    # if not service_name in AVAILABLE_SERVICES:
     #    return None
-
-    if not credentials or not profile_name:
-        return boto3.client(service_name)
-
     if credentials:
-        return boto3.Session(
+        session = boto3.Session(
             aws_access_key_id=credentials.get("access_key"),
-            aws_secret_access_key=credentials.get("secret_key")
-        ).client(service_name)
+            aws_secret_access_key=credentials.get("secret_key"),
+        )
+    elif profile_name:
+        session = boto3.Session(profile_name=profile_name)
+    else:
+        session = boto3
 
-    if profile_name:
-        return boto3.Session(
-            profile_name=profile_name
-        ).client(service_name)
+    return session.client(service_name)
 
 
-def get_boto_client(service_name):
+def get_boto_client(service_name) -> boto3.session.Session:
     # TODO: Come back and make this settable from the workspace settings
-    #if not cdev_settings.SETTINGS.get("CREDENTIALS"):
+    # if not cdev_settings.SETTINGS.get("CREDENTIALS"):
     return _get_boto_client(service_name)
 
 
-
-def monitor_status(func: Callable, params: dict, previous_val, lookup_func: Callable) -> dict: 
+def monitor_status(
+    func: Callable, params: dict, previous_val, lookup_func: Callable
+) -> dict:
     """
     This function is used to monitor the status of resources as they are created by aws. Alot of resources are created
     asynchronously by aws, which means the original create call returns before the actual resource is created. Therefor,
-    we use this function to handle repeatedly calling a status function to check if the resource was created.   
+    we use this function to handle repeatedly calling a status function to check if the resource was created.
     """
 
     MAX_RESOURCE_TIME = 600
     HEARTBEAT_PACE = 10
 
-    loops = int(MAX_RESOURCE_TIME/HEARTBEAT_PACE)
+    loops = int(MAX_RESOURCE_TIME / HEARTBEAT_PACE)
 
     for _ in range(loops):
         rv = func(**params)
 
         if rv.get("ResponseMetadata").get("HTTPStatusCode") == 200:
             new_value = lookup_func(rv)
-            
+
             if not new_value == previous_val:
                 return rv
-        
-        sleep(HEARTBEAT_PACE)       
 
+        sleep(HEARTBEAT_PACE)
 
     return None
 
 
-def run_client_function(service: str, function_name: str, args: dict, wait: dict = None):
-    args_as_string = f"({service}, {function_name}, {args}, {wait})"
-    
+def run_client_function(
+    service: str, function_name: str, args: dict, wait: dict = None
+) -> Any:
     rendered_client = _get_boto_client(service)
     method = getattr(rendered_client, function_name)
 
     if method:
         rv = method(**args)
-        
+
     if wait:
         waiter = rendered_client.get_waiter(wait.get("name"))
-        final_args = {
-            "WaiterConfig":
-                {
-                    'Delay': 10,
-                    'MaxAttempts': 60
-                }
-        }
-        final_args.update( wait.get("args") )
-        
-        
+        final_args = {"WaiterConfig": {"Delay": 10, "MaxAttempts": 60}}
+        final_args.update(wait.get("args"))
+
         waiter.wait(**final_args)
-        
 
     return rv
 
 
-def aws_resource_wait(service: str, wait: dict):
+def aws_resource_wait(service: str, wait: dict) -> None:
     rendered_client = _get_boto_client(service)
     waiter = rendered_client.get_waiter(wait.get("name"))
-    final_args = {
-        "WaiterConfig":
-            {
-                'Delay': 10,
-                'MaxAttempts': 60
-            }
-    }
-    final_args.update( wait.get("args") )
-    
-    
+    final_args = {"WaiterConfig": {"Delay": 10, "MaxAttempts": 60}}
+    final_args.update(wait.get("args"))
+
     waiter.wait(**final_args)
-    
+
 
 def get_aws_region() -> str:
-    return get_boto_client('s3').meta.region_name
+    return get_boto_client("s3").meta.region_name
 
 
 def get_account_number() -> str:
-    caller_info_rv =  run_client_function("sts", "get_caller_identity", {})
-    return caller_info_rv.get('Account')
+    caller_info_rv = run_client_function("sts", "get_caller_identity", {})
+    return caller_info_rv.get("Account")
```

### Comparing `cdev-0.0.8/core/default/mappers/simple/api_deployer.py` & `cdev-0.0.9/core/default/mappers/simple/api_deployer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from typing import Any, Dict, FrozenSet, List, Tuple
+from typing import Any, Dict, FrozenSet, List, Tuple, Optional
 from uuid import uuid4
 from core.constructs.models import frozendict
 
 from core.constructs.resource import Resource_Difference, Resource_Change_Type
 from core.constructs.output_manager import OutputTask
 from core.default.resources.simple import api as simple_api
 
-from .. import aws_client 
+from .. import aws_client
 
 
 class NoAuthorizerIdFoundError(Exception):
     pass
 
 
 def _create_simple_api(
-        transaction_token: str, 
-        namespace_token: str, 
-        resource: simple_api.simple_api_model, 
-        output_task: OutputTask
-    ) -> Dict:
+    transaction_token: str,
+    namespace_token: str,
+    resource: simple_api.simple_api_model,
+    output_task: OutputTask,
+) -> Dict:
     """
     Create an API on AWS.
 
     Args:
         transaction_token (str): Transaction token to use to identify this action over a resource.
         namespace_token (str): Token used to make sure that resources are created properly in AWS.
         resource (simple_api.simple_api_model): The information about what should be deployed.
@@ -30,15 +30,15 @@
 
     Raises:
         e: [description]
 
     Returns:
         Dict: Information from the cloud about the resource.
     """
-    
+
     base_args = {
         "Name": f"cdev-api-{namespace_token}-{str(uuid4())}",
         "ProtocolType": "HTTP",
     }
 
     cors_args = {
         "CorsConfiguration": {
@@ -54,93 +54,92 @@
             ],
         }
     }
 
     if resource.allow_cors:
         base_args.update(cors_args)
 
-    output_task.update(advance=1, comment='Creating Api')
+    output_task.update(advance=1, comment="Creating Api")
 
     try:
         rv = aws_client.run_client_function("apigatewayv2", "create_api", base_args)
     except Exception as e:
         output_task.print_error(e)
-        raise e 
+        raise e
 
     api_id = rv.get("ApiId")
 
     info = {
         "cloud_id": api_id,
         "endpoints": {},
     }
 
-    
     if resource.authorizers:
         _authorizer_outputs: Dict[str, Dict] = {}
-        
+
         for authorizer in resource.authorizers:
-            output_task.update(advance=1, comment=f'Creating Authorizer {authorizer.name}')
+            output_task.update(
+                advance=1, comment=f"Creating Authorizer {authorizer.name}"
+            )
             authorizer_id = _create_authorizer(api_id, authorizer)
             _authorizer_outputs[authorizer_id] = authorizer.dict()
 
-        info['authorizers'] = _authorizer_outputs
-        
-    
+        info["authorizers"] = _authorizer_outputs
 
     _stage_args = {
         "ApiId": info.get("cloud_id"),
         "AutoDeploy": True,
         "StageName": "live",
     }
-    
-    output_task.update(advance=1, comment='Creating Stage')
+
+    output_task.update(advance=1, comment="Creating Stage")
     try:
-        rv2 = aws_client.run_client_function('apigatewayv2', 'create_stage', _stage_args)
+        rv2 = aws_client.run_client_function(
+            "apigatewayv2", "create_stage", _stage_args
+        )
     except Exception as e:
         output_task.print_error(e)
-        raise e 
+        raise e
 
     info["endpoint"] = f"{rv.get('ApiEndpoint')}/{rv2.get('StageName')}"
 
-
     api_id = info.get("cloud_id")
     if resource.routes:
         _created_endpoints = {}
         for route in resource.routes:
-            output_task.update(advance=1, comment=f'Creating Route {route.path} [{route.verb}]')
-            
+            output_task.update(
+                advance=1, comment=f"Creating Route {route.path} [{route.verb}]"
+            )
+
             try:
-                authorizer_id = _find_authorization_id(route, info.get('authorizers') )
+                authorizer_id = _find_authorization_id(route, info.get("authorizers"))
 
                 route_cloud_id = _create_route(api_id, route, authorizer_id)
             except Exception as e:
                 output_task.print_error(e)
-                raise e 
-
+                raise e
 
             # Add route to the return info
-            dict_key = f'{route.path} {route.verb}'
+            dict_key = f"{route.path} {route.verb}"
 
             _created_endpoints[dict_key] = route_cloud_id
 
-        
         info["endpoints"] = _created_endpoints
 
-
     return info
 
 
 def _update_simple_api(
-    transaction_token: str, 
+    transaction_token: str,
     namespace_token: str,
     previous_resource: simple_api.simple_api_model,
     new_resource: simple_api.simple_api_model,
     previous_output: frozendict,
-    output_task: OutputTask
-    ) -> Dict:
+    output_task: OutputTask,
+) -> Dict:
     """
     Create an API on AWS.
 
     Args:
         transaction_token (str): Transaction token to use to identify this action over a resource.
         namespace_token (str): Token used to make sure that resources are created properly in AWS.
         previous_resource (simple_api.simple_api_model): The information about the previous API.
@@ -152,254 +151,285 @@
         e: [description]
 
     Returns:
         Dict: Information from the cloud about the resource.
     """
 
     mutable_previous_output = dict(previous_output)
-    previous_cloud_id = mutable_previous_output.get('cloud_id')
+    previous_cloud_id = mutable_previous_output.get("cloud_id")
 
     output_task.print(previous_resource)
 
-    
     # Change the CORS Settings of the API
     if not previous_resource.allow_cors == new_resource.allow_cors:
-        new_cors_policy =  {
-            "AllowOrigins": ["*"],
-            "AllowMethods": ["*"],
-            "AllowHeaders": [
-                "Content-Type",
-                "X-Amz-Date",
-                "Authorization",
-                "X-Api-Key",
-                "X-Amz-Security-Token",
-                "X-Amz-User-Agent",
-            ],
-        } if new_resource.allow_cors else {}
+        new_cors_policy = (
+            {
+                "AllowOrigins": ["*"],
+                "AllowMethods": ["*"],
+                "AllowHeaders": [
+                    "Content-Type",
+                    "X-Amz-Date",
+                    "Authorization",
+                    "X-Api-Key",
+                    "X-Amz-Security-Token",
+                    "X-Amz-User-Agent",
+                ],
+            }
+            if new_resource.allow_cors
+            else {}
+        )
 
-        output_task.update(advance=1, comment=f'Updating CORS Policy')
+        output_task.update(advance=1, comment=f"Updating CORS Policy")
         try:
             aws_client.run_client_function(
-                'apigatewayv2', 
-                'update_api', 
-                {
-                    'api_id': previous_cloud_id,
-                    'CorsConfiguration ': new_cors_policy
-                }
+                "apigatewayv2",
+                "update_api",
+                {"api_id": previous_cloud_id, "CorsConfiguration ": new_cors_policy},
             )
         except Exception as e:
             output_task.print_error(e)
-            raise e 
+            raise e
 
-    # If an authorizer is to be deleted, it must already be removed from any route, but to create a route with an authorizer, you must 
+    # If an authorizer is to be deleted, it must already be removed from any route, but to create a route with an authorizer, you must
     # have already created the authorizer. This means we can NOT do all the operations on the routes before authorizers but also can NOT do all
-    # the authorizers before the routes. 
+    # the authorizers before the routes.
 
-    # We must do them in an order that does not cause errors, so we are only going to perform update operations that must happen before the 
-    # authorizers are updated then defer the rest of the updates till after by storing their info in the `_update_route_info` and `_create_route_info` 
+    # We must do them in an order that does not cause errors, so we are only going to perform update operations that must happen before the
+    # authorizers are updated then defer the rest of the updates till after by storing their info in the `_update_route_info` and `_create_route_info`
     # list.
     _create_route_info: List[simple_api.route_model] = []
     _update_route_info: List[Tuple[str, simple_api.route_model]] = []
-    previous_route_info: Dict[str,str] = dict(mutable_previous_output.get('endpoints')) if mutable_previous_output.get('endpoints') else {}
+    previous_route_info: Dict[str, str] = (
+        dict(mutable_previous_output.get("endpoints"))
+        if mutable_previous_output.get("endpoints")
+        else {}
+    )
     new_output_info = {}
 
     if not previous_resource.routes == new_resource.routes:
-        
+
         update_routes = set()
 
         # Delete any route that is not in the new routes but in previous routes
-        routes_to_be_deleted: FrozenSet[simple_api.route_model] = previous_resource.routes.difference(new_resource.routes)
+        routes_to_be_deleted: FrozenSet[
+            simple_api.route_model
+        ] = previous_resource.routes.difference(new_resource.routes)
         # Create any route that is in the new routes but not in previous routes
-        routes_to_be_created: FrozenSet[simple_api.route_model] = new_resource.routes.difference(previous_resource.routes)
+        routes_to_be_created: FrozenSet[
+            simple_api.route_model
+        ] = new_resource.routes.difference(previous_resource.routes)
 
-        previous_route_ids = set([f"{x.path} {x.verb}" for x in previous_resource.routes])
+        previous_route_ids = set(
+            [f"{x.path} {x.verb}" for x in previous_resource.routes]
+        )
 
         for route in routes_to_be_created:
-            route_id = (
-                f'{route.path} {route.verb}'
-            )
+            route_id = f"{route.path} {route.verb}"
 
             if route_id in previous_route_ids:
                 # This is updating the routes authorization not making a new route
                 # There are a few states that require making an update to the current route before the authorizers are updated.
                 # Updating to a new Authorizer
                 #      - Previous Authorizer was none -> No update needed
-                #      - Previous Authorizer existed -> remove the authorizer from the route 
+                #      - Previous Authorizer existed -> remove the authorizer from the route
 
                 update_routes.add(route_id)
 
                 route_cloud_id = previous_route_info.get(route_id)
 
-                if not mutable_previous_output.get('authorizers'):
-                    # No previous authorization info means all route updates should wait til authorizations 
+                if not mutable_previous_output.get("authorizers"):
+                    # No previous authorization info means all route updates should wait til authorizations
                     # have completed
                     _update_route_info.append((route_cloud_id, route))
                     continue
 
                 # guranteed to have an element because the invariant of the if statement
-                previous_route = [x for x in previous_resource.routes if f"{x.path} {x.verb}" == route_id][0]
+                previous_route = [
+                    x
+                    for x in previous_resource.routes
+                    if f"{x.path} {x.verb}" == route_id
+                ][0]
 
                 # Find the previous id... we have to pass in the previous api since that was used in the previous computation regarding
                 # the default authorizer
                 try:
-                    previous_authorizer_id = _find_authorization_id(previous_route, mutable_previous_output.get('authorizers') )
+                    previous_authorizer_id = _find_authorization_id(
+                        previous_route, mutable_previous_output.get("authorizers")
+                    )
                 except NoAuthorizerIdFoundError as e:
                     # If a previous authorizer was to be found and it wasn't then there is something wrong since we should have all the info on previous
                     # authorizers
                     raise e
-                
+
                 if previous_authorizer_id:
                     # remove the previous authorizer, but defer the updating to the new one until after authorizers have finished
-                    print(f'soft update {route}')
+                    print(f"soft update {route}")
                     _update_route(previous_cloud_id, route_cloud_id, route, None)
                     _update_route_info.append((route_cloud_id, route))
 
                 else:
-                    # 1A 
+                    # 1A
                     # No previous authorizer so wait til after to complete the authorization
                     _update_route_info.append((route_cloud_id, route))
 
             else:
                 # All creates should just happen after the authorizers have been made
                 _create_route_info.append(route)
-                    
-    
+
         for route in routes_to_be_deleted:
             # All deletes should go ahead and occur now
-            route_id = (
-                f'{route.path} {route.verb}'
-            )
+            route_id = f"{route.path} {route.verb}"
 
             if route_id in update_routes:
                 continue
 
-            output_task.update(advance=1, comment=f'Deleting Route {route.path} [{route.verb}]')
+            output_task.update(
+                advance=1, comment=f"Deleting Route {route.path} [{route.verb}]"
+            )
             try:
-                _delete_route(
-                    previous_cloud_id, previous_route_info.get(route_id)
-                )
+                _delete_route(previous_cloud_id, previous_route_info.get(route_id))
             except Exception as e:
                 output_task.print_error(e)
-                raise e 
+                raise e
 
             previous_route_info.pop(route_id)
 
     if not previous_resource.authorizers == new_resource.authorizers:
         # Three options for types of changes to authorizers
-        # 1. Complete New 
+        # 1. Complete New
         # 2. Complete Remove
-        # 3. Update: This will show up as a delete and create when doing the set difference, so when going through the creates we 
-        #    should look through the past authorizers to find one with the same name. 
+        # 3. Update: This will show up as a delete and create when doing the set difference, so when going through the creates we
+        #    should look through the past authorizers to find one with the same name.
         new_authorizer_info = {}
-        previous_authorizers_info = dict(mutable_previous_output.get('authorizers')) if mutable_previous_output.get('authorizers') else {}
+        previous_authorizers_info = (
+            dict(mutable_previous_output.get("authorizers"))
+            if mutable_previous_output.get("authorizers")
+            else {}
+        )
         updated = set()
 
-
-
-        authorizers_to_delete: FrozenSet[simple_api.authorizer_model] = previous_resource.authorizers.difference(new_resource.authorizers)
-        authorizers_to_create: FrozenSet[simple_api.authorizer_model] = new_resource.authorizers.difference(previous_resource.authorizers)
+        authorizers_to_delete: FrozenSet[
+            simple_api.authorizer_model
+        ] = previous_resource.authorizers.difference(new_resource.authorizers)
+        authorizers_to_create: FrozenSet[
+            simple_api.authorizer_model
+        ] = new_resource.authorizers.difference(previous_resource.authorizers)
 
         for authorizer in authorizers_to_create:
             if any(x.name == authorizer.name for x in authorizers_to_delete):
-                #update not hard create
-                output_task.update(advance=1, comment=f'Updating Authorizer {authorizer.name}')
-                
-                authorizer_id = [id for id, v in previous_authorizers_info.items() if v.get("name") == authorizer.name][0]
-                _update_authorizer(previous_output.get('cloud_id'), authorizer_id, authorizer)
+                # update not hard create
+                output_task.update(
+                    advance=1, comment=f"Updating Authorizer {authorizer.name}"
+                )
+
+                authorizer_id = [
+                    id
+                    for id, v in previous_authorizers_info.items()
+                    if v.get("name") == authorizer.name
+                ][0]
+                _update_authorizer(
+                    previous_output.get("cloud_id"), authorizer_id, authorizer
+                )
 
                 # Add this to updated authorizers so that it does not delete the authorizer in next steps
                 updated.add(authorizer.name)
                 # In the previous output, update the authorization info
                 new_authorizer_info[authorizer_id] = authorizer.dict()
 
             else:
-                output_task.update(advance=1, comment=f'Creating Authorizer {authorizer.name}')
-                authorizer_id = _create_authorizer(previous_output.get('cloud_id'), authorizer)
+                output_task.update(
+                    advance=1, comment=f"Creating Authorizer {authorizer.name}"
+                )
+                authorizer_id = _create_authorizer(
+                    previous_output.get("cloud_id"), authorizer
+                )
                 new_authorizer_info[authorizer_id] = authorizer.dict()
 
-        
-
         for authorizer in authorizers_to_delete:
             if authorizer.name in updated:
                 continue
 
-            authorizer_id = [id for id, v in previous_authorizers_info.items() if v.get("name") == authorizer.name][0]
-            output_task.update(advance=1, comment=f'Deleteing Authorizer {authorizer.name}')
-            _delete_authorizer(previous_output.get('cloud_id'), authorizer_id)
+            authorizer_id = [
+                id
+                for id, v in previous_authorizers_info.items()
+                if v.get("name") == authorizer.name
+            ][0]
+            output_task.update(
+                advance=1, comment=f"Deleteing Authorizer {authorizer.name}"
+            )
+            _delete_authorizer(previous_output.get("cloud_id"), authorizer_id)
 
             previous_authorizers_info.pop(authorizer_id)
 
-
         previous_authorizers_info.update(new_authorizer_info)
-        mutable_previous_output['authorizers'] = previous_authorizers_info
+        mutable_previous_output["authorizers"] = previous_authorizers_info
 
-
-    
     for route in _create_route_info:
         # Now that all updates to the authorizers have completed, we can do the create routes
-        route_id = (
-            f'{route.path} {route.verb}'
-        )
+        route_id = f"{route.path} {route.verb}"
 
-        # Find the authorizer id 
-        authorizer_id = _find_authorization_id(route, mutable_previous_output.get('authorizers') )
+        # Find the authorizer id
+        authorizer_id = _find_authorization_id(
+            route, mutable_previous_output.get("authorizers")
+        )
 
-        output_task.update(advance=1, comment=f'Creating Route {route.path} [{route.verb}]')
+        output_task.update(
+            advance=1, comment=f"Creating Route {route.path} [{route.verb}]"
+        )
 
         route_cloud_id = _create_route(previous_cloud_id, route, authorizer_id)
-        
-        new_output_info[route_id] = route_cloud_id
 
+        new_output_info[route_id] = route_cloud_id
 
     for id, route in _update_route_info:
         # Now that all updates to the authorizers have completed, we can do the update routes that depends on the created
         # authorization
-        route_id = (
-            f'{route.path} {route.verb}'
-        )
+        route_id = f"{route.path} {route.verb}"
 
-        # Find the authorizer id 
-        authorizer_id = _find_authorization_id(route, mutable_previous_output.get('authorizers'))
+        # Find the authorizer id
+        authorizer_id = _find_authorization_id(
+            route, mutable_previous_output.get("authorizers")
+        )
 
-        output_task.update(advance=1, comment=f'Updating Route {route.path} [{route.verb}]')
+        output_task.update(
+            advance=1, comment=f"Updating Route {route.path} [{route.verb}]"
+        )
 
         _update_route(previous_cloud_id, id, route, authorizer_id)
 
     previous_route_info.update(new_output_info)
-    mutable_previous_output['endpoints'] = previous_route_info
+    mutable_previous_output["endpoints"] = previous_route_info
 
     return mutable_previous_output
 
 
 def _remove_simple_api(
-    transaction_token: str,  
-    previous_output: Dict, 
-    output_task: OutputTask
-    ):
+    transaction_token: str, previous_output: Dict, output_task: OutputTask
+) -> None:
     """
     Delete an API from AWS.
 
     Args:
         transaction_token (str): Transaction token to use to identify this action over a resource.
         previous_output (Dict): Cloud output of the resource. Used to determine what API to delete on AWS.
         output_task (OutputTask): Output Task to send any progress information.
 
     Raises:
         e: [description]
     """
 
     api_id = previous_output.get("cloud_id")
 
-    output_task.update(advance=1, comment=f'Deleting API')
+    output_task.update(advance=1, comment=f"Deleting API")
 
     try:
         aws_client.run_client_function("apigatewayv2", "delete_api", {"ApiId": api_id})
     except Exception as e:
         output_task.print_error(e)
-        raise e 
+        raise e
 
 
 def _create_authorizer(api_id: str, authorizer: simple_api.authorizer_model) -> str:
     """Helper function for creating new authorizers
 
     Args:
         api_id (str): Api ID of the api in AWS.
@@ -407,60 +437,60 @@
 
     Returns:
         str: Authorizer Id of the created Authorizer
     """
     args = {
         "ApiId": api_id,
         "Name": authorizer.name,
-        "AuthorizerType": 'JWT',
-        "IdentitySource":[
-            '$request.header.Authorization',
+        "AuthorizerType": "JWT",
+        "IdentitySource": [
+            "$request.header.Authorization",
         ],
         "JwtConfiguration": {
-            'Audience': [
+            "Audience": [
                 authorizer.audience,
             ],
-            "Issuer": authorizer.issuer_url
-        }
+            "Issuer": authorizer.issuer_url,
+        },
     }
 
-    rv = aws_client.run_client_function('apigatewayv2', 'create_authorizer', args)
+    rv = aws_client.run_client_function("apigatewayv2", "create_authorizer", args)
 
     return rv.get("AuthorizerId")
 
 
-def _update_authorizer(api_id: str, authorizer_id: str, authorizer: simple_api.authorizer_model):
+def _update_authorizer(
+    api_id: str, authorizer_id: str, authorizer: simple_api.authorizer_model
+):
     args = {
         "ApiId": api_id,
         "AuthorizerId": authorizer_id,
         "JwtConfiguration": {
-            'Audience': [
+            "Audience": [
                 authorizer.audience,
             ],
-            "Issuer": authorizer.issuer_url
-        }
+            "Issuer": authorizer.issuer_url,
+        },
     }
 
-    aws_client.run_client_function('apigatewayv2', 'update_authorizer', args)
+    aws_client.run_client_function("apigatewayv2", "update_authorizer", args)
 
 
-def _delete_authorizer(api_id: str, authorizer_id: str):
-    args = {
-        "ApiId": api_id,
-        "AuthorizerId": authorizer_id
-    }
-    aws_client.run_client_function('apigatewayv2', 'delete_authorizer', args)
+def _delete_authorizer(api_id: str, authorizer_id: str) -> None:
+    args = {"ApiId": api_id, "AuthorizerId": authorizer_id}
+    aws_client.run_client_function("apigatewayv2", "delete_authorizer", args)
 
 
-
-def _find_authorization_id(route: simple_api.route_model, output_ids: Dict[str, Dict]) -> str:
+def _find_authorization_id(
+    route: simple_api.route_model, output_ids: Dict[str, Dict]
+) -> Optional[str]:
     """Function for finding a route's authorizer cloud id
 
     This function takes into account that a route will by default use the api's default authorizer unless the route has the `override_authorizer_name`
-    set. Will return None if the route will not have an authorizer or there is not enough information to find the authorizer. 
+    set. Will return None if the route will not have an authorizer or there is not enough information to find the authorizer.
 
     Args:
         api_resource (simple_api.simple_api_model): _description_
         route (simple_api.route_model): _description_
         output_ids (Dict[str, Dict]): _description_
 
     Raises:
@@ -473,31 +503,31 @@
 
     if not route.authorizer_name:
         return None
 
     if not output_ids:
         return None
 
-    
-    found_id = [id for id, x in output_ids.items() if x.get("name") == route.authorizer_name]
-
+    found_id = [
+        id for id, x in output_ids.items() if x.get("name") == route.authorizer_name
+    ]
 
     if len(found_id) == 0 and route.authorizer_name:
         # We have an authorizer but can not find the info for it
         raise NoAuthorizerIdFoundError
 
     if len(found_id) > 1:
         raise Exception
 
     return found_id[0]
 
-    
 
-
-def _create_route(api_id: str, route: simple_api.route_model, authorizer_id: str=None) -> str:
+def _create_route(
+    api_id: str, route: simple_api.route_model, authorizer_id: str = None
+) -> str:
     """
     Helper Function for creating routes on an API. Note that any error raised by the aws client will not be caught by this function and should
     be handled by the caller of this function.
 
     Args:
         api_id (str): Api ID of the api in AWS.
         route (simple_api.route_event_model): Information about the route to create.
@@ -511,95 +541,87 @@
 
     _route_args = {
         "ApiId": api_id,
         "RouteKey": f"{route.verb} {route.path}",
     }
 
     if authorizer_id:
-        _authorizer_args['AuthorizerId'] = authorizer_id
-        _authorizer_args['AuthorizationType'] = 'JWT'
-        
+        _authorizer_args["AuthorizerId"] = authorizer_id
+        _authorizer_args["AuthorizationType"] = "JWT"
+
         if route.additional_scopes:
-            _authorizer_args['AuthorizationScopes'] = list(route.additional_scopes)
-    
+            _authorizer_args["AuthorizationScopes"] = list(route.additional_scopes)
 
     full_args.update(_route_args)
     full_args.update(_authorizer_args)
-    rv = aws_client.run_client_function('apigatewayv2', 'create_route', full_args)
+    rv = aws_client.run_client_function("apigatewayv2", "create_route", full_args)
 
     return rv.get("RouteId")
 
 
-def _delete_route(api_id: str, route_id: str):
+def _delete_route(api_id: str, route_id: str) -> None:
     """
     Helper Function for deleting routes on an API. Note that any error raised by the aws client will not be caught by this function and should
     be handled by the caller of this function.
 
     Args:
         api_id (str): Api ID of the api in AWS.
         route_id (lambda_event): Route ID of the route in AWS.
     """
 
     aws_client.run_client_function(
         "apigatewayv2", "delete_route", {"ApiId": api_id, "RouteId": route_id}
     )
 
 
-def _update_route(api_id: str, route_id: str, route: simple_api.route_model, authorizer_id: str=None):
+def _update_route(
+    api_id: str, route_id: str, route: simple_api.route_model, authorizer_id: str = None
+):
 
     args = {
         "ApiId": api_id,
         "RouteId": route_id,
     }
 
     if authorizer_id:
-        args['AuthorizerId'] = authorizer_id
-        args['AuthorizationType'] = 'JWT'
+        args["AuthorizerId"] = authorizer_id
+        args["AuthorizationType"] = "JWT"
 
         if route.additional_scopes:
-            args['AuthorizationScopes'] = list(route.additional_scopes)
+            args["AuthorizationScopes"] = list(route.additional_scopes)
 
     else:
-        args['AuthorizerId'] = ""
-        args['AuthorizationType'] = "NONE"
-        args['AuthorizationScopes'] = []
+        args["AuthorizerId"] = ""
+        args["AuthorizationType"] = "NONE"
+        args["AuthorizationScopes"] = []
 
-    aws_client.run_client_function('apigatewayv2', 'update_route', args)
-    
+    aws_client.run_client_function("apigatewayv2", "update_route", args)
 
 
 def handle_simple_api_deployment(
-        transaction_token: str, 
-        namespace_token: str, 
-        resource_diff: Resource_Difference, 
-        previous_output: Dict[str, Any],
-        output_task: OutputTask
-        ) -> Dict:
-    
+    transaction_token: str,
+    namespace_token: str,
+    resource_diff: Resource_Difference,
+    previous_output: Dict[str, Any],
+    output_task: OutputTask,
+) -> Dict:
+
     if resource_diff.action_type == Resource_Change_Type.CREATE:
         return _create_simple_api(
-            transaction_token,
-            namespace_token,
-            resource_diff.new_resource,
-            output_task
+            transaction_token, namespace_token, resource_diff.new_resource, output_task
         )
 
     elif resource_diff.action_type == Resource_Change_Type.UPDATE_IDENTITY:
         return _update_simple_api(
             transaction_token,
             namespace_token,
             simple_api.simple_api_model(**resource_diff.previous_resource.dict()),
             resource_diff.new_resource,
             previous_output,
-            output_task
+            output_task,
         )
-        
+
     elif resource_diff.action_type == Resource_Change_Type.DELETE:
 
-        _remove_simple_api(
-            transaction_token,
-            previous_output,
-            output_task
-        )
+        _remove_simple_api(transaction_token, previous_output, output_task)
 
         return {}
-
```

### Comparing `cdev-0.0.8/core/default/mappers/simple/bucket_deployer.py` & `cdev-0.0.9/core/default/mappers/simple/bucket_deployer.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,85 +3,113 @@
 from uuid import uuid4
 
 from core.constructs.resource import Resource_Difference, Resource_Change_Type
 from core.default.resources.simple import object_store as simple_object_store
 from core.constructs.output_manager import OutputTask
 from core.utils import hasher
 
-
 from .. import aws_client as raw_aws_client
 
-
 RUUID = "cdev::simple::bucket"
 
 
 class event_hander_types(Enum):
     SQS = "sqs"
     LAMBDA = "lambda"
     SNS = "sns"
 
 
 def _create_simple_bucket(
-    transaction_token: str, 
-    namespace_token: str, 
-    resource:  simple_object_store.bucket_model,
-    output_task: OutputTask
+    transaction_token: str,
+    namespace_token: str,
+    resource: simple_object_store.bucket_model,
+    output_task: OutputTask,
 ) -> Dict:
-
     full_namespace_suffix = hasher.hash_list([namespace_token, str(uuid4())])
 
     cloud_bucket_name = f"cdev-bucket-{full_namespace_suffix}"
 
-    output_task.update(comment=f'Creating Bucket {cloud_bucket_name}')
-    
+    output_task.update(comment=f"Creating Bucket {cloud_bucket_name}")
+
     # TODO create buckets in different region
     rv = raw_aws_client.run_client_function(
         "s3", "create_bucket", {"Bucket": cloud_bucket_name}
     )
 
-    output_task.update(comment=f'Created Bucket {cloud_bucket_name}')
+    output_task.update(comment=f"Created Bucket {cloud_bucket_name}")
 
     output_info = {
         "bucket_name": cloud_bucket_name,
         "cloud_id": f"arn:aws:s3:::{cloud_bucket_name}",
         "arn": f"arn:aws:s3:::{cloud_bucket_name}",
     }
 
-
     return output_info
 
 
 def _update_simple_bucket(
-    transaction_token: str, 
+    transaction_token: str,
     namespace_token: str,
     previous_resource: simple_object_store.bucket_model,
     new_resource: simple_object_store.bucket_model,
     previous_output: Dict,
-    output_task: OutputTask
+    output_task: OutputTask,
 ) -> Dict:
-
-    _remove_simple_bucket(transaction_token,  previous_output, output_task)
-    new_info =  _create_simple_bucket(transaction_token, namespace_token, new_resource, output_task)
+    _remove_simple_bucket(transaction_token, previous_output, output_task)
+    new_info = _create_simple_bucket(
+        transaction_token, namespace_token, new_resource, output_task
+    )
 
     return new_info
 
 
 def _remove_simple_bucket(
-    transaction_token: str,  previous_output: Dict, output_task: OutputTask
-):
+    transaction_token: str, previous_output: Dict, output_task: OutputTask
+) -> None:
+    previous_bucket_name = previous_output.get("bucket_name")
+
+    files = _get_bucket_files(previous_bucket_name)
+    if files:
+        total_files = len(files)
+        i = 1
+        for file in files:
+            output_task.update(
+                advance=1,
+                comment=f"Deleting File {i} from {total_files} from bucket {previous_bucket_name}",
+            )
+            _delete_simple_s3_file(previous_bucket_name, file["Key"])
+            i += 1
 
-    previous_bucket_name = previous_output.get('bucket_name')
+    output_task.update(advance=1, comment=f"Deleting Bucket {previous_bucket_name}")
 
-    output_task.update(advance=1, comment=f'Deleting Bucket {previous_bucket_name}')
+    _delete_empy_bucket(previous_bucket_name)
 
+    output_task.update(advance=1, comment=f"Deleted Bucket {previous_bucket_name}")
+
+
+def _delete_simple_s3_file(bucket_name: str, file_name: str) -> None:
     raw_aws_client.run_client_function(
-        "s3", "delete_bucket", {"Bucket": previous_bucket_name}
+        "s3",
+        "delete_object",
+        {"Bucket": bucket_name, "Key": file_name},
     )
 
-    output_task.update(advance=1, comment=f'Deleted Bucket {previous_bucket_name}')
+
+def _delete_empy_bucket(bucket_name: str) -> None:
+    raw_aws_client.run_client_function("s3", "delete_bucket", {"Bucket": bucket_name})
+
+
+def _get_bucket_files(bucket_name: str) -> List:
+    files = raw_aws_client.run_client_function(
+        "s3", "list_objects_v2", {"Bucket": bucket_name}
+    )
+    if "Contents" in files:
+        return files["Contents"]
+    else:
+        return []
 
 
 def add_eventsource(
     bucket_name: str,
     handler_type: event_hander_types,
     handler_arn: str,
     events: List[str],
@@ -96,15 +124,14 @@
     """
 
     current_events = _get_current_bucket_event_configuration(bucket_name)
 
     if not current_events:
         current_events = {}
 
-
     event_id = hasher.hash_list(
         [handler_type.value, handler_arn, hasher.hash_list(events)]
     )
     base_config = {"Events": events, "Id": event_id}
 
     if handler_type == event_hander_types.LAMBDA:
         base_config.update({"LambdaFunctionArn": handler_arn})
@@ -146,15 +173,14 @@
 
 def remove_eventsource(bucket_name: str, bucket_event_id: str) -> bool:
     current_events = _get_current_bucket_event_configuration(bucket_name)
 
     if not current_events:
         raise Exception
 
-
     keys = [
         "TopicConfigurations",
         "QueueConfigurations",
         "LambdaFunctionConfigurations",
     ]
 
     found_val = False
@@ -192,54 +218,43 @@
         "QueueConfigurations": aws_rv.get("QueueConfigurations"),
         "LambdaFunctionConfigurations": aws_rv.get("LambdaFunctionConfigurations"),
     }
 
     return rv
 
 
-def _deploy_bucket_event_configuration(bucket_name: str, new_config: Dict):
+def _deploy_bucket_event_configuration(bucket_name: str, new_config: Dict) -> None:
     final_config = {k: v for k, v in new_config.items() if v}
 
     raw_aws_client.run_client_function(
         "s3",
         "put_bucket_notification_configuration",
         {"Bucket": bucket_name, "NotificationConfiguration": final_config},
     )
 
 
-
-def handle_simple_bucket_deployment( 
-        transaction_token: str, 
-        namespace_token: str, 
-        resource_diff: Resource_Difference, 
-        previous_output: Dict[str, Any],
-        output_task: OutputTask
-    ) -> Dict:
-    
+def handle_simple_bucket_deployment(
+    transaction_token: str,
+    namespace_token: str,
+    resource_diff: Resource_Difference,
+    previous_output: Dict[str, Any],
+    output_task: OutputTask,
+) -> Dict:
     if resource_diff.action_type == Resource_Change_Type.CREATE:
         return _create_simple_bucket(
-            transaction_token,
-            namespace_token,
-            resource_diff.new_resource,
-            output_task
+            transaction_token, namespace_token, resource_diff.new_resource, output_task
         )
-        
+
     elif resource_diff.action_type == Resource_Change_Type.UPDATE_IDENTITY:
         return _update_simple_bucket(
             transaction_token,
             namespace_token,
             simple_object_store.bucket_model(**resource_diff.previous_resource.dict()),
             resource_diff.new_resource,
             previous_output,
-            output_task
+            output_task,
         )
 
     elif resource_diff.action_type == Resource_Change_Type.DELETE:
-        _remove_simple_bucket(
-            transaction_token,
-            previous_output,
-            output_task
-        )
+        _remove_simple_bucket(transaction_token, previous_output, output_task)
 
         return {}
-
-
```

### Comparing `cdev-0.0.8/core/default/mappers/simple/dynamodb_deployer.py` & `cdev-0.0.9/core/default/mappers/simple/dynamodb_deployer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,52 @@
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 from uuid import uuid4
 
 
 from core.constructs.resource import Resource_Difference, Resource_Change_Type
 from core.constructs.output_manager import OutputTask
 from core.default.resources.simple import table
 from core.utils import hasher
 
-from .. import aws_client 
+from .. import aws_client
+
 
 def _create_simple_dynamodb_table(
-    transaction_token: str, 
-    namespace_token: str, 
-    resource: table.simple_table_model, 
-    output_task: OutputTask
-) -> bool:
+    transaction_token: str,
+    namespace_token: str,
+    resource: table.simple_table_model,
+    output_task: OutputTask,
+) -> Dict:
 
     full_namespace_suffix = hasher.hash_list([namespace_token, str(uuid4())])
     table_name = f"cdev-table-{full_namespace_suffix}"
 
-    output_task.update(comment='[blink]Creating Table. This will take a few seconds.[/blink]')
+    output_task.update(
+        comment="[blink]Creating Table. This will take a few seconds.[/blink]"
+    )
+
+    key_schema = [
+        {"AttributeName": x.attribute_name, "KeyType": x.key_type.value}
+        for x in resource.keys
+    ]
 
-    key_schema = [{
-                "AttributeName": x.attribute_name,
-                "KeyType": x.key_type.value
-            } for x in resource.keys]
+    key_schema.sort(key=lambda x: x.get("KeyType"))
 
-    key_schema.sort(key=lambda x: x.get('KeyType'))
-    
     rv = aws_client.run_client_function(
         "dynamodb",
         "create_table",
         {
             "TableName": table_name,
-            "AttributeDefinitions": [{
-                "AttributeName": x.attribute_name,
-                "AttributeType": x.attribute_type.value
-            } for x in resource.attributes],
+            "AttributeDefinitions": [
+                {
+                    "AttributeName": x.attribute_name,
+                    "AttributeType": x.attribute_type.value,
+                }
+                for x in resource.attributes
+            ],
             "KeySchema": key_schema,
             "BillingMode": "PAY_PER_REQUEST",
         },
         wait={"name": "table_exists", "args": {"TableName": table_name}},
     )
 
     output_info = {
@@ -51,73 +57,61 @@
         "ruuid": resource.ruuid,
     }
 
     return output_info
 
 
 def _update_simple_dynamodb_table(
-    transaction_token: str, 
+    transaction_token: str,
     namespace_token: str,
     previous_resource: table.simple_table_model,
     new_resource: table.simple_table_model,
     previous_output: Dict,
-    output_task: OutputTask
-    ) -> bool:
+    output_task: OutputTask,
+) -> Dict:
     raise Exception
 
 
-
 def _remove_simple_dynamodb_table(
-    transaction_token: str,  
-    previous_output: Dict, 
-    output_task: OutputTask
-    ) -> bool:
+    transaction_token: str, previous_output: Dict, output_task: OutputTask
+) -> None:
 
     table_name = previous_output.get("table_name")
 
-    output_task.update(comment='[blink]Deleting Table. This will take a few seconds.[/blink]')
+    output_task.update(
+        comment="[blink]Deleting Table. This will take a few seconds.[/blink]"
+    )
 
     aws_client.run_client_function(
         "dynamodb",
         "delete_table",
         {
             "TableName": table_name,
         },
         wait={"name": "table_not_exists", "args": {"TableName": table_name}},
     )
 
 
+def handle_simple_table_deployment(
+    transaction_token: str,
+    namespace_token: str,
+    resource_diff: Resource_Difference,
+    previous_output: Dict[str, Any],
+    output_task: OutputTask,
+) -> Optional[Dict]:
 
-def handle_simple_table_deployment(transaction_token: str, 
-        namespace_token: str, 
-        resource_diff: Resource_Difference, 
-        previous_output: Dict[str, Any],
-        output_task: OutputTask
-        ) -> Dict:
-    
     if resource_diff.action_type == Resource_Change_Type.CREATE:
         return _create_simple_dynamodb_table(
-            transaction_token,
-            namespace_token,
-            resource_diff.new_resource,
-            output_task
+            transaction_token, namespace_token, resource_diff.new_resource, output_task
         )
     elif resource_diff.action_type == Resource_Change_Type.UPDATE_IDENTITY:
-
         return _update_simple_dynamodb_table(
             transaction_token,
             namespace_token,
             table.simple_table_model(**resource_diff.previous_resource.dict()),
             resource_diff.new_resource,
             previous_output,
-            output_task
+            output_task,
         )
-        
     elif resource_diff.action_type == Resource_Change_Type.DELETE:
-
-        _remove_simple_dynamodb_table(
-            transaction_token,
-            previous_output,
-            output_task
-        )
-
+        _remove_simple_dynamodb_table(transaction_token, previous_output, output_task)
         return {}
```

### Comparing `cdev-0.0.8/core/default/mappers/simple/event_deployer.py` & `cdev-0.0.9/core/default/mappers/simple/event_deployer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from time import sleep
-from typing import Dict, List
+from typing import Dict
 from uuid import uuid4
 
 from core.default.resources.simple import xlambda as simple_lambda
 from core.default.resources.simple import api as simple_api
 from core.default.resources.simple import object_store as simple_bucket
 from core.default.resources.simple import table as simple_table
 from core.default.resources.simple import queue as simple_queue
@@ -14,48 +14,49 @@
 from . import bucket_deployer
 from . import topic_deployer
 
 
 ##############################################
 ###### API GATEWAY ROUTE EVENTS
 ##############################################
-def _handle_adding_api_event(event: simple_api.route_event_model, cloud_function_id: str) -> Dict:
+def _handle_adding_api_event(
+    event: simple_api.route_event_model, cloud_function_id: str
+) -> Dict:
     # Needed info
     #   - Event model
     #   - originating resource output
     #   - responding resource output
-    
+
     # Returns:
     #   - Info about the deployed stuff
 
     api_id = event.api_id
     route_id = event.route_id
-    
+
     args = {
         "IntegrationType": "AWS_PROXY",
         "IntegrationUri": cloud_function_id,
         "PayloadFormatVersion": "2.0",
         "IntegrationMethod": event.verb,
         "ApiId": api_id,
     }
 
     if event.response_type:
-        args.update({
-            "ResponseParameters": {
-                "200": {
-                    "overwrite:header.Content-Type": event.response_type
+        args.update(
+            {
+                "ResponseParameters": {
+                    "200": {"overwrite:header.Content-Type": event.response_type}
                 }
             }
-        })
-    
+        )
+
     integration_rv = aws_client.run_client_function(
         "apigatewayv2", "create_integration", args
     )
 
-
     # Now that the integration has been created we need to attach it to the apigateway route
     update_info = {
         "ApiId": api_id,
         "RouteId": route_id,
         "Target": f"integrations/{integration_rv.get('IntegrationId')}",
     }
 
@@ -70,77 +71,67 @@
         "FunctionName": cloud_function_id,
         "Action": "lambda:InvokeFunction",
         "Principal": "apigateway.amazonaws.com",
         "StatementId": stmt_id,
         "SourceArn": f"arn:aws:execute-api:{aws_region}:{aws_account}:{api_id}/*/{event.verb}{event.path}",
     }
 
-    aws_client.run_client_function(
-        "lambda", "add_permission", permission_model_args
-    )
+    aws_client.run_client_function("lambda", "add_permission", permission_model_args)
 
     return {
         "integration_id": integration_rv.get("IntegrationId"),
         "permission_stmt_id": stmt_id,
         "api_id": api_id,
-        "route_id": route_id
+        "route_id": route_id,
     }
 
 
 def _handle_deleting_api_event(event: dict, function_cloud_id: str) -> bool:
     cloud_id = function_cloud_id
     integration_id = event.get("integration_id")
     stmt_id = event.get("permission_stmt_id")
-    
+
     api_id = event.get("api_id")
     route_id = event.get("route_id")
 
     # Delete the permission on the lambda function
     aws_client.run_client_function(
         "lambda",
         "remove_permission",
-        {
-            "FunctionName": cloud_id, 
-            "StatementId": stmt_id
-        },
+        {"FunctionName": cloud_id, "StatementId": stmt_id},
     )
 
-    # To delete a route event from a simple api we need to delete the integration.    
+    # To delete a route event from a simple api we need to delete the integration.
     # Leave the target blank so that the route has no integration.
     # Then delete the actual integration cloud obj
     update_info = {"ApiId": api_id, "RouteId": route_id, "Target": ""}
 
     aws_client.run_client_function("apigatewayv2", "update_route", update_info)
 
-
     aws_client.run_client_function(
         "apigatewayv2",
         "delete_integration",
-        {
-            "ApiId": api_id, 
-            "IntegrationId": integration_id
-        },
+        {"ApiId": api_id, "IntegrationId": integration_id},
     )
 
+
 ##############################################
 ##### DYNAMODB TABLE STREAM EVENT
 ##############################################
 
 
-def _handle_adding_stream_event(event: simple_table.stream_event_model, cloud_function_id) -> Dict:
+def _handle_adding_stream_event(
+    event: simple_table.stream_event_model, cloud_function_id
+) -> Dict:
     table_name = event.table_name
     view_type = event.view_type
     batch_size = event.batch_size
 
     rv = aws_client.run_client_function(
-        "dynamodb", 
-        "describe_table", 
-        {
-            "TableName": table_name
-        }
+        "dynamodb", "describe_table", {"TableName": table_name}
     )
 
     if not rv.get("Table").get("StreamSpecification"):
         rv = aws_client.run_client_function(
             "dynamodb",
             "update_table",
             {
@@ -170,53 +161,50 @@
 
         else:
             table_data = rv.get("Table")
 
     stream_arn = table_data.get("LatestStreamArn")
 
     sleep(5)
-    function_response_types = [] if event.batch_failure else ['ReportBatchItemFailures'] 
+    function_response_types = [] if event.batch_failure else ["ReportBatchItemFailures"]
 
     rv = aws_client.run_client_function(
         "lambda",
         "create_event_source_mapping",
         {
             "EventSourceArn": stream_arn,
             "FunctionName": cloud_function_id,
             "Enabled": True,
             "BatchSize": batch_size,
             "StartingPosition": "LATEST",
-            "FunctionResponseTypes": function_response_types
+            "FunctionResponseTypes": function_response_types,
         },
     )
 
     uuid = rv.get("UUID")
 
-    return {
-        "stream_arn": stream_arn,  
-        "stream_event_id": uuid
-    }
+    return {"stream_arn": stream_arn, "stream_event_id": uuid}
 
 
 def _handle_deleting_stream_event(event: dict, function_cloud_id: str):
     uuid = event.get("stream_event_id")
 
     aws_client.run_client_function(
         "lambda", "delete_event_source_mapping", {"UUID": uuid}
     )
 
 
-
 ##############################################
 ##### BUCKET EVENT TRIGGER
 ##############################################
 
 
-
-def _handle_adding_bucket_event(bucket_event: simple_bucket.bucket_event_model , cloud_function_id: str) -> Dict:
+def _handle_adding_bucket_event(
+    bucket_event: simple_bucket.bucket_event_model, cloud_function_id: str
+) -> Dict:
 
     bucket_arn = bucket_event.bucket_arn
     bucket_name = bucket_event.bucket_name
     events = [bucket_event.bucket_event_type.value]
 
     # Add permission to lambda to allow s3 to invoke this function
     stmt_id = f"stmt-{str(uuid4())}"
@@ -224,172 +212,154 @@
         "FunctionName": cloud_function_id,
         "Action": "lambda:InvokeFunction",
         "Principal": "s3.amazonaws.com",
         "StatementId": stmt_id,
         "SourceArn": bucket_arn,
     }
 
-    aws_client.run_client_function(
-        "lambda", "add_permission", permission_model_args
-    )
+    aws_client.run_client_function("lambda", "add_permission", permission_model_args)
 
     # Add trigger to the bucket... use helper function in the bucket deployer because bucket can send events to sqs and sns also
     print(f"event to add {events}")
 
     # Wait a few seconds for the newly added permissions to take hold
-    # if this happens too fast, it will say the lambda does not have correct permissions to be triggered. 
+    # if this happens too fast, it will say the lambda does not have correct permissions to be triggered.
     sleep(5)
-    
+
     bucket_event_id = bucket_deployer.add_eventsource(
         bucket_name,
         bucket_deployer.event_hander_types.LAMBDA,
         cloud_function_id,
-        events
+        events,
     )
 
     return {
         "bucket_event_id": bucket_event_id,
         "permission_stmt_id": stmt_id,
         "bucket_name": bucket_name,
     }
 
 
 def _handle_deleting_bucket_event(event: dict, function_cloud_id: str):
-    
+
     bucket_event_id = event.get("bucket_event_id")
-    bucket_name =event.get("bucket_name")
+    bucket_name = event.get("bucket_name")
     stmt_id = event.get("permission_stmt_id")
 
-
     # Delete the permission on the lambda function
     aws_client.run_client_function(
         "lambda",
         "remove_permission",
-        {
-            "FunctionName": function_cloud_id, 
-            "StatementId": stmt_id
-        },
+        {"FunctionName": function_cloud_id, "StatementId": stmt_id},
     )
 
     bucket_deployer.remove_eventsource(bucket_name, bucket_event_id)
 
 
 ##############################################
 ##### QUEUE EVENT TRIGGER
 ##############################################
 
 
-def _handle_adding_queue_event(event: simple_queue.queue_event_model, cloud_function_id) -> Dict:
+def _handle_adding_queue_event(
+    event: simple_queue.queue_event_model, cloud_function_id
+) -> Dict:
     queue_arn = event.queue_arn
     batch_size = event.batch_size
 
-    function_response_types = [] if event.batch_failure else ['ReportBatchItemFailures'] 
+    function_response_types = [] if event.batch_failure else ["ReportBatchItemFailures"]
 
     rv = aws_client.run_client_function(
         "lambda",
         "create_event_source_mapping",
         {
             "EventSourceArn": queue_arn,
             "FunctionName": cloud_function_id,
             "Enabled": True,
             "BatchSize": batch_size,
-            "FunctionResponseTypes": function_response_types
+            "FunctionResponseTypes": function_response_types,
         },
     )
 
     uuid = rv.get("UUID")
 
-    return {
-        "queue_event_id": uuid
-    }
+    return {"queue_event_id": uuid}
 
 
-def _handle_deleting_queue_event(event: dict, function_cloud_id: str):
-    queue_event_id = event.get('queue_event_id')
+def _handle_deleting_queue_event(event: dict, function_cloud_id: str) -> None:
+    queue_event_id = event.get("queue_event_id")
 
     aws_client.run_client_function(
-        "lambda", 
-        "delete_event_source_mapping",
-        {
-            "UUID": queue_event_id
-        }
+        "lambda", "delete_event_source_mapping", {"UUID": queue_event_id}
     )
 
 
-
 ##############################################
 ##### TOPIC EVENT TRIGGER
 ##############################################
 
 
-def _handle_adding_topic_subscription(event: simple_topic.topic_event_model, cloud_function_id) -> Dict:
+def _handle_adding_topic_subscription(
+    event: simple_topic.topic_event_model, cloud_function_id
+) -> Dict:
     topic_arn = event.topic_arn
 
     # Add permission to lambda to allow apigateway to invoke this function
     stmt_id = f"stmt-{str(uuid4())}"
     permission_model_args = {
         "FunctionName": cloud_function_id,
         "Action": "lambda:InvokeFunction",
         "Principal": "sns.amazonaws.com",
         "StatementId": stmt_id,
         "SourceArn": topic_arn,
     }
 
-    aws_client.run_client_function(
-        "lambda", "add_permission", permission_model_args
-    )
+    aws_client.run_client_function("lambda", "add_permission", permission_model_args)
 
     subscribe_arn = topic_deployer.add_subscriber(
         topic_arn, "lambda", cloud_function_id
     )
 
-    return {
-        "topic_event_id": subscribe_arn, 
-        "permission_stmt_id": stmt_id
-    }
+    return {"topic_event_id": subscribe_arn, "permission_stmt_id": stmt_id}
 
 
-def _handle_deleting_topic_subscription(event: dict, function_cloud_id: str):
+def _handle_deleting_topic_subscription(event: dict, function_cloud_id: str) -> bool:
     subscription_arn = event.get("topic_event_id")
     permission_stmt_id = event.get("permission_stmt_id")
 
     # Delete the permission on the lambda function
     aws_client.run_client_function(
         "lambda",
         "remove_permission",
-        {
-            "FunctionName": function_cloud_id, 
-            "StatementId": permission_stmt_id
-        },
+        {"FunctionName": function_cloud_id, "StatementId": permission_stmt_id},
     )
 
     # Remove subscription
     topic_deployer.remove_subscriber(subscription_arn)
 
     return True
 
 
 EVENT_TO_HANDLERS = {
     simple_lambda.RUUID: {
-        simple_api.RUUID:{   
+        simple_api.RUUID: {
             "CREATE": _handle_adding_api_event,
             "REMOVE": _handle_deleting_api_event,
         },
-        simple_bucket.RUUID:{
+        simple_bucket.RUUID: {
             "CREATE": _handle_adding_bucket_event,
             "REMOVE": _handle_deleting_bucket_event,
         },
-        simple_table.RUUID:{
+        simple_table.RUUID: {
             "CREATE": _handle_adding_stream_event,
             "REMOVE": _handle_deleting_stream_event,
         },
-        simple_queue.RUUID:{
+        simple_queue.RUUID: {
             "CREATE": _handle_adding_queue_event,
             "REMOVE": _handle_deleting_queue_event,
         },
-        simple_topic.RUUID:{
+        simple_topic.RUUID: {
             "CREATE": _handle_adding_topic_subscription,
             "REMOVE": _handle_deleting_topic_subscription,
-        }
+        },
     },
-    
 }
```

### Comparing `cdev-0.0.8/core/default/mappers/simple/lambda_deployer.py` & `cdev-0.0.9/core/default/mappers/simple/lambda_deployer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,49 @@
-import math
 import os
 from time import sleep
-from typing import Any, Dict, FrozenSet, Union, List, Tuple
+from typing import Any, Dict, List, Tuple, Optional
 from uuid import uuid4
 
 from core.constructs.resource import Resource_Difference, Resource_Change_Type
 from core.constructs.output_manager import OutputTask
 from core.constructs.models import frozendict
+from core.constructs.workspace import Workspace
 
 from core.default.resources.simple import xlambda as simple_xlambda
-from core.default.resources.simple.iam import permission_arn_model, permission_model
 
 from core.utils import paths as core_paths, hasher
 from core.utils.logger import log
 from core.utils.platforms import lambda_python_environment
 
 
-
-from .. import aws_client 
+from .. import aws_client
 from boto3.s3.transfer import TransferConfig
 
 
-#from .lambda_event_deployer import EVENT_TO_HANDLERS
+# from .lambda_event_deployer import EVENT_TO_HANDLERS
 from .role_deployer import (
     create_role_with_permissions,
     delete_role_and_permissions,
     add_policy,
     delete_policy,
     detach_policy,
 )
 
 
-from .event_deployer import (
-    EVENT_TO_HANDLERS
-)
+from .event_deployer import EVENT_TO_HANDLERS
 
 
 python_environment_to_aws_params: Dict[lambda_python_environment, Tuple] = {
-    lambda_python_environment.py37: ('python3.7', 'x86_64'),
-    lambda_python_environment.py38_x86_64: ('python3.8', 'x86_64'),
-    lambda_python_environment.py38_arm64: ('python3.8', 'arm64'),
-    lambda_python_environment.py39_x86_64: ('python3.9', 'x86_64'),
-    lambda_python_environment.py39_arm64: ('python3.9', 'arm64'),
-    lambda_python_environment.py3_x86_64: ('python3.9', 'x86_64'),
-    lambda_python_environment.py3_arm64: ('python3.9', ' arm64'),
+    lambda_python_environment.py37: ("python3.7", "x86_64"),
+    lambda_python_environment.py38_x86_64: ("python3.8", "x86_64"),
+    lambda_python_environment.py38_arm64: ("python3.8", "arm64"),
+    lambda_python_environment.py39_x86_64: ("python3.9", "x86_64"),
+    lambda_python_environment.py39_arm64: ("python3.9", "arm64"),
+    lambda_python_environment.py3_x86_64: ("python3.9", "x86_64"),
+    lambda_python_environment.py3_arm64: ("python3.9", " arm64"),
 }
 
 
 AssumeRolePolicyDocumentJSON = """{
   "Version": "2012-10-17",
   "Statement": [
     {
@@ -56,95 +52,88 @@
         "Service": "lambda.amazonaws.com"
       },
       "Action": "sts:AssumeRole"
     }
   ]
 }"""
 
-
-BUCKET = "cdev-demo-project-artifacts"
-
 ###########################
 ###### Main Handlers
 ###########################
+
+
 def _create_simple_lambda(
-        transaction_token: str, 
-        namespace_token: str, 
-        resource: simple_xlambda.simple_function_model, 
-        output_task: OutputTask
-    ) -> Dict:
+    transaction_token: str,
+    namespace_token: str,
+    resource: simple_xlambda.simple_function_model,
+    output_task: OutputTask,
+    artifact_bucket: str,
+) -> Dict:
     # Steps for creating a deployed lambda function
     # 1. Create IAM Role with needed permissions (note this is first to give aws more time to create the role in all regions and be available for use)
     # 2. Upload the artifact to S3 as the archive location
     # 3. Upload dependencies if needed
     # 4. Create the function
     # 5. Create any integrations that are need based on Events passed in
     log.debug("Create lambda %s", resource)
     full_namespace_suffix = hasher.hash_list([namespace_token, str(uuid4())])
 
     function_name = f"cdev_function_{full_namespace_suffix}"
     output_task.update(
         comment=f"Creating lambda function resources for lambda {function_name}"
     )
 
-    final_info = {
-        'function_name': function_name
-    }
+    final_info = {"function_name": function_name}
 
     output_task.update(
         comment=f"Creating IAM Role w/ permissions {resource.permissions}"
     )
     # Step 1
     role_name = f"role_{function_name}"
-    role_arn, permission_info = create_role_with_permissions(role_name, resource.permissions, AssumeRolePolicyDocumentJSON)
-
-    output_task.update(
-        comment=f"Create role for lambda function {resource.name}"
+    role_arn, permission_info = create_role_with_permissions(
+        role_name, resource.permissions, AssumeRolePolicyDocumentJSON
     )
 
+    output_task.update(comment=f"Create role for lambda function {resource.name}")
+
     final_info["role_id"] = role_arn
     final_info["role_name"] = role_name
     final_info["permissions"] = permission_info
 
     # Step 2
-    output_task.update(
-        comment=f"Uploading code for lambda function {resource.name}"
-    )
+    output_task.update(comment=f"Uploading code for lambda function {resource.name}")
 
-    keyname = _upload_s3_code_artifact(function_name, resource)
-    
+    keyname = _upload_s3_code_artifact(function_name, resource, artifact_bucket)
 
-    final_info["artifact_bucket"] = BUCKET
+    final_info["artifact_bucket"] = artifact_bucket
     final_info["artifact_key"] = keyname
 
-    
     # Step 4
     # TODO
     output_task.update(
         comment=f"[blink]Waiting for role to finish creating (~10s)[/blink]"
     )
     sleep(10)
     # ughhhh add a retry wrapper because it takes time to generate the IAM roles across all regions so we need to wait a few seconds to create this
-    
-    output_task.update(
-        comment=f"Create Lambda function"
-    )
+
+    output_task.update(comment=f"Create Lambda function")
 
     runtime, arch = python_environment_to_aws_params.get(resource.platform)
-    
+
     lambda_function_args = {
         "FunctionName": function_name,
         "Runtime": runtime,
         "Architectures": [arch],
         "Role": role_arn,
         "Handler": resource.configuration.handler,
-        "Code": {"S3Bucket": BUCKET, "S3Key": keyname},
-        "Environment": {
-            "Variables":resource.configuration.environment_variables._d
-        }
+        "MemorySize": resource.configuration.memory_size,
+        "EphemeralStorage": {"Size": resource.configuration.storage},
+        "Timeout": resource.configuration.timeout,
+        "Code": {"S3Bucket": artifact_bucket, "S3Key": keyname},
+        "Environment": {"Variables": resource.configuration.environment_variables._d}
         if resource.configuration.environment_variables
         else {},
         "Layers": list(resource.external_dependencies)
         if resource.external_dependencies
         else [],
     }
     log.debug("lambda configuration %s", lambda_function_args)
@@ -152,521 +141,725 @@
     lambda_function_rv = aws_client.run_client_function(
         "lambda", "create_function", lambda_function_args
     )
     final_info["layers"] = resource.external_dependencies
     final_info["cloud_id"] = lambda_function_rv.get("FunctionArn")
 
     # Step 5
-    
+
     if resource.events:
         available_event_handlers = EVENT_TO_HANDLERS.get(simple_xlambda.RUUID)
         function_cloud_id = final_info.get("cloud_id")
 
         event_to_output = {}
         for event in resource.events:
 
             if not event.originating_resource_type in available_event_handlers:
-                raise Exception(f'No handlers for {event.originating_resource_type} to {simple_xlambda.RUUID} events')            
-
-
-            output = EVENT_TO_HANDLERS.get(simple_xlambda.RUUID).get(event.originating_resource_type).get("CREATE")(
-                event, function_cloud_id
+                raise Exception(
+                    f"No handlers for {event.originating_resource_type} to {simple_xlambda.RUUID} events"
+                )
+
+            output = (
+                EVENT_TO_HANDLERS.get(simple_xlambda.RUUID)
+                .get(event.originating_resource_type)
+                .get("CREATE")(event, function_cloud_id)
             )
 
-
             event_to_output[event.hash] = output
-            
 
         final_info["events"] = event_to_output
 
     return final_info
 
 
 def _remove_simple_lambda(
-    transaction_token: str,  
-    previous_resource: simple_xlambda.simple_function_model, 
+    transaction_token: str,
+    previous_resource: simple_xlambda.simple_function_model,
     previous_output: Dict,
-    output_task: OutputTask
-) -> bool:
+    output_task: OutputTask,
+) -> None:
     # Steps:
     # Remove and event that is on the function to make sure resources are properly cleaned up
     # Remove the actual function
     # Remove the role associated with the function
-    
-    cloud_id = previous_output.get('cloud_id')
 
+    cloud_id = previous_output.get("cloud_id")
 
     if previous_resource.events:
-        output_task.update(
-            comment=f"Removing Events"
-        )
+        output_task.update(comment=f"Removing Events")
         event_hashes_to_events = {
-            x.get('hash'):x for x in [dict(y) for y in previous_resource.events]
+            x.get("hash"): x for x in [dict(y) for y in previous_resource.events]
         }
 
-
-        for event_id, event_output in previous_output.get('events').items():        
-            originating_resource_type = event_hashes_to_events.get(event_id).get('originating_resource_type')
-
-            EVENT_TO_HANDLERS.get(simple_xlambda.RUUID).get(originating_resource_type).get("REMOVE")(
-                event_output,  cloud_id
+        for event_id, event_output in previous_output.get("events").items():
+            originating_resource_type = event_hashes_to_events.get(event_id).get(
+                "originating_resource_type"
             )
-        
 
-    output_task.update(
-        comment=f"Deleting function resource for {cloud_id}"
-    )
+            EVENT_TO_HANDLERS.get(simple_xlambda.RUUID).get(
+                originating_resource_type
+            ).get("REMOVE")(event_output, cloud_id)
 
+    output_task.update(comment=f"Deleting function resource for {cloud_id}")
 
     aws_client.run_client_function(
         "lambda", "delete_function", {"FunctionName": cloud_id}
     )
 
-    role_arn = previous_output.get("role_id")
+    # role_arn = previous_output.get("role_id")
     role_name = previous_output.get("role_name")
-    permissions =  previous_output.get("permissions")
+    permissions = previous_output.get("permissions")
 
     delete_role_and_permissions(role_name, permissions)
 
-    output_task.update(
-        comment=f"Deleting permissions for the resource ({cloud_id})"
-    )
+    output_task.update(comment=f"Deleting permissions for the resource ({cloud_id})")
 
-   
-    output_task.update(
-        comment=f"Removed resources for lambda {cloud_id}"
-    )
+    output_task.update(comment=f"Removed resources for lambda {cloud_id}")
 
 
 def _update_simple_lambda(
-    transaction_token: str, 
+    transaction_token: str,
     namespace_token: str,
     previous_resource: simple_xlambda.simple_function_model,
     new_resource: simple_xlambda.simple_function_model,
     previous_output: Dict,
-    output_task: OutputTask
+    output_task: OutputTask,
+    artifact_bucket: str,
+) -> Dict:
+    """
+    Updates can be of:
+      - 1 Configuration
+      - 2 Permissions
+      - 3 Source code
+      - 4 Dependencies
+      - 5 Events
+    """
+
+    output_task.update(comment=f"Updating lambda function {new_resource.name}")
+
+    function_name = previous_output["cloud_id"]
+
+    mutable_previous_output = dict(previous_output)
+
+    _update_configuration(output_task, function_name, previous_resource, new_resource)
+
+    did_update_permission = _update_permissions(
+        output_task,
+        mutable_previous_output,
+        previous_output,
+        previous_resource,
+        new_resource,
+    )
+
+    did_update_src_code = _update_source_code(
+        output_task,
+        function_name,
+        mutable_previous_output,
+        previous_output,
+        previous_resource,
+        new_resource,
+        artifact_bucket,
+    )
+
+    _update_dependencies(
+        output_task,
+        function_name,
+        mutable_previous_output,
+        did_update_src_code,
+        previous_resource,
+        new_resource,
+    )
+
+    _update_events(
+        output_task,
+        function_name,
+        mutable_previous_output,
+        did_update_permission,
+        previous_resource,
+        new_resource,
+    )
+
+    return mutable_previous_output
+
+
+def _update_configuration(
+    output_task: OutputTask,
+    function_name: str,
+    previous_resource: simple_xlambda.simple_function_model,
+    new_resource: simple_xlambda.simple_function_model,
 ) -> bool:
-    # Updates can be of:
-    # Update source code or dependencies
-    # Update configuration
-    # Update events
 
-    
-    output_task.update(
-        comment=f"Updating lambda function {new_resource.name}"
+    updated_configuration = {}
+    __update_configuration_basic(
+        updated_configuration,
+        previous_resource.configuration,
+        new_resource.configuration,
     )
 
-    cloud_id = previous_output['cloud_id']
+    __update_configuration_environment_variables(
+        updated_configuration,
+        previous_resource.configuration.environment_variables,
+        new_resource.configuration.environment_variables,
+    )
 
-    did_update_permission = False
-    did_update_src_code = False
+    if not updated_configuration:
+        log.debug("Simple lambda, configuration didn't change")
+        return False
 
-    mutable_previous_output = dict(previous_output)
-    
-    # TODO all configurations
-    if not previous_resource.configuration == new_resource.configuration:
-        if (
-            not previous_resource.configuration.environment_variables
-            == new_resource.configuration.environment_variables
-        ):
-            output_task.update(
-                comment=f"Updating Environment Variables"
-            )
-            
-            aws_client.run_client_function(
-                "lambda",
-                "update_function_configuration",
-                {
-                    "FunctionName": cloud_id,
-                    "Environment": {
-                        "Variables":new_resource.configuration.environment_variables._d
-                    }
-                },
-            )
+    updated_configuration["FunctionName"] = function_name
+    output_task.update(comment=f"Updating configuration")
+    aws_client.run_client_function(
+        "lambda", "update_function_configuration", updated_configuration
+    )
 
-    if not previous_resource.permissions == new_resource.permissions:
-        output_task.update(
-            comment=f"Updating Policies"
-        )
-        permission_output: frozenset[Dict] = previous_output.get("permissions")
-        role_name_output = previous_output.get("role_name")
+    log.debug("Simple lambda, configuration updated")
+    return True
 
-        remove_permissions = previous_resource.permissions.difference(new_resource.permissions)
-        create_permissions = new_resource.permissions.difference(previous_resource.permissions)
 
+def __update_configuration_basic(
+    updated_configuration: Dict,
+    previous_configuration: simple_xlambda.simple_function_configuration_model,
+    new_configuration: simple_xlambda.simple_function_configuration_model,
+) -> None:
+    if previous_configuration == new_configuration:
+        log.debug("Simple lambda, basic configuration didn't change")
+    else:
+        log.debug("Simple lambda, basic configuration modified")
+        updated_configuration["Handler"] = new_configuration.handler
+        updated_configuration["MemorySize"] = new_configuration.memory_size
+        updated_configuration["Timeout"] = new_configuration.timeout
+        updated_configuration["EphemeralStorage"] = {"Size": new_configuration.storage}
+
+
+def __update_configuration_environment_variables(
+    updated_configuration: Dict,
+    previous_environment_variables: frozendict,
+    new_resource_environment_variables: frozendict,
+) -> None:
+    if previous_environment_variables == new_resource_environment_variables:
+        log.debug("Simple lambda, environment variables didn't change")
+    else:
+        log.debug("Simple lambda, environment variables modified")
+        updated_configuration["Environment"] = {
+            "Variables": new_resource_environment_variables._d
+        }
 
-        for permission in create_permissions:
-            
-            rv = frozendict(add_policy(role_name_output, permission))
-            tmp = list(permission_output)
-            tmp.append(rv)
-            permission_output = frozenset(tmp)
 
-        for permission in remove_permissions:
+def _update_permissions(
+    output_task: OutputTask,
+    mutable_previous_output: Dict,
+    previous_output: Dict,
+    previous_resource: simple_xlambda.simple_function_model,
+    new_resource: simple_xlambda.simple_function_model,
+) -> bool:
+    if previous_resource.permissions == new_resource.permissions:
+        log.debug("Simple lambda, permissions didn't change")
+        return False
+
+    permission_output = previous_output.get("permissions")
+    role_name_output = previous_output.get("role_name")
+
+    permission_output = __update_permissions_create(
+        output_task,
+        role_name_output,
+        permission_output,
+        previous_resource,
+        new_resource,
+    )
+    permission_output = __update_permissions_remove(
+        output_task,
+        role_name_output,
+        permission_output,
+        previous_resource,
+        new_resource,
+    )
 
-            previous_permission_output_list = [x for x in permission_output if x.get('hash') == permission.hash]
+    mutable_previous_output["permissions"] = permission_output
+    log.debug("Simple lambda, permissions updated")
+    return True
 
-            if len(previous_permission_output_list) > 1:
-                raise Exception
 
-            previous_permission_output = previous_permission_output_list[0]
-            
-            delete_policy(
-                role_name_output,
-                previous_permission_output
-            )
+def __update_permissions_create(
+    output_task: OutputTask,
+    role_name_output: str,
+    permission_output: "frozenset[Dict]",
+    previous_resource: simple_xlambda.simple_function_model,
+    new_resource: simple_xlambda.simple_function_model,
+) -> "frozenset[Dict]":
 
-            permission_output = frozenset([x for x in permission_output if not x.get('hash') == permission.hash])
+    create_permissions = new_resource.permissions.difference(
+        previous_resource.permissions
+    )
+    if not create_permissions:
+        log.debug("Simple lambda, no new permissions")
+        return permission_output
+
+    output_task.update(comment=f"Updating Policies, creating Permissions")
+    policies: List[frozendict] = []
+    for permission in create_permissions:
+        rv = frozendict(add_policy(role_name_output, permission))
+        policies.append(rv)
+
+    permission_output = frozenset(list(permission_output) + policies)
+    log.debug(f"Simple lambda, added {len(create_permissions)} permissions")
+    return permission_output
+
+
+def __update_permissions_remove(
+    output_task: OutputTask,
+    role_name_output: str,
+    permission_output: "frozenset[Dict]",
+    previous_resource: simple_xlambda.simple_function_model,
+    new_resource: simple_xlambda.simple_function_model,
+) -> "frozenset[Dict]":
 
-        mutable_previous_output['permissions'] = permission_output
-        
-        did_update_permission = True
+    remove_permissions = previous_resource.permissions.difference(
+        new_resource.permissions
+    )
+    if not remove_permissions:
+        log.debug("Simple lambda, no permissions to remove")
+        return permission_output
 
+    output_task.update(comment=f"Updating Policies, removing Permissions")
+    for permission in remove_permissions:
+        previous_permission_output_list = [
+            x for x in permission_output if x.get("hash") == permission.hash
+        ]
 
-    if not previous_resource.src_code_hash == new_resource.src_code_hash:
-        sleep(3)
-        output_task.update(
-            comment=f"Update Source Code"
-        )
+        if len(previous_permission_output_list) > 1:
+            raise Exception
+
+        previous_permission_output = previous_permission_output_list[0]
 
-        keyname = _upload_s3_code_artifact(previous_output.get('function_name'), new_resource)
-        
-        aws_client.run_client_function(
-            "lambda",
-            "update_function_code",
-            {
-                "FunctionName": cloud_id,
-                "S3Key": keyname,
-                "S3Bucket": BUCKET,
-                "Publish": True,
-            },
+        delete_policy(role_name_output, previous_permission_output)
+
+        permission_output = frozenset(
+            [x for x in permission_output if not x.get("hash") == permission.hash]
         )
 
-        mutable_previous_output["artifact_key"] = keyname
-        did_update_src_code = True
+    log.debug(f"Simple lambda, removed {len(remove_permissions)} permissions")
+    return permission_output
 
 
-    if (
-        not previous_resource.external_dependencies
-        == new_resource.external_dependencies
-    ):
-        if did_update_src_code:
-            output_task.update(
-                comment=f"[blink]Waiting for src code update to complete. ~5s[/blink]"
-            )
-            sleep(5)
+def _update_source_code(
+    output_task: OutputTask,
+    function_name: str,
+    mutable_previous_output: Dict,
+    previous_output: Dict,
+    previous_resource: simple_xlambda.simple_function_model,
+    new_resource: simple_xlambda.simple_function_model,
+    artifact_bucket: str,
+) -> bool:
 
+    if previous_resource.src_code_hash == new_resource.src_code_hash:
+        log.debug("Simple lambda, source code didn't change")
+        return False
 
-        output_task.update(
-            comment=f"Update Dependencies"
-        )
-        
-        remove_dependencies = previous_resource.external_dependencies.difference(new_resource.external_dependencies)
-        create_dependencies = new_resource.external_dependencies.difference(previous_resource.external_dependencies)
-        
-        previous_dependency_output: List =  list(mutable_previous_output.get("layers"))
-
-        for dependency in create_dependencies:
-            previous_dependency_output.append(dependency)
-
-        for dependency in remove_dependencies:
-            previous_dependency_output.remove(dependency)
-
-        aws_client.run_client_function(
-            "lambda",
-            "update_function_configuration",
-            {
-                "FunctionName": cloud_id,
-                "Layers": previous_dependency_output
-            },
-        )
+    sleep(3)
+    output_task.update(comment=f"Update Source Code")
 
-        mutable_previous_output['layers'] = previous_dependency_output
+    keyname = _upload_s3_code_artifact(
+        previous_output.get("function_name"), new_resource, artifact_bucket
+    )
 
-    if not previous_resource.events == new_resource.events:
-        if did_update_permission:
-            # Wait because the updated permission can effect if the event can be bound. 
-            output_task.update(
-                comment=f"[blink]Waiting for policies to complete. ~10s[/blink]"
-            )
-            sleep(10)
+    aws_client.run_client_function(
+        "lambda",
+        "update_function_code",
+        {
+            "FunctionName": function_name,
+            "S3Key": keyname,
+            "S3Bucket": artifact_bucket,
+            "Publish": True,
+        },
+    )
+
+    mutable_previous_output["artifact_key"] = keyname
+    log.debug("Simple lambda, source code updated")
+    return True
 
+
+def _update_dependencies(
+    output_task: OutputTask,
+    function_name: str,
+    mutable_previous_output: Dict,
+    did_update_src_code: bool,
+    previous_resource: simple_xlambda.simple_function_model,
+    new_resource: simple_xlambda.simple_function_model,
+) -> bool:
+
+    if previous_resource.external_dependencies == new_resource.external_dependencies:
+        log.debug("Simple lambda, dependencies didn't change")
+        return False
+
+    create_dependencies = new_resource.external_dependencies.difference(
+        previous_resource.external_dependencies
+    )
+    remove_dependencies = previous_resource.external_dependencies.difference(
+        new_resource.external_dependencies
+    )
+
+    if not create_dependencies and not remove_dependencies:
+        return False
+
+    if did_update_src_code:
         output_task.update(
-                comment=f"Updating Events"
-            )
+            comment=f"[blink]Waiting for src code update to complete. ~5s[/blink]"
+        )
+        sleep(5)
 
-        create_events = new_resource.events.difference(previous_resource.events)
-        remove_events = previous_resource.events.difference(new_resource.events)
+    output_task.update(comment=f"Update Dependencies")
+    previous_dependency_output: List = list(mutable_previous_output.get("layers"))
 
-        available_event_handlers = EVENT_TO_HANDLERS.get(simple_xlambda.RUUID)
+    for dependency in create_dependencies:
+        previous_dependency_output.append(dependency)
 
-        previous_event_output: dict = dict(mutable_previous_output.get('events')) if mutable_previous_output.get('events') else {}
+    for dependency in remove_dependencies:
+        previous_dependency_output.remove(dependency)
 
-       
-        for _event in create_events:
-            if not _event.originating_resource_type in available_event_handlers:
-                raise Exception(f'No handlers for {_event.originating_resource_type} to {simple_xlambda.RUUID} events')            
+    aws_client.run_client_function(
+        "lambda",
+        "update_function_configuration",
+        {"FunctionName": function_name, "Layers": previous_dependency_output},
+    )
 
+    mutable_previous_output["layers"] = previous_dependency_output
+    log.debug(
+        f"Simple lambda, dependencies updated. Added {len(create_dependencies)}, removed: {len(remove_dependencies)}"
+    )
+    return True
 
-            output_task.update(
-                comment=f"Create Event {_event}"
-            )
 
-            output = EVENT_TO_HANDLERS.get(simple_xlambda.RUUID).get(_event.originating_resource_type).get("CREATE")(
-                _event, cloud_id
-            )
+def _update_events(
+    output_task: OutputTask,
+    function_name: str,
+    mutable_previous_output: Dict,
+    did_update_permission: bool,
+    previous_resource: simple_xlambda.simple_function_model,
+    new_resource: simple_xlambda.simple_function_model,
+) -> bool:
+    if previous_resource.events == new_resource.events:
+        log.debug("Simple lambda, events didn't change")
+        return False
 
+    if did_update_permission:
+        # Wait because the updated permission can effect if the event can be bound.
+        output_task.update(
+            comment=f"[blink]Waiting for policies to complete. ~10s[/blink]"
+        )
+        sleep(10)
 
-            previous_event_output[_event.hash] = output
+    output_task.update(comment=f"Updating Events")
 
-        previous_event_hashes_to_output = {
-            hash:output for hash, output in [ (y.hash, dict(previous_event_output.get(y.hash))) for y in remove_events if previous_event_output.get(y.hash)]
-        }
+    create_events = new_resource.events.difference(previous_resource.events)
+    remove_events = previous_resource.events.difference(new_resource.events)
 
-        previous_hashes_to_events = {
-            x.get('hash'):x for x in [dict(y) for y in remove_events]
-        }
+    available_event_handlers = EVENT_TO_HANDLERS.get(simple_xlambda.RUUID)
 
-        for event_id, event_output in previous_event_hashes_to_output.items():        
-            originating_resource_type = previous_hashes_to_events.get(event_id).get('originating_resource_type')
+    previous_event_output: dict = (
+        dict(mutable_previous_output.get("events"))
+        if mutable_previous_output.get("events")
+        else {}
+    )
 
-            output_task.update(
-                comment=f"Delete Event {event_id}"
+    for _event in create_events:
+        if _event.originating_resource_type not in available_event_handlers:
+            raise Exception(
+                f"No handlers for {_event.originating_resource_type} to {simple_xlambda.RUUID} events"
             )
 
-            EVENT_TO_HANDLERS.get(simple_xlambda.RUUID).get(originating_resource_type).get("REMOVE")(
-                event_output,  cloud_id
-            )
+        output_task.update(comment=f"Create Event {_event}")
 
-            previous_event_output.pop(event_id)
+        output = (
+            EVENT_TO_HANDLERS.get(simple_xlambda.RUUID)
+            .get(_event.originating_resource_type)
+            .get("CREATE")(_event, function_name)
+        )
 
-        mutable_previous_output['events'] = previous_event_output
-        
-    
-    return mutable_previous_output
+        previous_event_output[_event.hash] = output
 
+    previous_event_hashes_to_output = {
+        hash: output
+        for hash, output in [
+            (y.hash, dict(previous_event_output.get(y.hash)))
+            for y in remove_events
+            if previous_event_output.get(y.hash)
+        ]
+    }
+
+    previous_hashes_to_events = {
+        x.get("hash"): x for x in [dict(y) for y in remove_events]
+    }
+
+    for event_id, event_output in previous_event_hashes_to_output.items():
+        originating_resource_type = previous_hashes_to_events.get(event_id).get(
+            "originating_resource_type"
+        )
+
+        output_task.update(comment=f"Delete Event {event_id}")
 
+        EVENT_TO_HANDLERS.get(simple_xlambda.RUUID).get(originating_resource_type).get(
+            "REMOVE"
+        )(event_output, function_name)
 
+        previous_event_output.pop(event_id)
 
+    mutable_previous_output["events"] = previous_event_output
+    log.debug("Simple lambda, events updated")
+    return True
 
 
 ###############################
 ###### Upload Artifacts to S3
 ###############################
 
+
 def _upload_s3_code_artifact(
-    function_name: str, 
+    function_name: str,
     resource: simple_xlambda.simple_function_model,
+    artifact_bucket: str,
 ) -> str:
     # Takes in a resource and create an s3 artifact that can be use as src code for lambda deployment
     keyname = function_name + f"-{resource.hash}" + ".zip"
     # original_zipname = resource.configuration.Handler.split(".")[0] + ".zip"
-    zip_location =  core_paths.get_full_path_from_workspace_base(resource.filepath)
+    zip_location = core_paths.get_full_path_from_workspace_base(resource.filepath)
 
     if not os.path.isfile(zip_location):
         # TODO better exception
         raise Exception
 
     with open(zip_location, "rb") as fh:
         object_args = {
-            "Bucket": BUCKET,
+            "Bucket": artifact_bucket,
             "Key": keyname,
             "Body": fh.read(),
         }
         aws_client.run_client_function("s3", "put_object", object_args)
 
     return keyname
 
+
 def _upload_s3_dependency(
     dependency: simple_xlambda.dependency_layer_model,
-    output_task: OutputTask
+    output_task: OutputTask,
+    artifact_bucket: str,
 ) -> str:
     # Takes in a resource and create an s3 artifact that can be use as src code for lambda deployment
     keyname = f"{dependency.name}-{dependency.hash}.zip"
 
-    zip_location = core_paths.get_full_path_from_workspace_base(dependency.artifact_path)
+    zip_location = core_paths.get_full_path_from_workspace_base(
+        dependency.artifact_path
+    )
 
-    total_bytes =  os.path.getsize(zip_location)
+    total_bytes = os.path.getsize(zip_location)
 
     if not os.path.isfile(zip_location):
         # TODO better exception
         raise Exception
 
     config = TransferConfig(
         multipart_threshold=1024 * 25,
         max_concurrency=10,
         multipart_chunksize=1024 * 25,
         use_threads=True,
     )
 
-    
-
     def update_progress_bar(x):
-        advance_amount = (x/total_bytes) * 4
-        output_task.update(advance=advance_amount, comment='[blink]Uploading Package[/blink]')
-
+        advance_amount = (x / total_bytes) * 4
+        output_task.update(
+            advance=advance_amount, comment="[blink]Uploading Package[/blink]"
+        )
 
     object_args = {
-        "Bucket": BUCKET,
+        "Bucket": artifact_bucket,
         "Key": keyname,
         "Filename": zip_location,
         "Callback": update_progress_bar,
         "Config": config,
     }
     aws_client.run_client_function("s3", "upload_file", object_args)
 
-    output_task.update( comment='Uploaded Package')
+    output_task.update(comment="Uploaded Package")
 
     return keyname
 
 
 #######################
 ##### Main Entry Point
 #######################
 
-def handle_simple_lambda_function_deployment( 
-        transaction_token: str, 
-        namespace_token: str, 
-        resource_diff: Resource_Difference, 
-        previous_output: Dict[str, Any],
-        output_task: OutputTask
-    ) -> Dict:
+
+def handle_simple_lambda_function_deployment(
+    transaction_token: str,
+    namespace_token: str,
+    resource_diff: Resource_Difference,
+    previous_output: Dict[str, Any],
+    output_task: OutputTask,
+) -> Optional[Dict]:
+
+    artifact_bucket = _get_artifact_bucket_name()
+
     try:
         log.debug("Calling lambda mapper")
+
         if resource_diff.action_type == Resource_Change_Type.CREATE:
             return _create_simple_lambda(
                 transaction_token,
                 namespace_token,
-                resource_diff.new_resource,  
-                output_task
+                resource_diff.new_resource,
+                output_task,
+                artifact_bucket,
             )
         elif resource_diff.action_type == Resource_Change_Type.UPDATE_IDENTITY:
 
             return _update_simple_lambda(
                 transaction_token,
                 namespace_token,
-                simple_xlambda.simple_function_model(**resource_diff.previous_resource.dict()),
+                simple_xlambda.simple_function_model(
+                    **resource_diff.previous_resource.dict()
+                ),
                 resource_diff.new_resource,
                 previous_output,
-                output_task
+                output_task,
+                artifact_bucket,
             )
         elif resource_diff.action_type == Resource_Change_Type.DELETE:
 
             return _remove_simple_lambda(
                 transaction_token,
                 resource_diff.previous_resource,
                 previous_output,
-                output_task
+                output_task,
             )
 
     except Exception as e:
         print(e)
         raise Exception("COULD NOT DEPLOY")
 
+
 ###################################
 ##### Layers
 ###################################
 
-def _create_simple_layer( 
-        transaction_token: str, 
-        namespace_token: str, 
-        resource: simple_xlambda.dependency_layer_model, 
-        output_task: OutputTask
-    ):
+
+def _create_simple_layer(
+    transaction_token: str,
+    namespace_token: str,
+    resource: simple_xlambda.dependency_layer_model,
+    output_task: OutputTask,
+    artifact_bucket: str,
+) -> Dict:
 
     output_task.update(
         comment=f"Creating dependencies for lambda function {resource.name}"
     )
 
-    key_name = _upload_s3_dependency(resource, output_task)
+    key_name = _upload_s3_dependency(resource, output_task, artifact_bucket)
 
     # key name will always include .zip so remove that part and change '-' into '_'
-    layer_name = key_name.replace("-", "_")[:-4].replace(".","")
+    layer_name = key_name.replace("-", "_")[:-4].replace(".", "")
     dependency_rv = aws_client.run_client_function(
         "lambda",
         "publish_layer_version",
         {
-            "Content": {"S3Bucket": BUCKET, "S3Key": key_name},
+            "Content": {"S3Bucket": artifact_bucket, "S3Key": key_name},
             "LayerName": f"{layer_name}_{namespace_token[:10]}",
-            "CompatibleRuntimes": [
-                "python3.7",
-                "python3.8",
-                "python3.9"
-            ],
+            "CompatibleRuntimes": ["python3.7", "python3.8", "python3.9"],
         },
     )
 
     return {
         "cloud_id": f"{dependency_rv.get('LayerArn')}:{dependency_rv.get('Version')}",
         "arn": dependency_rv.get("LayerArn"),
-        "version": dependency_rv.get('Version')
+        "version": dependency_rv.get("Version"),
     }
 
+
 def _update_simple_layer(
-        transaction_token: str, 
-        namespace_token: str,
-        previous_resource: simple_xlambda.dependency_layer_model,
-        new_resource: simple_xlambda.dependency_layer_model,
-        previous_output: Dict,
-        output_task: OutputTask
-    ):
+    transaction_token: str,
+    namespace_token: str,
+    previous_resource: simple_xlambda.dependency_layer_model,
+    new_resource: simple_xlambda.dependency_layer_model,
+    previous_output: Dict,
+    output_task: OutputTask,
+    artifact_bucket: str,
+) -> Dict:
     return _create_simple_layer(
-        transaction_token,
-        namespace_token,
-        new_resource,
-        output_task
+        transaction_token, namespace_token, new_resource, output_task, artifact_bucket
     )
-    
+
+
 def _remove_simple_layer(
-        transaction_token,
-        resource,
-        previous_output,
-        output_task
-    ):
-        aws_client.run_client_function(
-            "lambda",
-            "delete_layer_version",
-            {
-                "LayerName": previous_output.get("arn"),
-                "VersionNumber": previous_output.get("version"),
-            },
-        )
+    transaction_token, resource, previous_output, output_task
+) -> None:
+    aws_client.run_client_function(
+        "lambda",
+        "delete_layer_version",
+        {
+            "LayerName": previous_output.get("arn"),
+            "VersionNumber": previous_output.get("version"),
+        },
+    )
+
 
+def handle_simple_layer_deployment(
+    transaction_token: str,
+    namespace_token: str,
+    resource_diff: Resource_Difference,
+    previous_output: Dict[str, Any],
+    output_task: OutputTask,
+) -> Optional[Dict]:
 
+    artifact_bucket = _get_artifact_bucket_name()
 
-def handle_simple_layer_deployment( 
-        transaction_token: str, 
-        namespace_token: str, 
-        resource_diff: Resource_Difference, 
-        previous_output: Dict[str, Any],
-        output_task: OutputTask
-    ) -> Dict:
     try:
         if resource_diff.action_type == Resource_Change_Type.CREATE:
             return _create_simple_layer(
                 transaction_token,
                 namespace_token,
-                resource_diff.new_resource,  
-                output_task
+                resource_diff.new_resource,
+                output_task,
+                artifact_bucket,
             )
         elif resource_diff.action_type == Resource_Change_Type.UPDATE_IDENTITY:
 
             return _update_simple_layer(
                 transaction_token,
                 namespace_token,
-                simple_xlambda.dependency_layer_model(**resource_diff.previous_resource.dict()),
+                simple_xlambda.dependency_layer_model(
+                    **resource_diff.previous_resource.dict()
+                ),
                 resource_diff.new_resource,
                 previous_output,
-                output_task
+                output_task,
+                artifact_bucket,
             )
 
         elif resource_diff.action_type == Resource_Change_Type.DELETE:
             return _remove_simple_layer(
                 transaction_token,
                 resource_diff.previous_resource,
                 previous_output,
-                output_task
+                output_task,
             )
 
     except Exception as e:
         print(e)
         raise Exception("COULD NOT DEPLOY")
+
+
+def _get_artifact_bucket_name() -> str:
+    """Get the artifact bucket name from the Workspace
+
+    Raises:
+        Exception
+
+    Returns:
+        str: Bucket Name
+    """
+    ws = Workspace.instance()
+
+    if not ws.settings.S3_ARTIFACTS_BUCKET:
+        raise Exception(
+            "No artifact bucket provided by the Workspace. Need to set the `S3_ARTIFACTS_BUCKET` setting in your workspace."
+        )
+
+    return ws.settings.S3_ARTIFACTS_BUCKET
```

### Comparing `cdev-0.0.8/core/default/mappers/simple/queue_deployer.py` & `cdev-0.0.9/core/default/mappers/simple/queue_deployer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-from typing import Any, Dict, List
+from typing import Any, Dict
 from uuid import uuid4
 
 from core.constructs.resource import Resource_Difference, Resource_Change_Type
-from core.default.resources.simple import queue 
+from core.default.resources.simple import queue
 from core.constructs.output_manager import OutputTask
 from core.utils import hasher
 
 from .. import aws_client
 
+
 def _create_simple_queue(
-    transaction_token: str, 
-    namespace_token: str, 
-    resource:  queue.queue_model,
-    output_task: OutputTask
+    transaction_token: str,
+    namespace_token: str,
+    resource: queue.queue_model,
+    output_task: OutputTask,
 ) -> Dict:
 
     attributes = {}
 
     full_namespace_suffix = hasher.hash_list([namespace_token, str(uuid4())])
 
-    queue_name = f"cdev-queue-{full_namespace_suffix}.fifo" if resource.is_fifo else f"cdev-queue-{full_namespace_suffix}"
+    queue_name = (
+        f"cdev-queue-{full_namespace_suffix}.fifo"
+        if resource.is_fifo
+        else f"cdev-queue-{full_namespace_suffix}"
+    )
 
     if resource.is_fifo:
         attributes.update({"FifoQueue": str(resource.is_fifo)})
 
-    output_task.update(comment=f'Creating Queue {queue_name}')
+    output_task.update(comment=f"Creating Queue {queue_name}")
 
     rv = aws_client.run_client_function(
         "sqs",
         "create_queue",
-        {
-            "QueueName": queue_name, 
-            "Attributes": attributes
-        },
+        {"QueueName": queue_name, "Attributes": attributes},
     )
 
-   
     output_info = {
         "queue_name": queue_name,
         "cdev_name": resource.name,
         "queue_url": rv.get("QueueUrl"),
     }
 
     # rv does not contain the arn of the queue so we need a second call
@@ -57,66 +58,57 @@
         }
     )
 
     return output_info
 
 
 def _update_simple_queue(
-    transaction_token: str, 
+    transaction_token: str,
     namespace_token: str,
     previous_resource: queue.queue_model,
     new_resource: queue.queue_model,
     previous_output: Dict,
-    output_task: OutputTask
+    output_task: OutputTask,
 ) -> Dict:
     _remove_simple_queue(transaction_token, previous_output, output_task)
-    new_info = _create_simple_queue(transaction_token, namespace_token, new_resource, output_task)
+    new_info = _create_simple_queue(
+        transaction_token, namespace_token, new_resource, output_task
+    )
     return new_info
 
 
 def _remove_simple_queue(
     transaction_token: str, previous_output: Dict, output_task: OutputTask
-):
+) -> None:
     queue_url = previous_output.get("queue_url")
 
-    output_task.update(comment=f'Deleting Queue')
+    output_task.update(comment=f"Deleting Queue")
 
-    aws_client.run_client_function(
-        "sqs", 
-        "delete_queue",
-        {"QueueUrl": queue_url}
-    )
+    aws_client.run_client_function("sqs", "delete_queue", {"QueueUrl": queue_url})
 
 
 def handle_simple_queue_deployment(
-        transaction_token: str, 
-        namespace_token: str, 
-        resource_diff: Resource_Difference, 
-        previous_output: Dict[str, Any],
-        output_task: OutputTask
-    ) -> Dict:
+    transaction_token: str,
+    namespace_token: str,
+    resource_diff: Resource_Difference,
+    previous_output: Dict[str, Any],
+    output_task: OutputTask,
+) -> Dict:
     if resource_diff.action_type == Resource_Change_Type.CREATE:
         return _create_simple_queue(
-            transaction_token,
-            namespace_token,
-            resource_diff.new_resource,
-            output_task
+            transaction_token, namespace_token, resource_diff.new_resource, output_task
         )
-        
+
     elif resource_diff.action_type == Resource_Change_Type.UPDATE_IDENTITY:
         return _update_simple_queue(
             transaction_token,
             namespace_token,
             queue.queue_model(**resource_diff.previous_resource.dict()),
             resource_diff.new_resource,
             previous_output,
-            output_task
+            output_task,
         )
 
     elif resource_diff.action_type == Resource_Change_Type.DELETE:
-        _remove_simple_queue(
-            transaction_token,
-            previous_output,
-            output_task
-        )
+        _remove_simple_queue(transaction_token, previous_output, output_task)
 
         return {}
```

### Comparing `cdev-0.0.8/core/default/mappers/simple/relational_db_deployer.py` & `cdev-0.0.9/core/default/mappers/simple/relational_db_deployer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 import boto3
 import json
-from typing import Any, Dict, List
+from typing import Any, Dict
 from uuid import uuid4
 
 from core.constructs.resource import Resource_Difference, Resource_Change_Type
-from core.default.resources.simple import relational_db 
+from core.default.resources.simple import relational_db
 from core.constructs.output_manager import OutputTask
 from core.utils import hasher
 
 from .. import aws_client
 
 
-
 RUUID = "cdev::simple::relationaldb"
 
 
 def _create_simple_relational_db(
-    transaction_token: str, 
-    namespace_token: str, 
-    resource:  relational_db.simple_relational_db_model,
-    output_task: OutputTask
-) -> bool:
+    transaction_token: str,
+    namespace_token: str,
+    resource: relational_db.simple_relational_db_model,
+    output_task: OutputTask,
+) -> Dict:
 
     full_namespace_suffix = hasher.hash_list([namespace_token, str(uuid4())])
     cluster_name = f"cdev-relationaldb-{full_namespace_suffix}"
-    
-    output_task.update(comment=f'Creating DB {cluster_name}')
+
+    output_task.update(comment=f"Creating DB {cluster_name}")
 
     rv = aws_client.run_client_function(
         "rds",
         "create_db_cluster",
         {
             "DatabaseName": resource.DatabaseName,
             "DBClusterIdentifier": cluster_name,
             "Engine": resource.Engine.value,
             "MasterUsername": resource.MasterUsername,
             "MasterUserPassword": resource.MasterUserPassword,
             "EnableHttpEndpoint": resource.EnableHttpEndpoint,
             "ScalingConfiguration": {
                 "MinCapacity": resource.MinCapacity,
                 "MaxCapacity": resource.MinCapacity,
-                "AutoPause": resource.SecondsToPause == 0,
+                "AutoPause": resource.SecondsToPause != 0,
                 "SecondsUntilAutoPause": resource.SecondsToPause
                 if not resource.SecondsToPause == 0
                 else 300,
             },
             "EngineMode": "serverless",  # Hard Code for this resource type
         },
     )
 
-    output_task.update(comment=f'Creating Secrets for DB')    
+    output_task.update(comment=f"Creating Secrets for DB")
     # Need to create secret for this information so that it can be used with the data api
     secret_rv = aws_client.run_client_function(
         "secretsmanager",
         "create_secret",
         {
             "Name": f"{cluster_name}-config",
             "SecretString": json.dumps(
@@ -66,55 +65,55 @@
                     "username": resource.MasterUsername,
                     "password": resource.MasterUserPassword,
                 }
             ),
         },
     )
 
-    output_task.update(comment=f'Wating for DB to become available. This might take a minute.')
+    output_task.update(
+        comment=f"Wating for DB to become available. This might take a minute."
+    )
     aws_client.monitor_status(
         boto3.client("rds").describe_db_clusters,
         {
             "DBClusterIdentifier": cluster_name,
         },
         "creating",
         lambda x: x.get("DBClusters")[0].get("Status"),
     )
 
-   
     output_info = {
         "endpoint": rv.get("DBCluster").get("Endpoint"),
         "secret_arn": secret_rv.get("ARN"),
         "cloud_id": rv.get("DBCluster").get("DBClusterArn"),
         "cluster_arn": rv.get("DBCluster").get("DBClusterArn"),
         "cdev_name": resource.name,
-        "cluster_name": cluster_name
+        "cluster_name": cluster_name,
     }
 
     return output_info
 
 
 def _update_simple_relational_db(
-    transaction_token: str, 
+    transaction_token: str,
     previous_resource: relational_db.simple_relational_db_model,
     new_resource: relational_db.simple_relational_db_model,
     previous_output: Dict,
-    output_task: OutputTask
-) -> bool:
+    output_task: OutputTask,
+) -> Dict:
     if not new_resource.Engine.value == previous_resource.Engine:
         raise Exception
 
     if not new_resource.MasterUsername == previous_resource.MasterUsername:
         raise Exception
 
     if not new_resource.DatabaseName == previous_resource.DatabaseName:
         raise Exception
 
-
-    update_args = {"DBClusterIdentifier": previous_output.get('cluster_arn')}
+    update_args = {"DBClusterIdentifier": previous_output.get("cluster_arn")}
 
     scaling_config = {}
 
     update_configuration_secret = False
     if not new_resource.MasterUserPassword == previous_resource.MasterUserPassword:
         update_args["MasterUserPassword"] = new_resource.MasterUserPassword
         update_args["ApplyImmediately"] = True
@@ -134,28 +133,28 @@
         scaling_config["SecondsUntilAutoPause"] = (
             new_resource.SecondsToPause if not new_resource.SecondsToPause == 0 else 300
         )
 
     if scaling_config:
         update_args["ScalingConfiguration"] = scaling_config
 
-    output_task.update(comment=f'Updating DB Configuration')
+    output_task.update(comment=f"Updating DB Configuration")
     aws_client.run_client_function("rds", "modify_db_cluster", update_args)
 
     if update_configuration_secret:
         # Update the password in the secret
         secret_arn = previous_output.get("secret_arn")
 
         current_secret_rv = aws_client.run_client_function(
             "secretsmanager", "get_secret_value", {"SecretId": secret_arn}
         )
 
         current_secret_obj = json.loads(current_secret_rv.get("SecretString"))
 
-        output_task.update(comment=f'Updating DB Secret Configuration')
+        output_task.update(comment=f"Updating DB Secret Configuration")
         aws_client.run_client_function(
             "secretsmanager",
             "put_secret_value",
             {
                 "SecretId": secret_arn,
                 "SecretString": json.dumps(
                     {
@@ -169,73 +168,66 @@
                         "username": current_secret_obj.get("username"),
                         "password": new_resource.MasterUserPassword,
                     }
                 ),
             },
         )
 
-    # None of the updatable values actually effect the output 
+    # None of the updatable values actually effect the output
     return previous_output
 
 
 def _remove_simple_relational_db(
-    transaction_token: str, 
-    previous_output: Dict,
-    output_task: OutputTask
-):
-    cluster_id = previous_output.get('cluster_name')
-
+    transaction_token: str, previous_output: Dict, output_task: OutputTask
+) -> None:
+    cluster_id = previous_output.get("cluster_name")
 
-    output_task.update(comment=f'[blink]Deleting DB. This could take a few minutes[/blink]')
+    output_task.update(
+        comment=f"[blink]Deleting DB. This could take a few minutes[/blink]"
+    )
 
     aws_client.run_client_function(
         "rds",
         "delete_db_cluster",
         {
             "DBClusterIdentifier": cluster_id,
             "SkipFinalSnapshot": True,
         },
     )
 
     # Update the password in the secret
     secret_arn = previous_output.get("secret_arn")
 
-    output_task.update(comment=f'Deleting DB Secret')
+    output_task.update(comment=f"Deleting DB Secret")
 
     aws_client.run_client_function(
         "secretsmanager", "delete_secret", {"SecretId": secret_arn}
     )
 
 
-
 def handle_simple_relational_db_deployment(
-        transaction_token: str, 
-        namespace_token: str, 
-        resource_diff: Resource_Difference, 
-        previous_output: Dict[str, Any],
-        output_task: OutputTask
-    ) -> Dict:
+    transaction_token: str,
+    namespace_token: str,
+    resource_diff: Resource_Difference,
+    previous_output: Dict[str, Any],
+    output_task: OutputTask,
+) -> Dict:
     if resource_diff.action_type == Resource_Change_Type.CREATE:
         return _create_simple_relational_db(
-            transaction_token,
-            namespace_token,
-            resource_diff.new_resource,
-            output_task
+            transaction_token, namespace_token, resource_diff.new_resource, output_task
         )
-        
+
     elif resource_diff.action_type == Resource_Change_Type.UPDATE_IDENTITY:
         return _update_simple_relational_db(
             transaction_token,
-            relational_db.simple_relational_db_model(**resource_diff.previous_resource.dict()),
+            relational_db.simple_relational_db_model(
+                **resource_diff.previous_resource.dict()
+            ),
             resource_diff.new_resource,
             previous_output,
-            output_task
+            output_task,
         )
 
     elif resource_diff.action_type == Resource_Change_Type.DELETE:
-        _remove_simple_relational_db(
-            transaction_token,
-            previous_output,
-            output_task
-        )
+        _remove_simple_relational_db(transaction_token, previous_output, output_task)
 
         return {}
```

### Comparing `cdev-0.0.8/core/default/mappers/simple/role_deployer.py` & `cdev-0.0.9/core/default/mappers/simple/role_deployer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,104 +1,96 @@
 import json
 from typing import FrozenSet, List, Tuple, Union, Dict
 from uuid import uuid4
 
 from core.default.resources.simple.iam import permission_model, permission_arn_model
 
-from .. import aws_client 
+from .. import aws_client
 
 
 def create_role_with_permissions(
     role_name: str,
     permissions: FrozenSet[Union[permission_model, permission_arn_model]],
-    assume_role_policy: str
+    assume_role_policy: str,
 ) -> Tuple[str, List[Dict]]:
     """
     This function creates a new IAM role and policies such that the function will have correct access to resources.
 
     Arguments:
         role_name: Name of the role
         permissions [List[Union[permission_model, permission_arn_model]]]: The permission to assign to the role
-    
+
     Returns:
         str: The arn of the role created
         List[Tuple[str,bool]]: List of Tuple of permission arn and bool to denote if the permission should be destroyed on delete
-    
+
     """
 
     role_arn = _create_role(role_name, assume_role_policy)
-    permission_info: List[Tuple[str, bool]] = []
-
+    permission_info: List[Dict] = []
 
     for permission in permissions:
         permission_info.append(add_policy(role_name, permission))
 
-
     basic_execution_permission_arn = permission_arn_model(
         arn="arn:aws:iam::aws:policy/service-role/AWSLambdaBasicExecutionRole",
-        hash="arn:aws:iam::aws:policy/service-role/AWSLambdaBasicExecutionRole"
+        hash="arn:aws:iam::aws:policy/service-role/AWSLambdaBasicExecutionRole",
     )
 
-    permission_info.append(
-        add_policy(role_name, basic_execution_permission_arn)
-    )
+    permission_info.append(add_policy(role_name, basic_execution_permission_arn))
 
-    return (role_arn, permission_info)
+    return role_arn, permission_info
 
 
-def delete_role_and_permissions(
-    role_name: str, permission_arns: List[Dict]
-):
+def delete_role_and_permissions(role_name: str, permission_arns: List[Dict]) -> None:
     """
     Delete all permissions and the associated role
     """
     for info in permission_arns:
         delete_policy(role_name, info)
 
     aws_client.run_client_function("iam", "delete_role", {"RoleName": role_name})
 
 
-
-
-def delete_policy(role_name: str, permission_info: Dict):
+def delete_policy(role_name: str, permission_info: Dict) -> None:
     """
     Delete a policy
     """
-    detach_policy(role_name, permission_info.get('arn'))
+    detach_policy(role_name, permission_info.get("arn"))
 
-    if permission_info.get('was_created'):
+    if permission_info.get("was_created"):
         aws_client.run_client_function(
-            "iam", "delete_policy", {"PolicyArn": permission_info.get('arn')}
+            "iam", "delete_policy", {"PolicyArn": permission_info.get("arn")}
         )
 
 
 def add_policy(
-    role_name: str,
-    permission: Union[permission_model, permission_arn_model]
+    role_name: str, permission: Union[permission_model, permission_arn_model]
 ) -> Dict:
     """
     Creates a policy if needed and then adds the policy to the given role
     """
     if isinstance(permission, permission_arn_model):
         # Already deployed policy so just append arn
         returned_permission_arn = permission.arn
         was_created = False
-        
+
     else:
         returned_permission_arn = create_policy(permission)
         was_created = True
-        
+
     _attach_policy_to_arn(role_name, returned_permission_arn)
 
     return {
         "hash": permission.hash,
         "arn": returned_permission_arn,
-        "was_created": was_created
+        "was_created": was_created,
     }
 
+
 def create_policy(permission: permission_model) -> str:
     """
     Creates the policy and returns the arn
     """
 
     policy = {
         "Version": "2012-10-17",
@@ -110,57 +102,42 @@
     policy["Statement"] = [statement]
 
     permission_name = str(uuid4())
 
     rv = aws_client.run_client_function(
         "iam",
         "create_policy",
-        {
-            "PolicyName": permission_name, 
-            "PolicyDocument": json.dumps(policy)
-        },
+        {"PolicyName": permission_name, "PolicyDocument": json.dumps(policy)},
     )
 
     return rv.get("Policy").get("Arn")
 
 
-def detach_policy(role_name: str, permission_arn: str):
+def detach_policy(role_name: str, permission_arn: str) -> None:
     aws_client.run_client_function(
         "iam",
         "detach_role_policy",
-        {
-            "RoleName": role_name, 
-            "PolicyArn": permission_arn
-        },
+        {"RoleName": role_name, "PolicyArn": permission_arn},
     )
 
 
 def _create_role(name: str, assume_role_policy: str) -> str:
     """
     Creates the role and returns the arn
     """
-    
+
     rv = aws_client.run_client_function(
         "iam",
         "create_role",
         {
             "RoleName": name,
             "AssumeRolePolicyDocument": assume_role_policy,
         },
     )
 
     return rv.get("Role").get("Arn")
 
 
-def _attach_policy_to_arn(role_arn: str, policy_arn: str) -> bool:   
+def _attach_policy_to_arn(role_arn: str, policy_arn: str) -> None:
     aws_client.run_client_function(
-        "iam", 
-        "attach_role_policy", 
-        {
-            "RoleName": role_arn, 
-            "PolicyArn": policy_arn
-        }
+        "iam", "attach_role_policy", {"RoleName": role_arn, "PolicyArn": policy_arn}
     )
-
-
-
-
```

### Comparing `cdev-0.0.8/core/default/mappers/simple/static_site_deployer.py` & `cdev-0.0.9/core/default/mappers/simple/static_site_deployer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,42 @@
-import site
+
 import boto3
 import json
-from typing import Any, Dict, List
+from typing import Any, Dict
 from uuid import uuid4
 
 from core.constructs.resource import Resource_Difference, Resource_Change_Type
 from core.default.resources.simple import static_site
 from core.constructs.output_manager import OutputTask
 from core.utils import hasher
 
 
 from .. import aws_client
 
 
 def _create_simple_static_site(
-    transaction_token: str, 
-    namespace_token: str, 
-    resource:  static_site.simple_static_site_model,
-    output_task: OutputTask
+    transaction_token: str,
+    namespace_token: str,
+    resource: static_site.simple_static_site_model,
+    output_task: OutputTask,
 ) -> Dict:
 
-    
     full_namespace_suffix = hasher.hash_list([namespace_token, str(uuid4())])
 
     if not resource.domain_name:
-        site_name = f"cdev-staticsite-{full_namespace_suffix}" 
+        site_name = f"cdev-staticsite-{full_namespace_suffix}"
     else:
         site_name = resource.domain_name
 
-    output_task.update(comment=f'Creating Bucket')
+    output_task.update(comment=f"Creating Bucket")
     aws_client.run_client_function(
         "s3", "create_bucket", {"Bucket": site_name, "ACL": "public-read"}
     )
-   
-    output_task.update(comment=f'Add read object policy')
+
+    output_task.update(comment=f"Add read object policy")
     aws_client.run_client_function(
         "s3",
         "put_bucket_policy",
         {
             "Bucket": site_name,
             "Policy": json.dumps(
                 {
@@ -52,15 +51,15 @@
                         }
                     ],
                 }
             ),
         },
     )
 
-    output_task.update(comment=f'Set Website Configuration')
+    output_task.update(comment=f"Set Website Configuration")
     aws_client.run_client_function(
         "s3",
         "put_bucket_website",
         {
             "Bucket": site_name,
             "WebsiteConfiguration": {
                 "ErrorDocument": {"Key": resource.error_document},
@@ -68,303 +67,275 @@
             },
         },
     )
 
     ####################################
     ##### Distribution on CloudFront
     ####################################
-    
+
     domain_name = f"{site_name}.s3-website-us-east-1.amazonaws.com"
-        
+
     # https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/using-managed-cache-policies.html#managed-cache-policies-list
     # Disabled cache policy
-    cache_policy_id = '4135ea2d-6df8-44a3-9df3-4b5a84be39ad'
+    cache_policy_id = "4135ea2d-6df8-44a3-9df3-4b5a84be39ad"
 
     args = {
         "CallerReference": str(uuid4()),
-         
-        "Enabled":True,
+        "Enabled": True,
         "Origins": {
-            "Quantity": 1, 
+            "Quantity": 1,
             "Items": [
                 {
                     "Id": domain_name,
                     "DomainName": domain_name,
                     "CustomOriginConfig": {
-                        'HTTPPort': 80,
-                        'HTTPSPort': 443,
-                        'OriginProtocolPolicy': 'http-only',
-                        'OriginSslProtocols': {'Quantity': 3, 'Items': ['TLSv1', 'TLSv1.1', 'TLSv1.2']},
-                        'OriginReadTimeout': 30,
-                        'OriginKeepaliveTimeout': 5
+                        "HTTPPort": 80,
+                        "HTTPSPort": 443,
+                        "OriginProtocolPolicy": "http-only",
+                        "OriginSslProtocols": {
+                            "Quantity": 3,
+                            "Items": ["TLSv1", "TLSv1.1", "TLSv1.2"],
+                        },
+                        "OriginReadTimeout": 30,
+                        "OriginKeepaliveTimeout": 5,
                     },
                 }
-            ]
+            ],
         },
-        "DefaultCacheBehavior" : {
+        "DefaultCacheBehavior": {
             "TargetOriginId": domain_name,
-            "ViewerProtocolPolicy": 'redirect-to-https',
+            "ViewerProtocolPolicy": "redirect-to-https",
             "TrustedSigners": dict(Quantity=0, Enabled=False),
             "AllowedMethods": {
-                'Quantity': 2, 
-                'Items': ['HEAD', 'GET'], 
-                'CachedMethods': {
-                    'Quantity': 2, 
-                    'Items': ['HEAD', 'GET']
-                    }
-                },
-            "CachePolicyId": cache_policy_id 
-        },        
-        "CacheBehaviors": {'Quantity': 0},
-        "Comment":"cdev generated",
+                "Quantity": 2,
+                "Items": ["HEAD", "GET"],
+                "CachedMethods": {"Quantity": 2, "Items": ["HEAD", "GET"]},
+            },
+            "CachePolicyId": cache_policy_id,
+        },
+        "CacheBehaviors": {"Quantity": 0},
+        "Comment": "cdev generated",
         "ViewerCertificate": {
             "CloudFrontDefaultCertificate": True,
-        }
+        },
     }
 
     if resource.domain_name:
-        aliases = {
-            'Aliases': {
-                "Quantity": 1,
-                "Items": [resource.domain_name]
-            }
-            
-        }
+        aliases = {"Aliases": {"Quantity": 1, "Items": [resource.domain_name]}}
 
         args.update(aliases)
 
-
     if resource.ssl_certificate_arn:
         ssl_args = {
-            'ViewerCertificate': {
-                'CloudFrontDefaultCertificate': False,
-                'SSLSupportMethod': 'sni-only',
-                'MinimumProtocolVersion': 'TLSv1.2_2021',
-                'ACMCertificateArn': resource.ssl_certificate_arn
+            "ViewerCertificate": {
+                "CloudFrontDefaultCertificate": False,
+                "SSLSupportMethod": "sni-only",
+                "MinimumProtocolVersion": "TLSv1.2_2021",
+                "ACMCertificateArn": resource.ssl_certificate_arn,
             }
         }
 
         args.update(ssl_args)
 
+    final_args = {"DistributionConfig": args}
 
-    final_args = {
-        'DistributionConfig': args
-    }
+    output_task.update(
+        comment=f"[blink]Creating on the Aws Cloudfront CDN. This will take a few minutes[/blink]"
+    )
 
-    output_task.update(comment=f'[blink]Creating on the Aws Cloudfront CDN. This will take a few minutes[/blink]')
-    
-    rv = aws_client.run_client_function('cloudfront', "create_distribution", final_args)
+    rv = aws_client.run_client_function("cloudfront", "create_distribution", final_args)
 
     cloudfront_id = rv.get("Distribution").get("Id")
     cloudfront_arn = rv.get("Distribution").get("ARN")
     cloudfront_domain = rv.get("Distribution").get("DomainName")
 
     aws_client.monitor_status(
         boto3.client("cloudfront").get_distribution,
         {
             "Id": cloudfront_id,
         },
         "InProgress",
         lambda x: x.get("Distribution").get("Status"),
     )
 
-
     output_info = {
         "cloud_id": cloudfront_arn,
         "bucket_name": site_name,
         "cloudfront_id": cloudfront_id,
         "cloudfront_arn": cloudfront_arn,
-        "site_url": cloudfront_domain
+        "site_url": cloudfront_domain,
     }
 
-   
-    #if resource.sync_folder:
+    # if resource.sync_folder:
     #    output_task.update(comment=f'Sync Files')
     #    file_syncer = sync_files()
     #    file_syncer.command(
     #        **{"resource_name": resource.name, "dir": resource.content_folder}
     #    )
 
-
     return output_info
 
 
 def _update_simple_static_site(
-    transaction_token: str, 
+    transaction_token: str,
     namespace_token: str,
     previous_resource: static_site.simple_static_site_model,
     new_resource: static_site.simple_static_site_model,
     previous_output: Dict,
-    output_task: OutputTask
-) -> bool:
+    output_task: OutputTask,
+) -> Dict:
 
     if not previous_resource.domain_name == new_resource.domain_name:
-        raise Exception("Can not update 'domain_name' via an in place update. You must destroy this version and make a new static site resource.")
-
+        raise Exception(
+            "Can not update 'domain_name' via an in place update. You must destroy this version and make a new static site resource."
+        )
 
     if not previous_resource.ssl_certificate_arn == new_resource.ssl_certificate_arn:
-        raise Exception("Can not update 'ssl_certificate_arn' via an in place update. You must destroy this version and make a new static site resource.")
-
-
+        raise Exception(
+            "Can not update 'ssl_certificate_arn' via an in place update. You must destroy this version and make a new static site resource."
+        )
 
-    bucket_name = previous_output.get('bucket_name')
+    bucket_name = previous_output.get("bucket_name")
 
     if not previous_resource.index_document == new_resource.index_document:
         aws_client.run_client_function(
             "s3",
             "put_bucket_website",
             {
                 "Bucket": bucket_name,
                 "WebsiteConfiguration": {
                     "ErrorDocument": {"Key": new_resource.error_document},
                     "IndexDocument": {"Suffix": new_resource.index_document},
                 },
             },
         )
 
-
-
     if not previous_resource.error_document == new_resource.error_document:
         aws_client.run_client_function(
             "s3",
             "put_bucket_website",
             {
                 "Bucket": bucket_name,
                 "WebsiteConfiguration": {
                     "ErrorDocument": {"Key": new_resource.error_document},
                     "IndexDocument": {"Suffix": new_resource.index_document},
                 },
             },
         )
 
-
     if not previous_resource.sync_folder == new_resource.sync_folder:
         # If there has been a change in sync from false to true then sync the new directory
-        #if new_resource.sync_folder:
+        # if new_resource.sync_folder:
         #    output_task.update(comment=f'Syncing Files')
-        #    
+        #
         #    file_syncer = sync_files()
         #    file_syncer.command(
         #        **{
         #            "resource_name": new_resource.name,
         #            "dir": new_resource.content_folder,
         #        }
         #    )
-            
-        #else:
+
+        # else:
         #    output_task.update(comment=f'Disbled Sync Files')
         pass
 
-
-    #elif not previous_resource.content_folder == new_resource.content_folder:
+    # elif not previous_resource.content_folder == new_resource.content_folder:
     #    output_task.update(comment=f'Sync Files')
-#
+    #
     #    # If there was not change to sync but there is a change to the content folder. Clear the bucket and sync new folder
     #    s3 = boto3.resource("s3")
     #    bucket = s3.Bucket(site_name)
     #    bucket.object_versions.delete()
-    #   
+    #
     #    file_syncer = sync_files()
     #    file_syncer.command(
     #        **{"resource_name": new_resource.name, "dir": new_resource.content_folder}
     #    )
-    #    
+    #
 
     # No changes affect the actual cloud output
     return previous_output
 
+
 def _remove_simple_static_site(
-    transaction_token: str, 
-    previous_output: Dict, 
-    output_task: OutputTask
-):
-    previous_cloudfront_id = previous_output.get('cloudfront_id')
+    transaction_token: str, previous_output: Dict, output_task: OutputTask
+) -> None:
+    previous_cloudfront_id = previous_output.get("cloudfront_id")
 
-    all_info = aws_client.run_client_function("cloudfront", "get_distribution", 
-        {
-            "Id": previous_cloudfront_id
-        }
+    all_info = aws_client.run_client_function(
+        "cloudfront", "get_distribution", {"Id": previous_cloudfront_id}
     )
 
-
-    current_distribution_info = all_info.get('Distribution').get('DistributionConfig')
+    current_distribution_info = all_info.get("Distribution").get("DistributionConfig")
     e_tag = all_info.get("ETag")
 
-    current_distribution_info['Enabled'] = False
+    current_distribution_info["Enabled"] = False
 
     final_args = {
         "DistributionConfig": current_distribution_info,
         "Id": previous_cloudfront_id,
-        "IfMatch": e_tag
-
+        "IfMatch": e_tag,
     }
 
     # Disable the distribution
-    new_info =  aws_client.run_client_function("cloudfront", "update_distribution", final_args)
+    new_info = aws_client.run_client_function(
+        "cloudfront", "update_distribution", final_args
+    )
     new_etag = new_info.get("ETag")
 
-    output_task.update(comment='[blink]Disabling site on Aws Cloudfront CDN.This will take a few minutes[/blink]')
+    output_task.update(
+        comment="[blink]Disabling site on Aws Cloudfront CDN.This will take a few minutes[/blink]"
+    )
     aws_client.monitor_status(
         boto3.client("cloudfront").get_distribution,
-        {
-            "Id": previous_cloudfront_id
-        },
+        {"Id": previous_cloudfront_id},
         "InProgress",
         lambda x: x.get("Distribution").get("Status"),
     )
 
-
-    output_task.update(comment='Deleting site from Aws Cloudfront CDN')
-    aws_client.run_client_function("cloudfront", "delete_distribution",
-        {
-            "Id": previous_cloudfront_id,
-            "IfMatch": new_etag
-        }
+    output_task.update(comment="Deleting site from Aws Cloudfront CDN")
+    aws_client.run_client_function(
+        "cloudfront",
+        "delete_distribution",
+        {"Id": previous_cloudfront_id, "IfMatch": new_etag},
     )
 
-    bucket_name = previous_output.get('bucket_name')
+    bucket_name = previous_output.get("bucket_name")
 
     s3 = boto3.resource("s3")
     bucket = s3.Bucket(bucket_name)
-    output_task.update(comment='Deleting all items in the bucket')
+    output_task.update(comment="Deleting all items in the bucket")
     bucket.object_versions.delete()
 
-    output_task.update(comment='Deleting bucket')
-    aws_client.run_client_function(
-        "s3", "delete_bucket", {"Bucket": bucket_name}
-    )
-
+    output_task.update(comment="Deleting bucket")
+    aws_client.run_client_function("s3", "delete_bucket", {"Bucket": bucket_name})
 
 
 def handle_simple_static_site_deployment(
-        transaction_token: str, 
-        namespace_token: str, 
-        resource_diff: Resource_Difference, 
-        previous_output: Dict[str, Any],
-        output_task: OutputTask
-    ) -> Dict:
+    transaction_token: str,
+    namespace_token: str,
+    resource_diff: Resource_Difference,
+    previous_output: Dict[str, Any],
+    output_task: OutputTask,
+) -> Dict:
     if resource_diff.action_type == Resource_Change_Type.CREATE:
         return _create_simple_static_site(
-            transaction_token,
-            namespace_token,
-            resource_diff.new_resource,
-            output_task
+            transaction_token, namespace_token, resource_diff.new_resource, output_task
         )
-        
+
     elif resource_diff.action_type == Resource_Change_Type.UPDATE_IDENTITY:
         return _update_simple_static_site(
             transaction_token,
             namespace_token,
-            static_site.simple_static_site_model(**resource_diff.previous_resource.dict()),
+            static_site.simple_static_site_model(
+                **resource_diff.previous_resource.dict()
+            ),
             resource_diff.new_resource,
             previous_output,
-            output_task
+            output_task,
         )
 
     elif resource_diff.action_type == Resource_Change_Type.DELETE:
-        _remove_simple_static_site(
-            transaction_token,
-            previous_output,
-            output_task
-        )
+        _remove_simple_static_site(transaction_token, previous_output, output_task)
 
         return {}
```

### Comparing `cdev-0.0.8/core/default/mappers/simple/topic_deployer.py` & `cdev-0.0.9/core/default/mappers/simple/topic_deployer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,72 @@
-from typing import Any, Dict, List
+from typing import Any, Dict
 from uuid import uuid4
 
 from core.constructs.resource import Resource_Difference, Resource_Change_Type
-from core.default.resources.simple import topic 
+from core.default.resources.simple import topic
 from core.constructs.output_manager import OutputTask
 from core.utils import hasher
 
 from .. import aws_client
 
+
 def _create_simple_topic(
-    transaction_token: str, 
-    namespace_token: str, 
-    resource:  topic.simple_topic_model,
-    output_task: OutputTask
+    transaction_token: str,
+    namespace_token: str,
+    resource: topic.simple_topic_model,
+    output_task: OutputTask,
 ) -> Dict:
 
     attributes = {}
 
     full_namespace_suffix = hasher.hash_list([namespace_token, str(uuid4())])
 
-    topic_name = f"cdev-topic-{full_namespace_suffix}.fifo" if resource.is_fifo else f"cdev-topic-{full_namespace_suffix}"
+    topic_name = (
+        f"cdev-topic-{full_namespace_suffix}.fifo"
+        if resource.is_fifo
+        else f"cdev-topic-{full_namespace_suffix}"
+    )
 
     if resource.is_fifo:
         attributes.update({"FifoTopic": str(resource.is_fifo)})
 
-    output_task.update(comment=f'Creating Topic {topic_name}')
+    output_task.update(comment=f"Creating Topic {topic_name}")
 
     rv = aws_client.run_client_function(
         "sns", "create_topic", {"Name": topic_name, "Attributes": attributes}
     )
-    
+
     output_info = {
         "topic_name": topic_name,
         "cdev_name": resource.name,
         "arn": rv.get("TopicArn"),
         "cloud_id": rv.get("TopicArn"),
     }
 
-   
     return output_info
 
 
 def _update_simple_topic(
-    transaction_token: str, 
+    transaction_token: str,
     namespace_token: str,
     previous_resource: topic.simple_topic_model,
     new_resource: topic.simple_topic_model,
     previous_output: Dict,
-    output_task: OutputTask
+    output_task: OutputTask,
 ) -> Dict:
     _remove_simple_topic(transaction_token, previous_output, output_task)
-    new_rv = _create_simple_topic(transaction_token, namespace_token, new_resource, output_task)
+    new_rv = _create_simple_topic(
+        transaction_token, namespace_token, new_resource, output_task
+    )
     return new_rv
 
 
 def _remove_simple_topic(
     transaction_token: str, previous_output: Dict, output_task: OutputTask
-):
+) -> None:
     topic_arn = previous_output.get("cloud_id")
 
     aws_client.run_client_function("sns", "delete_topic", {"TopicArn": topic_arn})
 
 
 def add_subscriber(topic_arn: str, protocol: str, endpoint: str) -> str:
     rv = aws_client.run_client_function(
@@ -73,46 +79,39 @@
             "ReturnSubscriptionArn": True,
         },
     )
 
     return rv.get("SubscriptionArn")
 
 
-def remove_subscriber(subscription_arn: str):
+def remove_subscriber(subscription_arn: str) -> None:
     rv = aws_client.run_client_function(
         "sns", "unsubscribe", {"SubscriptionArn": subscription_arn}
     )
 
 
 def handle_simple_topic_deployment(
-        transaction_token: str, 
-        namespace_token: str, 
-        resource_diff: Resource_Difference, 
-        previous_output: Dict[str, Any],
-        output_task: OutputTask
-    ) -> Dict:
+    transaction_token: str,
+    namespace_token: str,
+    resource_diff: Resource_Difference,
+    previous_output: Dict[str, Any],
+    output_task: OutputTask,
+) -> Dict:
     if resource_diff.action_type == Resource_Change_Type.CREATE:
         return _create_simple_topic(
-            transaction_token,
-            namespace_token,
-            resource_diff.new_resource,
-            output_task
+            transaction_token, namespace_token, resource_diff.new_resource, output_task
         )
-        
+
     elif resource_diff.action_type == Resource_Change_Type.UPDATE_IDENTITY:
         return _update_simple_topic(
             transaction_token,
             namespace_token,
             topic.simple_topic_model(**resource_diff.previous_resource.dict()),
             resource_diff.new_resource,
             previous_output,
-            output_task
+            output_task,
         )
 
     elif resource_diff.action_type == Resource_Change_Type.DELETE:
-        _remove_simple_topic(
-            transaction_token,
-            previous_output,
-            output_task
-        )
+        _remove_simple_topic(transaction_token, previous_output, output_task)
 
         return {}
```

### Comparing `cdev-0.0.8/core/default/resources/simple/api.py` & `cdev-0.0.9/core/default/resources/simple/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,290 +1,316 @@
 """Set of constructs for creating HTTP APIs
 
 """
 from enum import Enum
 from typing import Any, Dict, FrozenSet, List, Optional
 
 from core.constructs.models import ImmutableModel
-from core.constructs.cloud_output import Cloud_Output_Mapping, Cloud_Output_Sequence, Cloud_Output_Str, OutputType
-
-from core.constructs.resource import Resource, ResourceModel, update_hash, ResourceOutputs
+from core.constructs.cloud_output import (
+    Cloud_Output_Mapping,
+    Cloud_Output_Sequence,
+    Cloud_Output_Str,
+    OutputType,
+)
+
+from core.constructs.resource import (
+    Resource,
+    ResourceModel,
+    update_hash,
+    ResourceOutputs,
+)
 from core.constructs.types import cdev_str_model
 from core.utils import hasher
 
 from core.default.resources.simple import events
 
 
 RUUID = "cdev::simple::api"
 
 ########################
 ##### Authorizer
 ########################
 
+
 class authorizer_model(ImmutableModel):
     """Model representing JWT authorizer information"""
+
     name: str
     issuer_url: str
     audience: str
 
 
-class Authorizer():
+class Authorizer:
     def __init__(self, name: str, issuer_url: str, audience: str) -> None:
         """JWT authorizer information.
 
-        Deployed Apis can validates the JWTs that clients submit with API requests to allow or deny 
+        Deployed Apis can validates the JWTs that clients submit with API requests to allow or deny
         requests based on token validation, and optionally, scopes in the token. You can provide authorization
-        from OpenID Connect (OIDC) and OAuth 2.0 frameworks. 
+        from OpenID Connect (OIDC) and OAuth 2.0 frameworks.
 
-        For examples on how to integrate with service like Auth0 visit our 
+        For examples on how to integrate with service like Auth0 visit our
         <a href="/docs/examples/user-authentication"> documentation </a>.
 
 
         Args:
             name (str): Name of the authorizer. Used as a unique identifier within the attached Api.
             issuer_url (str): The base domain of the identity provider that issues JSON Web Tokens.
             audience (str): The intended recipients of the JWT. A valid JWT must provide an aud that matches at this value.
         """
         self.name = name
         self.issuer_url = issuer_url
         self.audience = audience
 
-
     def render(self) -> authorizer_model:
         return authorizer_model(
             name=self.name,
             issuer_url=self.issuer_url,
             audience=self.audience,
         )
 
     def hash(self) -> str:
-        return hasher.hash_list([
-            self.name,
-            self.issuer_url,
-            self.audience
-        ])
-
+        return hasher.hash_list([self.name, self.issuer_url, self.audience])
 
 
 ########################
 ##### Route
 ########################
-class route_verb(str,Enum):
+class route_verb(str, Enum):
     """Route Verbs"""
+
     GET = "GET"
     PUT = "PUT"
     POST = "POST"
     DELETE = "DELETE"
     ANY = "ANY"
 
 
 class route_model(ImmutableModel):
     """Model to represent a route of an API"""
+
     path: str
     verb: str
     additional_scopes: Optional[FrozenSet[str]]
     authorizer_name: Optional[str]
 
     def __init__(__pydantic_self__, **data: Any) -> None:
         """"""
         super().__init__(**data)
 
 
-class Route():
-    def __init__(self, api_name: str, path: str, verb: route_verb, authorizer_name: str = None, additional_scopes: List[str] = []) -> None:
-        """Construct for representing a route that is apart of an HTTP API 
+class Route:
+    def __init__(
+        self,
+        api_name: str,
+        path: str,
+        verb: route_verb,
+        authorizer_name: str = None,
+        additional_scopes: List[str] = [],
+    ) -> None:
+        """Construct for representing a route that is apart of an HTTP API
 
         Args:
             api_name (str): Cdev name of the API this route is apart of
             path (str): Path of the route.
             verb (route_verb): Verb that this route handles
             authorizer_name (str): The `name` of the authorizer to use for this route.
             additional_scopes (List[str]): Set of scopes that must be present in an authorization JWT.
         """
         self.api_name = api_name
         self.path = path
         self.verb = verb
         self.authorizer_name = authorizer_name
         self.additional_scopes = additional_scopes
-       
+
     def hash(self) -> str:
-        return hasher.hash_list([
-            self.path,
-            self.verb,
-            hasher.hash_list(self.additional_scopes),
-            self.authorizer_name,
-        ])
+        return hasher.hash_list(
+            [
+                self.path,
+                self.verb,
+                hasher.hash_list(self.additional_scopes),
+                self.authorizer_name,
+            ]
+        )
 
     def render(self) -> route_model:
         return route_model(
             path=self.path,
             verb=self.verb,
             additional_scopes=frozenset(self.additional_scopes),
             authorizer_name=self.authorizer_name,
         )
 
-    def event(self, response_type: Optional[str]="") -> 'RouteEvent':
-        """Generate an Event Construct that other resources can bind to. 
+    def event(self, response_type: Optional[str] = "") -> "RouteEvent":
+        """Generate an Event Construct that other resources can bind to.
 
         Returns:
             `RouteEvent`
         """
         return RouteEvent(
             resource_name=self.api_name,
             path=self.path,
             verb=self.verb,
-            response_type=response_type
+            response_type=response_type,
         )
 
+
 class route_event_model(events.event_model):
     """Model to represent an event for a given route"""
+
     path: str
     verb: route_verb
     api_id: cdev_str_model
     route_id: cdev_str_model
     response_type: Optional[str]
 
     def __init__(__pydantic_self__, **data: Any) -> None:
         """"""
         super().__init__(**data)
 
 
-class RouteEvent():
+class RouteEvent:
     """Construct for representing a route that is apart of an HTTP API."""
 
-    def __init__(self, resource_name: str, path: str, verb: route_verb, response_type: Optional[str]="") -> None:
+    def __init__(
+        self,
+        resource_name: str,
+        path: str,
+        verb: route_verb,
+        response_type: Optional[str] = "",
+    ) -> None:
         """
         Args:
             resource_name (str): Cdev Name of the API this event is generated from
             path (str): Path of the route
             verb (`route_verb`): Verb of the route
 
         This construct should be generated with the `Route.event` method.
         """
         self.resource_name = resource_name
         self.path = path
         self.verb = verb
         self.api_id = Cloud_Output_Str(
-                name=resource_name, 
-                ruuid=RUUID, 
-                key='cloud_id',
-                type=OutputType.RESOURCE 
-            )
+            name=resource_name, ruuid=RUUID, key="cloud_id", type=OutputType.RESOURCE
+        )
         self.route_id = Cloud_Output_Mapping[Cloud_Output_Str](
-                name=resource_name, 
-                ruuid=RUUID, 
-                key='endpoints',
-                type=OutputType.RESOURCE,
-                _member_class=Cloud_Output_Str
-            )[f'{self.path} {self.verb}']
+            name=resource_name,
+            ruuid=RUUID,
+            key="endpoints",
+            type=OutputType.RESOURCE,
+            _member_class=Cloud_Output_Str,
+        )[f"{self.path} {self.verb}"]
 
         self.response_type = response_type
 
     def hash(self) -> str:
-        return hasher.hash_list([self.resource_name, self.path, self.verb, self.response_type])
+        return hasher.hash_list(
+            [self.resource_name, self.path, self.verb, self.response_type]
+        )
 
     def render(self) -> route_event_model:
         return route_event_model(
             originating_resource_name=self.resource_name,
             originating_resource_type=RUUID,
             hash=self.hash(),
             path=self.path,
             verb=self.verb,
             api_id=self.api_id.render(),
             route_id=self.route_id.render(),
-            response_type=self.response_type
+            response_type=self.response_type,
         )
 
+
 ########################
 ##### Output
 ########################
 class ApiOutput(ResourceOutputs):
     """Container object for the returned values from the cloud after an API has been deployed."""
+
     def __init__(self, name: str) -> None:
         super().__init__(name, RUUID)
-    
+
     @property
     def endpoint(self) -> Cloud_Output_Str:
         """The base url for the created API
 
         Returns:
             `core.constructs.cloud_output.Cloud_Output_Str`
         """
         return Cloud_Output_Str(
-            name=self._name,
-            ruuid=RUUID,
-            key='endpoint',
-            type=self.OUTPUT_TYPE
+            name=self._name, ruuid=RUUID, key="endpoint", type=self.OUTPUT_TYPE
         )
 
     @endpoint.setter
-    def endpoint(self, value: Any):
+    def endpoint(self, value: Any) -> None:
         raise Exception
 
-
     @property
     def endpoints(self) -> Cloud_Output_Mapping[Cloud_Output_Str]:
         """The created routes for the API.
 
-        Values are stored as a mapping of the (path,verb) to cloud route_id.  
-        
+        Values are stored as a mapping of the (path,verb) to cloud route_id.
+
         ex:
         ```
             {
                 '/hello_world [GET]': <route_id>
             }
         ```
 
         Returns:
             `core.constructs.cloud_output.Cloud_Output_Mapping`
         """
         return Cloud_Output_Mapping[Cloud_Output_Str](
             name=self._name,
             ruuid=RUUID,
-            key='endpoints',
+            key="endpoints",
             type=self.OUTPUT_TYPE,
-            _member_class=Cloud_Output_Str
+            _member_class=Cloud_Output_Str,
         )
 
     @endpoints.setter
-    def endpoints(self, value: Any):
+    def endpoints(self, value: Any) -> None:
         raise Exception
 
 
 ########################
 ##### Api
 ########################
 class simple_api_model(ResourceModel):
     """Model for representing a desired HTTP API"""
-    
+
     routes: FrozenSet[route_model]
     allow_cors: bool
     authorizers: Optional[FrozenSet[authorizer_model]]
 
     def __init__(self, **data: Any) -> None:
         """"""
         super().__init__(**data)
 
 
 class Api(Resource):
-
     @update_hash
     def __init__(
-        self, cdev_name: str, allow_cors: bool = True, authorizers: List[Authorizer] = [], default_authorizer: str= None, nonce: str = "",
+        self,
+        cdev_name: str,
+        allow_cors: bool = True,
+        authorizers: List[Authorizer] = [],
+        default_authorizer: str = None,
+        nonce: str = "",
     ):
         """Create a HTTP API.
 
         Args:
             cdev_name (str): Name for the resource.
             allow_cors (bool): Allow Cross Origin Resource Sharing (CORS) on the api.
-            authorizers (List[Authorizer]): List of JWT Authorizers for the api. 
-            default_authorizer (str): The name of an authorizer to add as the default to all routes. 
+            authorizers (List[Authorizer]): List of JWT Authorizers for the api.
+            default_authorizer (str): The name of an authorizer to add as the default to all routes.
             nonce (str): Nonce to make the resource hash unique if there are conflicting resources with same configuration.
 
-        With an HTTP API, you can create different routes that represent different requests to your backend service. Use the 
+        With an HTTP API, you can create different routes that represent different requests to your backend service. Use the
         `route` method to create these routes then attach them to other resource to handle the requests.
 
         HTTP Api's can take an authorizer to support JWT authorization for the Api. You can provide a default authorizer to the Api to apply
         to all created routes, or individually set the authorizer for each route.
 
         <a href="https://code.tutsplus.com/tutorials/a-beginners-guide-to-http-and-rest--net-16340"> More information on HTTP routes</a>
 
@@ -292,25 +318,24 @@
 
         <a href="https://docs.aws.amazon.com/apigatewayv2/latest/api-reference/api-reference.html"> Documentation on Deployed Resource in the Cloud</a>
 
         <a href="https://aws.amazon.com/api-gateway/pricing/"> Details on pricing</a>
         """
 
         super().__init__(cdev_name, RUUID, nonce)
-        
+
         self._allow_cors = allow_cors
         self._routes: List[Route] = []
 
         self._authorizers: List[Authorizer] = authorizers
 
         self._default_authorizer_name = default_authorizer
 
         self._output = ApiOutput(cdev_name)
 
-
     @property
     def output(self) -> ApiOutput:
         """Output generated by the Cloud when this resource is deployed."""
         return self._output
 
     @property
     def allow_cors(self) -> bool:
@@ -318,65 +343,68 @@
 
         [Notes on CORS]
         """
         return self._allow_cors
 
     @allow_cors.setter
     @update_hash
-    def allow_cors(self, value: bool):
+    def allow_cors(self, value: bool) -> None:
         self._allow_cors = value
 
     @update_hash
-    def route(self, path: str, verb: route_verb, additional_scopes: List[str] = [], override_authorizer_name: str = None) -> Route:
+    def route(
+        self,
+        path: str,
+        verb: route_verb,
+        additional_scopes: List[str] = [],
+        override_authorizer_name: str = None,
+    ) -> Route:
         """Create a route for the API.
 
         Args:
             path (str): The http path of the route created
             verb (`route_verb`): verb for the path
-            override_authorizer_name (str): The authorizer for this route. Overriding the default authorizer for the Api. 
+            override_authorizer_name (str): The authorizer for this route. Overriding the default authorizer for the Api.
         Returns:
-            `Route` 
+            `Route`
 
         Generate a `Route` that can be used as a trigger for other resources.
 
         ```
         route = myApi.route('/hello_world', 'GET')
         ```
         """
 
-        authorizer_name = override_authorizer_name if override_authorizer_name else self._default_authorizer_name
-    
-        route = Route(
-            self.name,
-            path, 
-            verb,
-            authorizer_name,
-            additional_scopes
-            
+        authorizer_name = (
+            override_authorizer_name
+            if override_authorizer_name
+            else self._default_authorizer_name
         )
 
+        route = Route(self.name, path, verb, authorizer_name, additional_scopes)
+
         self._routes.append(route)
 
         return route
 
-    def compute_hash(self):
+    def compute_hash(self) -> None:
         self._hash = hasher.hash_list(
             [
                 hasher.hash_list([x.hash() for x in self._routes]),
-                self.allow_cors, 
+                self.allow_cors,
                 self.nonce,
                 self._default_authorizer_name,
-                hasher.hash_list([x.hash() for x in self._authorizers])
+                hasher.hash_list([x.hash() for x in self._authorizers]),
             ]
         )
 
     def render(self) -> simple_api_model:
-        routes =  frozenset(self._routes)
-       
+        routes = frozenset(self._routes)
+
         return simple_api_model(
             ruuid=self.ruuid,
             name=self.name,
             hash=self.hash,
             routes=frozenset([x.render() for x in routes]),
             allow_cors=self.allow_cors,
-            authorizers=frozenset([x.render() for x in self._authorizers])
+            authorizers=frozenset([x.render() for x in self._authorizers]),
         )
```

### Comparing `cdev-0.0.8/core/default/resources/simple/events.py` & `cdev-0.0.9/core/default/resources/simple/events.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     originating_resource_type: str
 
     hash: str
 
     granting_permission: Optional[Union[permission_model, permission_arn_model]]
 
 
-
-class Event():
-    
+class Event:
     def hash(self) -> str:
         raise NotImplementedError
 
-    def render(self,) -> event_model:
+    def render(
+        self,
+    ) -> event_model:
         raise NotImplementedError
```

### Comparing `cdev-0.0.8/core/default/resources/simple/iam.py` & `cdev-0.0.9/core/default/resources/simple/iam.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Set of constructs for adding permissions and authorization 
+"""Set of constructs for adding permissions and authorization
 
 """
 
 from typing import Dict, FrozenSet, List, Optional, Union
 
 from core.constructs.models import ImmutableModel
 from core.constructs.cloud_output import Cloud_Output_Str
@@ -15,81 +15,83 @@
     cloud_id: cdev_str_model
     effect: str
     resource_suffix: Optional[str]
     hash: str
 
     class Config:
         use_enum_values = True
-        # Beta Feature but should be fine since this is simple data 
+        # Beta Feature but should be fine since this is simple data
         frozen = True
 
 
 class permission_arn_model(ImmutableModel):
     arn: str
     hash: str
-    
+
     class Config:
         use_enum_values = True
-        # Beta Feature but should be fine since this is simple data 
+        # Beta Feature but should be fine since this is simple data
         frozen = True
 
 
-class Permission():
+class Permission:
     """
     Permission that can be attached to a resource to give it permission to access other resources.
     """
 
     def __init__(
         self,
         actions: List[str],
         cloud_id: cdev_str,
         effect: str,
         resource_suffix: Optional[str] = "",
-    ):
+    ) -> None:
         """
         Arguments:
             actions (List[str]): List of the actions that this policy will include
             cloud_id (cdev_str): The cloud id of the resource that is giving the permission
             effect ('Allow', 'Deny'): Allow or Deny the permission
             resource_suffix (Optional[str]): Some permissions need suffixes added to the looked up aws resource (i.e. dynamodb streams )
         """
         self.actions = actions
         self.cloud_id = cloud_id
         self.effect = effect
         self.resource_suffix = resource_suffix
-            
+
     def render(self) -> permission_model:
 
         return permission_model(
             actions=frozenset(self.actions),
-            cloud_id=self.cloud_id.render() if isinstance(self.cloud_id, Cloud_Output_Str) else self.cloud_id,
+            cloud_id=self.cloud_id.render()
+            if isinstance(self.cloud_id, Cloud_Output_Str)
+            else self.cloud_id,
             effect=self.effect,
-            hash=self.hash()
+            hash=self.hash(),
         )
 
     def hash(self) -> str:
-        _hash = hasher.hash_list([
-            hasher.hash_list(self.actions),
-            self.cloud_id.hash() if isinstance(self.cloud_id, Cloud_Output_Str) else self.cloud_id,
-            self.effect
-        ])
+        _hash = hasher.hash_list(
+            [
+                hasher.hash_list(self.actions),
+                self.cloud_id.hash()
+                if isinstance(self.cloud_id, Cloud_Output_Str)
+                else self.cloud_id,
+                self.effect,
+            ]
+        )
 
         return _hash
 
 
-class PermissionArn():
+class PermissionArn:
     """
     Id of a permission that is already deployed on the cloud.
     """
+
     def __init__(self, arn: str) -> None:
         self.arn = arn
 
-
     def render(self) -> permission_arn_model:
-        return permission_arn_model(
-            arn=self.arn,
-            hash=self.hash()
-        )
+        return permission_arn_model(arn=self.arn, hash=self.hash())
 
     def hash(self) -> str:
         return hasher.hash_string(self.arn)
-
```

### Comparing `cdev-0.0.8/core/default/resources/simple/object_store.py` & `cdev-0.0.9/core/default/resources/simple/object_store.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 """Set of constructs for creating Cloud Object Stores like S3
 
 """
 
 from enum import Enum
 from typing import Any, List
 
-from core.constructs.resource import Resource, ResourceModel, update_hash, ResourceOutputs, PermissionsAvailableMixin
+from core.constructs.resource import (
+    Resource,
+    ResourceModel,
+    update_hash,
+    ResourceOutputs,
+    PermissionsAvailableMixin,
+)
 from core.constructs.cloud_output import Cloud_Output_Str, OutputType
 from core.constructs.types import cdev_str_model
 from core.utils import hasher
 
 from core.default.resources.simple.iam import Permission
 
 from core.default.resources.simple.events import Event, event_model
 
 RUUID = "cdev::simple::bucket"
 
+
 class Bucket_Event_Type(str, Enum):
     Object_Created = "s3:ObjectCreated:*"
     """Receive Events when Objects are created in the `Bucket`"""
     Object_Removed = "s3:ObjectRemoved:*"
     """Receive Events when Objects are removed from the `Bucket`"""
     Object_Restore = "s3:ObjectRestore:*"
     """Receive Events when Objects are restored to the `Bucket`"""
@@ -29,167 +36,153 @@
 
 class bucket_event_model(event_model):
     """Model representing an Event from a Bucket
 
     Args:
         bucket_arn (cdev_str_model)
         bucket_name (cdev_str_model)
-        bucket_event_type (Bucket_Event_Type)   
+        bucket_event_type (Bucket_Event_Type)
     """
+
     bucket_arn: cdev_str_model
     bucket_name: cdev_str_model
     bucket_event_type: Bucket_Event_Type
 
 
 class BucketEvent(Event):
-    """Construct representing an Event from a Bucket
-    """
+    """Construct representing an Event from a Bucket"""
 
     def __init__(self, bucket_name: str, bucket_event_type: Bucket_Event_Type) -> None:
         """
         Args:
             bucket_name (str): Cdev name of the bucket
             bucket_event_type (Bucket_Event_Type): Type fo events to create
         """
         self.bucket_cdev_name = bucket_name
         self.bucket_event_type = bucket_event_type
-        self.bucket_arn =  Cloud_Output_Str(
-                name=bucket_name, 
-                ruuid=RUUID, 
-                key='cloud_id',
-                type=OutputType.RESOURCE 
-            )
-        self.bucket_name =  Cloud_Output_Str(
-                name=bucket_name, 
-                ruuid=RUUID, 
-                key='bucket_name',
-                type=OutputType.RESOURCE 
-            )
+        self.bucket_arn = Cloud_Output_Str(
+            name=bucket_name, ruuid=RUUID, key="cloud_id", type=OutputType.RESOURCE
+        )
+        self.bucket_name = Cloud_Output_Str(
+            name=bucket_name, ruuid=RUUID, key="bucket_name", type=OutputType.RESOURCE
+        )
 
     def render(self) -> bucket_event_model:
         return bucket_event_model(
             originating_resource_name=self.bucket_cdev_name,
             originating_resource_type=RUUID,
             hash=self.hash(),
             bucket_event_type=self.bucket_event_type,
             bucket_arn=self.bucket_arn.render(),
-            bucket_name=self.bucket_name.render()
+            bucket_name=self.bucket_name.render(),
         )
 
     def hash(self) -> str:
-        return hasher.hash_list([
-            self.bucket_cdev_name,
-            self.bucket_event_type
-        ])
+        return hasher.hash_list([self.bucket_cdev_name, self.bucket_event_type])
 
 
 class BucketPermissions:
     RUUID = "cdev::simple::bucket"
 
     def __init__(self, resource_name: str) -> None:
+
+        self.LIST_BUCKET = Permission(
+            actions=["s3:ListBucket"],
+            cloud_id=Cloud_Output_Str(
+                resource_name, RUUID, "cloud_id", OutputType.RESOURCE
+            ),
+            effect="Allow",
+        )
+        """Permissions to list objects from the `Bucket`"""
+
         self.READ_BUCKET = Permission(
-            actions=[
-                "s3:GetObject",
-                "s3:GetObjectVersion", 
-                "s3:ListBucket"
-            ],
-            cloud_id=Cloud_Output_Str(resource_name, RUUID, 'cloud_id', OutputType.RESOURCE),
+            actions=["s3:GetObject", "s3:GetObjectVersion"],
+            cloud_id=Cloud_Output_Str(
+                resource_name, RUUID, "cloud_id", OutputType.RESOURCE
+            ).join(["", "/*"]),
             effect="Allow",
         )
         """Permissions to read objects from the `Bucket`"""
 
         self.WRITE_BUCKET = Permission(
-            actions=[
-                "s3:PutObject",
-                "s3:PutObjectAcl", 
-                "s3:ListBucket"
-            ],
-            cloud_id=Cloud_Output_Str(resource_name, RUUID, 'cloud_id', OutputType.RESOURCE),
+            actions=["s3:PutObject", "s3:PutObjectAcl"],
+            cloud_id=Cloud_Output_Str(
+                resource_name, RUUID, "cloud_id", OutputType.RESOURCE
+            ).join(["", "/*"]),
             effect="Allow",
         )
         """Permissions to write objects to the `Bucket`"""
 
         self.READ_AND_WRITE_BUCKET = Permission(
-            actions=[
-                "s3:*Object",
-                "s3:ListBucket"
-            ],
-            cloud_id=Cloud_Output_Str(resource_name, RUUID, 'cloud_id', OutputType.RESOURCE),
+            actions=["s3:*Object"],
+            cloud_id=Cloud_Output_Str(
+                resource_name, RUUID, "cloud_id", OutputType.RESOURCE
+            ).join(["", "/*"]),
             effect="Allow",
         )
         """Permissions to read and write objects to and from the `Bucket`"""
 
         self.READ_EVENTS = Permission(
-            actions=[
-                "s3:*Object",
-                "s3:ListBucket"
-            ],
-            cloud_id=Cloud_Output_Str(resource_name, RUUID, 'cloud_id', OutputType.RESOURCE),
+            actions=["s3:*Object"],
+            cloud_id=Cloud_Output_Str(
+                resource_name, RUUID, "cloud_id", OutputType.RESOURCE
+            ).join(["", "/*"]),
             effect="Allow",
         )
         """Permissions to receive events from the `Bucket`"""
 
 
 class bucket_model(ResourceModel):
     """Model representing a Bucket"""
+
     pass
 
 
 class BucketOutput(ResourceOutputs):
     """Container object for the returned values from the cloud after a Bucket has been deployed."""
+
     def __init__(self, name: str) -> None:
         super().__init__(name, RUUID)
 
-
     @property
     def bucket_name(self) -> Cloud_Output_Str:
         """The name of the generated bucket"""
         return Cloud_Output_Str(
-            name=self._name,
-            ruuid=RUUID,
-            key='bucket_name',
-            type=self.OUTPUT_TYPE
+            name=self._name, ruuid=RUUID, key="bucket_name", type=self.OUTPUT_TYPE
         )
 
     @bucket_name.setter
-    def bucket_name(self, value: Any):
+    def bucket_name(self, value: Any) -> None:
         raise Exception
 
 
 class Bucket(PermissionsAvailableMixin, Resource):
     """A Simple Bucket is a basic object store for applications to build on."""
-    
+
     @update_hash
-    def __init__(self, cdev_name: str, nonce: str="") -> None:
+    def __init__(self, cdev_name: str, nonce: str = "") -> None:
         """
         Args:
             cdev_name (str): Name of the resource
             nonce (str): Nonce to make the resource hash unique if there are conflicting resources with same configuration.
         """
         super().__init__(cdev_name, RUUID, nonce)
 
         self.available_permissions: BucketPermissions = BucketPermissions(cdev_name)
         self.output = BucketOutput(cdev_name)
 
-
-    def create_event_trigger(
-        self, event_type: Bucket_Event_Type
-    ) -> BucketEvent:
+    def create_event_trigger(self, event_type: Bucket_Event_Type) -> BucketEvent:
         """Create Construct of event that other resources can respond to"""
 
-        event = BucketEvent(
-            bucket_name=self.name,
-            bucket_event_type=event_type
-        )
+        event = BucketEvent(bucket_name=self.name, bucket_event_type=event_type)
 
         return event
 
-    def compute_hash(self):
+    def compute_hash(self) -> None:
         self._hash = hasher.hash_list([self.nonce])
-        
+
     def render(self) -> bucket_model:
         return bucket_model(
             ruuid=self.ruuid,
             name=self.name,
             hash=self.hash,
         )
-
```

### Comparing `cdev-0.0.8/core/default/resources/simple/queue.py` & `cdev-0.0.9/core/default/resources/simple/queue.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 """Set of constructs for making message queues
 
 """
 from typing import Any
 
-from core.constructs.resource import Resource, ResourceModel, update_hash, ResourceOutputs, PermissionsAvailableMixin
-from core.constructs.cloud_output import  Cloud_Output_Str, OutputType
+from core.constructs.resource import (
+    Resource,
+    ResourceModel,
+    update_hash,
+    ResourceOutputs,
+    PermissionsAvailableMixin,
+)
+from core.constructs.cloud_output import Cloud_Output_Str, OutputType
 from core.constructs.types import cdev_str_model
 
 from core.default.resources.simple.events import Event, event_model
 from core.default.resources.simple.iam import Permission
 
 from core.utils import hasher
 
@@ -21,135 +27,138 @@
 class queue_event_model(event_model):
     """Model representing a message queue event
 
     Arguments:
         batch_size: int
         batch_window: int
     """
-    queue_arn: cdev_str_model   
+
+    queue_arn: cdev_str_model
     batch_size: int
-    batch_failure: bool 
+    batch_failure: bool
 
 
 class QueueEvent(Event):
     """Construct representing the Events from the Queue"""
-    def __init__(self, queue_name: str, batch_size: int, batch_failure: bool = True) -> None:
+
+    def __init__(
+        self, queue_name: str, batch_size: int, batch_failure: bool = True
+    ) -> None:
 
         if batch_size > 10000 or batch_size < 0:
             raise Exception
 
         self.cdev_queue_name = queue_name
 
         self.queue_arn = Cloud_Output_Str(
-                name=queue_name, 
-                ruuid=RUUID, 
-                key='arn',
-                type=OutputType.RESOURCE 
-            )
+            name=queue_name, ruuid=RUUID, key="arn", type=OutputType.RESOURCE
+        )
 
         self.batch_size = batch_size
         self.batch_failure = batch_failure
 
-
     def render(self) -> queue_event_model:
         return queue_event_model(
             originating_resource_name=self.cdev_queue_name,
             originating_resource_type=RUUID,
             hash=self.hash(),
             queue_arn=self.queue_arn.render(),
             batch_size=self.batch_size,
-            batch_failure=self.batch_failure 
+            batch_failure=self.batch_failure,
         )
 
-
     def hash(self) -> str:
-        return hasher.hash_list([
-            self.cdev_queue_name,
-            self.batch_size,
-            self.batch_failure 
-        ])
+        return hasher.hash_list(
+            [self.cdev_queue_name, self.batch_size, self.batch_failure]
+        )
+
 
 ######################
 ###### Permission
 ######################
 class QueuePermissions:
-
     def __init__(self, resource_name: str) -> None:
         self.READ_QUEUE = Permission(
             actions=[
                 "sqs:ReceiveMessage",
                 "sqs:DeleteMessage",
                 "sqs:GetQueueAttributes",
             ],
-            cloud_id=Cloud_Output_Str(resource_name, RUUID, 'cloud_id', OutputType.RESOURCE),
+            cloud_id=Cloud_Output_Str(
+                resource_name, RUUID, "cloud_id", OutputType.RESOURCE
+            ),
             effect="Allow",
         )
         """Permission to poll for messages from the Queue"""
 
         self.WRITE_QUEUE = Permission(
             actions=[
                 "sqs:SendMessage",
                 "sqs:GetQueueAttributes",
             ],
-            cloud_id=Cloud_Output_Str(resource_name, RUUID, 'cloud_id', OutputType.RESOURCE),
+            cloud_id=Cloud_Output_Str(
+                resource_name, RUUID, "cloud_id", OutputType.RESOURCE
+            ),
             effect="Allow",
         )
         """Permission to write messages to the Queue"""
 
         self.READ_AND_WRITE_QUEUE = Permission(
             actions=[
                 "sqs:ReceiveMessage",
                 "sqs:DeleteMessage",
                 "sqs:GetQueueAttributes",
                 "sqs:SendMessage",
             ],
-            cloud_id=Cloud_Output_Str(resource_name, RUUID, 'cloud_id', OutputType.RESOURCE),
+            cloud_id=Cloud_Output_Str(
+                resource_name, RUUID, "cloud_id", OutputType.RESOURCE
+            ),
             effect="Allow",
         )
         """Permission to read and write messages to and from the Queue"""
 
         self.READ_EVENTS = Permission(
             actions=[
                 "sqs:ReceiveMessage",
                 "sqs:DeleteMessage",
                 "sqs:GetQueueAttributes",
             ],
-            cloud_id=Cloud_Output_Str(resource_name, RUUID, 'cloud_id', OutputType.RESOURCE),
+            cloud_id=Cloud_Output_Str(
+                resource_name, RUUID, "cloud_id", OutputType.RESOURCE
+            ),
             effect="Allow",
         )
         """Permission to receive events to and from the Queue"""
 
+
 ######################
 ##### Output
 ######################
 class QueueOutput(ResourceOutputs):
     def __init__(self, name: str) -> None:
         super().__init__(name, RUUID)
 
     @property
     def queue_name(self) -> Cloud_Output_Str:
         """The name of the generated queue"""
         return Cloud_Output_Str(
-            name=self._name,
-            ruuid=RUUID,
-            key='queue_name',
-            type=self.OUTPUT_TYPE
+            name=self._name, ruuid=RUUID, key="queue_name", type=self.OUTPUT_TYPE
         )
 
     @queue_name.setter
     def queue_name(self, value: Any):
         raise Exception
 
 
 ######################
 ##### Queue
 ######################
 class queue_model(ResourceModel):
     """Model representing a Message Queue"""
-    
+
     is_fifo: bool
     """Should the Queue guarantee ordering of messages"""
 
 
 class Queue(PermissionsAvailableMixin, Resource):
     """A Message Queue"""
 
@@ -162,19 +171,19 @@
             nonce (str): Nonce to make the resource hash unique if there are conflicting resources with same configuration.
         """
         super().__init__(cdev_name, RUUID, nonce)
 
         self.is_fifo = is_fifo
         self.output = QueueOutput(cdev_name)
         self._event = None
-        
+
         self.available_permissions: QueuePermissions = QueuePermissions(cdev_name)
 
     @property
-    def is_fifo(self):
+    def is_fifo(self) -> bool:
         """Should the Queue guarantee ordering of messages"""
         return self._is_fifo
 
     @is_fifo.setter
     @update_hash
     def is_fifo(self, value: bool):
         self._is_fifo = value
@@ -191,24 +200,24 @@
             Exception: _description_
             Exception: _description_
 
         Returns:
             QueueEvent
         """
         if self._event:
-            raise Exception("Already created stream on this table. Use `get_stream()` to get the current stream.")
-    
+            raise Exception(
+                "Already created stream on this table. Use `get_stream()` to get the current stream."
+            )
+
         # https://docs.aws.amazon.com/lambda/latest/dg/with-sqs.html#events-sqs-eventsource
         if self.is_fifo and batch_size > 10:
             raise Exception
 
         event = QueueEvent(
-            queue_name=self.name,
-            batch_size=batch_size,
-            batch_failure=batch_failure
+            queue_name=self.name, batch_size=batch_size, batch_failure=batch_failure
         )
 
         self._event = event
 
         return event
 
     def get_event(self) -> QueueEvent:
@@ -217,22 +226,23 @@
         Raises:
             Exception: _description_
 
         Returns:
             QueueEvent
         """
         if not self._event:
-            raise Exception("Queue Event has not been created. Create a stream for this table using the `create_stream` function before calling this function.")
+            raise Exception(
+                "Queue Event has not been created. Create a stream for this table using the `create_stream` function before calling this function."
+            )
 
         return self._event
 
-        
-    def compute_hash(self):
+    def compute_hash(self) -> None:
         self._hash = hasher.hash_list([self.is_fifo, self.nonce])
-        
+
     def render(self) -> queue_model:
         return queue_model(
             name=self.name,
             ruuid=self.ruuid,
             hash=self.hash,
             is_fifo=self.is_fifo,
         )
```

### Comparing `cdev-0.0.8/core/default/resources/simple/relational_db.py` & `cdev-0.0.9/core/default/resources/simple/relational_db.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,98 +1,97 @@
 """Set of constructs for making Serverless based Relational DBs
 
 """
 
 from enum import Enum
 from typing import Any
 
-from core.constructs.resource import Resource, ResourceModel, ResourceOutputs, update_hash, PermissionsAvailableMixin
-from core.constructs.cloud_output import  Cloud_Output_Str, OutputType
+from core.constructs.resource import (
+    Resource,
+    ResourceModel,
+    ResourceOutputs,
+    update_hash,
+    PermissionsAvailableMixin,
+)
+from core.constructs.cloud_output import Cloud_Output_Str, OutputType
 from core.utils import hasher
 
 from core.default.resources.simple.iam import Permission, PermissionArn
 
 
 RUUID = "cdev::simple::relationaldb"
 
 
 #####################
 ###### Permission
 ######################
 class RelationalDBPermissions:
-     
     def __init__(self, resource_name: str) -> None:
-        
+
         self.DATABASE_ACCESS = Permission(
             actions=[
                 "rds-data:BatchExecuteStatement",
                 "rds-data:BeginTransaction",
                 "rds-data:CommitTransaction",
                 "rds-data:ExecuteStatement",
                 "rds-data:RollbackTransaction",
             ],
-            cloud_id=Cloud_Output_Str(resource_name, RUUID, 'cloud_id', OutputType.RESOURCE),
+            cloud_id=Cloud_Output_Str(
+                resource_name, RUUID, "cloud_id", OutputType.RESOURCE
+            ),
             effect="Allow",
         )
         """Access to the DB"""
 
         self.SECRET_ACCESS = PermissionArn(
             arn="arn:aws:iam::aws:policy/SecretsManagerReadWrite"
         )
         """Access to the generated Secret that contains the connection information"""
 
 
 ##############
 ##### Output
 ##############
 class RelationalDBOutput(ResourceOutputs):
-    """Container object for the returned values from the cloud after a Relational DB has been deployed."""   
+    """Container object for the returned values from the cloud after a Relational DB has been deployed."""
+
     def __init__(self, name: str) -> None:
         super().__init__(name, RUUID)
 
     @property
     def cluster_arn(self) -> Cloud_Output_Str:
         """The name of the generated db cluster"""
         return Cloud_Output_Str(
-            name=self._name,
-            ruuid=RUUID,
-            key='cluster_arn',
-            type=self.OUTPUT_TYPE
+            name=self._name, ruuid=RUUID, key="cluster_arn", type=self.OUTPUT_TYPE
         )
 
     @cluster_arn.setter
-    def cluster_arn(self, value: Any):
+    def cluster_arn(self, value: Any) -> None:
         raise Exception
 
     @property
     def endpoint(self) -> Cloud_Output_Str:
         """The name of the generated db cluster"""
         return Cloud_Output_Str(
-            name=self._name,
-            ruuid=RUUID,
-            key='endpoint',
-            type=self.OUTPUT_TYPE
+            name=self._name, ruuid=RUUID, key="endpoint", type=self.OUTPUT_TYPE
         )
 
     @endpoint.setter
     def endpoint(self, value: Any):
         raise Exception
 
     @property
     def secret_arn(self) -> Cloud_Output_Str:
         """The arn of the secret value create that holds the password for the db"""
         return Cloud_Output_Str(
-            name=self._name,
-            ruuid=RUUID,
-            key='secret_arn',
-            type=self.OUTPUT_TYPE
+            name=self._name, ruuid=RUUID, key="secret_arn", type=self.OUTPUT_TYPE
         )
 
     @secret_arn.setter
-    def secret_arn(self, value: Any):
+    def secret_arn(self, value: Any) -> None:
         raise Exception
 
 
 ###############
 ##### RelationalDB
 ###############
 class db_engine(str, Enum):
@@ -102,52 +101,51 @@
     aurora_mysql = "aurora-mysql"
     """MySQL 5.7-compatible Aurora"""
 
     aurora_postgresql = "aurora-postgresql"
     """Postgres 10.4-compatible Aurora"""
 
 
-
 class simple_relational_db_model(ResourceModel):
     """Model that represents a relation db"""
+
     Engine: db_engine
     """DB engine"""
     MasterUsername: str
     """Username used to connect to the DB"""
     MasterUserPassword: str
     """Username used to connect to the DB"""
     DatabaseName: str
     """Name for the main db"""
     EnableHttpEndpoint: bool
     """Allow connection via a generated HTTP endpoint"""
     MaxCapacity: int
     """Maximum amount of capacity to scale to"""
-    MinCapacity: int    
+    MinCapacity: int
     """Amount of seconds to wait before scaling DB completely down."""
     SecondsToPause: int
     """Amount of seconds to wait before scaling DB completely down"""
 
 
-
 class RelationalDB(PermissionsAvailableMixin, Resource):
     """Construct for creating a Serverless Relational DB"""
-    
+
     @update_hash
     def __init__(
         self,
         cdev_name: str,
         engine: db_engine,
         username: str,
         password: str,
         database_name: str = "",
         enable_http_endpoint: bool = True,
         max_capacity: int = 64,
         min_capacity: int = 2,
         seconds_to_pause: int = 300,
-        nonce: str = ""
+        nonce: str = "",
     ) -> None:
         """
         Args:
             cdev_name (str): Name of the resource
             engine (db_engine): DB engine
             username (str): Username used to connect to the DB
             password (str): Password used to connect to the DB
@@ -166,108 +164,110 @@
         self._database_name = database_name
         self._enable_http_endpoint = enable_http_endpoint
         self._max_capacity = max_capacity
         self._min_capacity = min_capacity
         self._seconds_to_pause = seconds_to_pause
 
         self.output: RelationalDBOutput = RelationalDBOutput(cdev_name)
-        self.available_permissions: RelationalDBPermissions = RelationalDBPermissions(cdev_name)
+        self.available_permissions: RelationalDBPermissions = RelationalDBPermissions(
+            cdev_name
+        )
 
     @property
-    def seconds_to_pause(self):
+    def seconds_to_pause(self) -> int:
         """Amount of seconds to wait before scaling DB completely down"""
         return self._seconds_to_pause
 
     @seconds_to_pause.setter
     @update_hash
-    def seconds_to_pause(self, value: int):
+    def seconds_to_pause(self, value: int) -> None:
         self._seconds_to_pause = value
 
     @property
-    def min_capacity(self):
+    def min_capacity(self) -> int:
         """Amount of seconds to wait before scaling DB completely down."""
         return self._min_capacity
 
     @min_capacity.setter
     @update_hash
-    def min_capacity(self, value: int):
+    def min_capacity(self, value: int) -> None:
         self._min_capacity = value
 
     @property
-    def max_capacity(self):
+    def max_capacity(self) -> int:
         """Maximum amount of capacity to scale to"""
         return self._max_capacity
 
     @max_capacity.setter
     @update_hash
-    def max_capacity(self, value: int):
+    def max_capacity(self, value: int) -> None:
         self._max_capacity = value
 
     @property
     def enable_http_endpoint(self):
         """Allow connection via a generated HTTP endpoint"""
         return self._enable_http_endpoint
 
     @enable_http_endpoint.setter
     @update_hash
-    def enable_http_endpoint(self, value: bool):
+    def enable_http_endpoint(self, value: bool) -> None:
         self._enable_http_endpoint = value
 
     @property
-    def database_name(self):
+    def database_name(self) -> str:
         """Name for the main db"""
         return self._database_name
 
     @database_name.setter
     @update_hash
-    def database_name(self, value: str):
+    def database_name(self, value: str) -> None:
         self._database_name = value
 
     @property
-    def master_user_password(self):
+    def master_user_password(self) -> str:
         """Password used to connect to the DB"""
         return self._master_user_password
 
     @master_user_password.setter
     @update_hash
-    def master_user_password(self, value: str):
+    def master_user_password(self, value: str) -> None:
         self._master_user_password = value
 
     @property
-    def master_username(self):
+    def master_username(self) -> str:
         """Username used to connect to the DB"""
         return self._master_username
 
     @master_username.setter
     @update_hash
-    def master_username(self, value: str):
+    def master_username(self, value: str) -> None:
         self._master_username = value
 
     @property
     def engine(self):
         """DB engine"""
         return self._engine
 
     @engine.setter
     @update_hash
-    def engine(self, value: db_engine):
+    def engine(self, value: db_engine) -> None:
         self._engine = value
 
-    def compute_hash(self):
+    def compute_hash(self) -> None:
         self._hash = hasher.hash_list(
             [
                 self.engine,
                 self.master_username,
                 self.master_user_password,
                 self.database_name,
                 self.enable_http_endpoint,
                 self.max_capacity,
                 self.min_capacity,
                 self.seconds_to_pause,
-                self.nonce
+                self.nonce,
             ]
         )
 
     def render(self) -> simple_relational_db_model:
         return simple_relational_db_model(
             **{
                 "ruuid": self.ruuid,
@@ -279,8 +279,7 @@
                 "DatabaseName": self.database_name,
                 "EnableHttpEndpoint": self.enable_http_endpoint,
                 "MaxCapacity": self.max_capacity,
                 "MinCapacity": self.min_capacity,
                 "SecondsToPause": self.seconds_to_pause,
             }
         )
-
```

### Comparing `cdev-0.0.8/core/default/resources/simple/static_site.py` & `cdev-0.0.9/core/default/resources/simple/static_site.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,70 @@
 """Set of constructs for for making a website to serve Static Web Content
 
 """
 from typing import Any, Optional
 
-from core.constructs.resource import Resource, ResourceModel, update_hash, ResourceOutputs
-from core.constructs.cloud_output import  Cloud_Output_Str
+from core.constructs.resource import (
+    Resource,
+    ResourceModel,
+    update_hash,
+    ResourceOutputs,
+)
+from core.constructs.cloud_output import Cloud_Output_Str
 from core.utils import hasher
 
 RUUID = "cdev::simple::staticsite"
 
 
 class StaticSiteOutput(ResourceOutputs):
     def __init__(self, name: str) -> None:
         super().__init__(name, RUUID)
 
-
     @property
     def bucket_name(self) -> Cloud_Output_Str:
         """The name of the underlying S3 Bucket where the content for the site is stored."""
         return Cloud_Output_Str(
-            name=self._name,
-            ruuid=RUUID,
-            key='bucket_name',
-            type=self.OUTPUT_TYPE
+            name=self._name, ruuid=RUUID, key="bucket_name", type=self.OUTPUT_TYPE
         )
 
     @bucket_name.setter
-    def bucket_name(self, value: Any):
+    def bucket_name(self, value: Any) -> None:
         raise Exception
 
-
     @property
     def cloudfront_id(self) -> Cloud_Output_Str:
         """The id of the site on the Cloudfront CDN"""
         return Cloud_Output_Str(
-            name=self._name,
-            ruuid=RUUID,
-            key='cloudfront_id',
-            type=self.OUTPUT_TYPE
+            name=self._name, ruuid=RUUID, key="cloudfront_id", type=self.OUTPUT_TYPE
         )
 
     @cloudfront_id.setter
-    def cloudfront_id(self, value: Any):
+    def cloudfront_id(self, value: Any) -> None:
         raise Exception
 
-
     @property
     def cloudfront_arn(self) -> Cloud_Output_Str:
         """The arn of the site on the Cloudfront CDN"""
         return Cloud_Output_Str(
-            name=self._name,
-            ruuid=RUUID,
-            key='cloudfront_arn',
-            type=self.OUTPUT_TYPE
+            name=self._name, ruuid=RUUID, key="cloudfront_arn", type=self.OUTPUT_TYPE
         )
 
     @cloudfront_arn.setter
-    def cloudfront_arn(self, value: Any):
+    def cloudfront_arn(self, value: Any) -> None:
         raise Exception
 
-
-
     @property
     def site_url(self) -> Cloud_Output_Str:
         """The url of the created site"""
         return Cloud_Output_Str(
-            name=self._name,
-            ruuid=RUUID,
-            key='site_url',
-            type=self.OUTPUT_TYPE
+            name=self._name, ruuid=RUUID, key="site_url", type=self.OUTPUT_TYPE
         )
 
     @site_url.setter
-    def site_url(self, value: Any):
+    def site_url(self, value: Any) -> None:
         raise Exception
 
 
 ###############
 ##### Static Site
 ###############
 class simple_static_site_model(ResourceModel):
@@ -89,140 +77,138 @@
     content_folder: Optional[str]
     """The relative path within the Workspace of the folder containting the static content for the site."""
     domain_name: Optional[str]
     """The domain name to associate with this site. This will set up the site to be aliased via DNS to the given domain name."""
     ssl_certificate_arn: Optional[str]
     """Arn of a SSL certificate to use with the site."""
 
+
 class StaticSite(Resource):
-    """A Static Site that can be used to serve static web content. 
-    
-    """
-    
+    """A Static Site that can be used to serve static web content."""
+
     @update_hash
     def __init__(
         self,
         cdev_name: str,
         index_document: str = "index.html",
         error_document: str = "error.html",
         sync_folder: bool = False,
         content_folder: str = None,
         domain_name: str = None,
         ssl_certificate_arn: str = None,
-        nonce: str = ""
-
+        nonce: str = "",
     ) -> None:
         """Create a static hosted site.
 
         Arguments:
             cdev_name (str): [description]
             index_document (str): The suffix for documents when request are made for a folder.
             error_document (str): The absolute path of document within the site that will be used as a general error page.
             sync_folder (bool): Whether to consider changes in the state of the content folder to trigger a sync of the content folder.
             content_folder (str): The relative path within the `Workspace` of the folder containting the static content for the site.
             domain_name (str): The domain name to associate with this site. This will set up the site to be aliased via DNS to the given domain name.
-            ssl_certificate_arn (str): Arn of a SSL certificate to use with the site. 
+            ssl_certificate_arn (str): Arn of a SSL certificate to use with the site.
             nonce (str): Nonce to make the resource hash unique if there are conflicting resources with same configuration.
         """
         super().__init__(cdev_name, RUUID, nonce)
 
         self._index_document = index_document
         self._error_document = error_document
         self._sync_folder = sync_folder
         self._content_folder = content_folder
         self._domain_name = domain_name
         self._ssl_certificate_arn = ssl_certificate_arn
 
         self.output = StaticSiteOutput(cdev_name)
 
     @property
-    def index_document(self):
+    def index_document(self) -> str:
         """The suffix for documents when request are made for a folder."""
         return self._index_document
 
     @index_document.setter
     @update_hash
-    def index_document(self, value: str):
+    def index_document(self, value: str) -> None:
         self._index_document = value
 
     @property
-    def error_document(self):
+    def error_document(self) -> str:
         """The absolute path of document within the site that will be used as a general error page."""
         return self._error_document
 
     @error_document.setter
     @update_hash
-    def error_document(self, value: str):
+    def error_document(self, value: str) -> None:
         self._error_document = value
 
     @property
-    def content_folder(self):
+    def content_folder(self) -> str:
         """The relative path within the `Workspace` of the folder containting the static content for the site."""
         return self._content_folder
 
     @content_folder.setter
     @update_hash
-    def content_folder(self, value: str):
+    def content_folder(self, value: str) -> None:
         self._content_folder = value
 
     @property
-    def sync_folder(self):
+    def sync_folder(self) -> str:
         """Whether to consider changes in the state of the content folder to trigger a sync of the content folder."""
         return self._sync_folder
 
     @sync_folder.setter
     @update_hash
-    def sync_folder(self, value: bool):
+    def sync_folder(self, value: bool) -> None:
         self._sync_folder = value
 
     @property
-    def domain_name(self):
+    def domain_name(self) -> str:
         """The domain name to associate with this site. This will set up the site to be aliased via DNS to the given domain name."""
         return self._domain_name
 
     @domain_name.setter
     @update_hash
-    def domain_name(self, value: str):
+    def domain_name(self, value: str) -> None:
         self._domain_name = value
 
     @property
-    def ssl_certificate_arn(self):
+    def ssl_certificate_arn(self) -> str:
         """The domain name to associate with this site. This will set up the site to be aliased via DNS to the given domain name."""
         return self._ssl_certificate_arn
 
     @ssl_certificate_arn.setter
     @update_hash
-    def ssl_certificate_arn(self, value: str):
+    def ssl_certificate_arn(self, value: str) -> None:
         self._ssl_certificate_arn = value
 
-    def compute_hash(self):
+    def compute_hash(self) -> None:
         # TODO update component to look at the content if the sync folder command is given
         self._hash = hasher.hash_list(
             [
                 self.index_document,
                 self.error_document,
                 self.sync_folder,
                 self.content_folder,
                 self.domain_name,
                 self.ssl_certificate_arn,
-                self.nonce
+                self.nonce,
             ]
         )
 
     def render(self) -> simple_static_site_model:
         if self.sync_folder and not self.content_folder:
 
-            raise Exception(f"If sync_folder is set to 'True' then you must provide a path to the folder.")
+            raise Exception(
+                f"If sync_folder is set to 'True' then you must provide a path to the folder."
+            )
 
         return simple_static_site_model(
             ruuid=self.ruuid,
             name=self.name,
             hash=self.hash,
             index_document=self.index_document,
             error_document=self.error_document,
             sync_folder=self.sync_folder,
-            content_folder=self.content_folder,  
+            content_folder=self.content_folder,
             domain_name=self.domain_name,
-            ssl_certificate_arn=self.ssl_certificate_arn 
+            ssl_certificate_arn=self.ssl_certificate_arn,
         )
-
-
```

### Comparing `cdev-0.0.8/core/default/resources/simple/table.py` & `cdev-0.0.9/core/default/resources/simple/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 """Set of constructs for making No SQL DB Tables
 """
 from enum import Enum
 from typing import Any, FrozenSet, List
 
-from core.constructs.resource import Resource, ResourceModel, update_hash, ResourceOutputs, PermissionsAvailableMixin
-from core.constructs.cloud_output import  Cloud_Output_Str, OutputType
+from core.constructs.resource import (
+    Resource,
+    ResourceModel,
+    update_hash,
+    ResourceOutputs,
+    PermissionsAvailableMixin,
+)
+from core.constructs.cloud_output import Cloud_Output_Str, OutputType
 from core.constructs.types import cdev_str_model
 from core.constructs.models import ImmutableModel
 
 from core.default.resources.simple.events import Event, event_model
 from core.default.resources.simple.iam import Permission
 
 from core.utils import hasher
 
 RUUID = "cdev::simple::table"
 
 
 #################
 ##### Events
 #################
-#TODO: Add more documentation on the json schema of the events
+# TODO: Add more documentation on the json schema of the events
 class stream_type(str, Enum):
     """Type of streams for a table."""
 
     KEYS_ONLY = "KEYS_ONLY"
     """Only the key attributes of the modified item."""
     NEW_IMAGE = "NEW_IMAGE"
     """The entire item, as it appears after it was modified."""
@@ -37,62 +43,62 @@
     """Model to represent a stream event
 
     Args:
         table_name (str): Cdev name of the API this route is apart of
         view_type (stream_type): Type of eventthe stream produces
         batch_size (int): Size of event batches
     """
-    table_name: cdev_str_model    
+
+    table_name: cdev_str_model
     view_type: stream_type
     batch_size: int
-    batch_failure: bool 
+    batch_failure: bool
 
 
 class StreamEvent(Event):
     """Construct for representing the Stream of a `Table`"""
 
-    def __init__(self, table_name: str, view_type: stream_type, batch_size: int, batch_failure: bool= True) -> None:
+    def __init__(
+        self,
+        table_name: str,
+        view_type: stream_type,
+        batch_size: int,
+        batch_failure: bool = True,
+    ) -> None:
         """
         Args:
             table_name (str): Cdev name of the API this route is apart of
             view_type (stream_type): Type of eventthe stream produces
             batch_size (int): Size of event batches
         """
-        
+
         self.cdev_table_name = table_name
-        
-        self.table_name= Cloud_Output_Str(
-                name=table_name, 
-                ruuid=RUUID, 
-                key='table_name',
-                type=OutputType.RESOURCE 
-            )
-            
-        self.view_type=view_type
-        self.batch_size=batch_size
-        self.batch_failure = batch_failure
 
+        self.table_name = Cloud_Output_Str(
+            name=table_name, ruuid=RUUID, key="table_name", type=OutputType.RESOURCE
+        )
+
+        self.view_type = view_type
+        self.batch_size = batch_size
+        self.batch_failure = batch_failure
 
     def hash(self) -> str:
-        return hasher.hash_list([
-            self.cdev_table_name,
-            self.view_type,
-            self.batch_size,
-            self.batch_failure
-        ])
-        
+        return hasher.hash_list(
+            [self.cdev_table_name, self.view_type, self.batch_size, self.batch_failure]
+        )
+
     def render(self) -> stream_event_model:
         return stream_event_model(
             originating_resource_name=self.cdev_table_name,
             originating_resource_type=RUUID,
             hash=self.hash(),
             batch_size=self.batch_size,
             view_type=self.view_type.value,
             table_name=self.table_name.render(),
-            batch_failure=self.batch_failure
+            batch_failure=self.batch_failure,
         )
 
 
 #####################
 ###### Permission
 ######################
 class TablePermissions:
@@ -104,15 +110,17 @@
             actions=[
                 "dynamodb:GetItem",
                 "dynamodb:BatchGetItem",
                 "dynamodb:Scan",
                 "dynamodb:Query",
                 "dynamodb:ConditionCheckItem",
             ],
-            cloud_id=Cloud_Output_Str(resource_name, RUUID, 'cloud_id', OutputType.RESOURCE),
+            cloud_id=Cloud_Output_Str(
+                resource_name, RUUID, "cloud_id", OutputType.RESOURCE
+            ),
             effect="Allow",
         )
         """Permissions to read data from the Table"""
 
         self.WRITE_TABLE = Permission(
             actions=[
                 "dynamodb:BatchGetItem",
@@ -123,15 +131,17 @@
                 "dynamodb:DeleteItem",
                 "dynamodb:GetItem",
                 "dynamodb:Scan",
                 "dynamodb:Query",
                 "dynamodb:UpdateItem",
                 "dynamodb:DescribeLimits",
             ],
-            cloud_id=Cloud_Output_Str(resource_name, RUUID, 'cloud_id', OutputType.RESOURCE),
+            cloud_id=Cloud_Output_Str(
+                resource_name, RUUID, "cloud_id", OutputType.RESOURCE
+            ),
             effect="Allow",
         )
         """Permissions to write data to the Table"""
 
         self.READ_AND_WRITE_TABLE = Permission(
             actions=[
                 "dynamodb:BatchGetItem",
@@ -142,48 +152,51 @@
                 "dynamodb:DescribeTable",
                 "dynamodb:GetItem",
                 "dynamodb:PutItem",
                 "dynamodb:Query",
                 "dynamodb:Scan",
                 "dynamodb:UpdateItem",
             ],
-            cloud_id=Cloud_Output_Str(resource_name, RUUID, 'cloud_id', OutputType.RESOURCE),
+            cloud_id=Cloud_Output_Str(
+                resource_name, RUUID, "cloud_id", OutputType.RESOURCE
+            ),
             effect="Allow",
         )
         """Permissions to read and write data to and from the Table"""
 
         self.READ_STREAM = Permission(
             actions=[
                 "dynamodb:DescribeStream",
                 "dynamodb:GetRecords",
                 "dynamodb:GetShardIterator",
                 "dynamodb:ListShards",
                 "dynamodb:ListStreams",
             ],
-            cloud_id=Cloud_Output_Str(resource_name, RUUID, 'cloud_id', OutputType.RESOURCE).join(["", "/stream/*"]),
+            cloud_id=Cloud_Output_Str(
+                resource_name, RUUID, "cloud_id", OutputType.RESOURCE
+            ).join(["", "/stream/*"]),
             effect="Allow",
         )
         """Permissions to receive and process events from the Table Stream"""
 
+
 ##############
 ##### Output
 ##############
 class TableOutput(ResourceOutputs):
     """Container object for the returned values from the cloud after a `Table` has been deployed."""
+
     def __init__(self, name: str) -> None:
         super().__init__(name, RUUID)
 
     @property
     def table_name(self) -> Cloud_Output_Str:
         """The name of the generated table"""
         return Cloud_Output_Str(
-            name=self._name,
-            ruuid=RUUID,
-            key='table_name',
-            type=self.OUTPUT_TYPE
+            name=self._name, ruuid=RUUID, key="table_name", type=self.OUTPUT_TYPE
         )
 
     @table_name.setter
     def table_name(self, value: Any):
         raise Exception
 
 
@@ -204,15 +217,15 @@
     """Number"""
     B = "B"
     """Binary"""
 
 
 class key_type(str, Enum):
     """Type of key for a defined key on a table.
-    
+
     These value will be used by the primary key to determine how the data is stored in the table.
     visit https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.CoreComponents.html#HowItWorks.CoreComponents.PrimaryKey for more details.
     """
 
     HASH = "HASH"
     """Partion Key"""
     RANGE = "RANGE"
@@ -222,83 +235,80 @@
 class attribute_definition_model(ImmutableModel):
     """Model representing an attribute of a `Table`
 
     Args:
         attribute_name (str)
         attribute_type (`attribute_type`)
     """
-    attribute_name: str 
+
+    attribute_name: str
     attribute_type: attribute_type
 
-    
+
 class AttributeDefinition:
     """Construct representing an attribute of a `Table`"""
 
-    def __init__(self, name:str, type: attribute_type) -> None:
+    def __init__(self, name: str, type: attribute_type) -> None:
         """Create an attribute that will be part of a `Table`
-        
+
         Args:
             name (str): Name of the attribute
             type (attribute_type): Type of value the attribute stores
         """
         self.name = name
         self.type = type
 
-
     def render(self) -> attribute_definition_model:
         return attribute_definition_model(
-            attribute_name=self.name,
-            attribute_type=self.type
+            attribute_name=self.name, attribute_type=self.type
         )
 
 
 class key_definition_model(ImmutableModel):
     """Model representing a primary key of a `Table`
 
     Args:
         attribute_name (str)
         key_type (`key_type`)
     """
-    attribute_name: str 
+
+    attribute_name: str
     key_type: key_type
 
 
 class KeyDefinition:
     """Construct representing a primary key of a `Table`"""
 
-    def __init__(self, name:str, type: key_type) -> None:
+    def __init__(self, name: str, type: key_type) -> None:
         """
         Args:
             name (str): Name of the attribute
             type (key_type): Type of value the attribute stores
 
         Note that the `name` property must match a `name` of a given `AttributeDefinition` on the created
-        table. 
+        table.
 
-        The keys on a table will define the optimal way of retrieving data from the `Table`. 
+        The keys on a table will define the optimal way of retrieving data from the `Table`.
 
 
         """
         self.name = name
         self.type = type
 
-
     def render(self) -> key_definition_model:
-        return key_definition_model(
-            attribute_name=self.name,
-            key_type=self.type
-        )
+        return key_definition_model(attribute_name=self.name, key_type=self.type)
 
 
 class simple_table_model(ResourceModel):
     """Model representing a `Table`
 
     Args:
         ResourceModel ([type]): [description]
     """
+
     attributes: FrozenSet[attribute_definition_model]
     keys: FrozenSet[key_definition_model]
 
 
 class Table(PermissionsAvailableMixin, Resource):
     """Create a NoSql Table (DynamoDB)"""
 
@@ -358,15 +368,15 @@
     @property
     def keys(self) -> List[KeyDefinition]:
         """Current Primary Key Definitions"""
         return self._keys
 
     @keys.setter
     @update_hash
-    def keys(self, value: List[KeyDefinition]):
+    def keys(self, value: List[KeyDefinition]) -> None:
         self._keys = value
 
     def create_stream(
         self, view_type: stream_type, batch_size: int = 100, batch_failure: bool = True
     ) -> StreamEvent:
         """Create a `StreamEvent` for this table
 
@@ -378,21 +388,23 @@
         Raises:
             Exception: If this Table already has a Stream, throw exception. Should use `get_stream()`
 
         Returns:
             StreamEvent: The created `Stream_Event`
         """
         if self._stream:
-            raise Exception(f"Already created stream on this table. Use `get_stream()` to get the current stream.")
+            raise Exception(
+                f"Already created stream on this table. Use `get_stream()` to get the current stream."
+            )
 
         event = StreamEvent(
             table_name=self.name,
             view_type=view_type,
             batch_size=batch_size,
-            batch_failure=batch_failure
+            batch_failure=batch_failure,
         )
 
         self._stream = event
         return event
 
     def get_stream(self) -> StreamEvent:
         """Get the `StreamEvent` for this `Table`
@@ -400,70 +412,65 @@
         Raises:
             Exception: If this Table has not created a stream, throw exception
 
         Returns:
             StreamEvent: The `StreamEvent` for this Table
         """
         if not self._stream:
-            raise Exception("Stream has not been created. Create a stream for this table using the `create_stream` function.")
+            raise Exception(
+                "Stream has not been created. Create a stream for this table using the `create_stream` function."
+            )
 
         return self._stream
 
-
-    def _check_attributes_and_keys(
-        self
-    ) -> None:
+    def _check_attributes_and_keys(self) -> None:
         """
         Check key constraints based on https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.create_table
         """
         if len(self.keys) > 2:
             raise Exception("Only two primary keys can be used")
 
         primary_key = self.keys[0]
 
         if not primary_key:
             raise Exception("No Hash key provided")
 
         if not primary_key.type == key_type.HASH:
             raise Exception("First key is not Hash key")
 
-        if not primary_key.name in set(
-            [x.name for x in self.attributes]
-        ):
+        if not primary_key.name in set([x.name for x in self.attributes]):
             raise Exception(
                 f"Hash key 'AttributeName' ({primary_key.name}) not defined in attributes",
             )
 
         if len(self.keys) == 1:
-            return 
+            return
 
         range_key = self.keys[1]
 
         if not range_key.type == key_type.RANGE:
             raise Exception("Second key is not a Range key")
 
-        if not range_key.name in set(
-            [x.name for x in self.attributes]
-        ):
+        if not range_key.name in set([x.name for x in self.attributes]):
             raise Exception(
                 f"Range key 'AttributeName' ({range_key.name}) not defined in attributes",
             )
 
-    def compute_hash(self):
+    def compute_hash(self) -> None:
         self._hash = hasher.hash_list(
             [
-                [x.render() for x in self.attributes], 
-                [x.render() for x in self.keys], 
-                self.nonce
+                [x.render() for x in self.attributes],
+                [x.render() for x in self.keys],
+                self.nonce,
             ]
         )
 
     def render(self) -> simple_table_model:
         self._check_attributes_and_keys()
-        
+
         return simple_table_model(
             ruuid=RUUID,
             name=self.name,
             hash=self.hash,
             attributes=[x.render() for x in self.attributes],
             keys=[x.render() for x in self.keys],
         )
```

### Comparing `cdev-0.0.8/core/default/resources/simple/topic.py` & `cdev-0.0.9/core/default/resources/simple/topic.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 """Set of constructs for making fan our message topics
 
 """
 from typing import Any
 
-from core.constructs.resource import Resource, ResourceModel, update_hash, ResourceOutputs, PermissionsAvailableMixin
+from core.constructs.resource import (
+    Resource,
+    ResourceModel,
+    update_hash,
+    ResourceOutputs,
+    PermissionsAvailableMixin,
+)
 from core.constructs.cloud_output import Cloud_Output_Str, OutputType
 from core.constructs.types import cdev_str_model
 
 from core.default.resources.simple.events import Event, event_model
 from core.default.resources.simple.iam import Permission
 
 from core.utils import hasher
@@ -16,149 +22,145 @@
 
 
 ######################
 ##### Events
 ######################
 class topic_event_model(event_model):
     """Model representing a Topic event"""
-    topic_arn: cdev_str_model   
+
+    topic_arn: cdev_str_model
 
 
 class TopicEvent(Event):
     """Construct representing the Events from the Topic"""
-    
+
     def __init__(self, topic_name: str) -> None:
 
         self.cdev_topic_name = topic_name
 
         self.topic_arn = Cloud_Output_Str(
-                name=topic_name, 
-                ruuid=RUUID, 
-                key='arn',
-                type=OutputType.RESOURCE 
-            )
-
+            name=topic_name, ruuid=RUUID, key="arn", type=OutputType.RESOURCE
+        )
 
     def render(self) -> topic_event_model:
         return topic_event_model(
             originating_resource_name=self.cdev_topic_name,
             originating_resource_type=RUUID,
             hash=self.hash(),
             topic_arn=self.topic_arn.render(),
         )
 
-
     def hash(self) -> str:
-        return hasher.hash_list([
-            self.cdev_topic_name,
-        ])
+        return hasher.hash_list(
+            [
+                self.cdev_topic_name,
+            ]
+        )
 
 
 #####################
 ###### Permission
 ######################
 class TopicPermissions:
     def __init__(self, resource_name) -> None:
         self.SUBSCRIBE = Permission(
             actions=[
                 "sns:GetTopicAttributes",
                 "sns:Subscribe",
             ],
-            cloud_id=Cloud_Output_Str(resource_name, RUUID, 'cloud_id', OutputType.RESOURCE),
+            cloud_id=Cloud_Output_Str(
+                resource_name, RUUID, "cloud_id", OutputType.RESOURCE
+            ),
             effect="Allow",
         )
         """Permission to subscribe to the Topic"""
 
         self.PUBLISH = Permission(
-            actions=[
-                "sns:GetTopicAttributes",
-                "sns:Publish"
-            ],
-            cloud_id=Cloud_Output_Str(resource_name, RUUID, 'cloud_id', OutputType.RESOURCE),
+            actions=["sns:GetTopicAttributes", "sns:Publish"],
+            cloud_id=Cloud_Output_Str(
+                resource_name, RUUID, "cloud_id", OutputType.RESOURCE
+            ),
             effect="Allow",
         )
         """Permission to publish to the Topic"""
 
+
 ##############
 ##### Output
 ##############
 class TopicOutput(ResourceOutputs):
     """Container object for the returned values from the cloud after a Topic has been deployed."""
+
     def __init__(self, name: str) -> None:
         super().__init__(name, RUUID)
 
     @property
     def topic_name(self) -> Cloud_Output_Str:
         """The name of the generated topic"""
         return Cloud_Output_Str(
-            name=self._name,
-            ruuid=RUUID,
-            key='topic_name',
-            type=self.OUTPUT_TYPE
+            name=self._name, ruuid=RUUID, key="topic_name", type=self.OUTPUT_TYPE
         )
 
     @topic_name.setter
-    def topic_name(self, value: Any):
+    def topic_name(self, value: Any) -> None:
         raise Exception
 
 
 ###############
 ##### Topic
 ###############
 class simple_topic_model(ResourceModel):
     """Model representing a Pub/Sub Topic"""
 
     is_fifo: bool
     """Should the Topic guarantee ordering of messages"""
 
+
 class Topic(PermissionsAvailableMixin, Resource):
     """Construct for creating a managed SNS Pub/Sub Topic"""
 
     @update_hash
-    def __init__(
-        self, cdev_name: str, is_fifo: bool = False, nonce: str = ''
-    ) -> None:
+    def __init__(self, cdev_name: str, is_fifo: bool = False, nonce: str = "") -> None:
         """
         Args:
             cdev_name (str): Name of the resource.
             is_fifo (bool, default=False): If True, the Queue will guarantee ordering of messages.
             nonce (str): Nonce to make the resource hash unique if there are conflicting resources with same configuration.
         """
         super().__init__(cdev_name, RUUID, nonce)
 
         self._is_fifo = is_fifo
         self.output = TopicOutput(cdev_name)
         self.available_permissions: TopicPermissions = TopicPermissions(cdev_name)
         self._event = None
 
     @property
-    def is_fifo(self):
+    def is_fifo(self) -> bool:
         """Should the Pub/Sub Topic guarantee ordering of messages"""
         return self._is_fifo
 
     @is_fifo.setter
     @update_hash
-    def is_fifo(self, value: bool):
+    def is_fifo(self, value: bool) -> None:
         self._is_fifo = value
 
-    def create_event_trigger(
-        self
-    ) -> TopicEvent:
+    def create_event_trigger(self) -> TopicEvent:
         """Create an Event for the Topic that other resources can listen to
 
         Raises:
             Exception: _description_
             Exception: _description_
 
         Returns:
             QueueEvent
         """
         if self._event:
-            raise Exception("Already created an event on this topic. Use `get_event()` to get the current event.")
-    
+            raise Exception(
+                "Already created an event on this topic. Use `get_event()` to get the current event."
+            )
 
         event = TopicEvent(
             topic_name=self.name,
         )
 
         self._event = event
 
@@ -170,22 +172,23 @@
         Raises:
             Exception: _description_
 
         Returns:
             QueueEvent
         """
         if not self._event:
-            raise Exception("Topic Event has not been created. Create a Topic Event for this topic using the `create_event_trigger` function before calling this function.")
+            raise Exception(
+                "Topic Event has not been created. Create a Topic Event for this topic using the `create_event_trigger` function before calling this function."
+            )
 
         return self._event
 
-    def compute_hash(self):
+    def compute_hash(self) -> None:
         self._hash = hasher.hash_list([self.is_fifo, self.nonce])
 
     def render(self) -> simple_topic_model:
         return simple_topic_model(
             name=self.name,
             ruuid=self.ruuid,
             hash=self.hash,
             is_fifo=self.is_fifo,
         )
-
```

### Comparing `cdev-0.0.8/core/default/resources/simple/xlambda.py` & `cdev-0.0.9/core/default/resources/simple/xlambda.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,295 +4,391 @@
 
 import importlib
 import inspect
 import os
 from pydantic import FilePath
 from typing import Any, Callable, Dict, FrozenSet, List, Optional, Union
 
-from core.constructs.cloud_output import Cloud_Output, Cloud_Output_Dynamic, Cloud_Output_Str
-from core.constructs.resource import Resource, ResourceModel, update_hash, ResourceOutputs, PermissionsGrantableMixin
+from core.constructs.cloud_output import (
+    Cloud_Output,
+    Cloud_Output_Dynamic,
+    Cloud_Output_Str,
+)
+from core.constructs.resource import (
+    Resource,
+    ResourceModel,
+    update_hash,
+    ResourceOutputs,
+    PermissionsGrantableMixin,
+)
 from core.constructs.models import frozendict, ImmutableModel
-from core.constructs.types import cdev_str_model, cdev_str
+from core.constructs.types import cdev_str_model, cdev_str, cdev_int
 
 from core.utils import hasher
 from core.utils.platforms import lambda_python_environment, get_current_closest_platform
 
-from core.default.resources.simple.iam import Permission, PermissionArn, permission_arn_model, permission_model
+from core.default.resources.simple.iam import (
+    Permission,
+    PermissionArn,
+    permission_arn_model,
+    permission_model,
+)
 from core.default.resources.simple.events import Event, event_model
 
 
 LAMBDA_LAYER_RUUID = "cdev::simple::lambda_layer"
 RUUID = "cdev::simple::function"
 
+###################
+##### Exceptions
+###################
+class CallableError(Exception):
+    pass
+
+
 ################
-##### Dependencies 
+##### Dependencies
 ################
-class DeployedLayer():
+class DeployedLayer:
     """Construct that represents a Layer already deployed on the Cloud"""
+
     def __init__(self, arn: str) -> None:
         self.arn = arn
 
 
 class dependency_layer_model(ResourceModel):
     """Model that represents a local folder that will be deployed on the cloud as a Layer"""
+
     artifact_path: str
 
 
 class DependencyLayer(Resource):
     """Construct that represents a local folder that will be deployed on the cloud as a Layer"""
-    def __init__(self, cdev_name: str, artifact_path: FilePath, artifact_hash: str) -> None:
+
+    def __init__(
+        self, cdev_name: str, artifact_path: FilePath, artifact_hash: str
+    ) -> None:
         super().__init__(cdev_name, LAMBDA_LAYER_RUUID)
         self.artifact_path = artifact_path
         self.artifact_hash = artifact_hash
         self._hash = artifact_hash
         self.output = DependencyLayerOutput(cdev_name)
 
     def render(self) -> dependency_layer_model:
         return dependency_layer_model(
             ruuid=LAMBDA_LAYER_RUUID,
-            name=self.name, 
+            name=self.name,
             hash=self.artifact_hash,
-            artifact_path=self.artifact_path
+            artifact_path=self.artifact_path,
         )
 
+
 ################
 ##### Output
 ################
 
 
 class DependencyLayerOutput(ResourceOutputs):
     """Container object for the returned values from the cloud after a Layer has been deployed."""
+
     def __init__(self, name: str) -> None:
         super().__init__(name, LAMBDA_LAYER_RUUID)
 
-
     @property
     def layer_arn(self) -> Cloud_Output_Str:
         """The id of the created layer"""
         return Cloud_Output_Str(
-            name=self._name,
-            ruuid=LAMBDA_LAYER_RUUID,
-            key='arn',
-            type=self.OUTPUT_TYPE
+            name=self._name, ruuid=LAMBDA_LAYER_RUUID, key="arn", type=self.OUTPUT_TYPE
         )
 
     @layer_arn.setter
-    def layer_arn(self, value: Any):
+    def layer_arn(self, value: Any) -> None:
         raise Exception
 
 
 class FunctionOutput(ResourceOutputs):
     """Container object for the returned values from the cloud after a Serverless Function has been deployed."""
+
     def __init__(self, name: str) -> None:
         super().__init__(name, RUUID)
 
 
 ################
 ##### Function
 ################
 class simple_function_configuration_model(ImmutableModel):
     """Model representing the configuration of a Serverless Function"""
+
     handler: str
     description: Optional[cdev_str_model]
     environment_variables: frozendict
+    memory_size: int
+    timeout: int
+    storage: int
 
     class Config:
         use_enum_values = True
-        # Beta Feature but should be fine since this is simple data 
+        # Beta Feature but should be fine since this is simple data
         frozen = True
 
 
-class SimpleFunctionConfiguration():
+class SimpleFunctionConfiguration:
     """Container for the configuration settings of Serverless Function"""
-    def __init__(self, handler: cdev_str, description: cdev_str = "", environment_variables: Dict[str, cdev_str] = {} ) -> None:
+
+    def __init__(
+        self,
+        handler: cdev_str,
+        memory_size: cdev_int,
+        timeout: cdev_int,
+        storage: cdev_int,
+        description: cdev_str = "",
+        environment_variables: Dict[str, cdev_str] = {},
+    ) -> None:
         """
         Args:
             handler (cdev_str): The python module path of the handler function that is triggered by the Cloud Platform
             description (cdev_str, optional): A description of the Function. Defaults to "".
             environment_variables (Dict[str, cdev_str], optional): A dict of overriding variabled for the Environment. Defaults to {}.
         """
         self.handler = handler
+        self.memory_size = memory_size
+        self.timeout = timeout
+        self.storage = storage
         self.description = description
         self.environment_variables = environment_variables
 
-
     def render(self) -> simple_function_configuration_model:
         return simple_function_configuration_model(
-            handler=self.handler.render() if isinstance(self.handler, Cloud_Output_Dynamic) else self.handler,
-            description=self.description.render() if isinstance(self.description, Cloud_Output_Dynamic) else self.description,
-            environment_variables = frozendict(
-                {k:frozendict(v.render().dict()) if isinstance(v, Cloud_Output) else v for k,v in self.environment_variables.items()}
-            ) if self.environment_variables else frozendict({})
+            handler=self.handler.render()
+            if isinstance(self.handler, Cloud_Output_Dynamic)
+            else self.handler,
+            memory_size=self.memory_size.render()
+            if isinstance(self.memory_size, Cloud_Output_Dynamic)
+            else self.memory_size,
+            timeout=self.timeout.render()
+            if isinstance(self.timeout, Cloud_Output_Dynamic)
+            else self.timeout,
+            storage=self.storage.render()
+            if isinstance(self.storage, Cloud_Output_Dynamic)
+            else self.storage,
+            description=self.description.render()
+            if isinstance(self.description, Cloud_Output_Dynamic)
+            else self.description,
+            environment_variables=frozendict(
+                {
+                    k: frozendict(v.render().dict())
+                    if isinstance(v, Cloud_Output)
+                    else v
+                    for k, v in self.environment_variables.items()
+                }
+            )
+            if self.environment_variables
+            else frozendict({}),
         )
 
     def hash(self) -> str:
-        env_hashable = {k:(v if not isinstance(v, Cloud_Output) else v.hash()) for k,v in self.environment_variables.items()} 
-
-
-        return hasher.hash_list([
-            self.handler,
-            self.description,
-            hasher.hash_list(sorted(env_hashable.items()))
-        ])
+        env_hashable = {
+            k: (v if not isinstance(v, Cloud_Output) else v.hash())
+            for k, v in self.environment_variables.items()
+        }
 
+        return hasher.hash_list(
+            [
+                self.handler,
+                self.memory_size,
+                self.timeout,
+                self.storage,
+                self.description,
+                hasher.hash_list(sorted(env_hashable.items())),
+            ]
+        )
 
 
 class simple_function_model(ResourceModel):
     """Model representing a Serverless Function
 
     Args:
         Filepath ([type]): [description]
     """
+
     filepath: str  # Don't use FilePath because this will be a relative path and might not always point correctly to a file in all contexts
     configuration: simple_function_configuration_model
     events: FrozenSet[event_model]
     permissions: FrozenSet[Union[permission_model, permission_arn_model]]
     external_dependencies: FrozenSet[Any]
     src_code_hash: str
     platform: lambda_python_environment
 
 
-
 class SimpleFunction(PermissionsGrantableMixin, Resource):
     """Construct to represent a Serverless Function. It is recommend to generate this resource using the `simple_function_annotation`"""
+
     @update_hash
     def __init__(
         self,
         cdev_name: str,
         filepath: str,
         configuration: SimpleFunctionConfiguration,
         events: List[Event] = [],
         platform: lambda_python_environment = None,
         function_permissions: List[Union[Permission, PermissionArn]] = [],
-        external_dependencies: List[Union[DeployedLayer, DependencyLayer]]=[],
+        external_dependencies: List[Union[DeployedLayer, DependencyLayer]] = [],
         src_code_hash: str = None,
+        preserve_function: Callable = None,
         nonce: str = "",
     ) -> None:
         """
 
         Args:
             cdev_name (str): Cdev Name for the function
             filepath (str): Path the final artifact to upload.
             configuration (SimpleFunctionConfiguration):  Configuration options for the function.
             events (List[Event], optional):  List of event triggers for the function.. Defaults to [].
             platform (lambda_python_environment, optional): Option to override the deployment platform in the Cloud.. Defaults to None.
             function_permissions (List[Union[Permission, PermissionArn]], optional): List of Permissions to grant to the Function.. Defaults to [].
             external_dependencies (List[Union[DeployedLayer, DependencyLayer]], optional): Dependencies to link to in the Cloud. Defaults to [].
             src_code_hash (str, optional): identifying hash of the source code. Defaults to None.
+            preserve_function (Callable, optional): the original function that is being deployed. This allows the returned object ro remain Callable. Default to None.
             nonce (str, optional): Nonce to make the resource hash unique if there are conflicting resources with same configuration.
         """
         super().__init__(cdev_name, RUUID, nonce)
 
         self._filepath = filepath
         self._events = events
         self._configuration = configuration
         self._external_dependencies = external_dependencies
-        self._granted_permissions: List[Union[Permission, PermissionArn]] = function_permissions
+        self._granted_permissions: List[
+            Union[Permission, PermissionArn]
+        ] = function_permissions
+
+        self.src_code_hash = (
+            src_code_hash if src_code_hash else hasher.hash_file(filepath)
+        )
 
-        self.src_code_hash = src_code_hash if src_code_hash else hasher.hash_file(filepath)
+        self._platform = platform or get_current_closest_platform()
 
-        self._platform = platform if platform else get_current_closest_platform()
-        
+        self._preserved_function = preserve_function
+        self.__annotations__ = preserve_function.__annotations__
+        self.__doc__ = preserve_function.__doc__
 
     @property
-    def filepath(self):
+    def filepath(self) -> str:
         return self._filepath
 
     @filepath.setter
     @update_hash
-    def filepath(self, value: str):
+    def filepath(self, value: str) -> None:
         self._filepath = value
 
     @property
-    def events(self):
+    def events(self) -> List[Event]:
         return self._events
 
     @events.setter
     @update_hash
-    def events(self, value: List[Event]):
+    def events(self, value: List[Event]) -> None:
         self._events = value
 
     @property
-    def configuration(self):
+    def configuration(self) -> SimpleFunctionConfiguration:
         return self._configuration
 
     @configuration.setter
     @update_hash
     def configuration(self, value: SimpleFunctionConfiguration):
         self._configuration = value
 
     @property
-    def platform(self):
+    def platform(self) -> lambda_python_environment:
         return self._platform
 
     @platform.setter
     @update_hash
-    def platform(self, value: lambda_python_environment):
+    def platform(self, value: lambda_python_environment) -> None:
         self._platform = value
 
     @property
-    def external_dependencies(self):
+    def external_dependencies(self) -> List[Union[DeployedLayer, DependencyLayer]]:
         return self._external_dependencies
 
     @external_dependencies.setter
     @update_hash
-    def external_dependencies(self, value: List[Union[DeployedLayer, DependencyLayer]]):
+    def external_dependencies(
+        self, value: List[Union[DeployedLayer, DependencyLayer]]
+    ) -> None:
         self._external_dependencies = value
 
-    def compute_hash(self):
-        self._permissions_hash = hasher.hash_list([x.hash() for x in self._granted_permissions])
+    def compute_hash(self) -> None:
+        self._permissions_hash = hasher.hash_list(
+            [x.hash() for x in self._granted_permissions]
+        )
         self._config_hash = self._configuration.hash()
         self._events_hash = hasher.hash_list([x.hash() for x in self.events])
 
         self._hash = hasher.hash_list(
             [
                 self.src_code_hash,
                 self._config_hash,
                 self._events_hash,
                 self._permissions_hash,
                 self._nonce,
-                self._platform
+                self._platform,
             ]
         )
 
     def render(self) -> simple_function_model:
 
         premissions = [x.render() for x in self.granted_permissions]
 
-        dependencies = [x.output.cloud_id.render() if isinstance(x, DependencyLayer) else x.arn for x in self.external_dependencies]
-        
+        dependencies = [
+            x.output.cloud_id.render() if isinstance(x, DependencyLayer) else x.arn
+            for x in self.external_dependencies
+        ]
+
         return simple_function_model(
             name=self.name,
             ruuid=self.ruuid,
             hash=self.hash,
             configuration=self.configuration.render(),
             filepath=self.filepath,
             events=frozenset([x.render() for x in self.events]),
             permissions=frozenset(premissions),
             external_dependencies=frozenset(dependencies),
             src_code_hash=self.src_code_hash,
-            platform=self.platform
+            platform=self.platform,
         )
 
+    def __call__(self, *args: Any, **kwds: Any) -> Any:
+        if not self._preserved_function:
+            raise CallableError
+
+        return self._preserved_function(*args, **kwds)
+
 
 def simple_function_annotation(
     name: str,
     events: List[Event] = [],
     environment={},
+    memory_size: int = 128,
+    timeout: int = 30,
+    storage: int = 512,
     permissions: List[Union[Permission, PermissionArn]] = [],
     override_platform: lambda_python_environment = None,
     includes: List[str] = [],
-    nonce: str=""
+    nonce: str = "",
 ) -> Callable[[Callable], SimpleFunction]:
     """This annotation is used to designate that a function should be deployed as a Serverless function.
 
     Args:
         name (str): Cdev Name for the function
         events (List[Event], optional): List of event triggers for the function. Defaults to [].
         environment (dict, optional): Dictionary to apply to the Environment Variables of the deployed function. Defaults to {}.
+        memory_size (int, optional): Memory Size of you lambda in MB. Default is 128.
+        timeout (int, optional): Timeout of your lambda in seconds. Default is 30 sec and up to 900.
+        storage (int, optional): Storage of your lambda in MB. Default is 512 MB and can be up to 10240.
         permissions (List[Union[Permission, PermissionArn]], optional): List of Permissions to grant to the Function. Defaults to [].
         override_platform (lambda_python_environment, optional): Option to override the deployment platform in the Cloud. Defaults to None.
         includes (List[str], optional): Set of identifiers to extra global statements to include in parsed artifacts. Defaults to [].
         nonce (str, optional): Nonce to make the resource hash unique if there are conflicting resources with same configuration.
 
     Returns:
         Callable[[Callable], SimpleFunction]: wrapper that returns the `SimpleFunction`
@@ -305,30 +401,31 @@
 
                 if item[0] == "__name__":
                     handler_name = item[1]
                 elif item[0] == "__doc__":
                     description = item[1] if item[1] else ""
                 elif item[0] == "__module__":
                     mod_name = item[1]
-
-
         final_config = SimpleFunctionConfiguration(
             handler=handler_name,
+            memory_size=memory_size,
+            timeout=timeout,
+            storage=storage,
             description=description,
-            environment_variables=environment
+            environment_variables=environment,
         )
-
         mod = importlib.import_module(mod_name)
 
         full_filepath = os.path.abspath(mod.__file__)
 
         return SimpleFunction(
             cdev_name=name,
             filepath=full_filepath,
             events=events,
             configuration=final_config,
             platform=override_platform,
             function_permissions=permissions,
-            nonce=nonce
+            preserve_function=func,
+            nonce=nonce,
         )
 
     return create_function
```

### Comparing `cdev-0.0.8/core/default/workspace.py` & `cdev-0.0.9/core/default/workspace.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,192 +1,194 @@
 import json
 import os
-from typing import Callable, List, Dict, Optional, Any, Tuple, Union
+from typing import List, Dict, Optional, Any, Tuple
 from pydantic.main import BaseModel
 
-from pydantic.types import DirectoryPath, FilePath
+from pydantic.types import DirectoryPath
 
 from core.constructs.backend import Backend, Backend_Configuration, load_backend
 from core.constructs.mapper import CloudMapper
 from core.constructs.components import Component, ComponentModel
 from core.constructs.workspace import (
     Workspace_State,
     Workspace_Info,
     Workspace,
     WorkspaceManager,
     wrap_phase,
 )
-from core.constructs.cloud_output import Cloud_Output, cloud_output_dynamic_model, evaluate_dynamic_output, cloud_output_model
+from core.constructs.cloud_output import (
+    Cloud_Output,
+    cloud_output_dynamic_model,
+    evaluate_dynamic_output,
+    cloud_output_model,
+)
+from core.constructs.settings import Settings_Info
 
-from ..utils import file_manager, module_loader
+from ..utils import file_manager
 
 
-DEFAULT_COMMAND_LOCATIONS = [
-    'core.default.commands'
-]
+DEFAULT_COMMAND_LOCATIONS = ["core.default.commands"]
 
 ROOT_FOLDER_NAME = ".cdev"
 WORKSPACE_FILE_NAME = "workspace_info.json"
 
-class local_workspace_configuration(BaseModel):
-    initialization_module: str
-    backend_configuration: Backend_Configuration
-    resource_state_uuid: Optional[str]
-
 
 class local_workspace(Workspace):
     """
-    A singleton that encapsulates the configuration of a workspace that is implemented on the local filesystem. The singleton can be accessed during different
-    parts of the lifecycle of a cdev core command execution. When this singleton is created, it is registered as the global workspace for that execution.
+    A singleton that implements a workspace that is on the local filesystem. The singleton can be accessed during different
+    parts of the lifecycle of a cdev core command execution. When this singleton is created, it is registered as the global
+    workspace for that execution.
     """
 
     _instance = None
 
     _COMMANDS = DEFAULT_COMMAND_LOCATIONS
     _MAPPERS = []
     _COMPONENTS = []
+    _OUTPUT: List[Tuple[str, str, cloud_output_model]] = []
 
     _resource_state_uuid: str = None
-
     _backend: Backend = None
 
     _state: Workspace_State = Workspace_State.UNINITIALIZED
 
-    _output: List[Tuple[str, str, cloud_output_model]] = []
-
     _current_component: str = None
 
     def __new__(cls):
         if cls._instance is None:
             cls._instance = super(Workspace, cls).__new__(cls)
             # Put any initialization here.
 
             cls._instance.set_state(Workspace_State.UNINITIALIZED)
 
             # Load the backend
             cls._instance._backend = None
+            cls._instance._resource_state_uuid = None
 
             cls._instance._COMMANDS = DEFAULT_COMMAND_LOCATIONS
             cls._instance._MAPPERS = []
             cls._instance._COMPONENTS = []
-            cls._instance._resource_state_uuid = None
+            cls._instance._OUTPUT = []
 
             Workspace.set_global_instance(cls._instance)
 
         return cls._instance
 
     @classmethod
-    def terminate_singleton(cls):
+    def terminate_singleton(cls) -> None:
         cls._instance = None
 
     def initialize_workspace(
-        self, workspace_configuration_dict: local_workspace_configuration
-    ):
-
-        # It is the responsibility of the higher up callers to set the correct states for initialization.
-        # This allows the flexibility of higher up frameworks injecting initialization steps into the process.
-        workspace_configuration = local_workspace_configuration(
-            **workspace_configuration_dict
+        self,
+        settings_info: Settings_Info,
+        backend_info: Backend_Configuration,
+        resource_state_uuid: str,
+        initialization_modules: Optional[List[str]] = [],
+        configuration: Dict = {},
+    ) -> None:
+        super().initialize_workspace(
+            settings_info=settings_info,
+            backend_info=backend_info,
+            resource_state_uuid=resource_state_uuid,
+            initialization_modules=initialization_modules,
+            configuration=configuration,
         )
-        
-        try:
-            backend_config = workspace_configuration.backend_configuration
-            self.set_backend(load_backend(backend_config))
-        except Exception as e:
-            print(f"Could not load the load backend")
-            raise e
-
-        module_loader.import_module(workspace_configuration.initialization_module)
-        
-        if workspace_configuration.resource_state_uuid:
-            if not workspace_configuration.resource_state_uuid in set(
-                [x.uuid for x in self._backend.get_top_level_resource_states()]
-            ):
-                raise Exception(
-                    f"{workspace_configuration.resource_state_uuid} not in loaded backend ({self._backend.get_top_level_resource_states()})"
-                )
-
-        self.set_resource_state_uuid(workspace_configuration.resource_state_uuid)
-        
-        
 
-    def destroy_workspace(self):
+    def destroy_workspace(self) -> None:
         Workspace.destroy_workspace(self)
         local_workspace.terminate_singleton()
 
     ################
     ##### State
     ################
-    def set_state(self, value: Workspace_State):
+    def set_state(self, value: Workspace_State) -> None:
         self._state = value
 
     def get_state(self) -> Workspace_State:
         return self._state
 
-
     @wrap_phase([Workspace_State.EXECUTING_FRONTEND])
     def generate_current_state(self) -> List[ComponentModel]:
-        """
-        Execute the components of this workspace to generate the current desired state of the resources.
-
-        Returns:
-            Current State (List[ComponentModel]): The current state generated by the components.
-        """
-
         rv = []
         components: List[Component] = self.get_components()
 
         for component in components:
             self._current_component = component.name
             rv.append(component.render())
 
         return rv
 
+    @wrap_phase([Workspace_State.INITIALIZING])
+    def set_resource_state_uuid(self, resource_state_uuid: str) -> None:
+        """Set the Resource State UUID to denote the Resource State that this Workspace will execute over.
+
+        Note that this function should only be called during the `Workspace Initialization` part of the Cdev lifecycle.
+
+        Arguments:
+            resource_state_uuid (str): Resource State UUID from the Backend
+        """
+        self._resource_state_uuid = resource_state_uuid
+
+    @wrap_phase(
+        [
+            Workspace_State.INITIALIZED,
+            Workspace_State.EXECUTING_FRONTEND,
+            Workspace_State.EXECUTING_BACKEND,
+        ]
+    )
+    def get_resource_state_uuid(self) -> str:
+        """Get the Resource State UUID that this Workspace is executing over.
+
+        Note that this function should only be called during the `Workspace Initialized` part of the Cdev lifecycle.
+
+        Returns:
+            resource_state_uuid (str): Resource State UUID from the Backend
+        """
+        return self._resource_state_uuid
 
     #######################
     ##### Display Output
     #######################
-    @wrap_phase([Workspace_State.INITIALIZED, Workspace_State.EXECUTING_FRONTEND, Workspace_State.EXECUTING_BACKEND])
-    def display_output(self, tag: str, output: Cloud_Output):
-        self._output.append((tag, self._current_component, output.render()))
-
+    @wrap_phase(
+        [
+            Workspace_State.INITIALIZED,
+            Workspace_State.EXECUTING_FRONTEND,
+            Workspace_State.EXECUTING_BACKEND,
+        ]
+    )
+    def display_output(self, tag: str, output: Cloud_Output) -> None:
+        self._OUTPUT.append((tag, self._current_component, output.render()))
 
     @wrap_phase([Workspace_State.INITIALIZED, Workspace_State.EXECUTING_BACKEND])
     def render_outputs(self) -> List[Tuple[str, Any]]:
-        """Render the output associated with the Workspace
-
-        Returns:
-            List[Tuple[str, Any]]: The List of outputs with their associated tag
-        
-        """
         rv = []
 
-
         if not self._current_component:
             raise Exception
 
-        for tag, component, cloud_output in self._output:
+        for tag, component, cloud_output in self._OUTPUT:
             resolved_value = self.get_backend().get_cloud_output_value_by_name(
                 self.get_resource_state_uuid(),
                 component,
                 cloud_output.ruuid,
                 cloud_output.name,
-                cloud_output.key
+                cloud_output.key,
             )
 
             if isinstance(cloud_output, cloud_output_dynamic_model):
-                resolved_value = evaluate_dynamic_output(
-                    resolved_value,
-                    cloud_output
-                )
+                # If the cloud output object contains computations than evaluate the computations over the cloud output
+                resolved_value = evaluate_dynamic_output(resolved_value, cloud_output)
 
             rv.append((tag, resolved_value))
 
         return rv
 
+    def clear_output(self) -> None:
+        self._OUTPUT = []
+
     #################
     ##### Mappers
     #################
     @wrap_phase([Workspace_State.INITIALIZING])
     def add_mapper(self, mapper: CloudMapper) -> None:
         if not isinstance(mapper, CloudMapper):
             # TODO Throw error
@@ -217,92 +219,77 @@
 
         return rv
 
     #################
     ##### Commands
     #################
     @wrap_phase([Workspace_State.INITIALIZING])
-    def add_command(self, command_location: str):
+    def add_command(self, command_location: str) -> None:
         self._COMMANDS.append(command_location)
 
     @wrap_phase([Workspace_State.INITIALIZING])
-    def add_commands(self, command_locations: List[str]):
+    def add_commands(self, command_locations: List[str]) -> None:
         for command_location in command_locations:
             self.add_command(command_location)
 
     @wrap_phase([Workspace_State.INITIALIZED])
     def get_commands(self) -> List[str]:
         return self._COMMANDS
 
     #################
     ##### Components
     #################
     @wrap_phase([Workspace_State.INITIALIZING])
-    def add_component(self, component: Component):
+    def add_component(self, component: Component) -> None:
         self._COMPONENTS.append(component)
 
     @wrap_phase([Workspace_State.INITIALIZING])
-    def add_components(self, components: List[Component]):
+    def add_components(self, components: List[Component]) -> None:
         for component in components:
             self.add_component(component)
 
     @wrap_phase([Workspace_State.INITIALIZED, Workspace_State.EXECUTING_FRONTEND])
     def get_components(self) -> List[Component]:
         return self._COMPONENTS
 
     #################
     ##### Backend
     #################
     @wrap_phase([Workspace_State.INITIALIZING])
-    def set_backend(self, backend: Backend):
+    def set_backend(self, backend: Backend) -> None:
         if not isinstance(backend, Backend):
             raise Exception("Not a backend object")
 
         self._backend = backend
 
-    @wrap_phase([Workspace_State.INITIALIZED, Workspace_State.EXECUTING_FRONTEND, Workspace_State.EXECUTING_BACKEND])
+    @wrap_phase(
+        [
+            Workspace_State.INITIALIZED,
+            Workspace_State.EXECUTING_FRONTEND,
+            Workspace_State.EXECUTING_BACKEND,
+        ]
+    )
     def get_backend(self) -> Backend:
         return self._backend
 
-    @wrap_phase([Workspace_State.INITIALIZING])
-    def set_resource_state_uuid(self, resource_state_uuid: str):
-        self._resource_state_uuid = resource_state_uuid
-
-    @wrap_phase([Workspace_State.INITIALIZED, Workspace_State.EXECUTING_FRONTEND,  Workspace_State.EXECUTING_BACKEND])
-    def get_resource_state_uuid(self) -> str:
-        return self._resource_state_uuid
-
 
 class local_workspace_manager(WorkspaceManager):
     def __init__(
         self,
         base_dir: DirectoryPath,
         workspace_dir: str = None,
         workspace_filename: str = None,
     ) -> None:
         self.base_dir = base_dir
-        self.workspace_dir = (
-            workspace_dir if workspace_dir else ROOT_FOLDER_NAME
-        )
+        self.workspace_dir = workspace_dir if workspace_dir else ROOT_FOLDER_NAME
         self.workspace_filename = (
-            workspace_filename
-            if workspace_filename
-            else WORKSPACE_FILE_NAME
+            workspace_filename if workspace_filename else WORKSPACE_FILE_NAME
         )
 
-    def create_new_workspace(self, workspace_info: Workspace_Info):
-        """
-        Create a new workspace based on the information provided.
-
-        Args:
-            workspace_info (Workspace_Info): information about the backend configuration
-
-        Raises:
-            WorkSpaceAlreadyCreated
-        """
+    def create_new_workspace(self, workspace_info: Workspace_Info) -> None:
         base_cdev_dir = os.path.join(self.base_dir, self.workspace_dir)
         if not os.path.isdir(base_cdev_dir):
             os.mkdir(base_cdev_dir)
 
         file_manager.safe_json_write(
             workspace_info.dict(), os.path.join(base_cdev_dir, self.workspace_filename)
         )
```

### Comparing `cdev-0.0.8/core/utils/command_finder.py` & `cdev-0.0.9/core/utils/command_finder.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,65 +22,89 @@
 
 
 class TooManyCommandClasses(Exception):
     pass
 
 
 def find_specified_command(
-    command_list: List[str], 
-    all_search_locations_list: List[str]
+    command_list: List[str], all_search_locations_list: List[str]
 ) -> Tuple[Union[BaseCommand, BaseCommandContainer], str, str, bool]:
-    
+    """Search the provided locations for the given command.
+
+    Args:
+        command_list (List[str]): _description_
+        all_search_locations_list (List[str]): _description_
+
+    Raises:
+        NoCommandFound
+
+    Returns:
+        Tuple[Union[BaseCommand, BaseCommandContainer], str, str, bool]: _description_
+    """
+
     command_list_copy = command_list.copy()
 
     for search_location in all_search_locations_list:
         # Search locations are denoted as python module paths, so convert the module to a path to search from
         mod = import_module(search_location)
         search_location_path = os.path.dirname(mod.__file__)
-    
 
         did_find, is_command = _recursive_find_specified_command(
             command_list.copy(), search_location_path
         )
 
         if not did_find:
             continue
 
         full_command_module_name = f"{search_location}.{'.'.join(command_list_copy)}"
 
         if is_command:
             try:
-                initialized_object = initialize_command_module(
-                    full_command_module_name
-                )
+                initialized_object = initialize_command_module(full_command_module_name)
             except Exception as e:
                 print(e)
-                raise Exception(f"ERROR Initializing Command Module at {full_command_module_name}")
+                raise Exception(
+                    f"ERROR Initializing Command Module at {full_command_module_name}"
+                )
 
         else:
             try:
                 initialized_object = initialize_command_container_module(
                     full_command_module_name
                 )
             except Exception as e:
                 print(e)
-                raise Exception(f"ERROR Initializing Command Container Module at {search_location}.{command_list}")
+                raise Exception(
+                    f"ERROR Initializing Command Container Module at {search_location}.{command_list}"
+                )
 
-        
-        final_path_name =  f"{search_location}.{'.'.join(command_list_copy[:-1])}"
+        final_path_name = f"{search_location}.{'.'.join(command_list_copy[:-1])}"
         command_name = command_list_copy[-1]
         return initialized_object, final_path_name, command_name, is_command
 
-
     # If we loop through all the search locations and no commands were found then throw exception
-    raise NoCommandFound(f"No Command or Commands Container found for {command_list_copy}")
-        
+    raise NoCommandFound(
+        f"No Command or Commands Container found for {command_list_copy}"
+    )
+
 
 def initialize_command_module(mod_path: str) -> BaseCommand:
-    
+    """Given a path to a command, initialize the given command.
+
+    Args:
+        mod_path (str): path to the command module
+
+    Raises:
+        TooManyCommandClasses: The module contained more than one command
+        NoCommandFound: No command was found in the module
+
+    Returns:
+        BaseCommand
+    """
+
     mod = import_module(mod_path)
     # Check for the class that derives from BaseCommand... if there is more then one class then throw error (note this is a current implementation detail)
     # because it is easier if their is only one command per file so that we can use the file name as the command name
     _has_found_a_valid_command = False
     initialized_obj = None
     for item in dir(mod):
         potential_obj = getattr(mod, item)
@@ -100,74 +124,82 @@
     if not initialized_obj:
         raise NoCommandFound
 
     return initialized_obj
 
 
 def initialize_command_container_module(mod_path: str) -> BaseCommandContainer:
+    """Given a path to a command, initialize the given command container.
+
+    Args:
+        mod_path (str): path to the command module
+
+    Raises:
+        TooManyCommandClasses: The module contained more than one command
+        NoCommandFound: No command was found in the module
+
+    Returns:
+        BaseCommandContainer
+    """
     mod = import_module(mod_path)
-    
 
     # Check for the class that derives from BaseCommandContainer... if there is more then one class then throw error (note this is a current implementation detail)
     # because it is easier if their is only one command per file so that we can use the file name as the command name
     _has_found_a_valid_command_container = False
     initialized_obj = None
     for item in dir(mod):
         potential_obj = getattr(mod, item)
         if (
             inspect.isclass(potential_obj)
             and issubclass(potential_obj, BaseCommandContainer)
             and not (potential_obj == BaseCommandContainer)
         ):
             if _has_found_a_valid_command_container:
                 # TODO better exception
-                return
+                raise TooManyCommandClasses
 
             _has_found_a_valid_command_container = True
 
             initialized_obj = potential_obj()
 
     if not initialized_obj:
         raise NoCommandFound(f"Could not find command Container")
 
-    
     return initialized_obj
 
 
 def _recursive_find_specified_command(
     command_list: List[str], search_path: str
 ) -> Tuple[bool, bool]:
     """Return if the given command list results in a potential found command or command container
 
-    Recursively check at each step if the next part in the command list is valid. If at the end of the 
+    Recursively check at each step if the next part in the command list is valid. If at the end of the
     list return that something was found. If at any point there is a missing link then return False.
 
     Args:
         command_list (List[str]): List of command parts
         search_path (str): Path the search from
 
     Returns:
         Tuple[bool, bool]: Found, Is_Command
     """
-    
 
     if len(command_list) == 1:
         # A location was specified and we are the final part of the command so the command must be a py file in this dir
         # of be a directory that has a command container
-        if os.path.isfile(os.path.join(search_path, command_list[0]+".py")):
-            return (True, True)
+        if os.path.isfile(os.path.join(search_path, command_list[0] + ".py")):
+            return True, True
 
         if os.path.isdir(os.path.join(search_path, command_list[0])):
             if os.path.join(os.path.join(search_path, command_list[0], "__init__.py")):
-                return (True, False)
-
-        return (False, False)
+                return True, False
 
+        return False, False
 
     next_command_part = command_list.pop(0)
 
     if not next_command_part in os.listdir(search_path):
-        return (False, False)
-
-    return _recursive_find_specified_command(command_list, os.path.join(search_path, next_command_part))
-
+        return False, False
 
+    return _recursive_find_specified_command(
+        command_list, os.path.join(search_path, next_command_part)
+    )
```

### Comparing `cdev-0.0.8/core/utils/exceptions.py` & `cdev-0.0.9/core/utils/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Base Exceptions to use within the framework
 
 These are the two exceptions that are expected to be used at the module level throughout Cdev. Within a module, it should have its own more precise
-exceptions, but they should be wrapped in these classes before being exposed at the module level. Any other error that is raised will be treated as 
-an uncaught exception and not the responsibility of other modules. 
+exceptions, but they should be wrapped in these classes before being exposed at the module level. Any other error that is raised will be treated as
+an uncaught exception and not the responsibility of other modules.
 
 Warning: Something is not correct but the process can continue running.
-Error: Something has reached a state that should terminate the process. 
+Error: Something has reached a state that should terminate the process.
 
 """
 import sys
 
 
 class Cdev_Warning(Exception):
     def __init__(self, msg: str) -> None:
         self.msg = msg
         super().__init__(self.msg)
 
 
 class Cdev_Error(Exception):
-    def __init__(self, msg: str, nested_exceptions: Exception=None) -> None:
+    def __init__(self, msg: str, nested_exceptions: Exception = None) -> None:
         self.msg = msg
         self.nested_exceptions = nested_exceptions
         super().__init__(self.msg)
 
 
 def end_process():
     sys.exit(1)
```

### Comparing `cdev-0.0.8/core/utils/file_manager.py` & `cdev-0.0.9/core/utils/file_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,29 +9,31 @@
 from pydantic import FilePath
 import os
 import shutil
 from typing import Dict, List, Tuple
 from core.constructs.cloud_output import cloud_output_dynamic_model
 
 from core.constructs.resource_state import Resource_State
-from core.utils.exceptions import Cdev_Error  
+from core.utils.exceptions import Cdev_Error
 from ..constructs.models import frozendict
 
+
 class CustomEncoder(json.JSONEncoder):
     """Custom JSON encoder for handling immutable data
 
-    Since we want to store state as immutable structures to make direct comparisons easier within the framework, 
+    Since we want to store state as immutable structures to make direct comparisons easier within the framework,
     we need to provide this encoder to denote how we want those structures stored as json. Using this encoder means
     that there is some information loss when making the obj a json (i.e. cant tell the difference between a frozenset vs
     list), therefor when loading the json back into the system, a custom utility should be used that reintroduces the
-    immutable structures back into the data. 
+    immutable structures back into the data.
 
     Args:
         json ([type]): [description]
     """
+
     def default(self, obj):
         if isinstance(obj, set):
             return list(obj)
 
         if isinstance(obj, frozenset):
             return list(obj)
 
@@ -41,23 +43,22 @@
         if isinstance(obj, tuple):
             print(f"Trying to serialize tuple {obj}")
             return list(obj)
 
         return json.JSONEncoder.default(self, obj)
 
 
-def safe_json_write(obj: Dict, fp: FilePath):
+def safe_json_write(obj: Dict, fp: FilePath) -> None:
     """
     Safely write files by first writing to a tmp file then copying to final location. This ensures that no file is
     partially written thus leaving a file in an unrecoverable state.
 
     Args:
         obj (Dict): The dictionary that should be written
         fp (FilePath): The path the file should be written at
-
     """
 
     tmp_fp = f"{fp}.tmp"
 
     if os.path.isfile(tmp_fp):
         os.remove(tmp_fp)
 
@@ -68,15 +69,17 @@
     except Exception as e:
         print(e)
         raise Cdev_Error(f"Could not write data as a json into tmp file; {obj}", e)
 
     try:
         shutil.copyfile(tmp_fp, fp)
     except Exception as e:
-        raise Cdev_Error(f"Could not copy tmp file into actual location; {tmp_fp} -> {fp}", e)
+        raise Cdev_Error(
+            f"Could not copy tmp file into actual location; {tmp_fp} -> {fp}", e
+        )
 
     os.remove(tmp_fp)
 
 
 def load_resource_state(fp: FilePath) -> Resource_State:
     """Load the Resource State correctly from the json file.
 
@@ -88,108 +91,125 @@
     because they are `resource_models`.
 
     For the `references`, all the structures in the list container should be loaded as immutable objects
     because they are `references_models`.
 
     for the `cloud_output`, all the structures in the list container should be loaded as immutable objects
     because they are `cloud_output`models`. They have a special structure that needs to be preserved so that
-    the exectution order of the operations are preserved. 
+    the execution order of the operations are preserved.
 
     Args:
         fp (FilePath): Path to the file storing the resource state
 
     Returns:
         Resource_State
 
     Raises:
         Cdev_Error
     """
 
     if not os.path.isfile(fp):
-        raise Cdev_Error(f"Trying to load resource state from {fp} but it does not exist")
+        raise Cdev_Error(
+            f"Trying to load resource state from {fp} but it does not exist"
+        )
 
     try:
         with open(fp, "r") as fh:
             _mutable_json = json.load(fh)
-    
+
     except Exception as e:
-        raise Cdev_Error(f"Trying to load resource state from {fp} but could not load the file as a json")
+        raise Cdev_Error(
+            f"Trying to load resource state from {fp} but could not load the file as a json"
+        )
 
-    for component in _mutable_json['components']:
-        # The actual resource and reference models need to be immutable data structures so that they can have a 
+    for component in _mutable_json["components"]:
+        # The actual resource and reference models need to be immutable data structures so that they can have a
         # __hash__ value.
 
         try:
-            if component.get('resources'):
-                component['resources'] = [_recursive_make_immutable(x) for x in component.get('resources')]
-
-            if component.get('references'):
-                component['references'] = [_recursive_make_immutable(x) for x in component.get('references')]
-
-            if component.get('cloud_output'):
-                component['cloud_output'] = _recursive_make_immutable(component.get('cloud_output'))
+            if component.get("resources"):
+                component["resources"] = [
+                    _recursive_make_immutable(x) for x in component.get("resources")
+                ]
+
+            if component.get("references"):
+                component["references"] = [
+                    _recursive_make_immutable(x) for x in component.get("references")
+                ]
+
+            if component.get("cloud_output"):
+                component["cloud_output"] = _recursive_make_immutable(
+                    component.get("cloud_output")
+                )
 
         except Exception as e:
-            raise Cdev_Error(f"Trying to load resource state from {fp} but could not make dict immutable", e)
-
+            raise Cdev_Error(
+                f"Trying to load resource state from {fp} but could not make dict immutable",
+                e,
+            )
 
     try:
         rv = Resource_State(**_mutable_json)
     except Exception as e:
-        raise Cdev_Error(f"Trying to load resource state from {fp} but could not serialized Dict into Resource_State", e)
+        raise Cdev_Error(
+            f"Trying to load resource state from {fp} but could not serialized Dict into Resource_State",
+            e,
+        )
 
     return rv
-    
+
+
 def _recursive_make_immutable(o):
     """Recursively transform an object into an immutable form
 
     This is a cdev core specific transformation that is used to convert Dict and List and other native python
     types into frozendict, frozenset, etc. The purpose is that the later set of objects are immutable in python
-    and therefor can be used to directly compare against eachother and be used as __hash__ able objects in
+    and therefor can be used to directly compare against each other and be used as __hash__ able objects in
     things like dicts and `networkx` DAGs.
 
-    Note the special case of handling Cloud Output Dict. These are identified as a dict with the key `id` that has 
-    a value `cdev_cloud_output`. 
+    Note the special case of handling Cloud Output Dict. These are identified as a dict with the key `id` that has
+    a value `cdev_cloud_output`.
 
     Args:
         o (Any): original object
 
     Returns:
         transformed_os
     """
 
     # Note this is designed to be specifically used within the loading of a resource state. Therefor,
     # we do not much error handling and let an error in the structure of the data be passed up all the
     # way to `load_resource_state`
 
-
     if isinstance(o, list):
         return frozenset([_recursive_make_immutable(x) for x in o])
     elif isinstance(o, dict):
 
         if "id" in o:
-            if o.get('id') == 'cdev_cloud_output':
-                
+            if o.get("id") == "cdev_cloud_output":
+
                 tmp = {k: _recursive_make_immutable(v) for k, v in o.items()}
-                if not o.get('output_operations'):
+                if not o.get("output_operations"):
                     return frozendict(tmp)
 
-                correctly_loaded_output_operations = _load_cloud_output_operations(o.get('output_operations'))
+                correctly_loaded_output_operations = _load_cloud_output_operations(
+                    o.get("output_operations")
+                )
 
-                tmp['output_operations'] = correctly_loaded_output_operations
-                
+                tmp["output_operations"] = correctly_loaded_output_operations
 
                 return frozendict(tmp)
 
-
         return frozendict({k: _recursive_make_immutable(v) for k, v in o.items()})
     return o
 
 
-def _load_cloud_output_operations(cloud_output_operations: List[List]) -> Tuple[Tuple,...]:
+def _load_cloud_output_operations(
+    cloud_output_operations: List[List],
+) -> Tuple[Tuple, ...]:
     """Load data in structure to conform to being a `cloud_output_operation`
 
     Note this is designed to be specifically used within the loading of a resource state. Therefor,
     we do not much error handling and let an error in the structure of the data be passed up all the
     way to `load_resource_state`
 
     Args:
@@ -198,13 +218,11 @@
     Returns:
         Operations: Tuple(Tuple(func_name, args, kwarg),...)
     """
 
     # Note this is designed to be specifically used within the loading of a resource state. Therefor,
     # we do not much error handling and let an error in the structure of the data be passed up all the
     # way to `load_resource_state`
-    
+
     return tuple(
-        [
-            (x[0], tuple(x[1]), frozendict(x[2])) for x in cloud_output_operations
-        ]
+        [(x[0], tuple(x[1]), frozendict(x[2])) for x in cloud_output_operations]
     )
```

### Comparing `cdev-0.0.8/core/utils/fs_manager/standard_library_names/python_3_6` & `cdev-0.0.9/core/utils/fs_manager/standard_library_names/python_3_7`

 * *Files 7% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 contextlib
 copy
 copyreg
 crypt
 csv
 ctypes
 curses
+dataclasses
 datetime
 dbm
 decimal
 dict
 difflib
 dis
 distutils
@@ -60,15 +61,14 @@
 faulthandler
 fcntl
 filecmp
 fileinput
 float
 fnmatch
 formatter
-fpectl
 fractions
 frozenset
 ftplib
 functools
 gc
 getopt
 getpass
```

### Comparing `cdev-0.0.8/core/utils/fs_manager/standard_library_names/python_3_7` & `cdev-0.0.9/core/utils/fs_manager/standard_library_names/python_3_8`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 collections
 colorsys
 compileall
 complex
 concurrent
 configparser
 contextlib
+contextvars
 copy
 copyreg
 crypt
 csv
 ctypes
 curses
 dataclasses
@@ -95,15 +96,14 @@
 json
 keyword
 linecache
 list
 locale
 logging
 lzma
-macpath
 mailbox
 mailcap
 marshal
 math
 memoryview
 mimetypes
 mmap
```

### Comparing `cdev-0.0.8/core/utils/fs_manager/standard_library_names/python_3_8` & `cdev-0.0.9/core/utils/fs_manager/standard_library_names/python_3_9`

 * *Files identical despite different names*

### Comparing `cdev-0.0.8/core/utils/hasher.py` & `cdev-0.0.9/core/utils/hasher.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-"""Utilities to provide a 'standardized' way of producing hashes to identify uniqueness. 
+"""Utilities to provide a 'standardized' way of producing hashes to identify uniqueness.
 
 These hash functions are **not**
 cryptographically secure and should not be used for that. Instead, these functions should simply be used to create hashes
-that will be used to track changes throughout the system. 
+that will be used to track changes throughout the system.
 """
 
 import hashlib
 import os
 from typing import List
 
 from pydantic.types import FilePath
@@ -48,48 +48,47 @@
 
     Returns:
         str: hash of the value
     """
     return hashlib.md5(val.encode()).hexdigest()
 
 
-def clear_file_cache():
+def clear_file_cache() -> None:
     """Clear the cache used by the `hash_file` utility."""
     FILE_CACHE.cache = {}
 
 
 def hash_file(fp: FilePath, bypass_cache: bool = False) -> str:
     """Hash a file given a path
 
-    Note that the implementation contains a reference to a cache. Since this utility is primarily 
+    Note that the implementation contains a reference to a cache. Since this utility is primarily
     used as an internal tool with the framework, the cache helps speeds things up when we know the file has
-    not changed. Note that the framework periodically flushes this cache when needed within the context of 
-    the execution of the framework using the `clear_file_cache` function. 
+    not changed. Note that the framework periodically flushes this cache when needed within the context of
+    the execution of the framework using the `clear_file_cache` function.
 
     If using this outside the confides of the framework, you can by pass the cache by setting the `bypass_cache`
     flag.
 
-    Note that the implementation returns a md5 hash of the bytes in the file. 
+    Note that the implementation returns a md5 hash of the bytes in the file.
 
     Args:
         fp (FilePath): Path to the file. Must be a resolvable path on the filesystem.
         bypass_cache (Optional[bool]): By pass the internal cache. Default False.
 
     Returns:
         str: hash of the file
 
     Raises:
         Cdev_Error
     """
     if fp in FILE_CACHE.cache and not bypass_cache:
         return FILE_CACHE.cache.get(fp)
 
-
     if not os.path.isfile(fp):
         raise Cdev_Error(f"Could not find file ({fp}) to hash", FileNotFoundError)
 
     with open(fp, "rb") as fh:
-        hash = hashlib.md5(fh.read()).hexdigest()
+        the_hash = hashlib.md5(fh.read()).hexdigest()
 
-    FILE_CACHE.cache[fp] = hash
+    FILE_CACHE.cache[fp] = the_hash
 
-    return hash
+    return the_hash
```

### Comparing `cdev-0.0.8/core/utils/logger.py` & `cdev-0.0.9/core/utils/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Utilities for generating logs of framework executions
 
 Note that logging should work in a duality within the framework. Meaning, that all functions within the framework
 should use the same logging utilities, but how they are provided will differ. All files will have a module
 level definition of a default logger, this will allow the utilities to log when called as simple functions
 through normal python execution. Within the framework, all executions will be wrapped in a global namespace
-that has a logger, therefor when the functions are called as part of the framework, it will be this logger 
+that has a logger, therefor when the functions are called as part of the framework, it will be this logger
 that is used.
 
 This is important in mainting that utility functions for the framework are not bound to used within the framework,
-but it also allows there to be dynamic functionality of how logs will be proccessed and displayed to the user. 
+but it also allows there to be dynamic functionality of how logs will be proccessed and displayed to the user.
 
 """
 import logging.config
 import logging
 import os
 from typing import Dict, Union
 
@@ -51,17 +51,17 @@
                 "show_path": False,
                 "show_time": False,
                 "rich_tracebacks": True,
             },
         },
         "loggers": {
             "core_file": {
-                "level": log_level, 
-                "handlers": ["fileHandler"], \
-                "propagate": False
+                "level": log_level,
+                "handlers": ["fileHandler"],
+                "propagate": False,
             },
             "core_rich": {
                 "level": log_level,
                 "handlers": ["richHandler"],
                 "propagate": False,
             },
             "core_simple": {
@@ -72,42 +72,46 @@
         },
         "root": {"level": "ERROR", "handlers": ["simpleHandler"]},
         "disable_existing_loggers": False,
     }
 
 
 class cdev_logger:
-    """Wrapper around pythons basic logger object to provide a layer of flexibility for logging. 
-    
+    """Wrapper around pythons basic logger object to provide a layer of flexibility for logging.
+
     Specifically, this will add the ability to always process logs into a JSON file for debugging errors, while
     also allowing the user to provide a flag to set a logging level to display to the user.
 
     It will implement the functions of a Logger obj
     https://docs.python.org/3/library/logging.html#logging.Logger.propagate
 
 
     Note that when formating data into a log message, it must use '%' formatted strings instead of f
     strings. This is allows am optimization used by the logging library to not allocate strings unless the
-    log needs to be evaluated. Within the context of a framework, these allocations can add up. This should 
-    be enforced with code styling at the PR level. 
+    log needs to be evaluated. Within the context of a framework, these allocations can add up. This should
+    be enforced with code styling at the PR level.
 
-    Also note the optimization around formmatted logs. 
+    Also note the optimization around formmatted logs.
 
     For more info read https://docs.python.org/3/howto/logging.html#optimization
     """
 
-    def __init__(self, is_rich_formatted=True, show_logs: bool=False, logging_level: Union[str,int] = "ERROR") -> None:
+    def __init__(
+        self,
+        is_rich_formatted=True,
+        show_logs: bool = False,
+        logging_level: Union[str, int] = "ERROR",
+    ) -> None:
 
         self.is_rich_formatted = is_rich_formatted
         self.show_logs = show_logs
-        
+
         log_info = _create_logging_settings(logging_level)
 
-        fp = os.path.join(os.getcwd(), log_info.get('filename'))
-    
+        fp = os.path.join(os.getcwd(), log_info.get("filename"))
 
         if not os.path.isfile(fp):
             if not os.path.isdir(os.path.dirname(os.path.dirname(fp))):
                 os.mkdir(os.path.dirname(os.path.dirname(fp)))
 
             if not os.path.isdir(os.path.dirname(fp)):
                 os.mkdir(os.path.dirname(fp))
@@ -116,102 +120,85 @@
                 os.utime(fp, None)
 
         logging.config.dictConfig(log_info)
         self._json_logger = logging.getLogger("core_file")
         self._simple_logger = logging.getLogger("core_simple")
         self._rich_logger = logging.getLogger("core_rich")
 
-    def _write_log(self, *args, func_name: str, original_msg: str, formatted_msg: str = "",  **kw_args):
+    def _write_log(
+        self,
+        *args,
+        func_name: str,
+        original_msg: str,
+        formatted_msg: str = "",
+        **kw_args,
+    ) -> None:
         # Always write a log to the json file
         getattr(self._json_logger, func_name)(original_msg, *args, **kw_args)
         if self.show_logs:
             # We need to write logs to console
             # Either write a plain log or rich formatted log to the console
             if not self.is_rich_formatted:
                 getattr(self._simple_logger, func_name)(original_msg, *args, **kw_args)
             else:
                 getattr(self._rich_logger, func_name)(formatted_msg, *args, **kw_args)
 
-
-    def debug(self, msg, *args, **kw_args):
+    def debug(self, msg, *args, **kw_args) -> None:
         if self.is_rich_formatted:
             self._write_log(
                 *args,
-                func_name="debug", 
-                original_msg=msg, 
+                func_name="debug",
+                original_msg=msg,
                 formatted_msg=f"[bold blue]{msg}",
-                **kw_args
+                **kw_args,
             )
 
         else:
-            self._write_log(
-                *args,
-                func_name="debug", 
-                original_msg=msg, 
-                **kw_args
-            )
-
+            self._write_log(*args, func_name="debug", original_msg=msg, **kw_args)
 
     def info(self, msg, *args, **kw_args):
         if self.is_rich_formatted:
             self._write_log(
                 *args,
-                func_name="info", 
-                original_msg=msg, 
+                func_name="info",
+                original_msg=msg,
                 formatted_msg=f"[bold blue]{msg}",
-                **kw_args
+                **kw_args,
             )
 
         else:
-            self._write_log(
-                *args,
-                func_name="info", 
-                original_msg=msg, 
-                **kw_args
-            )
+            self._write_log(*args, func_name="info", original_msg=msg, **kw_args)
 
-
-    def warning(self, msg, *args, **kw_args):
+    def warning(self, msg, *args, **kw_args) -> None:
         if self.is_rich_formatted:
             self._write_log(
                 *args,
-                func_name="warning", 
-                original_msg=msg, 
+                func_name="warning",
+                original_msg=msg,
                 formatted_msg=f"[bold yellow blink]{msg}",
-                **kw_args
+                **kw_args,
             )
 
         else:
-            self._write_log(
-                *args,
-                func_name="warning", 
-                original_msg=msg, 
-                **kw_args
-            )
-            
+            self._write_log(*args, func_name="warning", original_msg=msg, **kw_args)
 
-    def error(self, msg, *args, **kw_args):
+    def error(self, msg, *args, **kw_args) -> None:
         if self.is_rich_formatted:
             self._write_log(
                 *args,
                 func_name="error",
                 original_msg=msg,
                 formatted_msg=f"[bold red blink]:cross_mark: :cross_mark: :cross_mark: {msg} :cross_mark: :cross_mark: :cross_mark:",
-                **kw_args
+                **kw_args,
             )
 
         else:
-            self._write_log(
-                *args,
-                func_name="error",
-                original_msg=msg,
-                **kw_args
-            )
+            self._write_log(*args, func_name="error", original_msg=msg, **kw_args)
 
-    def exception(self, msg):
+    def exception(self, msg) -> None:
         self._write_log("exception", msg, msg)
 
 
 class global_log_container:
     def __init__(self, logger: cdev_logger) -> None:
         self._logger = logger
 
@@ -219,34 +206,30 @@
     def is_rich_formatted(self) -> bool:
         return self._logger.is_rich_formatted
 
     @property
     def show_logs(self) -> bool:
         return self._logger.show_logs
 
-    def debug(self, msg, *args, **kw_args):
+    def debug(self, msg, *args, **kw_args) -> None:
         self._logger.debug(msg, *args, **kw_args)
 
-    def info(self, msg, *args, **kw_args):
+    def info(self, msg, *args, **kw_args) -> None:
         self._logger.info(msg, *args, **kw_args)
 
-    def warning(self, msg, *args, **kw_args):
+    def warning(self, msg, *args, **kw_args) -> None:
         self._logger.warning(msg, *args, **kw_args)
-        
-    def error(self, msg, *args, **kw_args):
+
+    def error(self, msg, *args, **kw_args) -> None:
         self._logger.error(msg, *args, **kw_args)
 
-    def exception(self, msg):
+    def exception(self, msg) -> None:
         self._logger.exception(msg)
-        
 
-log = global_log_container(cdev_logger())
 
+log = global_log_container(cdev_logger())
 
 
-def set_global_logger(new_logger: cdev_logger):
+def set_global_logger(new_logger: cdev_logger) -> None:
     global log
 
     log._logger = new_logger
-
-
-
```

### Comparing `cdev-0.0.8/core/utils/module_loader.py` & `cdev-0.0.9/core/utils/module_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 import importlib
 from types import ModuleType
 import sys
 from typing import TextIO
 import inspect
 
 
-def import_module(module_name: str, denote_output: bool = False, override_stdout: bool = True) -> ModuleType:
+def import_module(
+    module_name: str, denote_output: bool = False, override_stdout: bool = True
+) -> ModuleType:
     """Helper function for dynamically loading python modules.
-    
-    This function should be used whenever a python module needs to be dynamically loaded within the framework. 
-    
+
+    This function should be used whenever a python module needs to be dynamically loaded within the framework.
+
     For more information about python modules see https://docs.python.org/3/tutorial/modules.html. Any changes
     to the PYTHONPATH needed to find the module should be done before this function is called.
-    
-    Arguments:
+
+    Args:
         module_name (str): The python module to be loaded. Note that this is not a file path. It is the name of a module that can be loaded.
 
     Raises:
         Exception
     """
 
     if denote_output:
@@ -68,17 +70,17 @@
         if not item_name == class_name:
             continue
 
         potential_obj = getattr(mod, item_name)
         if inspect.isclass(potential_obj):
             return potential_obj
 
-        
     raise Exception
 
+
 class override_sys_out(TextIO):
-   
-    encoding = sys.__stdout__.encoding 
 
-    def write(s: str):
+    encoding = sys.__stdout__.encoding
+
+    def write(s: str) -> None:
         if len(s) > 0 and not s == "\n":
             sys.__stdout__.write(f"> {s}\n")
```

### Comparing `cdev-0.0.8/core/utils/paths.py` & `cdev-0.0.9/core/utils/paths.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,74 @@
 """Utilities to help work with filesystem paths within the framework.
 
 
 To make projects work on multiple developers machines, it is important that paths that
-need to be stored in the state be written as relative paths. The relative paths can be 
+need to be stored in the state be written as relative paths. The relative paths can be
 started from two places: Workspace and Intermediate.
 
-The Workspace base is the base folder for all information that is unique to the current work 
+The Workspace base is the base folder for all information that is unique to the current work
 space. This will be default be the directory that a cli command is issued from. Changing
 this value should be done with caution and understanding of how to framework/cli bootstraps
 itself.
 
 
 The Intermediate base is the base folder for any artifacts that are created by the framework
 that need to be uploaded to the cloud. Any file made in this folder should be able to be deleted
 and recreated without affecting the larger framework. Right now this folder will be within the
 wWorkspace folder, but it is helpful to have the location as a seperate entity to make it possible
 in the future to have a smart implementation of a cache of artifacts that can be shared across multiple
 workspaces.
 
 
 
-TODO: Make a custom type that denotes a path is a relative path to the workspace. 
+TODO: Make a custom type that denotes a path is a relative path to the workspace.
 This could be a pydantic type that way the constraints are validated at runtime.
-This is a important part to improve the DX of the working with library. 
+This is a important part to improve the DX of the working with library.
 """
 
 import os
 from pydantic import DirectoryPath
 from pydantic.types import FilePath
 
 from core.constructs.workspace import Workspace
 
+
 def get_relative_to_workspace_path(fullpath: FilePath) -> str:
-    """Generate a relative path starting from the base path of the workspace. 
-    
-    Note that the given path must be a descendent of the workspace path. 
+    """Generate a relative path starting from the base path of the workspace.
+
+    Note that the given path must be a descendent of the workspace path.
 
     Args:
         fullpath (str): Path to convert to a relative path
 
     Returns:
         str: Relative to the Workspace path
     """
 
     base_path = Workspace.instance().settings.BASE_PATH
     return os.path.relpath(fullpath, start=base_path)
 
 
 def get_relative_to_intermediate_path(fullpath: str) -> str:
     """
-    Generate a relative path starting from the intermediate directory of the workspace. The given path must be a descendent of the intermediate directory. 
+    Generate a relative path starting from the intermediate directory of the workspace. The given path must be a descendent of the intermediate directory.
 
     Args:
         fullpath (str): Path to convert to a relative path
 
     Returns:
         str: Relative to the intermediate path path
     """
     intermediate_path = Workspace.instance().settings.INTERMEDIATE_FOLDER_LOCATION
-    return os.path.relpath(
-        fullpath, start=intermediate_path
-    )
+    return os.path.relpath(fullpath, start=intermediate_path)
 
 
 def get_full_path_from_workspace_base(relative_path: str) -> FilePath:
     """
-    Given a relative path from the workspace path, create the full absolute path on the current filesystem. 
+    Given a relative path from the workspace path, create the full absolute path on the current filesystem.
 
     Args:
         relative_path (str): Relative Path from the workspace path.
 
     Returns:
         FilePath: Absolute path the file.
     """
@@ -78,56 +77,51 @@
         base_path,
         relative_path,
     )
 
 
 def get_full_path_from_intermediate_base(relative_path: str) -> FilePath:
     """
-    Given a relative path from the intermediate folder, create the full absolute path on the current filesystem. 
+    Given a relative path from the intermediate folder, create the full absolute path on the current filesystem.
 
     Args:
         relative_path (str): Relative Path from the workspace path.
 
     Returns:
         FilePath: Absolute path the file.
     """
     intermediate_path = Workspace.instance().settings.INTERMEDIATE_FOLDER_LOCATION
-    return os.path.join(
-        intermediate_path, relative_path
-    )
+    return os.path.join(intermediate_path, relative_path)
 
 
 def is_in_workspace(full_path: str) -> bool:
-    """Check if a given file is within the workspace filespace
+    """Check if a given file is within the workspace file space
 
     Args:
-        full_path (str): [description]
+        full_path (str): The full path to check
 
     Returns:
-        bool: [description]
+        bool
     """
     base_path = Workspace.instance().settings.BASE_PATH
-    return os.path.commonprefix(
-        [full_path, base_path]
-    ) == base_path
+    return os.path.commonprefix([full_path, base_path]) == base_path
 
 
 def is_in_intermediate(full_path: str) -> bool:
-    """Check if a given file is within the intermediate filespace
+    """Check if a given file is within the intermediate file space
 
     Args:
-        full_path (str): [description]
+        full_path (str): The full path to check
 
     Returns:
-        bool: [description]
+        bool
     """
     intermediate_path = Workspace.instance().settings.INTERMEDIATE_FOLDER_LOCATION
-    return os.path.commonprefix(
-        [full_path, intermediate_path]
-    ) == intermediate_path
+    t = os.path.commonprefix([full_path, intermediate_path])
+    return t == str(intermediate_path)
 
 
 def get_workspace_path() -> DirectoryPath:
     """Get the Workspace path
 
     Returns:
         DirectoryPath: Path to workspace directory
@@ -142,36 +136,76 @@
     Returns:
         DirectoryPath: Path to intermediate directory
     """
     intermediate_path = Workspace.instance().settings.INTERMEDIATE_FOLDER_LOCATION
     return intermediate_path
 
 
+def create_path_from_workspace(desired_path: DirectoryPath) -> None:
+
+    if not is_in_workspace(desired_path):
+        raise Exception
+
+    if os.path.isdir(desired_path):
+        return
+
+    relative_parts = get_relative_to_workspace_path(desired_path).split("/")
+
+    create_path(get_workspace_path(), relative_parts)
+
+
 def create_path(startingpath, fullpath) -> DirectoryPath:
     """This functions takes a starting path and list of child dir and makes them all
 
-    
     Example
 
         create_path("./basedir", ["sub1", "sub2"])
 
         creates:\n
             ./basedir/sub1/\n
             ./basedir/sub1/sub2\n
 
     Returns:
         DirectoryPath: the final path
-    
+
     """
 
     if not os.path.isdir(startingpath):
         raise Exception
 
     intermediate_path = startingpath
 
     for p in fullpath:
         if not os.path.isdir(os.path.join(intermediate_path, p)):
             os.mkdir(os.path.join(intermediate_path, p))
 
         intermediate_path = os.path.join(intermediate_path, p)
 
     return intermediate_path
+
+
+def touch_file(file_path: FilePath) -> None:
+    """Helper function to touch a file
+
+    Args:
+        file_path (FilePath)
+
+    Raises:
+        Exception: Directory does not exist
+    """
+    if not os.path.isdir(os.path.dirname(file_path)):
+        raise Exception(
+            f"Can not create {file_path} because {os.path.dirname(file_path)} is not a directory."
+        )
+
+    with open(file_path, "a"):
+        pass
+
+
+def mkdir(directory_path: DirectoryPath) -> None:
+    """Create a directory if it does not already exist.
+
+    Args:
+        directory_path (DirectoryPath)
+    """
+    if not os.path.isdir(directory_path):
+        os.mkdir(directory_path)
```

### Comparing `cdev-0.0.8/core/utils/topological_helper.py` & `cdev-0.0.9/core/utils/topological_helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,346 +1,488 @@
 """Utilities to help work with the Resource Dependency Graph.
 
 One of the core components of the Cdev Core framework is the Resource Dependency Graph. This graph is implemented
-using the `networkx` packages as it provides helpful utilities for working with graph data structures. 
+using the `networkx` packages as it provides helpful utilities for working with graph data structures.
 """
 
 from concurrent.futures import ThreadPoolExecutor, Future
 from enum import Enum
 
 from networkx.classes.digraph import DiGraph
 from networkx.classes.reportviews import NodeView
 
 
 from typing import Callable, Dict, List, Set, Tuple
 from time import sleep
 
-from core.constructs.resource import Resource_Change_Type, Resource_Reference_Change_Type, ResourceModel, Resource_Difference, Resource_Reference_Difference
+from core.constructs.resource import (
+    Resource_Change_Type,
+    Resource_Reference_Change_Type,
+    ResourceModel,
+    Resource_Difference,
+    Resource_Reference_Difference,
+)
 from core.constructs.cloud_output import OutputType, cloud_output_model
 from core.constructs.components import Component_Change_Type, Component_Difference
 from core.constructs.output_manager import OutputManager, OutputTask
 from core.constructs.models import frozendict
 
-deliminator = '+'
+from core.utils.operations import concatenate
+
+deliminator = "+"
+
 
 def find_parents(resource: ResourceModel) -> Tuple[List, List]:
     """Find any parents resources via any linked Cloud Output Models
 
-    If a resource constains the cloud output of another resource, the relationship
+    If a resource contains the cloud output of another resource, the relationship
     needs to be identified as a parent-child relationship with the Resource Dependency
     Graph.
 
     Args:
         resource (ResourceModel): Resource to look for any parents with
 
     Returns:
         Tuple[
             parent_resources: List[Tuple[ruuid, name]]
             parent_resources: List[Tuple[ruuid, name]]
         ]
     """
     resource_as_obj = resource.dict()
-    
+
     cloud_outputs = find_cloud_output(resource_as_obj)
 
-    parent_resources = [(x.ruuid,x.name) for x in cloud_outputs if x.type == OutputType.RESOURCE ]
-    parent_references = [(x.ruuid,x.name) for x in cloud_outputs if x.type == OutputType.REFERENCE]
-    
+    parent_resources = [
+        (x.ruuid, x.name) for x in cloud_outputs if x.type == OutputType.RESOURCE
+    ]
+    parent_references = [
+        (x.ruuid, x.name) for x in cloud_outputs if x.type == OutputType.REFERENCE
+    ]
 
     return parent_resources, parent_references
 
 
 def find_cloud_output(obj: dict) -> List[cloud_output_model]:
+    """Given an object representing the cloud output generate all the parent cloud output models
+
+    Args:
+        obj (dict)
+
+    Returns:
+        List[cloud_output_model]
+    """
 
     rv = _recursive_find_output(obj)
 
     return list(set(rv))
 
 
 def _recursive_find_output(obj) -> List[cloud_output_model]:
-    rv = []
-
-    if isinstance(obj, frozendict) or isinstance(obj, dict): 
-        
-        if "id" in obj and obj.get("id") == 'cdev_cloud_output':
-            rv.append(cloud_output_model(**obj))
+    if isinstance(obj, frozendict) or isinstance(obj, dict):
+        if "id" in obj and obj.get("id") == "cdev_cloud_output":
+            return [cloud_output_model(**obj)]
         else:
-            for k,v in obj.items():
-                if isinstance(v, frozendict) or isinstance(v, dict):
-                    if "id" in v and v.get("id") == 'cdev_cloud_output':
-                        rv.append(cloud_output_model(**v))
-                    else:
-                        rv.extend(_recursive_find_output(v))
+            return concatenate([_recursive_find_output(v) for _, v in obj.items()])
 
-                elif isinstance(v, frozenset) or isinstance(v, list):
-                    all_items_rendered = [_recursive_find_output(x) for x in v]
+    elif isinstance(obj, frozenset) or isinstance(obj, list):
+        return concatenate([_recursive_find_output(x) for x in obj])
 
-                    for item in all_items_rendered:
-                        rv.extend(item)
+    else:
+        return []
 
-        return rv
 
-    elif isinstance(obj, frozenset) or isinstance(obj, list):
-        all_items_rendered = [_recursive_find_output(x) for x in obj]
-                
-        for item in all_items_rendered:
-            rv.extend(item)
+def generate_sorted_resources(
+    differences: Tuple[
+        List[Component_Difference],
+        List[Resource_Difference],
+        List[Resource_Reference_Difference],
+    ]
+) -> DiGraph:
+    """Given the tuple of all differences, generate a DiGraph representing a topologically valid way of applying the changes.
 
-    return rv
+    Args:
+        differences (Tuple[ List[Component_Difference], List[Resource_Difference], List[Resource_Reference_Difference], ]): _description_
 
+    Raises:
+        Exception
 
-def generate_sorted_resources(differences: Tuple[List[Component_Difference], List[Resource_Difference], List[Resource_Reference_Difference]]) -> DiGraph:
+    Returns:
+        DiGraph
+    """
     # nx graphs work on the element level by using the __hash__ of objects added to the graph, so all the elements added to the graph should be a pydantic Model with
     # the 'frozen' feature set
     change_dag = DiGraph()
 
-
     component_differences = differences[0]
     resource_differences = differences[1]
     reference_differences = differences[2]
-    
 
-    component_ids = {_create_component_id(x.new_name):x for x in component_differences if x.action_type == Component_Change_Type.CREATE or x.action_type == Component_Change_Type.UPDATE_NAME or x.action_type == Component_Change_Type.UPDATE_IDENTITY}
-    component_ids.update({_create_component_id(x.previous_name):x for x in component_differences if x.action_type == Component_Change_Type.DELETE})
+    component_ids = {
+        _create_component_id(x.new_name): x
+        for x in component_differences
+        if x.action_type == Component_Change_Type.CREATE
+        or x.action_type == Component_Change_Type.UPDATE_NAME
+        or x.action_type == Component_Change_Type.UPDATE_IDENTITY
+    }
+    component_ids.update(
+        {
+            _create_component_id(x.previous_name): x
+            for x in component_differences
+            if x.action_type == Component_Change_Type.DELETE
+        }
+    )
+
+    resource_ids = {
+        _create_resource_id(
+            x.component_name, x.new_resource.ruuid, x.new_resource.name
+        ): x
+        for x in resource_differences
+        if x.action_type == Resource_Change_Type.UPDATE_IDENTITY
+        or x.action_type == Resource_Change_Type.CREATE
+        or x.action_type == Resource_Change_Type.UPDATE_NAME
+    }
+    resource_ids.update(
+        {
+            _create_resource_id(
+                x.component_name, x.previous_resource.ruuid, x.previous_resource.name
+            ): x
+            for x in resource_differences
+            if x.action_type == Resource_Change_Type.DELETE
+        }
+    )
+
+    reference_ids = {
+        _create_reference_id(
+            x.originating_component_name,
+            x.resource_reference.component_name,
+            x.resource_reference.ruuid,
+            x.resource_reference.name,
+        ): x
+        for x in reference_differences
+    }
 
-    
-    resource_ids = {_create_resource_id(x.component_name, x.new_resource.ruuid, x.new_resource.name):x for x in resource_differences if x.action_type == Resource_Change_Type.UPDATE_IDENTITY or x.action_type == Resource_Change_Type.CREATE or x.action_type == Resource_Change_Type.UPDATE_NAME}
-    resource_ids.update({_create_resource_id(x.component_name, x.previous_resource.ruuid, x.previous_resource.name):x for x in resource_differences if x.action_type == Resource_Change_Type.DELETE})
-
-    
-    reference_ids = {_create_reference_id(x.originating_component_name, x.resource_reference.component_name, x.resource_reference.ruuid, x.resource_reference.name):x for x in reference_differences}
-
-    
     for _, component in component_ids.items():
         change_dag.add_node(component)
 
-
     for _, resource in resource_ids.items():
         change_dag.add_node(resource)
 
         component_id = _create_component_id(resource.component_name)
 
         if component_id in component_ids:
-            if resource.action_type == Resource_Change_Type.DELETE and component_ids.get(component_id).action_type == Component_Change_Type.DELETE:
+            if (
+                resource.action_type == Resource_Change_Type.DELETE
+                and component_ids.get(component_id).action_type
+                == Component_Change_Type.DELETE
+            ):
                 # Since these are both deletes, it should happen in the reverse order
-                change_dag.add_edge(resource,component_ids.get(component_id))
+                change_dag.add_edge(resource, component_ids.get(component_id))
 
             else:
                 change_dag.add_edge(component_ids.get(component_id), resource)
         else:
-            raise Exception(f"There should always be a change in a component for a resource change {resource}")
-
-        parent_resources, parent_references = find_parents(resource.new_resource) if not resource.action_type == Resource_Change_Type.DELETE else find_parents(resource.previous_resource)
+            raise Exception(
+                f"There should always be a change in a component for a resource change {resource}"
+            )
+
+        parent_resources, parent_references = (
+            find_parents(resource.new_resource)
+            if not resource.action_type == Resource_Change_Type.DELETE
+            else find_parents(resource.previous_resource)
+        )
 
         if not parent_resources and not parent_references:
             continue
 
-
         for parent_ruuid, parent_name in parent_resources:
             # Parent resources must be in the same component
-            
+
             # Cloud outputs of a resource will always be from the same component
-            parent_resource_id = _create_resource_id(resource.component_name, parent_ruuid, parent_name)
+            parent_resource_id = _create_resource_id(
+                resource.component_name, parent_ruuid, parent_name
+            )
 
             if parent_resource_id in resource_ids:
                 if resource.action_type == Resource_Change_Type.DELETE:
                     # Since this is a delete, it should happen in the reverse order
                     change_dag.add_edge(resource, resource_ids.get(parent_resource_id))
 
                 else:
                     # Make this resource change a child of the parent resource change
                     change_dag.add_edge(resource_ids.get(parent_resource_id), resource)
 
         for parent_ruuid, parent_name in parent_references:
-            parent_reference_id = _create_reference_id(resource.component_name, resource.component_name, parent_ruuid, parent_name)
+            parent_reference_id = _create_reference_id(
+                resource.component_name,
+                resource.component_name,
+                parent_ruuid,
+                parent_name,
+            )
 
             if parent_reference_id in reference_ids:
                 if resource.action_type == Resource_Change_Type.DELETE:
                     # Since this is a delete, it should happen in the reverse order
                     change_dag.add_edge(resource, resource_ids.get(parent_reference_id))
 
                 else:
                     change_dag.add_edge(resource_ids.get(parent_reference_id), resource)
 
     for _, reference in reference_ids.items():
         change_dag.add_node(reference)
 
         # Reference changes should be a child to an Update Identity component diff
-        originating_component_id = _create_component_id(reference.originating_component_name)
+        originating_component_id = _create_component_id(
+            reference.originating_component_name
+        )
 
         if originating_component_id in component_ids:
             change_dag.add_edge(component_ids.get(originating_component_id), reference)
 
         else:
-            raise Exception(f"There should always be a change in a component for a reference change {resource}")
-
+            raise Exception(
+                f"There should always be a change in a component for a reference change {resource}"
+            )
 
         # Reference change should also be a child to any change to the referenced resource
-        resource_id = _create_resource_id(reference.resource_reference.component_name, reference.resource_reference.ruuid, reference.resource_reference.name)
+        resource_id = _create_resource_id(
+            reference.resource_reference.component_name,
+            reference.resource_reference.ruuid,
+            reference.resource_reference.name,
+        )
         if resource_id in resource_ids:
             # If there is also a change to the component this reference is apart of then the changes need to be ordered
             if reference.action_type == Resource_Reference_Change_Type.CREATE:
-                if resource_ids.get(resource_id).action_type == Resource_Change_Type.DELETE:
+                if (
+                    resource_ids.get(resource_id).action_type
+                    == Resource_Change_Type.DELETE
+                ):
                     # We can not create a reference if that resource is currently being destroyed.
-                    raise Exception(f"Trying to reference a resource that is being deleted {reference} -> {resource_id}")
+                    raise Exception(
+                        f"Trying to reference a resource that is being deleted {reference} -> {resource_id}"
+                    )
 
-                # Since the reference is being created, we should perform the operation after the changes to the underlying resource 
+                # Since the reference is being created, we should perform the operation after the changes to the underlying resource
                 change_dag.add_edge(resource_ids.get(resource_id), reference)
 
             else:
                 change_dag.add_edge(reference, resource_ids.get(resource_id))
 
         else:
             # Since the original resource is not in the change set, it should be checked to be sure that it is accessible from the backend
             pass
-            
 
     return change_dag
 
 
-def _create_component_id(component_name: str ) -> str:
-    # Component Differences will be identified by the key component<deliminator><component_name>
-    return f'component{deliminator}{component_name}'
+def _create_component_id(component_name: str) -> str:
+    """Create the id for a given component
+
+    Component Differences will be identified by the key component<deliminator><component_name>
+
+    Args:
+        component_name (str)
+
+    Returns:
+        str
+    """
+    return f"component{deliminator}{component_name}"
 
 
 def _create_resource_id(component_name: str, ruuid: str, name: str) -> str:
-    # Resource Differences will be identified by the key resource<deliminator><ruuid><deliminator><name>
-    return f'resource{deliminator}{component_name}{deliminator}{ruuid}{deliminator}{name}'
+    """Create id for a given resource
 
+    Resource Differences will be identified by the key resource<deliminator><ruuid><deliminator><name>
 
-def _create_reference_id(originating_component_name: str, component_name: str, ruuid: str, name: str) -> str:
-    # Reference Differences will be identified by the key reference<deliminator><ruuid><deliminator><name>
-    return f'reference{deliminator}{originating_component_name}{deliminator}{component_name}{deliminator}{ruuid}{deliminator}{name}'
+    Args:
+        component_name (str): component the resource is in
+        ruuid (str): resource type id
+        name (str): name of the resource
 
+    Returns:
+        str
+    """
+    return (
+        f"resource{deliminator}{component_name}{deliminator}{ruuid}{deliminator}{name}"
+    )
+
+
+def _create_reference_id(
+    originating_component_name: str, component_name: str, ruuid: str, name: str
+) -> str:
+    """Create id for a given reference
+
+    Reference Differences will be identified by the key reference<deliminator><ruuid><deliminator><name>
+
+    Args:
+        originating_component_name (str): component original resource resides in
+        component_name (str): component the reference is in
+        ruuid (str): resource type id
+        name (str): name of the reference
 
+    Returns:
+        str: _description_
+    """
+    return f"reference{deliminator}{originating_component_name}{deliminator}{component_name}{deliminator}{ruuid}{deliminator}{name}"
 
 
 class node_state(str, Enum):
     UNPROCESSED = "UNPROCESSED"
     PROCESSING = "PROCESSING"
     PROCESSED = "PROCESSED"
     ERROR = "ERROR"
     PARENT_ERROR = "PARENT_ERROR"
 
 
-def topological_iteration(dag: DiGraph, process: Callable[[NodeView], None], failed_parent_handler: Callable[[NodeView], None]=None, thread_count: int = 1, interval: float = .3, pass_through_exceptions: bool = False):
-    """Execute the `process` over a DAG in a topologically constrained way. 
-    
-    This means that the `process` will not be executed on a node until the `process` has been executed on all parents of that node. 
-    
-    If the `process` throws an Exception when executing on a Node, then any child nodes will not be executed (if provided, the 
-    failed_parent_handler will be executed on the child nodes). 
-    
-    This iteration supports multiple threads via the `thread_count` param. Multiple threads can speed up the total iteration time if the `process` 
+def topological_iteration(
+    dag: DiGraph,
+    process: Callable[[NodeView], None],
+    failed_parent_handler: Callable[[NodeView], None] = None,
+    thread_count: int = 1,
+    interval: float = 0.3,
+    pass_through_exceptions: bool = False,
+) -> None:
+    """Execute the `process` over a DAG in a topologically constrained way.
+
+    This means that the `process` will not be executed on a node until the `process` has been executed on all parents of that node.
+
+    If the `process` throws an Exception when executing on a Node, then any child nodes will not be executed (if provided, the
+    failed_parent_handler will be executed on the child nodes).
+
+    This iteration supports multiple threads via the `thread_count` param. Multiple threads can speed up the total iteration time if the `process`
     is not CPU bound and there are non-dependant paths through the DAG. Note that the `process` provided should be thread safe when using multiple threads.
 
     Args:
         dag (DiGraph): The graph to execute over.
         process (Callable[[NodeView], None]): The function to call on each Node.
         failed_parent_handler (Callable[[NodeView], None], optional): A function to call on Nodes that do not execute because a parent failed.
-        thread_count (int, optional): [description]. Defaults to 1 
+        thread_count (int, optional): [description]. Defaults to 1
         interval (float, optional): Interval (in seconds) to poll threads for completion. Defaults to .3
     """
-    
+
     all_children: Set[NodeView] = set(x[1] for x in dag.edges)
     all_nodes: Set[NodeView] = set(x for x in dag.nodes())
 
     # starting nodes are those that have no parents
     starting_nodes = all_nodes - all_children
-    
+
     nodes_to_process: list[NodeView] = []
     nodes_to_process.extend(starting_nodes)
 
     _processing_future_to_resource: Dict[Future, NodeView] = {}
 
     # Keep track of the state of all nodes to determine when the entire DAG has been traversed
-    _node_to_state: Dict[NodeView,node_state] = {x:node_state.UNPROCESSED for x in all_nodes}
+    _node_to_state: Dict[NodeView, node_state] = {
+        x: node_state.UNPROCESSED for x in all_nodes
+    }
 
     executor = ThreadPoolExecutor(thread_count)
-    
+
     # While any node is unprocessed or still processing
-    while any(_node_to_state.get(x) == node_state.UNPROCESSED or _node_to_state.get(x) == node_state.PROCESSING for x in all_nodes):
-        
+    while any(
+        _node_to_state.get(x) == node_state.UNPROCESSED
+        or _node_to_state.get(x) == node_state.PROCESSING
+        for x in all_nodes
+    ):
+
         # Pull any ready nodes to be processed and add them to the thread pool
         for _ in range(0, len(nodes_to_process)):
             node_to_process = nodes_to_process.pop(0)
             future = executor.submit(process, node_to_process)
 
             _processing_future_to_resource[future] = node_to_process
             _node_to_state[node_to_process] = node_state.PROCESSING
 
-        
         # Check if any of the futures are finished and then make decisions about their children from the rv of the future
         for fut, node in _processing_future_to_resource.copy().items():
             # Note python throws runtime error if you change a dict size while iterating so use a copy for now.
             # TODO: Check if there is a more optimized way to do this
 
             if not fut.done():
                 # Still processing
                 continue
 
-
             try:
                 result = fut.result()
 
                 # No exceptions raised so process completed correctly
                 _node_to_state[node] = node_state.PROCESSED
 
                 children = dag.successors(node)
 
                 for child in children:
                     # If any of the parents of the child have not been processed, than the child node is not ready to be processed
-                    if any(not _node_to_state.get(x) == node_state.PROCESSED for x in dag.predecessors(child)):
+                    if any(
+                        not _node_to_state.get(x) == node_state.PROCESSED
+                        for x in dag.predecessors(child)
+                    ):
                         continue
-                    
+
                     nodes_to_process.append(child)
 
             except Exception as e:
                 # Since this returned a error need to mark all children as unable to deploy
                 _node_to_state[node] = node_state.ERROR
-                
-                  
+
                 # mark an descdents of this node as unable to process
-                _recursively_mark_parent_failure(_node_to_state, dag, node, handler=failed_parent_handler)
+                _recursively_mark_parent_failure(
+                    _node_to_state, dag, node, handler=failed_parent_handler
+                )
 
                 if pass_through_exceptions:
-                    raise e 
-                         
+                    raise e
 
             # Remove the future from the dictionary
             _processing_future_to_resource.pop(fut)
 
         sleep(interval)
 
-
     executor.shutdown()
 
 
-def _recursively_mark_parent_failure(_node_to_state: Dict[NodeView, node_state], dag: DiGraph, parent_node: NodeView, handler: Callable[[NodeView, OutputTask], None]=None, pass_through_exceptions: bool = False) -> None:
+def _recursively_mark_parent_failure(
+    _node_to_state: Dict[NodeView, node_state],
+    dag: DiGraph,
+    parent_node: NodeView,
+    handler: Callable[[NodeView, OutputTask], None] = None,
+    pass_through_exceptions: bool = False,
+) -> None:
+    """Recursively mark all descendent of a failure
+
+    Args:
+        _node_to_state (Dict[NodeView, node_state]): mapping between nodes and final states
+        dag (DiGraph): graph
+        parent_node (NodeView): starting node
+        handler (Callable[[NodeView, OutputTask], None], optional): function to call on children. Defaults to None.
+        pass_through_exceptions (bool, optional): suppress any additional errors. Defaults to False.
+
+    Raises:
+        Exception
+    """
 
     if parent_node not in _node_to_state:
-        raise Exception(f"trying to mark node ({parent_node}) but cant not find it in given dict")
+        raise Exception(
+            f"trying to mark node ({parent_node}) but cant not find it in given dict"
+        )
 
-    
     children = dag.successors(parent_node)
 
     for child in children:
 
         if child not in _node_to_state:
-            raise Exception(f"trying to mark node ({child}) but cant not find it in given dict")
-        
+            raise Exception(
+                f"trying to mark node ({child}) but cant not find it in given dict"
+            )
+
         _node_to_state[child] = node_state.PARENT_ERROR
 
         if handler:
             # Call a handler that does extra busines logic for items that fail because of their parent
             try:
                 handler(child)
 
             except Exception as e:
-                #handler threw exception but we should continue
-                
-                if pass_through_exceptions:
-                    raise e 
+                # handler threw exception but we should continue
 
+                if pass_through_exceptions:
+                    raise e
 
         _recursively_mark_parent_failure(_node_to_state, dag, child)
-
```

### Comparing `cdev-0.0.8/serverless_parser/__init__.py` & `cdev-0.0.9/serverless_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `cdev-0.0.8/serverless_parser/parser.py` & `cdev-0.0.9/serverless_parser/parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-import os
-import hashlib
-from typing import List
-from pydantic.types import DirectoryPath, FilePath
-
-from sortedcontainers import SortedDict
+from pydantic.types import DirectoryPath
 
 from .parser_objects import *
-from .import parser_utils as p_utils
+from . import parser_utils as p_utils
 from .parser_exceptions import *
 
 
-
 ## This file has the highest level functions for use by other modules. Only this file will expose functionality to other modules.
 
 
-def parse_functions_from_file(file_loc, include_functions=[], function_manual_includes={}, global_manual_includes=[], remove_top_annotation=False) -> file_information:
+def parse_functions_from_file(
+    file_loc,
+    include_functions=[],
+    function_manual_includes={},
+    global_manual_includes=[],
+    remove_top_annotation=False,
+) -> file_information:
     try:
         file_information = p_utils.get_file_information(
-            file_loc, include_functions, function_manual_includes, global_manual_includes, remove_top_annotation)
+            file_loc,
+            include_functions,
+            function_manual_includes,
+            global_manual_includes,
+            remove_top_annotation,
+        )
     except InvalidDataError as e:
         file_information = None
         print(f"{type(e)} -> {e.message}")
     except CouldNotParseFileError as e:
         file_information = None
         print(f"{type(e.error)} -> {e.error.message}")
 
     return file_information
 
 
-
 def parse_file_for_dependencies(file_loc: DirectoryPath):
     return p_utils.get_file_imported_symbols(file_loc)
```

### Comparing `cdev-0.0.8/serverless_parser/parser_exceptions.py` & `cdev-0.0.9/serverless_parser/parser_exceptions.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 class CdevError(Exception):
     pass
 
 
-
 class CouldNotParseFileError(CdevError):
     def __init__(self, error):
         self.error = error
 
 
 class CdevFileNotFoundError(FileNotFoundError):
     def __init__(self, message):
@@ -14,11 +13,12 @@
 
 
 class InvalidParamError(CdevError):
     # This error should be thrown when anything is passed a wrong param
     def __init__(self, message):
         self.message = message
 
+
 class InvalidDataError(CdevError):
     # This error should be thrown when there is a problem with the integrity of data passed into a system
     def __init__(self, message):
         self.message = message
```

### Comparing `cdev-0.0.8/serverless_parser/parser_objects.py` & `cdev-0.0.9/serverless_parser/parser_objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,97 +5,102 @@
 import tokenize
 import re
 import hashlib
 from typing import List
 
 from sortedcontainers import SortedList
 
-INCLUDE_REGEX = '^#include <(\w+)>$'
+INCLUDE_REGEX = "^#include <(\w+)>$"
+
 
 def _hash_line_numbers(line_no_1: int, line_no_2: int) -> str:
     s_numbers = f"{line_no_1}:{line_no_2}"
-    return int.from_bytes( hashlib.md5(s_numbers.encode()).digest(), byteorder='big')
+    return int.from_bytes(hashlib.md5(s_numbers.encode()).digest(), byteorder="big")
 
 
-class parsed_function():
+class parsed_function:
     """
-        This class represents the information for a parsed function. It mostly is used to house a function that can keep track of the line numbers.
+    This class represents the information for a parsed function. It mostly is used to house a function that can keep track of the line numbers.
     """
 
     def __init__(self, name):
         self.name: str = name
         self.needed_line_numbers = SortedList(key=lambda x: x[0])
 
         # set of imported packages
         self.imported_packages: str = set()
 
-        # some packages come with the lambda runtime so they do not need to be packaged into a layer so we need to make a new set with 
+        # some packages come with the lambda runtime so they do not need to be packaged into a layer so we need to make a new set with
         # just packages we need to actually package into layers
         # EX: 'os' does not need to be packaged into a layer
         self.needed_imports = set()
 
         self.needed_imports_hash = ""
 
-    def __eq__(self):
+    def __eq__(self) -> bool:
         return self.name == self.name
 
-    def add_line_numbers(self, line_no):
+    def add_line_numbers(self, line_no) -> None:
         # Use a sorted list
         self.needed_line_numbers.add(line_no)
 
-    def get_line_numbers(self):
+    def get_line_numbers(self) -> SortedList:
         return self.needed_line_numbers
 
-    def get_line_numbers_serializeable(self):
+    def get_line_numbers_serializeable(self) -> List:
         return list(self.needed_line_numbers)
 
-    def add_import(self, global_import_obj):
-        #self.add_line_numbers(global_import_obj.get_line_no())
+    def add_import(self, global_import_obj) -> None:
+        # self.add_line_numbers(global_import_obj.get_line_no())
         # original package will be how it is denoted in the import statement
         # for absolute packages we only want the top level name (absolutes don't start with '.')
         # for relative packages we want the entire name (relatives start with '.')
-        top_level_package_name = global_import_obj.original_package.split('.')[0] if not global_import_obj.original_package.startswith('.') else global_import_obj.original_package
+        top_level_package_name = (
+            global_import_obj.original_package.split(".")[0]
+            if not global_import_obj.original_package.startswith(".")
+            else global_import_obj.original_package
+        )
         self.imported_packages.add(top_level_package_name)
 
 
 class GlobalStatementType(Enum):
     STANDARD = 1
     FUNCTION = 2
     IMPORT = 3
     CLASS_DEF = 4
 
 
-class GlobalStatement():
+class GlobalStatement:
     """
-        This class represents the extra information for the global statements of a file. A global statement are the first children in the 
-        ast for a file. 
+    This class represents the extra information for the global statements of a file. A global statement are the first children in the
+    ast for a file.
     """
-    def __init__(self, node, line_no, symbols):
+
+    def __init__(self, node, line_no, symbols) -> None:
         self.line_no = line_no
 
         self.set_symbols(symbols)
 
         self.node = node
 
         self.hashed = _hash_line_numbers(self.line_no[0], self.line_no[1])
 
         # The type of statement
         self.statement_type = GlobalStatementType.STANDARD
 
-
     def __hash__(self):
         return self.hashed
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:
         return self.hashed == other.hashed
 
     def __repr__(self):
         return f"<statement at {self.line_no[0]} thru {self.line_no[1]}>"
 
-    def set_symbols(self, symbols: List[str]):
+    def set_symbols(self, symbols: List[str]) -> None:
         self.symbols = symbols
 
     def get_symbols(self) -> List[str]:
         return self.symbols
 
     def get_line_no(self):
         return self.line_no
@@ -124,65 +129,62 @@
     def get_type(self):
         return GlobalStatementType.IMPORT
 
 
 class FunctionStatement(GlobalStatement):
 
     # function name is a func
-    func_name = ""
+    func_name: str = ""
 
-    has_decremented = False
+    has_decremented: bool = False
 
-    def __init__(self, node, line_no, symbol_table, name):
+    def __init__(self, node, line_no, symbol_table, name) -> None:
         super().__init__(node, line_no, symbol_table)
         self.func_name = name
         self.has_decremented = False
 
     def get_type(self):
         return GlobalStatementType.FUNCTION
 
-    def get_function_name(self):
+    def get_function_name(self) -> str:
         return self.func_name
 
-    def decrement_line_number(self):
+    def decrement_line_number(self) -> None:
         if self.has_decremented:
             return
-        
-        
+
         old_lineno = self.line_no
-        self.line_no = [old_lineno[0]+1, old_lineno[1]]
+        self.line_no = [old_lineno[0] + 1, old_lineno[1]]
         self.has_decremented = True
 
 
 class ClassDefinitionStatement(GlobalStatement):
-
     def __init__(self, node, line_no, symbol_table, name):
         super().__init__(node, line_no, symbol_table)
         self.class_name = name
 
     def get_type(self):
         return GlobalStatementType.CLASS_DEF
 
-    def get_class_name(self):
+    def get_class_name(self) -> str:
         return self.class_name
-    
-
 
 
-class file_information():
+class file_information:
     """
-        This class represents a file that needs to have functions parsed out of it. 
+    This class represents a file that needs to have functions parsed out of it.
     """
 
     # init method or constructor
-    def __init__(self, location):
+    def __init__(self, location) -> None:
         if not os.path.isfile(location):
             raise FileNotFoundError(
-                f"parser_utils: could not find file at -> {location}")
-        
+                f"parser_utils: could not find file at -> {location}"
+            )
+
         # Path to the file
         self.file_location = location
 
         # Source code
         self.src_code = []
 
         # dict<str, global_statement>: imported symbol name to global statement
@@ -193,15 +195,14 @@
 
         # List of parsed function objects
         self.parsed_functions: List[parsed_function] = []
 
         # dict<str, global_statement>: function name to its global statement
         self.global_functions = {}
 
-        
         # dict<statement, list(str)>: function from statement to symbols
         self.statement_to_symbol = {}
 
         # dict<str, list(statement)>: dictionary from string name of symbol to global statement
         self.symbol_to_statement = {}
 
         # list[global_statements]
@@ -212,83 +213,81 @@
 
         # dict<str, globalobj>: dict from label for manual override to the line number of the comment
         self.include_overrides_glob = {}
 
         # symbol table for the file
         self.symbol_table = None
 
-        
         # abstract syntax tree for the file
         self.ast = ""
 
-        with open(location, 'r') as fh:
+        with open(location, "r") as fh:
             self.src_code = fh.readlines()
             fh.seek(0)
 
             for toktype, tok, start, end, line in tokenize.generate_tokens(fh.readline):
                 # we can also use token.tok_name[toktype] instead of 'COMMENT'
-                # from the token module 
+                # from the token module
                 if toktype == tokenize.COMMENT:
                     self._evaluate_comment(line, start)
 
         try:
-            self.symbol_table = symtable.symtable("".join(self.src_code),
-                                                  location, 'exec')
+            self.symbol_table = symtable.symtable(
+                "".join(self.src_code), location, "exec"
+            )
         except SyntaxError as e:
             print(e)
 
         try:
             self.ast = ast.parse("".join(self.src_code))
         except Exception as e:
             print(e)
 
     def _evaluate_comment(self, line, start):
-        #print(f"COMMENT {start} {line}")
+        # print(f"COMMENT {start} {line}")
 
         match_obj = re.match(INCLUDE_REGEX, line)
 
         if match_obj:
             if len(match_obj.groups()) == 1:
                 self.include_overrides_lineno[match_obj.groups()[0]] = start[0]
 
-
-    def get_source_code(self):
+    def get_source_code(self) -> str:
         return "".join(self.src_code)
 
-    def get_lines_of_source_code(self, start_line, end_line):
-        return "".join(self.src_code[(start_line - 1):(end_line)])
+    def get_lines_of_source_code(self, start_line, end_line) -> str:
+        return "".join(self.src_code[(start_line - 1) : (end_line)])
 
     def get_symbol_table(self):
         return self.symbol_table
 
     def get_ast(self):
         return self.ast
 
-    def add_global_statement(self, global_statement):
+    def add_global_statement(self, global_statement) -> None:
         self.top_level_statements.append(global_statement)
         self.statement_to_symbol[global_statement] = set()
 
     def get_global_statements(self) -> List[GlobalStatement]:
         return self.top_level_statements
 
-    def get_file_length(self):
+    def get_file_length(self) -> int:
         return len(self.src_code)
 
-    def add_global_function(self, name, global_obj):
+    def add_global_function(self, name, global_obj) -> None:
         self.global_functions[name] = global_obj
         self.add_global_statement(global_obj)
 
-    def add_global_import(self, global_obj):
-        self.imported_symbol_to_global_statement[
-            global_obj.as_symbol] = global_obj
-            
+    def add_global_import(self, global_obj) -> None:
+        self.imported_symbol_to_global_statement[global_obj.as_symbol] = global_obj
+
         self.add_global_statement(global_obj)
 
-    def add_class_definition(self, name, global_obj):
+    def add_class_definition(self, name, global_obj) -> None:
         self.global_functions[name] = global_obj
         self.add_global_statement(global_obj)
 
-    def add_parsed_functions(self, func):
+    def add_parsed_functions(self, func) -> None:
         self.parsed_functions.append(func)
 
-    def set_imported_symbols(self, symbols):
+    def set_imported_symbols(self, symbols) -> None:
         self.imported_symbols = symbols
```

### Comparing `cdev-0.0.8/serverless_parser/parser_utils.py` & `cdev-0.0.9/serverless_parser/parser_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,106 +3,126 @@
 from sys import modules, version_info
 
 from typing import Dict, List, Set, Tuple, Union
 from pydantic.types import FilePath
 
 
 from .parser_objects import *
-from .parser_exceptions import InvalidParamError, CouldNotParseFileError, CdevFileNotFoundError, InvalidDataError
+from .parser_exceptions import (
+    InvalidParamError,
+    CouldNotParseFileError,
+    CdevFileNotFoundError,
+    InvalidDataError,
+)
 
 EXCLUDED_SYMBOLS = set(["print"])
 
 line_type = Union[ast.stmt, ast.expr]
 
-def parse_line_numbers(objs: List[line_type], final_line: int) -> List[Tuple[ line_type, Tuple[int,int] ] ]:
+
+def parse_line_numbers(
+    objs: List[line_type], final_line: int
+) -> List[Tuple[line_type, Tuple[int, int]]]:
     rv = []
     previous_info = None
     for node in objs:
-        #_tmp_global_information[node] = [node.lineno, node.end_lineno]
+        # _tmp_global_information[node] = [node.lineno, node.end_lineno]
         if previous_info:
             previous_name, previous_start_line = previous_info
-            line_nos = (previous_start_line, node.lineno-1)
-            rv.append( (previous_name , line_nos) )
+            line_nos = (previous_start_line, node.lineno - 1)
+            rv.append((previous_name, line_nos))
 
         previous_info = (node, node.lineno)
 
     # Set the last line of the last global statement to the last line of the file
     previous_name, previous_start_line = previous_info
     line_nos = (previous_start_line, final_line)
-    rv.append( (previous_name , line_nos) )
+    rv.append((previous_name, line_nos))
 
     return rv
 
 
-def find_ending_line(file_info_obj: file_information, start_line: int, end_line: int, line_start_match: str, ):
-    for i in range(start_line+1, end_line):
+def find_ending_line(
+    file_info_obj: file_information,
+    start_line: int,
+    end_line: int,
+    line_start_match: str,
+) -> int:
+    for i in range(start_line + 1, end_line):
         tmp = file_info_obj.get_lines_of_source_code(i, i)
-        
+
         if tmp.startswith(line_start_match):
             return i
 
     raise Exception("Should not end loop without returning")
 
 
-def _get_global_variables_in_symboltable(table):
+def _get_global_variables_in_symboltable(table) -> Set:
     if not isinstance(table, symtable.SymbolTable):
-        raise InvalidParamError(f"Invalid Param in _get_functions_in_symboltable: Expected symtable.SymbolTable got {type(table)}")
+        raise InvalidParamError(
+            f"Invalid Param in _get_functions_in_symboltable: Expected symtable.SymbolTable got {type(table)}"
+        )
 
     symbols = table.get_symbols()
 
     rv_variables = set()
 
     for sym in symbols:
         # Check all symbols to see if they are not a namespace. Check if the symbol is a global.
         if not sym.is_namespace():
             if sym.is_global():
                 rv_variables.add(sym.get_name())
 
     return rv_variables
 
 
-def _get_imported_variables_in_symboltable(table):
+def _get_imported_variables_in_symboltable(table) -> Set:
     # TODO Change error that is raised
     if not isinstance(table, symtable.SymbolTable):
-        raise InvalidParamError(f"Invalid Param in _get_functions_in_symboltable: Expected symtable.SymbolTable got {type(table)}")
+        raise InvalidParamError(
+            f"Invalid Param in _get_functions_in_symboltable: Expected symtable.SymbolTable got {type(table)}"
+        )
 
     symbols = table.get_symbols()
 
     rv_variables = set()
 
     for sym in symbols:
         # Check all symbols to see if they are not a namespace. If not then they are a normal symbols for this symboltable.
         if not sym.is_namespace():
             if sym.is_imported():
                 rv_variables.add(sym.get_name())
 
     return rv_variables
 
 
-def _get_local_variables_in_symboltable(table):
+def _get_local_variables_in_symboltable(table) -> Set:
     if not isinstance(table, symtable.SymbolTable):
-        raise InvalidParamError(f"Invalid Param in _get_functions_in_symboltable: Expected symtable.SymbolTable got {type(table)}")
+        raise InvalidParamError(
+            f"Invalid Param in _get_functions_in_symboltable: Expected symtable.SymbolTable got {type(table)}"
+        )
 
     symbols = table.get_symbols()
 
     rv_variables = set()
 
     for sym in symbols:
         # Check all symbols to see if they are not a namespace. If not then they are a normal gloabl variable for this symboltable.
         if not sym.is_namespace():
-            if not sym.is_imported() and not sym.is_free(
-            ) and not sym.is_global():
+            if not sym.is_imported() and not sym.is_free() and not sym.is_global():
                 rv_variables.add(sym.get_name())
 
     return rv_variables
 
 
-def _get_functions_in_symboltable(table):
+def _get_functions_in_symboltable(table) -> Set:
     if not isinstance(table, symtable.SymbolTable):
-        raise InvalidParamError(f"Invalid Param in _get_functions_in_symboltable: Expected symtable.SymbolTable got {type(table)}")
+        raise InvalidParamError(
+            f"Invalid Param in _get_functions_in_symboltable: Expected symtable.SymbolTable got {type(table)}"
+        )
 
     symbols = table.get_symbols()
 
     rv_functions = set()
 
     for sym in symbols:
         # Check all symbols to see if they are a namespace (only functions and classes are namespaces)
@@ -112,17 +132,19 @@
                 if isinstance(ns, symtable.Function):
                     rv_functions.add(sym.get_name())
                     continue
 
     return rv_functions
 
 
-def _get_global_class_definitions_in_symboltable(table):
+def _get_global_class_definitions_in_symboltable(table) -> Set:
     if not isinstance(table, symtable.SymbolTable):
-        raise InvalidParamError(f"Invalid Param in _get_functions_in_symboltable: Expected symtable.SymbolTable got {type(table)}")
+        raise InvalidParamError(
+            f"Invalid Param in _get_functions_in_symboltable: Expected symtable.SymbolTable got {type(table)}"
+        )
 
     symbols = table.get_symbols()
 
     rv_class_defs = set()
 
     for sym in symbols:
         # Check all symbols to see if they are a namespace (only functions and classes are namespaces)
@@ -132,168 +154,202 @@
                 if isinstance(ns, symtable.Class):
                     rv_class_defs.add(sym.get_name())
                     continue
 
     return rv_class_defs
 
 
-def _generate_global_statement(file_info_obj: file_information, ast_node: ast.NodeVisitor, line_info: List[str], remove_annotation_functions: Set[str] = set()):
+def _generate_global_statement(
+    file_info_obj: file_information,
+    ast_node: ast.NodeVisitor,
+    line_info: List[str],
+    remove_annotation_functions: Set[str] = set(),
+) -> None:
     # This function is used to determine the type of global statement the node is and create the corresponding global statement obj
 
     last_line = line_info[1]
 
     manual_include = False
     manual_include_sym = ""
 
     # Need to adjust the starting line if using python3.8 or greater
     start_line = line_info[0]
 
-    if (isinstance(ast_node, ast.FunctionDef) and ast_node.decorator_list):
-        # Since python < 3.8 does not include the end_line info on an ast.node, we need to handle removing the top annotation differently 
-        if version_info < (3,8):
+    if isinstance(ast_node, ast.FunctionDef) and ast_node.decorator_list:
+        # Since python < 3.8 does not include the end_line info on an ast.node, we need to handle removing the top annotation differently
+        if version_info < (3, 8):
             if not ast_node.name in remove_annotation_functions:
                 start_line = ast_node.decorator_list[0].lineno
 
             else:
                 # Since we have no way of know when the first decorator ends because there is not end_lineno property,
                 # we have to check each line below it to see if it is either the function declaration ('def ') or
                 # the next annotation definition ('@')
                 match_line = "def " if len(ast_node.decorator_list) == 1 else "@"
 
                 # search for the next definition based on the match_line and search at longest til you get to the first line of the body of the function
-                start_line = find_ending_line(file_info_obj, ast_node.decorator_list[0].lineno, ast_node.body[0].lineno, match_line)
+                start_line = find_ending_line(
+                    file_info_obj,
+                    ast_node.decorator_list[0].lineno,
+                    ast_node.body[0].lineno,
+                    match_line,
+                )
         else:
             # for python>=3.8
-            start_line = ast_node.decorator_list[0].end_lineno + 1 if ast_node.name in remove_annotation_functions else ast_node.decorator_list[0].lineno
+            start_line = (
+                ast_node.decorator_list[0].end_lineno + 1
+                if ast_node.name in remove_annotation_functions
+                else ast_node.decorator_list[0].lineno
+            )
 
     # Look one line above the start for a manual include
     for k in file_info_obj.include_overrides_lineno:
-        if file_info_obj.include_overrides_lineno.get(k) == start_line-1:
+        if file_info_obj.include_overrides_lineno.get(k) == start_line - 1:
             manual_include = True
             manual_include_sym = k
             break
 
-    tmp_src_code = file_info_obj.get_lines_of_source_code(
-        start_line, last_line)
-
-    tmp_symbol_table = symtable.symtable(tmp_src_code,
-                                         file_info_obj.file_location, 'exec')
+    tmp_src_code = file_info_obj.get_lines_of_source_code(start_line, last_line)
 
+    tmp_symbol_table = symtable.symtable(
+        tmp_src_code, file_info_obj.file_location, "exec"
+    )
 
     need_to_check_function = False
     need_to_check_class_def = False
 
     for sym in tmp_symbol_table.get_symbols():
         if sym.is_namespace():
             if isinstance(sym.get_namespaces()[0], symtable.Function):
                 need_to_check_function = True
             elif isinstance(sym.get_namespaces()[0], symtable.Class):
                 need_to_check_class_def = True
-        
 
     if need_to_check_function:
         single_symbol = tmp_symbol_table.get_symbols()[0]
-        
+
         if single_symbol.is_namespace():
-            if isinstance(single_symbol.get_namespaces()[0],
-                          symtable.Function):
-                    
+            if isinstance(single_symbol.get_namespaces()[0], symtable.Function):
+
                 name = single_symbol.get_name()
-                
-                function_symbols = set([x.get_name() for x in single_symbol.get_namespaces()[0].get_symbols()])
 
-                function_symbols.update(set([x.get_name() for x in tmp_symbol_table.get_symbols()]))
-               
-                fs = FunctionStatement(ast_node, [start_line, last_line],
-                                       list(function_symbols), name)
+                function_symbols = set(
+                    [
+                        x.get_name()
+                        for x in single_symbol.get_namespaces()[0].get_symbols()
+                    ]
+                )
+
+                function_symbols.update(
+                    set([x.get_name() for x in tmp_symbol_table.get_symbols()])
+                )
+
+                fs = FunctionStatement(
+                    ast_node, [start_line, last_line], list(function_symbols), name
+                )
                 file_info_obj.add_global_function(name, fs)
 
                 if manual_include:
                     file_info_obj.include_overrides_glob[manual_include_sym] = fs
 
                 return
 
     if need_to_check_class_def:
 
         class_def_table = tmp_symbol_table.get_children()[0]
 
-        class_def = ClassDefinitionStatement(ast_node, [start_line, last_line], [x.get_name() for x in class_def_table.get_symbols()] , class_def_table.get_name())
+        class_def = ClassDefinitionStatement(
+            ast_node,
+            [start_line, last_line],
+            [x.get_name() for x in class_def_table.get_symbols()],
+            class_def_table.get_name(),
+        )
         file_info_obj.add_class_definition(class_def_table.get_name(), class_def)
-        return 
+        return
 
     ts = {s.get_name() for s in tmp_symbol_table.get_symbols()}
 
     used_imported_symbols = file_info_obj.imported_symbols.intersection(ts)
     if len(used_imported_symbols) > 0:
         # This statement uses an imported symbol so we need to check it to see if it is the import statement
         for n in ast.walk(ast_node):
-            #print(n)
+            # print(n)
             if isinstance(n, ast.Import):
-                #print(f"IMPORT: {n}")
-                #print(f"FIELDS { [(cn.name, cn.asname)  for cn in n.names] }")
+                # print(f"IMPORT: {n}")
+                # print(f"FIELDS { [(cn.name, cn.asname)  for cn in n.names] }")
                 for imprt in n.names:
-                    #print(f"FIELDS: {imprt.name}; {imprt.asname}")
+                    # print(f"FIELDS: {imprt.name}; {imprt.asname}")
                     if not imprt.asname:
                         asname = imprt.name
                     else:
                         asname = imprt.asname
 
-                    imp_statement = ImportStatement(ast_node,
-                                                    [start_line, last_line],
-                                                    [x.get_name() for x in tmp_symbol_table.get_symbols()], asname,
-                                                    imprt.name)
+                    imp_statement = ImportStatement(
+                        ast_node,
+                        [start_line, last_line],
+                        [x.get_name() for x in tmp_symbol_table.get_symbols()],
+                        asname,
+                        imprt.name,
+                    )
 
-                    #print(f"{ast.dump(n)} -> {asname}?{imprt.name}")
+                    # print(f"{ast.dump(n)} -> {asname}?{imprt.name}")
                     file_info_obj.add_global_import(imp_statement)
                     continue
 
             if isinstance(n, ast.ImportFrom):
                 for imprt in n.names:
                     if not imprt.asname:
                         asname = imprt.name
                     else:
                         asname = imprt.asname
-                    
 
                     if n.level > 0:
                         if not n.module:
                             asmodule = f"{'.' * n.level}{asname}"
                         else:
                             asmodule = f"{'.' * n.level}{n.module}"
-                            
 
                     else:
-                        asmodule =  n.module
+                        asmodule = n.module
 
-                    #print(f"{ast.dump(n)} -> {asname}?{asmodule}")
-                    imp_statement = ImportStatement(ast_node,
-                                                    [start_line, last_line],
-                                                    [x.get_name() for x in tmp_symbol_table.get_symbols()], asname,
-                                                    asmodule)
+                    # print(f"{ast.dump(n)} -> {asname}?{asmodule}")
+                    imp_statement = ImportStatement(
+                        ast_node,
+                        [start_line, last_line],
+                        [x.get_name() for x in tmp_symbol_table.get_symbols()],
+                        asname,
+                        asmodule,
+                    )
 
                     file_info_obj.add_global_import(imp_statement)
                 continue
 
-    global_statement_obj = GlobalStatement(ast_node, [start_line, last_line],
-                                           [x.get_name() for x in tmp_symbol_table.get_symbols()])
-
+    global_statement_obj = GlobalStatement(
+        ast_node,
+        [start_line, last_line],
+        [x.get_name() for x in tmp_symbol_table.get_symbols()],
+    )
 
-    
     file_info_obj.add_global_statement(global_statement_obj)
 
     if manual_include:
         file_info_obj.include_overrides_glob[manual_include_sym] = global_statement_obj
 
 
-
-def get_file_information(file_path: str, include_functions: List[str] =[], function_manual_includes: Dict[str, str]={}, global_manual_includes: List[str]=[], remove_top_annotation: bool =False):
+def get_file_information(
+    file_path: str,
+    include_functions: List[str] = [],
+    function_manual_includes: Dict[str, str] = {},
+    global_manual_includes: List[str] = [],
+    remove_top_annotation: bool = False,
+) -> file_information:
     if not os.path.isfile(file_path):
-        raise CouldNotParseFileError(CdevFileNotFoundError(
-            f"cdev_parser: could not find file at -> {file_path}"))
-
+        raise CouldNotParseFileError(
+            CdevFileNotFoundError(f"cdev_parser: could not find file at -> {file_path}")
+        )
 
     file_info_obj = file_information(file_path)
 
     symbol_table = file_info_obj.get_symbol_table()
 
     # Need to get some basic information about the global namespace in the file. This includes:
     # - all defined functions (_get_functions_in_symboltable)
@@ -313,56 +369,63 @@
         global_symbols = _get_global_variables_in_symboltable(symbol_table)
 
         class_definitions = _get_global_class_definitions_in_symboltable(symbol_table)
     except InvalidParamError as e:
         raise CouldNotParseFileError(e)
         return
 
-    for item in functions.union(local_variables).union(imported_symbols).union(
-            global_symbols).union(class_definitions):
+    for item in (
+        functions.union(local_variables)
+        .union(imported_symbols)
+        .union(global_symbols)
+        .union(class_definitions)
+    ):
         file_info_obj.symbol_to_statement[item] = set()
 
     file_info_obj.set_imported_symbols(imported_symbols)
 
     # Need to get the line range of each global statement, but this requires looping over all the global nodes in the ast
-    # in the top level of the file. 
-    # 
+    # in the top level of the file.
+    #
     # Python3.8 introduced node.end_lineno to ast nodes, which makes it easier to get the ending line info
-    # 
+    #
     # To support earlier versions of python (<3.8) we must use the starting line of
     # the next statement as the last line of previous node. We are going to store this info in a tmp dict then
     # once we have all the information create the objects
 
     file_ast = file_info_obj.get_ast()
 
     # dict<ast.node, [line1,line2]>
     _tmp_global_information = {}
 
     # sys.version_info
-    if version_info < (3,8):
-        _tmp_global_information = dict(parse_line_numbers(file_ast.body, file_info_obj.get_file_length() + 1 ))
+    if version_info < (3, 8):
+        _tmp_global_information = dict(
+            parse_line_numbers(file_ast.body, file_info_obj.get_file_length() + 1)
+        )
     else:
         for node in file_ast.body:
             _tmp_global_information[node] = [node.lineno, node.end_lineno]
 
-
-
-    remove_function_annotations = set(include_functions) if remove_top_annotation else set()
+    remove_function_annotations = (
+        set(include_functions) if remove_top_annotation else set()
+    )
     # Now that the information has been collected for the global statements, we can create the actual objs and add
     # them to the file_info_obj
     for node, line_info in _tmp_global_information.items():
-        _generate_global_statement(file_info_obj, node, line_info, remove_function_annotations)
-
+        _generate_global_statement(
+            file_info_obj, node, line_info, remove_function_annotations
+        )
 
     # Build a two-way binding of a symbol to statement and a statement to a symbol.
     # This information is needed to get all dependencies of symbols, which is needed
     # to reconstruct just the necessary lines
     for i in file_info_obj.get_global_statements():
         syms = i.get_symbols()
-        
+
         for sym in syms:
             if not sym in file_info_obj.symbol_to_statement:
                 continue
 
             # Some symbols do no create a dependency so they should not be added
             if sym in EXCLUDED_SYMBOLS:
                 continue
@@ -379,33 +442,30 @@
             if i.get_type() == GlobalStatementType.FUNCTION:
                 continue
 
             tmp = file_info_obj.symbol_to_statement.get(sym)
             tmp.add(i)
             file_info_obj.symbol_to_statement[sym] = tmp
 
-
         # if this global object is a function then we need to add the global object to its own symbol name dependency list. That way
-        # if another global statement calls this function we include this global statement (which is the definition of the function) 
+        # if another global statement calls this function we include this global statement (which is the definition of the function)
         if i.get_type() == GlobalStatementType.FUNCTION:
             tmp = file_info_obj.symbol_to_statement.get(i.get_function_name())
             tmp.add(i)
             file_info_obj.symbol_to_statement[i.get_function_name()] = tmp
 
         if i.get_type() == GlobalStatementType.CLASS_DEF:
             tmp = file_info_obj.symbol_to_statement.get(i.get_class_name())
             tmp.add(i)
             file_info_obj.symbol_to_statement[i.get_class_name()] = tmp
 
-
     # If a list of functions was not included then parse all top level functions
     if not include_functions:
         include_functions = file_info_obj.global_functions.keys()
 
-
     # manual includes is a dictionary from function name to global statement
     for function_name in include_functions:
         # Create new parsed function obj
         p_function = parsed_function(function_name)
 
         # Start with a set that already includes the symbol for itself
         already_included_symbols = set([function_name])
@@ -415,55 +475,57 @@
         needed_global_objects = set([file_info_obj.global_functions.get(function_name)])
 
         # if the function has any manual statement includes
         # function_manual_includes is the dict from function name to the name of the manual include
         if function_name in function_manual_includes:
             for include in function_manual_includes.get(function_name):
                 if not include in file_info_obj.include_overrides_glob:
-                    raise InvalidDataError(f"""function_manual_includes param data issue: Trying to manually include '{include}' for function '{function_name} but '{include}' is not present in file""")
-                    
+                    raise InvalidDataError(
+                        f"""function_manual_includes param data issue: Trying to manually include '{include}' for function '{function_name} but '{include}' is not present in file"""
+                    )
+
+                needed_global_objects.add(
+                    file_info_obj.include_overrides_glob.get(include)
+                )
 
-                needed_global_objects.add(file_info_obj.include_overrides_glob.get(include))
-        
         # global_manual_includes is a list of the names of manual includes that need to be added to every function
         for include in global_manual_includes:
             if not include in file_info_obj.include_overrides_glob:
-                raise InvalidDataError(f"""function_manual_includes param data issue: Trying to manually include '{include}' as a global manual include but '{include}' is not present in file""")
+                raise InvalidDataError(
+                    f"""function_manual_includes param data issue: Trying to manually include '{include}' as a global manual include but '{include}' is not present in file"""
+                )
 
             needed_global_objects.add(file_info_obj.include_overrides_glob.get(include))
 
-        
         next_symbols = set()
         already_included_global_obj = set()
 
-        
         for global_object in needed_global_objects:
             # Add the functions lines to the parsed function
             p_function.add_line_numbers(global_object.get_line_no())
 
             # Start with a set that already includes the global statement for itself
             already_included_global_obj.add(global_object)
 
             # next symbols is the set of symbols that need their dependant global statements
-            next_symbols = next_symbols.union(file_info_obj.statement_to_symbol.get(global_object))
+            next_symbols = next_symbols.union(
+                file_info_obj.statement_to_symbol.get(global_object)
+            )
 
             # Some symbols won't be included in the mapping because they are excluded, but they need to be kept track of to look at imports
             all_used_symbols = set(global_object.get_symbols())
 
         keep_looping = True
         remaining_symbols = set()
 
         while keep_looping:
             # If there are no more symbols than break the loop
-            
-
 
             # Add the previous iterations symbols as already seen so they are not readded
-            already_included_symbols = already_included_symbols.union(
-                remaining_symbols)
+            already_included_symbols = already_included_symbols.union(remaining_symbols)
             remaining_symbols = next_symbols
 
             if not next_symbols:
                 break
 
             next_symbols = set()
 
@@ -471,92 +533,101 @@
                 if sym in already_included_symbols:
                     # If we have already added this symbol than we have all of its dependencies
                     continue
 
                 # Add all dependant global statements to this symbol needs to the need lines for the function
                 for glob_obj in file_info_obj.symbol_to_statement.get(sym):
                     if glob_obj in already_included_global_obj:
-                        #IF this global statement has already been added continue
+                        # IF this global statement has already been added continue
                         continue
 
                     # Add the lines numbers and place it in the already included set
                     p_function.add_line_numbers(glob_obj.get_line_no())
                     already_included_global_obj.add(glob_obj)
 
                     # include this statements
-                    all_used_symbols = all_used_symbols.union(set(glob_obj.get_symbols()) )
+                    all_used_symbols = all_used_symbols.union(
+                        set(glob_obj.get_symbols())
+                    )
 
                     # Get the set of symbols that this statement depends on
-                    set_symbols = file_info_obj.statement_to_symbol.get(
-                        glob_obj)
+                    set_symbols = file_info_obj.statement_to_symbol.get(glob_obj)
                     # Remove the symbols that have already been included
                     new_needed_symbols = set_symbols.difference(
-                        already_included_symbols)
+                        already_included_symbols
+                    )
                     actual_new_needed_symbols = new_needed_symbols.difference(
-                        remaining_symbols)
+                        remaining_symbols
+                    )
 
                     # Add the actually needed new symbols to the set of symbols to be looped over next
-                    next_symbols = next_symbols.union(
-                        actual_new_needed_symbols)
+                    next_symbols = next_symbols.union(actual_new_needed_symbols)
 
-        #print(f"all pkg in file -> {file_info_obj.imported_symbol_to_global_statement}")
+        # print(f"all pkg in file -> {file_info_obj.imported_symbol_to_global_statement}")
         for symbol in all_used_symbols:
-            if symbol in file_info_obj.imported_symbol_to_global_statement and not symbol in EXCLUDED_SYMBOLS:
+            if (
+                symbol in file_info_obj.imported_symbol_to_global_statement
+                and not symbol in EXCLUDED_SYMBOLS
+            ):
                 p_function.add_import(
                     file_info_obj.imported_symbol_to_global_statement.get(symbol)
                 )
 
-        
-        
-        #finally add the parsed function object to the file info
+        # finally add the parsed function object to the file info
         file_info_obj.add_parsed_functions(p_function)
 
     return file_info_obj
 
 
 _individual_file_cache = {}
-def _get_individual_files_imported_symbols(file_location):
+
+
+def _get_individual_files_imported_symbols(file_location) -> Set:
     if file_location in _individual_file_cache:
         return _individual_file_cache.get(file_location)
 
     rv = set()
-    
-    with open(file_location, 'r') as fh:
+
+    with open(file_location, "r") as fh:
         src_code = fh.readlines()
         fh.seek(0)
 
     ast_rep = ast.parse("".join(src_code))
 
-    
-
     for node in ast.walk(ast_rep):
-        
+
         if isinstance(node, ast.Import):
             for pkg_name in node.names:
-                
-                asname = pkg_name.name.split('.')[0] if not pkg_name.name.startswith('.') else pkg_name.name
-                    
-                rv.add((asname, None))
-    
+
+                asname = (
+                    pkg_name.name.split(".")[0]
+                    if not pkg_name.name.startswith(".")
+                    else pkg_name.name
+                )
+
+                rv.add(asname)
+
         elif isinstance(node, ast.ImportFrom):
-            # if the import has levels > 0 and no module it is a local referenced package and will already be included
-            # if not then it is a package on the PYTHONPATH and we need to add it as a dependency
-            
-            asname = node.module.split('.')[0] if not node.module.startswith('.') else node.module
-                    
-            rv.add((asname, None))
-    
+            # IF the import has a named module then it can either be a relative or absolute import
+            # If the import does not have a named module, it must be a relative import
 
-    _individual_file_cache[file_location] = rv
-                
-    return rv
+            if node.module:
+                asname = (
+                    node.module.split(".")[0]
+                    if node.level == 0
+                    else f"{node.level * '.'}{node.module}"
+                )
+                rv.add(asname)
 
+            else:
+                [rv.add(f"{node.level * '.'}{x.name}") for x in node.names]
 
+    _individual_file_cache[file_location] = rv
+
+    return rv
 
 
-def get_file_imported_symbols(file_loc: FilePath):
+def get_file_imported_symbols(file_loc: FilePath) -> Set:
     # Walk the whole dir/children importing all python files and then searching their symbol tree to find import statements
     rv = _get_individual_files_imported_symbols(file_loc)
 
     return rv
-
-
```

