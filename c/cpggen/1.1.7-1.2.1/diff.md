# Comparing `tmp/cpggen-1.1.7.tar.gz` & `tmp/cpggen-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-1.1.7.tar", max compression
+gzip compressed data, was "cpggen-1.2.1.tar", max compression
```

## Comparing `cpggen-1.1.7.tar` & `cpggen-1.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-05-23 19:15:31.782543 cpggen-1.1.7/LICENSE
--rw-r--r--   0        0        0    12901 2023-05-23 19:15:31.782543 cpggen-1.1.7/README.md
--rw-r--r--   0        0        0        0 2023-05-23 19:15:31.782543 cpggen-1.1.7/cpggen/__init__.py
--rw-r--r--   0        0        0    21095 2023-05-23 19:15:31.782543 cpggen-1.1.7/cpggen/cli.py
--rw-r--r--   0        0        0    41249 2023-05-23 19:15:31.782543 cpggen-1.1.7/cpggen/executor.py
--rw-r--r--   0        0        0     1079 2023-05-23 19:15:31.782543 cpggen-1.1.7/cpggen/logger.py
--rw-r--r--   0        0        0        0 2023-05-23 19:15:31.782543 cpggen-1.1.7/cpggen/source/__init__.py
--rw-r--r--   0        0        0     4001 2023-05-23 19:15:31.782543 cpggen-1.1.7/cpggen/source/ghsa.py
--rw-r--r--   0        0        0    18139 2023-05-23 19:15:31.782543 cpggen-1.1.7/cpggen/utils.py
--rw-r--r--   0        0        0     1363 2023-05-23 19:15:31.786543 cpggen-1.1.7/pyproject.toml
--rw-r--r--   0        0        0    14172 1970-01-01 00:00:00.000000 cpggen-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-25 00:12:42.173056 cpggen-1.2.1/LICENSE
+-rw-r--r--   0        0        0    13160 2023-05-25 00:12:42.173056 cpggen-1.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-25 00:12:42.177056 cpggen-1.2.1/cpggen/__init__.py
+-rw-r--r--   0        0        0    21260 2023-05-25 00:12:42.177056 cpggen-1.2.1/cpggen/cli.py
+-rw-r--r--   0        0        0    42470 2023-05-25 00:12:42.177056 cpggen-1.2.1/cpggen/executor.py
+-rw-r--r--   0        0        0     1079 2023-05-25 00:12:42.177056 cpggen-1.2.1/cpggen/logger.py
+-rw-r--r--   0        0        0        0 2023-05-25 00:12:42.177056 cpggen-1.2.1/cpggen/source/__init__.py
+-rw-r--r--   0        0        0     4002 2023-05-25 00:12:42.177056 cpggen-1.2.1/cpggen/source/ghsa.py
+-rw-r--r--   0        0        0    18139 2023-05-25 00:12:42.177056 cpggen-1.2.1/cpggen/utils.py
+-rw-r--r--   0        0        0     1363 2023-05-25 00:12:42.177056 cpggen-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    14431 1970-01-01 00:00:00.000000 cpggen-1.2.1/PKG-INFO
```

### Comparing `cpggen-1.1.7/LICENSE` & `cpggen-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-1.1.7/README.md` & `cpggen-1.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 [![Discord](https://img.shields.io/badge/-Discord-lime?style=for-the-badge&logo=discord&logoColor=white&color=black)](https://discord.gg/tmmtjCEHNV)
 
 ## Pre-requisites
 
 - JDK 11 or above
 - Python 3.10
 - Docker or podman (Windows, Linux or Mac) or
-- Joern [natively installed](https://docs.joern.io/installation) (Linux only)
+- [Atom](https://github.com/AppThreat/atom#installation) or [Joern](https://docs.joern.io/installation)
 
 ## Installation
 
 cpggen is available as a single executable binary, [PyPI package](https://pypi.org/project/cpggen/) or as a [container image](https://github.com/AppThreat/cpggen/pkgs/container/cpggen).
 
 ### Single executable binaries
 
@@ -36,14 +36,22 @@
 
 ```bash
 curl -LO https://github.com/AppThreat/cpggen/releases/latest/download/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
+OSS version without any Qwiet.AI binary frontends.
+
+```bash
+curl -LO https://github.com/AppThreat/cpggen/releases/latest/download/cpggen-oss-linux-amd64
+chmod +x cpggen-oss-linux-amd64
+./cpggen-oss-linux-amd64 --help
+```
+
 On Windows,
 
 ```powershell
 curl -LO https://github.com/appthreat/cpggen/releases/latest/download/cpggen.exe
 .\cpggen.exe --help
 ```
 
@@ -285,15 +293,15 @@
   --export-out-dir EXPORT_OUT_DIR
                         Export output directory
   --verbose             Run cpggen in verbose mode
   --skip-sbom           Do not generate SBoM
   --slice               Extract intra-procedural slices from the CPG
   --slice-mode {Usages,DataFlow}
                         Mode used for CPG slicing
-  --use-parse           Use joern-parse command instead of invoking the language frontends. Useful when default overlays are important
+  --use-atom            Use atom toolkit
   --vectors             Extract vector representations of code from CPG
 ```
 
 ## Environment variables
 
 | Name                    | Purpose                                                                    |
 | ----------------------- | -------------------------------------------------------------------------- |
@@ -311,14 +319,15 @@
 | CPG_SLICE_MODE          | Slice mode. Default Usages                                                 |
 | CPG_VECTORS             | Set to true to generate vector representations of code from CPG            |
 | SHIFTLEFT_ACCESS_TOKEN  | Set to automatically submit the CPG for analysis by Qwiet AI               |
 | CDXGEN_ARGS             | Extra arguments to pass to cdxgen                                          |
 | ENABLE_SBOM             | Enable SBoM generation using cdxgen                                        |
 | JIMPLE_ANDROID_JAR      | Path to android.jar for use with jimple for .apk or .dex to CPG conversion |
 | GITHUB_TOKEN            | Token with read:packages scope to analyze CVE or GitHub Advisory           |
+| USE_ATOM                | Use AppThreat atom instead of joern frontends                              |
 
 ## GitHub actions
 
 Use the marketplace [action](https://github.com/marketplace/actions/cpggen) to generate CPGs using GitHub actions. Optionally, the upload the generated CPGs as build artifacts use the below step.
 
 ```
 - name: Upload cpg
```

### Comparing `cpggen-1.1.7/cpggen/cli.py` & `cpggen-1.2.1/cpggen/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,23 @@
 ██╔════╝██╔══██╗██╔════╝
 ██║     ██████╔╝██║  ███╗
 ██║     ██╔═══╝ ██║   ██║
 ╚██████╗██║     ╚██████╔╝
  ╚═════╝╚═╝      ╚═════╝
 """
 
+ATOM_LOGO = """
+ █████╗ ████████╗ ██████╗ ███╗   ███╗
+██╔══██╗╚══██╔══╝██╔═══██╗████╗ ████║
+███████║   ██║   ██║   ██║██╔████╔██║
+██╔══██║   ██║   ██║   ██║██║╚██╔╝██║
+██║  ██║   ██║   ╚██████╔╝██║ ╚═╝ ██║
+╚═╝  ╚═╝   ╚═╝    ╚═════╝ ╚═╝     ╚═╝
+"""
+
 app = Quart(__name__)
 app.config.from_prefixed_env()
 
 
 def build_args():
     """
     Constructs command line arguments for the scanner
@@ -61,20 +70,16 @@
         default=False,
     )
     parser.add_argument(
         "--build",
         dest="auto_build",
         help="Attempt to build the project automatically",
         action="store_true",
-        default=True
-        if (
-            os.getenv("AUTO_BUILD") in ("true", "1")
-            or os.getenv("SHIFTLEFT_ACCESS_TOKEN")
-        )
-        else False,
+        default=os.getenv("AUTO_BUILD") in ("true", "1")
+        or os.getenv("SHIFTLEFT_ACCESS_TOKEN"),
     )
     parser.add_argument(
         "--joern-home",
         dest="joern_home",
         help="Joern installation directory",
         default=os.getenv(
             "JOERN_HOME", str(Path.home() / "bin" / "joern" / "joern-cli")
@@ -98,15 +103,15 @@
         default=os.getenv("CPGGEN_PORT", "7072"),
         dest="server_port",
         help="cpggen server port",
     )
     parser.add_argument(
         "--export",
         action="store_true",
-        default=True if os.getenv("CPG_EXPORT") in ("true", "1") else False,
+        default=os.getenv("CPG_EXPORT") in ("true", "1"),
         dest="export",
         help="Export CPG as a graph",
     )
     parser.add_argument(
         "--export-repr",
         default=os.getenv("CPG_EXPORT_REPR", "cpg14"),
         dest="export_repr",
@@ -131,66 +136,63 @@
         default=False,
         dest="verbose_mode",
         help="Run cpggen in verbose mode",
     )
     parser.add_argument(
         "--skip-sbom",
         action="store_true",
-        default=True
-        if not os.getenv("SHIFTLEFT_ACCESS_TOKEN") and not os.getenv("ENABLE_SBOM")
-        else False,
+        default=not os.getenv("SHIFTLEFT_ACCESS_TOKEN")
+        and not os.getenv("ENABLE_SBOM"),
         dest="skip_sbom",
         help="Do not generate SBoM",
     )
     parser.add_argument(
         "--slice",
         action="store_true",
-        default=True if os.getenv("CPG_SLICE") in ("true", "1") else False,
+        default=os.getenv("CPG_SLICE") in ("true", "1"),
         dest="slice",
         help="Extract intra-procedural slices from the CPG",
     )
     parser.add_argument(
         "--slice-mode",
         default=os.getenv("CPG_SLICE_MODE", "Usages"),
         dest="slice_mode",
         choices=["Usages", "DataFlow"],
         help="Mode used for CPG slicing",
     )
     parser.add_argument(
-        "--use-parse",
-        dest="use_parse",
-        help="Use joern-parse command instead of invoking the language frontends. Useful when default overlays are "
-        "important",
+        "--use-atom",
+        dest="use_atom",
+        help="Use atom toolkit",
         action="store_true",
-        default=False,
+        default=os.getenv("USE_ATOM") in ("true", "1"),
     )
     parser.add_argument(
         "--vectors",
         action="store_true",
-        default=True if os.getenv("CPG_VECTORS") in ("true", "1") else False,
+        default=os.getenv("CPG_VECTORS") in ("true", "1"),
         dest="vectors",
         help="Extract vector representations of code from CPG",
     )
     return parser.parse_args()
 
 
 @app.get("/")
 async def index():
     """Index route"""
     return {}
 
 
 def run_server(args):
     """Run cpggen as a server"""
-    console.print(PRODUCT_LOGO, style="info")
     console.print(f"cpggen server running on {args.server_host}:{args.server_port}")
     app.run(
         host=args.server_host,
         port=args.server_port,
-        debug=True if os.getenv("AT_DEBUG_MODE") in ("debug", "true", "1") else False,
+        debug=os.getenv("AT_DEBUG_MODE") in ("debug", "true", "1"),
         use_reloader=False,
     )
 
 
 @app.route("/cpg", methods=["GET", "POST"])
 async def generate_cpg():
     """Method to generate CPG via the http route"""
@@ -200,15 +202,15 @@
     src = ""
     languages = ""
     cpg_out_dir = None
     auto_build = True
     skip_sbom = True
     export = False
     should_slice = False
-    use_parse = False
+    use_atom = False
     slice_mode = "Usages"
     app_manifest_list = []
     errors_warnings = []
     vectors = False
     if not params:
         params = {}
     if q.get("url"):
@@ -268,27 +270,24 @@
     if cpg_out_dir and not os.path.exists(cpg_out_dir):
         os.makedirs(cpg_out_dir, exist_ok=True)
     if not languages or languages == "autodetect":
         languages = utils.detect_project_type(src)
     else:
         languages = languages.split(",")
     for lang in languages:
-        # Use the deps version of the language when using auto build mode
-        if lang in ("c", "cpp", "java", "kotlin") and auto_build:
-            lang = f"{lang}-with-deps"
         mlist = executor.exec_tool(
             lang,
             src,
             cpg_out_dir,
             src,
             joern_home=os.getenv(
                 "JOERN_HOME", str(Path.home() / "bin" / "joern" / "joern-cli")
             ),
             use_container=False,
-            use_parse=use_parse,
+            use_atom=use_atom,
             auto_build=auto_build,
             extra_args={
                 "skip_sbom": skip_sbom,
                 "slice_mode": slice_mode,
                 "for_export": export,
                 "for_slice": should_slice,
                 "for_vectors": vectors,
@@ -309,15 +308,15 @@
                     ml.get("cpg"),
                     cpg_out_dir,
                     src,
                     joern_home=os.getenv(
                         "JOERN_HOME", str(Path.home() / "bin" / "joern" / "joern-cli")
                     ),
                     use_container=False,
-                    use_parse=use_parse,
+                    use_atom=use_atom,
                     auto_build=False,
                     extra_args={
                         "slice_mode": slice_mode,
                         "slice_out": ml.get("slice_out"),
                     },
                 )
                 if not os.path.exists(ml.get("slice_out")):
@@ -370,15 +369,15 @@
 
 def cpg(
     src,
     cpg_out_dir,
     languages,
     joern_home,
     use_container=False,
-    use_parse=False,
+    use_atom=False,
     auto_build=False,
     skip_sbom=False,
     export=False,
     should_slice=False,
     slice_mode=None,
     vectors=False,
 ):
@@ -394,31 +393,31 @@
                     url = src
                     clone_dir = tempfile.mkdtemp(prefix="cpggen")
                     if src.startswith("http") or src.startswith("git://"):
                         utils.clone_repo(src, clone_dir)
                     else:
                         utils.download_package_unsafe(src, clone_dir)
                     src = clone_dir
-                    if not languages or languages == "autodetect":
-                        languages = utils.detect_project_type(src)
-                    else:
-                        languages = languages.split(",")
+                if not languages or languages == "autodetect":
+                    languages = utils.detect_project_type(src)
+                else:
+                    languages = languages.split(",")
                 for lang in languages:
                     LOG.debug("Generating CPG for the language %s at %s", lang, src)
                     exec_results.append(
                         pool.apply_async(
                             executor.exec_tool,
                             (
                                 lang,
                                 src,
                                 cpg_out_dir,
                                 src,
                                 joern_home,
                                 use_container,
-                                use_parse,
+                                use_atom,
                                 auto_build,
                                 {
                                     "skip_sbom": skip_sbom,
                                     "slice_mode": slice_mode,
                                     "for_export": export,
                                     "for_slice": should_slice,
                                     "for_vectors": vectors,
@@ -450,15 +449,15 @@
     return export_repr
 
 
 def export_slice_cpg(
     cpg_out_dir,
     joern_home,
     use_container,
-    use_parse,
+    use_atom,
     export,
     export_repr,
     export_format,
     export_out_dir,
     should_slice=False,
     slice_mode=None,
     vectors=False,
@@ -507,15 +506,15 @@
                         (
                             export_tool,
                             cpg_path,
                             app_export_out_dir,
                             cpg_out_dir,
                             joern_home,
                             use_container,
-                            use_parse,
+                            use_atom,
                             False,
                             {
                                 "export_repr": fix_export_repr(
                                     export_repr, export_format
                                 )
                                 if export
                                 else None,
@@ -529,30 +528,33 @@
             except KeyboardInterrupt:
                 pool.terminate()
             pool.join()
 
 
 def main():
     """Main method"""
-    print(PRODUCT_LOGO)
+    if os.getenv("ATOM_HOME"):
+        print(ATOM_LOGO)
+    else:
+        print(PRODUCT_LOGO)
     args = build_args()
     # Turn on verbose mode
     if args.verbose_mode:
         enable_debug()
     if args.server_mode:
         return run_server(args)
     src = args.src
     cpg_out_dir, export_out_dir, is_temp_dir = get_output_dir(
         src, args.cpg_out_dir, args.export_out_dir
     )
     if os.path.exists(src):
         src = str(PurePath(src))
     joern_home = args.joern_home
     use_container = args.use_container
-    use_parse = args.use_parse
+    use_atom = args.use_atom
     is_bundled_exe = False
     try:
         if getattr(sys, "_MEIPASS"):
             is_bundled_exe = True
             # Reset joern_home for bundled exe
             if not os.path.exists(joern_home):
                 joern_home = ""
@@ -574,28 +576,28 @@
         joern_home = ""
     cpg_manifests = cpg(
         src,
         cpg_out_dir,
         args.language,
         joern_home=joern_home,
         use_container=use_container,
-        use_parse=use_parse,
+        use_atom=use_atom,
         auto_build=args.auto_build,
         skip_sbom=args.skip_sbom,
         export=args.export,
         should_slice=args.slice,
         slice_mode=args.slice_mode,
         vectors=args.vectors,
     )
     if args.export or args.slice or args.vectors:
         export_slice_cpg(
             cpg_out_dir,
             joern_home=joern_home,
             use_container=use_container,
-            use_parse=use_parse,
+            use_atom=use_atom,
             export=args.export,
             export_repr=args.export_repr,
             export_format=args.export_format,
             export_out_dir=export_out_dir,
             should_slice=args.slice,
             slice_mode=args.slice_mode,
             vectors=args.vectors,
```

### Comparing `cpggen-1.1.7/cpggen/executor.py` & `cpggen-1.2.1/cpggen/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,67 +31,78 @@
 CPU_COUNT = str(psutil.cpu_count())
 
 only_bat_ext = ".bat" if sys.platform == "win32" else ""
 bin_ext = ".bat" if sys.platform == "win32" else ".sh"
 exe_ext = ".exe" if sys.platform == "win32" else ""
 USE_SHELL = True if sys.platform == "win32" else False
 
+ATOM_VERSION = "1.0.0"
+
 
 def resource_path(relative_path):
+    """Function to construct the path to resources in a bundled exe"""
     try:
-        base_path = sys._MEIPASS
-    except Exception:
+        base_path = getattr(sys, "_MEIPASS")
+    except AttributeError:
         base_path = os.path.dirname(__file__)
     return os.path.join(base_path, relative_path)
 
 
 # Check if we are running as a bundled executable and
 # extract the binaries
 cdxgen_cmd = os.environ.get("CDXGEN_CMD", "cdxgen")
 local_bin_dir = resource_path("local_bin")
 if os.path.exists(local_bin_dir):
     csharp2cpg_bundled = resource_path(
-        os.path.join("local_bin", "joern-cli", "csharp2cpg.zip")
+        os.path.join("local_bin", f"atom-{ATOM_VERSION}", "csharp2cpg.zip")
     )
-    joern_bundled = resource_path(os.path.join("local_bin", "joern-cli.zip"))
+    atom_bundled = resource_path(os.path.join("local_bin", "atom.zip"))
     if os.path.exists(csharp2cpg_bundled) and not os.path.exists(
-        os.path.join(local_bin_dir, "joern-cli", "bin", "csharp2cpg")
+        os.path.join(local_bin_dir, f"atom-{ATOM_VERSION}", "bin", "csharp2cpg")
     ):
         try:
             with zipfile.ZipFile(csharp2cpg_bundled, "r") as zip_ref:
-                zip_ref.extractall(os.path.join(local_bin_dir, "joern-cli"))
+                zip_ref.extractall(os.path.join(local_bin_dir, f"atom-{ATOM_VERSION}"))
                 LOG.debug("Extracted %s", csharp2cpg_bundled)
                 if not os.path.exists(
-                    os.path.join(local_bin_dir, "joern-cli", "bin", "csharp2cpg")
+                    os.path.join(
+                        local_bin_dir, f"atom-{ATOM_VERSION}", "bin", "csharp2cpg"
+                    )
                 ):
                     LOG.debug("csharp2cpg could not be found after extraction")
         except Exception as e:
             LOG.info(
                 "cpggen was prevented from extracting the csharp2cpg frontend.\nPlease check if your terminal has administrative privileges or if the antivirus is preventing this process.\nAlternatively, use container-based execution."
             )
             LOG.error(e)
-    if os.path.exists(joern_bundled) and not os.path.exists(
-        os.path.join(local_bin_dir, "joern-cli", "c2cpg.sh")
+    if os.path.exists(atom_bundled) and not os.path.exists(
+        os.path.join(local_bin_dir, f"atom-{ATOM_VERSION}", "bin", "atom")
     ):
         try:
-            with zipfile.ZipFile(joern_bundled, "r") as zip_ref:
+            with zipfile.ZipFile(atom_bundled, "r") as zip_ref:
                 zip_ref.extractall(local_bin_dir)
                 # Add execute permissions
                 for dirname, subdirs, files in os.walk(local_bin_dir):
                     for filename in files:
                         if not filename.endswith(".jar") and (
                             filename.endswith("%(bin_ext)s")
                             or "2cpg" in filename
                             or "joern-" in filename
+                            or "atom" in filename
                         ):
                             os.chmod(os.path.join(dirname, filename), 0o755)
-                LOG.debug("Extracted %s", joern_bundled)
-                os.environ["JOERN_HOME"] = os.path.join(local_bin_dir, "joern-cli")
+                LOG.debug("Extracted %s", atom_bundled)
+                os.environ["ATOM_HOME"] = os.path.join(
+                    local_bin_dir, f"atom-{ATOM_VERSION}"
+                )
+                os.environ["ATOM_BIN_DIR"] = os.path.join(
+                    local_bin_dir, f"atom-{ATOM_VERSION}", "bin", ""
+                )
                 os.environ["CPGGEN_BIN_DIR"] = local_bin_dir
-                os.environ["PATH"] += os.sep + os.environ["JOERN_HOME"] + os.sep
+                os.environ["PATH"] += os.sep + os.environ["ATOM_BIN_DIR"] + os.sep
         except Exception as e:
             LOG.info(
                 "cpggen was prevented from extracting the joern library.\nPlease check if your terminal has administrative privileges or if the antivirus is preventing this process.\nAlternatively, use container-based execution."
             )
             LOG.error(e)
     if not shutil.which(cdxgen_cmd):
         local_cdxgen_cmd = resource_path(
@@ -116,14 +127,15 @@
         value = os.environ.get(config_name.replace("-", "_").upper())
     if value is None:
         value = default_value
     return value
 
 
 cpg_tools_map = {
+    "atom": "%(atom_bin_dir)satom%(only_bat_ext)s -J-Xmx%(memory)s --language %(parse_lang)s --output %(cpg_out)s %(src)s",
     "c": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "cpp": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "c-with-deps": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
     "cpp-with-deps": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
     "java": "%(joern_home)sjavasrc2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "java-with-deps": "%(joern_home)sjavasrc2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.m2",
     "java-with-gradle-deps": "%(joern_home)sjavasrc2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.gradle/caches/modules-2/files-2.1",
@@ -303,15 +315,15 @@
                     stderr=subprocess.PIPE,
                     cwd=export_out_dir,
                     env=env,
                     check=False,
                     shell=USE_SHELL,
                     encoding="utf-8",
                 )
-            except Exception as e:
+            except subprocess.SubprocessError as e:
                 LOG.debug(e)
     else:
         LOG.debug(
             "Install graphviz package and ensure the command `dot` is available in the PATH to convert to png automatically"
         )
 
 
@@ -337,22 +349,22 @@
             if "%(" in build_args_str:
                 gradle_cmd = "gradle"
                 maven_cmd = "mvn"
                 if os.path.exists(os.path.join(base_dir, "gradlew")):
                     gradle_cmd = "gradlew"
                     try:
                         os.chmod(os.path.join(base_dir, "gradlew"), 0o755)
-                    except Exception:
+                    except OSError:
                         # Ignore errors
                         pass
                 if os.path.exists(os.path.join(base_dir, "mvnw")):
                     maven_cmd = "mvnw"
                     try:
                         os.chmod(os.path.join(base_dir, "mvnw"), 0o755)
-                    except Exception:
+                    except OSError:
                         # Ignore errors
                         pass
                 build_args_str = build_args_str % dict(
                     gradle_cmd=gradle_cmd, maven_cmd=maven_cmd
                 )
             try:
                 LOG.debug("Executing build command: %s in %s", build_args_str, base_dir)
@@ -441,15 +453,15 @@
 def exec_tool(
     tool_lang,
     src,
     cpg_out_dir,
     cwd=None,
     joern_home=None,
     use_container=False,
-    use_parse=False,
+    use_atom=False,
     auto_build=False,
     extra_args=None,
     env=None,
     stdout=subprocess.DEVNULL,
 ):
     """Method to execute tools to generate cpg or perform exports"""
     if env is None:
@@ -463,14 +475,21 @@
         redirect_stdout=False,
         refresh_per_second=1,
     ) as progress:
         task = None
         lang_build_crashes = {}
         app_manifest_list = []
         tool_lang_simple = tool_lang.split("-")[0]
+        atom_home = os.getenv("ATOM_HOME", "")
+        atom_bin_dir = os.getenv("ATOM_BIN_DIR")
+        if not atom_bin_dir:
+            if atom_home:
+                atom_bin_dir = os.path.join(atom_home, "bin", "")
+            else:
+                atom_bin_dir = "/usr/local/bin/"
         # Set joern_home from environment variable
         # This is required to handle bundled exe mode
         if (
             not joern_home
             and os.getenv("JOERN_HOME")
             and os.path.exists(os.getenv("JOERN_HOME"))
         ):
@@ -478,14 +497,19 @@
         if cwd:
             if os.path.isfile(cwd):
                 cwd = os.path.dirname(cwd)
             else:
                 cwd = os.path.abspath(cwd)
         if joern_home and not joern_home.endswith(os.path.sep):
             joern_home = f"{joern_home}{os.path.sep}"
+        if atom_home and not atom_home.endswith(os.path.sep):
+            atom_home = f"{atom_home}{os.path.sep}"
+            # Use atom for supported languages if available
+            if tool_lang_simple in ("java", "c", "cpp", "js", "jimple", "ts", "python"):
+                use_atom = True
         try:
             stderr = subprocess.DEVNULL
             if LOG.isEnabledFor(DEBUG):
                 stdout = subprocess.PIPE
                 stderr = stdout
             tool_verb = f"Building CPG with {tool_lang} frontend"
             if tool_lang == "export":
@@ -497,19 +521,19 @@
             task = progress.add_task(
                 "[green]" + tool_verb,
                 total=100,
                 start=False,
             )
             cpg_cmd_lang = tool_lang
             # If the intention is to export or slice then use joern-parse
-            if use_parse or (
+            if use_atom or (
                 extra_args
                 and (extra_args.get("for_export") or extra_args.get("for_slice"))
             ):
-                cpg_cmd_lang = "parse"
+                cpg_cmd_lang = "atom"
             cmd_with_args = cpg_tools_map.get(cpg_cmd_lang)
             if not cmd_with_args:
                 return
             # Perform build first
             if build_tools_map.get(tool_lang):
                 if os.getenv("CI"):
                     LOG.debug(
@@ -597,14 +621,15 @@
                     slice_out = slice_out + (
                         ".json" if extra_args.get("slice_mode") == "Usages" else ".cpg"
                     )
                     extra_args["slice_out"] = slice_out
                 cmd_with_args = cmd_with_args % dict(
                     src=os.path.abspath(amodule),
                     cpg_out=cpg_out,
+                    atom_bin_dir=atom_bin_dir,
                     joern_home=joern_home,
                     home_dir=str(Path.home()),
                     uber_jar=uber_jar,
                     csharp_artifacts=csharp_artifacts,
                     memory=os.getenv("CPGGEN_MEMORY", max_memory),
                     tool_lang=tool_lang,
                     parse_lang=joern_parse_lang_map.get(
@@ -637,29 +662,30 @@
                     bin_ext=bin_ext,
                     exe_ext=exe_ext,
                     only_bat_ext=only_bat_ext,
                     os_path_sep=os.path.sep,
                     cdxgen_args=f' {os.getenv("CDXGEN_ARGS", "").strip()}'
                     if os.getenv("CDXGEN_ARGS")
                     else "",
+                    atom_bin_dir=atom_bin_dir,
                     cpggen_bin_dir=os.getenv("CPGGEN_BIN_DIR", "/usr/local/bin"),
                     **extra_args,
                 )
                 cmd_list_with_args = cmd_with_args.split(" ")
                 sbom_cmd_list_with_args = sbom_cmd_with_args.split(" ")
                 lang_cmd = cmd_list_with_args[0]
                 if not check_command(lang_cmd) and not os.path.exists(lang_cmd):
                     if not use_container:
                         LOG.warning(
                             "%s is not found. Try running cpggen with --use-container argument.",
                             lang_cmd,
                         )
-                    elif not use_parse:
+                    elif not use_atom:
                         LOG.warning(
-                            "Try running cpggen with --use-parse argument to use joern-parse command instead of language frontends."
+                            "Try running cpggen with --use-atom argument to use AppThreat atom command."
                         )
                     else:
                         LOG.warning(
                             "%s is not found. Ensure the PATH variable in your container image is set to the bin directory of Joern.",
                             lang_cmd,
                         )
                     return
@@ -749,30 +775,29 @@
                                     "Unable to %s %s to %s. Try running joern-%s manually using the command %s",
                                     tool_lang,
                                     src,
                                     check_dir,
                                     tool_lang,
                                     " ".join(cmd_list_with_args),
                                 )
-                    except Exception as e:
+                    except subprocess.SubprocessError:
                         LOG.warning(
                             "Unable to %s %s to %s",
                             tool_lang,
                             src,
                             cpg_out_dir,
                             exc_info=True,
                         )
                     progress.update(task, completed=100, total=100)
                     continue
                 LOG.debug(
-                    '⚡︎ Generating CPG for the {} app "{}" - "{}"'.format(
-                        tool_lang,
-                        os.path.basename(amodule),
-                        " ".join(cmd_list_with_args),
-                    )
+                    '⚡︎ Generating CPG for the %s app "%s" - "%s"',
+                    tool_lang,
+                    os.path.basename(amodule),
+                    " ".join(cmd_list_with_args),
                 )
                 cwd = amodule
                 if tool_lang in ("binary",):
                     cwd = os.getcwd()
                 if tool_lang != "binary" and not extra_args.get("skip_sbom"):
                     # Generate sbom first since this would even download dependencies for java
                     try:
@@ -904,14 +929,14 @@
                         )
                     if cp.stdout:
                         LOG.info(cp.stdout)
                     if cp.stderr:
                         LOG.info(cp.stderr)
                     troubleshoot_app(lang_build_crashes, tool_lang)
                 progress.update(task, completed=100, total=100)
-        except Exception as e:
+        except subprocess.SubprocessError as se:
             if not os.getenv("AT_DEBUG_MODE"):
                 LOG.info(
                     "Set the environment variable AT_DEBUG_MODE to debug to see the debug logs"
                 )
-            LOG.warning(e)
+            LOG.warning(se)
     return app_manifest_list
```

### Comparing `cpggen-1.1.7/cpggen/logger.py` & `cpggen-1.2.1/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.1.7/cpggen/source/ghsa.py` & `cpggen-1.2.1/cpggen/source/ghsa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+
 import httpx
 
 # GitHub advisory feed url
 ghsa_api_url = os.getenv("GITHUB_GRAPHQL_URL", "https://api.github.com/graphql")
 api_token = os.getenv("GITHUB_TOKEN")
 headers = {"Authorization": f"token {api_token}"}
```

### Comparing `cpggen-1.1.7/cpggen/utils.py` & `cpggen-1.2.1/cpggen/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 import re
 import shutil
-import tempfile
 import tarfile
+import tempfile
 import zipfile
 from pathlib import Path
 from sys import platform
 
 import httpx
 import rich.progress
 from packageurl import PackageURL
```

### Comparing `cpggen-1.1.7/pyproject.toml` & `cpggen-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "1.1.7"
+version = "1.2.1"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-1.1.7/PKG-INFO` & `cpggen-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 1.1.7
+Version: 1.2.1
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8.1,<3.12
@@ -47,15 +47,15 @@
 [![Discord](https://img.shields.io/badge/-Discord-lime?style=for-the-badge&logo=discord&logoColor=white&color=black)](https://discord.gg/tmmtjCEHNV)
 
 ## Pre-requisites
 
 - JDK 11 or above
 - Python 3.10
 - Docker or podman (Windows, Linux or Mac) or
-- Joern [natively installed](https://docs.joern.io/installation) (Linux only)
+- [Atom](https://github.com/AppThreat/atom#installation) or [Joern](https://docs.joern.io/installation)
 
 ## Installation
 
 cpggen is available as a single executable binary, [PyPI package](https://pypi.org/project/cpggen/) or as a [container image](https://github.com/AppThreat/cpggen/pkgs/container/cpggen).
 
 ### Single executable binaries
 
@@ -67,14 +67,22 @@
 
 ```bash
 curl -LO https://github.com/AppThreat/cpggen/releases/latest/download/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
+OSS version without any Qwiet.AI binary frontends.
+
+```bash
+curl -LO https://github.com/AppThreat/cpggen/releases/latest/download/cpggen-oss-linux-amd64
+chmod +x cpggen-oss-linux-amd64
+./cpggen-oss-linux-amd64 --help
+```
+
 On Windows,
 
 ```powershell
 curl -LO https://github.com/appthreat/cpggen/releases/latest/download/cpggen.exe
 .\cpggen.exe --help
 ```
 
@@ -316,15 +324,15 @@
   --export-out-dir EXPORT_OUT_DIR
                         Export output directory
   --verbose             Run cpggen in verbose mode
   --skip-sbom           Do not generate SBoM
   --slice               Extract intra-procedural slices from the CPG
   --slice-mode {Usages,DataFlow}
                         Mode used for CPG slicing
-  --use-parse           Use joern-parse command instead of invoking the language frontends. Useful when default overlays are important
+  --use-atom            Use atom toolkit
   --vectors             Extract vector representations of code from CPG
 ```
 
 ## Environment variables
 
 | Name                    | Purpose                                                                    |
 | ----------------------- | -------------------------------------------------------------------------- |
@@ -342,14 +350,15 @@
 | CPG_SLICE_MODE          | Slice mode. Default Usages                                                 |
 | CPG_VECTORS             | Set to true to generate vector representations of code from CPG            |
 | SHIFTLEFT_ACCESS_TOKEN  | Set to automatically submit the CPG for analysis by Qwiet AI               |
 | CDXGEN_ARGS             | Extra arguments to pass to cdxgen                                          |
 | ENABLE_SBOM             | Enable SBoM generation using cdxgen                                        |
 | JIMPLE_ANDROID_JAR      | Path to android.jar for use with jimple for .apk or .dex to CPG conversion |
 | GITHUB_TOKEN            | Token with read:packages scope to analyze CVE or GitHub Advisory           |
+| USE_ATOM                | Use AppThreat atom instead of joern frontends                              |
 
 ## GitHub actions
 
 Use the marketplace [action](https://github.com/marketplace/actions/cpggen) to generate CPGs using GitHub actions. Optionally, the upload the generated CPGs as build artifacts use the below step.
 
 ```
 - name: Upload cpg
```

