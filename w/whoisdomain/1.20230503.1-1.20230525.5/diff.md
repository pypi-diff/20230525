# Comparing `tmp/whoisdomain-1.20230503.1.tar.gz` & `tmp/whoisdomain-1.20230525.5.tar.gz`

## Comparing `whoisdomain-1.20230503.1.tar` & `whoisdomain-1.20230525.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/whoisdomain/_0_init_tld.py
--rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/whoisdomain/_1_query.py
--rw-r--r--   0        0        0     9065 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/whoisdomain/_2_parse.py
--rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/whoisdomain/_3_adjust.py
--rw-r--r--   0        0        0    10648 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/whoisdomain/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/whoisdomain/exceptions.py
--rwxr-xr-x   0        0        0    17812 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/whoisdomain/main.py
--rw-r--r--   0        0        0   104916 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/whoisdomain/tld_regexpr.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/whoisdomain/version.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/.gitignore
--rw-r--r--   0        0        0     7575 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/README.md
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/pyproject.toml
--rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 whoisdomain-1.20230503.1/PKG-INFO
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.5/whoisdomain/_0_init_tld.py
+-rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.5/whoisdomain/_1_query.py
+-rw-r--r--   0        0        0    10112 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.5/whoisdomain/_2_parse.py
+-rw-r--r--   0        0        0     9507 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.5/whoisdomain/_3_adjust.py
+-rw-r--r--   0        0        0    13509 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.5/whoisdomain/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.5/whoisdomain/exceptions.py
+-rwxr-xr-x   0        0        0    17816 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.5/whoisdomain/main.py
+-rw-r--r--   0        0        0   131262 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.5/whoisdomain/tld_regexpr.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.5/whoisdomain/version.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.5/.gitignore
+-rw-r--r--   0        0        0     8724 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.5/README.md
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.5/pyproject.toml
+-rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.5/PKG-INFO
```

### Comparing `whoisdomain-1.20230503.1/whoisdomain/_0_init_tld.py` & `whoisdomain-1.20230525.5/whoisdomain/_0_init_tld.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230503.1/whoisdomain/_1_query.py` & `whoisdomain-1.20230525.5/whoisdomain/_1_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,93 +5,60 @@
 import platform
 import json
 from .exceptions import WhoisCommandFailed, WhoisCommandTimeout
 
 from typing import Dict, List, Optional, Tuple
 
 
-PYTHON_VERSION = sys.version_info[0]
+# PYTHON_VERSION = sys.version_info[0]
 CACHE: Dict[str, Tuple[int, str]] = {}
 CACHE_MAX_AGE = 60 * 60 * 48  # 48h
 
 
-def cache_load(cf: str) -> None:
+def _cache_load(cf: str) -> None:
     if not os.path.isfile(cf):
         return
 
     global CACHE
     f = open(cf, "r")
 
     try:
         CACHE = json.load(f)
     except Exception as e:
         print(f"ignore lson load err: {e}", file=sys.stderr)
 
     f.close()
 
 
-def cache_save(cf: str) -> None:
+def _cache_save(cf: str) -> None:
     global CACHE
 
     f = open(cf, "w")
     json.dump(CACHE, f)
     f.close()
 
 
-def do_query(
+def _testWhoisPythonFromStaticTestData(
     dl: List[str],
-    force: bool = False,
-    cache_file: Optional[str] = None,
-    cache_age: int = CACHE_MAX_AGE,
-    slow_down: int = 0,
-    ignore_returncode: bool = False,
+    ignore_returncode: bool,
     server: Optional[str] = None,
     verbose: bool = False,
-    timeout: Optional[float] = None,
-    wh: str = "whois",
-    simplistic: bool = False,
 ) -> str:
-    k = ".".join(dl)
-
-    if cache_file:
-        if verbose:
-            print(f"using cache file: {cache_file}", file=sys.stderr)
-        cache_load(cache_file)
-
-    # actually also whois uses cache, so if you really dont want to use cache
-    # you should also pass the --force-lookup flag (on linux)
-    if force or k not in CACHE or CACHE[k][0] < time.time() - cache_age:
-        if verbose:
-            print(f"force = {force}", file=sys.stderr)
-
-        # slow down before so we can force individual domains at a slower tempo
-        if slow_down:
-            time.sleep(slow_down)
-
-        # populate a fresh cache entry
-        CACHE[k] = (
-            int(time.time()),
-            _do_whois_query(
-                dl=dl,
-                ignore_returncode=ignore_returncode,
-                server=server,
-                verbose=verbose,
-                timeout=timeout,
-                wh=wh,
-                simplistic=simplistic,
-            ),
-        )
-
-        if cache_file:
-            cache_save(cache_file)
+    domain = ".".join(dl)
+    testDir = os.getenv("TEST_WHOIS_PYTHON")
+    pathToTestFile = f"{testDir}/{domain}/input"
+    if os.path.exists(pathToTestFile):
+        with open(pathToTestFile, mode="rb") as f:  # switch to binary mode as that is what Popen uses
+            # make sure the data is treated exactly the same as the output of Popen
+            return f.read().decode(errors="ignore")
 
-    return CACHE[k][1]
+    raise WhoisCommandFailed("")
 
 
-def tryInstallMissingWhoisOnWindows(
+def _tryInstallMissingWhoisOnWindows(
     verbose: bool = False,
 ) -> None:
     """
     Windows 'whois' command wrapper
     https://docs.microsoft.com/en-us/sysinternals/downloads/whois
     """
     folder = os.getcwd()
@@ -104,84 +71,77 @@
         copy_command,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
         shell=True,
     )
 
 
-def makeWhoisCommandToRun(
+def _makeWhoisCommandToRun(
     dl: List[str],
     server: Optional[str] = None,
     verbose: bool = False,
     wh: str = "whois",
 ) -> List[str]:
     domain = ".".join(dl)
 
-    if platform.system() == "Windows":
-        # Usage: whois [-v] domainname [whois.server]
-
-        if os.path.exists("whois.exe"):
-            wh = r".\whois.exe"
-        else:
-            find = False
-            paths = os.environ["path"].split(";")
-            for path in paths:
-                wpath = os.path.join(path, "whois.exe")
-                if os.path.exists(wpath):
-                    wh = wpath
-                    find = True
-                    break
+    if " " in wh:
+        whList = wh.split(" ")
+    else:
+        whList = [wh]
 
-            if not find:
-                tryInstallMissingWhoisOnWindows(verbose)
+    if platform.system() == "Windows":
+        if wh == "whois":  # only if the use did not specify what whois to use
+            if os.path.exists("whois.exe"):
+                wh = r".\whois.exe"
+            else:
+                find = False
+                paths = os.environ["path"].split(";")
+                for path in paths:
+                    wpath = os.path.join(path, "whois.exe")
+                    if os.path.exists(wpath):
+                        wh = wpath
+                        find = True
+                        break
+
+                if not find:
+                    _tryInstallMissingWhoisOnWindows(verbose)
+        whList = [wh]
 
         if server:
-            return [wh, "-v", "-nobanner", domain, server]
-        return [wh, "-v", "-nobanner", domain]
+            return whList + ["-v", "-nobanner", domain, server]
+        return whList + ["-v", "-nobanner", domain]
 
+    # not windows
     if server:
-        return [wh, domain, "-h", server]
-        # return [wh, domain, "-i", "-d", "-h", server]
-    return [wh, domain]
-
-
-def testWhoisPythonFromStaticTestData(
-    dl: List[str],
-    ignore_returncode: bool,
-    server: Optional[str] = None,
-    verbose: bool = False,
-) -> str:
-    domain = ".".join(dl)
-    testDir = os.getenv("TEST_WHOIS_PYTHON")
-    pathToTestFile = f"{testDir}/{domain}/input"
-    if os.path.exists(pathToTestFile):
-        with open(pathToTestFile, mode="rb") as f:  # switch to binary mode as that is what Popen uses
-            # make sure the data is treated exactly the same as the output of Popen
-            return f.read().decode(errors="ignore")
-
-    raise WhoisCommandFailed("")
+        return whList + [domain, "-h", server]
+    return whList + [domain]
 
 
 def _do_whois_query(
     dl: List[str],
     ignore_returncode: bool,
     server: Optional[str] = None,
     verbose: bool = False,
     timeout: Optional[float] = None,
     wh: str = "whois",
     simplistic: bool = False,
 ) -> str:
     # if getenv[TEST_WHOIS_PYTON] fake whois by reading static data from a file
     # this wasy we can actually implemnt a test run with known data in and expected data out
     if os.getenv("TEST_WHOIS_PYTHON"):
-        return testWhoisPythonFromStaticTestData(dl, ignore_returncode, server, verbose)
+        return _testWhoisPythonFromStaticTestData(dl, ignore_returncode, server, verbose)
 
-    cmd = makeWhoisCommandToRun(dl=dl, server=server, verbose=verbose, wh=wh)
+    cmd = _makeWhoisCommandToRun(
+        dl=dl,
+        server=server,
+        verbose=verbose,
+        wh=wh,
+    )
     if verbose:
-        print(cmd, file=sys.stderr)
+        print(cmd, wh, file=sys.stderr)
 
     # LANG=en is added to make the ".jp" output consist across all environments
     p = subprocess.Popen(
         cmd,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
         env={"LANG": "en"} if dl[-1] in ".jp" else None,
@@ -189,15 +149,15 @@
 
     try:
         r = p.communicate(timeout=timeout)[0].decode(errors="ignore")
     except subprocess.TimeoutExpired:
         # Kill the child process & flush any output buffers
         p.kill()
         p.communicate()
-        raise WhoisCommandTimeout()
+        raise WhoisCommandTimeout(f"timeout: query took more then {timeout} seconds")
 
     if verbose:
         print(r, file=sys.stderr)
 
     if ignore_returncode is False and p.returncode not in [0, 1]:
         # network error, "fgets: Connection reset by peer" fix, ignore
         if "fgets: Connection reset by peer" in r:
@@ -208,7 +168,60 @@
 
         if simplistic:
             return r
 
         raise WhoisCommandFailed(r)
 
     return r
+
+
+# PUBLIC
+
+
+def do_query(
+    dl: List[str],
+    force: bool = False,
+    cache_file: Optional[str] = None,
+    cache_age: int = CACHE_MAX_AGE,
+    slow_down: int = 0,
+    ignore_returncode: bool = False,
+    server: Optional[str] = None,
+    verbose: bool = False,
+    timeout: Optional[float] = None,
+    wh: str = "whois",
+    simplistic: bool = False,
+) -> str:
+    k = ".".join(dl)
+
+    if cache_file:
+        if verbose:
+            print(f"using cache file: {cache_file}", file=sys.stderr)
+        _cache_load(cache_file)
+
+    # actually also whois uses cache, so if you really dont want to use cache
+    # you should also pass the --force-lookup flag (on linux)
+    if force or k not in CACHE or CACHE[k][0] < time.time() - cache_age:
+        if verbose:
+            print(f"force = {force}", file=sys.stderr)
+
+        # slow down before so we can force individual domains at a slower tempo
+        if slow_down:
+            time.sleep(slow_down)
+
+        # populate a fresh cache entry
+        CACHE[k] = (
+            int(time.time()),
+            _do_whois_query(
+                dl=dl,
+                ignore_returncode=ignore_returncode,
+                server=server,
+                verbose=verbose,
+                timeout=timeout,
+                wh=wh,
+                simplistic=simplistic,
+            ),
+        )
+
+        if cache_file:
+            _cache_save(cache_file)
+
+    return CACHE[k][1]
```

### Comparing `whoisdomain-1.20230503.1/whoisdomain/_2_parse.py` & `whoisdomain-1.20230525.5/whoisdomain/_2_parse.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,16 +8,22 @@
     Optional,
     List,
     Tuple,
 )
 
 from ._0_init_tld import TLD_RE
 
-from .exceptions import FailedParsingWhoisOutput
-from .exceptions import WhoisQuotaExceeded
+from ._3_adjust import (
+    Domain,
+)
+
+from .exceptions import (
+    FailedParsingWhoisOutput,
+    WhoisQuotaExceeded,
+)
 
 Verbose: bool = True
 
 NONESTRINGS: List[str] = [
     "the domain has not been registered",
     "no match found for",
     "no matching record",
@@ -47,89 +53,22 @@
     "can temporarily not be answered",
     "please try again.",
     "queried interval is too short",
     "number of allowed queries exceeded",
 ]
 
 
-def NoneStrings() -> List[str]:
-    return sorted(NONESTRINGS)
-
-
-def NoneStringsAdd(aString: str) -> None:
-    if aString and isinstance(aString, str) and len(aString) > 0:
-        NONESTRINGS.append(aString)
-
-
-def QuotaStrings() -> List[str]:
-    return sorted(QUOTASTRINGS)
-
-
-def QuotaStringsAdd(aString: str) -> None:
-    if aString and isinstance(aString, str) and len(aString) > 0:
-        NONESTRINGS.append(aString)
-
-
-def cleanupWhoisResponse(
-    whois_str: str,
-    verbose: bool = False,
-    with_cleanup_results: bool = False,
-) -> str:
-    tmp2: List[str] = []
-
-    # note we cannot do yet rstrip() on the lines as many registrars use \r and even trailing whitespace after entries
-    # as the resulting matches are all stripped of leading and trailing whitespace this currently is fixed there
-    # and relaxes the regexes: you will often see a capture with (.*)
-    # we would have to fix all regexes to allow stripping all trailing whitespace
-    # it would make many matches easier though.
-
-    skipFromHere = False
-    tmp: List[str] = whois_str.split("\n")
-    for line in tmp:
-        if skipFromHere is True:
-            continue
-
-        # some servers respond with: % Quota exceeded in the comment section (lines starting with %)
-        if "quota exceeded" in line.lower():
-            raise WhoisQuotaExceeded(whois_str)
-
-        if with_cleanup_results is True and line.startswith("%"):  # only remove if requested
-            continue
-
-        if "REDACTED FOR PRIVACY" in line:  # these lines contibute nothing so ignore
-            continue
-
-        if (
-            "Please query the RDDS service of the Registrar of Record" in line
-        ):  # these lines contibute nothing so ignore
-            continue
-
-        # regular responses may at the end have meta info starting with a line >>> some texte <<<
-        # similar trailing info exists with lines starting with -- but we wil handle them later
-        # unfortunalery we have domains (google.st) that have this early at the top
-        if 0:
-            if line.startswith(">>>"):
-                skipFromHere = True
-                continue
-
-        if line.startswith("Terms of Use:"):  # these lines contibute nothing so ignore
-            continue
-
-        tmp2.append(line.strip("\r"))
-
-    return "\n".join(tmp2)
-
-
-def handleShortResponse(
+def _handleShortResponse(
     tld: str,
     dl: List[str],
     whois_str: str,
     verbose: bool = False,
-) -> None:
-    # returns None or raises one of (WhoisQuotaExceeded, FailedParsingWhoisOutput)
+    simplistic: bool = False,
+    include_raw_whois_text: bool = False,
+) -> Optional[Domain]:
     if verbose:
         d = ".".join(dl)
         print(f"line count < 5:: {tld} {d} {whois_str}", file=sys.stderr)
 
     # TODO: some short responses are actually valid:
     # lookfor Domain: and Status but all other fields are missing so the regexec could fail
     # this domain is taken already or reserved
@@ -156,44 +95,63 @@
             print("i see 'error' in the result, return: None", file=sys.stderr)
         return None
 
     # ---------------------------------
     quotaStrings = QuotaStrings()
     for i in quotaStrings:
         if i in s:
+            if simplistic:
+                msg = "WhoisQuotaExceeded"
+                return Domain(
+                    data={},
+                    whois_str=whois_str,
+                    verbose=verbose,
+                    include_raw_whois_text=include_raw_whois_text,
+                    exeptionStr=msg,
+                )
             raise WhoisQuotaExceeded(whois_str)
 
+    if simplistic:
+        msg = "FailedParsingWhoisOutput"
+        return Domain(
+            data={},
+            whois_str=whois_str,
+            verbose=verbose,
+            include_raw_whois_text=include_raw_whois_text,
+            exeptionStr=msg,
+        )
+
     raise FailedParsingWhoisOutput(whois_str)
 
 
-def doDnsSec(
+def _doDnsSec(
     whois_str: str,
 ) -> bool:
     whois_dnssec: Any = whois_str.split("DNSSEC:")
     if len(whois_dnssec) >= 2:
         whois_dnssec = whois_dnssec[1].split("\n")[0]
         if whois_dnssec.strip() == "signedDelegation" or whois_dnssec.strip() == "yes":
             return True
     return False
 
 
-def doIfServerNameLookForDomainName(
+def _doIfServerNameLookForDomainName(
     whois_str: str,
     verbose: bool = False,
 ) -> str:
     # not often available anymore
     if re.findall(r"Server Name:\s?(.+)", whois_str, re.IGNORECASE):
         if verbose:
             msg = "i have seen Server Name:, looking for Domain Name:"
             print(msg, file=sys.stderr)
         whois_str = whois_str[whois_str.find("Domain Name:") :]
     return whois_str
 
 
-def doExtractPattensIanaFromWhoisString(
+def _doExtractPattensIanaFromWhoisString(
     tld: str,
     r: Dict[str, Any],
     whois_str: str,
     verbose: bool = False,
 ) -> Dict[str, Any]:
     # now handle the actual format if this whois response
     iana = {
@@ -206,15 +164,15 @@
         if zz:
             if verbose:
                 print(f"parsing iana data only for tld: {tld}, {zz}", file=sys.stderr)
             r[k] = zz
     return r
 
 
-def doExtractPattensFromWhoisString(
+def _doExtractPattensFromWhoisString(
     tld: str,
     r: Dict[str, Any],
     whois_str: str,
     verbose: bool = False,
 ) -> Dict[str, Any]:
     for k, v in TLD_RE.get(tld, TLD_RE["com"]).items():  # use TLD_RE["com"] as default if a regex is missing
         if k.startswith("_"):  # skip meta element like: _server or _privateRegistry
@@ -225,15 +183,15 @@
             r[k] = [""]
         else:
             r[k] = v.findall(whois_str) or [""]
 
     return r
 
 
-def doSourceIana(
+def _doSourceIana(
     tld: str,
     r: Dict[str, Any],
     whois_str: str,
     verbose: bool = False,
 ) -> Tuple[str, Optional[Dict[str, Any]]]:
     # here we can handle the example.com and example.net permanent IANA domains
     k = "source:       IANA"
@@ -252,60 +210,143 @@
         if verbose:
             msg = f"after: {k} we see not only whitespace: {whois_splitted[1]}"
             print(msg, file=sys.stderr)
 
         return whois_splitted[1], None
 
     # try to parse this as a IANA domain as after is only whitespace
-    r = doExtractPattensFromWhoisString(
+    r = _doExtractPattensFromWhoisString(
         tld,
         r,
         whois_str,
         verbose,
     )  # set default values
 
     # now handle the actual format if this whois response
-    r = doExtractPattensIanaFromWhoisString(
+    r = _doExtractPattensIanaFromWhoisString(
         tld,
         r,
         whois_str,
         verbose,
     )
 
     return whois_str, r
 
 
+# PUBLIC
+
+
+def cleanupWhoisResponse(
+    whois_str: str,
+    verbose: bool = False,
+    with_cleanup_results: bool = False,
+    withRedacted: bool = False,
+) -> str:
+    tmp2: List[str] = []
+
+    # note we cannot do yet rstrip() on the lines as many registrars use \r and even trailing whitespace after entries
+    # as the resulting matches are all stripped of leading and trailing whitespace this currently is fixed there
+    # and relaxes the regexes: you will often see a capture with (.*)
+    # we would have to fix all regexes to allow stripping all trailing whitespace
+    # it would make many matches easier though.
+
+    skipFromHere = False
+    tmp: List[str] = whois_str.split("\n")
+    for line in tmp:
+        if skipFromHere is True:
+            continue
+
+        # some servers respond with: % Quota exceeded in the comment section (lines starting with %)
+        if "quota exceeded" in line.lower():
+            raise WhoisQuotaExceeded(whois_str)
+
+        if with_cleanup_results is True and line.startswith("%"):  # only remove if requested
+            continue
+
+        if withRedacted is True:
+            if "REDACTED FOR PRIVACY" in line:  # these lines contibute nothing so ignore
+                continue
+
+        if (
+            "Please query the RDDS service of the Registrar of Record" in line
+        ):  # these lines contibute nothing so ignore
+            continue
+
+        # regular responses may at the end have meta info starting with a line >>> some texte <<<
+        # similar trailing info exists with lines starting with -- but we wil handle them later
+        # unfortunalery we have domains (google.st) that have this early at the top
+        if 0:
+            if line.startswith(">>>"):
+                skipFromHere = True
+                continue
+
+        if line.startswith("Terms of Use:"):  # these lines contibute nothing so ignore
+            continue
+
+        tmp2.append(line.strip("\r"))
+
+    return "\n".join(tmp2)
+
+
+def NoneStrings() -> List[str]:
+    return sorted(NONESTRINGS)
+
+
+def NoneStringsAdd(aString: str) -> None:
+    if aString and isinstance(aString, str) and len(aString) > 0:
+        NONESTRINGS.append(aString)
+
+
+def QuotaStrings() -> List[str]:
+    return sorted(QUOTASTRINGS)
+
+
+def QuotaStringsAdd(aString: str) -> None:
+    if aString and isinstance(aString, str) and len(aString) > 0:
+        NONESTRINGS.append(aString)
+
+
 def do_parse(
     whois_str: str,
     tld: str,
     dl: List[str],
     verbose: bool = False,
     with_cleanup_results: bool = False,
     simplistic: bool = False,
-) -> Optional[Dict[str, Any]]:
+    include_raw_whois_text: bool = False,
+    withRedacted: bool = False,
+) -> Any:
 
     whois_str = cleanupWhoisResponse(
         whois_str=whois_str,
         verbose=verbose,
         with_cleanup_results=with_cleanup_results,
+        withRedacted=withRedacted,
     )
 
     if whois_str.count("\n") < 5:
-        # return handleShortResponse(tld, dl, whois_str, verbose)
-        handleShortResponse(tld, dl, whois_str, verbose)
-        return None
+        result = _handleShortResponse(  # may raise:    FailedParsingWhoisOutput,    WhoisQuotaExceeded,
+            tld=tld,
+            dl=dl,
+            whois_str=whois_str,
+            verbose=verbose,
+            simplistic=simplistic,
+            include_raw_whois_text=include_raw_whois_text,
+        )
+        return result
 
+    # this is the beginning of the return data
     r: Dict[str, Any] = {
         "tld": tld,
-        "DNSSEC": doDnsSec(whois_str),
+        "DNSSEC": _doDnsSec(whois_str),
     }
 
     if "source:       IANA" in whois_str:  # prepare for handling historical IANA domains
-        whois_str, ianaDomain = doSourceIana(tld, r, whois_str, verbose)
+        whois_str, ianaDomain = _doSourceIana(tld, r, whois_str, verbose)
         if ianaDomain is not None:
             ianaDomain = cast(Optional[Dict[str, Any]], ianaDomain)
             return ianaDomain
 
     if "Server Name" in whois_str:  # handle old type Server Name (not very common anymore)
-        whois_str = doIfServerNameLookForDomainName(whois_str, verbose)
+        whois_str = _doIfServerNameLookForDomainName(whois_str, verbose)
 
-    return doExtractPattensFromWhoisString(tld, r, whois_str, verbose)
+    return _doExtractPattensFromWhoisString(tld, r, whois_str, verbose)
```

### Comparing `whoisdomain-1.20230503.1/whoisdomain/_3_adjust.py` & `whoisdomain-1.20230525.5/whoisdomain/_3_adjust.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,105 +1,97 @@
 import re
 import sys
 import datetime
 from .exceptions import UnknownDateFormat
 
 from typing import Any, List, Dict, Optional
 
-PYTHON_VERSION = sys.version_info[0]
+# PYTHON_VERSION = sys.version_info[0]
 
 
 class Domain:
-    # make sure all fields actually exist allways
+    # mandatory fields we expect always to be present (but can be None or '')
     name: Optional[str] = None
     tld: Optional[str] = None
     registrar: Optional[str] = None
     registrant_country: Optional[str] = None
 
     creation_date = None
     expiration_date = None
     last_updated = None
 
     status: Optional[str] = None
     statuses: List[str] = []
 
     dnssec: bool = False
     name_servers: List[str] = []
+
+    # optional fields
     owner: Optional[str] = None
     abuse_contact = None
     reseller = None
     registrant = None
     admin = None
+    emails: List[str] = []
 
-    def __init__(
+    def _cleanupArray(
         self,
-        data: Dict[str, Any],
-        whois_str: Optional[str] = None,
-        verbose: bool = False,
-        include_raw_whois_text: bool = False,
-        return_raw_text_for_unsupported_tld: bool = False,
-    ):
-        if include_raw_whois_text and whois_str is not None:
-            self.text = whois_str
+        data: List[str],
+    ) -> List[str]:
+        if "" in data:
+            index = data.index("")
+            data.pop(index)
+        return data
 
-        if return_raw_text_for_unsupported_tld is True:
-            self.tld = data["tld"]
-            self.name = data["domain_name"][0].strip().lower()
-            return
-
-        self.name = data["domain_name"][0].strip().lower()
-        self.tld = data["tld"].lower()
-
-        self.registrar = data["registrar"][0].strip()
-        self.registrant_country = data["registrant_country"][0].strip()
-
-        self.creation_date = str_to_date(data["creation_date"][0], self.tld, verbose=verbose)
-        self.expiration_date = str_to_date(data["expiration_date"][0], self.tld, verbose=verbose)
-        self.last_updated = str_to_date(data["updated_date"][0], self.tld, verbose=verbose)
-
-        self.status = data["status"][0].strip()
-        self.statuses = sorted(  # sorted added to get predictable output during test
-            list(  # list(set(...))) to deduplicate results
-                set(
-                    [s.strip() for s in data["status"]],
-                ),
-            ),
-        )
-
-        self.dnssec = data["DNSSEC"]
-
-        # ----------------------------
-        # name_servers
-        tmp = []
+    def _doNameservers(
+        self,
+        data: Dict[str, Any],
+    ) -> None:
+        tmp: List[str] = []
         for x in data["name_servers"]:
             if isinstance(x, str):
                 tmp.append(x.strip().lower())
                 continue
             # not a string but an array
             for y in x:
                 tmp.append(y.strip().lower())
 
-        if 0:
-            if verbose:
-                print(tmp, file=sys.stderr)
-
         self.name_servers = []
         for x in tmp:
-            x = x.strip(" .")  # remove ant leading or trailing spaces and/or dots
+            x = x.strip(" .")  # remove any leading or trailing spaces and/or dots
             if x:
                 if " " in x:
                     x, _ = x.split(" ", 1)
                     x = x.strip(" .")
 
                 x = x.lower()
                 if x not in self.name_servers:
                     self.name_servers.append(x)
         self.name_servers = sorted(self.name_servers)
-        # ----------------------------
 
+    def _doStatus(
+        self,
+        data: Dict[str, Any],
+    ) -> None:
+        self.status = data["status"][0].strip()
+        self.statuses = sorted(  # sorted added to get predictable output during test
+            list(  # list(set(...))) to deduplicate results
+                set(
+                    [s.strip() for s in data["status"]],
+                ),
+            ),
+        )
+        if "" in self.statuses:
+            self.statuses = self._cleanupArray(self.statuses)
+
+    def _doOptionalFields(
+        self,
+        data: Dict[str, Any],
+    ) -> None:
+        # optional fiels
         if "owner" in data:
             self.owner = data["owner"][0].strip()
 
         if "abuse_contact" in data:
             self.abuse_contact = data["abuse_contact"][0].strip()
 
         if "reseller" in data:
@@ -115,14 +107,54 @@
             self.emails = sorted(  # sorted added to get predictable output during test
                 list(  # list(set(...))) to deduplicate results
                     set(
                         [s.strip() for s in data["emails"]],
                     ),
                 ),
             )
+            if "" in self.emails:
+                self.emails = self._cleanupArray(self.emails)
+
+    def __init__(
+        self,
+        data: Dict[str, Any],
+        whois_str: Optional[str] = None,
+        verbose: bool = False,
+        include_raw_whois_text: bool = False,
+        return_raw_text_for_unsupported_tld: bool = False,
+        exeptionStr: Optional[str] = None,
+    ):
+        if include_raw_whois_text and whois_str is not None:
+            self.text = whois_str
+
+        if exeptionStr is not None:
+            self._exception = exeptionStr
+            return
+
+        self.name = data["domain_name"][0].strip().lower()
+        self.tld = data["tld"].lower()
+
+        if return_raw_text_for_unsupported_tld is True:
+            return
+
+        # process mandatory fields that we expact always to be present even if we have None or ''
+        self.registrar = data["registrar"][0].strip()
+        self.registrant_country = data["registrant_country"][0].strip()
+
+        # date time items
+        self.creation_date = str_to_date(data["creation_date"][0], self.tld, verbose=verbose)
+        self.expiration_date = str_to_date(data["expiration_date"][0], self.tld, verbose=verbose)
+        self.last_updated = str_to_date(data["updated_date"][0], self.tld, verbose=verbose)
+
+        self.dnssec = data["DNSSEC"]
+        self._doStatus(data)
+        self._doNameservers(data)
+
+        # optional fiels
+        self._doOptionalFields(data)
 
 
 # http://docs.python.org/library/datetime.html#strftime-strptime-behavior
 DATE_FORMATS = [
     "%d-%b-%Y",  # 02-jan-2000
     "%d-%m-%Y",  # 02-01-2000
     "%d.%m.%Y",  # 02.02.2000
@@ -182,15 +214,19 @@
 ]
 
 CUSTOM_DATE_FORMATS = {
     "ml": "%m/%d/%Y",
 }
 
 
-def str_to_date(text: str, tld: Optional[str] = None, verbose: bool = False) -> Optional[datetime.datetime]:
+def str_to_date(
+    text: str,
+    tld: Optional[str] = None,
+    verbose: bool = False,
+) -> Optional[datetime.datetime]:
     text = text.strip().lower()
 
     if verbose:
         print(f"tld: {tld}; str_to_date: {text}", file=sys.stderr)
 
     noDate = [
         "not defined",
@@ -223,15 +259,22 @@
 
     # Remove consecutive whitespace
     text = re.sub(r"\s\s+", r" ", text)
 
     # 07 january 2020 at 23:38:30.772
     # %d %B %Y at %H:%M %S.%f
     if tld and tld in CUSTOM_DATE_FORMATS:
-        return datetime.datetime.strptime(text, CUSTOM_DATE_FORMATS[tld]).astimezone().replace(tzinfo=None)
+        return (
+            datetime.datetime.strptime(
+                text,
+                CUSTOM_DATE_FORMATS[tld],
+            )
+            .astimezone()
+            .replace(tzinfo=None)
+        )
 
     for f in DATE_FORMATS:
         try:
             if verbose:
                 print(f"try with {f} on text: {text}", file=sys.stderr)
             z = datetime.datetime.strptime(text, f)
             z = z.astimezone()
```

### Comparing `whoisdomain-1.20230503.1/whoisdomain/exceptions.py` & `whoisdomain-1.20230525.5/whoisdomain/exceptions.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230503.1/whoisdomain/main.py` & `whoisdomain-1.20230525.5/whoisdomain/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,24 +201,25 @@
 
 
 def testItem(
     d: str,
     printgetRawWhoisResult: bool = False,
 ) -> None:
     global PrintGetRawWhoisResult
+    global SIMPLISTIC
 
-    timout = 30  # seconds
+    timeout = 30  # seconds
 
     w = whois.query(
         d,
         ignore_returncode=IgnoreReturncode,
         verbose=Verbose,
         internationalized=True,
         include_raw_whois_text=PrintGetRawWhoisResult,
-        timeout=timout,
+        timeout=timeout,
         simplistic=SIMPLISTIC,
     )
 
     if w is None:
         print("None")
         print("\n", whois.get_last_raw_whois_data())
         return
@@ -475,18 +476,14 @@
 
     name: str = os.path.basename(sys.argv[0])
     if name == "test2.py":
         SIMPLISTIC = False
     else:
         SIMPLISTIC = True
 
-    if 0:
-        print(name, SIMPLISTIC)
-        exit(0)
-
     try:
         opts, args = getopt.getopt(
             sys.argv[1:],
             "jRSpvVIhaf:d:D:r:H:C:",
             [
                 "json",
                 "Ruleset",
@@ -592,21 +589,23 @@
                 testAllTld = False
 
         if opt in ("-d", "--domain"):
             domain = arg
             if domain not in domains:
                 domains.append(domain)
 
+    if Verbose:
+        print(f"{name} SIMPLISTIC: {SIMPLISTIC}", file=sys.stderr)
+
     if Ruleset is True and len(domains):
         for domain in domains:
             ShowRuleset(domain)
         sys.exit(0)
 
     if testAllTld:
-        print("## ===== TEST CURRENT TLD's")
         allMetaTld = makeMetaAllCurrentTld(allHaving, allRegex)
         testDomains(allMetaTld)
         showFailures()
         sys.exit(0)
 
     if len(dirs):
         fileData = {}
```

### Comparing `whoisdomain-1.20230503.1/whoisdomain/tld_regexpr.py` & `whoisdomain-1.20230525.5/whoisdomain/tld_regexpr.py`

 * *Files 25% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "expiration_date": r"(?:Expiry|Expiration) Date:[ \t]*([^\n]*)",  # Expiration Date
     "updated_date": r"Updated Date:[\t ]*([^\n]*)",
     "name_servers": r"Name Server:\s*(.+)\s*",  # host -t ns <domain> often has more nameservers then the output of whois
     "status": r"Status:\s?(.+)",
     # the trailing domain must have minimal 2 parts firstname.lastname@fld.tld
     # it may actually have more then 4 levels
     # to match the dot in firstname.lastname we must use \.
-    "emails": r"[\w\.-]+@[\w\.-]+\.[\w]{2,4}",
+    "emails": r"([\w\.-]+@[\w\.-]+\.[\w]{2,4})",
 }
 
 # United Kingdom - academic sub-domain
 ZZ["ac.uk"] = {
     "extend": "uk",
     "domain_name": r"Domain:\n\s?(.+)",
     "owner": r"Domain Owner:\n\s?(.+)",
@@ -184,25 +184,27 @@
     "expiration_date": r"Registry Expiry Date:\s?(.+)",
     "updated_date": r"Updated Date:\s?(.+)",
     "status": None,
 }
 
 ZZ["br"] = {
     "extend": "com",
+    "_server": "whois.registro.br",
     "domain_name": r"domain:\s?(.+)",
     "registrar": "nic.br",
     "registrant": None,
     "owner": r"owner:\s?(.+)",
     "creation_date": r"created:\s?(.+)",
     "expiration_date": r"expires:\s?(.+)",
     "updated_date": r"changed:\s?(.+)",
     "name_servers": r"nserver:\s*(.+)",
     "status": r"status:\s?(.+)",
 }
 
+
 ZZ["by"] = {  # fix multiple dns by removing test for \n at the beginning as it is not needed
     "extend": "com",
     "domain_name": r"Domain Name:\s*(.+)",
     "registrar": r"Registrar:\s*(.+)",
     "registrant": r"Org:\s*(.+)",
     "registrant_country": r"Country:\s*(.+)",
     "creation_date": r"Creation Date:\s*(.+)",
@@ -392,19 +394,20 @@
     "registrant": r"Registrant:\nname:\s+(.+)\n",
     "registrant_country": r"Registrant:(?:\n+.+\n*)*country:\s+(.+)\n",
     "creation_date": r"Domain:(?:\n+.+\n*)*registered:\s+(.+)\n",
     "expiration_date": r"Domain:(?:\n+.+\n*)*expire:\s+(.+)\n",
     "updated_date": r"Domain:(?:\n+.+\n*)*changed:\s+(.+)\n",
     "name_servers": r"nserver:\s*(.+)",
     "status": r"Domain:(?:\n+.+\n*)*status:\s+(.+)\n",
-    "emails": r"[\w\.-]+@[\w\.-]+\.[\w]{2,4}",
+    # "emails": r"[\w\.-]+@[\w\.-]+\.[\w]{2,4}",
 }
 
 ZZ["eu"] = {
     "extend": "com",
+    "_server": "whois.eu",
     "registrar": r"Name:\s?(.+)",
     "domain_name": r"\nDomain:\s*(.+)",
     "name_servers": r"Name servers:\n(?:\s+(\S+)\n)(?:\s+(\S+)\n)?(?:\s+(\S+)\n)?(?:\s+(\S+)\n)?(?:\s+(\S+)\n)?(?:\s+(\S+)\n)\n?",
 }
 
 ZZ["fi"] = {
     "extend": None,
@@ -456,14 +459,15 @@
 ZZ["hn"] = {
     "extend": "com",
 }
 
 # Hong Kong
 ZZ["hk"] = {
     "extend": "com",
+    "_server": "whois.hkirc.hk",
     "domain_name": r"Domain Name:\s+(.+)",
     "registrar": r"Registrar Name:\s?(.+)",
     "registrant": r"Company English Name.*:\s?(.+)",
     "registrant_country": None,
     "creation_date": r"Domain Name Commencement Date:\s?(.+)",
     "expiration_date": r"Expiry Date:\s?(.+)",
     "updated_date": None,
@@ -492,17 +496,15 @@
     "registrant_country": None,
     "creation_date": "",
     "expiration_date": r"Expiry Date:\s?(.+)",
     "updated_date": "",
     "name_servers": r"Name Server:(.+)",
 }
 
-ZZ["in"] = {
-    "extend": "com",
-}
+ZZ["in"] = {"extend": "com", "_server": "whois.registry.in"}
 
 ZZ["info"] = {
     "extend": "com",
 }
 
 ZZ["ink"] = {
     "extend": "amsterdam",
@@ -522,24 +524,25 @@
     "status": None,
     "expiration_date": r"expire-date:\s?(.+)",
     "updated_date": r"last-updated:\s?(.+)",
     "name_servers": r"nserver:\s*(.+)\s*",
 }
 
 ZZ["is"] = {
+    "extend": "com",
     "domain_name": r"domain:\s?(.+)",
     "registrar": None,
     "registrant": r"registrant:\s?(.+)",
     "registrant_country": None,
     "creation_date": r"created:\s?(.+)",
     "expiration_date": r"expires:\s?(.+)",
     "updated_date": None,
     "name_servers": r"nserver:\s?(.+)",
     "status": None,
-    "emails": r"[\w\.-]+@[\w\.-]+\.[\w]{2,4}",
+    # "emails": r"[\w\.-]+@[\w\.-]+\.[\w]{2,4}",
 }
 
 ZZ["it"] = {
     "extend": "com",
     "domain_name": r"Domain:\s?(.+)",
     "registrar": r"Registrar\s*Organization:\s*(.+)",
     "registrant": r"Registrant\s*Organization:\s*(.+)",
@@ -567,15 +570,15 @@
     #    'updated_date':             r'\[最終更新\]\s?(.+)',
     "creation_date": r"\[Created on\]\s?(.+)",
     "expiration_date": r"\[Expires on\]\s?(.+)",
     "updated_date": r"\[Last Updated\]\s?(.+)",
     "name_servers": r"\[Name Server\]\s*(.+)",
     #    'status':                   r'\[状態\]\s?(.+)',
     "status": r"\[Status\]\s?(.+)",
-    "emails": r"[\w\.-]+@[\w\.-]+\.[\w]{2,4}",
+    "emails": r"([\w\.-]+@[\w\.-]+\.[\w]{2,4})",
 }
 
 # The Japanese whois servers always return English unless a Japanese locale is specified in the user's LANG environmental variable.
 # See: https://www.computerhope.com/unix/uwhois.htm
 # Additionally, whois qeuries can explicitly request english:
 # 	To suppress Japanese output, add'/e' at the end of command, e.g. 'whois -h whois.jprs.jp xxx/e'.
 #
@@ -620,14 +623,15 @@
 # Saint Kitts and Nevis
 ZZ["kn"] = {
     "extend": "com",
 }
 
 ZZ["kr"] = {
     "extend": "com",
+    "_server": "whois.kr",
     "domain_name": r"Domain Name\s*:\s?(.+)",
     "registrar": r"Authorized Agency\s*:\s*(.+)",
     "registrant": r"Registrant\s*:\s*(.+)",
     "creation_date": r"Registered Date\s*:\s?(.+)",
     "expiration_date": r"Expiration Date\s*:\s?(.+)",
     "updated_date": r"Last Updated Date\s*:\s?(.+)",
     "status": r"status\s*:\s?(.+)",
@@ -681,15 +685,15 @@
     "domain_name": r"Domain name:\s*([^(i|\n)]+)",
     "registrar": r"(?<=Owner contact:\s)[\s\S]*?Organization:(.*)",
     "registrant_country": r"(?<=Owner contact:\s)[\s\S]*?Country:(.*)",
     "registrant": r"(?<=Owner contact:\s)[\s\S]*?Name:(.*)",
     "creation_date": r"Domain registered: *(.+)",
     "expiration_date": r"Record will expire on: *(.+)",
     "name_servers": r"Domain Nameservers:\s*(.+)\n\s*(.+)\n",
-    "emails": r"[\w\.-]+@[\w\.-]+\.[\w]{2,4}",
+    # "emails": r"[\w\.-]+@[\w\.-]+\.[\w]{2,4}",
 }
 
 ZZ["mobi"] = {
     "extend": "com",
     "expiration_date": r"\nRegistry Expiry Date:\s?(.+)",
     "updated_date": r"\nUpdated Date:\s?(.+)",
 }
@@ -801,27 +805,25 @@
     "registrant": r"registrant_contact_name:\s?(.+)",
     "registrant_country": None,
     "creation_date": r"domain_dateregistered:\s?(.+)",
     "expiration_date": r"domain_datebilleduntil:\s?(.+)",
     "updated_date": r"domain_datelastmodified:\s?(.+)",
     "name_servers": r"ns_name_[0-9]{2}:\s?(.+)",
     "status": r"query_status:\s?(.+)",
-    "emails": r"[\w\.-]+@[\w\.-]+\.[\w]{2,4}",
+    "emails": r"([\w\.-]+@[\w\.-]+\.[\w]{2,4})",
 }
 
 ZZ["org"] = {
     "extend": "com",
     "expiration_date": r"\nRegistry Expiry Date:\s?(.+)",
     "updated_date": r"\nLast Updated On:\s?(.+)",
     "name_servers": r"Name Server:\s?(.+)\s*",
 }
 
-ZZ["ovh"] = {
-    "extend": "com",
-}
+ZZ["ovh"] = {"extend": "com", "_server": "whois.nic.ovh"}
 
 ZZ["pe"] = {
     "extend": "com",
     "registrant": r"Registrant Name:\s?(.+)",
     "admin": r"Admin Name:\s?(.+)",
 }
 
@@ -1027,15 +1029,15 @@
     "registrant": r"Owner Contact\n+Name\.+:\s?(.+)",
     "registrant_country": r"Owner Contact\n(?:.+\n)+Country\.+:\s(.+)",
     "creation_date": r"Creation date\.+:\s?(.+)",
     "expiration_date": None,
     "updated_date": None,
     "name_servers": r"DNS servers\n(?:Name\.+:\s*(\S+)\n)(?:Name\.+:\s*(\S+)\n)?(?:Name\.+:\s*(\S+)\n)?(?:Name\.+:\s*(\S+)\n)?",
     "status": r"Domain status\.+:(.+)",
-    "emails": r"[\w\.-]+@[\w\.-]+\.[\w]{2,4}",
+    # "emails": r"[\w\.-]+@[\w\.-]+\.[\w]{2,4}",
 }
 
 ZZ["tokyo"] = {
     "extend": "com",
     "_server": "whois.nic.tokyo",
 }
 
@@ -1740,14 +1742,15 @@
     "_server": "whois.nic.td",
     "extend": "ac",
     "registrant_country": r"Registrant Country:\s+(.+)",
 }
 
 ZZ["tw"] = {
     "extend": None,
+    "_server": "whois.twnic.net.tw",
     "domain_name": r"Domain Name:\s+(.+)",
     "creation_date": r"\s+Record created on\s+(.+)",
     "expiration_date": r"\s+Record expires on\s+(.+)",
     "status": r"\s+Domain Status:\s+(.+)",
     "registrar": r"Registration\s+Service\s+Provider:\s+(.+)",
     "updated_date": None,
     "registrant_country": None,
@@ -2080,14 +2083,22 @@
     # to match the dot in firstname.lastname we must use \.
     "emails": r"[\w\.-]+@[\w\.-]+\.[\w]{2,4}",
 }
 
 ZZ["observer"] = {"extend": "com", "_server": "whois.nic.observer"}
 ZZ["one"] = {"extend": "com", "_server": "whois.nic.one"}
 ZZ["page"] = {"extend": "com", "_server": "whois.nic.google"}
+ZZ["esq"] = {"extend": "com", "_server": "whois.nic.google"}
+ZZ["dad"] = {"extend": "com", "_server": "whois.nic.google"}
+ZZ["foo"] = {"extend": "com", "_server": "whois.nic.google"}
+ZZ["mov"] = {"extend": "com", "_server": "whois.nic.google"}
+ZZ["nexus"] = {"extend": "com", "_server": "whois.nic.google"}
+ZZ["phd"] = {"extend": "com", "_server": "whois.nic.google"}
+ZZ["prof"] = {"extend": "com", "_server": "whois.nic.google"}
+ZZ["zip"] = {"extend": "com", "_server": "whois.nic.google"}
 
 ZZ["bf"] = {
     "extend": "com",
     "_server": "whois.nic.bf",
     "registrant": r"Registrant Name:\s?(.+)",
 }
 ZZ["bz"] = {"extend": "_privateReg"}
@@ -2764,7 +2775,459 @@
     "extend": "com",
     # "expiration_date": r"Registry Expiry Date:\s?(.+)",
 }
 ZZ["онлайн"] = {
     "extend": "com",
     # "expiration_date": r"Registry Expiry Date:\s?(.+)",
 }
+
+ZZ["ps"] = {
+    # Registrant Name
+    "extend": "com",
+    "registrant": r"Registrant\s+Name:\s?(.+)",
+}
+
+# experimental autodetect via iana tld
+
+ZZ["abarth"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["abbott"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["active"] = {"_privateRegistry": True}
+ZZ["adac"] = {"_privateRegistry": True}
+ZZ["afamilycompany"] = {"_privateRegistry": True}
+ZZ["agakhan"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["aigo"] = {"_privateRegistry": True}
+ZZ["akdn"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["alfaromeo"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["allstate"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["an"] = {"_privateRegistry": True}
+ZZ["apple"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["audi"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["avianca"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["beats"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["bl"] = {"_privateRegistry": True}
+ZZ["blanco"] = {"_privateRegistry": True}
+ZZ["bnl"] = {"_privateRegistry": True}
+ZZ["bnpparibas"] = {"_server": "whois.afilias-srs.net", "extend": "com"}  # 'group.bnpparibas' works
+ZZ["boehringer"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["boots"] = {"_privateRegistry": True}
+ZZ["bq"] = {"_privateRegistry": True}
+ZZ["budapest"] = {"_privateRegistry": True}
+ZZ["bugatti"] = {"_privateRegistry": True}
+ZZ["cancerresearch"] = {"_privateRegistry": True}
+ZZ["cartier"] = {"_privateRegistry": True}
+ZZ["caseih"] = {"_privateRegistry": True}
+ZZ["cbs"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["ceb"] = {"_privateRegistry": True}
+ZZ["cern"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["chloe"] = {"_privateRegistry": True}
+ZZ["chrysler"] = {"_privateRegistry": True}
+ZZ["cipriani"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["creditunion"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["csc"] = {"_privateRegistry": True}
+ZZ["dabur"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["dodge"] = {"_privateRegistry": True}
+ZZ["doha"] = {"_privateRegistry": True}
+ZZ["doosan"] = {"_privateRegistry": True}
+ZZ["duck"] = {"_privateRegistry": True}
+ZZ["duns"] = {"_privateRegistry": True}
+ZZ["edeka"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["eh"] = {"_privateRegistry": True}
+ZZ["emerck"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["epost"] = {"_privateRegistry": True}
+ZZ["esurance"] = {"_privateRegistry": True}
+ZZ["everbank"] = {"_privateRegistry": True}
+ZZ["extraspace"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["fage"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["fiat"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["fido"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["flsmidth"] = {"_privateRegistry": True}
+ZZ["fujixerox"] = {"_privateRegistry": True}
+ZZ["glade"] = {"_privateRegistry": True}
+ZZ["goodhands"] = {"_privateRegistry": True}
+ZZ["hermes"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["honeywell"] = {"_privateRegistry": True}
+ZZ["htc"] = {"_privateRegistry": True}
+ZZ["iinet"] = {"_privateRegistry": True}
+ZZ["imamat"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["intel"] = {"_privateRegistry": True}
+ZZ["iselect"] = {"_privateRegistry": True}
+ZZ["ismaili"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["itv"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["iveco"] = {"_privateRegistry": True}
+ZZ["iwc"] = {"_privateRegistry": True}
+ZZ["jcp"] = {"_privateRegistry": True}
+ZZ["jeep"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["jlc"] = {"_privateRegistry": True}
+ZZ["jll"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["ladbrokes"] = {"_privateRegistry": True}
+ZZ["lamborghini"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["lancia"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["lancome"] = {"_privateRegistry": True}
+ZZ["lasalle"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["liaison"] = {"_privateRegistry": True}
+ZZ["lixil"] = {"_privateRegistry": True}
+ZZ["loft"] = {"_privateRegistry": True}
+ZZ["lupin"] = {"_privateRegistry": True}
+ZZ["marriott"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["mcd"] = {"_privateRegistry": True}
+ZZ["mcdonalds"] = {"_privateRegistry": True}
+ZZ["meo"] = {"_privateRegistry": True}
+ZZ["metlife"] = {"_privateRegistry": True}
+ZZ["mf"] = {"_privateRegistry": True}
+ZZ["mit"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["mobily"] = {"_privateRegistry": True}
+ZZ["montblanc"] = {"_privateRegistry": True}
+ZZ["mopar"] = {"_privateRegistry": True}
+ZZ["movistar"] = {"_privateRegistry": True}
+ZZ["mtpc"] = {"_privateRegistry": True}
+ZZ["mutuelle"] = {"_privateRegistry": True}
+ZZ["nadex"] = {"_privateRegistry": True}
+ZZ["nationwide"] = {"_privateRegistry": True}
+ZZ["newholland"] = {"_privateRegistry": True}
+ZZ["nokia"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["nra"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["off"] = {"_privateRegistry": True}
+ZZ["onyourside"] = {"_privateRegistry": True}
+ZZ["orientexpress"] = {"_privateRegistry": True}
+ZZ["pamperedchef"] = {"_privateRegistry": True}
+ZZ["panerai"] = {"_privateRegistry": True}
+ZZ["piaget"] = {"_privateRegistry": True}
+ZZ["progressive"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["pwc"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["qvc"] = {"_privateRegistry": True}
+ZZ["raid"] = {"_privateRegistry": True}
+ZZ["redumbrella"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["rightathome"] = {"_privateRegistry": True}
+ZZ["rmit"] = {"_privateRegistry": True}
+ZZ["rogers"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["sapo"] = {"_privateRegistry": True}
+ZZ["schaeffler"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["scjohnson"] = {"_privateRegistry": True}
+ZZ["scor"] = {"_privateRegistry": True}
+ZZ["ses"] = {"_privateRegistry": True}
+ZZ["sew"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["shaw"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["showtime"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["shriram"] = {"_privateRegistry": True}
+ZZ["spiegel"] = {"_privateRegistry": True}
+ZZ["spreadbetting"] = {"_privateRegistry": True}
+ZZ["srt"] = {"_privateRegistry": True}
+ZZ["stada"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["starhub"] = {"_privateRegistry": True}
+ZZ["statoil"] = {"_privateRegistry": True}
+ZZ["stockholm"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["swiftcover"] = {"_privateRegistry": True}
+ZZ["symantec"] = {"_privateRegistry": True}
+ZZ["telecity"] = {"_privateRegistry": True}
+ZZ["telefonica"] = {"_privateRegistry": True}
+ZZ["temasek"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["tp"] = {"_privateRegistry": True}
+ZZ["travelers"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["travelersinsurance"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["trv"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["uconnect"] = {"_privateRegistry": True}
+ZZ["um"] = {"_privateRegistry": True}
+ZZ["viking"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["vista"] = {"_privateRegistry": True}
+ZZ["vistaprint"] = {"_privateRegistry": True}
+ZZ["volkswagen"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["warman"] = {"_privateRegistry": True}
+ZZ["xn--0zwm56d"] = {"_privateRegistry": True}
+ZZ["xn--11b5bs3a9aj6g"] = {"_privateRegistry": True}
+ZZ["xn--3oq18vl8pn36a"] = {"_privateRegistry": True}
+ZZ["xn--80akhbyknj4f"] = {"_privateRegistry": True}
+ZZ["xn--9t4b11yi5a"] = {"_privateRegistry": True}
+ZZ["xn--b4w605ferd"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["xn--deba0ad"] = {"_privateRegistry": True}
+ZZ["xn--estv75g"] = {"_privateRegistry": True}
+ZZ["xn--g6w251d"] = {"_privateRegistry": True}
+ZZ["xn--hgbk6aj7f53bba"] = {"_privateRegistry": True}
+ZZ["xn--hlcj6aya9esc7a"] = {"_privateRegistry": True}
+ZZ["xn--jlq61u9w7b"] = {"_privateRegistry": True}
+ZZ["xn--jxalpdlp"] = {"_privateRegistry": True}
+ZZ["xn--kgbechtv"] = {"_privateRegistry": True}
+ZZ["xn--kpu716f"] = {"_privateRegistry": True}
+ZZ["xn--mgbb9fbpob"] = {"_privateRegistry": True}
+ZZ["xn--pbt977c"] = {"_privateRegistry": True}
+ZZ["xn--zckzah"] = {"_privateRegistry": True}
+ZZ["xperia"] = {"_privateRegistry": True}
+ZZ["zara"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["zippo"] = {"_privateRegistry": True}
+ZZ["gi"] = {"_server": "whois2.afilias-grs.net", "extend": "com"}
+ZZ["ads"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["android"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["cal"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["chrome"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["dclk"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["docs"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["drive"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["eat"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["fly"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["gbiz"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["gle"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["gmail"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["goog"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["guge"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["hangout"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["here"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["ing"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["map"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["meet"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["meme"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["play"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["prod"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["search"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["xn--flw351e"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["xn--qcka1pmc"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["youtube"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["datsun"] = {"_server": "whois.nic.gmo", "extend": "com"}
+ZZ["fujitsu"] = {"_server": "whois.nic.gmo", "extend": "com"}
+ZZ["goo"] = {"_server": "whois.nic.gmo", "extend": "com"}
+ZZ["hisamitsu"] = {"_server": "whois.nic.gmo", "extend": "com"}
+ZZ["hitachi"] = {"_server": "whois.nic.gmo", "extend": "com"}
+ZZ["infiniti"] = {"_server": "whois.nic.gmo", "extend": "com"}
+ZZ["jcb"] = {"_server": "whois.nic.gmo", "extend": "com"}
+ZZ["mitsubishi"] = {"_server": "whois.nic.gmo", "extend": "com"}
+ZZ["nissan"] = {"_server": "whois.nic.gmo", "extend": "com"}
+ZZ["panasonic"] = {"_server": "whois.nic.gmo", "extend": "com"}
+ZZ["sharp"] = {"_server": "whois.nic.gmo", "extend": "com"}
+ZZ["yodobashi"] = {"_server": "whois.nic.gmo", "extend": "com"}
+ZZ["baidu"] = {"_server": "whois.gtld.knet.cn", "extend": "com"}
+ZZ["xn--30rr7y"] = {"_server": "whois.gtld.knet.cn", "extend": "com"}
+ZZ["xn--3bst00m"] = {"_server": "whois.gtld.knet.cn", "extend": "com"}
+ZZ["xn--9et52u"] = {"_server": "whois.gtld.knet.cn", "extend": "com"}
+ZZ["xn--fiq64b"] = {"_server": "whois.gtld.knet.cn", "extend": "com"}
+ZZ["xn--clchc0ea0b2g2a9gcd"] = {"_server": "whois.sgnic.sg", "extend": "sg"}
+ZZ["xn--yfro4i67o"] = {"_server": "whois.sgnic.sg", "extend": "sg"}
+ZZ["anquan"] = {"extend": "_teleinfo"}
+ZZ["shouji"] = {"extend": "_teleinfo"}
+ZZ["xihuan"] = {"extend": "_teleinfo"}
+ZZ["xn--vuq861b"] = {"extend": "_teleinfo"}
+ZZ["yun"] = {"extend": "_teleinfo"}
+ZZ["etisalat"] = {"extend": "_centralnic"}
+ZZ["xn--mgbaakc7dvf"] = {"extend": "_centralnic"}
+ZZ["xn--2scrj9c"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["xn--3hcrj9c"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["xn--45br5cyl"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["xn--45brj9c"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["xn--fpcrj9c3d"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["xn--gecrj9c"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["xn--h2breg3eve"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["xn--h2brj9c"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["xn--h2brj9c8c"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["xn--mgbbh1a"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["xn--mgbbh1a71e"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["xn--mgbgu82a"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["xn--rvc1e0am3e"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["xn--s9brj9c"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["xn--xkc2dl3a5ee0h"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["xn--xhq521b"] = {"_server": "whois.ngtld.cn", "extend": "com"}
+ZZ["xn--kprw13d"] = {"extend": "tw"}
+ZZ["xn--kpry57d"] = {"extend": "tw"}
+ZZ["th"] = {"_server": "whois.thnic.co.th", "extend": "co.th"}
+# whois.thnic.co.th ['co.th']
+ZZ["xn--d1alf"] = {"_server": "whois.marnet.mk", "extend": "mk"}
+# whois.marnet.mk ['mk']
+ZZ["xn--mgb9awbf"] = {"_server": "whois.registry.om", "extend": "om"}
+# whois.registry.om ['om']
+ZZ["xn--mgbah1a3hjkrd"] = {"_server": "whois.nic.mr", "extend": "mr"}
+# whois.nic.mr ['mr']
+ZZ["xn--mix891f"] = {"_server": "whois.monic.mo", "extend": "mo"}
+# whois.monic.mo ['mo']
+ZZ["xn--o3cw4h"] = {"_server": "whois.thnic.co.th", "extend": "co.th"}
+# whois.thnic.co.th ['co.th']
+ZZ["xn--ogbpf8fl"] = {"_server": "whois.tld.sy", "extend": "sy"}
+# whois.tld.sy ['sy']
+ZZ["xn--wgbl6a"] = {"_server": "whois.registry.qa", "extend": "qa"}
+# whois.registry.qa ['qa']
+ZZ["xn--j6w193g"] = {"_server": "whois.hkirc.hk", "extend": "hk"}
+# whois.hkirc.hk ['hk']
+ZZ["xn--e1a4c"] = {"_server": "whois.eu", "extend": "eu"}
+# whois.eu ['eu']
+ZZ["xn--qxa6a"] = {"_server": "whois.eu", "extend": "eu"}
+# whois.eu ['eu']
+
+ZZ["bom"] = {"extend": "com", "_server": "whois.gtlds.nic.br"}
+ZZ["final"] = {"_server": "whois.gtlds.nic.br", "extend": "bom"}
+# whois.gtlds.nic.br ['bom']
+ZZ["globo"] = {"_server": "whois.gtlds.nic.br", "extend": "bom"}
+# whois.gtlds.nic.br ['bom']
+ZZ["natura"] = {"_server": "whois.gtlds.nic.br", "extend": "bom"}
+# whois.gtlds.nic.br ['bom']
+ZZ["rio"] = {"_server": "whois.gtlds.nic.br", "extend": "bom"}
+# whois.gtlds.nic.br ['bom']
+ZZ["uol"] = {"_server": "whois.gtlds.nic.br", "extend": "bom"}
+# whois.gtlds.nic.br ['bom']
+ZZ["xn--3e0b707e"] = {"_server": "whois.kr", "extend": "kr"}
+# whois.kr ['kr']
+ZZ["xn--cg4bki"] = {"_server": "whois.kr", "extend": "kr"}
+# whois.kr ['kr']
+
+# testing  unicode domains autodetect
+ZZ["测试"] = {"_privateRegistry": True}
+# ZZ["कम"] = {"_server": "whois.nic.xn--11b4c3d", "extend": "xn--11b4c3d"} # whois.nic.xn--11b4c3d ['xn--11b4c3d']
+ZZ["परकष"] = {"_privateRegistry": True}
+ZZ["佛山"] = {"_server": "whois.ngtld.cn", "extend": "com"}
+ZZ["ಭರತ"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["慈善"] = {"_server": "whois.gtld.knet.cn", "extend": "com"}
+ZZ["集团"] = {"_server": "whois.gtld.knet.cn", "extend": "com"}
+ZZ["한국"] = {"_server": "whois.kr", "extend": "kr"}  # whois.kr ['kr', 'xn--3e0b707e', 'xn--cg4bki']
+ZZ["ଭରତ"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["大众汽车"] = {"_privateRegistry": True}
+ZZ["点看"] = {"_server": "whois.nic.xn--3pxu8k", "extend": "xn--3pxu8k"}  # whois.nic.xn--3pxu8k ['xn--3pxu8k']
+ZZ["คอม"] = {"_server": "whois.nic.xn--42c2d9a", "extend": "xn--42c2d9a"}  # whois.nic.xn--42c2d9a ['xn--42c2d9a']
+ZZ["ভৰত"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["ভরত"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["موقع"] = {"_server": "whois.nic.xn--4gbrim", "extend": "xn--4gbrim"}  # whois.nic.xn--4gbrim ['xn--4gbrim']
+ZZ["公司"] = {"_server": "whois.ngtld.cn", "extend": "com"}
+ZZ["香格里拉"] = {
+    "_server": "whois.nic.xn--5su34j936bgsg",
+    "extend": "xn--5su34j936bgsg",
+}  # whois.nic.xn--5su34j936bgsg ['xn--5su34j936bgsg']
+ZZ["网站"] = {"_server": "whois.nic.xn--5tzm5g", "extend": "xn--5tzm5g"}  # whois.nic.xn--5tzm5g ['xn--5tzm5g']
+ZZ["移动"] = {"_server": "whois.nic.xn--6frz82g", "extend": "xn--6frz82g"}  # whois.nic.xn--6frz82g ['xn--6frz82g']
+ZZ["我爱你"] = {"_server": "whois.gtld.knet.cn", "extend": "com"}
+ZZ["москва"] = {
+    "_server": "whois.nic.xn--80adxhks",
+    "extend": "xn--80adxhks",
+}  # whois.nic.xn--80adxhks ['xn--80adxhks']
+ZZ["испытание"] = {"_privateRegistry": True}
+ZZ["католик"] = {
+    "_server": "whois.nic.xn--80aqecdr1a",
+    "extend": "xn--80aqecdr1a",
+}  # whois.nic.xn--80aqecdr1a ['xn--80aqecdr1a']
+ZZ["сайт"] = {"_server": "whois.nic.xn--80aswg", "extend": "xn--80aswg"}  # whois.nic.xn--80aswg ['xn--80aswg']
+ZZ["联通"] = {"_server": "whois.gtld.knet.cn", "extend": "com"}
+ZZ["קום"] = {"_server": "whois.nic.xn--9dbq2a", "extend": "xn--9dbq2a"}  # whois.nic.xn--9dbq2a ['xn--9dbq2a']
+ZZ["时尚"] = {"_server": "whois.gtld.knet.cn", "extend": "com"}
+ZZ["微博"] = {"_server": "whois.nic.xn--9krt00a", "extend": "xn--9krt00a"}  # whois.nic.xn--9krt00a ['xn--9krt00a']
+ZZ["테스트"] = {"_privateRegistry": True}
+ZZ["淡马锡"] = {"_server": "whois.afilias-srs.net", "extend": "com"}
+ZZ["орг"] = {"_server": "whois.nic.xn--c1avg", "extend": "xn--c1avg"}  # whois.nic.xn--c1avg ['xn--c1avg']
+ZZ["नट"] = {"_server": "whois.nic.xn--c2br7g", "extend": "xn--c2br7g"}  # whois.nic.xn--c2br7g ['xn--c2br7g']
+ZZ["アマゾン"] = {
+    "_server": "whois.nic.xn--cckwcxetd",
+    "extend": "xn--cckwcxetd",
+}  # whois.nic.xn--cckwcxetd ['xn--cckwcxetd']
+ZZ["삼성"] = {"_server": "whois.kr", "extend": "kr"}  # whois.kr ['kr', 'xn--3e0b707e', 'xn--cg4bki']
+ZZ["சஙகபபர"] = {"_server": "whois.sgnic.sg", "extend": "sg"}
+ZZ["商店"] = {"_server": "whois.nic.xn--czrs0t", "extend": "xn--czrs0t"}  # whois.nic.xn--czrs0t ['xn--czrs0t']
+ZZ["мкд"] = {"_server": "whois.marnet.mk", "extend": "mk"}  # whois.marnet.mk ['mk', 'xn--d1alf']
+ZZ["טעסט"] = {"_privateRegistry": True}
+ZZ["ею"] = {"_server": "whois.eu", "extend": "eu"}  # whois.eu ['eu', 'xn--e1a4c', 'xn--qxa6a']
+ZZ["新闻"] = {"_server": "whois.gtld.knet.cn", "extend": "com"}
+ZZ["工行"] = {"_privateRegistry": True}
+ZZ["كوم"] = {"_server": "whois.nic.xn--fhbei", "extend": "xn--fhbei"}  # whois.nic.xn--fhbei ['xn--fhbei']
+ZZ["中信"] = {"_server": "whois.gtld.knet.cn", "extend": "com"}
+ZZ["中国"] = {"_server": "cwhois.cnnic.cn", "extend": "xn--fiqs8s"}  # cwhois.cnnic.cn ['xn--fiqs8s', 'xn--fiqz9s']
+ZZ["中國"] = {"_server": "cwhois.cnnic.cn", "extend": "xn--fiqs8s"}  # cwhois.cnnic.cn ['xn--fiqs8s', 'xn--fiqz9s']
+ZZ["娱乐"] = {"_server": "whois.nic.xn--fjq720a", "extend": "xn--fjq720a"}  # whois.nic.xn--fjq720a ['xn--fjq720a']
+ZZ["谷歌"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["భరత"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["電訊盈科"] = {
+    "_server": "whois.nic.xn--fzys8d69uvgm",
+    "extend": "xn--fzys8d69uvgm",
+}  # whois.nic.xn--fzys8d69uvgm ['xn--fzys8d69uvgm']
+ZZ["測試"] = {"_privateRegistry": True}
+ZZ["ભરત"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["भरतम"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["भरत"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["भरत"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["آزمایشی"] = {"_privateRegistry": True}
+ZZ["பரடச"] = {"_privateRegistry": True}
+ZZ["सगठन"] = {
+    "_server": "whois.nic.xn--i1b6b1a6a2e",
+    "extend": "xn--i1b6b1a6a2e",
+}  # whois.nic.xn--i1b6b1a6a2e ['xn--i1b6b1a6a2e']
+ZZ["网络"] = {"_server": "whois.ngtld.cn", "extend": "com"}
+ZZ["ком"] = {"_server": "whois.nic.xn--j1aef", "extend": "xn--j1aef"}  # whois.nic.xn--j1aef ['xn--j1aef']
+ZZ["香港"] = {"_server": "whois.hkirc.hk", "extend": "hk"}  # whois.hkirc.hk ['hk', 'xn--j6w193g']
+ZZ["亚马逊"] = {
+    "_server": "whois.nic.xn--jlq480n2rg",
+    "extend": "xn--jlq480n2rg",
+}  # whois.nic.xn--jlq480n2rg ['xn--jlq480n2rg']
+ZZ["诺基亚"] = {"_privateRegistry": True}
+ZZ["δοκιμή"] = {"_privateRegistry": True}
+ZZ["飞利浦"] = {
+    "_server": "whois.nic.xn--kcrx77d1x4a",
+    "extend": "xn--kcrx77d1x4a",
+}  # whois.nic.xn--kcrx77d1x4a ['xn--kcrx77d1x4a']
+ZZ["إختبار"] = {"_privateRegistry": True}
+ZZ["台湾"] = {"_server": "whois.twnic.net.tw", "extend": "tw"}
+ZZ["台灣"] = {"_server": "whois.twnic.net.tw", "extend": "tw"}
+ZZ["手表"] = {"_privateRegistry": True}
+ZZ["手机"] = {"_server": "whois.nic.xn--kput3i", "extend": "xn--kput3i"}  # whois.nic.xn--kput3i ['xn--kput3i']
+ZZ["عمان"] = {"_server": "whois.registry.om", "extend": "om"}  # whois.registry.om ['om', 'xn--mgb9awbf']
+ZZ["العليان"] = {
+    "_server": "whois.nic.xn--mgba7c0bbn0a",
+    "extend": "xn--mgba7c0bbn0a",
+}  # whois.nic.xn--mgba7c0bbn0a ['xn--mgba7c0bbn0a']
+ZZ["اتصالات"] = {"_server": "whois.centralnic.com", "extend": "_centralnic"}
+ZZ["بازار"] = {
+    "_server": "whois.nic.xn--mgbab2bd",
+    "extend": "xn--mgbab2bd",
+}  # whois.nic.xn--mgbab2bd ['xn--mgbab2bd']
+ZZ["موريتانيا"] = {"_server": "whois.nic.mr", "extend": "mr"}  # whois.nic.mr ['mr', 'xn--mgbah1a3hjkrd']
+ZZ["موبايلي"] = {"_privateRegistry": True}
+ZZ["بارت"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["بھارت"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["ابوظبي"] = {
+    "_server": "whois.nic.xn--mgbca7dzdo",
+    "extend": "xn--mgbca7dzdo",
+}  # whois.nic.xn--mgbca7dzdo ['xn--mgbca7dzdo']
+ZZ["ڀارت"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["كاثوليك"] = {
+    "_server": "whois.nic.xn--mgbi4ecexp",
+    "extend": "xn--mgbi4ecexp",
+}  # whois.nic.xn--mgbi4ecexp ['xn--mgbi4ecexp']
+ZZ["همراه"] = {
+    "_server": "whois.nic.xn--mgbt3dhd",
+    "extend": "xn--mgbt3dhd",
+}  # whois.nic.xn--mgbt3dhd ['xn--mgbt3dhd']
+ZZ["澳門"] = {"_server": "whois.monic.mo", "extend": "mo"}  # whois.monic.mo ['mo', 'xn--mix891f']
+ZZ["닷컴"] = {"_server": "whois.nic.xn--mk1bu44c", "extend": "xn--mk1bu44c"}  # whois.nic.xn--mk1bu44c ['xn--mk1bu44c']
+ZZ["政府"] = {"_server": "whois.nic.xn--mxtq1m", "extend": "xn--mxtq1m"}  # whois.nic.xn--mxtq1m ['xn--mxtq1m']
+ZZ["شبكة"] = {"_server": "whois.nic.xn--ngbc5azd", "extend": "xn--ngbc5azd"}  # whois.nic.xn--ngbc5azd ['xn--ngbc5azd']
+ZZ["بيتك"] = {"_server": "whois.nic.xn--ngbe9e0a", "extend": "xn--ngbe9e0a"}  # whois.nic.xn--ngbe9e0a ['xn--ngbe9e0a']
+ZZ["عرب"] = {"_server": "whois.nic.xn--ngbrx", "extend": "xn--ngbrx"}  # whois.nic.xn--ngbrx ['xn--ngbrx']
+ZZ["机构"] = {"_server": "whois.nic.xn--nqv7f", "extend": "xn--nqv7f"}  # whois.nic.xn--nqv7f ['xn--nqv7f']
+ZZ["组织机构"] = {
+    "_server": "whois.nic.xn--nqv7fs00ema",
+    "extend": "xn--nqv7fs00ema",
+}  # whois.nic.xn--nqv7fs00ema ['xn--nqv7fs00ema']
+ZZ["ไทย"] = {"_server": "whois.thnic.co.th", "extend": "co.th"}  # whois.thnic.co.th ['co.th', 'th', 'xn--o3cw4h']
+ZZ["سورية"] = {"_server": "whois.tld.sy", "extend": "sy"}  # whois.tld.sy ['sy', 'xn--ogbpf8fl']
+ZZ["珠宝"] = {"_privateRegistry": True}
+ZZ["大拿"] = {"_server": "whois.nic.xn--pssy2u", "extend": "xn--pssy2u"}  # whois.nic.xn--pssy2u ['xn--pssy2u']
+ZZ["みんな"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["グーグル"] = {"_server": "whois.nic.google", "extend": "com"}
+ZZ["ευ"] = {"_server": "whois.eu", "extend": "eu"}  # whois.eu ['eu', 'xn--e1a4c', 'xn--qxa6a']
+ZZ["ഭരത"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["ਭਰਤ"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["网址"] = {"_server": "whois.gtld.knet.cn", "extend": "com"}
+ZZ["닷넷"] = {"_server": "whois.nic.xn--t60b56a", "extend": "xn--t60b56a"}  # whois.nic.xn--t60b56a ['xn--t60b56a']
+ZZ["コム"] = {"_server": "whois.nic.xn--tckwe", "extend": "xn--tckwe"}  # whois.nic.xn--tckwe ['xn--tckwe']
+ZZ["天主教"] = {
+    "_server": "whois.nic.xn--tiq49xqyj",
+    "extend": "xn--tiq49xqyj",
+}  # whois.nic.xn--tiq49xqyj ['xn--tiq49xqyj']
+ZZ["游戏"] = {"_server": "whois.nic.xn--unup4y", "extend": "xn--unup4y"}  # whois.nic.xn--unup4y ['xn--unup4y']
+ZZ["vermögensberater"] = {
+    "_server": "whois.nic.xn--vermgensberater-ctb",
+    "extend": "xn--vermgensberater-ctb",
+}  # whois.nic.xn--vermgensberater-ctb ['xn--vermgensberater-ctb']
+ZZ["vermögensberatung"] = {
+    "_server": "whois.nic.xn--vermgensberatung-pwb",
+    "extend": "xn--vermgensberatung-pwb",
+}  # whois.nic.xn--vermgensberatung-pwb ['xn--vermgensberatung-pwb']
+ZZ["企业"] = {"_server": "whois.nic.xn--vhquv", "extend": "xn--vhquv"}  # whois.nic.xn--vhquv ['xn--vhquv']
+ZZ["信息"] = {"_server": "whois.teleinfo.cn", "extend": "_teleinfo"}
+ZZ["嘉里大酒店"] = {
+    "_server": "whois.nic.xn--w4r85el8fhu5dnra",
+    "extend": "xn--w4r85el8fhu5dnra",
+}  # whois.nic.xn--w4r85el8fhu5dnra ['xn--w4r85el8fhu5dnra']
+ZZ["嘉里"] = {"_server": "whois.nic.xn--w4rs40l", "extend": "xn--w4rs40l"}  # whois.nic.xn--w4rs40l ['xn--w4rs40l']
+ZZ["قطر"] = {"_server": "whois.registry.qa", "extend": "qa"}  # whois.registry.qa ['qa', 'xn--wgbl6a']
+ZZ["广东"] = {"_server": "whois.ngtld.cn", "extend": "com"}
+ZZ["இநதய"] = {"_server": "whois.registry.in", "extend": "com"}
+ZZ["新加坡"] = {"_server": "whois.sgnic.sg", "extend": "sg"}
+ZZ["テスト"] = {"_privateRegistry": True}
```

### Comparing `whoisdomain-1.20230503.1/README.md` & `whoisdomain-1.20230525.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,18 +24,28 @@
  * raise a exception on PrivateRegistry tld's where we know the tld and know we don't know anything
  * allow for optional cleaning the response before extracting information
  * optionally allow IDN's to be translated to Punycode
  * optional specify the whois command on query(...,cmd="whois") as in: https://github.com/gen1us2k/python-whois/
  * the module is now 'mypy --strict' clean
  * the module now also exports a cli command domainwhois
  * both the module and the cli now support showing the version with lib:whois.getVersion() or cli:whoisdomain -V
+ * the whoisdomain can now output json data (one per domain: e.g 'whoisdomain -d google.com -j' )
 
 ## Dependencies
   * please install also the command line "whois" of your distribution as this library parses the output of the "whois" cli command of your operating system
 
+## Docker
+ * docker pull mbootgithub/whoisdomain:latest
+ * docker run mbootgithub/whoisdomain -V # show version
+ * docker run mbootgithub/whoisdomain -d google.com # run one domain
+ * docker run mbootgithub/whoisdomain -a # run all tld
+ * docker run mbootgithub/whoisdomain -d google.com -j | jq -r . # run one domains , output in json and reformat with jq
+ * docker run mbootgithub/whoisdomain -d google.com -j | jq -r '.expiration_date' # output only expire date
+ * docker run mbootgithub/whoisdomain -d google.com -j | jq -r '[ .expiration_date, .creation_date ]
+
 ## Usage example
 
 Install the cli `whois` of your operating system if it is not present already,
 e.g 'apt install whois' or 'yum install whois'
 
 ```
 # fedora 37
@@ -60,28 +70,27 @@
 ```
 # fedora 37
 sudo yum install whois
 pip3 install whoisdomain
 whoisdomain -d google.com
 
 test domain: <<<<<<<<<< google.com >>>>>>>>>>>>>>>>>>>>
-name               str               'google.com'
-tld                str               'com'
-registrar          str               'MarkMonitor, Inc.'
-registrant_country str               'US'
-creation_date      datetime.datetime 1997-09-15 09:00:00
-expiration_date    datetime.datetime 2028-09-13 09:00:00
-last_updated       datetime.datetime 2019-09-09 17:39:04
-status             str               'clientUpdateProhibited (https://www.icann.org/epp#clientUpdateProhibited)'
-statuses           list              ['clientDeleteProhibited (https://www.icann.org/epp#clientDeleteProhibited)', 'clientTransferProhibited (https://www.icann.org/epp#clientTransferProhibited)', 'clientUpdateProhibited (https://www.icann.org/epp#clientUpdateProhibited)', 'serverDeleteProhibited (https://www.icann.org/epp#serverDeleteProhibited)', 'serverTransferProhibited (https://www.icann.org/epp#serverTransferProhibited)', 'serverUpdateProhibited (https://www.icann.org/epp#serverUpdateProhibited)']
-dnssec             bool              False
-name_servers       list              ['ns1.google.com', 'ns2.google.com', 'ns3.google.com', 'ns4.google.com']
-registrant         str               'Google LLC'
-emails             list              ['abusecomplaints@markmonitor.com', 'whoisrequest@markmonitor.com']
-
+name               'google.com'
+tld                'com'
+registrar          'MarkMonitor, Inc.'
+registrant_country 'US'
+creation_date      1997-09-15 09:00:00
+expiration_date    2028-09-13 09:00:00
+last_updated       2019-09-09 17:39:04
+status             'clientUpdateProhibited (https://www.icann.org/epp#clientUpdateProhibited)'
+statuses           ['clientDeleteProhibited (https://www.icann.org/epp#clientDeleteProhibited)', 'clientTransferProhibited (https://www.icann.org/epp#clientTransferProhibited)', 'clientUpdateProhibited (https://www.icann.org/epp#clientUpdateProhibited)', 'serverDeleteProhibited (https://www.icann.org/epp#serverDeleteProhibited)', 'serverTransferProhibited (https://www.icann.org/epp#serverTransferProhibited)', 'serverUpdateProhibited (https://www.icann.org/epp#serverUpdateProhibited)']
+dnssec             False
+name_servers       ['ns1.google.com', 'ns2.google.com', 'ns3.google.com', 'ns4.google.com']
+registrant         'Google LLC'
+emails             ['abusecomplaints@markmonitor.com', 'whoisrequest@markmonitor.com']
  ```
 
 A short intro into the cli whoisdomain command
 ```
 whoisdomain
     [ -h | --usage ]
         print this text and exit
@@ -114,14 +123,17 @@
         only analyze the given domains
         the option can be repeated to specify more domain's
 
     [ -v | --verbose ]
         set verbose to True,
         verbose output will be printed on stderr only
 
+    [ -j | --json ]
+        print each result as json
+
     [ -I | --IgnoreReturncode ]
         sets the IgnoreReturncode to True,
 
     [ -p | --print ]
         also print text containing the raw output of the cli whois
 
     [ -R | --Ruleset ]
@@ -139,16 +151,42 @@
     example: whoisdomain -v -I -a
 
     # test one specific file with verbose and IgnoreReturncode
     example: whoisdomain -v -I -f tests/ok-domains.txt
 
     # test one specific directory with verbose and IgnoreReturncode
     example: whoisdomain -v -I -D tests
+
 ```
 
+# Json output
+```
+{
+  "name": "hello.xyz",
+  "tld": "xyz",
+  "registrar": "Namecheap",
+  "registrant_country": "IS",
+  "creation_date": "2014-03-20 15:01:22",
+  "expiration_date": "2024-03-20 23:59:59",
+  "last_updated": "2023-03-14 09:24:32",
+  "status": "clientTransferProhibited https://icann.org/epp#clientTransferProhibited",
+  "statuses": [
+    "clientTransferProhibited https://icann.org/epp#clientTransferProhibited"
+  ],
+  "dnssec": false,
+  "name_servers": [
+    "dns1.registrar-servers.com",
+    "dns2.registrar-servers.com"
+  ],
+  "registrant": "Privacy service provided by Withheld for Privacy ehf",
+  "emails": [
+    "abuse@namecheap.com"
+  ]
+}
+```
 ## ccTLD & TLD support
 see the file: ./whoisdomain/tld_regexpr.py
 or call lib:whoisdomain.validTlds() or cli:whoisdomain -S
 
 ## Support
  * Python 3.x is supported for x >= 6
  * Python 2.x IS NOT supported.
```

### Comparing `whoisdomain-1.20230503.1/pyproject.toml` & `whoisdomain-1.20230525.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Makefile",
     ".gitignore",
     "/.gitignore",
 ]
 
 [project]
 name = "whoisdomain"
-version = "1.20230503.1"
+version = "1.20230525.5"
 
 authors = [
   { name="DannyCork"},
 ]
 
 maintainers = [
   { name="Maarten Boot", email="130295084+mboot-github@users.noreply.github.com" },
```

### Comparing `whoisdomain-1.20230503.1/PKG-INFO` & `whoisdomain-1.20230525.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whoisdomain
-Version: 1.20230503.1
+Version: 1.20230525.5
 Summary: Python package for retrieving WHOIS information of domains.
 Project-URL: Bug Tracker, https://github.com/mboot-github/WhoisDomain/issues
 Project-URL: Home Page, https://github.com/mboot-github/WhoisDomain/
 Project-URL: Repository, https://github.com/mboot-github/WhoisDomain/
 Author: DannyCork
 Maintainer-email: Maarten Boot <130295084+mboot-github@users.noreply.github.com>
 License-Expression: MIT
@@ -50,18 +50,28 @@
  * raise a exception on PrivateRegistry tld's where we know the tld and know we don't know anything
  * allow for optional cleaning the response before extracting information
  * optionally allow IDN's to be translated to Punycode
  * optional specify the whois command on query(...,cmd="whois") as in: https://github.com/gen1us2k/python-whois/
  * the module is now 'mypy --strict' clean
  * the module now also exports a cli command domainwhois
  * both the module and the cli now support showing the version with lib:whois.getVersion() or cli:whoisdomain -V
+ * the whoisdomain can now output json data (one per domain: e.g 'whoisdomain -d google.com -j' )
 
 ## Dependencies
   * please install also the command line "whois" of your distribution as this library parses the output of the "whois" cli command of your operating system
 
+## Docker
+ * docker pull mbootgithub/whoisdomain:latest
+ * docker run mbootgithub/whoisdomain -V # show version
+ * docker run mbootgithub/whoisdomain -d google.com # run one domain
+ * docker run mbootgithub/whoisdomain -a # run all tld
+ * docker run mbootgithub/whoisdomain -d google.com -j | jq -r . # run one domains , output in json and reformat with jq
+ * docker run mbootgithub/whoisdomain -d google.com -j | jq -r '.expiration_date' # output only expire date
+ * docker run mbootgithub/whoisdomain -d google.com -j | jq -r '[ .expiration_date, .creation_date ]
+
 ## Usage example
 
 Install the cli `whois` of your operating system if it is not present already,
 e.g 'apt install whois' or 'yum install whois'
 
 ```
 # fedora 37
@@ -86,28 +96,27 @@
 ```
 # fedora 37
 sudo yum install whois
 pip3 install whoisdomain
 whoisdomain -d google.com
 
 test domain: <<<<<<<<<< google.com >>>>>>>>>>>>>>>>>>>>
-name               str               'google.com'
-tld                str               'com'
-registrar          str               'MarkMonitor, Inc.'
-registrant_country str               'US'
-creation_date      datetime.datetime 1997-09-15 09:00:00
-expiration_date    datetime.datetime 2028-09-13 09:00:00
-last_updated       datetime.datetime 2019-09-09 17:39:04
-status             str               'clientUpdateProhibited (https://www.icann.org/epp#clientUpdateProhibited)'
-statuses           list              ['clientDeleteProhibited (https://www.icann.org/epp#clientDeleteProhibited)', 'clientTransferProhibited (https://www.icann.org/epp#clientTransferProhibited)', 'clientUpdateProhibited (https://www.icann.org/epp#clientUpdateProhibited)', 'serverDeleteProhibited (https://www.icann.org/epp#serverDeleteProhibited)', 'serverTransferProhibited (https://www.icann.org/epp#serverTransferProhibited)', 'serverUpdateProhibited (https://www.icann.org/epp#serverUpdateProhibited)']
-dnssec             bool              False
-name_servers       list              ['ns1.google.com', 'ns2.google.com', 'ns3.google.com', 'ns4.google.com']
-registrant         str               'Google LLC'
-emails             list              ['abusecomplaints@markmonitor.com', 'whoisrequest@markmonitor.com']
-
+name               'google.com'
+tld                'com'
+registrar          'MarkMonitor, Inc.'
+registrant_country 'US'
+creation_date      1997-09-15 09:00:00
+expiration_date    2028-09-13 09:00:00
+last_updated       2019-09-09 17:39:04
+status             'clientUpdateProhibited (https://www.icann.org/epp#clientUpdateProhibited)'
+statuses           ['clientDeleteProhibited (https://www.icann.org/epp#clientDeleteProhibited)', 'clientTransferProhibited (https://www.icann.org/epp#clientTransferProhibited)', 'clientUpdateProhibited (https://www.icann.org/epp#clientUpdateProhibited)', 'serverDeleteProhibited (https://www.icann.org/epp#serverDeleteProhibited)', 'serverTransferProhibited (https://www.icann.org/epp#serverTransferProhibited)', 'serverUpdateProhibited (https://www.icann.org/epp#serverUpdateProhibited)']
+dnssec             False
+name_servers       ['ns1.google.com', 'ns2.google.com', 'ns3.google.com', 'ns4.google.com']
+registrant         'Google LLC'
+emails             ['abusecomplaints@markmonitor.com', 'whoisrequest@markmonitor.com']
  ```
 
 A short intro into the cli whoisdomain command
 ```
 whoisdomain
     [ -h | --usage ]
         print this text and exit
@@ -140,14 +149,17 @@
         only analyze the given domains
         the option can be repeated to specify more domain's
 
     [ -v | --verbose ]
         set verbose to True,
         verbose output will be printed on stderr only
 
+    [ -j | --json ]
+        print each result as json
+
     [ -I | --IgnoreReturncode ]
         sets the IgnoreReturncode to True,
 
     [ -p | --print ]
         also print text containing the raw output of the cli whois
 
     [ -R | --Ruleset ]
@@ -165,16 +177,42 @@
     example: whoisdomain -v -I -a
 
     # test one specific file with verbose and IgnoreReturncode
     example: whoisdomain -v -I -f tests/ok-domains.txt
 
     # test one specific directory with verbose and IgnoreReturncode
     example: whoisdomain -v -I -D tests
+
 ```
 
+# Json output
+```
+{
+  "name": "hello.xyz",
+  "tld": "xyz",
+  "registrar": "Namecheap",
+  "registrant_country": "IS",
+  "creation_date": "2014-03-20 15:01:22",
+  "expiration_date": "2024-03-20 23:59:59",
+  "last_updated": "2023-03-14 09:24:32",
+  "status": "clientTransferProhibited https://icann.org/epp#clientTransferProhibited",
+  "statuses": [
+    "clientTransferProhibited https://icann.org/epp#clientTransferProhibited"
+  ],
+  "dnssec": false,
+  "name_servers": [
+    "dns1.registrar-servers.com",
+    "dns2.registrar-servers.com"
+  ],
+  "registrant": "Privacy service provided by Withheld for Privacy ehf",
+  "emails": [
+    "abuse@namecheap.com"
+  ]
+}
+```
 ## ccTLD & TLD support
 see the file: ./whoisdomain/tld_regexpr.py
 or call lib:whoisdomain.validTlds() or cli:whoisdomain -S
 
 ## Support
  * Python 3.x is supported for x >= 6
  * Python 2.x IS NOT supported.
```

