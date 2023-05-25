# Comparing `tmp/bowtie_json_schema-2023.5.8.tar.gz` & `tmp/bowtie_json_schema-2023.5.9.tar.gz`

## Comparing `bowtie_json_schema-2023.5.8.tar` & `bowtie_json_schema-2023.5.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/.flake8
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/.readthedocs.yml
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/action.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/io-schema.json -> bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/noxfile.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/test-requirements.in
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/test-requirements.txt
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/.github/SECURITY.md
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/.github/release.yml
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/.github/workflows/ci.yml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/.github/workflows/dependabot-merge.yml
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/.github/workflows/images.yml
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/.github/workflows/report.yml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/bowtie/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/bowtie/__main__.py
--rw-r--r--   0        0        0    30648 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/bowtie/_cli.py
--rw-r--r--   0        0        0     8501 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/bowtie/_commands.py
--rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/bowtie/_core.py
--rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/bowtie/_report.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/bowtie/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/bowtie/schemas/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/docs/Makefile
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/docs/cli.rst
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/docs/conf.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/docs/contributing.rst
--rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/docs/implementers.rst
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/docs/index.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/docs/requirements.in
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/docs/requirements.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/docs/_static/dreamed.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/tests/conftest.py
--rw-r--r--   0        0        0    22418 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/tests/test_integration.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/tests/fauxmplementations/badsonschema/Dockerfile
--rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/tests/fauxmplementations/badsonschema/badsonschema
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/tests/fauxmplementations/lintsonschema/Dockerfile
--rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/tests/fauxmplementations/lintsonschema/io-schema.json
--rwxr-xr-x   0        0        0     2890 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/bowtie/templates/report.html.j2
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/LICENSE
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/README.rst
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/pyproject.toml
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.8/PKG-INFO
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.flake8
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.readthedocs.yml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/action.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/io-schema.json -> bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/noxfile.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/test-requirements.in
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/test-requirements.txt
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.github/SECURITY.md
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.github/release.yml
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.github/workflows/dependabot-merge.yml
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.github/workflows/images.yml
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.github/workflows/report.yml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/bowtie/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/bowtie/__main__.py
+-rw-r--r--   0        0        0    31313 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/bowtie/_cli.py
+-rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/bowtie/_commands.py
+-rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/bowtie/_core.py
+-rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/bowtie/_report.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/bowtie/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/bowtie/schemas/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/docs/Makefile
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/docs/cli.rst
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/docs/conf.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/docs/contributing.rst
+-rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/docs/implementers.rst
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/docs/index.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/docs/requirements.in
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/docs/requirements.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/docs/_static/dreamed.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/tests/conftest.py
+-rw-r--r--   0        0        0    23967 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/tests/test_integration.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/tests/fauxmplementations/badsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/tests/fauxmplementations/badsonschema/badsonschema
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/tests/fauxmplementations/lintsonschema/Dockerfile
+-rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/tests/fauxmplementations/lintsonschema/io-schema.json
+-rwxr-xr-x   0        0        0     2890 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/bowtie/templates/report.html.j2
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/LICENSE
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/README.rst
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/pyproject.toml
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.9/PKG-INFO
```

### Comparing `bowtie_json_schema-2023.5.8/.flake8` & `bowtie_json_schema-2023.5.9/.flake8`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/.pre-commit-config.yaml` & `bowtie_json_schema-2023.5.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/noxfile.py` & `bowtie_json_schema-2023.5.9/noxfile.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/test-requirements.txt` & `bowtie_json_schema-2023.5.9/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/.github/SECURITY.md` & `bowtie_json_schema-2023.5.9/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/.github/dependabot.yml` & `bowtie_json_schema-2023.5.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/.github/workflows/ci.yml` & `bowtie_json_schema-2023.5.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/.github/workflows/dependabot-merge.yml` & `bowtie_json_schema-2023.5.9/.github/workflows/dependabot-merge.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/.github/workflows/images.yml` & `bowtie_json_schema-2023.5.9/.github/workflows/images.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/.github/workflows/report.yml` & `bowtie_json_schema-2023.5.9/.github/workflows/report.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/bowtie/_cli.py` & `bowtie_json_schema-2023.5.9/bowtie/_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from collections.abc import Awaitable, Callable, Iterable
 from contextlib import AsyncExitStack, asynccontextmanager
 from fnmatch import fnmatch
 from io import BytesIO
 from pathlib import Path
-from typing import Any, TextIO, Union
+from typing import Any, AsyncIterator, TextIO, Union
 from urllib.parse import urljoin
 import asyncio
 import json
 import os
 import sys
 import zipfile
 
@@ -72,14 +72,24 @@
     "draft3": DRAFT3,
 }
 LATEST_DIALECT_NAME = "draft2020-12"
 
 #: Should match the magic value used to validate `schema`s in `io-schema.json`
 CURRENT_DIALECT_URI = "urn:current-dialect"
 
+FORMAT = click.option(
+    "--format",
+    "-f",
+    "format",
+    help="What format to use for the output",
+    default=lambda: "pretty" if sys.stdout.isatty() else "json",
+    show_default="pretty if stdout is a tty, otherwise JSON",
+    type=click.Choice(["json", "pretty"]),
+)
+
 
 @click.group(context_settings=dict(help_option_names=["--help", "-h"]))
 @click.version_option(prog_name="bowtie", package_name="bowtie-json-schema")
 def main():
     """
     A meta-validator for the JSON Schema specifications.
     """
@@ -132,22 +142,15 @@
         dialect = report_data["run_info"].dialect
         report_data["summary"].generate_badges(badges, dialect)
     template = env.get_template("report.html.j2")
     output.write(template.render(**report_data))
 
 
 @main.command()
-@click.option(
-    "--format",
-    "-f",
-    help="What format to use for the output",
-    default=lambda: "pretty" if sys.stdout.isatty() else "json",
-    show_default="pretty if stdout is a tty, otherwise JSON",
-    type=click.Choice(["json", "pretty"]),
-)
+@FORMAT
 @click.option(
     "--show",
     "-s",
     help="""Configure whether to display validation results
     (whether instances are valid or not) or test failure results
     (whether the validation results match expected validation results)""",
     default="validation",
@@ -449,23 +452,16 @@
     )
     exit_code = asyncio.run(_run(fail_fast=False, **kwargs, cases=[case]))
     context.exit(exit_code)
 
 
 @main.command()
 @click.pass_context
+@FORMAT
 @IMPLEMENTATION
-@click.option(
-    "--format",
-    "-f",
-    help="What format to use for the output",
-    default=lambda: "pretty" if sys.stdout.isatty() else "json",
-    show_default="pretty if stdout is a tty, otherwise JSON",
-    type=click.Choice(["json", "pretty"]),
-)
 def info(context: click.Context, **kwargs: Any):
     """
     Retrieve a particular implementation (harness)'s metadata.
     """
     exit_code = asyncio.run(_info(**kwargs))
     context.exit(exit_code)
 
@@ -515,45 +511,47 @@
                     ),
                 )
     return exit_code
 
 
 @main.command()
 @click.pass_context
+@FORMAT
 @IMPLEMENTATION
 def smoke(context: click.Context, **kwargs: Any):
     """
     Smoke test one or more implementations for basic correctness.
     """
     exit_code = asyncio.run(_smoke(**kwargs))
     context.exit(exit_code)
 
 
-async def _smoke(image_names: list[str]):
+async def _smoke(image_names: list[str], format: str):
     exit_code = 0
     async with _start(
         image_names=image_names,
         make_validator=validator_for_dialect,
         reporter=_report.Reporter(),
     ) as starting:
         for each in asyncio.as_completed(starting):
             try:
                 implementation = await each
             except NoSuchImage as error:
                 exit_code |= os.EX_CONFIG
                 click.echo(
                     f"❗ (error): {error.name!r} is not a known Bowtie implementation.",  # noqa: E501
+                    file=sys.stderr,
                 )
                 continue
 
-            click.echo(f"Testing {implementation.name!r}...")
+            click.echo(f"Testing {implementation.name!r}...", file=sys.stderr)
 
             if implementation.metadata is None:
                 exit_code |= os.EX_CONFIG
-                click.echo("  ❗ (error): startup failed")
+                click.echo("  ❗ (error): startup failed", file=sys.stderr)
                 continue
 
             dialect = implementation.dialects[0]
             runner = await implementation.start_speaking(dialect)
 
             cases = [
                 TestCase(
@@ -568,30 +566,47 @@
                     description="allow-nothing schema",
                     schema={"$schema": dialect, "not": {}},
                     tests=[
                         Test(description="First", instance=12, valid=False),
                     ],
                 ),
             ]
-            for seq, case in enumerate(cases):
-                response = await runner.run_case(seq=seq, case=case)
-                if response.errored:  # type: ignore[reportGeneralTypeIssues]  # noqa: E501
-                    exit_code |= os.EX_DATAERR
-                    message = "❗ (error)"
-                elif response.failed:  # type: ignore[reportGeneralTypeIssues]  # noqa: E501
-                    exit_code |= os.EX_DATAERR
-                    message = "✗ (failed)"
-                else:
-                    message = "✓"
-                click.echo(f"  {message}: {case.description}")
+            responses: AsyncIterator[tuple[TestCase, ReportableResult]] = (  # type: ignore[reportGeneralTypeIssues]  # noqa: E501
+                (case, await runner.run_case(seq=seq, case=case))
+                for seq, case in enumerate(cases)
+            )
+
+            if format == "json":
+                serializable = [
+                    {
+                        "case": case.without_expected_results(),
+                        "response": dict(
+                            errored=response.errored,
+                            failed=response.failed,
+                        ),
+                    }
+                    async for case, response in responses
+                ]
+                click.echo(json.dumps(serializable, indent=2))
+            else:
+                async for case, response in responses:
+                    if response.errored:  # type: ignore[reportGeneralTypeIssues]  # noqa: E501
+                        exit_code |= os.EX_DATAERR
+                        message = "❗ (error)"
+                    elif response.failed:  # type: ignore[reportGeneralTypeIssues]  # noqa: E501
+                        exit_code |= os.EX_DATAERR
+                        message = "✗ (failed)"
+                    else:
+                        message = "✓"
+                    click.echo(f"  {message}: {case.description}")
 
     if exit_code:
-        click.echo("\n❌ some failures")
+        click.echo("\n❌ some failures", file=sys.stderr)
     else:
-        click.echo("\n✅ all passed")
+        click.echo("\n✅ all passed", file=sys.stderr)
 
     return exit_code
 
 
 class _TestSuiteCases(click.ParamType):
     name = "json-schema-org/JSON-Schema-Test-Suite test cases"
```

### Comparing `bowtie_json_schema-2023.5.8/bowtie/_commands.py` & `bowtie_json_schema-2023.5.9/bowtie/_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,14 +239,15 @@
         if message:
             return message
         return "Encountered an error."
 
 
 class ReportableResult(Protocol):
     errored: bool
+    failed: bool
 
     def report(self, reporter: _report._CaseReporter) -> None:  # type: ignore[reportPrivateUsage]  # noqa: E501
         pass
 
 
 @frozen
 class CaseResult:
@@ -283,15 +284,20 @@
                 and expected != test.valid  # type: ignore[reportUnknownMemberType]  # noqa: E501
             )
             yield test, failed
 
 
 @frozen
 class CaseErrored:
+    """
+    A full test case errored.
+    """
+
     errored = True
+    failed = False
 
     implementation: str
     seq: int
     context: dict[str, Any]
 
     caught: bool = True
 
@@ -311,15 +317,20 @@
             caught=False,
             context=context,
         )
 
 
 @frozen
 class CaseSkipped:
+    """
+    A full test case was skipped.
+    """
+
     errored = False
+    failed = False
 
     implementation: str
     seq: int
 
     message: str | None = None
     issue_url: str | None = None
     skipped: bool = field(init=False, default=True)
@@ -331,14 +342,15 @@
 @frozen
 class Empty:
     """
     An implementation didn't send a response.
     """
 
     errored = True
+    failed = False
 
     implementation: str
 
     def report(self, reporter: _report._CaseReporter):  # type: ignore[reportPrivateUsage]  # noqa: E501
         reporter.no_response(implementation=self.implementation)
```

### Comparing `bowtie_json_schema-2023.5.8/bowtie/_core.py` & `bowtie_json_schema-2023.5.9/bowtie/_core.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/bowtie/_report.py` & `bowtie_json_schema-2023.5.9/bowtie/_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/bowtie/exceptions.py` & `bowtie_json_schema-2023.5.9/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/docs/Makefile` & `bowtie_json_schema-2023.5.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/docs/cli.rst` & `bowtie_json_schema-2023.5.9/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/docs/conf.py` & `bowtie_json_schema-2023.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/docs/contributing.rst` & `bowtie_json_schema-2023.5.9/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/docs/implementers.rst` & `bowtie_json_schema-2023.5.9/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/docs/index.rst` & `bowtie_json_schema-2023.5.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/docs/requirements.txt` & `bowtie_json_schema-2023.5.9/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/docs/_static/dreamed.png` & `bowtie_json_schema-2023.5.9/docs/_static/dreamed.png`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/tests/test_integration.py` & `bowtie_json_schema-2023.5.9/tests/test_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -408,32 +408,80 @@
 
     assert results == [[{"valid": True}]], stderr
     assert stderr != ""
     assert returncode == 0, stderr
 
 
 @pytest.mark.asyncio
-async def test_smoke(envsonschema):
+async def test_smoke_pretty(envsonschema):
     proc = await asyncio.create_subprocess_exec(
         sys.executable,
         "-m",
         "bowtie",
         "smoke",
+        "--format",
+        "pretty",
         "-i",
         envsonschema,
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.PIPE,
     )
     _, _ = await proc.communicate()
     # FIXME: This != 0 is because indeed envsonschema gets answers wrong
     #        Change to asserting about the smoke stdout once that's there.
     assert proc.returncode != 0
 
 
 @pytest.mark.asyncio
+async def test_smoke_json(envsonschema):
+    proc = await asyncio.create_subprocess_exec(
+        sys.executable,
+        "-m",
+        "bowtie",
+        "smoke",
+        "--format",
+        "json",
+        "-i",
+        envsonschema,
+        stdout=asyncio.subprocess.PIPE,
+        stderr=asyncio.subprocess.PIPE,
+    )
+    stdout, stderr = await proc.communicate()
+    # FIXME: This != 0 is because indeed envsonschema gets answers wrong
+    #        Change to asserting about the smoke stdout once that's there.
+    assert proc.returncode == 0, (stdout, stderr)
+    assert json.loads(stdout) == [
+        {
+            "case": {
+                "description": "allow-everything schema",
+                "schema": {
+                    "$schema": "https://json-schema.org/draft/2020-12/schema",
+                },
+                "tests": [
+                    {"description": "First", "instance": 1},
+                    {"description": "Second", "instance": "foo"},
+                ],
+            },
+            "response": {"errored": False, "failed": True},
+        },
+        {
+            "case": {
+                "description": "allow-nothing schema",
+                "schema": {
+                    "$schema": "https://json-schema.org/draft/2020-12/schema",
+                    "not": {},
+                },
+                "tests": [{"description": "First", "instance": 12}],
+            },
+            "response": {"errored": False, "failed": False},
+        },
+    ]
+
+
+@pytest.mark.asyncio
 async def test_info_pretty(envsonschema):
     proc = await asyncio.create_subprocess_exec(
         sys.executable,
         "-m",
         "bowtie",
         "info",
         "--format",
@@ -672,15 +720,15 @@
         "no-such-image",
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.PIPE,
     )
     stdout, stderr = await proc.communicate()
     assert (
         b"'ghcr.io/bowtie-json-schema/no-such-image' is not a known Bowtie implementation.\n"  # noqa: E501
-        in stdout
+        in stderr
     )
     assert proc.returncode != 0
 
     proc = await asyncio.create_subprocess_exec(
         sys.executable,
         "-m",
         "bowtie",
```

### Comparing `bowtie_json_schema-2023.5.8/tests/fauxmplementations/badsonschema/badsonschema` & `bowtie_json_schema-2023.5.9/tests/fauxmplementations/badsonschema/badsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2023.5.9/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/tests/fauxmplementations/lintsonschema/io-schema.json` & `bowtie_json_schema-2023.5.9/tests/fauxmplementations/lintsonschema/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2023.5.9/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/bowtie/templates/report.html.j2` & `bowtie_json_schema-2023.5.9/bowtie/templates/report.html.j2`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/bowtie/schemas/io-schema.json` & `bowtie_json_schema-2023.5.9/bowtie/schemas/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/.gitignore` & `bowtie_json_schema-2023.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/LICENSE` & `bowtie_json_schema-2023.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/README.rst` & `bowtie_json_schema-2023.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/pyproject.toml` & `bowtie_json_schema-2023.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.8/PKG-INFO` & `bowtie_json_schema-2023.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bowtie-json-schema
-Version: 2023.5.8
+Version: 2023.5.9
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://bowtie-json-schema.readthedocs.io/
 Project-URL: Homepage, https://github.com/bowtie-json-schema/bowtie
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author: Julian Berman
 Author-email: Julian+bowtie@GrayVines.com
```

