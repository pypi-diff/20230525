# Comparing `tmp/qtstrap-0.4.2.tar.gz` & `tmp/qtstrap-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtstrap-0.4.2.tar", last modified: Sat Apr 29 17:00:22 2023, max compression
+gzip compressed data, was "qtstrap-0.5.0.tar", last modified: Thu May 25 10:53:51 2023, max compression
```

## Comparing `qtstrap-0.4.2.tar` & `qtstrap-0.5.0.tar`

### file list

```diff
@@ -1,193 +1,194 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.424636 qtstrap-0.4.2/
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:21.287636 qtstrap-0.4.2/.github/
--rw-rw-rw-   0        0        0      784 2023-03-26 02:17:30.000000 qtstrap-0.4.2/.github/FUNDING.yml
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:21.289135 qtstrap-0.4.2/.github/workflows/
--rw-rw-rw-   0        0        0      978 2022-07-30 04:06:00.000000 qtstrap-0.4.2/.github/workflows/main.yml
--rw-rw-rw-   0        0        0      161 2022-11-24 04:51:10.000000 qtstrap-0.4.2/.gitignore
--rw-rw-rw-   0        0        0     1090 2021-04-01 21:16:04.000000 qtstrap-0.4.2/LICENSE
--rw-rw-rw-   0        0        0       96 2021-04-01 21:16:04.000000 qtstrap-0.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2600 2023-03-07 12:46:55.000000 qtstrap-0.4.2/Makefile
--rw-rw-rw-   0        0        0     3396 2023-04-29 17:00:22.425138 qtstrap-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     2441 2023-03-27 09:49:48.000000 qtstrap-0.4.2/README.md
--rw-rw-rw-   0        0        0      272 2022-07-30 03:58:00.000000 qtstrap-0.4.2/build_docs.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:21.317633 qtstrap-0.4.2/docs/
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:21.776635 qtstrap-0.4.2/docs/api/
--rw-rw-rw-   0        0        0       68 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/.pages
--rw-rw-rw-   0        0        0     4540 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.code_editor.code_editor.md
--rw-rw-rw-   0        0        0     1305 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.code_editor.code_line.md
--rw-rw-rw-   0        0        0      448 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.code_editor.highlighters.md
--rw-rw-rw-   0        0        0     3021 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.code_editor.highlighters.python.md
--rw-rw-rw-   0        0        0      464 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.code_editor.md
--rw-rw-rw-   0        0        0     8390 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.command_palette.command_palette.md
--rw-rw-rw-   0        0        0      439 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.command_palette.md
--rw-rw-rw-   0        0        0     2349 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.log_monitor.log_database_handler.md
--rw-rw-rw-   0        0        0    13379 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.log_monitor.log_filter_controls.md
--rw-rw-rw-   0        0        0     3604 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.log_monitor.log_profile.md
--rw-rw-rw-   0        0        0     4181 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.log_monitor.log_table_view.md
--rw-rw-rw-   0        0        0     4558 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.log_monitor.log_widget.md
--rw-rw-rw-   0        0        0      887 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.log_monitor.md
--rw-rw-rw-   0        0        0      342 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.md
--rw-rw-rw-   0        0        0      802 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.style.colors.md
--rw-rw-rw-   0        0        0      772 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.style.dark_palette.md
--rw-rw-rw-   0        0        0      430 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.style.md
--rw-rw-rw-   0        0        0     1259 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.style.themes.md
--rw-rw-rw-   0        0        0      546 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/options.md
--rw-rw-rw-   0        0        0    11165 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/overview.md
--rw-rw-rw-   0        0        0      754 2022-07-30 03:58:01.000000 qtstrap-0.4.2/docs/api/settings.md
--rw-rw-rw-   0        0        0     1958 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.adapter.md
--rw-rw-rw-   0        0        0      784 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.call_later.md
--rw-rw-rw-   0        0        0      599 2022-07-30 03:58:01.000000 qtstrap-0.4.2/docs/api/utils.decorators.md
--rw-rw-rw-   0        0        0     1019 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.defer.md
--rw-rw-rw-   0        0        0     1641 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.drag_and_drop.md
--rw-rw-rw-   0        0        0      742 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.get_ip.md
--rw-rw-rw-   0        0        0      459 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.md
--rw-rw-rw-   0        0        0      946 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.signals.md
--rw-rw-rw-   0        0        0      607 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.singleton.md
--rw-rw-rw-   0        0        0     1414 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.string_builder.md
--rw-rw-rw-   0        0        0     1597 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.timestamp.md
--rw-rw-rw-   0        0        0      641 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.trace.md
--rw-rw-rw-   0        0        0     2555 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.utils.md
--rw-rw-rw-   0        0        0     4948 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/widgets.buttons.md
--rw-rw-rw-   0        0        0     2853 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/widgets.labeledit.md
--rw-rw-rw-   0        0        0    16745 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/widgets.layouts.md
--rw-rw-rw-   0        0        0     1464 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/widgets.line_widgets.md
--rw-rw-rw-   0        0        0     1764 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/widgets.link_label.md
--rw-rw-rw-   0        0        0      555 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/widgets.md
--rw-rw-rw-   0        0        0     3040 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/widgets.persistent_tab_widget.md
--rw-rw-rw-   0        0        0     7854 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/widgets.persistent_widgets.md
--rw-rw-rw-   0        0        0     7763 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/widgets.toggle.md
--rw-rw-rw-   0        0        0     1276 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/widgets.toolbar.md
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:21.842636 qtstrap-0.4.2/docs/extras/
--rw-rw-rw-   0        0        0      684 2023-03-27 09:12:02.000000 qtstrap-0.4.2/docs/extras/code_editor.md
--rw-rw-rw-   0        0        0     1183 2023-03-27 09:27:16.000000 qtstrap-0.4.2/docs/extras/command_palette.md
--rw-rw-rw-   0        0        0      105 2023-03-27 09:29:20.000000 qtstrap-0.4.2/docs/extras/index.md
--rw-rw-rw-   0        0        0     1594 2023-03-27 09:42:00.000000 qtstrap-0.4.2/docs/extras/log_monitor.md
--rw-rw-rw-   0        0        0       48 2023-03-27 09:41:38.000000 qtstrap-0.4.2/docs/extras/styles.md
--rw-rw-rw-   0        0        0     1611 2023-03-26 02:25:27.000000 qtstrap-0.4.2/docs/index.md
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:21.910637 qtstrap-0.4.2/docs/quickstart/
--rw-rw-rw-   0        0        0     2618 2021-04-01 21:16:04.000000 qtstrap-0.4.2/docs/quickstart/baseapplication.md
--rw-rw-rw-   0        0        0      920 2021-04-01 21:16:04.000000 qtstrap-0.4.2/docs/quickstart/basemainwindow.md
--rw-rw-rw-   0        0        0     1700 2021-04-01 21:16:04.000000 qtstrap-0.4.2/docs/quickstart/context_layouts.md
--rw-rw-rw-   0        0        0     1264 2021-04-02 17:24:51.000000 qtstrap-0.4.2/docs/quickstart/gettingstarted.md
--rw-rw-rw-   0        0        0      857 2021-04-01 21:16:04.000000 qtstrap-0.4.2/docs/quickstart/installation.md
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.166135 qtstrap-0.4.2/docs/reference/
--rw-rw-rw-   0        0        0      759 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/base_application.md
--rw-rw-rw-   0        0        0      682 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/base_window.md
--rw-rw-rw-   0        0        0      653 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/options.md
--rw-rw-rw-   0        0        0      287 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/settings.md
--rw-rw-rw-   0        0        0      962 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/toolbar.md
--rw-rw-rw-   0        0        0     1484 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/utils.adapter.md
--rw-rw-rw-   0        0        0       88 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/utils.decorators.md
--rw-rw-rw-   0        0        0      618 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/utils.defer.md
--rw-rw-rw-   0        0        0      353 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/utils.md
--rw-rw-rw-   0        0        0      576 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/utils.signals.md
--rw-rw-rw-   0        0        0      105 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/utils.singleton.md
--rw-rw-rw-   0        0        0      690 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/utils.timestamp.md
--rw-rw-rw-   0        0        0     1349 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/utils.utils.md
--rw-rw-rw-   0        0        0     2361 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/widgets.buttons.md
--rw-rw-rw-   0        0        0     1196 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/widgets.labeledit.md
--rw-rw-rw-   0        0        0     4766 2022-07-30 03:40:51.000000 qtstrap-0.4.2/docs/reference/widgets.layouts.md
--rw-rw-rw-   0        0        0      516 2022-07-30 03:40:51.000000 qtstrap-0.4.2/docs/reference/widgets.line_widgets.md
--rw-rw-rw-   0        0        0      638 2022-07-30 03:40:51.000000 qtstrap-0.4.2/docs/reference/widgets.link_label.md
--rw-rw-rw-   0        0        0     1408 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/widgets.md
--rw-rw-rw-   0        0        0     1324 2022-07-30 03:40:51.000000 qtstrap-0.4.2/docs/reference/widgets.persistent_tab_widget.md
--rw-rw-rw-   0        0        0     3704 2022-07-30 03:40:51.000000 qtstrap-0.4.2/docs/reference/widgets.persistent_widgets.md
--rw-rw-rw-   0        0        0     2949 2021-04-01 21:16:04.000000 qtstrap-0.4.2/docs/screenshot1.png
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.194635 qtstrap-0.4.2/docs/structure/
--rw-rw-rw-   0        0        0     1193 2021-04-01 21:16:04.000000 qtstrap-0.4.2/docs/structure/makefile.md
--rw-rw-rw-   0        0        0     3013 2022-07-30 00:37:45.000000 qtstrap-0.4.2/docs/structure/structure.md
--rw-rw-rw-   0        0        0     7886 2022-07-30 03:01:48.000000 qtstrap-0.4.2/docs/test.md
--rw-rw-rw-   0        0        0      987 2023-03-27 08:50:48.000000 qtstrap-0.4.2/mkdocs.yml
--rw-rw-rw-   0        0        0      345 2022-07-30 04:03:13.000000 qtstrap-0.4.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.232138 qtstrap-0.4.2/qtstrap/
--rw-rw-rw-   0        0        0     1035 2023-03-07 12:33:33.000000 qtstrap-0.4.2/qtstrap/__init__.py
--rw-rw-rw-   0        0        0     1901 2023-03-27 08:38:01.000000 qtstrap-0.4.2/qtstrap/__main__.py
--rw-rw-rw-   0        0        0     2051 2023-03-07 12:17:44.000000 qtstrap-0.4.2/qtstrap/base_application.py
--rw-rw-rw-   0        0        0     2074 2023-03-07 12:38:24.000000 qtstrap-0.4.2/qtstrap/base_window.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.303636 qtstrap-0.4.2/qtstrap/experimental/
--rw-rw-rw-   0        0        0        0 2023-04-03 00:57:28.000000 qtstrap-0.4.2/qtstrap/experimental/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.305137 qtstrap-0.4.2/qtstrap/extras/
--rw-rw-rw-   0        0        0        0 2021-04-08 13:05:51.000000 qtstrap-0.4.2/qtstrap/extras/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.311637 qtstrap-0.4.2/qtstrap/extras/code_editor/
--rw-rw-rw-   0        0        0      113 2022-05-01 01:28:19.000000 qtstrap-0.4.2/qtstrap/extras/code_editor/__init__.py
--rw-rw-rw-   0        0        0    12535 2023-03-27 09:14:21.000000 qtstrap-0.4.2/qtstrap/extras/code_editor/code_editor.py
--rw-rw-rw-   0        0        0      847 2022-12-10 23:54:46.000000 qtstrap-0.4.2/qtstrap/extras/code_editor/code_line.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.316135 qtstrap-0.4.2/qtstrap/extras/code_editor/highlighters/
--rw-rw-rw-   0        0        0       37 2021-04-25 18:57:56.000000 qtstrap-0.4.2/qtstrap/extras/code_editor/highlighters/__init__.py
--rw-rw-rw-   0        0        0     6354 2023-03-07 12:26:48.000000 qtstrap-0.4.2/qtstrap/extras/code_editor/highlighters/python.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.318634 qtstrap-0.4.2/qtstrap/extras/command_palette/
--rw-rw-rw-   0        0        0       52 2021-07-23 15:36:03.000000 qtstrap-0.4.2/qtstrap/extras/command_palette/__init__.py
--rw-rw-rw-   0        0        0    11678 2023-03-27 09:27:44.000000 qtstrap-0.4.2/qtstrap/extras/command_palette/command_palette.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.332635 qtstrap-0.4.2/qtstrap/extras/log_monitor/
--rw-rw-rw-   0        0        0     1124 2022-12-23 00:25:27.000000 qtstrap-0.4.2/qtstrap/extras/log_monitor/__init__.py
--rw-rw-rw-   0        0        0     2437 2022-12-23 00:25:31.000000 qtstrap-0.4.2/qtstrap/extras/log_monitor/log_database_handler.py
--rw-rw-rw-   0        0        0    16819 2023-04-29 15:39:56.000000 qtstrap-0.4.2/qtstrap/extras/log_monitor/log_filter_controls.py
--rw-rw-rw-   0        0        0     4165 2022-12-22 21:39:18.000000 qtstrap-0.4.2/qtstrap/extras/log_monitor/log_profile.py
--rw-rw-rw-   0        0        0     3935 2023-04-29 15:35:41.000000 qtstrap-0.4.2/qtstrap/extras/log_monitor/log_table_view.py
--rw-rw-rw-   0        0        0     4710 2023-03-03 07:38:29.000000 qtstrap-0.4.2/qtstrap/extras/log_monitor/log_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.352135 qtstrap-0.4.2/qtstrap/extras/style/
--rw-rw-rw-   0        0        0      129 2023-03-03 07:24:23.000000 qtstrap-0.4.2/qtstrap/extras/style/__init__.py
--rw-rw-rw-   0        0        0     1085 2023-01-12 03:06:47.000000 qtstrap-0.4.2/qtstrap/extras/style/colors.py
--rw-rw-rw-   0        0        0     2040 2023-03-03 07:24:23.000000 qtstrap-0.4.2/qtstrap/extras/style/dark_palette.py
--rw-rw-rw-   0        0        0     4105 2023-03-07 12:55:24.000000 qtstrap-0.4.2/qtstrap/extras/style/themes.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.353636 qtstrap-0.4.2/qtstrap/optional/
--rw-rw-rw-   0        0        0        0 2023-04-03 00:57:38.000000 qtstrap-0.4.2/qtstrap/optional/__init__.py
--rw-rw-rw-   0        0        0     1174 2022-12-10 01:10:44.000000 qtstrap-0.4.2/qtstrap/options.py
--rw-rw-rw-   0        0        0      694 2023-03-27 08:40:17.000000 qtstrap-0.4.2/qtstrap/qt.py
--rw-rw-rw-   0        0        0      504 2022-12-09 05:56:13.000000 qtstrap-0.4.2/qtstrap/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.360637 qtstrap-0.4.2/qtstrap/template/
--rw-rw-rw-   0        0        0     3629 2022-07-30 00:00:03.000000 qtstrap-0.4.2/qtstrap/template/Makefile
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.362136 qtstrap-0.4.2/qtstrap/template/app/
--rw-rw-rw-   0        0        0      953 2021-04-02 17:24:51.000000 qtstrap-0.4.2/qtstrap/template/app/main.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.366135 qtstrap-0.4.2/qtstrap/template/app/resources/
--rw-rw-rw-   0        0        0    59285 2021-04-01 21:16:04.000000 qtstrap-0.4.2/qtstrap/template/app/resources/application.ico
--rw-rw-rw-   0        0        0     5523 2021-04-01 21:16:04.000000 qtstrap-0.4.2/qtstrap/template/app/resources/icon.svg
--rw-rw-rw-   0        0        0     1195 2022-09-11 05:33:04.000000 qtstrap-0.4.2/qtstrap/template/bundle.spec
--rw-rw-rw-   0        0        0     2450 2022-07-29 23:52:21.000000 qtstrap-0.4.2/qtstrap/template/installer.iss
--rw-rw-rw-   0        0        0        0 2021-04-01 21:16:04.000000 qtstrap-0.4.2/qtstrap/template/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.392636 qtstrap-0.4.2/qtstrap/utils/
--rw-rw-rw-   0        0        0      390 2022-12-08 21:10:40.000000 qtstrap-0.4.2/qtstrap/utils/__init__.py
--rw-rw-rw-   0        0        0     2469 2023-03-26 02:15:24.000000 qtstrap-0.4.2/qtstrap/utils/adapter.py
--rw-rw-rw-   0        0        0      265 2022-10-20 22:39:10.000000 qtstrap-0.4.2/qtstrap/utils/call_later.py
--rw-rw-rw-   0        0        0      652 2021-05-13 17:33:19.000000 qtstrap-0.4.2/qtstrap/utils/defer.py
--rw-rw-rw-   0        0        0     2800 2022-12-12 00:29:52.000000 qtstrap-0.4.2/qtstrap/utils/drag_and_drop.py
--rw-rw-rw-   0        0        0      629 2022-11-03 16:33:13.000000 qtstrap-0.4.2/qtstrap/utils/get_ip.py
--rw-rw-rw-   0        0        0      378 2023-02-04 21:57:48.000000 qtstrap-0.4.2/qtstrap/utils/signals.py
--rw-rw-rw-   0        0        0      255 2022-11-03 16:23:26.000000 qtstrap-0.4.2/qtstrap/utils/singleton.py
--rw-rw-rw-   0        0        0      751 2023-02-04 22:01:45.000000 qtstrap-0.4.2/qtstrap/utils/string_builder.py
--rw-rw-rw-   0        0        0      531 2021-10-30 07:31:06.000000 qtstrap-0.4.2/qtstrap/utils/timestamp.py
--rw-rw-rw-   0        0        0      291 2022-12-11 02:07:30.000000 qtstrap-0.4.2/qtstrap/utils/trace.py
--rw-rw-rw-   0        0        0     2491 2022-11-03 16:16:04.000000 qtstrap-0.4.2/qtstrap/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.411638 qtstrap-0.4.2/qtstrap/widgets/
--rw-rw-rw-   0        0        0      890 2023-02-23 14:40:05.000000 qtstrap-0.4.2/qtstrap/widgets/__init__.py
--rw-rw-rw-   0        0        0     2973 2022-12-09 06:51:34.000000 qtstrap-0.4.2/qtstrap/widgets/buttons.py
--rw-rw-rw-   0        0        0     1590 2022-05-15 05:13:52.000000 qtstrap-0.4.2/qtstrap/widgets/labeledit.py
--rw-rw-rw-   0        0        0     8559 2023-04-29 16:55:24.000000 qtstrap-0.4.2/qtstrap/widgets/layouts.py
--rw-rw-rw-   0        0        0      665 2021-04-01 21:16:04.000000 qtstrap-0.4.2/qtstrap/widgets/line_widgets.py
--rw-rw-rw-   0        0        0      824 2022-10-26 07:40:04.000000 qtstrap-0.4.2/qtstrap/widgets/link_label.py
--rw-rw-rw-   0        0        0     3161 2021-05-06 02:08:19.000000 qtstrap-0.4.2/qtstrap/widgets/persistent_tab_widget.py
--rw-rw-rw-   0        0        0     5473 2022-11-10 17:33:23.000000 qtstrap-0.4.2/qtstrap/widgets/persistent_widgets.py
--rw-rw-rw-   0        0        0     7568 2023-03-03 08:21:01.000000 qtstrap-0.4.2/qtstrap/widgets/toggle.py
--rw-rw-rw-   0        0        0      910 2022-11-07 02:00:59.000000 qtstrap-0.4.2/qtstrap/widgets/toolbar.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.302640 qtstrap-0.4.2/qtstrap.egg-info/
--rw-rw-rw-   0        0        0     3396 2023-04-29 17:00:21.000000 qtstrap-0.4.2/qtstrap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4908 2023-04-29 17:00:21.000000 qtstrap-0.4.2/qtstrap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 17:00:21.000000 qtstrap-0.4.2/qtstrap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-29 17:00:21.000000 qtstrap-0.4.2/qtstrap.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-12-23 00:34:54.000000 qtstrap-0.4.2/qtstrap.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       52 2023-04-29 17:00:21.000000 qtstrap-0.4.2/qtstrap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-29 17:00:21.000000 qtstrap-0.4.2/qtstrap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1141 2022-11-30 17:51:25.000000 qtstrap-0.4.2/requirements.txt
--rw-rw-rw-   0        0        0      529 2022-10-26 06:20:37.000000 qtstrap-0.4.2/requirements_build.txt
--rw-rw-rw-   0        0        0      520 2022-10-26 06:55:20.000000 qtstrap-0.4.2/requirements_test.txt
--rw-rw-rw-   0        0        0      158 2022-11-24 06:15:10.000000 qtstrap-0.4.2/run_tox_tests.py
--rw-rw-rw-   0        0        0     1254 2023-04-29 17:00:22.428137 qtstrap-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0       96 2022-07-30 01:23:30.000000 qtstrap-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.422135 qtstrap-0.4.2/test/
--rw-rw-rw-   0        0        0      876 2021-04-01 21:16:04.000000 qtstrap-0.4.2/test/test_base_app.py
--rw-rw-rw-   0        0        0     1073 2021-04-01 21:16:04.000000 qtstrap-0.4.2/test/test_base_window.py
--rw-rw-rw-   0        0        0      616 2022-11-24 06:02:31.000000 qtstrap-0.4.2/test/test_layouts.py
--rw-rw-rw-   0        0        0     2689 2022-11-24 05:29:55.000000 qtstrap-0.4.2/test/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.423635 qtstrap-0.4.2/test/utils/
--rw-rw-rw-   0        0        0      230 2022-11-24 04:25:54.000000 qtstrap-0.4.2/test/utils/test_defer.py
--rw-rw-rw-   0        0        0      348 2022-11-30 16:27:29.000000 qtstrap-0.4.2/tox.ini
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:51.549517 qtstrap-0.5.0/
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:50.421516 qtstrap-0.5.0/.github/
+-rw-rw-rw-   0        0        0      784 2023-03-26 02:17:30.000000 qtstrap-0.5.0/.github/FUNDING.yml
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:50.423018 qtstrap-0.5.0/.github/workflows/
+-rw-rw-rw-   0        0        0      978 2022-07-30 04:06:00.000000 qtstrap-0.5.0/.github/workflows/main.yml
+-rw-rw-rw-   0        0        0      161 2022-11-24 04:51:10.000000 qtstrap-0.5.0/.gitignore
+-rw-rw-rw-   0        0        0     1090 2021-04-01 21:16:04.000000 qtstrap-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0       96 2021-04-01 21:16:04.000000 qtstrap-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2600 2023-03-07 12:46:55.000000 qtstrap-0.5.0/Makefile
+-rw-rw-rw-   0        0        0     3396 2023-05-25 10:53:51.549517 qtstrap-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2441 2023-03-27 09:49:48.000000 qtstrap-0.5.0/README.md
+-rw-rw-rw-   0        0        0      272 2022-07-30 03:58:00.000000 qtstrap-0.5.0/build_docs.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:50.449019 qtstrap-0.5.0/docs/
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:50.869517 qtstrap-0.5.0/docs/api/
+-rw-rw-rw-   0        0        0       68 2023-03-27 09:43:37.000000 qtstrap-0.5.0/docs/api/.pages
+-rw-rw-rw-   0        0        0     4540 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/extras.code_editor.code_editor.md
+-rw-rw-rw-   0        0        0     1305 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/extras.code_editor.code_line.md
+-rw-rw-rw-   0        0        0      448 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/extras.code_editor.highlighters.md
+-rw-rw-rw-   0        0        0     3021 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/extras.code_editor.highlighters.python.md
+-rw-rw-rw-   0        0        0      464 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/extras.code_editor.md
+-rw-rw-rw-   0        0        0     8390 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/extras.command_palette.command_palette.md
+-rw-rw-rw-   0        0        0      439 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/extras.command_palette.md
+-rw-rw-rw-   0        0        0     2349 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/extras.log_monitor.log_database_handler.md
+-rw-rw-rw-   0        0        0    13379 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/extras.log_monitor.log_filter_controls.md
+-rw-rw-rw-   0        0        0     3604 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/extras.log_monitor.log_profile.md
+-rw-rw-rw-   0        0        0     4181 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/extras.log_monitor.log_table_view.md
+-rw-rw-rw-   0        0        0     4558 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/extras.log_monitor.log_widget.md
+-rw-rw-rw-   0        0        0      887 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/extras.log_monitor.md
+-rw-rw-rw-   0        0        0      342 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/extras.md
+-rw-rw-rw-   0        0        0      802 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/extras.style.colors.md
+-rw-rw-rw-   0        0        0      772 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/extras.style.dark_palette.md
+-rw-rw-rw-   0        0        0      430 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/extras.style.md
+-rw-rw-rw-   0        0        0     1259 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/extras.style.themes.md
+-rw-rw-rw-   0        0        0      546 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/options.md
+-rw-rw-rw-   0        0        0    11165 2023-03-27 09:43:37.000000 qtstrap-0.5.0/docs/api/overview.md
+-rw-rw-rw-   0        0        0      754 2022-07-30 03:58:01.000000 qtstrap-0.5.0/docs/api/settings.md
+-rw-rw-rw-   0        0        0     1958 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/utils.adapter.md
+-rw-rw-rw-   0        0        0      784 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/utils.call_later.md
+-rw-rw-rw-   0        0        0      599 2022-07-30 03:58:01.000000 qtstrap-0.5.0/docs/api/utils.decorators.md
+-rw-rw-rw-   0        0        0     1019 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/utils.defer.md
+-rw-rw-rw-   0        0        0     1641 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/utils.drag_and_drop.md
+-rw-rw-rw-   0        0        0      742 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/utils.get_ip.md
+-rw-rw-rw-   0        0        0      459 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/utils.md
+-rw-rw-rw-   0        0        0      946 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/utils.signals.md
+-rw-rw-rw-   0        0        0      607 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/utils.singleton.md
+-rw-rw-rw-   0        0        0     1414 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/utils.string_builder.md
+-rw-rw-rw-   0        0        0     1597 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/utils.timestamp.md
+-rw-rw-rw-   0        0        0      641 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/utils.trace.md
+-rw-rw-rw-   0        0        0     2555 2023-03-27 09:43:36.000000 qtstrap-0.5.0/docs/api/utils.utils.md
+-rw-rw-rw-   0        0        0     4948 2023-03-27 09:43:37.000000 qtstrap-0.5.0/docs/api/widgets.buttons.md
+-rw-rw-rw-   0        0        0     2853 2023-03-27 09:43:37.000000 qtstrap-0.5.0/docs/api/widgets.labeledit.md
+-rw-rw-rw-   0        0        0    16745 2023-03-27 09:43:37.000000 qtstrap-0.5.0/docs/api/widgets.layouts.md
+-rw-rw-rw-   0        0        0     1464 2023-03-27 09:43:37.000000 qtstrap-0.5.0/docs/api/widgets.line_widgets.md
+-rw-rw-rw-   0        0        0     1764 2023-03-27 09:43:37.000000 qtstrap-0.5.0/docs/api/widgets.link_label.md
+-rw-rw-rw-   0        0        0      555 2023-03-27 09:43:37.000000 qtstrap-0.5.0/docs/api/widgets.md
+-rw-rw-rw-   0        0        0     3040 2023-03-27 09:43:37.000000 qtstrap-0.5.0/docs/api/widgets.persistent_tab_widget.md
+-rw-rw-rw-   0        0        0     7854 2023-03-27 09:43:37.000000 qtstrap-0.5.0/docs/api/widgets.persistent_widgets.md
+-rw-rw-rw-   0        0        0     7763 2023-03-27 09:43:37.000000 qtstrap-0.5.0/docs/api/widgets.toggle.md
+-rw-rw-rw-   0        0        0     1276 2023-03-27 09:43:37.000000 qtstrap-0.5.0/docs/api/widgets.toolbar.md
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:50.917018 qtstrap-0.5.0/docs/extras/
+-rw-rw-rw-   0        0        0      684 2023-03-27 09:12:02.000000 qtstrap-0.5.0/docs/extras/code_editor.md
+-rw-rw-rw-   0        0        0     1183 2023-03-27 09:27:16.000000 qtstrap-0.5.0/docs/extras/command_palette.md
+-rw-rw-rw-   0        0        0      105 2023-03-27 09:29:20.000000 qtstrap-0.5.0/docs/extras/index.md
+-rw-rw-rw-   0        0        0     1594 2023-03-27 09:42:00.000000 qtstrap-0.5.0/docs/extras/log_monitor.md
+-rw-rw-rw-   0        0        0       48 2023-03-27 09:41:38.000000 qtstrap-0.5.0/docs/extras/styles.md
+-rw-rw-rw-   0        0        0     1611 2023-03-26 02:25:27.000000 qtstrap-0.5.0/docs/index.md
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:50.966016 qtstrap-0.5.0/docs/quickstart/
+-rw-rw-rw-   0        0        0     2618 2021-04-01 21:16:04.000000 qtstrap-0.5.0/docs/quickstart/baseapplication.md
+-rw-rw-rw-   0        0        0      920 2021-04-01 21:16:04.000000 qtstrap-0.5.0/docs/quickstart/basemainwindow.md
+-rw-rw-rw-   0        0        0     1700 2021-04-01 21:16:04.000000 qtstrap-0.5.0/docs/quickstart/context_layouts.md
+-rw-rw-rw-   0        0        0     1264 2021-04-02 17:24:51.000000 qtstrap-0.5.0/docs/quickstart/gettingstarted.md
+-rw-rw-rw-   0        0        0      857 2021-04-01 21:16:04.000000 qtstrap-0.5.0/docs/quickstart/installation.md
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:51.219018 qtstrap-0.5.0/docs/reference/
+-rw-rw-rw-   0        0        0      759 2022-07-30 03:40:50.000000 qtstrap-0.5.0/docs/reference/base_application.md
+-rw-rw-rw-   0        0        0      682 2022-07-30 03:40:50.000000 qtstrap-0.5.0/docs/reference/base_window.md
+-rw-rw-rw-   0        0        0      653 2022-07-30 03:40:50.000000 qtstrap-0.5.0/docs/reference/options.md
+-rw-rw-rw-   0        0        0      287 2022-07-30 03:40:50.000000 qtstrap-0.5.0/docs/reference/settings.md
+-rw-rw-rw-   0        0        0      962 2022-07-30 03:40:50.000000 qtstrap-0.5.0/docs/reference/toolbar.md
+-rw-rw-rw-   0        0        0     1484 2022-07-30 03:40:50.000000 qtstrap-0.5.0/docs/reference/utils.adapter.md
+-rw-rw-rw-   0        0        0       88 2022-07-30 03:40:50.000000 qtstrap-0.5.0/docs/reference/utils.decorators.md
+-rw-rw-rw-   0        0        0      618 2022-07-30 03:40:50.000000 qtstrap-0.5.0/docs/reference/utils.defer.md
+-rw-rw-rw-   0        0        0      353 2022-07-30 03:40:50.000000 qtstrap-0.5.0/docs/reference/utils.md
+-rw-rw-rw-   0        0        0      576 2022-07-30 03:40:50.000000 qtstrap-0.5.0/docs/reference/utils.signals.md
+-rw-rw-rw-   0        0        0      105 2022-07-30 03:40:50.000000 qtstrap-0.5.0/docs/reference/utils.singleton.md
+-rw-rw-rw-   0        0        0      690 2022-07-30 03:40:50.000000 qtstrap-0.5.0/docs/reference/utils.timestamp.md
+-rw-rw-rw-   0        0        0     1349 2022-07-30 03:40:50.000000 qtstrap-0.5.0/docs/reference/utils.utils.md
+-rw-rw-rw-   0        0        0     2361 2022-07-30 03:40:50.000000 qtstrap-0.5.0/docs/reference/widgets.buttons.md
+-rw-rw-rw-   0        0        0     1196 2022-07-30 03:40:50.000000 qtstrap-0.5.0/docs/reference/widgets.labeledit.md
+-rw-rw-rw-   0        0        0     4766 2022-07-30 03:40:51.000000 qtstrap-0.5.0/docs/reference/widgets.layouts.md
+-rw-rw-rw-   0        0        0      516 2022-07-30 03:40:51.000000 qtstrap-0.5.0/docs/reference/widgets.line_widgets.md
+-rw-rw-rw-   0        0        0      638 2022-07-30 03:40:51.000000 qtstrap-0.5.0/docs/reference/widgets.link_label.md
+-rw-rw-rw-   0        0        0     1408 2022-07-30 03:40:50.000000 qtstrap-0.5.0/docs/reference/widgets.md
+-rw-rw-rw-   0        0        0     1324 2022-07-30 03:40:51.000000 qtstrap-0.5.0/docs/reference/widgets.persistent_tab_widget.md
+-rw-rw-rw-   0        0        0     3704 2022-07-30 03:40:51.000000 qtstrap-0.5.0/docs/reference/widgets.persistent_widgets.md
+-rw-rw-rw-   0        0        0     2949 2021-04-01 21:16:04.000000 qtstrap-0.5.0/docs/screenshot1.png
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:51.243019 qtstrap-0.5.0/docs/structure/
+-rw-rw-rw-   0        0        0     1193 2021-04-01 21:16:04.000000 qtstrap-0.5.0/docs/structure/makefile.md
+-rw-rw-rw-   0        0        0     3013 2022-07-30 00:37:45.000000 qtstrap-0.5.0/docs/structure/structure.md
+-rw-rw-rw-   0        0        0     7886 2022-07-30 03:01:48.000000 qtstrap-0.5.0/docs/test.md
+-rw-rw-rw-   0        0        0      987 2023-03-27 08:50:48.000000 qtstrap-0.5.0/mkdocs.yml
+-rw-rw-rw-   0        0        0      345 2022-07-30 04:03:13.000000 qtstrap-0.5.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:51.263022 qtstrap-0.5.0/qtstrap/
+-rw-rw-rw-   0        0        0     1103 2023-05-25 09:28:50.000000 qtstrap-0.5.0/qtstrap/__init__.py
+-rw-rw-rw-   0        0        0     1901 2023-03-27 08:38:01.000000 qtstrap-0.5.0/qtstrap/__main__.py
+-rw-rw-rw-   0        0        0     2051 2023-03-07 12:17:44.000000 qtstrap-0.5.0/qtstrap/base_application.py
+-rw-rw-rw-   0        0        0     2074 2023-03-07 12:38:24.000000 qtstrap-0.5.0/qtstrap/base_window.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:51.325516 qtstrap-0.5.0/qtstrap/experimental/
+-rw-rw-rw-   0        0        0        0 2023-04-03 00:57:28.000000 qtstrap-0.5.0/qtstrap/experimental/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:51.328017 qtstrap-0.5.0/qtstrap/extras/
+-rw-rw-rw-   0        0        0        0 2021-04-08 13:05:51.000000 qtstrap-0.5.0/qtstrap/extras/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:51.383519 qtstrap-0.5.0/qtstrap/extras/code_editor/
+-rw-rw-rw-   0        0        0      113 2022-05-01 01:28:19.000000 qtstrap-0.5.0/qtstrap/extras/code_editor/__init__.py
+-rw-rw-rw-   0        0        0    12535 2023-03-27 09:14:21.000000 qtstrap-0.5.0/qtstrap/extras/code_editor/code_editor.py
+-rw-rw-rw-   0        0        0      847 2022-12-10 23:54:46.000000 qtstrap-0.5.0/qtstrap/extras/code_editor/code_line.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:51.408017 qtstrap-0.5.0/qtstrap/extras/code_editor/highlighters/
+-rw-rw-rw-   0        0        0       37 2021-04-25 18:57:56.000000 qtstrap-0.5.0/qtstrap/extras/code_editor/highlighters/__init__.py
+-rw-rw-rw-   0        0        0     6354 2023-03-07 12:26:48.000000 qtstrap-0.5.0/qtstrap/extras/code_editor/highlighters/python.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:51.445518 qtstrap-0.5.0/qtstrap/extras/command_palette/
+-rw-rw-rw-   0        0        0       52 2021-07-23 15:36:03.000000 qtstrap-0.5.0/qtstrap/extras/command_palette/__init__.py
+-rw-rw-rw-   0        0        0    11678 2023-03-27 09:27:44.000000 qtstrap-0.5.0/qtstrap/extras/command_palette/command_palette.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:51.456517 qtstrap-0.5.0/qtstrap/extras/log_monitor/
+-rw-rw-rw-   0        0        0     1124 2022-12-23 00:25:27.000000 qtstrap-0.5.0/qtstrap/extras/log_monitor/__init__.py
+-rw-rw-rw-   0        0        0     2437 2022-12-23 00:25:31.000000 qtstrap-0.5.0/qtstrap/extras/log_monitor/log_database_handler.py
+-rw-rw-rw-   0        0        0    16819 2023-04-29 15:39:56.000000 qtstrap-0.5.0/qtstrap/extras/log_monitor/log_filter_controls.py
+-rw-rw-rw-   0        0        0     4165 2022-12-22 21:39:18.000000 qtstrap-0.5.0/qtstrap/extras/log_monitor/log_profile.py
+-rw-rw-rw-   0        0        0     3935 2023-04-29 15:35:41.000000 qtstrap-0.5.0/qtstrap/extras/log_monitor/log_table_view.py
+-rw-rw-rw-   0        0        0     4710 2023-03-03 07:38:29.000000 qtstrap-0.5.0/qtstrap/extras/log_monitor/log_widget.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:51.475520 qtstrap-0.5.0/qtstrap/extras/style/
+-rw-rw-rw-   0        0        0      129 2023-03-03 07:24:23.000000 qtstrap-0.5.0/qtstrap/extras/style/__init__.py
+-rw-rw-rw-   0        0        0     1085 2023-01-12 03:06:47.000000 qtstrap-0.5.0/qtstrap/extras/style/colors.py
+-rw-rw-rw-   0        0        0     2040 2023-03-03 07:24:23.000000 qtstrap-0.5.0/qtstrap/extras/style/dark_palette.py
+-rw-rw-rw-   0        0        0     4105 2023-03-07 12:55:24.000000 qtstrap-0.5.0/qtstrap/extras/style/themes.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:51.479020 qtstrap-0.5.0/qtstrap/optional/
+-rw-rw-rw-   0        0        0        0 2023-04-03 00:57:38.000000 qtstrap-0.5.0/qtstrap/optional/__init__.py
+-rw-rw-rw-   0        0        0     1174 2022-12-10 01:10:44.000000 qtstrap-0.5.0/qtstrap/options.py
+-rw-rw-rw-   0        0        0      694 2023-03-27 08:40:17.000000 qtstrap-0.5.0/qtstrap/qt.py
+-rw-rw-rw-   0        0        0      504 2023-05-25 09:28:21.000000 qtstrap-0.5.0/qtstrap/settings.py
+-rw-rw-rw-   0        0        0      860 2023-05-25 09:58:36.000000 qtstrap-0.5.0/qtstrap/settings_model.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:51.485019 qtstrap-0.5.0/qtstrap/template/
+-rw-rw-rw-   0        0        0     3629 2022-07-30 00:00:03.000000 qtstrap-0.5.0/qtstrap/template/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:51.487018 qtstrap-0.5.0/qtstrap/template/app/
+-rw-rw-rw-   0        0        0      953 2021-04-02 17:24:51.000000 qtstrap-0.5.0/qtstrap/template/app/main.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:51.490018 qtstrap-0.5.0/qtstrap/template/app/resources/
+-rw-rw-rw-   0        0        0    59285 2021-04-01 21:16:04.000000 qtstrap-0.5.0/qtstrap/template/app/resources/application.ico
+-rw-rw-rw-   0        0        0     5523 2021-04-01 21:16:04.000000 qtstrap-0.5.0/qtstrap/template/app/resources/icon.svg
+-rw-rw-rw-   0        0        0     1195 2022-09-11 05:33:04.000000 qtstrap-0.5.0/qtstrap/template/bundle.spec
+-rw-rw-rw-   0        0        0     2450 2022-07-29 23:52:21.000000 qtstrap-0.5.0/qtstrap/template/installer.iss
+-rw-rw-rw-   0        0        0        0 2021-04-01 21:16:04.000000 qtstrap-0.5.0/qtstrap/template/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:51.520517 qtstrap-0.5.0/qtstrap/utils/
+-rw-rw-rw-   0        0        0      390 2022-12-08 21:10:40.000000 qtstrap-0.5.0/qtstrap/utils/__init__.py
+-rw-rw-rw-   0        0        0     2469 2023-03-26 02:15:24.000000 qtstrap-0.5.0/qtstrap/utils/adapter.py
+-rw-rw-rw-   0        0        0      265 2022-10-20 22:39:10.000000 qtstrap-0.5.0/qtstrap/utils/call_later.py
+-rw-rw-rw-   0        0        0      652 2021-05-13 17:33:19.000000 qtstrap-0.5.0/qtstrap/utils/defer.py
+-rw-rw-rw-   0        0        0     2800 2022-12-12 00:29:52.000000 qtstrap-0.5.0/qtstrap/utils/drag_and_drop.py
+-rw-rw-rw-   0        0        0      629 2022-11-03 16:33:13.000000 qtstrap-0.5.0/qtstrap/utils/get_ip.py
+-rw-rw-rw-   0        0        0      378 2023-02-04 21:57:48.000000 qtstrap-0.5.0/qtstrap/utils/signals.py
+-rw-rw-rw-   0        0        0      255 2022-11-03 16:23:26.000000 qtstrap-0.5.0/qtstrap/utils/singleton.py
+-rw-rw-rw-   0        0        0      751 2023-02-04 22:01:45.000000 qtstrap-0.5.0/qtstrap/utils/string_builder.py
+-rw-rw-rw-   0        0        0      531 2021-10-30 07:31:06.000000 qtstrap-0.5.0/qtstrap/utils/timestamp.py
+-rw-rw-rw-   0        0        0      291 2022-12-11 02:07:30.000000 qtstrap-0.5.0/qtstrap/utils/trace.py
+-rw-rw-rw-   0        0        0     2491 2022-11-03 16:16:04.000000 qtstrap-0.5.0/qtstrap/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:51.538519 qtstrap-0.5.0/qtstrap/widgets/
+-rw-rw-rw-   0        0        0      890 2023-02-23 14:40:05.000000 qtstrap-0.5.0/qtstrap/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2973 2022-12-09 06:51:34.000000 qtstrap-0.5.0/qtstrap/widgets/buttons.py
+-rw-rw-rw-   0        0        0     1590 2022-05-15 05:13:52.000000 qtstrap-0.5.0/qtstrap/widgets/labeledit.py
+-rw-rw-rw-   0        0        0     8757 2023-05-25 07:31:41.000000 qtstrap-0.5.0/qtstrap/widgets/layouts.py
+-rw-rw-rw-   0        0        0      665 2021-04-01 21:16:04.000000 qtstrap-0.5.0/qtstrap/widgets/line_widgets.py
+-rw-rw-rw-   0        0        0      824 2022-10-26 07:40:04.000000 qtstrap-0.5.0/qtstrap/widgets/link_label.py
+-rw-rw-rw-   0        0        0     3161 2021-05-06 02:08:19.000000 qtstrap-0.5.0/qtstrap/widgets/persistent_tab_widget.py
+-rw-rw-rw-   0        0        0     5473 2022-11-10 17:33:23.000000 qtstrap-0.5.0/qtstrap/widgets/persistent_widgets.py
+-rw-rw-rw-   0        0        0     7568 2023-03-03 08:21:01.000000 qtstrap-0.5.0/qtstrap/widgets/toggle.py
+-rw-rw-rw-   0        0        0      910 2022-11-07 02:00:59.000000 qtstrap-0.5.0/qtstrap/widgets/toolbar.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:51.324017 qtstrap-0.5.0/qtstrap.egg-info/
+-rw-rw-rw-   0        0        0     3396 2023-05-25 10:53:50.000000 qtstrap-0.5.0/qtstrap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4934 2023-05-25 10:53:50.000000 qtstrap-0.5.0/qtstrap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 10:53:50.000000 qtstrap-0.5.0/qtstrap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-25 10:53:50.000000 qtstrap-0.5.0/qtstrap.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-12-23 00:34:54.000000 qtstrap-0.5.0/qtstrap.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       61 2023-05-25 10:53:50.000000 qtstrap-0.5.0/qtstrap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 10:53:50.000000 qtstrap-0.5.0/qtstrap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1141 2022-11-30 17:51:25.000000 qtstrap-0.5.0/requirements.txt
+-rw-rw-rw-   0        0        0      529 2022-10-26 06:20:37.000000 qtstrap-0.5.0/requirements_build.txt
+-rw-rw-rw-   0        0        0      520 2022-10-26 06:55:20.000000 qtstrap-0.5.0/requirements_test.txt
+-rw-rw-rw-   0        0        0      158 2022-11-24 06:15:10.000000 qtstrap-0.5.0/run_tox_tests.py
+-rw-rw-rw-   0        0        0     1265 2023-05-25 10:53:51.552517 qtstrap-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0       96 2022-07-30 01:23:30.000000 qtstrap-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:51.546519 qtstrap-0.5.0/test/
+-rw-rw-rw-   0        0        0      876 2021-04-01 21:16:04.000000 qtstrap-0.5.0/test/test_base_app.py
+-rw-rw-rw-   0        0        0     1073 2021-04-01 21:16:04.000000 qtstrap-0.5.0/test/test_base_window.py
+-rw-rw-rw-   0        0        0      616 2022-11-24 06:02:31.000000 qtstrap-0.5.0/test/test_layouts.py
+-rw-rw-rw-   0        0        0     2689 2022-11-24 05:29:55.000000 qtstrap-0.5.0/test/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:53:51.548519 qtstrap-0.5.0/test/utils/
+-rw-rw-rw-   0        0        0      230 2022-11-24 04:25:54.000000 qtstrap-0.5.0/test/utils/test_defer.py
+-rw-rw-rw-   0        0        0      348 2022-11-30 16:27:29.000000 qtstrap-0.5.0/tox.ini
```

### Comparing `qtstrap-0.4.2/.github/FUNDING.yml` & `qtstrap-0.5.0/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/.github/workflows/main.yml` & `qtstrap-0.5.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/LICENSE` & `qtstrap-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/Makefile` & `qtstrap-0.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/PKG-INFO` & `qtstrap-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtstrap
-Version: 0.4.2
+Version: 0.5.0
 Summary: Like Bootstrap, but qt-er.
 Home-page: https://github.com/qtstrap/qtstrap
 Author: David Kincaid
 Author-email: dlkincaid0@gmail.com
 License: MIT
 Project-URL: Documentation, https://qtstrap.github.io/qtstrap/
 Project-URL: Source, https://github.com/qtstrap/qtstrap
```

### Comparing `qtstrap-0.4.2/README.md` & `qtstrap-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/extras.code_editor.code_editor.md` & `qtstrap-0.5.0/docs/api/extras.code_editor.code_editor.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/extras.code_editor.code_line.md` & `qtstrap-0.5.0/docs/api/extras.code_editor.code_line.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/extras.code_editor.highlighters.python.md` & `qtstrap-0.5.0/docs/api/extras.code_editor.highlighters.python.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/extras.command_palette.command_palette.md` & `qtstrap-0.5.0/docs/api/extras.command_palette.command_palette.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/extras.log_monitor.log_database_handler.md` & `qtstrap-0.5.0/docs/api/extras.log_monitor.log_database_handler.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/extras.log_monitor.log_filter_controls.md` & `qtstrap-0.5.0/docs/api/extras.log_monitor.log_filter_controls.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/extras.log_monitor.log_profile.md` & `qtstrap-0.5.0/docs/api/extras.log_monitor.log_profile.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/extras.log_monitor.log_table_view.md` & `qtstrap-0.5.0/docs/api/extras.log_monitor.log_table_view.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/extras.log_monitor.log_widget.md` & `qtstrap-0.5.0/docs/api/extras.log_monitor.log_widget.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/extras.log_monitor.md` & `qtstrap-0.5.0/docs/api/extras.log_monitor.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/extras.style.colors.md` & `qtstrap-0.5.0/docs/api/extras.style.colors.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/extras.style.dark_palette.md` & `qtstrap-0.5.0/docs/api/extras.style.dark_palette.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/extras.style.themes.md` & `qtstrap-0.5.0/docs/api/extras.style.themes.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/options.md` & `qtstrap-0.5.0/docs/api/options.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/overview.md` & `qtstrap-0.5.0/docs/api/overview.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/settings.md` & `qtstrap-0.5.0/docs/api/settings.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/utils.adapter.md` & `qtstrap-0.5.0/docs/api/utils.adapter.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/utils.call_later.md` & `qtstrap-0.5.0/docs/api/utils.call_later.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/utils.decorators.md` & `qtstrap-0.5.0/docs/api/utils.decorators.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/utils.defer.md` & `qtstrap-0.5.0/docs/api/utils.defer.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/utils.drag_and_drop.md` & `qtstrap-0.5.0/docs/api/utils.drag_and_drop.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/utils.get_ip.md` & `qtstrap-0.5.0/docs/api/utils.get_ip.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/utils.signals.md` & `qtstrap-0.5.0/docs/api/utils.signals.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/utils.singleton.md` & `qtstrap-0.5.0/docs/api/utils.singleton.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/utils.string_builder.md` & `qtstrap-0.5.0/docs/api/utils.string_builder.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/utils.timestamp.md` & `qtstrap-0.5.0/docs/api/utils.timestamp.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/utils.trace.md` & `qtstrap-0.5.0/docs/api/utils.trace.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/utils.utils.md` & `qtstrap-0.5.0/docs/api/utils.utils.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/widgets.buttons.md` & `qtstrap-0.5.0/docs/api/widgets.buttons.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/widgets.labeledit.md` & `qtstrap-0.5.0/docs/api/widgets.labeledit.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/widgets.layouts.md` & `qtstrap-0.5.0/docs/api/widgets.layouts.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/widgets.line_widgets.md` & `qtstrap-0.5.0/docs/api/widgets.line_widgets.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/widgets.link_label.md` & `qtstrap-0.5.0/docs/api/widgets.link_label.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/widgets.md` & `qtstrap-0.5.0/docs/api/widgets.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/widgets.persistent_tab_widget.md` & `qtstrap-0.5.0/docs/api/widgets.persistent_tab_widget.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/widgets.persistent_widgets.md` & `qtstrap-0.5.0/docs/api/widgets.persistent_widgets.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/widgets.toggle.md` & `qtstrap-0.5.0/docs/api/widgets.toggle.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/api/widgets.toolbar.md` & `qtstrap-0.5.0/docs/api/widgets.toolbar.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/extras/code_editor.md` & `qtstrap-0.5.0/docs/extras/code_editor.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/extras/command_palette.md` & `qtstrap-0.5.0/docs/extras/command_palette.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/extras/log_monitor.md` & `qtstrap-0.5.0/docs/extras/log_monitor.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/index.md` & `qtstrap-0.5.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/quickstart/baseapplication.md` & `qtstrap-0.5.0/docs/quickstart/baseapplication.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/quickstart/basemainwindow.md` & `qtstrap-0.5.0/docs/quickstart/basemainwindow.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/quickstart/context_layouts.md` & `qtstrap-0.5.0/docs/quickstart/context_layouts.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/quickstart/gettingstarted.md` & `qtstrap-0.5.0/docs/quickstart/gettingstarted.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/quickstart/installation.md` & `qtstrap-0.5.0/docs/quickstart/installation.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/reference/base_application.md` & `qtstrap-0.5.0/docs/reference/base_application.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/reference/base_window.md` & `qtstrap-0.5.0/docs/reference/base_window.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/reference/options.md` & `qtstrap-0.5.0/docs/reference/options.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/reference/toolbar.md` & `qtstrap-0.5.0/docs/reference/toolbar.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/reference/utils.adapter.md` & `qtstrap-0.5.0/docs/reference/utils.adapter.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/reference/utils.defer.md` & `qtstrap-0.5.0/docs/reference/utils.defer.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/reference/utils.signals.md` & `qtstrap-0.5.0/docs/reference/utils.signals.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/reference/utils.timestamp.md` & `qtstrap-0.5.0/docs/reference/utils.timestamp.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/reference/utils.utils.md` & `qtstrap-0.5.0/docs/reference/utils.utils.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/reference/widgets.buttons.md` & `qtstrap-0.5.0/docs/reference/widgets.buttons.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/reference/widgets.labeledit.md` & `qtstrap-0.5.0/docs/reference/widgets.labeledit.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/reference/widgets.layouts.md` & `qtstrap-0.5.0/docs/reference/widgets.layouts.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/reference/widgets.line_widgets.md` & `qtstrap-0.5.0/docs/reference/widgets.line_widgets.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/reference/widgets.link_label.md` & `qtstrap-0.5.0/docs/reference/widgets.link_label.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/reference/widgets.md` & `qtstrap-0.5.0/docs/reference/widgets.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/reference/widgets.persistent_tab_widget.md` & `qtstrap-0.5.0/docs/reference/widgets.persistent_tab_widget.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/reference/widgets.persistent_widgets.md` & `qtstrap-0.5.0/docs/reference/widgets.persistent_widgets.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/screenshot1.png` & `qtstrap-0.5.0/docs/screenshot1.png`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/structure/makefile.md` & `qtstrap-0.5.0/docs/structure/makefile.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/structure/structure.md` & `qtstrap-0.5.0/docs/structure/structure.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/docs/test.md` & `qtstrap-0.5.0/docs/test.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/mkdocs.yml` & `qtstrap-0.5.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/__init__.py` & `qtstrap-0.5.0/qtstrap/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,20 +17,22 @@
     try:
         from .qt import *
     except ModuleNotFoundError as e:
         raise ModuleNotFoundError(
             'No Qt Bindings found. Try "pip install PySide6" or "pip install PySide6"'
         ) from e
     else:
-        from .settings import *
+        from .settings import PortableSettings
         
         if OPTIONS.portable:
             from .settings import PortableSettings as QSettings
             QSettings._install()
 
+        from .settings_model import SettingsModel
+
         from .utils import *
         from .widgets import *
         from .base_application import (
             BaseApplication,
             install_app_info,
             install_ctrlc_handler,
         )
```

### Comparing `qtstrap-0.4.2/qtstrap/__main__.py` & `qtstrap-0.5.0/qtstrap/__main__.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/base_application.py` & `qtstrap-0.5.0/qtstrap/base_application.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/base_window.py` & `qtstrap-0.5.0/qtstrap/base_window.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/extras/code_editor/code_editor.py` & `qtstrap-0.5.0/qtstrap/extras/code_editor/code_editor.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/extras/code_editor/code_line.py` & `qtstrap-0.5.0/qtstrap/extras/code_editor/code_line.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/extras/code_editor/highlighters/python.py` & `qtstrap-0.5.0/qtstrap/extras/code_editor/highlighters/python.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/extras/command_palette/command_palette.py` & `qtstrap-0.5.0/qtstrap/extras/command_palette/command_palette.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/extras/log_monitor/__init__.py` & `qtstrap-0.5.0/qtstrap/extras/log_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/extras/log_monitor/log_database_handler.py` & `qtstrap-0.5.0/qtstrap/extras/log_monitor/log_database_handler.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/extras/log_monitor/log_filter_controls.py` & `qtstrap-0.5.0/qtstrap/extras/log_monitor/log_filter_controls.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/extras/log_monitor/log_profile.py` & `qtstrap-0.5.0/qtstrap/extras/log_monitor/log_profile.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/extras/log_monitor/log_table_view.py` & `qtstrap-0.5.0/qtstrap/extras/log_monitor/log_table_view.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/extras/log_monitor/log_widget.py` & `qtstrap-0.5.0/qtstrap/extras/log_monitor/log_widget.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/extras/style/colors.py` & `qtstrap-0.5.0/qtstrap/extras/style/colors.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/extras/style/dark_palette.py` & `qtstrap-0.5.0/qtstrap/extras/style/dark_palette.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/extras/style/themes.py` & `qtstrap-0.5.0/qtstrap/extras/style/themes.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/options.py` & `qtstrap-0.5.0/qtstrap/options.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/qt.py` & `qtstrap-0.5.0/qtstrap/qt.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/template/Makefile` & `qtstrap-0.5.0/qtstrap/template/Makefile`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/template/app/main.py` & `qtstrap-0.5.0/qtstrap/template/app/main.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/template/app/resources/application.ico` & `qtstrap-0.5.0/qtstrap/template/app/resources/application.ico`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/template/app/resources/icon.svg` & `qtstrap-0.5.0/qtstrap/template/app/resources/icon.svg`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/template/bundle.spec` & `qtstrap-0.5.0/qtstrap/template/bundle.spec`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/template/installer.iss` & `qtstrap-0.5.0/qtstrap/template/installer.iss`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/utils/adapter.py` & `qtstrap-0.5.0/qtstrap/utils/adapter.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/utils/defer.py` & `qtstrap-0.5.0/qtstrap/utils/defer.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/utils/drag_and_drop.py` & `qtstrap-0.5.0/qtstrap/utils/drag_and_drop.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/utils/get_ip.py` & `qtstrap-0.5.0/qtstrap/utils/get_ip.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/utils/string_builder.py` & `qtstrap-0.5.0/qtstrap/utils/string_builder.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/utils/timestamp.py` & `qtstrap-0.5.0/qtstrap/utils/timestamp.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/utils/utils.py` & `qtstrap-0.5.0/qtstrap/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/widgets/__init__.py` & `qtstrap-0.5.0/qtstrap/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/widgets/buttons.py` & `qtstrap-0.5.0/qtstrap/widgets/buttons.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/widgets/labeledit.py` & `qtstrap-0.5.0/qtstrap/widgets/labeledit.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/widgets/layouts.py` & `qtstrap-0.5.0/qtstrap/widgets/layouts.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,21 +145,24 @@
 class CSplitter(QSplitter):
     def __init__(self, parent=None, margins=None, orientation=None, **kwargs):
         if orientation in orientations:
             orientation = orientations[orientation]
 
         if isinstance(parent, QWidget):
             super().__init__(parent, orientation, **kwargs)
-            CHBoxLayout(parent).add(self)
+            CHBoxLayout(parent, margins=margins).add(self)
         elif isinstance(parent, QLayout):
             super().__init__(orientation, **kwargs)
             parent.add(self)
 
-        if margins:
-            self.setContentsMargins(*margins)
+        if margins is not None:
+            if isinstance(margins, tuple):
+                self.setContentsMargins(*margins)
+            elif isinstance(margins, int):
+                self.setContentsMargins(margins, margins, margins, margins)
 
         if orientation:
             self.setOrientation(orientation)
 
     def __iadd__(self, item):
         self.add(item)
         return self
```

### Comparing `qtstrap-0.4.2/qtstrap/widgets/line_widgets.py` & `qtstrap-0.5.0/qtstrap/widgets/line_widgets.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/widgets/link_label.py` & `qtstrap-0.5.0/qtstrap/widgets/link_label.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/widgets/persistent_tab_widget.py` & `qtstrap-0.5.0/qtstrap/widgets/persistent_tab_widget.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/widgets/persistent_widgets.py` & `qtstrap-0.5.0/qtstrap/widgets/persistent_widgets.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/widgets/toggle.py` & `qtstrap-0.5.0/qtstrap/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap/widgets/toolbar.py` & `qtstrap-0.5.0/qtstrap/widgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/qtstrap.egg-info/PKG-INFO` & `qtstrap-0.5.0/qtstrap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtstrap
-Version: 0.4.2
+Version: 0.5.0
 Summary: Like Bootstrap, but qt-er.
 Home-page: https://github.com/qtstrap/qtstrap
 Author: David Kincaid
 Author-email: dlkincaid0@gmail.com
 License: MIT
 Project-URL: Documentation, https://qtstrap.github.io/qtstrap/
 Project-URL: Source, https://github.com/qtstrap/qtstrap
```

### Comparing `qtstrap-0.4.2/qtstrap.egg-info/SOURCES.txt` & `qtstrap-0.5.0/qtstrap.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 qtstrap/__init__.py
 qtstrap/__main__.py
 qtstrap/base_application.py
 qtstrap/base_window.py
 qtstrap/options.py
 qtstrap/qt.py
 qtstrap/settings.py
+qtstrap/settings_model.py
 qtstrap.egg-info/PKG-INFO
 qtstrap.egg-info/SOURCES.txt
 qtstrap.egg-info/dependency_links.txt
 qtstrap.egg-info/entry_points.txt
 qtstrap.egg-info/not-zip-safe
 qtstrap.egg-info/requires.txt
 qtstrap.egg-info/top_level.txt
```

### Comparing `qtstrap-0.4.2/requirements.txt` & `qtstrap-0.5.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/requirements_build.txt` & `qtstrap-0.5.0/requirements_build.txt`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/requirements_test.txt` & `qtstrap-0.5.0/requirements_test.txt`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/setup.cfg` & `qtstrap-0.5.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2071 7473 7472 6170 0d0a 7665 7273   = qtstrap..vers
-00000020: 696f 6e20 3d20 302e 342e 320d 0a64 6573  ion = 0.4.2..des
+00000020: 696f 6e20 3d20 302e 352e 300d 0a64 6573  ion = 0.5.0..des
 00000030: 6372 6970 7469 6f6e 203d 204c 696b 6520  cription = Like 
 00000040: 426f 6f74 7374 7261 702c 2062 7574 2071  Bootstrap, but q
 00000050: 742d 6572 2e0d 0a6c 6f6e 675f 6465 7363  t-er...long_desc
 00000060: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000070: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
 00000080: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
 00000090: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
@@ -55,25 +55,26 @@
 00000360: 730d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  s....[options]..
 00000370: 7a69 705f 7361 6665 203d 2046 616c 7365  zip_safe = False
 00000380: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
 00000390: 643a 0d0a 706c 6174 666f 726d 7320 3d20  d:..platforms = 
 000003a0: 616e 790d 0a69 6e63 6c75 6465 5f70 6163  any..include_pac
 000003b0: 6b61 6765 5f64 6174 6120 3d20 7472 7565  kage_data = true
 000003c0: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
-000003d0: 6573 203d 200d 0a09 5174 5079 0d0a 0963  es = ...QtPy...c
-000003e0: 6c69 636b 0d0a 0969 6e71 7569 7265 7270  lick...inquirerp
-000003f0: 790d 0a09 6170 7064 6972 730d 0a09 7174  y...appdirs...qt
-00000400: 6177 6573 6f6d 650d 0a09 7079 696e 7374  awesome...pyinst
-00000410: 616c 6c65 720d 0a70 7974 686f 6e5f 7265  aller..python_re
-00000420: 7175 6972 6573 203d 203e 3d33 2e38 0d0a  quires = >=3.8..
-00000430: 0d0a 5b62 6469 7374 5f77 6865 656c 5d0d  ..[bdist_wheel].
-00000440: 0a75 6e69 7665 7273 616c 203d 2031 0d0a  .universal = 1..
-00000450: 0d0a 5b61 6c69 6173 6573 5d0d 0a74 6573  ..[aliases]..tes
-00000460: 7420 3d20 7079 7465 7374 0d0a 0d0a 5b6f  t = pytest....[o
-00000470: 7074 696f 6e73 2e65 6e74 7279 5f70 6f69  ptions.entry_poi
-00000480: 6e74 735d 0d0a 636f 6e73 6f6c 655f 7363  nts]..console_sc
-00000490: 7269 7074 7320 3d20 0d0a 0971 7473 7472  ripts = ...qtstr
-000004a0: 6170 3d71 7473 7472 6170 2e5f 5f6d 6169  ap=qtstrap.__mai
-000004b0: 6e5f 5f3a 6d61 696e 0d0a 0d0a 5b65 6767  n__:main....[egg
-000004c0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-000004d0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-000004e0: 2030 0d0a 0d0a                            0....
+000003d0: 6573 203d 200d 0a09 5174 5079 0d0a 0970  es = ...QtPy...p
+000003e0: 7964 616e 7469 630d 0a09 636c 6963 6b0d  ydantic...click.
+000003f0: 0a09 696e 7175 6972 6572 7079 0d0a 0961  ..inquirerpy...a
+00000400: 7070 6469 7273 0d0a 0971 7461 7765 736f  ppdirs...qtaweso
+00000410: 6d65 0d0a 0970 7969 6e73 7461 6c6c 6572  me...pyinstaller
+00000420: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
+00000430: 7320 3d20 3e3d 332e 380d 0a0d 0a5b 6264  s = >=3.8....[bd
+00000440: 6973 745f 7768 6565 6c5d 0d0a 756e 6976  ist_wheel]..univ
+00000450: 6572 7361 6c20 3d20 310d 0a0d 0a5b 616c  ersal = 1....[al
+00000460: 6961 7365 735d 0d0a 7465 7374 203d 2070  iases]..test = p
+00000470: 7974 6573 740d 0a0d 0a5b 6f70 7469 6f6e  ytest....[option
+00000480: 732e 656e 7472 795f 706f 696e 7473 5d0d  s.entry_points].
+00000490: 0a63 6f6e 736f 6c65 5f73 6372 6970 7473  .console_scripts
+000004a0: 203d 200d 0a09 7174 7374 7261 703d 7174   = ...qtstrap=qt
+000004b0: 7374 7261 702e 5f5f 6d61 696e 5f5f 3a6d  strap.__main__:m
+000004c0: 6169 6e0d 0a0d 0a5b 6567 675f 696e 666f  ain....[egg_info
+000004d0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+000004e0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+000004f0: 0a                                       .
```

### Comparing `qtstrap-0.4.2/test/test_base_app.py` & `qtstrap-0.5.0/test/test_base_app.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/test/test_base_window.py` & `qtstrap-0.5.0/test/test_base_window.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/test/test_layouts.py` & `qtstrap-0.5.0/test/test_layouts.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.2/test/test_utils.py` & `qtstrap-0.5.0/test/test_utils.py`

 * *Files identical despite different names*

