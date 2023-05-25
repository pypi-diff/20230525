# Comparing `tmp/scipion-pyworkflow-3.0.8.tar.gz` & `tmp/scipion-pyworkflow-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scipion-pyworkflow-3.0.8.tar", last modified: Fri Dec 11 16:07:30 2020, max compression
+gzip compressed data, was "scipion-pyworkflow-3.0.9.tar", last modified: Mon Feb  1 09:45:05 2021, max compression
```

## Comparing `scipion-pyworkflow-3.0.8.tar` & `scipion-pyworkflow-3.0.9.tar`

### file list

```diff
@@ -1,270 +1,270 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2020-12-11 16:07:30.890427 scipion-pyworkflow-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35148 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      251 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4022 2020-12-11 16:07:30.890427 scipion-pyworkflow-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2243 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2020-12-11 16:07:30.862426 scipion-pyworkflow-3.0.8/pyworkflow/
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2020-12-11 16:07:30.866426 scipion-pyworkflow-3.0.8/pyworkflow/apps/
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1356 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1829 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     3055 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_project.py
--rw-r--r--   0 runner    (1001) docker     (121)     5368 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_protocol_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1952 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_protocol_mpirun.py
--rw-r--r--   0 runner    (1001) docker     (121)     2707 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_protocol_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_protocol_run.py
--rw-r--r--   0 runner    (1001) docker     (121)    11868 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_run_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     9040 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_schedule_run.py
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_sleep.py
--rw-r--r--   0 runner    (1001) docker     (121)    16530 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_sync_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2595 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_viewer.py
--rw-r--r--   0 runner    (1001) docker     (121)     8393 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     4464 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      507 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2020-12-11 16:07:30.866426 scipion-pyworkflow-3.0.8/pyworkflow/gui/
--rw-r--r--   0 runner    (1001) docker     (121)     1351 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23402 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/browser.py
--rw-r--r--   0 runner    (1001) docker     (121)    36994 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/canvas.py
--rw-r--r--   0 runner    (1001) docker     (121)    27922 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/dialog.py
--rw-r--r--   0 runner    (1001) docker     (121)   106438 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/form.py
--rw-r--r--   0 runner    (1001) docker     (121)     8810 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     9856 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/graph_layout.py
--rw-r--r--   0 runner    (1001) docker     (121)    16949 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (121)     7086 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/matplotlib_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     8116 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2020-12-11 16:07:30.866426 scipion-pyworkflow-3.0.8/pyworkflow/gui/project/
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7694 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/project/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/project/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     7251 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/project/labels.py
--rw-r--r--   0 runner    (1001) docker     (121)    18168 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/project/project.py
--rw-r--r--   0 runner    (1001) docker     (121)     3057 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/project/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    19468 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/project/viewdata.py
--rw-r--r--   0 runner    (1001) docker     (121)    21347 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/project/viewprojects.py
--rw-r--r--   0 runner    (1001) docker     (121)   109042 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/project/viewprotocols.py
--rw-r--r--   0 runner    (1001) docker     (121)    27645 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/text.py
--rw-r--r--   0 runner    (1001) docker     (121)     8531 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/tooltip.py
--rw-r--r--   0 runner    (1001) docker     (121)    22023 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/tree.py
--rw-r--r--   0 runner    (1001) docker     (121)    10761 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/gui/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2020-12-11 16:07:30.866426 scipion-pyworkflow-3.0.8/pyworkflow/mapper/
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7354 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/mapper/mapper.py
--rw-r--r--   0 runner    (1001) docker     (121)    54781 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/mapper/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (121)     4724 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/mapper/sqlite_db.py
--rw-r--r--   0 runner    (1001) docker     (121)    10720 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/mapper/xmlmapper.py
--rw-r--r--   0 runner    (1001) docker     (121)    48759 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/object.py
--rw-r--r--   0 runner    (1001) docker     (121)    25158 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2020-12-11 16:07:30.866426 scipion-pyworkflow-3.0.8/pyworkflow/project/
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11818 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/project/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     6706 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/project/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    67249 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/project/project.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2020-12-11 16:07:30.870426 scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2580 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/clean_projects.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2921 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2488 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/create.py
--rw-r--r--   0 runner    (1001) docker     (121)     2909 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/edit_workflow.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      890 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/fix_links.py
--rw-r--r--   0 runner    (1001) docker     (121)     2685 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/load.py
--rw-r--r--   0 runner    (1001) docker     (121)     2564 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/refresh.py
--rw-r--r--   0 runner    (1001) docker     (121)     3461 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/schedule.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      901 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/stack2volume.py
--rw-r--r--   0 runner    (1001) docker     (121)     2452 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/stop.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2020-12-11 16:07:30.870426 scipion-pyworkflow-3.0.8/pyworkflow/protocol/
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/protocol/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (121)     2976 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/protocol/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    14674 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/protocol/executor.py
--rw-r--r--   0 runner    (1001) docker     (121)    11869 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/protocol/hosts.py
--rw-r--r--   0 runner    (1001) docker     (121)     9256 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/protocol/launch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1444 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/protocol/package.py
--rw-r--r--   0 runner    (1001) docker     (121)    23108 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/protocol/params.py
--rw-r--r--   0 runner    (1001) docker     (121)    85721 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/protocol/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2020-12-11 16:07:30.882427 scipion-pyworkflow-3.0.8/pyworkflow/resources/
--rw-r--r--   0 runner    (1001) docker     (121)     6187 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/ChimeraLogoSmall.gif
--rw-r--r--   0 runner    (1001) docker     (121)     6798 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/I2PC.gif
--rw-r--r--   0 runner    (1001) docker     (121)    64364 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/background_section.gif
--rw-r--r--   0 runner    (1001) docker     (121)      987 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/bookmark.gif
--rw-r--r--   0 runner    (1001) docker     (121)     3771 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/ccp4_200.gif
--rw-r--r--   0 runner    (1001) docker     (121)      161 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/class_obj.gif
--rw-r--r--   0 runner    (1001) docker     (121)    16491 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/cryoem_logo.gif
--rw-r--r--   0 runner    (1001) docker     (121)    34177 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/cryomethods_logo.gif
--rw-r--r--   0 runner    (1001) docker     (121)       99 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/debug.gif
--rw-r--r--   0 runner    (1001) docker     (121)      586 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/doc_icon.gif
--rw-r--r--   0 runner    (1001) docker     (121)      418 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/download_icon.gif
--rw-r--r--   0 runner    (1001) docker     (121)    27027 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/error_page.jpg
--rw-r--r--   0 runner    (1001) docker     (121)      103 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-arrow-left.gif
--rw-r--r--   0 runner    (1001) docker     (121)      105 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-arrow-up.gif
--rw-r--r--   0 runner    (1001) docker     (121)       83 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-ban.gif
--rw-r--r--   0 runner    (1001) docker     (121)       67 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-bars.gif
--rw-r--r--   0 runner    (1001) docker     (121)       73 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-check.gif
--rw-r--r--   0 runner    (1001) docker     (121)       72 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-checked.gif
--rw-r--r--   0 runner    (1001) docker     (121)      343 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-cog.gif
--rw-r--r--   0 runner    (1001) docker     (121)       87 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-cogs.gif
--rw-r--r--   0 runner    (1001) docker     (121)       78 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-database.gif
--rw-r--r--   0 runner    (1001) docker     (121)       92 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-delete-operation.gif
--rw-r--r--   0 runner    (1001) docker     (121)       75 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-download.gif
--rw-r--r--   0 runner    (1001) docker     (121)      257 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-exclamation-triangle_alert.gif
--rw-r--r--   0 runner    (1001) docker     (121)       77 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-external-link.gif
--rw-r--r--   0 runner    (1001) docker     (121)       78 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-eye.gif
--rw-r--r--   0 runner    (1001) docker     (121)       89 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-failure.gif
--rw-r--r--   0 runner    (1001) docker     (121)       78 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-file-o.gif
--rw-r--r--   0 runner    (1001) docker     (121)       82 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-files-o.gif
--rw-r--r--   0 runner    (1001) docker     (121)       76 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-folder-open.gif
--rw-r--r--   0 runner    (1001) docker     (121)      113 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-home.gif
--rw-r--r--   0 runner    (1001) docker     (121)       84 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-iconmoon-link.gif
--rw-r--r--   0 runner    (1001) docker     (121)      266 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-info-circle_alert.gif
--rw-r--r--   0 runner    (1001) docker     (121)       66 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-install.gif
--rw-r--r--   0 runner    (1001) docker     (121)       90 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-installed.gif
--rw-r--r--   0 runner    (1001) docker     (121)       74 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-laptop.gif
--rw-r--r--   0 runner    (1001) docker     (121)       77 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-lightbulb-o.gif
--rw-r--r--   0 runner    (1001) docker     (121)       76 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-list-ul.gif
--rw-r--r--   0 runner    (1001) docker     (121)       79 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-magic.gif
--rw-r--r--   0 runner    (1001) docker     (121)       67 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-minus-square.gif
--rw-r--r--   0 runner    (1001) docker     (121)       75 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-next.gif
--rw-r--r--   0 runner    (1001) docker     (121)       74 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-paint-brush.gif
--rw-r--r--   0 runner    (1001) docker     (121)       79 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-pencil.gif
--rw-r--r--   0 runner    (1001) docker     (121)       91 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-play-circle-o.gif
--rw-r--r--   0 runner    (1001) docker     (121)      110 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-plus-circle.gif
--rw-r--r--   0 runner    (1001) docker     (121)       73 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-plus-square.gif
--rw-r--r--   0 runner    (1001) docker     (121)       75 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-previous.gif
--rw-r--r--   0 runner    (1001) docker     (121)       88 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-processing.gif
--rw-r--r--   0 runner    (1001) docker     (121)       79 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-question-circle.gif
--rw-r--r--   0 runner    (1001) docker     (121)       77 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-refresh.gif
--rw-r--r--   0 runner    (1001) docker     (121)       77 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-rocket.gif
--rw-r--r--   0 runner    (1001) docker     (121)       82 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-save.gif
--rw-r--r--   0 runner    (1001) docker     (121)       79 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-search.gif
--rw-r--r--   0 runner    (1001) docker     (121)       78 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-sign-in.gif
--rw-r--r--   0 runner    (1001) docker     (121)       79 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-sign-out.gif
--rw-r--r--   0 runner    (1001) docker     (121)       76 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-sitemap.gif
--rw-r--r--   0 runner    (1001) docker     (121)       91 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-stop-workflow.gif
--rw-r--r--   0 runner    (1001) docker     (121)       73 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-stop.gif
--rw-r--r--   0 runner    (1001) docker     (121)      691 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-tags.gif
--rw-r--r--   0 runner    (1001) docker     (121)      277 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-times-circle_alert.gif
--rw-r--r--   0 runner    (1001) docker     (121)       76 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-times.gif
--rw-r--r--   0 runner    (1001) docker     (121)       87 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-to_install.gif
--rw-r--r--   0 runner    (1001) docker     (121)       81 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-trash-o.gif
--rw-r--r--   0 runner    (1001) docker     (121)       70 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-unchecked.gif
--rw-r--r--   0 runner    (1001) docker     (121)       76 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-undo.gif
--rw-r--r--   0 runner    (1001) docker     (121)       68 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-uninstall.gif
--rw-r--r--   0 runner    (1001) docker     (121)       76 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-update.gif
--rw-r--r--   0 runner    (1001) docker     (121)       75 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-upload.gif
--rw-r--r--   0 runner    (1001) docker     (121)      718 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/favicon.gif
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     3808 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/file.gif
--rw-r--r--   0 runner    (1001) docker     (121)      216 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/file_folder.gif
--rw-r--r--   0 runner    (1001) docker     (121)      340 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/file_generic.gif
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/file_image.gif
--rw-r--r--   0 runner    (1001) docker     (121)      570 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/file_java.gif
--rw-r--r--   0 runner    (1001) docker     (121)      249 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/file_log.gif
--rw-r--r--   0 runner    (1001) docker     (121)      564 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/file_md.gif
--rw-r--r--   0 runner    (1001) docker     (121)      544 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/file_python.gif
--rw-r--r--   0 runner    (1001) docker     (121)      545 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/file_sqlite.gif
--rw-r--r--   0 runner    (1001) docker     (121)      104 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/file_stack.gif
--rw-r--r--   0 runner    (1001) docker     (121)      561 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/file_text.gif
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/file_vol.gif
--rw-r--r--   0 runner    (1001) docker     (121)    16824 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/loading.gif
--rw-r--r--   0 runner    (1001) docker     (121)      876 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/logoInstruct.gif
--rw-r--r--   0 runner    (1001) docker     (121)     4345 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/logo_cnb_without_title.gif
--rw-r--r--   0 runner    (1001) docker     (121)     3982 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/logo_i2pc_with_title.gif
--rw-r--r--   0 runner    (1001) docker     (121)      465 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/newProt.gif
--rw-r--r--   0 runner    (1001) docker     (121)    16902 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/no-image.gif
--rw-r--r--   0 runner    (1001) docker     (121)     3660 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/no-image.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     6923 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/no-image128.gif
--rw-r--r--   0 runner    (1001) docker     (121)    28320 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/phenix.gif
--rw-r--r--   0 runner    (1001) docker     (121)      343 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/prot_disabled.gif
--rw-r--r--   0 runner    (1001) docker     (121)      544 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/python_file.gif
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/question.gif
--rw-r--r--   0 runner    (1001) docker     (121)       83 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/rename.gif
--rw-r--r--   0 runner    (1001) docker     (121)       68 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/root.gif
--rw-r--r--   0 runner    (1001) docker     (121)    42677 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_bn.gif
--rw-r--r--   0 runner    (1001) docker     (121)     1428 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_icon.gif
--rw-r--r--   0 runner    (1001) docker     (121)   126140 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_icon.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3900 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_icon_proj.gif
--rw-r--r--   0 runner    (1001) docker     (121)     6251 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_icon_projs.gif
--rw-r--r--   0 runner    (1001) docker     (121)     4878 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_icon_prot.gif
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_logo.gif
--rw-r--r--   0 runner    (1001) docker     (121)    13219 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_logo_normal.gif
--rw-r--r--   0 runner    (1001) docker     (121)     2958 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_logo_small.gif
--rw-r--r--   0 runner    (1001) docker     (121)     3725 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_logo_small_web.gif
--rw-r--r--   0 runner    (1001) docker     (121)     3304 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_logo_transparent.gif
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2020-12-11 16:07:30.882427 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/
--rw-r--r--   0 runner    (1001) docker     (121)      268 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/arrowDown.png
--rw-r--r--   0 runner    (1001) docker     (121)      276 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/arrowUp.png
--rw-r--r--   0 runner    (1001) docker     (121)   284666 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/background_section.png
--rw-r--r--   0 runner    (1001) docker     (121)      208 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/colRowModeOff.png
--rw-r--r--   0 runner    (1001) docker     (121)      180 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/colRowModeOn.png
--rw-r--r--   0 runner    (1001) docker     (121)      624 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/delete.png
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/doc_icon.png
--rw-r--r--   0 runner    (1001) docker     (121)      792 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/download_icon.png
--rw-r--r--   0 runner    (1001) docker     (121)      493 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/enabled_gallery.png
--rw-r--r--   0 runner    (1001) docker     (121)      173 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/galleryViewOff.png
--rw-r--r--   0 runner    (1001) docker     (121)      159 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/galleryViewOn.png
--rw-r--r--   0 runner    (1001) docker     (121)      451 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/goto.png
--rw-r--r--   0 runner    (1001) docker     (121)     2736 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/menu.png
--rw-r--r--   0 runner    (1001) docker     (121)      288 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/separator.png
--rw-r--r--   0 runner    (1001) docker     (121)      200 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/tableViewOff.png
--rw-r--r--   0 runner    (1001) docker     (121)      172 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/tableViewOn.png
--rw-r--r--   0 runner    (1001) docker     (121)      262 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 runner    (1001) docker     (121)      332 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0 runner    (1001) docker     (121)      280 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 runner    (1001) docker     (121)      751 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/volumeOff.png
--rw-r--r--   0 runner    (1001) docker     (121)      614 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/volumeOn.png
--rw-r--r--   0 runner    (1001) docker     (121)      118 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/resources/users.gif
--rw-r--r--   0 runner    (1001) docker     (121)     8702 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2020-12-11 16:07:30.882427 scipion-pyworkflow-3.0.8/pyworkflow/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    12576 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      493 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10673 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/tests/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2020-12-11 16:07:30.886427 scipion-pyworkflow-3.0.8/pyworkflow/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     1429 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14943 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     3442 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/utils/echo.py
--rw-r--r--   0 runner    (1001) docker     (121)    31140 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/utils/file_transfer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5365 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/utils/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     4636 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     5703 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/utils/mpi.py
--rw-r--r--   0 runner    (1001) docker     (121)    14765 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (121)     4349 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (121)     2218 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     5345 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (121)    18461 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/utils/properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     4189 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/utils/reflection.py
--rw-r--r--   0 runner    (1001) docker     (121)     7399 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/utils/remote.py
--rw-r--r--   0 runner    (1001) docker     (121)    24116 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8534 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/utils/which.py
--rw-r--r--   0 runner    (1001) docker     (121)    10941 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2020-12-11 16:07:30.886427 scipion-pyworkflow-3.0.8/pyworkflow/webservices/
--rw-r--r--   0 runner    (1001) docker     (121)      294 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/webservices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      575 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/webservices/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     6242 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/webservices/notifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     2365 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/webservices/repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     2764 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflow/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2020-12-11 16:07:30.886427 scipion-pyworkflow-3.0.8/pyworkflowtests/
--rw-r--r--   0 runner    (1001) docker     (121)     1616 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflowtests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2102 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflowtests/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (121)    28478 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflowtests/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)     4460 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflowtests/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2020-12-11 16:07:30.886427 scipion-pyworkflow-3.0.8/pyworkflowtests/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflowtests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2685 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflowtests/tests/test_canvas.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1624 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflowtests/tests/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (121)     4272 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflowtests/tests/test_logs.py
--rw-r--r--   0 runner    (1001) docker     (121)    13558 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflowtests/tests/test_mappers.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14592 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflowtests/tests/test_object.py
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflowtests/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (121)     2430 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflowtests/tests/test_protocol_execution.py
--rw-r--r--   0 runner    (1001) docker     (121)     3291 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflowtests/tests/test_protocol_export.py
--rw-r--r--   0 runner    (1001) docker     (121)     5755 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflowtests/tests/test_protocol_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     5544 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/pyworkflowtests/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      116 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2020-12-11 16:07:30.886427 scipion-pyworkflow-3.0.8/scipion_pyworkflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4022 2020-12-11 16:07:30.000000 scipion-pyworkflow-3.0.8/scipion_pyworkflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8734 2020-12-11 16:07:30.000000 scipion-pyworkflow-3.0.8/scipion_pyworkflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2020-12-11 16:07:30.000000 scipion-pyworkflow-3.0.8/scipion_pyworkflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2020-12-11 16:07:30.000000 scipion-pyworkflow-3.0.8/scipion_pyworkflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      117 2020-12-11 16:07:30.000000 scipion-pyworkflow-3.0.8/scipion_pyworkflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2020-12-11 16:07:30.000000 scipion-pyworkflow-3.0.8/scipion_pyworkflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2020-12-11 16:07:30.890427 scipion-pyworkflow-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     9111 2020-12-11 16:07:19.000000 scipion-pyworkflow-3.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.612883 scipion-pyworkflow-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (122)    35148 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4022 2021-02-01 09:45:05.612883 scipion-pyworkflow-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2243 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.588883 scipion-pyworkflow-3.0.9/pyworkflow/
+-rw-r--r--   0 runner    (1001) docker     (122)     1246 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.588883 scipion-pyworkflow-3.0.9/pyworkflow/apps/
+-rw-r--r--   0 runner    (1001) docker     (122)     1187 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1356 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1829 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3055 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_project.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5368 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_protocol_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1952 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_protocol_mpirun.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2707 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_protocol_remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1635 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_protocol_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11868 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9040 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_schedule_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_sleep.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16530 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_sync_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2595 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8393 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4464 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.588883 scipion-pyworkflow-3.0.9/pyworkflow/gui/
+-rw-r--r--   0 runner    (1001) docker     (122)     1351 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23402 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/browser.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36994 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27922 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (122)   106438 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/form.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8810 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9856 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/graph_layout.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16949 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7086 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/matplotlib_image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8116 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.588883 scipion-pyworkflow-3.0.9/pyworkflow/gui/project/
+-rw-r--r--   0 runner    (1001) docker     (122)     1118 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7694 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/project/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1852 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/project/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7251 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/project/labels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18168 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3057 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/project/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19468 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/project/viewdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21347 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/project/viewprojects.py
+-rw-r--r--   0 runner    (1001) docker     (122)   109042 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/project/viewprotocols.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27645 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/text.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8531 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22023 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10761 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.592883 scipion-pyworkflow-3.0.9/pyworkflow/mapper/
+-rw-r--r--   0 runner    (1001) docker     (122)     1219 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7354 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/mapper/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    54781 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/mapper/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4724 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/mapper/sqlite_db.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10720 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/mapper/xmlmapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48759 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/object.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25158 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.592883 scipion-pyworkflow-3.0.9/pyworkflow/project/
+-rw-r--r--   0 runner    (1001) docker     (122)     1384 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11818 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6706 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)    67249 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/project.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.592883 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2580 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/clean_projects.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2921 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2488 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2909 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/edit_workflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      890 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/fix_links.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2685 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/load.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2564 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3461 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/schedule.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      901 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/stack2volume.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2452 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/stop.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.592883 scipion-pyworkflow-3.0.9/pyworkflow/protocol/
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2122 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/protocol/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2976 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/protocol/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14633 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/protocol/executor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11869 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/protocol/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9256 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/protocol/launch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/protocol/package.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23108 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/protocol/params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    85721 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/protocol/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.604883 scipion-pyworkflow-3.0.9/pyworkflow/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)     6187 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/ChimeraLogoSmall.gif
+-rw-r--r--   0 runner    (1001) docker     (122)     6798 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/I2PC.gif
+-rw-r--r--   0 runner    (1001) docker     (122)    64364 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/background_section.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      987 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/bookmark.gif
+-rw-r--r--   0 runner    (1001) docker     (122)     3771 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/ccp4_200.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/class_obj.gif
+-rw-r--r--   0 runner    (1001) docker     (122)    16491 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/cryoem_logo.gif
+-rw-r--r--   0 runner    (1001) docker     (122)    34177 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/cryomethods_logo.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/debug.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      586 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/doc_icon.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      418 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/download_icon.gif
+-rw-r--r--   0 runner    (1001) docker     (122)    27027 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/error_page.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-arrow-left.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-arrow-up.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-ban.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-bars.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-check.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-checked.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-cog.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-cogs.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-database.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-delete-operation.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-download.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-exclamation-triangle_alert.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-external-link.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-eye.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-failure.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-file-o.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-files-o.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-folder-open.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-home.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-iconmoon-link.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-info-circle_alert.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-install.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-installed.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-laptop.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-lightbulb-o.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-list-ul.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-magic.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-minus-square.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-next.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-paint-brush.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-pencil.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-play-circle-o.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-plus-circle.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-plus-square.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-previous.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-processing.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-question-circle.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-refresh.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-rocket.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-save.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-search.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-sign-in.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-sign-out.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-sitemap.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-stop-workflow.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-stop.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-tags.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-times-circle_alert.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-times.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-to_install.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-trash-o.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-unchecked.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-undo.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-uninstall.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-update.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-upload.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      718 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/favicon.gif
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)     3808 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_folder.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      340 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_generic.gif
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_image.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      570 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_java.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_log.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_md.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_python.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_sqlite.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_stack.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_text.gif
+-rw-r--r--   0 runner    (1001) docker     (122)     1072 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_vol.gif
+-rw-r--r--   0 runner    (1001) docker     (122)    16824 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      876 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/logoInstruct.gif
+-rw-r--r--   0 runner    (1001) docker     (122)     4345 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/logo_cnb_without_title.gif
+-rw-r--r--   0 runner    (1001) docker     (122)     3982 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/logo_i2pc_with_title.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      465 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/newProt.gif
+-rw-r--r--   0 runner    (1001) docker     (122)    16902 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/no-image.gif
+-rw-r--r--   0 runner    (1001) docker     (122)     3660 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/no-image.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)     6923 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/no-image128.gif
+-rw-r--r--   0 runner    (1001) docker     (122)    28320 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/phenix.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/prot_disabled.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/python_file.gif
+-rw-r--r--   0 runner    (1001) docker     (122)     1176 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/question.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/rename.gif
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/root.gif
+-rw-r--r--   0 runner    (1001) docker     (122)    42677 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_bn.gif
+-rw-r--r--   0 runner    (1001) docker     (122)     1428 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_icon.gif
+-rw-r--r--   0 runner    (1001) docker     (122)   126140 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_icon_proj.gif
+-rw-r--r--   0 runner    (1001) docker     (122)     6251 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_icon_projs.gif
+-rw-r--r--   0 runner    (1001) docker     (122)     4878 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_icon_prot.gif
+-rw-r--r--   0 runner    (1001) docker     (122)     1004 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_logo.gif
+-rw-r--r--   0 runner    (1001) docker     (122)    13219 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_logo_normal.gif
+-rw-r--r--   0 runner    (1001) docker     (122)     2958 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_logo_small.gif
+-rw-r--r--   0 runner    (1001) docker     (122)     3725 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_logo_small_web.gif
+-rw-r--r--   0 runner    (1001) docker     (122)     3304 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_logo_transparent.gif
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.608883 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/arrowDown.png
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/arrowUp.png
+-rw-r--r--   0 runner    (1001) docker     (122)   284666 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/background_section.png
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/colRowModeOff.png
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/colRowModeOn.png
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/delete.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1015 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/doc_icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)      792 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/download_icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/enabled_gallery.png
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/galleryViewOff.png
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/galleryViewOn.png
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/goto.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2736 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/menu.png
+-rw-r--r--   0 runner    (1001) docker     (122)      288 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/separator.png
+-rw-r--r--   0 runner    (1001) docker     (122)      200 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/tableViewOff.png
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/tableViewOn.png
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/volumeOff.png
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/volumeOn.png
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/users.gif
+-rw-r--r--   0 runner    (1001) docker     (122)     8702 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/template.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.608883 scipion-pyworkflow-3.0.9/pyworkflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    12576 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10673 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.608883 scipion-pyworkflow-3.0.9/pyworkflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     1429 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14943 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3442 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/echo.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31140 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/file_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5365 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4636 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5703 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14765 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4349 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2218 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5345 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18461 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4189 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7399 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24116 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8534 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/which.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10941 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.608883 scipion-pyworkflow-3.0.9/pyworkflow/webservices/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/webservices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/webservices/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6242 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/webservices/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2365 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/webservices/repository.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2764 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.608883 scipion-pyworkflow-3.0.9/pyworkflowtests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1616 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2102 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28478 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4460 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.612883 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2685 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_canvas.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1624 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4272 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13558 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_mappers.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    14592 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2430 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_protocol_execution.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3291 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_protocol_export.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5755 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_protocol_output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5544 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.612883 scipion-pyworkflow-3.0.9/scipion_pyworkflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4022 2021-02-01 09:45:05.000000 scipion-pyworkflow-3.0.9/scipion_pyworkflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8734 2021-02-01 09:45:05.000000 scipion-pyworkflow-3.0.9/scipion_pyworkflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2021-02-01 09:45:05.000000 scipion-pyworkflow-3.0.9/scipion_pyworkflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2021-02-01 09:45:05.000000 scipion-pyworkflow-3.0.9/scipion_pyworkflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2021-02-01 09:45:05.000000 scipion-pyworkflow-3.0.9/scipion_pyworkflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2021-02-01 09:45:05.000000 scipion-pyworkflow-3.0.9/scipion_pyworkflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2021-02-01 09:45:05.612883 scipion-pyworkflow-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     9111 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/setup.py
```

### Comparing `scipion-pyworkflow-3.0.8/LICENSE.txt` & `scipion-pyworkflow-3.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/PKG-INFO` & `scipion-pyworkflow-3.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-pyworkflow
-Version: 3.0.8
+Version: 3.0.9
 Summary: Simple workflow platform used in scientific applications, initially developed within the Scipion framework for image processing in Electron Microscopy.
 Home-page: https://github.com/scipion-em/scipion-pyworkflow
 Author: J.M. De la Rosa Trevin, Roberto Marabini, Grigory Sharov, Josue Gomez Blanco, Pablo Conesa, Yunior Fonseca Reyna
 Author-email: delarosatrevin@scilifelab.se, roberto@cnb.csic.es, gsharov@mrc-lmb.cam.ac.uk, josue.gomez-blanco@mcgill.ca, pconesa@cnb.csic.es, fonsecareyna@cnb.csic.es
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-pyworkflow/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-pyworkflow/
```

### Comparing `scipion-pyworkflow-3.0.8/README.rst` & `scipion-pyworkflow-3.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/__init__.py` & `scipion-pyworkflow-3.0.9/pyworkflow/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/apps/__init__.py` & `scipion-pyworkflow-3.0.9/pyworkflow/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_manager.py` & `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_manager.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_plot.py` & `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_plot.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_project.py` & `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_project.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_protocol_list.py` & `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_protocol_list.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_protocol_mpirun.py` & `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_protocol_mpirun.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_protocol_remote.py` & `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_protocol_remote.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_protocol_run.py` & `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_protocol_run.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_run_tests.py` & `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_run_tests.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_schedule_run.py` & `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_schedule_run.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_sleep.py` & `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_sleep.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_sync_data.py` & `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_sync_data.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/apps/pw_viewer.py` & `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_viewer.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/config.py` & `scipion-pyworkflow-3.0.9/pyworkflow/config.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/constants.py` & `scipion-pyworkflow-3.0.9/pyworkflow/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 CORE_VERSION = '3.0.0'
 
 # Versions
 VERSION_1 = '1.0.0'
 VERSION_1_1 = '1.1.0'
 VERSION_1_2 = '1.2.0'
 VERSION_2_0 = '2.0.0'
-VERSION_3_0 = '3.0.8'
+VERSION_3_0 = '3.0.9'
 
 # For a new release, define a new constant and assign it to LAST_VERSION
 # The existing one has to be added to OLD_VERSIONS list.
 LAST_VERSION = VERSION_3_0
 OLD_VERSIONS = (VERSION_1, VERSION_1_1, VERSION_1_2, VERSION_2_0)
 
 # Dir names
```

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/__init__.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/browser.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/browser.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/canvas.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/canvas.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/dialog.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/dialog.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/form.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/form.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/graph.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/graph.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/graph_layout.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/graph_layout.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/gui.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/gui.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/matplotlib_image.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/matplotlib_image.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/plotter.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/plotter.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/project/__init__.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/project/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/project/base.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/project/base.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/project/constants.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/project/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/project/labels.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/project/labels.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/project/project.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/project/project.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/project/utils.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/project/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/project/viewdata.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/project/viewdata.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/project/viewprojects.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/project/viewprojects.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/project/viewprotocols.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/project/viewprotocols.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/text.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/text.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/tooltip.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/tooltip.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/tree.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/tree.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/gui/widgets.py` & `scipion-pyworkflow-3.0.9/pyworkflow/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/mapper/__init__.py` & `scipion-pyworkflow-3.0.9/pyworkflow/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/mapper/mapper.py` & `scipion-pyworkflow-3.0.9/pyworkflow/mapper/mapper.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/mapper/sqlite.py` & `scipion-pyworkflow-3.0.9/pyworkflow/mapper/sqlite.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/mapper/sqlite_db.py` & `scipion-pyworkflow-3.0.9/pyworkflow/mapper/sqlite_db.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/mapper/xmlmapper.py` & `scipion-pyworkflow-3.0.9/pyworkflow/mapper/xmlmapper.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/object.py` & `scipion-pyworkflow-3.0.9/pyworkflow/object.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/plugin.py` & `scipion-pyworkflow-3.0.9/pyworkflow/plugin.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/project/__init__.py` & `scipion-pyworkflow-3.0.9/pyworkflow/project/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/project/config.py` & `scipion-pyworkflow-3.0.9/pyworkflow/project/config.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/project/manager.py` & `scipion-pyworkflow-3.0.9/pyworkflow/project/manager.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/project/project.py` & `scipion-pyworkflow-3.0.9/pyworkflow/project/project.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/clean_projects.py` & `scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/clean_projects.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/config.py` & `scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/config.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/create.py` & `scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/create.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/edit_workflow.py` & `scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/edit_workflow.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/fix_links.py` & `scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/fix_links.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/load.py` & `scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/load.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/refresh.py` & `scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/refresh.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/schedule.py` & `scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/schedule.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/stack2volume.py` & `scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/stack2volume.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/project/scripts/stop.py` & `scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/stop.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/protocol/__init__.py` & `scipion-pyworkflow-3.0.9/pyworkflow/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/protocol/bibtex.py` & `scipion-pyworkflow-3.0.9/pyworkflow/protocol/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/protocol/constants.py` & `scipion-pyworkflow-3.0.9/pyworkflow/protocol/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/protocol/executor.py` & `scipion-pyworkflow-3.0.9/pyworkflow/protocol/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,22 +168,21 @@
         self.gpuDict = {}
 
         if self.gpuList:
             nodes = range(nThreads)
             nGpu = len(self.gpuList)
 
             if nGpu > nThreads:
-                chunk = nGpu / nThreads
+                chunk = int(nGpu / nThreads)
                 for i, node in enumerate(nodes):
                     self.gpuDict[node] = list(self.gpuList[i*chunk:(i+1)*chunk])
             else:
                 # Expand gpuList repeating until reach nThreads items
                 if nThreads > nGpu:
-                    import numpy as np
-                    newList = np.asarray(self.gpuList) * (nThreads/nGpu+1)
+                    newList = self.gpuList * (int(nThreads/nGpu)+1)
                     self.gpuList = newList[:nThreads]
 
                 for node, gpu in zip(nodes, self.gpuList):
                     self.gpuDict[node] = [gpu]
 
     def getGpuList(self):
         """ Return the GPU list assigned to current thread
```

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/protocol/hosts.py` & `scipion-pyworkflow-3.0.9/pyworkflow/protocol/hosts.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/protocol/launch.py` & `scipion-pyworkflow-3.0.9/pyworkflow/protocol/launch.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/protocol/package.py` & `scipion-pyworkflow-3.0.9/pyworkflow/protocol/package.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/protocol/params.py` & `scipion-pyworkflow-3.0.9/pyworkflow/protocol/params.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/protocol/protocol.py` & `scipion-pyworkflow-3.0.9/pyworkflow/protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/ChimeraLogoSmall.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/ChimeraLogoSmall.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/I2PC.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/I2PC.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/background_section.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/background_section.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/bookmark.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/bookmark.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/ccp4_200.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/ccp4_200.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/cryoem_logo.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/cryoem_logo.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/cryomethods_logo.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/cryomethods_logo.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/doc_icon.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/doc_icon.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/error_page.jpg` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/error_page.jpg`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/fa-tags.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-tags.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/favicon.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/favicon.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/favicon.ico` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/file.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/file.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/file_image.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/file_image.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/file_java.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/file_java.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/file_md.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/file_md.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/file_python.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/file_python.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/file_sqlite.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/file_sqlite.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/file_text.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/file_text.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/file_vol.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/file_vol.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/loading.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/loading.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/logoInstruct.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/logoInstruct.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/logo_cnb_without_title.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/logo_cnb_without_title.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/logo_i2pc_with_title.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/logo_i2pc_with_title.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/no-image.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/no-image.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/no-image.jpg` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/no-image.jpg`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/no-image128.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/no-image128.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/phenix.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/phenix.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/python_file.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/python_file.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/question.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/question.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_bn.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_bn.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_icon.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_icon.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_icon.svg` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_icon.svg`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_icon_proj.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_icon_proj.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_icon_projs.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_icon_projs.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_icon_prot.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_icon_prot.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_logo.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_logo.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_logo_normal.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_logo_normal.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_logo_small.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_logo_small.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_logo_small_web.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_logo_small_web.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/scipion_logo_transparent.gif` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_logo_transparent.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/background_section.png` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/background_section.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/delete.png` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/delete.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/doc_icon.png` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/doc_icon.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/download_icon.png` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/download_icon.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/menu.png` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/menu.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/volumeOff.png` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/volumeOff.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/resources/showj/volumeOn.png` & `scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/volumeOn.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/template.py` & `scipion-pyworkflow-3.0.9/pyworkflow/template.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/tests/__init__.py` & `scipion-pyworkflow-3.0.9/pyworkflow/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/tests/tests.py` & `scipion-pyworkflow-3.0.9/pyworkflow/tests/tests.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/utils/__init__.py` & `scipion-pyworkflow-3.0.9/pyworkflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/utils/dataset.py` & `scipion-pyworkflow-3.0.9/pyworkflow/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/utils/echo.py` & `scipion-pyworkflow-3.0.9/pyworkflow/utils/echo.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/utils/file_transfer.py` & `scipion-pyworkflow-3.0.9/pyworkflow/utils/file_transfer.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/utils/graph.py` & `scipion-pyworkflow-3.0.9/pyworkflow/utils/graph.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/utils/log.py` & `scipion-pyworkflow-3.0.9/pyworkflow/utils/log.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/utils/mpi.py` & `scipion-pyworkflow-3.0.9/pyworkflow/utils/mpi.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/utils/path.py` & `scipion-pyworkflow-3.0.9/pyworkflow/utils/path.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/utils/process.py` & `scipion-pyworkflow-3.0.9/pyworkflow/utils/process.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/utils/profiler.py` & `scipion-pyworkflow-3.0.9/pyworkflow/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/utils/progressbar.py` & `scipion-pyworkflow-3.0.9/pyworkflow/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/utils/properties.py` & `scipion-pyworkflow-3.0.9/pyworkflow/utils/properties.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/utils/reflection.py` & `scipion-pyworkflow-3.0.9/pyworkflow/utils/reflection.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/utils/remote.py` & `scipion-pyworkflow-3.0.9/pyworkflow/utils/remote.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/utils/utils.py` & `scipion-pyworkflow-3.0.9/pyworkflow/utils/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/utils/which.py` & `scipion-pyworkflow-3.0.9/pyworkflow/utils/which.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/viewer.py` & `scipion-pyworkflow-3.0.9/pyworkflow/viewer.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/webservices/config.py` & `scipion-pyworkflow-3.0.9/pyworkflow/webservices/config.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/webservices/notifier.py` & `scipion-pyworkflow-3.0.9/pyworkflow/webservices/notifier.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/webservices/repository.py` & `scipion-pyworkflow-3.0.9/pyworkflow/webservices/repository.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflow/wizard.py` & `scipion-pyworkflow-3.0.9/pyworkflow/wizard.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflowtests/__init__.py` & `scipion-pyworkflow-3.0.9/pyworkflowtests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflowtests/bibtex.py` & `scipion-pyworkflow-3.0.9/pyworkflowtests/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflowtests/objects.py` & `scipion-pyworkflow-3.0.9/pyworkflowtests/objects.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflowtests/protocols.py` & `scipion-pyworkflow-3.0.9/pyworkflowtests/protocols.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflowtests/tests/test_canvas.py` & `scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_canvas.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflowtests/tests/test_domain.py` & `scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflowtests/tests/test_logs.py` & `scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_logs.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflowtests/tests/test_mappers.py` & `scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_mappers.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflowtests/tests/test_object.py` & `scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_object.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflowtests/tests/test_project.py` & `scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflowtests/tests/test_protocol_execution.py` & `scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_protocol_execution.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflowtests/tests/test_protocol_export.py` & `scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_protocol_export.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflowtests/tests/test_protocol_output.py` & `scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_protocol_output.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/pyworkflowtests/tests/test_utils.py` & `scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/scipion_pyworkflow.egg-info/PKG-INFO` & `scipion-pyworkflow-3.0.9/scipion_pyworkflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-pyworkflow
-Version: 3.0.8
+Version: 3.0.9
 Summary: Simple workflow platform used in scientific applications, initially developed within the Scipion framework for image processing in Electron Microscopy.
 Home-page: https://github.com/scipion-em/scipion-pyworkflow
 Author: J.M. De la Rosa Trevin, Roberto Marabini, Grigory Sharov, Josue Gomez Blanco, Pablo Conesa, Yunior Fonseca Reyna
 Author-email: delarosatrevin@scilifelab.se, roberto@cnb.csic.es, gsharov@mrc-lmb.cam.ac.uk, josue.gomez-blanco@mcgill.ca, pconesa@cnb.csic.es, fonsecareyna@cnb.csic.es
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-pyworkflow/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-pyworkflow/
```

### Comparing `scipion-pyworkflow-3.0.8/scipion_pyworkflow.egg-info/SOURCES.txt` & `scipion-pyworkflow-3.0.9/scipion_pyworkflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.8/setup.py` & `scipion-pyworkflow-3.0.9/setup.py`

 * *Files identical despite different names*

