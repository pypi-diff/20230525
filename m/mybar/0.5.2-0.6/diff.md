# Comparing `tmp/mybar-0.5.2.tar.gz` & `tmp/mybar-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mybar-0.5.2.tar", last modified: Mon Mar 20 08:32:09 2023, max compression
+gzip compressed data, was "mybar-0.6.tar", last modified: Thu May 25 10:20:50 2023, max compression
```

## Comparing `mybar-0.5.2.tar` & `mybar-0.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-03-20 08:32:09.319806 mybar-0.5.2/
--rw-r--r--   0 sam       (1000) sam       (1000)     1077 2023-03-16 08:41:11.000000 mybar-0.5.2/LICENSE
--rw-r--r--   0 sam       (1000) sam       (1000)     1000 2023-03-20 08:32:09.319806 mybar-0.5.2/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)      155 2023-03-16 08:41:11.000000 mybar-0.5.2/README.md
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-03-20 08:32:09.318806 mybar-0.5.2/mybar/
--rw-r--r--   0 sam       (1000) sam       (1000)      637 2023-03-20 08:29:45.000000 mybar-0.5.2/mybar/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)      293 2023-03-16 08:41:11.000000 mybar-0.5.2/mybar/__main__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1898 2023-03-16 08:41:11.000000 mybar-0.5.2/mybar/_setups.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6372 2023-03-16 08:41:11.000000 mybar-0.5.2/mybar/_types.py
--rw-r--r--   0 sam       (1000) sam       (1000)    36492 2023-03-18 03:38:58.000000 mybar-0.5.2/mybar/bar.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6921 2023-03-16 08:41:11.000000 mybar-0.5.2/mybar/cli.py
--rw-r--r--   0 sam       (1000) sam       (1000)      591 2023-03-16 08:41:11.000000 mybar-0.5.2/mybar/constants.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3554 2023-03-16 08:41:11.000000 mybar-0.5.2/mybar/errors.py
--rw-r--r--   0 sam       (1000) sam       (1000)    23527 2023-03-18 03:33:00.000000 mybar-0.5.2/mybar/field.py
--rw-r--r--   0 sam       (1000) sam       (1000)    15666 2023-03-20 08:26:57.000000 mybar-0.5.2/mybar/field_funcs.py
--rw-r--r--   0 sam       (1000) sam       (1000)    13184 2023-03-16 08:41:11.000000 mybar-0.5.2/mybar/formatting.py
--rw-r--r--   0 sam       (1000) sam       (1000)      284 2023-03-16 08:41:11.000000 mybar-0.5.2/mybar/log.py
--rw-r--r--   0 sam       (1000) sam       (1000)      124 2023-03-16 08:41:11.000000 mybar-0.5.2/mybar/templates.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5690 2023-03-16 08:41:11.000000 mybar-0.5.2/mybar/utils.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-03-20 08:32:09.319806 mybar-0.5.2/mybar.egg-info/
--rw-r--r--   0 sam       (1000) sam       (1000)     1000 2023-03-20 08:32:09.000000 mybar-0.5.2/mybar.egg-info/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)      436 2023-03-20 08:32:09.000000 mybar-0.5.2/mybar.egg-info/SOURCES.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-03-20 08:32:09.000000 mybar-0.5.2/mybar.egg-info/dependency_links.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-03-20 08:32:09.000000 mybar-0.5.2/mybar.egg-info/requires.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        6 2023-03-20 08:32:09.000000 mybar-0.5.2/mybar.egg-info/top_level.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       81 2023-03-16 08:41:11.000000 mybar-0.5.2/pyproject.toml
--rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-03-16 08:41:11.000000 mybar-0.5.2/requirements.txt
--rw-r--r--   0 sam       (1000) sam       (1000)      892 2023-03-20 08:32:09.320806 mybar-0.5.2/setup.cfg
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-05-25 10:20:50.149733 mybar-0.6/
+-rw-r--r--   0 sam       (1000) sam       (1000)     1077 2023-03-16 08:41:11.000000 mybar-0.6/LICENSE
+-rw-r--r--   0 sam       (1000) sam       (1000)      998 2023-05-25 10:20:50.149733 mybar-0.6/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)      155 2023-03-16 08:41:11.000000 mybar-0.6/README.md
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-05-25 10:20:50.149733 mybar-0.6/mybar/
+-rw-r--r--   0 sam       (1000) sam       (1000)      634 2023-05-25 10:17:15.000000 mybar-0.6/mybar/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1254 2023-05-23 09:48:03.000000 mybar-0.6/mybar/__main__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1898 2023-05-03 22:40:40.000000 mybar-0.6/mybar/_setups.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6381 2023-04-30 05:49:24.000000 mybar-0.6/mybar/_types.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    41160 2023-05-25 09:53:23.000000 mybar-0.6/mybar/bar.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     9230 2023-04-30 05:26:06.000000 mybar-0.6/mybar/cli.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      668 2023-03-21 09:17:30.000000 mybar-0.6/mybar/constants.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3554 2023-03-16 08:41:11.000000 mybar-0.6/mybar/errors.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    26274 2023-05-25 09:51:04.000000 mybar-0.6/mybar/field.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    16948 2023-05-25 09:55:29.000000 mybar-0.6/mybar/field_funcs.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    16853 2023-05-23 12:13:22.000000 mybar-0.6/mybar/formatting.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      284 2023-03-16 08:41:11.000000 mybar-0.6/mybar/log.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    13368 2023-05-03 06:07:43.000000 mybar-0.6/mybar/sync.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      124 2023-03-16 08:41:11.000000 mybar-0.6/mybar/templates.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5690 2023-03-16 08:41:11.000000 mybar-0.6/mybar/utils.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-05-25 10:20:50.149733 mybar-0.6/mybar.egg-info/
+-rw-r--r--   0 sam       (1000) sam       (1000)      998 2023-05-25 10:20:50.000000 mybar-0.6/mybar.egg-info/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)      450 2023-05-25 10:20:50.000000 mybar-0.6/mybar.egg-info/SOURCES.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-05-25 10:20:50.000000 mybar-0.6/mybar.egg-info/dependency_links.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-05-25 10:20:50.000000 mybar-0.6/mybar.egg-info/requires.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        6 2023-05-25 10:20:50.000000 mybar-0.6/mybar.egg-info/top_level.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       81 2023-03-16 08:41:11.000000 mybar-0.6/pyproject.toml
+-rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-03-16 08:41:11.000000 mybar-0.6/requirements.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)      890 2023-05-25 10:20:50.149733 mybar-0.6/setup.cfg
```

### Comparing `mybar-0.5.2/LICENSE` & `mybar-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mybar-0.5.2/PKG-INFO` & `mybar-0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mybar
-Version: 0.5.2
+Version: 0.6
 Summary: An async status bar with a highly customizable API.
-Home-page: https://github.com/sleepyabsol/mybar
-Author: sleepyabsol
+Home-page: https://github.com/lonelyabsol/mybar
+Author: lonelyabsol
 License: MIT
-Project-URL: GitHub: repo, https://github.com/sleepyabsol/mybar
+Project-URL: GitHub: repo, https://github.com/lonelyabsol/mybar
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `mybar-0.5.2/mybar/_setups.py` & `mybar-0.6/mybar/_setups.py`

 * *Files identical despite different names*

### Comparing `mybar-0.5.2/mybar/_types.py` & `mybar-0.6/mybar/_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,16 @@
 class MissingFieldnameError(FormatStringError):
     '''
     Raised when a format string field lacks a fieldname (i.e. is positional)
     when one is expected.
 
     '''
     @classmethod
-    def with_highlighting(cls,
+    def with_highlighting(
+        cls,
         sigs: FormatterFieldSig,
         epilogue: str
     ) -> Self:
         '''
         '''
         rebuilt = ""
         highlight = " "  # Account for the repr quotation mark.
```

### Comparing `mybar-0.5.2/mybar/bar.py` & `mybar-0.6/mybar/bar.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,16 @@
     :type defaults: :class:`dict`
 
     .. note:: `options` and `defaults` must be :class:`dict` instances
         of form :class:`_types.BarTemplateSpec`
 
     '''
 
-    def __init__(self,
+    def __init__(
+        self,
         options: BarTemplateSpec = {},
         defaults: BarTemplateSpec = None,
     ) -> None:
         if defaults is None:
             self.defaults = Bar._default_params.copy()
         else:
             self.defaults = defaults.copy()
@@ -96,15 +97,16 @@
         cls = type(self).__name__
         file = self.file
         maybe_file = f"{file=}, " if file else ""
         params = {**self}
         return f"<{cls} {maybe_file}{params}>"
 
     @classmethod
-    def from_file(cls,
+    def from_file(
+        cls,
         file: PathLike = None,
         *,
         defaults: BarTemplateSpec = None,
         overrides: BarTemplateSpec = {},
     ) -> Self:
         '''
         Return a new :class:`BarTemplate` from a config file path.
@@ -141,16 +143,17 @@
 
         options = file_spec | overrides
         t = cls(options, defaults)
         t.file = absolute
         return t
 
     @classmethod
-    def from_stdin(cls,
-        write_new_file_dft: bool = False
+    def from_stdin(
+        cls,
+        write_new_file_dft: bool = True
     ) -> Self:
         '''Return a new :class:`BarTemplate` using args from STDIN.
         Prompt the user before writing a new config file if one does
         not exist.
 
         :param write_new_file_dft: Automatically write new files,
             defaults to ``False``
@@ -168,24 +171,21 @@
 ##        except OSError as e:
 ##            parser.quit(e)
 
         try:
             template = cls.from_file(overrides=bar_options)
         except OSError as e:
             file = e.filename
-            errmsg = (
-                f"{parser.prog}: error:\n"
-                f"The config file at {file!r} does not exist."
-            )
+            msg = (f"The config file at {file!r} does not exist.")
             question = "Would you like to make it now?"
             write_options = {'y': True, 'n': False}
             default = 'ny'[write_new_file_dft]
             handler = cli.OptionsAsker(write_options, default, question)
 
-            print(errmsg)
+            print(msg)
             write_new_file = handler.ask()
             if write_new_file:
                 cls.write_file(file, bar_options)
                 print(f"Wrote new config file at {file!r}")
                 template = cls.from_file(file)
             else:
                 parser.quit()
@@ -324,26 +324,27 @@
 
     _default_params = {
         'separator': '|',
         'refresh_rate': 1.0,
         'field_order': list(_default_field_order)
     }
 
-    def __init__(self,
+    def __init__(
+        self,
         fmt: str = None,
         fields: Iterable[Field | str] = None,
         *,
         field_order: Iterable[FieldName] = None,
         separator: str = '|',
         refresh_rate: float = 1.0,
         stream: IO = sys.stdout,
         run_once: bool = False,
         align_to_seconds: bool = True,
         join_empty_fields: bool = False,
-        override_cooldown: float = 1/60,
+        override_cooldown: float = 1/8,
         thread_cooldown: float = 1/8,
 
         # Set this to use different seps for different output streams:
         separators: Sequence[PTY_Separator, TTY_Separator] = None,
 
         debug: bool = DEBUG,  # Not yet implemented!
     ) -> None:
@@ -423,22 +424,27 @@
         # interval when the bar stops.
         # (A shorter cooldown means faster exits):
         self._thread_cooldown = thread_cooldown
 
         # The set of field threads the bar must wait to join before
         # printing a line with run_once:
         self._threads = set()
+        self._printer_thread = None
+
+        self._coros = []
+        self._timely_fields = []
 
         # Calling run() sets this Event. Unsetting it stops all fields:
         self._can_run = threading.Event()
+        self.running = self._can_run.is_set
 
         # The bar's async event loop:
         self._loop = asyncio.new_event_loop()
 
-    def __contains__(self, other) -> bool:
+    def __contains__(self, other: FieldPrecursor) -> bool:
         if isinstance(other, str):
             weak_test = (other in self._field_order)
             return weak_test
 
         elif isinstance(other, Field):
             less_weak_test = (other.name in self._field_order)
             return less_weak_test
@@ -472,58 +478,17 @@
 
     def __repr__(self) -> str:
         names = self._field_order
         fields = utils.join_options(names, final_sep='', limit=3)
         cls = type(self).__name__
         return f"{cls}(fields=[{fields}])"
 
-    def append(self, field: FieldPrecursor) -> Self:
-        '''
-        Append a new Field to the bar.
-
-        `field` will be converted to :class:`Field`,
-        appended to the field list and joined to the end of the bar output.
-        If :attr:`Bar.fmt` is defined, it will override the new field order.
-
-        :param field: The field to append
-        :type field: :class:`FieldPrecursor`
-
-        :returns: The modified bar
-        :rtype: :class:`Bar`
-        '''
-        (name,), normalized = self._normalize_fields((field,))
-        self._fields.update(normalized)
-        self._buffers[name] = ''
-        self._field_order.append(name)
-        return self
-
-    def extend(self, fields: Iterable[FieldPrecursor]) -> Self:
-        '''
-        Append several new Fields to the bar.
-        Field precursors in `fields` will be converted to :class:`Field`,
-        appended to the field list and joined to the end of the bar output.
-        If :attr:`Bar.fmt` is defined, it will override the new field order.
-        the fields are displayed.
-
-        :param field: The fields to append
-        :type field: :class:`FieldPrecursor`
-
-        :returns: The modified bar
-        :rtype: :class:`Bar`
-        '''
-        #TODO: Consider Bar.fmt += FormatterFieldSig(field).as_string()
-        names, normalized = self._normalize_fields(fields)
-        self._fields.update(normalized)
-        self._buffers.update(dict.fromkeys(names, ''))
-        self._field_order.extend(names)
-        return self
-
-
     @classmethod
-    def from_template(cls,
+    def from_template(
+        cls,
         tmpl: BarTemplate,
         *,
         ignore_with: Pattern | tuple[Pattern] | None = '//'
     ) -> Self:
         '''
         Return a new :class:`Bar` from a :class:`BarTemplate`
         or a dict of :class:`Bar` parameters.
@@ -576,20 +541,22 @@
                 )
         else:
             field_order, field_sigs = cls.parse_fmt(fmt)
 
         # Ensure icon assignments correspond to valid fields:
         for name in field_icons:
             if name not in field_order:
-                expctd_from_icons = utils.join_options(field_order)
+                deduped = dict.fromkeys(field_order)  # Preserve order
+                expctd_from_icons = utils.join_options(deduped)
                 exc = utils.make_error_message(
                     InvalidFieldError,
                     doing_what="parsing custom Field icons",
                     blame=f"{name!r}",
-                    expected=f"a Field name found in {expctd_from_icons}"
+                    expected=f"a Field name from among {expctd_from_icons}",
+                    epilogue="Only assign icons to Fields that will be in the Bar."
                 )
                 raise exc from None
 
         # Gather Field parameters and instantiate them:
         fields = {}
         expctd_name="the name of a default or properly defined `custom` Field"
 
@@ -686,14 +653,17 @@
 
         :returns: a new :class:`Bar` using command line arguments
         :rtype: :class:`Bar`
         '''
         template = BarTemplate.from_stdin()
         return cls.from_template(template)
 
+##    @classmethod
+##    def as_generator(cls, 
+
     @property
     def clearline_char(self) -> str:
         '''
         A special character printed to TTY streams between refreshes.
         Its purpose is to clear characters left behind by longer lines.
         '''
         if self._stream is None:
@@ -720,14 +690,56 @@
         It defaults to the TTY sep (self._separators[1]) if no stream is set.
         '''
         if self._stream is None:
             # Default to using the terminal separator:
             return self._separators[1]
         return self._separators[self._stream.isatty()]
 
+    def append(self, field: FieldPrecursor) -> Self:
+        '''
+        Append a new Field to the bar.
+
+        `field` will be converted to :class:`Field`,
+        appended to the field list and joined to the end of the bar output.
+        If :attr:`Bar.fmt` is defined, it will override the new field order.
+
+        :param field: The field to append
+        :type field: :class:`FieldPrecursor`
+
+        :returns: The modified bar
+        :rtype: :class:`Bar`
+        '''
+        (name,), normalized = self._normalize_fields((field,))
+        self._fields.update(normalized)
+        self._buffers[name] = ''
+        self._field_order.append(name)
+        return self
+
+    def extend(self, fields: Iterable[FieldPrecursor]) -> Self:
+        '''
+        Append several new Fields to the bar.
+        Field precursors in `fields` will be converted to :class:`Field`,
+        appended to the field list and joined to the end of the bar output.
+        If :attr:`Bar.fmt` is defined, it will override the new field order.
+        the fields are displayed.
+
+        :param field: The fields to append
+        :type field: :class:`FieldPrecursor`
+
+        :returns: The modified bar
+        :rtype: :class:`Bar`
+        '''
+        #TODO: Consider Bar.fmt += FormatterFieldSig(field).as_string()
+        names, normalized = self._normalize_fields(fields)
+        self._fields.update(normalized)
+        self._buffers.update(dict.fromkeys(names, ''))
+        self._field_order.extend(names)
+        return self
+
+
     @staticmethod
     def parse_fmt(
         fmt: FormatStr
     ) -> tuple[FieldOrder, FmtStrStructure]:
         '''
         Return a dict mapping field names to :class:`FormatterFieldSig`.
         Keys of the dict can act as a field order.
@@ -773,15 +785,16 @@
         if not all(hasattr(stream, a) for a in io_methods):
             io_method_calls = [a + '()' for a in io_methods]
             joined = utils.join_options(io_method_calls, final_sep='and')
             raise TypeError(
                 f"Output stream {stream!r} needs {joined} methods."
             )
 
-    def _normalize_fields(self,
+    def _normalize_fields(
+        self,
         fields: Iterable[FieldPrecursor],
     ) -> tuple[FieldOrder, dict[FieldName, Field]]:
         '''
         Convert :class:`Field` precursors to :class:`Field` instances.
 
         Take an iterable of field names, :class:`Field` instances, or
         :class:`FormatterFieldSig` tuples and convert them to
@@ -825,14 +838,24 @@
                 raise InvalidFieldError(f"Invalid field precursor: {field!r}")
 
             normalized[new_field.name] = new_field
             names.append(new_field.name)
 
         return names, normalized
 
+    def line_generator(self) -> Iterator:
+        '''
+        Return a generator yielding status lines.
+        '''
+        while self.running():
+            if self._timely_fields:
+                self._preload_timely_fields()
+            line = self._make_one_line()
+            yield line
+
     def run(self, once: bool = None, stream: IO = None) -> None:
         '''
         Run the bar in the specified output stream.
         Block until an exception is raised and exit smoothly.
 
         :param stream: The IO stream in which to run the bar,
             defaults to :attr:`Bar._stream`
@@ -846,69 +869,181 @@
         .. note::
             This method cannot be called within an async event loop.
         '''
         if stream is not None:
             self._stream = stream
         if once is None:
             once = self.run_once
+        else:
+            self.run_once = once
 
-        # Allow the bar to run repeatedly in the same interpreter.
+        # Allow the bar to run repeatedly in the same interpreter:
         if self._loop.is_closed():
             self._loop = asyncio.new_event_loop()
+
         try:
+            # The following must be done in a very specific order.
             self._can_run.set()
-            self._loop.run_until_complete(self._startup(once))
+            self._prepare_fields()
+
+            # When printing indefinitely, if the line printer is not
+            # started before coros, the bar is blank the whole time.
+            if not once:
+                self._start_printer()
+
+            self._loop.run_until_complete(self._start_coros())
+
+            # Wait for threads to finish to get a full line, then print.
+            while self._threads:
+                time.sleep(self._thread_cooldown)
+            self._print_one_line()
+
+            if once:
+                self._can_run.clear()
+
+            # Block the main thread while other threads run, if there
+            # are no coroutines.
+            while self.running():
+                time.sleep(self._thread_cooldown)
 
         except KeyboardInterrupt:
             pass
 
         finally:
             self._shutdown()
 
-    async def _startup(self, run_once: bool = False) -> None:
-        '''
-        Run field coroutines, threads and the line printer in parallel.
-        '''
+    def _prepare_fields(self) -> None:
         overriding = False
-        gathered = []
-
         for field in self:
             if field.overrides_refresh:
                 overriding = True
 
             if field.threaded:
-                await field.send_to_thread(run_once=run_once)
+                field.send_to_thread(run_once=self.run_once)
+            elif field.timely:
+                self._timely_fields.append(field)
             else:
-                gathered.append(field.run(run_once))
+                self._coros.append(field.run(self.run_once))
+##        if overriding:  # Currently disabled!
+##            self._coros.append(self._handle_overrides())
 
-        if run_once:
-            await asyncio.gather(*gathered)
-            # Wait for threads to finish:
-            while self._threads:
-                await asyncio.sleep(self._thread_cooldown)
-            self._print_one_line()
+    async def _start_coros(self) -> None:
+        await asyncio.gather(*self._coros)
+
+    def _preload_timely_fields(self) -> None:
+        '''
+        Update the bar buffers for Fields with :attr:`Field.timely`.
+        This is used most often right before printing a line.
+        '''
+        for f in self._timely_fields:
+            if f.is_async:
+                result = asyncio.run(f._func(*f.args, **f.kwargs))
+            else:
+                result = f._func(*f.args, **f.kwargs)
+            self._buffers[f.name] = result
+
+    def _start_printer(self, end: str = '\r') -> None:
+        self._printer_thread = threading.Thread(
+            target=self._threaded_continuous_line_printer,
+            name='PRINTER',
+            args=(end,)
+        )
+        self._threads.add(self._printer_thread)
+        self._printer_thread.start()
+
+    def _threaded_continuous_line_printer(self, end: str = '\r') -> None:
+        '''
+        The bar's primary line-printing mechanism.
+        Fields with the ``timely`` attribute get run here.
+        Other fields are responsible for sending data to bar buffers.
+        This only writes using the current buffer contents.
 
+        :param end: The string appended to the end of each line
+        :type end: :class:`str`
+        '''
+        using_format_str = (self.fmt is not None)
+        sep = self.separator
+        clock = time.monotonic
+
+        if self.in_a_tty:
+            beginning = self.clearline_char + end
+            self._stream.write(CSI + HIDE_CURSOR)
         else:
-            if overriding:
-                gathered.append(self._handle_overrides())
-            await asyncio.gather(
-                *gathered,
-                self._continuous_line_printer()
-            )
+            beginning = self.clearline_char
+
+        # Flushing the buffer before writing to it fixes poor i3bar alignment.
+        self._stream.flush()
+
+        # Print something right away just so that the bar is not empty:
+        self._print_one_line()
+
+        if self.align_to_seconds:
+            # Begin every refresh at the start of a clock second:
+            clock = time.time
+            time.sleep(1 - (clock() % 1))
+
+        step = self._thread_cooldown
+        count = 0
+        needed = round(self.refresh_rate / step)
+
+        start_time = clock()
+        while self.running():
+
+            # Sleep until the next refresh cycle, pausing for a bit in
+            # case the bar stops.
+            if count < needed:
+                count += 1
+
+                # Latency from nonzero execution times causes drift,
+                # where sleeps become out-of-sync and the bar skips
+                # field updates.
+                # This is especially noticeable in fields that update
+                # routinely, such as the time.
+
+                # To negate drift, when sleeping until the beginning of
+                # the next cycle, we must also compensate for latency.
+                time.sleep(
+                    step - (
+                        # Get the current latency, which can vary:
+                        clock() % step
+                    )
+                )
+                continue
+
+            count = 0
+
+            # Run time-sensitive fields right away:
+            for f in self._timely_fields:
+                if f.is_async:
+                    result = asyncio.run(f._func(*f.args, **f.kwargs))
+                else:
+                    result = f._func(*f.args, **f.kwargs)
+                self._buffers[f.name] = result
+
+            if using_format_str:
+                line = self.fmt.format_map(self._buffers)
+            else:
+                line = sep.join(
+                    buf for field in self._field_order
+                        if (buf := self._buffers[field])
+                        or self.join_empty_fields
+                )
+
+            self._stream.write(beginning + line + end)
+            self._stream.flush()
 
     def _shutdown(self) -> None:
         '''
         Notify fields that the bar has stopped and join threads.
         Also print a newline and unhide the cursor if the bar was
         running in a TTY.
         '''
         self._can_run.clear()
-        for field in self:
-            if field.threaded and field._thread is not None:
-                field._thread.join()
+        for thread in self._threads:
+            thread.join()
 
         if self.in_a_tty:
             self._stream.write('\n')
             self._stream.write(CSI + UNHIDE_CURSOR)
 
     async def _continuous_line_printer(self, end: str = '\r') -> None:
         '''
@@ -917,15 +1052,14 @@
         This only writes using the current buffer contents.
 
         :param end: The string appended to the end of each line
         :type end: :class:`str`
         '''
         using_format_str = (self.fmt is not None)
         sep = self.separator
-        running = self._can_run.is_set
         clock = time.monotonic
 
         if self.in_a_tty:
             beginning = self.clearline_char + end
             self._stream.write(CSI + HIDE_CURSOR)
         else:
             beginning = self.clearline_char
@@ -938,15 +1072,15 @@
 
         if self.align_to_seconds:
             # Begin every refresh at the start of a clock second:
             clock = time.time
             await asyncio.sleep(1 - (clock() % 1))
 
         start_time = clock()
-        while running():
+        while self.running():
             if using_format_str:
                 line = self.fmt.format_map(self._buffers)
             else:
                 line = sep.join(
                     buf for field in self._field_order
                         if (buf := self._buffers[field])
                         or self.join_empty_fields
@@ -970,23 +1104,22 @@
         Print a line when fields with overrides_refresh send new data.
 
         :param end: The string appended to the end of each line
         :type end: :class:`str`
         '''
         sep = self.separator
         using_format_str = (self.fmt is not None)
-        running = self._can_run.is_set
 
         if self.in_a_tty:
             beginning = self.clearline_char + end
         else:
             beginning = self.clearline_char
 
         start_time = time.time()
-        while running():
+        while self.running():
 
             try:
                 # Wait until a field with overrides_refresh sends new
                 # data to be printed:
                 field, contents = await self._override_queue.get()
                 # if DEBUG:
                     # logger.debug(f"handler: {field} {time.time() - start_time}")
@@ -1034,15 +1167,18 @@
             beginning = self.clearline_char + end
         else:
             beginning = self.clearline_char
 
         # Flushing the buffer before writing to it fixes poor i3bar alignment.
         self._stream.flush()
 
+        if self._timely_fields:
+            self._preload_timely_fields()
         self._stream.write(beginning + self._make_one_line() + end)
+
         self._stream.flush()
 
 
 def run(once: bool = False, file: PathLike = None) -> NoReturn | None:
     '''
     Generate a new :class:`Bar` and run it in STDOUT.
     Optionally generate the bar from a config file.
```

### Comparing `mybar-0.5.2/mybar/constants.py` & `mybar-0.6/mybar/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,8 +20,10 @@
 '''VT100 escape code to clear the line.'''
 HIDE_CURSOR: ConsoleControlCode = '?25l'
 '''VT100 escape code to hide the cursor.'''
 UNHIDE_CURSOR: ConsoleControlCode = '?25h'
 '''VT100 escape code to unhide the cursor.'''
 
 
+FONTAWESOME_ICONS = tuple('')
+USING_FONTAWESOME = False
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mybar-0.5.2/mybar/errors.py` & `mybar-0.6/mybar/errors.py`

 * *Files identical despite different names*

### Comparing `mybar-0.5.2/mybar/field.py` & `mybar-0.6/mybar/field.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,17 @@
 
     :param interval: How often in seconds field contents are updated, defaults to ``1.0``
     :type interval: :class:`float`
 
     :param align_to_seconds: Update contents at the start of each second, defaults to ``False``
     :type align_to_seconds: :class:`bool`
 
+    :param timely: Run the field as soon as possible after every refresh, defaults to ``False``
+    :type timely: :class:`bool`
+
     :param overrides_refresh: Updates to this field re-print the bar between refreshes, defaults to ``False``
     :type overrides_refresh: :class:`bool`
 
     :param threaded: Run this field in a separate thread, defaults to ``False``
     :type threaded: :class:`bool`
 
     :param always_show_icon: Show icons even when contents are empty, defaults to ``False``
@@ -174,37 +177,41 @@
             'icons': [' ', 'Bat '],
         },
 
         'net_stats': {
             'name': 'net_stats',
             'func': field_funcs.get_net_stats,
             'interval': 4,
+            'threaded': True,
             'icons': [' ', ''],
         },
 
         'datetime': {
             'name': 'datetime',
             # 'func': field_funcs.precision_datetime,
             'func': field_funcs.get_datetime,
             'align_to_seconds': True,
+            'timely': True,
             'kwargs': {
                 'fmt': "%Y-%m-%d %H:%M:%S"
             },
         }
 
     }
 
-    def __init__(self,
+    def __init__(
+        self,
         *,
         name: FieldName = None,
         func: Callable[P, str] = None,
         icon: str = '',
         fmt: FormatStr = None,
         interval: float = 1.0,
         align_to_seconds: bool = False,
+        timely: bool = False,
         overrides_refresh: bool = False,
         threaded: bool = False,
         always_show_icon: bool = False,
         run_once: bool = False,
         constant_output: str = None,
         bar: Bar_T = None,
         args: Args = None,
@@ -248,33 +255,38 @@
 
         if fmt is None and icons is None:
             raise IncompatibleArgsError(
                 "An icon is required when fmt is None."
             )
         self.fmt = fmt
 
-        self._bar = bar
+        self.is_async = asyncio.iscoroutinefunction(func)
 
-        if asyncio.iscoroutinefunction(func) or threaded:
+        if self.is_async or threaded or timely:
             self._callback = func
         else:
-            # Wrap a synchronous function if the field is not threaded:
+            # Wrap synchronous functions if they aren't special:
             self._callback = self._asyncify
 
+        self._bar = bar
+
+        self.timely = timely
         self.align_to_seconds = align_to_seconds
         self.always_show_icon = always_show_icon
         self._buffer = None
         self.constant_output = constant_output
         self.interval = interval
         self.overrides_refresh = overrides_refresh
         self.run_once = run_once
 
         self.threaded = threaded
         self._thread = None
 
+        self._do_setup()
+
     def __repr__(self) -> str:
         cls = type(self).__name__
         name = self.name
         # attrs = utils.join_options(...)
         return f"{cls}({name=})"
 
     def __eq__(self, other: Field) -> bool:
@@ -298,15 +310,16 @@
             and self.args == other.args
             and self.kwargs == other.kwargs
         ):
             return True
         return False
 
     @classmethod
-    def from_default(cls: Field,
+    def from_default(
+        cls: Field,
         name: str,
         *,
         overrides: FieldSpec = {},
         source: dict[FieldName, FieldSpec] = None,
         fmt_sig: FormatStr = None
     ) -> Field:
         '''Quickly get a default Field and customize its parameters.
@@ -329,15 +342,15 @@
             source = cls._default_fields
 
         try:
             default: FieldSpec = source[name].copy()
         except KeyError:
             raise DefaultFieldNotFoundError(
                 f"{name!r} is not the name of a default Field."
-            )
+            ) from None
 
         if 'kwargs' in overrides and 'kwargs' in default:
             # default['kwargs'].update(overrides['kwargs'])
             # default['kwargs'] |= overrides['kwargs']
             overrides['kwargs'] = default['kwargs'] | overrides['kwargs']
 
         spec = default | overrides
@@ -383,14 +396,89 @@
             if always_show_icon or text:
                 return icon + text
             else:
                 return text
         else:
             return fmt.format(text, icon=icon)
 
+    def _auto_format(self, text: str) -> 'Contents':
+        '''Non-staticmethod _format_contents...'''
+        if self.fmt is None:
+            if self.always_show_icon or text:
+                return self.icon + text
+            else:
+                return text
+        else:
+            return self.fmt.format(text, icon=self.icon)
+
+    def as_generator(self, once: bool = False) :
+        yield self._func
+
+    def _do_setup(self, args: Args = None, kwargs: Kwargs = None) -> None:
+        # Use the pre-defined _setupfunc() to gather constant variables
+        # for func() which might only be evaluated at runtime:
+        if self._setupfunc is None:
+            return
+
+        if args is None:
+            args = self.args
+        if kwargs is None:
+            kwargs = self.kwargs
+
+        try:
+            if asyncio.iscoroutinefunction(self._setupfunc):
+                setupvars = asyncio.run(
+                    self._setupfunc(*self.args, **self.kwargs)
+                )
+            else:
+                setupvars = self._setupfunc(*self.args, **self.kwargs)
+
+        # If _setupfunc raises FailedSetup with a backup value,
+        # use it as the field's new constant_output:
+        except FailedSetup as e:
+            backup = e.backup
+            self.constant_output = self._auto_format(backup)
+            return
+
+        # On success, give new values to kwargs to pass to _func().
+        # return setupvars
+        kwargs['setupvars'] = setupvars
+
+
+##    # For threaded fields, still run continuously!!!
+
+    def sync_run(self, once: bool = None) -> 'Contents':
+        # Do not run fields which have a constant output;
+        # only set their bar buffer.
+        if self.constant_output is not None:
+            return self._auto_format(self.constant_output)
+
+        if self.is_async:
+            result = asyncio.run(self._func(*self.args, **self.kwargs))
+        else:
+            result = self._func(*self.args, **self.kwargs)
+        contents = self._auto_format(result)
+
+        return contents
+
+    def gen_run(self, once: bool = None) -> 'Contents':
+        # Do not run fields which have a constant output;
+        # only set their bar buffer.
+        if self.constant_output is not None:
+            return self._auto_format(self.constant_output)
+
+        while True:
+            if self.is_async:
+                result = self._func(*self.args, **self.kwargs)
+            else:
+                result = asyncio.run(self._func(*self.args, **self.kwargs))
+            contents = self._auto_format(result)
+
+            yield contents
+
     async def run(self, once: bool = False) -> None:
         '''
         Run an asynchronous field callback and send updates to the bar.
         '''
         self._check_bar()
         bar = self._bar
         # Do not run fields which have a constant output;
@@ -439,20 +527,15 @@
 
             # On success, give new values to kwargs to pass to func().
             self.kwargs['setupvars'] = setupvars
 
         # Run at least once at the start to ensure the bar is not empty:
         result = await func(*self.args, **self.kwargs)
         last_val = result
-        contents = self._format_contents(
-            result,
-            self.icon,
-            self.fmt,
-            self.always_show_icon
-        )
+        contents = self._auto_format(result)
         bar._buffers[self.name] = contents
 
         if self.run_once or once:
             return
 
         if self.align_to_seconds:
             # Sleep until the beginning of the next second.
@@ -528,18 +611,16 @@
         step = bar._thread_cooldown
         func = self._callback
         using_format_str = (self.fmt is not None)
         last_val = None
 
         # If the field's callback is asynchronous,
         # it must be run in a new event loop.
-        is_async = asyncio.iscoroutinefunction(func)
         local_loop = asyncio.new_event_loop()
 
-
         # Use the pre-defined _setupfunc() to gather constant variables
         # for func() which might only be evaluated at runtime:
         if self._setupfunc is not None:
             try:
                 if asyncio.iscoroutinefunction(self._setupfunc):
                     setupvars = local_loop.run_until_complete(
                         self._setupfunc(*self.args, **self.kwargs)
@@ -562,15 +643,15 @@
                 bar._buffers[self.name] = str(contents)
                 return
 
             # On success, give new values to kwargs to pass to func().
             self.kwargs['setupvars'] = setupvars
 
         # Run at least once at the start to ensure the bar is not empty:
-        if is_async:
+        if self.is_async:
             result = local_loop.run_until_complete(
                 func(*self.args, **self.kwargs)
             )
         else:
             result = func(*self.args, **self.kwargs)
         last_val = result
         contents = self._format_contents(
@@ -622,15 +703,15 @@
                         # (clock() - start_time) % step  # Preserve offset
                     )
                 )
                 continue
 
             count = 0
 
-            if is_async:
+            if self.is_async:
                 result = local_loop.run_until_complete(
                     func(*self.args, **self.kwargs)
                 )
             else:
                 result = func(*self.args, **self.kwargs)
 
             if result == last_val:
@@ -671,27 +752,27 @@
             if no_error:
                 return False
             raise MissingBarError(
                 "Fields cannot run until they belong to a Bar."
             )
         return True
 
-    async def send_to_thread(self, *, run_once: bool = True) -> None:
+    def send_to_thread(self, *, run_once: bool = True) -> None:
         '''
         Make and start a thread in which to run the :class:`Field` callback.
 
         :param run_once: Only run the :class:`Field` callback once,
             defaults to ``True`` to prevent uncontrolled thread spawning
         :type run_once: :class:`bool`
         '''
+        self._check_bar()
         self._thread = threading.Thread(
             target=self.run_threaded,
             name=self.name,
             args=(run_once,)
         )
-        if self._bar is not None:
-            self._bar._threads.add(self._thread)
+        self._bar._threads.add(self._thread)
         self._thread.start()
 
 
 FieldPrecursor: TypeAlias = FieldName | Field | FormatterFieldSig
```

### Comparing `mybar-0.5.2/mybar/field_funcs.py` & `mybar-0.6/mybar/field_funcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 from .errors import *
 from .formatting import ElapsedTime, ConditionalFormatStr
 from .utils import join_options
 from ._types import Contents, FormatStr, NmConnFilterSpec
 
 from collections.abc import Callable, Iterable
-from typing import Literal, TypeAlias
+from typing import Literal, TypeAlias, NamedTuple, Any
+from enum import Enum
 
 
 FormatterLiteral: TypeAlias = str|None
 FormatterFname: TypeAlias = str|None
 FormatterFormatSpec: TypeAlias = str|None
 FormatterConversion: TypeAlias = str|None
 FmtStrStructure: TypeAlias = tuple[tuple[tuple[
@@ -88,14 +89,62 @@
     avg_pct = sum(int(p) for p in pcts) // len(pcts)
     is_on = any(s == 'on' for s in states)
     # return is_on, avg_pct
     state = "" if is_on else "M"
     return fmt.format(avg_pct, state=state)
 
 
+class Context(NamedTuple):
+    contents: str = None
+    state: Any = None
+
+class BatteryStates(Enum):
+    CHARGING = 'charging'
+    DISCHARGING = 'discharging'
+
+def ctx_get_battery_info(
+    fmt: FormatStr = "{icon}{pct:02.0f}",
+    # fmt: FormatStr = "{icon}{pct:02.0f}{state}",
+    *args, **kwargs
+) -> Context:
+    '''
+    Battery capacity as a percent and whether or not it is charging.
+    '''
+
+    # if not (battery := psutil.sensors_battery()):
+    battery = psutil.sensors_battery()
+    if not battery:
+        return Context()
+##        # return (None, None)
+    # state = "CHG" if battery.power_plugged else ''
+
+    # Progressive/dynamic battery icons!
+    icon_bank = "    ".split()
+    # return icon_bank
+
+    def mapper(n):
+        icon = ""
+        for i, test in enumerate((10, 25, 50, 75, 100)):
+            if n <= test:
+                icon = icon_bank[i]
+                return icon + " "
+
+    if battery.power_plugged:
+        icon = ""
+        # state = "CHG"
+    else:
+        icon = mapper(battery.percent)
+        # state = ""
+    # print(repricon)
+
+    info = fmt.format_map({'icon': icon, 'pct': battery.percent, 'state': battery.power_plugged})
+##    return battery.power_plugged, info
+    return info
+
+
 async def get_battery_info(
     fmt: FormatStr = "{pct:02.0f}{state}",
     *args, **kwargs
 ) -> Contents:
     '''
     Battery capacity as a percent and whether or not it is charging.
 
@@ -171,15 +220,15 @@
     :param interval: Time to block before returning a result.
         Only set this in a threaded :class:`Field`.
     :type interval: :class:`float`, optional
     '''
     return fmt.format(psutil.cpu_percent(interval))
 
 
-async def get_datetime(
+def get_datetime(
     fmt: str = "%Y-%m-%d %H:%M:%S",
     *args, **kwargs
 ) -> Contents:
     '''
     Current time as formatted with `fmt`.
 
     :param fmt: A format string with %-based format codes used by ``datetime.strftime()``,
```

### Comparing `mybar-0.5.2/mybar/utils.py` & `mybar-0.6/mybar/utils.py`

 * *Files identical despite different names*

### Comparing `mybar-0.5.2/mybar.egg-info/PKG-INFO` & `mybar-0.6/mybar.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mybar
-Version: 0.5.2
+Version: 0.6
 Summary: An async status bar with a highly customizable API.
-Home-page: https://github.com/sleepyabsol/mybar
-Author: sleepyabsol
+Home-page: https://github.com/lonelyabsol/mybar
+Author: lonelyabsol
 License: MIT
-Project-URL: GitHub: repo, https://github.com/sleepyabsol/mybar
+Project-URL: GitHub: repo, https://github.com/lonelyabsol/mybar
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `mybar-0.5.2/setup.cfg` & `mybar-0.6/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
 name = mybar
-version = 0.5.2
+version = 0.6
 description = An async status bar with a highly customizable API.
 long_description = file: README.md
 long_description_content_type = text/markdown
-author = sleepyabsol
-url = https://github.com/sleepyabsol/mybar
+author = lonelyabsol
+url = https://github.com/lonelyabsol/mybar
 project_urls = 
-	GitHub: repo = https://github.com/sleepyabsol/mybar
+	GitHub: repo = https://github.com/lonelyabsol/mybar
 classifiers = 
 	Development Status :: 3 - Alpha
 	Environment :: Console
 	Framework :: AsyncIO
 	Intended Audience :: End Users/Desktop
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
```

