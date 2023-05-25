# Comparing `tmp/griffon-0.2.3.tar.gz` & `tmp/griffon-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griffon-0.2.3.tar", last modified: Wed May 24 12:45:22 2023, max compression
+gzip compressed data, was "griffon-0.2.4.tar", last modified: Thu May 25 07:47:51 2023, max compression
```

## Comparing `griffon-0.2.3.tar` & `griffon-0.2.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:45:22.455450 griffon-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-24 12:45:07.000000 griffon-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-24 12:45:22.455450 griffon-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-24 12:45:07.000000 griffon-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:45:22.451450 griffon-0.2.3/griffon/
--rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:45:22.451450 griffon-0.2.3/griffon/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:45:22.451450 griffon-0.2.3/griffon/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/commands/docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:45:22.451450 griffon-0.2.3/griffon/commands/entities/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/commands/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26909 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/commands/entities/community_component_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    27264 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/commands/entities/corgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/commands/entities/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/commands/entities/osidb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/commands/plugin_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:45:22.455450 griffon-0.2.3/griffon/commands/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/commands/plugins/bugzilla.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/commands/plugins/cve_mitre.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/commands/plugins/cvelib.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/commands/plugins/fcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/commands/plugins/go_vuln.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/commands/plugins/osv.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/commands/plugins/semgrep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/commands/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    24381 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/commands/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/commands/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    52162 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:45:22.455450 griffon-0.2.3/griffon/services/
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/services/core_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    36879 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/services/core_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    20730 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/services/core_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:45:22.455450 griffon-0.2.3/griffon/static/
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-24 12:45:07.000000 griffon-0.2.3/griffon/static/default_griffonrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:45:22.451450 griffon-0.2.3/griffon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-24 12:45:22.000000 griffon-0.2.3/griffon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-24 12:45:22.000000 griffon-0.2.3/griffon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:45:22.000000 griffon-0.2.3/griffon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-24 12:45:22.000000 griffon-0.2.3/griffon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-24 12:45:22.000000 griffon-0.2.3/griffon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-24 12:45:22.000000 griffon-0.2.3/griffon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-24 12:45:07.000000 griffon-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 12:45:22.455450 griffon-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-24 12:45:07.000000 griffon-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:45:22.455450 griffon-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-24 12:45:07.000000 griffon-0.2.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-24 12:45:07.000000 griffon-0.2.3/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-24 12:45:07.000000 griffon-0.2.3/tests/test_manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-24 12:45:07.000000 griffon-0.2.3/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-24 12:45:07.000000 griffon-0.2.3/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-24 12:45:07.000000 griffon-0.2.3/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-24 12:45:07.000000 griffon-0.2.3/tests/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-24 12:45:07.000000 griffon-0.2.3/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:47:51.815697 griffon-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-25 07:47:35.000000 griffon-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-25 07:47:51.815697 griffon-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-25 07:47:35.000000 griffon-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:47:51.811696 griffon-0.2.4/griffon/
+-rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:47:51.811696 griffon-0.2.4/griffon/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:47:51.811696 griffon-0.2.4/griffon/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:47:51.811696 griffon-0.2.4/griffon/commands/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26909 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/entities/community_component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27403 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/entities/corgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/entities/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/entities/osidb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/plugin_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:47:51.815697 griffon-0.2.4/griffon/commands/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/plugins/bugzilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/plugins/cve_mitre.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/plugins/cvelib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/plugins/fcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/plugins/go_vuln.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/plugins/osv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/plugins/semgrep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24381 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52663 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:47:51.815697 griffon-0.2.4/griffon/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/services/core_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37045 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/services/core_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20730 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/services/core_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:47:51.815697 griffon-0.2.4/griffon/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/static/default_griffonrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:47:51.811696 griffon-0.2.4/griffon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-25 07:47:51.000000 griffon-0.2.4/griffon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-25 07:47:51.000000 griffon-0.2.4/griffon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:47:51.000000 griffon-0.2.4/griffon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 07:47:51.000000 griffon-0.2.4/griffon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-25 07:47:51.000000 griffon-0.2.4/griffon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-25 07:47:51.000000 griffon-0.2.4/griffon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-25 07:47:35.000000 griffon-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:47:51.815697 griffon-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-25 07:47:35.000000 griffon-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:47:51.815697 griffon-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-25 07:47:35.000000 griffon-0.2.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-25 07:47:35.000000 griffon-0.2.4/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-25 07:47:35.000000 griffon-0.2.4/tests/test_manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-25 07:47:35.000000 griffon-0.2.4/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-25 07:47:35.000000 griffon-0.2.4/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-25 07:47:35.000000 griffon-0.2.4/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-25 07:47:35.000000 griffon-0.2.4/tests/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-25 07:47:35.000000 griffon-0.2.4/tests/test_unit.py
```

### Comparing `griffon-0.2.3/LICENSE` & `griffon-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/PKG-INFO` & `griffon-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griffon
-Version: 0.2.3
+Version: 0.2.4
 Summary: Red Hat Product Security CLI
 Home-page: https://github.com/RedHatProductSecurity/griffon
 Author: James Fuller, Red Hat Product Security
 License: MIT
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `griffon-0.2.3/README.md` & `griffon-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/griffon/__init__.py` & `griffon-0.2.4/griffon/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import osidb_bindings
 from osidb_bindings.bindings.python_client.models import Affect, Flaw, Tracker
 from pkg_resources import resource_filename  # type: ignore
 from rich.logging import RichHandler
 
 from griffon.output import console
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 
 if "CORGI_API_URL" not in os.environ:
     print("Must set CORGI_API_URL environment variable.")
     exit(1)
 CORGI_API_URL = os.environ["CORGI_API_URL"]
 
 if "OSIDB_API_URL" not in os.environ:
```

### Comparing `griffon-0.2.3/griffon/autocomplete/__init__.py` & `griffon-0.2.4/griffon/autocomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/griffon/cli.py` & `griffon-0.2.4/griffon/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,27 +105,28 @@
     "verbose",
     count=True,
     default=get_config_option("default", "verbosity", 0),
     help="Verbose output, more detailed search results, can be used multiple times (e.g. -vvv).",
 )  # noqa
 @click.option("--no-progress-bar", is_flag=True, help="Disable progress bar.")
 @click.option("--no-color", is_flag=True, help="Disable output of color ansi esc sequences.")
+@click.option("--no-wrap", is_flag=True, help="Disable wrapping of text output.")
 @click.option(
     "--profile",
     "profile",
     type=click.Choice(list_config_sections()),
     default=get_config_option(
         "default",
         "profile",
     ),
     help="Activate profile, defined in .griffonrc.",
 )
 @click.option("--editor/--no-editor", default=True, help="Allow text editor prompt.")
 @click.pass_context
-def cli(ctx, debug, format, verbose, no_progress_bar, no_color, profile, editor):
+def cli(ctx, debug, format, verbose, no_progress_bar, no_color, no_wrap, profile, editor):
     """Red Hat product security CLI"""
 
     if ctx.invoked_subcommand is None:
         click.echo(ctx.parent.get_help())
 
     if not debug:
         config_logging(level="INFO")
@@ -137,13 +138,16 @@
     ctx.obj["SHOW_INACTIVE"] = False
     ctx.obj["SHOW_PURL"] = False
     ctx.obj["SHOW_UPSTREAM"] = False
     ctx.obj["FORMAT"] = format
     ctx.obj["VERBOSE"] = verbose
     ctx.obj["NO_PROGRESS_BAR"] = no_progress_bar
     ctx.obj["NO_COLOR"] = no_color
+    ctx.obj["NO_WRAP"] = get_config_option("default", "no_wrap", False)
+    if no_wrap:
+        ctx.obj["NO_WRAP"] = no_wrap
     ctx.obj["PROFILE"] = profile
     ctx.obj["SHORT_VERSION_VALUES"] = True
     ctx.obj["EDITOR"] = editor
 
 
 cli.help = "Red Hat Product Security CLI"
```

### Comparing `griffon-0.2.3/griffon/commands/configure.py` & `griffon-0.2.4/griffon/commands/configure.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/griffon/commands/docs.py` & `griffon-0.2.4/griffon/commands/docs.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/griffon/commands/entities/__init__.py` & `griffon-0.2.4/griffon/commands/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/griffon/commands/entities/community_component_registry.py` & `griffon-0.2.4/griffon/commands/entities/community_component_registry.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/griffon/commands/entities/corgi.py` & `griffon-0.2.4/griffon/commands/entities/corgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -532,15 +532,19 @@
         ctx.obj["FORMAT"] = "json"  # TODO - investigate if we need yaml format.
     ps = None
     if ofuri:
         ps = session.product_streams.retrieve_list(ofuri=ofuri).additional_properties
     if product_stream_name:
         ps = session.product_streams.retrieve_list(name=product_stream_name).additional_properties
     if not ps:
-        logger.warning("could not find active product stream.")
+        logger.error("could not find active product stream.")
+        ctx.exit()
+    if not ps["manifest"]:
+        logger.error(f"could not find manifest for {product_stream_name}.")
+        ctx.exit()
     data = requests.get(ps["manifest"])
     cprint(data.json(), ctx=ctx)
 
 
 # BUILDS
```

### Comparing `griffon-0.2.3/griffon/commands/entities/helpers.py` & `griffon-0.2.4/griffon/commands/entities/helpers.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/griffon/commands/entities/osidb.py` & `griffon-0.2.4/griffon/commands/entities/osidb.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/griffon/commands/plugin_commands.py` & `griffon-0.2.4/griffon/commands/plugin_commands.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/griffon/commands/plugins/bugzilla.py` & `griffon-0.2.4/griffon/commands/plugins/bugzilla.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/griffon/commands/plugins/cve_mitre.py` & `griffon-0.2.4/griffon/commands/plugins/cve_mitre.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/griffon/commands/plugins/go_vuln.py` & `griffon-0.2.4/griffon/commands/plugins/go_vuln.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/griffon/commands/plugins/osv.py` & `griffon-0.2.4/griffon/commands/plugins/osv.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/griffon/commands/plugins/semgrep.py` & `griffon-0.2.4/griffon/commands/plugins/semgrep.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/griffon/commands/process.py` & `griffon-0.2.4/griffon/commands/process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/griffon/commands/queries.py` & `griffon-0.2.4/griffon/commands/queries.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/griffon/commands/reports.py` & `griffon-0.2.4/griffon/commands/reports.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/griffon/output.py` & `griffon-0.2.4/griffon/output.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,24 +99,24 @@
             if show_purl:
                 label = f"{item['node_type']}: {item['purl']}"
             child = tree.add(label)
             walk_component_tree(item, None, child, show_purl=show_purl)
     return tree
 
 
-def text_output_tree(ctx, output):
+def text_output_tree(ctx, output, no_wrap=False):
     tree = Tree(
         "component dependency tree",
         guide_style="bold magenta",
     )
     console.print(walk_component_tree(output, None, tree, show_purl=ctx.params["show_purl"]))
     ctx.exit()
 
 
-def text_output_product_summary(ctx, output, format, exclude_products):
+def text_output_product_summary(ctx, output, format, exclude_products, no_wrap=False):
     ordered_results = sorted(output["results"], key=lambda d: d["name"])
 
     if exclude_products:
         exclude_products_results = []
         for result in ordered_results:
             if result["product_version"] not in exclude_products:
                 exclude_products_results.append(result)
@@ -125,50 +125,52 @@
     if ctx.obj["VERBOSE"] == 0:
         for item in ordered_results:
             console.print(
                 Text(item["product"], style="bold magenta u"),
                 Text(item["product_version"], style="magenta"),
                 Text(item["name"], style="white"),
                 f"{item['brew_tags']}",
-                no_wrap=False,
+                no_wrap=no_wrap,
             )
     if ctx.obj["VERBOSE"] == 1:
         for item in ordered_results:
             console.print(
                 Text(item["product"], style="bold magenta u"),
                 Text(item["product_version"], style="magenta"),
                 Text(item["name"], style="white"),
                 item["brew_tags"],
                 item["ofuri"],
-                no_wrap=False,
+                no_wrap=no_wrap,
             )
     if ctx.obj["VERBOSE"] > 1:
         for item in ordered_results:
             console.print(
                 Text(item["product"], style="bold magenta u"),
                 Text(item["product_version"], style="magenta"),
                 Text(item["name"], style="white"),
                 item["brew_tags"],
                 item["ofuri"],
                 item["manifest_link"],
-                no_wrap=False,
+                no_wrap=no_wrap,
             )
     ctx.exit()
 
 
-def text_output_products_contain_component(ctx, output, exclude_products, exclude_components):
+def text_output_products_contain_component(
+    ctx, output, exclude_products, exclude_components, no_wrap=False
+):
     search_component_name = ctx.params["component_name"]
 
     # handle single component
     if ctx.params["purl"]:
         ordered_results = sorted(output["results"], key=lambda d: d["ofuri"])
         for item in ordered_results:
             console.print(
                 Text(item["ofuri"], style="bold magenta u"),
-                no_wrap=False,
+                no_wrap=no_wrap,
             )
         ctx.exit()
 
     # handle multiple components
     if "results" in output and output["count"] > 0:
         console.highlighter = None
 
@@ -262,15 +264,15 @@
                 ):
                     component_names.remove(f"{search_component_name}-container")
                 for cn in component_names:
                     # ensure {component name} is not in profile exclude components enum
                     if not any([match in cn for match in exclude_components]):
                         console.print(
                             f"{pv}/{cn}={flaw_operation}",
-                            no_wrap=False,
+                            no_wrap=no_wrap,
                         )
         else:
 
             if ctx.obj["VERBOSE"] == 0:  # product_version X component_name
                 for pv in result_tree.keys():
                     component_names = set()
                     for ps in result_tree[pv].keys():
@@ -281,22 +283,20 @@
                         and f"{search_component_name}-container" in component_names
                     ):
                         component_names.remove(f"{search_component_name}-container")
                     for cn in component_names:
                         # ensure {component name} is not in profile exclude components enum
                         if not any([match in cn for match in exclude_components]):
                             # highlight search term
-                            dep_name = re.sub(
-                                search_component_name, f"[b]{search_component_name}[/b]", cn
-                            )
+                            dep_name = re.sub(cn, f"[b]{cn}[/b]", cn)
                             dep = f"[grey93]{dep_name}[/grey93]"
                             console.print(
                                 Text(pv, style="magenta b u"),
                                 dep,
-                                no_wrap=False,
+                                no_wrap=no_wrap,
                             )
             if ctx.obj["VERBOSE"] == 1:  # product_stream X nvr x related_url
                 for pv in result_tree.keys():
                     for ps in result_tree[pv].keys():
                         for cn in result_tree[pv][ps].keys():
                             # ensure {component name} is not in profile exclude components enum
                             if not any([match in cn for match in exclude_components]):
@@ -332,15 +332,15 @@
                                         if len(upstream_component_names) > 1:
                                             upstream_component_name = f"[cyan]{upstream_component_names[0]} and {len(upstream_component_names) - 1} more[/cyan]"  # noqa
                                         console.print(
                                             Text(ps, style="magenta b u"),
                                             upstream_component_name,
                                             dep,
                                             f"([grey]{related_url}[/grey])",
-                                            no_wrap=False,
+                                            no_wrap=no_wrap,
                                         )
                                     source_component_names = list(
                                         set(
                                             [
                                                 source["name"]
                                                 for source in result_tree[pv][ps][cn][nvr][
                                                     "sources"
@@ -355,25 +355,25 @@
                                         if len(source_component_names) > 1:
                                             source_component_name = f"[red]{source_component_names[0]} and {len(source_component_names) - 1} more[/red]"  # noqa
                                         console.print(
                                             Text(ps, style="magenta b u"),
                                             source_component_name,
                                             dep,
                                             f"([grey]{related_url}[/grey])",
-                                            no_wrap=False,
+                                            no_wrap=no_wrap,
                                         )
                                     if (
                                         len(result_tree[pv][ps][cn][nvr]["upstreams"]) == 0
                                         and len(result_tree[pv][ps][cn][nvr]["sources"]) == 0
                                     ):
                                         console.print(
                                             Text(ps, style="magenta b u"),
                                             dep,
                                             f"([grey]{related_url}[/grey])",
-                                            no_wrap=False,
+                                            no_wrap=no_wrap,
                                         )
             if ctx.obj["VERBOSE"] == 2:  # product_stream X nvr x related_url x build_source_url
                 for pv in result_tree.keys():
                     for ps in result_tree[pv].keys():
                         for cn in result_tree[pv][ps].keys():
                             if not any([match in cn for match in exclude_components]):
                                 for nvr in result_tree[pv][ps][cn].keys():
@@ -413,15 +413,15 @@
                                             upstream_component_name = f"[cyan]{upstream_component_names[0]} and {len(upstream_component_names) - 1} more[/cyan]"  # noqa
                                         console.print(
                                             Text(ps, style="magenta b u"),
                                             upstream_component_name,
                                             dep,
                                             f"([grey]{related_url}[/grey])",
                                             f"([grey]{build_source_url}[/grey])",
-                                            no_wrap=False,
+                                            no_wrap=no_wrap,
                                         )
                                     source_component_names = list(
                                         set(
                                             [
                                                 source["name"]
                                                 for source in result_tree[pv][ps][cn][nvr][
                                                     "sources"
@@ -437,25 +437,25 @@
                                             source_component_name = f"[red]{source_component_names[0]} and {len(source_component_names) - 1} more[/red]"  # noqa
                                         console.print(
                                             Text(ps, style="magenta b u"),
                                             source_component_name,
                                             dep,
                                             f"([grey]{related_url}[/grey])",
                                             f"([grey]{build_source_url}[/grey])",
-                                            no_wrap=False,
+                                            no_wrap=no_wrap,
                                         )
                                     if (
                                         len(result_tree[pv][ps][cn][nvr]["upstreams"]) == 0
                                         and len(result_tree[pv][ps][cn][nvr]["sources"]) == 0
                                     ):
                                         console.print(
                                             Text(ps, style="magenta b u"),
                                             dep,
                                             f"([grey]{related_url}[/grey])",
-                                            no_wrap=False,
+                                            no_wrap=no_wrap,
                                         )
             if (
                 ctx.obj["VERBOSE"] == 3
             ):  # product_stream X nvr (full source/upstreams) x related_url x build_source_url
                 for pv in result_tree.keys():
                     for ps in result_tree[pv].keys():
                         for cn in result_tree[pv][ps].keys():
@@ -492,15 +492,15 @@
                                     for upstream_name in upstream_component_names:
                                         console.print(
                                             Text(ps, style="magenta b u"),
                                             f"[cyan]{upstream_name}[/cyan]",
                                             dep,
                                             f"([grey]{related_url}[/grey])",
                                             f"([grey]{build_source_url}[/grey])",
-                                            no_wrap=False,
+                                            no_wrap=no_wrap,
                                         )
                                     source_component_names = list(
                                         set(
                                             [
                                                 source["name"]
                                                 for source in result_tree[pv][ps][cn][nvr][
                                                     "sources"
@@ -511,26 +511,26 @@
                                     for source_name in source_component_names:
                                         console.print(
                                             Text(ps, style="magenta b u"),
                                             f"[light_blue]{source_name}[/light_blue]",
                                             dep,
                                             f"([grey]{related_url}[/grey])",
                                             f"([grey]{build_source_url}[/grey])",
-                                            no_wrap=False,
+                                            no_wrap=no_wrap,
                                         )
                                     if (
                                         not result_tree[pv][ps][cn][nvr]["upstreams"]
                                         and not result_tree[pv][ps][cn][nvr]["sources"]
                                     ):
                                         console.print(
                                             Text(ps, style="magenta b u"),
                                             dep,
                                             f"([grey]{related_url}[/grey])",
                                             f"([grey]{build_source_url}[/grey])",
-                                            no_wrap=False,
+                                            no_wrap=no_wrap,
                                         )
             if (
                 ctx.obj["VERBOSE"] > 3
             ):  # product_stream X nvr (full source/upstreams) x related_url x build_source_url
                 for pv in result_tree.keys():
                     for ps in result_tree[pv].keys():
                         for cn in result_tree[pv][ps].keys():
@@ -567,15 +567,15 @@
                                     for upstream_name in upstream_component_names:
                                         console.print(
                                             Text(ps, style="magenta b u"),
                                             f"[cyan]{upstream_name}[/cyan]",
                                             dep,
                                             f"([grey]{related_url}[/grey])",
                                             f"([grey]{build_source_url}[/grey])",
-                                            no_wrap=False,
+                                            no_wrap=no_wrap,
                                         )
                                     source_component_names = list(
                                         set(
                                             [
                                                 source["nvr"]
                                                 for source in result_tree[pv][ps][cn][nvr][
                                                     "sources"
@@ -586,32 +586,34 @@
                                     for source_name in source_component_names:
                                         console.print(
                                             Text(ps, style="magenta b u"),
                                             f"[light_blue]{source_name}[/light_blue]",
                                             dep,
                                             f"([grey]{related_url}[/grey])",
                                             f"([grey]{build_source_url}[/grey])",
-                                            no_wrap=False,
+                                            no_wrap=no_wrap,
                                         )
                                     if (
                                         not result_tree[pv][ps][cn][nvr]["upstreams"]
                                         and not result_tree[pv][ps][cn][nvr]["sources"]
                                     ):
                                         console.print(
                                             Text(ps, style="magenta b u"),
                                             dep,
                                             f"([grey]{related_url}[/grey])",
                                             f"([grey]{build_source_url}[/grey])",
-                                            no_wrap=False,
+                                            no_wrap=no_wrap,
                                         )
 
         ctx.exit()
 
 
-def text_output_components_contain_component(ctx, output, format, exclude_components):
+def text_output_components_contain_component(
+    ctx, output, format, exclude_components, no_wrap=False
+):
     if "results" in output:
         for item in output["results"]:
             component_name = item["name"]
             component_nvr = item["nvr"]
             related_url = item["related_url"]
             download_url = item["download_url"]
             arch = item["arch"]
@@ -634,15 +636,15 @@
                                 component_ns = Text(source_purl.namespace.upper(), style="bold red")
 
                             console.print(
                                 component_ns,
                                 source_purl.type.upper(),
                                 root_component,
                                 Text(component_name, style="bold white"),
-                                no_wrap=False,
+                                no_wrap=no_wrap,
                             )
                 if ctx.obj["VERBOSE"] == 1:
                     ordered_sources = sorted(item["sources"], key=lambda d: d["purl"])
                     for source in ordered_sources:
                         if "arch=noarch" in source["purl"] or "arch=src" in source["purl"]:
                             source_purl = PackageURL.from_string(source["purl"])
                             root_component = f"{source_purl.name}-{source_purl.version}"
@@ -658,15 +660,15 @@
                                 component_ns = Text(source_purl.namespace.upper(), style="bold red")
                             console.print(
                                 component_ns,
                                 source_purl.type.upper(),
                                 root_component,
                                 Text(component_nvr, style="bold white"),
                                 arch,
-                                no_wrap=False,
+                                no_wrap=no_wrap,
                             )
                 if ctx.obj["VERBOSE"] > 1:
                     ordered_sources = sorted(item["sources"], key=lambda d: d["purl"])
                     for source in ordered_sources:
                         if "arch=noarch" in source["purl"] or "arch=src" in source["purl"]:
                             source_purl = PackageURL.from_string(source["purl"])
                             root_component = f"{source_purl.name}-{source_purl.version}"
@@ -684,20 +686,20 @@
                                 component_ns,
                                 source_purl.type.upper(),
                                 root_component,
                                 Text(component_nvr, style="bold white"),
                                 arch,
                                 related_url,
                                 download_url,
-                                no_wrap=False,
+                                no_wrap=no_wrap,
                             )
     ctx.exit()
 
 
-def text_output_components_affected_by_cve(ctx, output, format):
+def text_output_components_affected_by_cve(ctx, output, format, no_wrap=False):
     console.print("Flaw Title:", output["title"])
     console.print(
         "affects:",
     )
     for component in output["components"]:
         affected_component1 = f"({component['purl']})"
         if not ctx.obj["SHOW_PURL"]:
@@ -708,81 +710,81 @@
             affected_component = f"([bold cyan]{ns}[/bold cyan] {purl.name}-{purl.version},{purl.type.upper()})"  # noqa
             versions = [pv["name"] for pv in component["product_versions"]]
             if ctx.obj["VERBOSE"] == 0:
                 console.print(
                     Text(str(versions), style="bold magenta u"),
                     ns,
                     affected_component,
-                    no_wrap=False,
+                    no_wrap=no_wrap,
                 )
             if ctx.obj["VERBOSE"] == 1:
                 console.print(
                     Text(component["product_streams"], style="bold magenta u"),
                     ns,
                     affected_component1,
-                    no_wrap=False,
+                    no_wrap=no_wrap,
                 )
             if ctx.obj["VERBOSE"] > 1:
                 console.print(
                     Text(component["product_streams"], style="bold magenta u"),
                     ns,
                     affected_component1,
                     Text(component["build_source_url"], style="i"),
                     Text(component["related_url"], style="i"),
                     Text(component["download_url"], style="i"),
-                    no_wrap=False,
+                    no_wrap=no_wrap,
                 )
     ctx.exit()
 
 
-def text_output_products_affected_by_cve(ctx, output, format, exclude_products):
+def text_output_products_affected_by_cve(ctx, output, format, exclude_products, no_wrap=False):
     console.print("[white]link:[/white]", output["link"])
     console.print("[white]cve_id:[/white]", output["cve_id"])
     console.print("[white]title:[/white]", output["title"])
     if ctx.obj["VERBOSE"] == 0:
         console.print(
             "[white]product_versions:[/white]",
         )
         ordered_product_versions = sorted(output["product_versions"])
         for product_version in ordered_product_versions:
-            console.print(Text(product_version, style="bold magenta u"), no_wrap=True)
+            console.print(Text(product_version, style="bold magenta u"), no_wrap=no_wrap)
     if ctx.obj["VERBOSE"] > 0:
         console.print(
             "[white]product_streams:[/white]",
         )
         ordered_product_streams = sorted(output["product_streams"])
         for product_stream in ordered_product_streams:
             console.print(Text(product_stream, style="bold magenta u"), no_wrap=True)
     ctx.exit()
 
 
-def text_output_get_manifest(ctx, output, format):
+def text_output_get_manifest(ctx, output, format, no_wrap=False):
     if not ctx.obj["SHOW_PURL"]:
         for component in output["packages"]:
             if "pkg:" in component["externalRefs"][0]["referenceLocator"]:
                 purl = PackageURL.from_string(component["externalRefs"][0]["referenceLocator"])
                 ns = "[cyan]UPSTREAM[/cyan]"
                 component = f"([bold turquoise2]{ns}[/bold turquoise2] [white]{purl.name}-{purl.version}[/white],{component_type_style(purl.type.upper())})"  # noqa
                 if purl.namespace == "redhat":
                     ns = f"[red]{purl.namespace.upper()}[/red]"
                     component = f"([white]{purl.name}-{purl.version}[/white],{component_type_style(purl.type.upper())})"  # noqa
                 else:
                     if purl.namespace:
                         ns = f"[white]{purl.namespace.upper()}[/white]"
                     component = f"([white]{purl.name}-{purl.version}[/white],{component_type_style(purl.type.upper())})"  # noqa
-                console.print(ns, component, no_wrap=False)  # noqa
+                console.print(ns, component, no_wrap=no_wrap)  # noqa
     else:
         for component in output["packages"]:
             purl = component["externalRefs"][0]["referenceLocator"]
-            console.print(purl, no_wrap=False)  # noqa
+            console.print(purl, no_wrap=no_wrap)  # noqa
 
     ctx.exit()
 
 
-def text_output_component_flaws(ctx, output, format):
+def text_output_component_flaws(ctx, output, format, no_wrap=False):
     ordered_components = sorted(output["results"], key=lambda d: d["name"])
     for item in ordered_components:
         component_name = item["name"]
         # sorting should work when there is no title or cve-id key
         ordered_affects = sorted(item["affects"], key=lambda d: d["flaw_cve_id"])
         for affect in ordered_affects:
             flaw_cve_id = "Vulnerability"
@@ -792,26 +794,26 @@
                 console.print(
                     Text(flaw_cve_id, style="magenta"),
                     Text(component_name, style="white"),
                     Text(affect["affect_product_version"], style="cyan"),
                     affect["affect_affectedness"],
                     affect["affect_impact"],
                     affect["affect_resolution"],
-                    no_wrap=True,
+                    no_wrap=no_wrap,
                 )
             if ctx.obj["VERBOSE"] == 1:
                 console.print(
                     Text(flaw_cve_id, style="magenta"),
                     Text(component_name, style="white"),
                     Text(affect["affect_product_version"], style="cyan"),
                     f"(state: {affect['flaw_state']} resolution:{affect['flaw_resolution']})",
                     affect["affect_affectedness"],
                     affect["affect_impact"],
                     affect["affect_resolution"],
-                    no_wrap=True,
+                    no_wrap=no_wrap,
                 )
             if ctx.obj["VERBOSE"] > 1:
                 console.print(Text(affect["title"], style="white"))
                 console.print(
                     Text(component_name, style="magenta"),
                     Text(affect["affect_product_version"], style="cyan"),
                     f"(state: {affect['flaw_state']} resolution:{affect['flaw_resolution']})",
@@ -819,58 +821,58 @@
                     affect["affect_impact"],
                     affect["affect_resolution"],
                     no_wrap=True,
                 )
     ctx.exit()
 
 
-def text_output_product_flaws(ctx, output, format):
+def text_output_product_flaws(ctx, output, format, no_wrap=False):
     for item in output["results"]:
         component_name = item["name"]
         for affect in item["affects"]:
             flaw_cve_id = "Vulnerability"
             if affect["flaw_cve_id"]:
                 flaw_cve_id = affect["flaw_cve_id"]
             if ctx.obj["VERBOSE"] == 0:
                 console.print(
                     Text(flaw_cve_id, style="magenta"),
                     Text(component_name, style="white"),
                     affect["affect_component_name"],
                     affect["affect_affectedness"],
                     affect["affect_impact"],
                     affect["affect_resolution"],
-                    no_wrap=True,
+                    no_wrap=no_wrap,
                 )
             if ctx.obj["VERBOSE"] == 1:
                 console.print(
                     Text(flaw_cve_id, style="magenta"),
                     Text(component_name, style="white"),
                     f"(state: {affect['flaw_state']} resolution:{affect['flaw_resolution']})",
                     affect["affect_component_name"],
                     affect["affect_affectedness"],
                     affect["affect_impact"],
                     affect["affect_resolution"],
-                    no_wrap=True,
+                    no_wrap=no_wrap,
                 )
             if ctx.obj["VERBOSE"] > 1:
                 console.print(affect["title"])
                 console.print(
                     Text(flaw_cve_id, style="magenta"),
                     Text(component_name, style="white"),
                     f"(state: {affect['flaw_state']} resolution:{affect['flaw_resolution']})",
                     affect["affect_component_name"],
                     affect["affect_affectedness"],
                     affect["affect_impact"],
                     affect["affect_resolution"],
-                    no_wrap=True,
+                    no_wrap=no_wrap,
                 )
     ctx.exit()
 
 
-def text_output_list(ctx, output, format, exclude_components):
+def text_output_list(ctx, output, format, exclude_components, no_wrap=False):
     if "results" in output and output["count"] > 0:
         # handle component
         if "purl" in output["results"][0]:
             ordered_components = sorted(output["results"], key=lambda d: d["name"])
             for row in ordered_components:
                 if not any([match in row["purl"] for match in exclude_components]):
                     if "purl" in row:
@@ -921,60 +923,60 @@
         if "cve_id" in output["results"][0]:
             for row in output["results"]:
                 console.print(
                     row["title"],
                     row["state"],
                     row["impact"],
                     row["resolution"],
-                    no_wrap=True,
+                    no_wrap=no_wrap,
                 )
 
         # handle trackers
         if "external_system_id" in output["results"][0]:
             for row in output["results"]:
                 console.print(
                     row["external_system_id"],
                     row["type"],
                     row["status"],
-                    no_wrap=True,
+                    no_wrap=no_wrap,
                 )
 
         # handle products
         if "ofuri" in output["results"][0]:
             for row in output["results"]:
                 console.print(
                     Text(row["name"], style="magenta bold u"),
                     row["ofuri"],
-                    no_wrap=True,
+                    no_wrap=no_wrap,
                 )
         # handle channels
         if "relative_url" in output["results"][0]:
             for row in output["results"]:
                 console.print(
                     Text(row["name"], style="magenta bold u"),
                     row["type"],
                     row["description"],
-                    no_wrap=True,
+                    no_wrap=no_wrap,
                 )
         # handle builds
         if "build_id" in output["results"][0]:
             for row in output["results"]:
                 console.print(
                     Text(str(row["build_id"]), style="magenta bold u"),
                     row["build_type"],
                     Text(row["name"], style="white"),
                     row["created_at"],
                     Text(row["link"], style="i"),
-                    no_wrap=False,
+                    no_wrap=no_wrap,
                 )
 
     ctx.exit()
 
 
-def text_output_purls(ctx, output, format):
+def text_output_purls(ctx, output, format, no_wrap=False):
     if "results" in output and output["count"] > 0:
         # handle component
         if "purl" in output["results"][0]:
             ordered_components = sorted(output["results"], key=lambda d: d["purl"])
             for row in ordered_components:
                 if "purl" in row:
                     purl = PackageURL.from_string(row["purl"])
@@ -985,34 +987,34 @@
                     if ctx.obj["VERBOSE"] == 0:
                         console.print(
                             component_ns,
                             purl.type.upper(),
                             Text(purl.name, style="bold white"),
                             purl.version,
                             purl.qualifiers.get("arch"),
-                            no_wrap=False,
+                            no_wrap=no_wrap,
                         )
                     if ctx.obj["VERBOSE"] > 0:
                         console.print(
                             component_ns,
                             purl.type.upper(),
                             Text(purl.name, style="bold white"),
                             purl.version,
                             purl.qualifiers.get("arch"),
                             row["link"],
-                            no_wrap=False,
+                            no_wrap=no_wrap,
                         )
         ctx.exit()
 
 
-def text_output_generic(ctx, output, format):
+def text_output_generic(ctx, output, format, no_wrap=False):
     for k, v in output.items():
         key_name = Text(k)
         key_name.stylize("bold magenta")
-        console.print(key_name, " : ", v, no_wrap=True)
+        console.print(key_name, " : ", v, no_wrap=no_wrap)
 
 
 def cprint(
     data,
     dest=DEST.CONSOLE,
     filename=None,
     ctx=None,
@@ -1034,43 +1036,48 @@
     output = raw_json_transform(data, show_count)
     if ctx and ctx.obj["NO_COLOR"]:
         console.no_color = True
     format = OUTPUT_FORMAT.JSON
     if ctx and "FORMAT" in ctx.obj:
         format = OUTPUT_FORMAT(ctx.obj["FORMAT"])
     if format is OUTPUT_FORMAT.TEXT:
+        no_wrap = ctx.obj["NO_WRAP"]
         if ctx.info_name == "product-summary":
-            text_output_product_summary(ctx, output, format, exclude_products)
+            text_output_product_summary(ctx, output, format, exclude_products, no_wrap=no_wrap)
         if ctx.info_name == "products-contain-component":
             text_output_products_contain_component(
-                ctx, output, exclude_products, exclude_components
+                ctx, output, exclude_products, exclude_components, no_wrap=no_wrap
             )
         if ctx.info_name == "components-contain-component":
-            text_output_components_contain_component(ctx, output, format, exclude_components)
+            text_output_components_contain_component(
+                ctx, output, format, exclude_components, no_wrap=no_wrap
+            )
         if ctx.info_name == "components-affected-by-flaw":
-            text_output_components_affected_by_cve(ctx, output, format)
+            text_output_components_affected_by_cve(ctx, output, format, no_wrap=no_wrap)
         if ctx.info_name == "products-affected-by-flaw":
-            text_output_products_affected_by_cve(ctx, output, format, exclude_products)
+            text_output_products_affected_by_cve(
+                ctx, output, format, exclude_products, no_wrap=no_wrap
+            )
         if ctx.info_name == "get-manifest":
-            text_output_get_manifest(ctx, output, format)
+            text_output_get_manifest(ctx, output, format, no_wrap=no_wrap)
         if ctx.info_name == "list":
-            text_output_list(ctx, output, format, exclude_components)
+            text_output_list(ctx, output, format, exclude_components, no_wrap=no_wrap)
         if ctx.info_name == "component-flaws":
-            text_output_component_flaws(ctx, output, format)
+            text_output_component_flaws(ctx, output, format, no_wrap=no_wrap)
         if ctx.info_name == "product-flaws":
-            text_output_product_flaws(ctx, output, format)
+            text_output_product_flaws(ctx, output, format, no_wrap=no_wrap)
         if ctx.info_name == "provides":
-            text_output_purls(ctx, output, format)
+            text_output_purls(ctx, output, format, no_wrap=no_wrap)
         if ctx.info_name == "sources":
-            text_output_purls(ctx, output, format)
+            text_output_purls(ctx, output, format, no_wrap=no_wrap)
         if ctx.info_name == "tree":
-            text_output_tree(ctx, output)
+            text_output_tree(ctx, output, no_wrap=no_wrap)
 
         # last chance text formatted output
-        text_output_generic(ctx, output, format)
+        text_output_generic(ctx, output, format, no_wrap=no_wrap)
 
     if format is OUTPUT_FORMAT.JSON:
         if dest is DEST.CONSOLE:
             console.print_json(json.dumps(output))
 
     # if we instructed to open browser, open that up now
     if ctx:
```

### Comparing `griffon-0.2.3/griffon/services/__init__.py` & `griffon-0.2.4/griffon/services/__init__.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/griffon/services/core_process.py` & `griffon-0.2.4/griffon/services/core_process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/griffon/services/core_queries.py` & `griffon-0.2.4/griffon/services/core_queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,26 +69,29 @@
                     # "build_count": ps.build_count,
                     "manifest_link": ps.manifest,
                     "latest_components_link": f"{CORGI_API_URL}/api/v1/components?ofuri={ps.ofuri}&view=summary",  # noqa
                     "all_components_link": f"{CORGI_API_URL}/api/v1/components?product_streams={ps.ofuri}&include_fields=link,name,purl",  # noqa
                 }
                 results.append(result)
         else:
-            result = {
-                "link": product_streams["link"],
-                "ofuri": product_streams["ofuri"],
-                "name": product_streams["name"],
-                "product": product_streams["products"][0]["name"],
-                "product_version": product_streams["product_versions"][0]["name"],
-                "brew_tags": "",
-                "manifest_link": product_streams["manifest"],
-                "latest_components_link": f"{CORGI_API_URL}/api/v1/components?ofuri={product_streams['ofuri']}&view=summary",  # noqa
-                "all_components_link": f"{CORGI_API_URL}/api/v1/components?product_streams={product_streams['ofuri']}&include_fields=link,name,purl",  # noqa
-            }
-            results.append(result)
+            if "ofuri" in product_streams:
+                result = {
+                    "link": product_streams["link"],
+                    "ofuri": product_streams["ofuri"],
+                    "name": product_streams["name"],
+                    "product": product_streams["products"][0]["name"],
+                    "product_version": product_streams["product_versions"][0]["name"],
+                    "brew_tags": "",
+                    "manifest_link": product_streams["manifest"],
+                    "latest_components_link": f"{CORGI_API_URL}/api/v1/components?ofuri={product_streams['ofuri']}&view=summary",  # noqa
+                    "all_components_link": f"{CORGI_API_URL}/api/v1/components?product_streams={product_streams['ofuri']}&include_fields=link,name,purl",  # noqa
+                }
+                results.append(result)
+            else:
+                logger.warning("No such product stream")
         return results
 
 
 class products_versions_affected_by_specific_cve_query:
     """Given a specific CVE ID, what products are affected?"""
 
     name = "product-versions-affected-by-specific-cve"
```

### Comparing `griffon-0.2.3/griffon/services/core_reports.py` & `griffon-0.2.4/griffon/services/core_reports.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/griffon/static/default_griffonrc` & `griffon-0.2.4/griffon/static/default_griffonrc`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [default]
 format = text
 history_log = ~/.griffon/history.log
 profile = default
 verbosity = 0
+no_wrap = True
 sfm2_api_url = http://localhost:5600
 custom_plugin_dir = ~/.griffon/plugins/
 editor = vi
 exclude_components = -container-source
     -debuginfo
     -debugsource
     -static
```

### Comparing `griffon-0.2.3/griffon.egg-info/PKG-INFO` & `griffon-0.2.4/griffon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griffon
-Version: 0.2.3
+Version: 0.2.4
 Summary: Red Hat Product Security CLI
 Home-page: https://github.com/RedHatProductSecurity/griffon
 Author: James Fuller, Red Hat Product Security
 License: MIT
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `griffon-0.2.3/griffon.egg-info/SOURCES.txt` & `griffon-0.2.4/griffon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/pyproject.toml` & `griffon-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/setup.py` & `griffon-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/tests/test_cli.py` & `griffon-0.2.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/tests/test_entities.py` & `griffon-0.2.4/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/tests/test_manage.py` & `griffon-0.2.4/tests/test_manage.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/tests/test_plugins.py` & `griffon-0.2.4/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/tests/test_process.py` & `griffon-0.2.4/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/tests/test_queries.py` & `griffon-0.2.4/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/tests/test_reports.py` & `griffon-0.2.4/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.3/tests/test_unit.py` & `griffon-0.2.4/tests/test_unit.py`

 * *Files identical despite different names*

