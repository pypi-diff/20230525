# Comparing `tmp/seeFretboard-0.0.9.4.tar.gz` & `tmp/seeFretboard-0.0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seeFretboard-0.0.9.4.tar", last modified: Thu May 25 04:10:34 2023, max compression
+gzip compressed data, was "seeFretboard-0.0.9.5.tar", last modified: Thu May 25 04:34:59 2023, max compression
```

## Comparing `seeFretboard-0.0.9.4.tar` & `seeFretboard-0.0.9.5.tar`

### file list

```diff
@@ -1,868 +1,868 @@
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.940025 seeFretboard-0.0.9.4/
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.698562 seeFretboard-0.0.9.4/.venv/
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.698616 seeFretboard-0.0.9.4/.venv/lib/
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.698665 seeFretboard-0.0.9.4/.venv/lib/python3.11/
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.703865 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.708093 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/_distutils_hack/
--rw-r--r--   0 lindazhang   (501) staff       (20)     6128 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/_distutils_hack/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)       44 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/_distutils_hack/override.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.710412 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/
--rw-r--r--   0 lindazhang   (501) staff       (20)      355 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1198 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/__main__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1444 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/__pip-runner__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.712374 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/
--rw-r--r--   0 lindazhang   (501) staff       (20)      573 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10192 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/build_env.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10734 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cache.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.714610 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/
--rw-r--r--   0 lindazhang   (501) staff       (20)      132 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6676 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7842 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    29250 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      774 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2472 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4338 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10817 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1968 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18172 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5118 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      116 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/status_codes.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.721047 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/
--rw-r--r--   0 lindazhang   (501) staff       (20)     3882 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7582 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1685 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4129 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9815 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6591 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5289 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2951 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1703 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1132 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4762 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3188 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    32234 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    12343 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5697 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6419 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3755 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7396 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13529 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/configuration.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.722133 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/distributions/
--rw-r--r--   0 lindazhang   (501) staff       (20)      858 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1221 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      729 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6494 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1164 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    24091 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/exceptions.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.723174 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/index/
--rw-r--r--   0 lindazhang   (501) staff       (20)       30 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    16504 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    37873 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6557 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/index/sources.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.724243 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/locations/
--rw-r--r--   0 lindazhang   (501) staff       (20)    17794 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6319 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8149 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2556 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      340 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/main.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.727389 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/metadata/
--rw-r--r--   0 lindazhang   (501) staff       (20)     4280 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2595 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    25277 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/metadata/base.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.728251 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/
--rw-r--r--   0 lindazhang   (501) staff       (20)      107 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1882 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8181 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7457 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9773 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.731662 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/
--rw-r--r--   0 lindazhang   (501) staff       (20)       63 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      990 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6442 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2520 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1030 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/index.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2617 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18602 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/link.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      738 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4644 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1907 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3858 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3600 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/wheel.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.734074 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/network/
--rw-r--r--   0 lindazhang   (501) staff       (20)       50 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    16507 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2145 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6096 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/network/download.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7638 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18443 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/network/session.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4073 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1791 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.734677 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.736468 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4133 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1422 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1474 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2198 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1075 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1417 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3064 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5122 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9784 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/freeze.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.738160 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/
--rw-r--r--   0 lindazhang   (501) staff       (20)       51 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1354 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4105 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/legacy.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    27407 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    25091 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6987 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/pyproject.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.740132 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/req/
--rw-r--r--   0 lindazhang   (501) staff       (20)     2807 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    16611 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    17646 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    35763 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2858 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    24045 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.740747 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      583 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/base.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.741643 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    24129 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.744243 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5220 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18963 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    27878 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5705 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9914 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2526 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5455 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11533 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8167 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.752793 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1015 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1665 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1884 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5377 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      242 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5764 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3206 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1115 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/distutils_args.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2118 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1169 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3064 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5122 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      716 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3110 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4831 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      795 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11632 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    22253 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1193 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2108 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5662 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9200 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7702 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8821 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1759 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3456 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4549 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/wheel.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.753947 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/vcs/
--rw-r--r--   0 lindazhang   (501) staff       (20)      596 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3519 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18116 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5238 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11729 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    22811 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13079 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/wheel_builder.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.754687 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/
--rw-r--r--   0 lindazhang   (501) staff       (20)     4966 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.756646 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/
--rw-r--r--   0 lindazhang   (501) staff       (20)      465 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1379 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5033 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1535 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.757144 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/
--rw-r--r--   0 lindazhang   (501) staff       (20)      242 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5271 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1033 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      778 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    16416 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3946 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4154 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7105 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      774 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.757701 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/
--rw-r--r--   0 lindazhang   (501) staff       (20)       94 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      255 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4279 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/core.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.777748 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/
--rw-r--r--   0 lindazhang   (501) staff       (20)     4797 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    31274 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1763 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10032 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3915 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5420 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.778126 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3242 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3732 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      542 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1860 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1683 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4006 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    12176 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3934 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13566 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1753 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    36913 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1753 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    20735 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1759 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14537 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    25796 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    42498 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1752 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    27055 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   104562 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    98484 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    98196 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   101363 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   128035 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   102774 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    95372 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5380 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6077 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3715 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2131 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    30391 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.778520 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13560 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      402 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/resultdict.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6400 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4137 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4007 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14848 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8505 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2812 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      244 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/version.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.779668 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/
--rw-r--r--   0 lindazhang   (501) staff       (20)      266 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2522 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11128 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3325 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.781137 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/
--rw-r--r--   0 lindazhang   (501) staff       (20)       75 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2839 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10678 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6741 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1866 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1079 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3709 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6181 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7134 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.784628 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/
--rw-r--r--   0 lindazhang   (501) staff       (20)      581 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    41259 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    51697 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    20834 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    51991 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14811 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5058 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    39801 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10820 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18102 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    66262 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    23513 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/version.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    43898 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.786060 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distro/
--rw-r--r--   0 lindazhang   (501) staff       (20)      981 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)       64 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    49330 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distro/distro.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.791031 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/idna/
--rw-r--r--   0 lindazhang   (501) staff       (20)      849 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3374 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      321 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    12950 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    44375 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1881 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0 lindazhang   (501) staff       (20)       21 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   206539 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.793809 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/
--rw-r--r--   0 lindazhang   (501) staff       (20)     1132 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1081 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6080 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    34557 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.795881 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/
--rw-r--r--   0 lindazhang   (501) staff       (20)      661 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      497 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11488 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4378 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1431 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8487 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4676 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    30110 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    15699 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4200 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14665 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/version.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.796732 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/
--rw-r--r--   0 lindazhang   (501) staff       (20)   108287 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      562 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/py31compat.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.798468 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/
--rw-r--r--   0 lindazhang   (501) staff       (20)    12936 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1176 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4068 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4910 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2655 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6911 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      160 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6596 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.801697 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/
--rw-r--r--   0 lindazhang   (501) staff       (20)     2999 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      353 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    23685 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1697 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1938 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.801957 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/
--rw-r--r--   0 lindazhang   (501) staff       (20)    40386 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2917 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.804532 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/
--rw-r--r--   0 lindazhang   (501) staff       (20)     4810 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4104 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3314 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5086 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    35441 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    21938 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5871 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    19351 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5073 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2212 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5014 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7335 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4674 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11753 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    32005 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.805195 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/
--rw-r--r--   0 lindazhang   (501) staff       (20)    11174 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    70232 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    53376 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      986 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2591 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3072 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3092 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4630 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6257 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/style.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.805438 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/
--rw-r--r--   0 lindazhang   (501) staff       (20)     3419 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6184 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    63187 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9110 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/util.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.809637 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/
--rw-r--r--   0 lindazhang   (501) staff       (20)     9171 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6426 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    12936 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   213344 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.809811 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/
--rw-r--r--   0 lindazhang   (501) staff       (20)    23685 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9023 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    39129 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    25341 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13402 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10787 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6805 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.810482 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/
--rw-r--r--   0 lindazhang   (501) staff       (20)      491 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      138 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11920 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.810882 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/
--rw-r--r--   0 lindazhang   (501) staff       (20)      546 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10927 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.814286 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/
--rw-r--r--   0 lindazhang   (501) staff       (20)     5178 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      435 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1397 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    21443 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6377 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10187 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      575 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1286 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18560 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3823 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3879 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      733 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    35288 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      695 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    30180 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4235 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2912 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    33240 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/utils.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.815199 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/
--rw-r--r--   0 lindazhang   (501) staff       (20)      537 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.815489 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      156 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5872 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1583 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    17592 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4794 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.835560 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/
--rw-r--r--   0 lindazhang   (501) staff       (20)     6090 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8478 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10096 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   140235 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1064 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2114 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      265 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9695 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3225 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1236 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1643 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7063 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      423 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5472 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    19919 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      351 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      417 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    22820 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1926 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2783 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1840 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      890 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10368 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6819 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3264 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9842 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4503 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18015 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1054 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7131 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    97992 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1288 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5497 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6630 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7954 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      972 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2501 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      642 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1616 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2508 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9585 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5053 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3252 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14007 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14172 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3667 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11903 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8198 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5305 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4970 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      828 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3396 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10574 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    37414 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    59836 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8165 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11303 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1391 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      166 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4436 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4773 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2843 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1591 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    24224 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4374 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4425 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    26332 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1258 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    34995 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    39684 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3370 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    45686 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3627 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      102 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    26070 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9169 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    34549 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/six.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.837700 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/
--rw-r--r--   0 lindazhang   (501) staff       (20)    18364 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3314 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1944 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1496 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1376 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1908 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1383 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7550 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2790 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2145 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8011 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.838558 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/
--rw-r--r--   0 lindazhang   (501) staff       (20)      396 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    22633 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2943 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      254 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    80114 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.841039 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/
--rw-r--r--   0 lindazhang   (501) staff       (20)     3333 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10811 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0 lindazhang   (501) staff       (20)       64 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    20070 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    39095 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.844087 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      957 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.845416 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    17632 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13922 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11036 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4528 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    17081 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    34448 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7097 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8217 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8579 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2440 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.846057 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.846660 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1417 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    34665 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    19786 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5985 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    30641 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.850013 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/
--rw-r--r--   0 lindazhang   (501) staff       (20)     1155 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4901 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1605 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      498 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3997 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3510 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    22003 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    17177 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5758 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6895 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10003 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14298 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5403 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.851429 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/
--rw-r--r--   0 lindazhang   (501) staff       (20)    10579 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8979 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1305 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6563 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4307 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.851614 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/
--rw-r--r--   0 lindazhang   (501) staff       (20)   108568 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.852957 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    24701 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/appdirs.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.854955 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/
--rw-r--r--   0 lindazhang   (501) staff       (20)      506 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4504 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2741 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2706 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      884 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3494 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3886 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3566 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2836 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.855391 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5420 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13515 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.855567 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/
--rw-r--r--   0 lindazhang   (501) staff       (20)    15526 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.856387 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/
--rw-r--r--   0 lindazhang   (501) staff       (20)       83 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   132569 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18410 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.859327 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/
--rw-r--r--   0 lindazhang   (501) staff       (20)      661 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      497 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11488 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4378 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1431 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8496 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4706 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    30110 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    15699 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4200 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14665 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.862821 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/
--rw-r--r--   0 lindazhang   (501) staff       (20)     9159 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6426 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/actions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    12936 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/common.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   213310 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/core.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.863069 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/
--rw-r--r--   0 lindazhang   (501) staff       (20)    23668 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9023 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    39129 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    25341 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/results.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13402 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/testing.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10787 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6805 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/util.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8425 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.863315 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/extern/
--rw-r--r--   0 lindazhang   (501) staff       (20)     2426 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/extern/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.871142 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/
--rw-r--r--   0 lindazhang   (501) staff       (20)     8429 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      218 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_deprecation_warning.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.879862 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/
--rw-r--r--   0 lindazhang   (501) staff       (20)      537 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1330 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/_collections.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      411 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/_functools.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      239 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/_macos_compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    19672 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8603 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14789 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    47369 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    17973 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/cmd.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.885075 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/
--rw-r--r--   0 lindazhang   (501) staff       (20)      430 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1614 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5441 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4701 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    22051 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5617 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7728 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    31558 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    16568 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5624 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4888 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/check.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2603 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13137 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/config.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    30221 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2779 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2785 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1189 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8434 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1936 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      672 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11765 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/register.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    19241 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7477 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4920 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/config.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9451 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/core.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    12537 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      139 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/debug.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3423 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8082 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    50186 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/dist.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3589 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/errors.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10270 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/extension.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    17910 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8226 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/file_util.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13713 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/filelist.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1972 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/log.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    30235 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    23602 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      217 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/py38compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      639 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3517 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/spawn.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18858 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    12096 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/text_file.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    15641 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    18128 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/util.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    12952 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/version.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5248 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1972 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_entry_points.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2392 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_imp.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1311 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_importlib.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      675 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_itertools.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      749 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_path.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      501 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_reqs.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.886014 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.887573 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/
--rw-r--r--   0 lindazhang   (501) staff       (20)    30130 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1862 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      743 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1828 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2895 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2068 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1154 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2166 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.889218 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/
--rw-r--r--   0 lindazhang   (501) staff       (20)      506 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4504 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2741 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2706 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      884 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3494 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3886 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3566 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2836 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.889888 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5420 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13512 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.890128 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/
--rw-r--r--   0 lindazhang   (501) staff       (20)    15517 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.893397 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/
--rw-r--r--   0 lindazhang   (501) staff       (20)       82 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   117959 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    16256 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    15130 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.898989 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/
--rw-r--r--   0 lindazhang   (501) staff       (20)      661 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      497 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11488 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4378 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1431 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8493 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4700 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    30110 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    15699 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4200 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14665 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.902027 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/
--rw-r--r--   0 lindazhang   (501) staff       (20)     9159 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6426 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/actions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    12936 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/common.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   213310 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/core.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.902285 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/
--rw-r--r--   0 lindazhang   (501) staff       (20)    23668 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     9023 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/exceptions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    39129 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/helpers.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    25341 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/results.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13402 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/testing.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    10787 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/unicode.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6805 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/util.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.903112 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/
--rw-r--r--   0 lindazhang   (501) staff       (20)      396 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    22633 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2943 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      254 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_types.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    87149 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8425 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/zipp.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7346 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/archive_util.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    19539 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/build_meta.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.909416 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/
--rw-r--r--   0 lindazhang   (501) staff       (20)      396 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2381 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/alias.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    16623 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/bdist_egg.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1182 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6595 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/build.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4415 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/build_clib.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    15821 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/build_ext.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14115 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/build_py.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7012 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/develop.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4800 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/dist_info.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    85662 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/easy_install.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    31188 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/editable_wheel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    26795 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/egg_info.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5163 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/install.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2226 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/install_egg_info.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3875 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/install_lib.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2612 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/install_scripts.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4946 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/py36compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      468 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/register.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2128 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/rotate.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      658 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/saveopts.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7071 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/sdist.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5086 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/setopt.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8102 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/test.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      462 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/upload.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7494 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/upload_docs.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.913579 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/
--rw-r--r--   0 lindazhang   (501) staff       (20)     1121 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    13398 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.916667 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/
--rw-r--r--   0 lindazhang   (501) staff       (20)     1038 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    11266 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1153 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1612 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-r--r--   0 lindazhang   (501) staff       (20)   269900 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8736 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    16319 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/expand.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    19304 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    25198 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/setupcfg.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      949 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/dep_util.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5499 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/depends.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    20799 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/discovery.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    45578 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/dist.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2464 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/errors.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     5591 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/extension.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.916905 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/extern/
--rw-r--r--   0 lindazhang   (501) staff       (20)     2512 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/extern/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4873 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/glob.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3824 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/installer.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      812 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/launch.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1210 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/logging.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4857 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/monkey.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    47724 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/msvc.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3093 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/namespaces.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    40020 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/package_index.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      245 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/py34compat.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    14348 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/sandbox.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      941 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/unicode_utils.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      144 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/version.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     8376 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/wheel.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      718 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/windows_support.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.917372 seeFretboard-0.0.9.4/Examples/
--rw-r--r--   0 lindazhang   (501) staff       (20)      239 2023-05-25 01:54:18.000000 seeFretboard-0.0.9.4/Examples/horizontalFretboard.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1072 2023-05-24 18:18:02.000000 seeFretboard-0.0.9.4/LICENSE
--rw-r--r--   0 lindazhang   (501) staff       (20)       56 2023-05-25 02:46:38.000000 seeFretboard-0.0.9.4/MANIFEST.in
--rw-r--r--   0 lindazhang   (501) staff       (20)     1372 2023-05-25 04:10:34.939861 seeFretboard-0.0.9.4/PKG-INFO
--rw-r--r--   0 lindazhang   (501) staff       (20)     1005 2023-05-02 18:53:11.000000 seeFretboard-0.0.9.4/README.md
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.918491 seeFretboard-0.0.9.4/Tests/
--rw-r--r--   0 lindazhang   (501) staff       (20)     7163 2023-05-24 07:07:44.000000 seeFretboard-0.0.9.4/Tests/StylesTest.py
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:56:48.000000 seeFretboard-0.0.9.4/Tests/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      287 2023-05-25 01:57:45.000000 seeFretboard-0.0.9.4/pyproject.toml
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.922762 seeFretboard-0.0.9.4/seeFretboard/
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.928391 seeFretboard-0.0.9.4/seeFretboard/Designs/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-24 06:03:38.000000 seeFretboard-0.0.9.4/seeFretboard/Designs/Buttons.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     2163 2023-05-23 16:51:07.000000 seeFretboard-0.0.9.4/seeFretboard/Designs/CirlceNote.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3207 2023-05-24 16:53:11.000000 seeFretboard-0.0.9.4/seeFretboard/Designs/FretboardFigure.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     6610 2023-05-23 21:33:59.000000 seeFretboard-0.0.9.4/seeFretboard/Designs/FretboardStyle.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      139 2023-05-24 19:26:22.000000 seeFretboard-0.0.9.4/seeFretboard/Designs/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.934666 seeFretboard-0.0.9.4/seeFretboard/Examples/
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:55:42.000000 seeFretboard-0.0.9.4/seeFretboard/Examples/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      602 2023-05-17 18:35:46.000000 seeFretboard-0.0.9.4/seeFretboard/Examples/arpeggio.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      554 2023-05-23 22:12:06.000000 seeFretboard-0.0.9.4/seeFretboard/Examples/createMidiAudio.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      754 2023-05-24 06:43:40.000000 seeFretboard-0.0.9.4/seeFretboard/Examples/createVideo.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      829 2023-05-24 06:45:32.000000 seeFretboard-0.0.9.4/seeFretboard/Examples/createVideoWithAudio.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1013 2023-05-24 06:41:18.000000 seeFretboard-0.0.9.4/seeFretboard/Examples/createVideoWithMidiAudio.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      416 2023-05-24 13:28:52.000000 seeFretboard-0.0.9.4/seeFretboard/Examples/figureNextToEachOther.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      438 2023-05-24 15:45:15.000000 seeFretboard-0.0.9.4/seeFretboard/Examples/generateScriptAndDiv.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      278 2023-05-24 15:59:25.000000 seeFretboard-0.0.9.4/seeFretboard/Examples/generateStandalone.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      421 2023-05-16 18:33:07.000000 seeFretboard-0.0.9.4/seeFretboard/Examples/groundtruthVPredictionTest.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      239 2023-05-24 19:24:55.000000 seeFretboard-0.0.9.4/seeFretboard/Examples/horizontalFretboard.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      282 2023-05-16 17:18:49.000000 seeFretboard-0.0.9.4/seeFretboard/Examples/horizontalFretboardAddNotes.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      492 2023-05-16 18:32:52.000000 seeFretboard-0.0.9.4/seeFretboard/Examples/interval.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      648 2023-05-23 17:47:04.000000 seeFretboard-0.0.9.4/seeFretboard/Examples/saveVideoWithAudio.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      825 2023-05-17 13:39:03.000000 seeFretboard-0.0.9.4/seeFretboard/Examples/scale.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      980 2023-05-16 18:32:51.000000 seeFretboard-0.0.9.4/seeFretboard/Examples/testText.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      238 2023-05-16 18:32:51.000000 seeFretboard-0.0.9.4/seeFretboard/Examples/verticalFretboard.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      282 2023-05-16 18:32:51.000000 seeFretboard-0.0.9.4/seeFretboard/Examples/verticalFretboardAddNotes.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      349 2023-05-24 19:59:19.000000 seeFretboard-0.0.9.4/seeFretboard/NotePosition.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1002 2023-05-24 15:44:17.000000 seeFretboard-0.0.9.4/seeFretboard/PathInfo.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7371 2023-05-23 15:53:29.000000 seeFretboard-0.0.9.4/seeFretboard/PitchCollection.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    49005 2023-05-25 03:59:18.000000 seeFretboard-0.0.9.4/seeFretboard/SeeFretboard.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.936531 seeFretboard-0.0.9.4/seeFretboard/Utilities/
--rw-r--r--   0 lindazhang   (501) staff       (20)     1760 2023-05-24 16:11:25.000000 seeFretboard-0.0.9.4/seeFretboard/Utilities/Constants.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     3532 2023-05-23 05:52:24.000000 seeFretboard-0.0.9.4/seeFretboard/Utilities/Util.py
--rw-r--r--   0 lindazhang   (501) staff       (20)       44 2023-05-24 19:20:02.000000 seeFretboard-0.0.9.4/seeFretboard/Utilities/__init__.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.939386 seeFretboard-0.0.9.4/seeFretboard/Videos/
--rw-r--r--   0 lindazhang   (501) staff       (20)     2731 2023-05-24 04:39:52.000000 seeFretboard-0.0.9.4/seeFretboard/Videos/Audio.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      377 2023-04-26 17:58:37.000000 seeFretboard-0.0.9.4/seeFretboard/Videos/Frame.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1035 2023-05-24 05:48:56.000000 seeFretboard-0.0.9.4/seeFretboard/Videos/Images.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7079 2023-05-24 06:00:03.000000 seeFretboard-0.0.9.4/seeFretboard/Videos/TabSequence.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4603 2023-05-24 06:46:51.000000 seeFretboard-0.0.9.4/seeFretboard/Videos/Video.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     4093 2023-05-24 06:41:15.000000 seeFretboard-0.0.9.4/seeFretboard/Videos/VideoManager.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      549 2023-05-24 16:47:03.000000 seeFretboard-0.0.9.4/seeFretboard/Videos/VideoNote.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      262 2023-05-24 19:19:22.000000 seeFretboard-0.0.9.4/seeFretboard/Videos/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      240 2023-05-25 03:20:42.000000 seeFretboard-0.0.9.4/seeFretboard/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      430 2023-05-24 17:03:19.000000 seeFretboard-0.0.9.4/seeFretboard/generalTest.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:10:34.926328 seeFretboard-0.0.9.4/seeFretboard.egg-info/
--rw-r--r--   0 lindazhang   (501) staff       (20)     1372 2023-05-25 04:10:34.000000 seeFretboard-0.0.9.4/seeFretboard.egg-info/PKG-INFO
--rw-r--r--   0 lindazhang   (501) staff       (20)    52152 2023-05-25 04:10:34.000000 seeFretboard-0.0.9.4/seeFretboard.egg-info/SOURCES.txt
--rw-r--r--   0 lindazhang   (501) staff       (20)        1 2023-05-25 04:10:34.000000 seeFretboard-0.0.9.4/seeFretboard.egg-info/dependency_links.txt
--rw-r--r--   0 lindazhang   (501) staff       (20)        9 2023-05-25 04:10:34.000000 seeFretboard-0.0.9.4/seeFretboard.egg-info/requires.txt
--rw-r--r--   0 lindazhang   (501) staff       (20)       13 2023-05-25 04:10:34.000000 seeFretboard-0.0.9.4/seeFretboard.egg-info/top_level.txt
--rw-r--r--   0 lindazhang   (501) staff       (20)       38 2023-05-25 04:10:34.940067 seeFretboard-0.0.9.4/setup.cfg
--rw-r--r--   0 lindazhang   (501) staff       (20)      732 2023-05-25 04:07:20.000000 seeFretboard-0.0.9.4/setup.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.389978 seeFretboard-0.0.9.5/
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.178462 seeFretboard-0.0.9.5/.venv/
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.178514 seeFretboard-0.0.9.5/.venv/lib/
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.178573 seeFretboard-0.0.9.5/.venv/lib/python3.11/
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.183587 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.186896 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/_distutils_hack/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6128 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/_distutils_hack/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)       44 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/_distutils_hack/override.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.187812 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      355 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1198 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/__main__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1444 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/__pip-runner__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.189725 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      573 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10192 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10734 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cache.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.192367 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      132 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6676 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7842 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    29250 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      774 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2472 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4338 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10817 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1968 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18172 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5118 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      116 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/status_codes.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.196112 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3882 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7582 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1685 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4129 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9815 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6591 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5289 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2951 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1703 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1132 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4762 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3188 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    32234 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12343 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5697 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6419 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3755 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7396 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13529 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/configuration.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.197080 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/distributions/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      858 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1221 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      729 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6494 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1164 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    24091 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/exceptions.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.198411 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/index/
+-rw-r--r--   0 lindazhang   (501) staff       (20)       30 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    16504 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    37873 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6557 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/index/sources.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.199426 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/locations/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    17794 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6319 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8149 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2556 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      340 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/main.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.200269 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/metadata/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4280 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2595 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    25277 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/metadata/base.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.201134 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      107 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1882 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8181 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7457 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9773 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.203634 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/
+-rw-r--r--   0 lindazhang   (501) staff       (20)       63 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      990 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6442 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2520 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1030 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2617 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18602 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      738 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4644 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1907 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3858 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3600 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/wheel.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.205058 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/network/
+-rw-r--r--   0 lindazhang   (501) staff       (20)       50 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    16507 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2145 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6096 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7638 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18443 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4073 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1791 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.205657 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.207085 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4133 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1422 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1474 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2198 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1075 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1417 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3064 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5122 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9784 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/freeze.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.207838 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/
+-rw-r--r--   0 lindazhang   (501) staff       (20)       51 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1354 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4105 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/legacy.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    27407 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    25091 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6987 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/pyproject.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.209223 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/req/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2807 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    16611 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    17646 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    35763 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2858 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    24045 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.209650 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      583 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/base.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.210038 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    24129 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.212881 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5220 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18963 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    27878 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5705 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9914 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2526 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5455 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11533 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8167 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.219432 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1015 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1665 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1884 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5377 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      242 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5764 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3206 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1115 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/distutils_args.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2118 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1169 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3064 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5122 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      716 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3110 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4831 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      795 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11632 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    22253 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1193 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2108 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5662 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9200 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7702 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8821 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1759 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3456 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4549 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/wheel.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.220556 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/vcs/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      596 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3519 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18116 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5238 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11729 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    22811 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13079 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/wheel_builder.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.221371 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4966 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.223479 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      465 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1379 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5033 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1535 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.223978 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      242 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5271 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1033 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      778 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    16416 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3946 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4154 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7105 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      774 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.224438 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 lindazhang   (501) staff       (20)       94 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      255 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4279 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/core.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.239219 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4797 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    31274 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1763 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10032 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3915 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5420 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.239467 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3242 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3732 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      542 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1860 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1683 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4006 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12176 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3934 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13566 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1753 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    36913 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1753 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    20735 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1759 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14537 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    25796 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    42498 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1752 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    27055 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   104562 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    98484 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    98196 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   101363 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   128035 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   102774 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    95372 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5380 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6077 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3715 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2131 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    30391 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.240299 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13560 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      402 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6400 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4137 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4007 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14848 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8505 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2812 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      244 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/version.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.244682 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      266 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2522 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11128 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3325 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.246069 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/
+-rw-r--r--   0 lindazhang   (501) staff       (20)       75 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2839 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10678 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6741 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1866 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1079 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3709 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6181 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7134 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.251427 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      581 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    41259 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    51697 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    20834 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    51991 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14811 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5058 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    39801 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10820 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18102 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    66262 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    23513 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/version.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    43898 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.252800 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      981 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)       64 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    49330 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distro/distro.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.256460 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      849 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3374 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      321 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12950 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    44375 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1881 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)       21 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   206539 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.257625 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1132 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1081 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6080 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    34557 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.259995 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      661 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      497 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11488 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4378 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1431 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8487 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4676 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    30110 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    15699 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4200 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14665 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/version.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.260850 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/
+-rw-r--r--   0 lindazhang   (501) staff       (20)   108287 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      562 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/py31compat.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.262163 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12936 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1176 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4068 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4910 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2655 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6911 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      160 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6596 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.267938 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2999 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      353 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    23685 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1697 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1938 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.268227 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    40386 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2917 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.271644 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4810 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4104 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3314 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5086 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    35441 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    21938 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5871 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    19351 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5073 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2212 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5014 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7335 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4674 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11753 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    32005 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.272311 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11174 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    70232 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    53376 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      986 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2591 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3072 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3092 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4630 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6257 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/style.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.272557 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3419 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6184 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    63187 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9110 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/util.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.274831 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9171 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6426 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12936 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   213344 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.275011 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    23685 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9023 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    39129 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    25341 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13402 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10787 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6805 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.275589 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      491 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      138 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11920 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.276035 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      546 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10927 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.280161 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5178 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      435 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1397 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    21443 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6377 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10187 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      575 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1286 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18560 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3823 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3879 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      733 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    35288 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      695 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    30180 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4235 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2912 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    33240 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/utils.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.281471 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      537 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.281885 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      156 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5872 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1583 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    17592 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4794 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.301482 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6090 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8478 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10096 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   140235 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1064 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2114 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      265 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9695 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3225 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1236 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1643 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7063 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      423 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5472 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    19919 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      351 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      417 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    22820 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1926 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2783 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1840 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      890 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10368 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6819 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3264 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9842 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4503 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18015 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1054 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7131 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    97992 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1288 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5497 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6630 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7954 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      972 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2501 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      642 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1616 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2508 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9585 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5053 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3252 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14007 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14172 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3667 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11903 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8198 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5305 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4970 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      828 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3396 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10574 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    37414 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    59836 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8165 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11303 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1391 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      166 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4436 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4773 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2843 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1591 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    24224 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4374 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4425 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    26332 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1258 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    34995 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    39684 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3370 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    45686 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3627 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      102 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    26070 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9169 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    34549 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/six.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.303607 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18364 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3314 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1944 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1496 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1376 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1908 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1383 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7550 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2790 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2145 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8011 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.304433 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      396 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    22633 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2943 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      254 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    80114 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.307713 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3333 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10811 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)       64 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    20070 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    39095 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.309784 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      957 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.310829 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    17632 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13922 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11036 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4528 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    17081 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    34448 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7097 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8217 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8579 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2440 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.311192 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.311582 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1417 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    34665 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    19786 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5985 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    30641 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.316441 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1155 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4901 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1605 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      498 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3997 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3510 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    22003 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    17177 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5758 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6895 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10003 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14298 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5403 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.317999 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10579 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8979 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1305 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6563 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4307 2023-02-02 16:11:15.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.318205 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/
+-rw-r--r--   0 lindazhang   (501) staff       (20)   108568 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.320266 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    24701 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/appdirs.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.321987 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      506 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4504 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2741 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2706 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      884 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3494 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3886 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3566 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2836 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.322700 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5420 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13515 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.322930 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    15526 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.323740 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-r--r--   0 lindazhang   (501) staff       (20)       83 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   132569 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18410 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.325876 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      661 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      497 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11488 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4378 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1431 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8496 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4706 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    30110 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    15699 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4200 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14665 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.328213 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9159 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6426 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/actions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12936 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/common.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   213310 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/core.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.328433 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    23668 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9023 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    39129 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    25341 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/results.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13402 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/testing.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10787 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6805 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/util.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8425 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.328650 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/extern/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2426 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/extern/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.337408 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8429 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      218 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_deprecation_warning.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.344534 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      537 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1330 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/_collections.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      411 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/_functools.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      239 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    19672 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8603 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14789 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    47369 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    17973 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/cmd.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.350830 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      430 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1614 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5441 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4701 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    22051 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5617 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7728 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    31558 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    16568 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5624 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4888 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/check.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2603 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13137 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/config.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    30221 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2779 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2785 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1189 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8434 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1936 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      672 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11765 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/register.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    19241 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7477 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4920 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/config.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9451 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/core.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12537 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      139 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/debug.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3423 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8082 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    50186 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/dist.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3589 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/errors.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10270 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/extension.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    17910 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8226 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/file_util.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13713 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/filelist.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1972 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/log.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    30235 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    23602 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      217 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/py38compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      639 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3517 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/spawn.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18858 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12096 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/text_file.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    15641 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    18128 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/util.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12952 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/version.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5248 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1972 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_entry_points.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2392 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_imp.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1311 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_importlib.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      675 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_itertools.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      749 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_path.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      501 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_reqs.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.351915 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.353939 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    30130 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1862 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      743 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1828 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2895 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2068 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1154 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2166 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.357597 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      506 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4504 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2741 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2706 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      884 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3494 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3886 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3566 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2836 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.358022 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5420 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13512 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.358191 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    15517 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.359282 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/
+-rw-r--r--   0 lindazhang   (501) staff       (20)       82 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   117959 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    16256 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    15130 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.361548 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      661 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      497 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11488 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4378 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1431 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8493 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4700 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    30110 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    15699 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4200 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14665 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.364247 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9159 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6426 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/actions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    12936 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/common.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   213310 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/core.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.364481 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/
+-rw-r--r--   0 lindazhang   (501) staff       (20)    23668 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     9023 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    39129 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/helpers.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    25341 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/results.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13402 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/testing.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    10787 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/unicode.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6805 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/util.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.365479 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      396 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    22633 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2943 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      254 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    87149 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8425 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/zipp.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7346 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/archive_util.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    19539 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/build_meta.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.370991 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      396 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2381 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/alias.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    16623 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/bdist_egg.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1182 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6595 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/build.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4415 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/build_clib.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    15821 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/build_ext.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14115 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/build_py.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7012 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/develop.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4800 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/dist_info.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    85662 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/easy_install.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    31188 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/editable_wheel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    26795 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/egg_info.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5163 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/install.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2226 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/install_egg_info.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3875 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/install_lib.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2612 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/install_scripts.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4946 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/py36compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      468 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/register.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2128 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/rotate.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      658 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/saveopts.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7071 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/sdist.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5086 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/setopt.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8102 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/test.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      462 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/upload.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7494 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/upload_docs.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.372392 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1121 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    13398 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.374017 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1038 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    11266 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1153 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1612 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)   269900 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8736 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    16319 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/expand.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    19304 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    25198 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/setupcfg.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      949 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/dep_util.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5499 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/depends.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    20799 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/discovery.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    45578 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/dist.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2464 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/errors.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     5591 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/extension.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.374201 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/extern/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2512 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/extern/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4873 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/glob.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3824 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/installer.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      812 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/launch.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1210 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/logging.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4857 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/monkey.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    47724 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/msvc.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3093 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/namespaces.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    40020 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/package_index.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      245 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/py34compat.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    14348 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/sandbox.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      941 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/unicode_utils.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      144 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/version.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     8376 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/wheel.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      718 2023-02-02 16:11:14.000000 seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/windows_support.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.374380 seeFretboard-0.0.9.5/Examples/
+-rw-r--r--   0 lindazhang   (501) staff       (20)      239 2023-05-25 01:54:18.000000 seeFretboard-0.0.9.5/Examples/horizontalFretboard.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1072 2023-05-24 18:18:02.000000 seeFretboard-0.0.9.5/LICENSE
+-rw-r--r--   0 lindazhang   (501) staff       (20)       56 2023-05-25 02:46:38.000000 seeFretboard-0.0.9.5/MANIFEST.in
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1372 2023-05-25 04:34:59.389827 seeFretboard-0.0.9.5/PKG-INFO
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1005 2023-05-02 18:53:11.000000 seeFretboard-0.0.9.5/README.md
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.375096 seeFretboard-0.0.9.5/Tests/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7163 2023-05-24 07:07:44.000000 seeFretboard-0.0.9.5/Tests/StylesTest.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:56:48.000000 seeFretboard-0.0.9.5/Tests/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      287 2023-05-25 01:57:45.000000 seeFretboard-0.0.9.5/pyproject.toml
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.376852 seeFretboard-0.0.9.5/seeFretboard/
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.378875 seeFretboard-0.0.9.5/seeFretboard/Designs/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-24 06:03:38.000000 seeFretboard-0.0.9.5/seeFretboard/Designs/Buttons.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2163 2023-05-23 16:51:07.000000 seeFretboard-0.0.9.5/seeFretboard/Designs/CirlceNote.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3207 2023-05-24 16:53:11.000000 seeFretboard-0.0.9.5/seeFretboard/Designs/FretboardFigure.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6610 2023-05-23 21:33:59.000000 seeFretboard-0.0.9.5/seeFretboard/Designs/FretboardStyle.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      139 2023-05-24 19:26:22.000000 seeFretboard-0.0.9.5/seeFretboard/Designs/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.384870 seeFretboard-0.0.9.5/seeFretboard/Examples/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:55:42.000000 seeFretboard-0.0.9.5/seeFretboard/Examples/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      602 2023-05-17 18:35:46.000000 seeFretboard-0.0.9.5/seeFretboard/Examples/arpeggio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      554 2023-05-23 22:12:06.000000 seeFretboard-0.0.9.5/seeFretboard/Examples/createMidiAudio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      754 2023-05-24 06:43:40.000000 seeFretboard-0.0.9.5/seeFretboard/Examples/createVideo.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      829 2023-05-24 06:45:32.000000 seeFretboard-0.0.9.5/seeFretboard/Examples/createVideoWithAudio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1013 2023-05-24 06:41:18.000000 seeFretboard-0.0.9.5/seeFretboard/Examples/createVideoWithMidiAudio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      416 2023-05-24 13:28:52.000000 seeFretboard-0.0.9.5/seeFretboard/Examples/figureNextToEachOther.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      438 2023-05-24 15:45:15.000000 seeFretboard-0.0.9.5/seeFretboard/Examples/generateScriptAndDiv.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      278 2023-05-24 15:59:25.000000 seeFretboard-0.0.9.5/seeFretboard/Examples/generateStandalone.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      421 2023-05-16 18:33:07.000000 seeFretboard-0.0.9.5/seeFretboard/Examples/groundtruthVPredictionTest.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      239 2023-05-24 19:24:55.000000 seeFretboard-0.0.9.5/seeFretboard/Examples/horizontalFretboard.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      282 2023-05-16 17:18:49.000000 seeFretboard-0.0.9.5/seeFretboard/Examples/horizontalFretboardAddNotes.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      492 2023-05-16 18:32:52.000000 seeFretboard-0.0.9.5/seeFretboard/Examples/interval.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      648 2023-05-23 17:47:04.000000 seeFretboard-0.0.9.5/seeFretboard/Examples/saveVideoWithAudio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      825 2023-05-17 13:39:03.000000 seeFretboard-0.0.9.5/seeFretboard/Examples/scale.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      980 2023-05-16 18:32:51.000000 seeFretboard-0.0.9.5/seeFretboard/Examples/testText.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      238 2023-05-16 18:32:51.000000 seeFretboard-0.0.9.5/seeFretboard/Examples/verticalFretboard.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      282 2023-05-16 18:32:51.000000 seeFretboard-0.0.9.5/seeFretboard/Examples/verticalFretboardAddNotes.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      349 2023-05-24 19:59:19.000000 seeFretboard-0.0.9.5/seeFretboard/NotePosition.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1002 2023-05-24 15:44:17.000000 seeFretboard-0.0.9.5/seeFretboard/PathInfo.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7371 2023-05-23 15:53:29.000000 seeFretboard-0.0.9.5/seeFretboard/PitchCollection.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)    49005 2023-05-25 03:59:18.000000 seeFretboard-0.0.9.5/seeFretboard/SeeFretboard.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.385728 seeFretboard-0.0.9.5/seeFretboard/Utilities/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1760 2023-05-24 16:11:25.000000 seeFretboard-0.0.9.5/seeFretboard/Utilities/Constants.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3532 2023-05-23 05:52:24.000000 seeFretboard-0.0.9.5/seeFretboard/Utilities/Util.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)       44 2023-05-24 19:20:02.000000 seeFretboard-0.0.9.5/seeFretboard/Utilities/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.389328 seeFretboard-0.0.9.5/seeFretboard/Videos/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2731 2023-05-24 04:39:52.000000 seeFretboard-0.0.9.5/seeFretboard/Videos/Audio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      377 2023-04-26 17:58:37.000000 seeFretboard-0.0.9.5/seeFretboard/Videos/Frame.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1035 2023-05-24 05:48:56.000000 seeFretboard-0.0.9.5/seeFretboard/Videos/Images.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7079 2023-05-24 06:00:03.000000 seeFretboard-0.0.9.5/seeFretboard/Videos/TabSequence.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4603 2023-05-24 06:46:51.000000 seeFretboard-0.0.9.5/seeFretboard/Videos/Video.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4093 2023-05-24 06:41:15.000000 seeFretboard-0.0.9.5/seeFretboard/Videos/VideoManager.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      549 2023-05-24 16:47:03.000000 seeFretboard-0.0.9.5/seeFretboard/Videos/VideoNote.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      262 2023-05-24 19:19:22.000000 seeFretboard-0.0.9.5/seeFretboard/Videos/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)       70 2023-05-25 04:32:17.000000 seeFretboard-0.0.9.5/seeFretboard/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      268 2023-05-25 04:34:00.000000 seeFretboard-0.0.9.5/seeFretboard/generalTest.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-25 04:34:59.377717 seeFretboard-0.0.9.5/seeFretboard.egg-info/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1372 2023-05-25 04:34:58.000000 seeFretboard-0.0.9.5/seeFretboard.egg-info/PKG-INFO
+-rw-r--r--   0 lindazhang   (501) staff       (20)    52152 2023-05-25 04:34:59.000000 seeFretboard-0.0.9.5/seeFretboard.egg-info/SOURCES.txt
+-rw-r--r--   0 lindazhang   (501) staff       (20)        1 2023-05-25 04:34:58.000000 seeFretboard-0.0.9.5/seeFretboard.egg-info/dependency_links.txt
+-rw-r--r--   0 lindazhang   (501) staff       (20)        9 2023-05-25 04:34:58.000000 seeFretboard-0.0.9.5/seeFretboard.egg-info/requires.txt
+-rw-r--r--   0 lindazhang   (501) staff       (20)       13 2023-05-25 04:34:58.000000 seeFretboard-0.0.9.5/seeFretboard.egg-info/top_level.txt
+-rw-r--r--   0 lindazhang   (501) staff       (20)       38 2023-05-25 04:34:59.390060 seeFretboard-0.0.9.5/setup.cfg
+-rw-r--r--   0 lindazhang   (501) staff       (20)      732 2023-05-25 04:34:35.000000 seeFretboard-0.0.9.5/setup.py
```

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/_distutils_hack/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/__main__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/__pip-runner__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/build_env.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cache.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/base_command.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/command_context.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/main.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/parser.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/req_command.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/cli/spinners.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/cache.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/check.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/completion.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/configuration.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/debug.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/download.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/freeze.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/hash.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/help.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/index.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/inspect.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/install.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/list.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/search.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/show.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/commands/wheel.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/configuration.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/distributions/base.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/distributions/installed.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/exceptions.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/index/collector.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/index/package_finder.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/index/sources.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/locations/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/locations/base.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/metadata/_json.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/metadata/base.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/candidate.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/direct_url.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/format_control.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/index.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/installation_report.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/link.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/scheme.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/search_scope.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/target_python.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/models/wheel.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/network/auth.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/network/cache.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/network/download.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/network/session.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/network/utils.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/check.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/freeze.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/legacy.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/legacy.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/operations/prepare.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/pyproject.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/req/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/req/constructors.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/req/req_file.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/req/req_install.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/req/req_set.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/base.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/_log.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/compat.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/distutils_args.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/distutils_args.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/encoding.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/glibc.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/hashes.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/logging.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/misc.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/models.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/packaging.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/urls.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/utils/wheel.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/vcs/git.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_internal/wheel_builder.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/core.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/database.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/index.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/util.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/version.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/distro/distro.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/idna/codec.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/idna/core.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/version.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/py31compat.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/console.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/style.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/token.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/util.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/api.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/auth.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/certs.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/compat.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/help.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/models.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/packages.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/structures.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/requests/utils.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/abc.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/align.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/bar.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/box.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/cells.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/columns.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/console.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/containers.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/control.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/errors.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/json.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/layout.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/logging.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/markup.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/measure.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/padding.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pager.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/palette.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/panel.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/repr.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/rule.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/scope.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/screen.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/segment.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/status.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/style.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/styled.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/table.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/text.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/theme.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/rich/tree.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/six.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/appdirs.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__about__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/actions.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/common.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/core.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/helpers.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/results.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/testing.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/unicode.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/util.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/pkg_resources/extern/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/_collections.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/_collections.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/cmd.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/check.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/config.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/register.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/config.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/core.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/dist.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/errors.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/extension.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/file_util.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/filelist.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/log.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/spawn.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/text_file.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/util.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/version.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_entry_points.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_entry_points.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_imp.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_importlib.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_importlib.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_itertools.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_itertools.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_path.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_path.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/__about__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/actions.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/common.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/core.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/exceptions.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/helpers.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/results.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/testing.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/unicode.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/util.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/_vendor/zipp.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/archive_util.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/build_meta.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/alias.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/bdist_egg.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/build.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/build.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/build_clib.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/build_ext.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/build_py.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/develop.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/dist_info.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/easy_install.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/editable_wheel.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/editable_wheel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/egg_info.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/install.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/install_egg_info.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/install_lib.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/install_scripts.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/py36compat.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/py36compat.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/rotate.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/saveopts.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/sdist.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/setopt.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/test.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/command/upload_docs.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/expand.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/expand.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/config/setupcfg.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/config/setupcfg.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/dep_util.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/depends.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/discovery.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/discovery.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/dist.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/errors.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/extension.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/extern/__init__.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/glob.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/installer.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/launch.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/logging.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/logging.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/monkey.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/msvc.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/namespaces.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/package_index.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/sandbox.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/unicode_utils.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/wheel.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/.venv/lib/python3.11/site-packages/setuptools/windows_support.py` & `seeFretboard-0.0.9.5/.venv/lib/python3.11/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/LICENSE` & `seeFretboard-0.0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/PKG-INFO` & `seeFretboard-0.0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeFretboard
-Version: 0.0.9.4
+Version: 0.0.9.5
 Summary: Testing installation of Package
 Home-page: https://github.com/LindaRZhang/seeFretboard
 Author: Linda Rong Zhang
 Author-email: ronglindaz@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/LindaRZhang/seeFretboard/issues
 Description-Content-Type: text/markdown
```

### Comparing `seeFretboard-0.0.9.4/README.md` & `seeFretboard-0.0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/Tests/StylesTest.py` & `seeFretboard-0.0.9.5/Tests/StylesTest.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/Designs/CirlceNote.py` & `seeFretboard-0.0.9.5/seeFretboard/Designs/CirlceNote.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/Designs/FretboardFigure.py` & `seeFretboard-0.0.9.5/seeFretboard/Designs/FretboardFigure.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/Designs/FretboardStyle.py` & `seeFretboard-0.0.9.5/seeFretboard/Designs/FretboardStyle.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/Examples/arpeggio.py` & `seeFretboard-0.0.9.5/seeFretboard/Examples/arpeggio.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/Examples/createMidiAudio.py` & `seeFretboard-0.0.9.5/seeFretboard/Examples/createMidiAudio.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/Examples/createVideo.py` & `seeFretboard-0.0.9.5/seeFretboard/Examples/createVideo.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/Examples/createVideoWithAudio.py` & `seeFretboard-0.0.9.5/seeFretboard/Examples/createVideoWithAudio.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/Examples/createVideoWithMidiAudio.py` & `seeFretboard-0.0.9.5/seeFretboard/Examples/createVideoWithMidiAudio.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/Examples/saveVideoWithAudio.py` & `seeFretboard-0.0.9.5/seeFretboard/Examples/saveVideoWithAudio.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/Examples/scale.py` & `seeFretboard-0.0.9.5/seeFretboard/Examples/scale.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/Examples/testText.py` & `seeFretboard-0.0.9.5/seeFretboard/Examples/testText.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/PathInfo.py` & `seeFretboard-0.0.9.5/seeFretboard/PathInfo.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/PitchCollection.py` & `seeFretboard-0.0.9.5/seeFretboard/PitchCollection.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/SeeFretboard.py` & `seeFretboard-0.0.9.5/seeFretboard/SeeFretboard.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/Utilities/Constants.py` & `seeFretboard-0.0.9.5/seeFretboard/Utilities/Constants.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/Utilities/Util.py` & `seeFretboard-0.0.9.5/seeFretboard/Utilities/Util.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/Videos/Audio.py` & `seeFretboard-0.0.9.5/seeFretboard/Videos/Audio.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/Videos/Images.py` & `seeFretboard-0.0.9.5/seeFretboard/Videos/Images.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/Videos/TabSequence.py` & `seeFretboard-0.0.9.5/seeFretboard/Videos/TabSequence.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/Videos/Video.py` & `seeFretboard-0.0.9.5/seeFretboard/Videos/Video.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/Videos/VideoManager.py` & `seeFretboard-0.0.9.5/seeFretboard/Videos/VideoManager.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard/Videos/VideoNote.py` & `seeFretboard-0.0.9.5/seeFretboard/Videos/VideoNote.py`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/seeFretboard.egg-info/PKG-INFO` & `seeFretboard-0.0.9.5/seeFretboard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeFretboard
-Version: 0.0.9.4
+Version: 0.0.9.5
 Summary: Testing installation of Package
 Home-page: https://github.com/LindaRZhang/seeFretboard
 Author: Linda Rong Zhang
 Author-email: ronglindaz@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/LindaRZhang/seeFretboard/issues
 Description-Content-Type: text/markdown
```

### Comparing `seeFretboard-0.0.9.4/seeFretboard.egg-info/SOURCES.txt` & `seeFretboard-0.0.9.5/seeFretboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.9.4/setup.py` & `seeFretboard-0.0.9.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setuptools, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='seeFretboard',
-    version='0.0.9.4',
+    version='0.0.9.5',
     author='Linda Rong Zhang',
     author_email='ronglindaz@gmail.com',
     description='Testing installation of Package',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/LindaRZhang/seeFretboard',
     project_urls = {
```

