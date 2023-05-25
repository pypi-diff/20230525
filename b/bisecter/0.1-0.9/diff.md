# Comparing `tmp/bisecter-0.1.tar.gz` & `tmp/bisecter-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bisecter-0.1.tar", last modified: Mon Jan 30 18:33:44 2023, max compression
+gzip compressed data, was "bisecter-0.9.tar", last modified: Thu May 25 08:18:24 2023, max compression
```

## Comparing `bisecter-0.1.tar` & `bisecter-0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 medic     (1000) medic     (1000)        0 2023-01-30 18:33:44.049530 bisecter-0.1/
--rw-rw-r--   0 medic     (1000) medic     (1000)    35149 2020-06-26 11:39:18.000000 bisecter-0.1/LICENSE
--rw-r--r--   0 medic     (1000) medic     (1000)     1738 2023-01-30 18:33:44.049530 bisecter-0.1/PKG-INFO
--rw-r--r--   0 medic     (1000) medic     (1000)     1045 2023-01-30 18:29:37.000000 bisecter-0.1/README
-drwxr-xr-x   0 medic     (1000) medic     (1000)        0 2023-01-30 18:33:44.048530 bisecter-0.1/bisecter/
--rw-r--r--   0 medic     (1000) medic     (1000)    19418 2023-01-30 18:29:37.000000 bisecter-0.1/bisecter/__init__.py
-drwxr-xr-x   0 medic     (1000) medic     (1000)        0 2023-01-30 18:33:44.049530 bisecter-0.1/bisecter.egg-info/
--rw-r--r--   0 medic     (1000) medic     (1000)     1738 2023-01-30 18:33:44.000000 bisecter-0.1/bisecter.egg-info/PKG-INFO
--rw-r--r--   0 medic     (1000) medic     (1000)      220 2023-01-30 18:33:44.000000 bisecter-0.1/bisecter.egg-info/SOURCES.txt
--rw-r--r--   0 medic     (1000) medic     (1000)        1 2023-01-30 18:33:44.000000 bisecter-0.1/bisecter.egg-info/dependency_links.txt
--rw-r--r--   0 medic     (1000) medic     (1000)        7 2023-01-30 18:33:44.000000 bisecter-0.1/bisecter.egg-info/requires.txt
--rw-r--r--   0 medic     (1000) medic     (1000)        9 2023-01-30 18:33:44.000000 bisecter-0.1/bisecter.egg-info/top_level.txt
-drwxr-xr-x   0 medic     (1000) medic     (1000)        0 2023-01-30 18:33:44.049530 bisecter-0.1/scripts/
--rwxr-xr-x   0 medic     (1000) medic     (1000)      682 2023-01-30 18:04:12.000000 bisecter-0.1/scripts/bisecter
--rw-r--r--   0 medic     (1000) medic     (1000)       38 2023-01-30 18:33:44.049530 bisecter-0.1/setup.cfg
--rwxr-xr-x   0 medic     (1000) medic     (1000)     2890 2023-01-30 18:29:48.000000 bisecter-0.1/setup.py
+drwxr-xr-x   0 medic     (1000) medic     (1000)        0 2023-05-25 08:18:24.256896 bisecter-0.9/
+-rw-rw-r--   0 medic     (1000) medic     (1000)    35149 2020-06-26 11:39:18.000000 bisecter-0.9/LICENSE
+-rw-r--r--   0 medic     (1000) medic     (1000)     1738 2023-05-25 08:18:24.255896 bisecter-0.9/PKG-INFO
+-rw-r--r--   0 medic     (1000) medic     (1000)     1045 2023-01-30 18:29:37.000000 bisecter-0.9/README
+drwxr-xr-x   0 medic     (1000) medic     (1000)        0 2023-05-25 08:18:24.255896 bisecter-0.9/bisecter/
+-rw-r--r--   0 medic     (1000) medic     (1000)    26873 2023-05-25 08:14:19.000000 bisecter-0.9/bisecter/__init__.py
+-rw-r--r--   0 medic     (1000) medic     (1000)      166 2023-02-01 10:41:47.000000 bisecter-0.9/bisecter/__main__.py
+-rw-r--r--   0 medic     (1000) medic     (1000)     7423 2023-05-05 06:06:41.000000 bisecter-0.9/bisecter/utils.py
+drwxr-xr-x   0 medic     (1000) medic     (1000)        0 2023-05-25 08:18:24.255896 bisecter-0.9/bisecter.egg-info/
+-rw-r--r--   0 medic     (1000) medic     (1000)     1738 2023-05-25 08:18:24.000000 bisecter-0.9/bisecter.egg-info/PKG-INFO
+-rw-r--r--   0 medic     (1000) medic     (1000)      228 2023-05-25 08:18:24.000000 bisecter-0.9/bisecter.egg-info/SOURCES.txt
+-rw-r--r--   0 medic     (1000) medic     (1000)        1 2023-05-25 08:18:24.000000 bisecter-0.9/bisecter.egg-info/dependency_links.txt
+-rw-r--r--   0 medic     (1000) medic     (1000)        9 2023-05-25 08:18:24.000000 bisecter-0.9/bisecter.egg-info/top_level.txt
+drwxr-xr-x   0 medic     (1000) medic     (1000)        0 2023-05-25 08:18:24.255896 bisecter-0.9/scripts/
+-rwxr-xr-x   0 medic     (1000) medic     (1000)      682 2023-01-30 18:04:12.000000 bisecter-0.9/scripts/bisecter
+-rw-r--r--   0 medic     (1000) medic     (1000)       38 2023-05-25 08:18:24.256896 bisecter-0.9/setup.cfg
+-rwxr-xr-x   0 medic     (1000) medic     (1000)     2882 2023-01-31 13:34:54.000000 bisecter-0.9/setup.py
```

### Comparing `bisecter-0.1/LICENSE` & `bisecter-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bisecter-0.1/PKG-INFO` & `bisecter-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisecter
-Version: 0.1
+Version: 0.9
 Summary: Allows to bisect over arbitrary number of arguments.
 Home-page: https://github.com/ldoktor/bisecter
 Author: Lukas Doktor
 Author-email: ldoktor@redhat.com
 License: GPLv2+
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `bisecter-0.1/README` & `bisecter-0.9/README`

 * *Files identical despite different names*

### Comparing `bisecter-0.1/bisecter/__init__.py` & `bisecter-0.9/bisecter/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,44 +8,29 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 #
 # See LICENSE for more details.
 #
 # Copyright: Red Hat Inc. 2023
 # Author: Lukas Doktor <ldoktor@redhat.com>
-"""
-Example usage:
-
-bisecter start '["some", "values"]' '["another", "values"]'
-my_script "$(bisecter args)" $(bisecter id)
-bisecter good
-my_script "$(bisecter args)" $(bisecter id)
-bisecter bad
-...
-bisecter log
-bisecter reset
-
-bisecter start '["some", "values"]' '["another", "values"]'
-bisecter run my_script
-bisecter log
-bisecter reset
-"""
+"""Tool to drive bisection over multiple set of arguments"""
 
 import argparse
-import ast
 import dataclasses
 import enum
 import math
 import os
 import pickle
 import pipes
 import re
 import subprocess
 import sys
 
+from bisecter import utils
+
 
 class BisectionStatus(enum.Enum):
     """Bisection status"""
     GOOD = 0
     BAD = 1
     SKIP = 125
 
@@ -60,122 +45,132 @@
         return (f"{self.status.name:4s} "
                 f"{'-'.join(str(_) for _ in self.identifier)}")
 
     def __repr__(self):
         return (f"{self.status.name:4s} "
                 f"{'-'.join(str(_) for _ in self.identifier)}")
 
+    def __eq__(self, other):
+        if isinstance(other, BisectionLogEntry):
+            return self.identifier == other.identifier
+        if isinstance(other, str):
+            return '-'.join(str(_) for _ in self.identifier) == other
+        return self.identifier == other
+
 
 class Bisection:
     """
     Object to keep track of a single bisection
     """
     current = None
     _good = None
     _bad = None
-    _last_good = 0
 
     def __init__(self, values):
-        self._values = values
+        self.values = values
+        self.current = self._first_bad = self.last_index = len(values) - 1
+        self._good = 0
+        self._bad = self.last_index
         self._skips = []
-        self.current = 0
+        # TODO: Investigate improvements for skip columns cases
+        # self.no_good = True
 
     def value(self, index=None):
         """Value associated to the ``index`` value (by default current one)"""
         if index is not None:
-            return self._values[index]
-        return self._values[self.current]
+            return self.values[index]
+        return self.values[self.current]
 
-    def _update_current(self):
+    def update_current(self):
+        """Update current according to good and bad"""
         self.current = (self._good + self._bad) // 2
 
     def good(self):
         """Mark the current step as good (go to right)"""
-        self._last_good = self.current
         new = self.current + 1
         # We iterate over multiple arrays and can not be sure the last
         # one of each is bad
         if (self._bad <= new and
-                not new == len(self._values) - 1):
-            self.reset(self._last_good, self._last_good)
+                new != self.last_index):
+            self.reset(self._first_bad, self._first_bad)
             return None
         self._good = new
-        self._update_current()
+        self.update_current()
         return self.current
 
     def bad(self):
         """Mark the current step as bad (go to left)"""
+        self._first_bad = self.current
         if self.current <= self._good:
-            self.reset(self._last_good, self._last_good)
+            self.reset(self._first_bad, self._first_bad)
             return None
         self._bad = self.current
-        self._update_current()
+        self.update_current()
         if self.current <= 0:
-            self.reset(self._last_good, self._last_good)
+            self.reset(self._first_bad, self._first_bad)
             return None
         return self.current
 
     def skip(self):
         """Mark the current step as skip (untestable)"""
         self._skips.append(self.current)
-        offset = -1
-        new = (self._good + self._bad) // 2 + offset
-        # We iterate over multiple arrays and can not be sure the last
-        # one of each is bad
-        if new < self._good or (new >= self._bad and
-                                 new != (len(self._values) - 1)):
-            self.reset(self._last_good, self._last_good)
-            return None
+        new = (self._good + self._bad) // 2
+        max_offset = new * 2
+        offset = 0
         while new in self._skips:
             if offset < 0:
                 offset = 1 - offset
             else:
-                offset = - 1 - offset
-            new += offset
-            # We iterate over multiple arrays and can not be sure the last
-            # one of each is bad
-            if new <= self._good or (new >= self._bad and
-                                     new != (len(self._values) - 1)):
-                self.reset(self._last_good, self._last_good)
+                offset = -1 - offset
+            if abs(offset) > max_offset:
+                self.reset(self._first_bad, self._first_bad)
                 return None
+            new += offset
+            if new <= self._good or new >= self._bad:
+                # We don't want to test good and bad, but we still want to
+                # test the remaining items up to the max offset
+                self._skips.append(new)
         self.current = new
         return self.current
 
     def steps_left(self):
         """Report the approximate number of remaining steps"""
         variants = self.variants_left()
         if variants > 1:
             return math.ceil((math.log2(variants + 1)))
         return 0
 
     def variants_left(self):
         """Report the number of variants"""
         if self._bad is None:
-            return len(self._values)
+            return len(self.values)
         return self._bad - self._good - len(self._skips)
 
     def reset(self, good=None, bad=None):
         """Reset the bisection, optionally select good/bad positions"""
         self._good = 0 if good is None else good
-        self._bad = (len(self._values) - 1) if bad is None else bad
+        self._bad = self.last_index if bad is None else bad
         self._skips = []
-        self._update_current()
+        self.update_current()
 
 
 class Bisections:
     """
     Keeps track of a bisection over multiple arrays
     """
 
     def __init__(self, args):
         self.args = [Bisection(arg) for arg in args]
-        if args:
-            self.args[0].reset()
-        self._log = []
-        self._active = 0
+        # Initialize log with first and last checks (trust the user)
+        self._log = [BisectionLogEntry(BisectionStatus.GOOD,
+                                       [0 for _ in args]),
+                     BisectionLogEntry(BisectionStatus.BAD,
+                                       [len(_) - 1 for _ in args])]
+        self._active = -1
+        self._postprocess_current(None)
 
     def current(self):
         """Reports the current variant indexes"""
         return [arg.current for arg in self.args]
 
     def value(self, variant=None):
         """Reports parameters of the current variant"""
@@ -185,59 +180,112 @@
                 for i, index in enumerate(variant)]
 
     def good(self):
         """Mark the current step as good (go to right)"""
         current = self.current()
         self._log.append(BisectionLogEntry(BisectionStatus.GOOD, current))
         if self._active >= len(self.args):
-            return None
-        this = self.args[self._active].good()
-        if this is None or this == 0:
-            self._active += 1
-            if self._active >= len(self.args):
-                return None
+            return self._postprocess_current(None)
+        #self.args[self._active].no_good = False
+        if self.args[self._active].current == 0:
+            # It won't reproduce with the first argument, which means we have
+            # to investigate this item. Reset it and start bisection
             self.args[self._active].reset()
-        return self.current()
+            return self._postprocess_current(0)
+        this = self.args[self._active].good()
+        return self._postprocess_current(this)
 
     def bad(self):
         """Mark the current step as bad (go to left)"""
         self._log.append(BisectionLogEntry(BisectionStatus.BAD,
                                            self.current()))
         if self._active >= len(self.args):
-            return None
-        #_this = self.args[self._active].current
+            return self._postprocess_current(None)
+        if self.args[self._active].current == 0:
+            # Still failing with the first argument, this axis is irrelevant,
+            # skip it
+            self.args[self._active].reset(0, 0)
+            return self._postprocess_current(None)
         this = self.args[self._active].bad()
-        if this is None:  # or this == 0:
-            self._active += 1
-            if self._active >= len(self.args):
-                return None
-            self.args[self._active].reset()
-        return self.current()
+        return self._postprocess_current(this)
 
     def skip(self):
         """Mark the current step as skip (untestable)"""
         self._log.append(BisectionLogEntry(BisectionStatus.SKIP,
                                            self.current()))
         if self._active >= len(self.args):
-            return None
+            return self._postprocess_current(None)
         this = self.args[self._active].skip()
+        return self._postprocess_current(this)
+
+    def _postprocess_current(self, this):
+        """
+        Perform common checks on the next variant
+
+        Based on the values it can skip to the next axis, report the previously
+        logged status or simply return the next "current" variant
+
+        :param this: Value of the next index of the current active axis (7)
+        :return: next "current" variant (0-0-7)
+        """
         if this is None:  # or this == 0:
             self._active += 1
             if self._active >= len(self.args):
+                # TODO: Investigate improvements for skip columns cases
+                """
+                # In case of many skips certain columns might have not been
+                # tested yet
+                for i, arg in enumerate(self.args):
+                    '''
+                    if arg._good == arg.last_index:
+                        variant = [_.current if i == j else 0
+                                   for j, _ in enumerate(self.args)]
+                        if variant not in self._log:
+                            arg.reset()
+                            arg.current = 0
+                            return self.current()
+                    '''
+                    if getattr(arg, 'no_good', False) is True:
+                        # I need to go up on these
+                        #import pydevd; pydevd.settrace("127.0.0.1", True, True)
+                        #for _ in self.args:
+                        #    if _.no_good is True:
+                        #        _.reset()
+                        #        _.curret = _.last_index
+                        arg.current = 0
+                        # Set this one to False to skip it next time
+                        arg.no_good = False
+                        self._active = i
+                        return self.current()
+                """
                 return None
-            self.args[self._active].reset()
-        return self.current()
+            # Initialize the next axis to 0 to try if it is important
+            self.args[self._active].current = 0
+            return self._postprocess_current(0)
+        current = self.current()
+        if current in self._log:
+            status = [_.status for _ in self._log if _ == current][0]
+            action = {BisectionStatus.GOOD: "good",
+                      BisectionStatus.BAD: "bad",
+                      BisectionStatus.SKIP: "skip"}[status]
+            return self._postprocess_current(getattr(self.args[self._active],
+                                              action)())
+        return current
 
     def steps_left(self):
         """Report how many steps to test"""
-        return sum(_.steps_left() for _ in self.args)
+        return (sum(_.steps_left() for _ in self.args) +
+                len(self.args) - self._active)
 
     def variants_left(self):
         """Report how many variants to test"""
-        return sum(_.variants_left() for _ in self.args)
+        variants = [_.variants_left() or 1 for _ in self.args[self._active:]]
+        if not variants:
+            return 0
+        return math.prod(variants)
 
     def log(self):
         """Report bisection log"""
         return('\n'.join(str(entry) for entry in self._log))
 
 
 class Bisecter:
@@ -258,64 +306,80 @@
                 'skip': self.status,
                 'run': self.run,
                 'args': self.arguments,
                 'id': self.identifier,
                 'log': self.log,
                 'reset': self.reset}.get(self.args.cmd)
         if func is None:
-            sys.stderr.write("Unknown command {self.args.cmd}\n")
+            sys.stderr.write(f"Unknown command {self.args.cmd}\n")
             sys.exit(-1)
         return func()
 
     def parse_args(self, command_line=None):
         """
         Define arguments
         """
+
         def variant_id(arg):
             """Parse variant ID"""
+            if arg in ('good', 'bad'):
+                return arg
             return [int(_) for _ in arg.split('-')]
+
         parser = argparse.ArgumentParser(prog='Bisecter', description='Allows '
                                          'to bisect over arbitrary number of '
                                          'arguments.')
         parser.add_argument('--state-file', help='Override path to the '
                             'bisection metadata file (%(default)s)',
                             default='./.bisecter_state',
                             type=os.path.abspath)
         subparsers = parser.add_subparsers(dest='cmd')
         start = subparsers.add_parser('start', help='Initialize bisection')
-        start.add_argument('--from-file', help='Read arguments from YAML file')
+        start.add_argument('--from-yaml', help='Read arguments from YAML file')
         start.add_argument('--extended-arguments', '-E', help='On top of the '
                            'comma separated arguments allow certain evals, '
                            'eg. foo,range(10,31,10),bar becomes ["foo", "10", '
                            '"20", "30", "bar"]', action='store_true')
+        start.add_argument('--dry-run', help='Do not actually start bisection,'
+                           'only parse the arguments and report the axis',
+                           action='store_true')
         start.add_argument('arguments', help='Specify one or multiple comma '
                            'separated lists of values this bisection will '
                            'iterate over; bisecter assumes '
                            'the first item of each argument as good and the '
-                           'last item as bad.', nargs='+')
+                           'last item as bad.', nargs='*')
         for status in ("good", "bad", "skip"):
             _ = subparsers.add_parser(status, help='Tag the current '
                                       f'result as {status}; get the '
                                       'next arguments by running '
                                       '"bisecter args"')
         run = subparsers.add_parser('run', help='Run your script, appending '
                                     'combinations of the arguments '
                                     'specified in "bisecter start". Exit '
                                     'code 0 means good; 1 - 124 and 126 - 127 '
                                     'means bad; 125 means skip; 128 - 255 '
                                     'means interrupt the bisection.')
+        run.add_argument("--template", "-t", action="store_true", help="Allows"
+                         " to use a simple templating in the to-be-executed "
+                         "command which replaces {\\d} entries for bisection "
+                         "values using the \\d number as index (allowing "
+                         "negative values). Use double brackets to skip "
+                         "the replacement.")
         run.add_argument('command', help='Command to be executed',
                          nargs=argparse.REMAINDER)
         args = subparsers.add_parser('args', help='Report the variant '
                                      'arguments. To consume them you can use '
                                      '\'your_script "$(bisecter args)"\' (use '
                                      'the " quotation to preserve special '
                                      'characters).')
-        args.add_argument('id', help='Id of the variant which arguments you '
-                          'are interested in (current)', nargs='?',
+        args.add_argument('axis', help='Optionally select only one axis'
+                          'index to report arguments of', type=int,
+                          nargs='?')
+        args.add_argument('--id', '-i', help='Id of the variant which '
+                          'arguments you are interested in (current)',
                           type=variant_id)
         args.add_argument('--raw', '-r', help="Report raw arguments in "
                           "python format", action='store_true')
         _ = subparsers.add_parser('id', help='Report the current variant'
                                   ' identifier that can serve to link '
                                   'log entries to arguments')
         _ = subparsers.add_parser('log', help='Report the bisection log')
@@ -326,18 +390,14 @@
     def _save_state(self):
         """
         Records the self.bisection in a state file
         """
         try:
             with open(self.args.state_file, 'bw') as fd_state:
                 pickle.dump(self.bisection, fd_state)
-        except pickle.UnpicklingError as details:
-            sys.stderr.write("Failed to write bisecter state to "
-                             f"{self.args.state_file}: {details}\n")
-            sys.exit(-1)
         except IOError as details:
             sys.stderr.write("Failed to open bisecter state file "
                              f"{self.args.state_file}: {details}\n")
             sys.exit(-1)
 
     def _load_state(self):
         """
@@ -353,148 +413,233 @@
         except IOError as details:
             sys.stderr.write("Failed to open bisecter state file "
                              f"{self.args.state_file}, please run "
                              f"'{sys.argv[0]} start' first ({details})\n")
             sys.exit(-1)
 
     def _parse_extended_args(self, arguments):
+
         def range_repl(matchobj):
             args = []
-            if '.' in matchobj.group(2):
-                args.append(float(matchobj.group(2)))
-            else:
-                args.append(int(matchobj.group(2)))
+            args.append(int(matchobj.group(2)))
             for arg in matchobj.groups()[2:]:
                 if arg is None:
                     continue
-                if '.' in arg:
-                    args.append(float(arg[1:]))
-                else:
-                    args.append(int(arg[1:]))
+                args.append(int(arg[1:]))
             return ','.join(str(_) for _ in range(*args))
 
-        re_range = re.compile(r'(range\(([^\),]+)(,[^\),]+)?(,[^\),]+)?\))')
+        re_range = re.compile(r'(range\((\d+)(,\s*\d+\s*)?(,\s*\d+\s*)?\))')
         args = []
         for arg in arguments:
-            line = re_range.sub(range_repl, arg)
-            args.append(self._split_by_comma(line))
+            if arg.startswith("beaker://"):
+                parsed_args = utils.range_beaker(arg)
+            elif arg.startswith("url://"):
+                parsed_args = utils.range_url(arg)
+            else:
+                line = re_range.sub(range_repl, arg)
+                parsed_args = self._split_by_comma(line)
+            if not parsed_args:
+                raise ValueError(f"Extended argument {arg} resulted in empty "
+                                 "list.")
+            args.append(parsed_args)
         return args
 
     @staticmethod
     def _split_by_comma(arg):
         return [val.replace('\\,', ',') for val in re.split(r'(?<!\\),', arg)]
 
     def start(self):
         """
         Initialize the work dirs and define arguments
         """
-        if self.args.from_file:
+        if self.args.from_yaml:
             if self.args.arguments:
                 sys.stderr.write('WARNING: Replacing arguments specified '
                                  'as positional arguments with the ones '
-                                 f'from "{self.args.from_file}" file\n')
+                                 f'from "{self.args.from_yaml}" file\n')
             try:
-                import yaml     # optional dependency pylint: disable=C0415
+                import yaml  # optional dependency pylint: disable=C0415
             except ImportError:
                 sys.stderr.write("PyYAML not installed, unable to load "
                                  "arguments from file\n")
                 sys.exit(-1)
             try:
-                with open(self.args.from_file, encoding='utf8') as inp:
+                with open(self.args.from_yaml, encoding='utf8') as inp:
                     arguments = yaml.load(inp, yaml.SafeLoader)
+                    try:
+                        arguments = [[str(arg) for arg in args]
+                                     for args in arguments]
+                    except Exception as details:
+                        sys.stderr.write('Failed to parse arguments from '
+                                         f'{self.args.from_yaml}, ensure '
+                                         'it contains list of lists '
+                                         'convertable to strings: '
+                                         f'{details}\n')
+                        sys.exit(-1)
             except yaml.YAMLError as details:
                 sys.stderr.write('Failed to load arguments from '
-                                 f'{self.args.from_file}: {details}\n')
+                                 f'{self.args.from_yaml}: {details}\n')
                 sys.exit(-1)
             except IOError as details:
                 sys.stderr.write('Failed to read arguments file '
-                                 f'{self.args.from_file}: {details}\n')
+                                 f'{self.args.from_yaml}: {details}\n')
                 sys.exit(-1)
         elif self.args.extended_arguments:
             arguments = self._parse_extended_args(self.args.arguments)
         else:
             arguments = []
             for arg in self.args.arguments:
                 arguments.append(self._split_by_comma(arg))
         self.bisection = Bisections(arguments)
         if os.path.exists(self.args.state_file):
             sys.stderr.write(f"Bisection in '{self.args.state_file}' already "
                              "in progress\n")
             sys.exit(-1)
+        self._report_remaining_steps()
+        self._report_detailed_stats()
+        if self.args.dry_run:
+            print("Bisection not started, running in --dry-run mode")
+            return
         self._save_state()
-        self._value()
+        print(self._current_value())
 
-    def _value(self, variant=None):
+    def _current_value(self, variant=None):
         """
         Report value of the current variant in a simple form
         """
-        print(' '.join(pipes.quote(_) for _ in self.bisection.value(variant)))
+        return ' '.join(pipes.quote(_) for _ in self.bisection.value(variant))
 
     def _report_remaining_steps(self):
         """
         Report remaining steps count
         """
-        sys.stderr.write(f"Bisecting: {self.bisection.variants_left()} variants "
+        sys.stderr.write(f"Bisecter: {self.bisection.variants_left()} variants"
                          " left to test after this (roughly "
                          f"{self.bisection.steps_left()} steps)\n")
 
+    def _report_detailed_stats(self):
+        """
+        Report details about axis
+        """
+        for i, axis in enumerate(self.bisection.args):
+            sys.stderr.write(f"{i} ({len(axis.values)}): "
+                             f"{','.join(str(_) for _ in axis.values)}\n")
+
     def status(self):
         """
         Set the result of the current bisection combination
         """
         self._load_state()
         ret = getattr(self.bisection, self.args.cmd)()
         self._save_state()
         if ret is None:
-            # TODO: Add clever messages about first/last arguments...
-            print("Bisection complete, last good combination is "
-                  f"{self._value()}")
-            return
+            self._print_complete_status()
         self._report_remaining_steps()
-        self._value()
+        print(self._current_value())
+
+    def _print_complete_status(self):
+        current = self.bisection.current()
+        prefix = f"Bisection complete in {len(self.bisection._log)} steps, "
+        if any(current):
+            axes = [str(i) for i, v in enumerate(current) if v != 0]
+            if len(axes) == len(self.bisection.args):
+                last = True
+                for arg in self.bisection.args:
+                    if arg.current != arg.last_index:
+                        last = False
+                        break
+                if last:
+                    print(f"{prefix}only the last combination "
+                          "is failing (is the last one really failing?):")
+                else:
+                    print(f"{prefix}failure is caused by a "
+                          "combination of all axes; first bad "
+                          "combination is:")
+            elif len(axes) > 1:
+                print(f"{prefix}failure is caused by a "
+                      f"combination of axes {','.join(axes)}; first "
+                      "bad combination is:")
+            else:
+                if current[-1] == 1:
+                    print(f"{prefix}all tested combinations are "
+                          "failing (is the first one really passing?)")
+                else:
+                    print(f"{prefix}failure is caused only by "
+                          f"axis {axes[0]}, first bad combination is:")
+        else:
+            print(f"{prefix}even the first (expected to be good) "
+                  "combination reports failure:")
+        print(self._current_value())
 
     def run(self):
         """
         Keep executing args.command using it's exit code to drive the bisection
         """
+        def get_cmd():
+            if self.args.template:
+                try:
+                    return utils.simple_template(self.args.command,
+                                                 self.bisection.value())
+                except utils.ReplaceIndexError as exc:
+                    sys.stderr.write(f"{exc}\n")
+                    sys.exit(-1)
+            return self.args.command + self.bisection.value()
+
         self._load_state()
-        with open(os.devnull, "r+", encoding="utf-8") as devnull:
-            bret = True
-            while bret is not None:
+        bret = True
+        while bret is not None:
+            self._report_remaining_steps()
+            args = get_cmd()
+            sys.stderr.write(f"Bisecter: Running: {args}\n")
+            ret = subprocess.run(args, check=False)
+            if ret.returncode == 0:
+                sys.stderr.write(f"Bisecter: GOOD {self._current_value()}\n")
+                bret = self.bisection.good()
+            elif ret.returncode == 125:
+                sys.stderr.write(f"Bisecter: SKIP {self._current_value()}\n")
+                bret = self.bisection.skip()
+            elif ret.returncode <= 127:
+                sys.stderr.write(f"Bisecter: BAD {self._current_value()}\n")
+                bret = self.bisection.bad()
+            else:
                 self._save_state()
-                self._report_remaining_steps()
-                args = self.args.command + self.bisection.value()
-                sys.stderr.write(f"Running {args}\n")
-                ret = subprocess.run(args, stdin=devnull, check=False)
-                if ret.returncode == 0:
-                    bret = self.bisection.good()
-                elif ret.returncode == 125:
-                    bret = self.bisection.skip()
-                elif ret.returncode <= 127:
-                    bret = self.bisection.bad()
-                else:
-                    sys.stderr.write(f"Command {' '.join(self.args.command)}"
-                                     f"returned {ret.returncode}, interrupting"
-                                     " the automated bisection.")
-                    sys.exit(-1)
-        self._value()
+                sys.stderr.write(f"Command {' '.join(self.args.command)}"
+                                 f"returned {ret.returncode}, interrupting"
+                                 " the automated bisection.\n")
+                sys.exit(-1)
+            self._save_state()
+        self._print_complete_status()
 
     def arguments(self):
         """
         Print arguments of the bisection variant
         """
         self._load_state()
         if self.args.id:
-            variant = self.args.id
+            if self.args.id == 'good':
+                variant = [0] * len(self.bisection.args)
+            elif self.args.id == 'bad':
+                variant = [-1] * len(self.bisection.args)
+            else:
+                variant = self.args.id
         else:
             variant = None
-        if self.args.raw:
-            print(self.bisection.value(variant))
-        else:
-            self._value(variant)
+        try:
+            if self.args.axis is not None:
+                out = self.bisection.value(variant)[self.args.axis]
+                print(out)
+            else:
+                if self.args.raw:
+                    print(self.bisection.value(variant))
+                else:
+                    print(self._current_value(variant))
+        except IndexError:
+            sys.stderr.write("Incorrect id "
+                             f"{'-'.join(str(_) for _ in variant)}\n")
+            sys.exit(-1)
 
     def identifier(self):
         """
         Print identifier of the current variant as shown by log
         """
         self._load_state()
         print('-'.join(str(_) for _ in self.bisection.current()))
@@ -502,16 +647,16 @@
     def log(self):
         """
         Print bisection log
         """
         self._load_state()
         print(self.bisection.log())
         if self.bisection.variants_left() == 0:
-            print("Bisection complete, last good combination:")
-            self._value()
+            print("Bisection complete, first bad combination:")
+            print(self._current_value())
 
     def reset(self):
         """
         Remove associated files
         """
         if not os.path.exists(self.args.state_file):
             sys.stderr.write(f"No bisection in '{self.args.state_file}' "
@@ -519,11 +664,7 @@
         else:
             try:
                 os.remove(self.args.state_file)
             except IOError as details:
                 sys.stderr.write(f"Failed to remove '{self.args.state_file}': "
                                  f"{details}\n")
                 sys.exit(-1)
-
-if __name__ == '__main__':
-    APP = Bisecter()
-    sys.exit(APP())
```

### Comparing `bisecter-0.1/bisecter.egg-info/PKG-INFO` & `bisecter-0.9/bisecter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisecter
-Version: 0.1
+Version: 0.9
 Summary: Allows to bisect over arbitrary number of arguments.
 Home-page: https://github.com/ldoktor/bisecter
 Author: Lukas Doktor
 Author-email: ldoktor@redhat.com
 License: GPLv2+
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `bisecter-0.1/scripts/bisecter` & `bisecter-0.9/scripts/bisecter`

 * *Files identical despite different names*

### Comparing `bisecter-0.1/setup.py` & `bisecter-0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,8 +78,8 @@
               "Programming Language :: Python :: 3",
               ],
           packages=find_packages(exclude=('selftests*',)),
           include_package_data=True,
           scripts=['scripts/bisecter'],
           test_suite='selftests',
           python_requires='>=3.5',
-          install_requires=['PyYAML'])
+          install_requires=[])
```

