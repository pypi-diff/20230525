# Comparing `tmp/arc_cli-8.4.2.tar.gz` & `tmp/arc_cli-8.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arc_cli-8.4.2.tar", max compression
+gzip compressed data, was "arc_cli-8.5.0.tar", max compression
```

## Comparing `arc_cli-8.4.2.tar` & `arc_cli-8.5.0.tar`

### file list

```diff
@@ -1,76 +1,77 @@
--rw-r--r--   0        0        0     1063 2023-05-10 21:06:03.754164 arc_cli-8.4.2/LICENSE
--rw-r--r--   0        0        0     1055 2023-05-10 22:16:10.825438 arc_cli-8.4.2/README.md
--rw-r--r--   0        0        0      737 2023-05-24 23:53:59.316827 arc_cli-8.4.2/arc/__init__.py
--rw-r--r--   0        0        0     1449 2023-05-10 22:23:55.102127 arc_cli-8.4.2/arc/api.py
--rw-r--r--   0        0        0     6902 2023-05-08 22:45:01.072694 arc_cli-8.4.2/arc/autocompletions.py
--rw-r--r--   0        0        0      114 2023-05-04 03:31:42.941981 arc_cli-8.4.2/arc/color.py
--rw-r--r--   0        0        0     6534 2023-05-08 22:45:01.072694 arc_cli-8.4.2/arc/config.py
--rw-r--r--   0        0        0      385 2023-05-08 22:45:01.072694 arc_cli-8.4.2/arc/constants.py
--rw-r--r--   0        0        0      121 2023-05-04 03:31:42.941981 arc_cli-8.4.2/arc/define/__init__.py
--rw-r--r--   0        0        0     1379 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/define/alias.py
--rw-r--r--   0        0        0     1768 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/define/classful.py
--rw-r--r--   0        0        0    17006 2023-05-22 02:08:31.587212 arc_cli-8.4.2/arc/define/command.py
--rw-r--r--   0        0        0     3101 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/define/documentation.py
--rw-r--r--   0        0        0      219 2023-05-04 03:31:42.941981 arc_cli-8.4.2/arc/define/param/__init__.py
--rw-r--r--   0        0        0     8036 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/define/param/constructors.py
--rw-r--r--   0        0        0     3480 2023-05-24 23:52:23.271126 arc_cli-8.4.2/arc/define/param/groups.py
--rw-r--r--   0        0        0     8694 2023-05-10 22:23:55.102127 arc_cli-8.4.2/arc/define/param/param.py
--rw-r--r--   0        0        0     8549 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/define/param/param_definition.py
--rw-r--r--   0        0        0     3388 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/define/param/param_mixin.py
--rw-r--r--   0        0        0     1889 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/define/param/param_tree.py
--rw-r--r--   0        0        0     6314 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/errors.py
--rw-r--r--   0        0        0     1070 2023-05-10 02:23:27.369848 arc_cli-8.4.2/arc/logging.py
--rw-r--r--   0        0        0    16336 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/parser.py
--rw-r--r--   0        0        0      402 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/present/__init__.py
--rw-r--r--   0        0        0     6168 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/present/ansi.py
--rw-r--r--   0        0        0     4681 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/present/box.py
--rw-r--r--   0        0        0     5319 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/present/console.py
--rw-r--r--   0        0        0      187 2023-05-04 03:31:42.945314 arc_cli-8.4.2/arc/present/data.py
--rw-r--r--   0        0        0     2126 2023-05-04 03:31:42.945314 arc_cli-8.4.2/arc/present/drawing.py
--rw-r--r--   0        0        0     2748 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/present/formatters.py
--rw-r--r--   0        0        0     9376 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/present/help_formatter.py
--rw-r--r--   0        0        0     3024 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/present/joiner.py
--rw-r--r--   0        0        0       54 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/present/markdown/__init__.py
--rw-r--r--   0        0        0     6614 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/present/markdown/markdown_parser.py
--rw-r--r--   0        0        0     3894 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/present/markdown/nodes.py
--rw-r--r--   0        0        0     1632 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/present/out.py
--rw-r--r--   0        0        0      987 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/present/pager.py
--rw-r--r--   0        0        0     9825 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/present/table.py
--rw-r--r--   0        0        0     5182 2023-05-08 22:45:01.076028 arc_cli-8.4.2/arc/present/wrap.py
--rw-r--r--   0        0        0      288 2023-05-04 03:31:42.945314 arc_cli-8.4.2/arc/prompt/__init__.py
--rw-r--r--   0        0        0     3731 2023-05-10 04:25:05.907299 arc_cli-8.4.2/arc/prompt/helpers.py
--rw-r--r--   0        0        0     5926 2023-05-10 22:23:55.105460 arc_cli-8.4.2/arc/prompt/prompt.py
--rw-r--r--   0        0        0      812 2023-05-08 22:45:01.079361 arc_cli-8.4.2/arc/prompt/prompts.py
--rw-r--r--   0        0        0     7111 2023-05-22 01:33:53.734884 arc_cli-8.4.2/arc/prompt/questions.py
--rw-r--r--   0        0        0        0 2023-05-04 03:31:42.948647 arc_cli-8.4.2/arc/py.typed
--rw-r--r--   0        0        0      304 2023-05-08 22:45:01.079361 arc_cli-8.4.2/arc/runtime/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-10 22:34:20.111031 arc_cli-8.4.2/arc/runtime/app.py
--rw-r--r--   0        0        0     2786 2023-05-10 22:23:55.105460 arc_cli-8.4.2/arc/runtime/context.py
--rw-r--r--   0        0        0    12733 2023-05-22 02:24:16.465843 arc_cli-8.4.2/arc/runtime/exec.py
--rw-r--r--   0        0        0    10026 2023-05-10 22:34:20.111031 arc_cli-8.4.2/arc/runtime/init.py
--rw-r--r--   0        0        0     7484 2023-05-24 23:43:58.232827 arc_cli-8.4.2/arc/runtime/middleware.py
--rw-r--r--   0        0        0     3097 2023-05-08 22:45:01.079361 arc_cli-8.4.2/arc/runtime/plugin.py
--rw-r--r--   0        0        0      382 2023-05-08 22:45:01.079361 arc_cli-8.4.2/arc/safe.py
--rw-r--r--   0        0        0     1866 2023-05-08 22:45:01.079361 arc_cli-8.4.2/arc/suggest.py
--rw-r--r--   0        0        0      362 2023-05-10 02:47:29.523000 arc_cli-8.4.2/arc/types/__init__.py
--rw-r--r--   0        0        0    14196 2023-05-10 02:57:55.763259 arc_cli-8.4.2/arc/types/aliases.py
--rw-r--r--   0        0        0      670 2023-05-10 22:23:55.105460 arc_cli-8.4.2/arc/types/convert.py
--rw-r--r--   0        0        0      545 2023-05-08 22:45:01.082694 arc_cli-8.4.2/arc/types/default.py
--rw-r--r--   0        0        0     4419 2023-05-10 03:51:44.284628 arc_cli-8.4.2/arc/types/file.py
--rw-r--r--   0        0        0       79 2023-05-04 03:31:42.951981 arc_cli-8.4.2/arc/types/middleware/__init__.py
--rw-r--r--   0        0        0     1397 2023-05-10 03:41:31.066410 arc_cli-8.4.2/arc/types/middleware/observers.py
--rw-r--r--   0        0        0     2630 2023-05-08 22:45:01.082694 arc_cli-8.4.2/arc/types/middleware/transformers.py
--rw-r--r--   0        0        0     4236 2023-05-10 02:44:59.447809 arc_cli-8.4.2/arc/types/middleware/validators.py
--rw-r--r--   0        0        0     3486 2023-05-08 22:45:01.082694 arc_cli-8.4.2/arc/types/network.py
--rw-r--r--   0        0        0      854 2023-05-04 03:31:42.951981 arc_cli-8.4.2/arc/types/numbers.py
--rw-r--r--   0        0        0      860 2023-05-08 22:45:01.082694 arc_cli-8.4.2/arc/types/path.py
--rw-r--r--   0        0        0     6881 2023-05-08 22:45:01.082694 arc_cli-8.4.2/arc/types/semver.py
--rw-r--r--   0        0        0      877 2023-05-08 22:45:01.082694 arc_cli-8.4.2/arc/types/state.py
--rw-r--r--   0        0        0     1960 2023-05-10 02:48:47.609034 arc_cli-8.4.2/arc/types/strings.py
--rw-r--r--   0        0        0     2300 2023-05-10 03:16:28.712436 arc_cli-8.4.2/arc/types/type_arg.py
--rw-r--r--   0        0        0     2718 2023-05-08 22:45:01.082694 arc_cli-8.4.2/arc/types/type_info.py
--rw-r--r--   0        0        0     3176 2023-05-08 22:45:01.082694 arc_cli-8.4.2/arc/types/users.py
--rw-r--r--   0        0        0     2257 2023-05-10 22:23:55.105460 arc_cli-8.4.2/arc/typing.py
--rw-r--r--   0        0        0     1036 2023-05-24 23:54:00.086819 arc_cli-8.4.2/pyproject.toml
--rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 arc_cli-8.4.2/setup.py
--rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 arc_cli-8.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-10 21:06:03.754164 arc_cli-8.5.0/LICENSE
+-rw-r--r--   0        0        0     1055 2023-05-10 22:16:10.825438 arc_cli-8.5.0/README.md
+-rw-r--r--   0        0        0      737 2023-05-25 00:49:19.714874 arc_cli-8.5.0/arc/__init__.py
+-rw-r--r--   0        0        0     1449 2023-05-10 22:23:55.102127 arc_cli-8.5.0/arc/api.py
+-rw-r--r--   0        0        0     6902 2023-05-08 22:45:01.072694 arc_cli-8.5.0/arc/autocompletions.py
+-rw-r--r--   0        0        0      114 2023-05-04 03:31:42.941981 arc_cli-8.5.0/arc/color.py
+-rw-r--r--   0        0        0     6534 2023-05-08 22:45:01.072694 arc_cli-8.5.0/arc/config.py
+-rw-r--r--   0        0        0      385 2023-05-08 22:45:01.072694 arc_cli-8.5.0/arc/constants.py
+-rw-r--r--   0        0        0      121 2023-05-04 03:31:42.941981 arc_cli-8.5.0/arc/define/__init__.py
+-rw-r--r--   0        0        0     1379 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/define/alias.py
+-rw-r--r--   0        0        0     1768 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/define/classful.py
+-rw-r--r--   0        0        0    17006 2023-05-22 02:08:31.587212 arc_cli-8.5.0/arc/define/command.py
+-rw-r--r--   0        0        0     3101 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/define/documentation.py
+-rw-r--r--   0        0        0      219 2023-05-04 03:31:42.941981 arc_cli-8.5.0/arc/define/param/__init__.py
+-rw-r--r--   0        0        0     8036 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/define/param/constructors.py
+-rw-r--r--   0        0        0     3480 2023-05-24 23:52:23.271126 arc_cli-8.5.0/arc/define/param/groups.py
+-rw-r--r--   0        0        0     8694 2023-05-10 22:23:55.102127 arc_cli-8.5.0/arc/define/param/param.py
+-rw-r--r--   0        0        0     8549 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/define/param/param_definition.py
+-rw-r--r--   0        0        0     3388 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/define/param/param_mixin.py
+-rw-r--r--   0        0        0     1889 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/define/param/param_tree.py
+-rw-r--r--   0        0        0     6314 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/errors.py
+-rw-r--r--   0        0        0     1070 2023-05-10 02:23:27.369848 arc_cli-8.5.0/arc/logging.py
+-rw-r--r--   0        0        0    16336 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/parser.py
+-rw-r--r--   0        0        0      402 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/present/__init__.py
+-rw-r--r--   0        0        0     6168 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/present/ansi.py
+-rw-r--r--   0        0        0     4681 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/present/box.py
+-rw-r--r--   0        0        0     5319 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/present/console.py
+-rw-r--r--   0        0        0      187 2023-05-04 03:31:42.945314 arc_cli-8.5.0/arc/present/data.py
+-rw-r--r--   0        0        0     2126 2023-05-04 03:31:42.945314 arc_cli-8.5.0/arc/present/drawing.py
+-rw-r--r--   0        0        0     2748 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/present/formatters.py
+-rw-r--r--   0        0        0     9376 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/present/help_formatter.py
+-rw-r--r--   0        0        0     3024 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/present/joiner.py
+-rw-r--r--   0        0        0       54 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/present/markdown/__init__.py
+-rw-r--r--   0        0        0     6614 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/present/markdown/markdown_parser.py
+-rw-r--r--   0        0        0     3894 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/present/markdown/nodes.py
+-rw-r--r--   0        0        0     1632 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/present/out.py
+-rw-r--r--   0        0        0      987 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/present/pager.py
+-rw-r--r--   0        0        0     9825 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/present/table.py
+-rw-r--r--   0        0        0     5182 2023-05-08 22:45:01.076028 arc_cli-8.5.0/arc/present/wrap.py
+-rw-r--r--   0        0        0      288 2023-05-04 03:31:42.945314 arc_cli-8.5.0/arc/prompt/__init__.py
+-rw-r--r--   0        0        0     3731 2023-05-10 04:25:05.907299 arc_cli-8.5.0/arc/prompt/helpers.py
+-rw-r--r--   0        0        0     5926 2023-05-10 22:23:55.105460 arc_cli-8.5.0/arc/prompt/prompt.py
+-rw-r--r--   0        0        0      812 2023-05-08 22:45:01.079361 arc_cli-8.5.0/arc/prompt/prompts.py
+-rw-r--r--   0        0        0     7111 2023-05-22 01:33:53.734884 arc_cli-8.5.0/arc/prompt/questions.py
+-rw-r--r--   0        0        0        0 2023-05-04 03:31:42.948647 arc_cli-8.5.0/arc/py.typed
+-rw-r--r--   0        0        0      304 2023-05-08 22:45:01.079361 arc_cli-8.5.0/arc/runtime/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-10 22:34:20.111031 arc_cli-8.5.0/arc/runtime/app.py
+-rw-r--r--   0        0        0     2786 2023-05-10 22:23:55.105460 arc_cli-8.5.0/arc/runtime/context.py
+-rw-r--r--   0        0        0    12733 2023-05-22 02:24:16.465843 arc_cli-8.5.0/arc/runtime/exec.py
+-rw-r--r--   0        0        0    10026 2023-05-10 22:34:20.111031 arc_cli-8.5.0/arc/runtime/init.py
+-rw-r--r--   0        0        0     7484 2023-05-24 23:43:58.232827 arc_cli-8.5.0/arc/runtime/middleware.py
+-rw-r--r--   0        0        0     3097 2023-05-08 22:45:01.079361 arc_cli-8.5.0/arc/runtime/plugin.py
+-rw-r--r--   0        0        0      382 2023-05-08 22:45:01.079361 arc_cli-8.5.0/arc/safe.py
+-rw-r--r--   0        0        0     1866 2023-05-08 22:45:01.079361 arc_cli-8.5.0/arc/suggest.py
+-rw-r--r--   0        0        0      383 2023-05-25 00:49:10.328292 arc_cli-8.5.0/arc/types/__init__.py
+-rw-r--r--   0        0        0    15634 2023-05-25 00:49:10.328292 arc_cli-8.5.0/arc/types/aliases.py
+-rw-r--r--   0        0        0      670 2023-05-10 22:23:55.105460 arc_cli-8.5.0/arc/types/convert.py
+-rw-r--r--   0        0        0      522 2023-05-25 00:49:10.328292 arc_cli-8.5.0/arc/types/dates.py
+-rw-r--r--   0        0        0      545 2023-05-08 22:45:01.082694 arc_cli-8.5.0/arc/types/default.py
+-rw-r--r--   0        0        0     4419 2023-05-10 03:51:44.284628 arc_cli-8.5.0/arc/types/file.py
+-rw-r--r--   0        0        0       79 2023-05-04 03:31:42.951981 arc_cli-8.5.0/arc/types/middleware/__init__.py
+-rw-r--r--   0        0        0     1397 2023-05-10 03:41:31.066410 arc_cli-8.5.0/arc/types/middleware/observers.py
+-rw-r--r--   0        0        0     2630 2023-05-08 22:45:01.082694 arc_cli-8.5.0/arc/types/middleware/transformers.py
+-rw-r--r--   0        0        0     4236 2023-05-10 02:44:59.447809 arc_cli-8.5.0/arc/types/middleware/validators.py
+-rw-r--r--   0        0        0     3486 2023-05-08 22:45:01.082694 arc_cli-8.5.0/arc/types/network.py
+-rw-r--r--   0        0        0      854 2023-05-04 03:31:42.951981 arc_cli-8.5.0/arc/types/numbers.py
+-rw-r--r--   0        0        0      860 2023-05-08 22:45:01.082694 arc_cli-8.5.0/arc/types/path.py
+-rw-r--r--   0        0        0     6881 2023-05-08 22:45:01.082694 arc_cli-8.5.0/arc/types/semver.py
+-rw-r--r--   0        0        0      877 2023-05-08 22:45:01.082694 arc_cli-8.5.0/arc/types/state.py
+-rw-r--r--   0        0        0     1960 2023-05-10 02:48:47.609034 arc_cli-8.5.0/arc/types/strings.py
+-rw-r--r--   0        0        0     2300 2023-05-10 03:16:28.712436 arc_cli-8.5.0/arc/types/type_arg.py
+-rw-r--r--   0        0        0     2718 2023-05-08 22:45:01.082694 arc_cli-8.5.0/arc/types/type_info.py
+-rw-r--r--   0        0        0     3176 2023-05-08 22:45:01.082694 arc_cli-8.5.0/arc/types/users.py
+-rw-r--r--   0        0        0     2257 2023-05-10 22:23:55.105460 arc_cli-8.5.0/arc/typing.py
+-rw-r--r--   0        0        0     1036 2023-05-25 00:49:20.191536 arc_cli-8.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 arc_cli-8.5.0/setup.py
+-rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 arc_cli-8.5.0/PKG-INFO
```

### Comparing `arc_cli-8.4.2/LICENSE` & `arc_cli-8.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/README.md` & `arc_cli-8.5.0/README.md`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/__init__.py` & `arc_cli-8.5.0/arc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "8.4.2"
+__version__ = "8.5.0"
 
 from arc import types, prompt, present, errors
 from arc.config import (
     ColorConfig,
     Config,
     LinksConfig,
     SuggestionConfig,
```

### Comparing `arc_cli-8.4.2/arc/api.py` & `arc_cli-8.5.0/arc/api.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/autocompletions.py` & `arc_cli-8.5.0/arc/autocompletions.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/config.py` & `arc_cli-8.5.0/arc/config.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/define/alias.py` & `arc_cli-8.5.0/arc/define/alias.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/define/classful.py` & `arc_cli-8.5.0/arc/define/classful.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/define/command.py` & `arc_cli-8.5.0/arc/define/command.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/define/documentation.py` & `arc_cli-8.5.0/arc/define/documentation.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/define/param/constructors.py` & `arc_cli-8.5.0/arc/define/param/constructors.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/define/param/groups.py` & `arc_cli-8.5.0/arc/define/param/groups.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/define/param/param.py` & `arc_cli-8.5.0/arc/define/param/param.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/define/param/param_definition.py` & `arc_cli-8.5.0/arc/define/param/param_definition.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/define/param/param_mixin.py` & `arc_cli-8.5.0/arc/define/param/param_mixin.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/define/param/param_tree.py` & `arc_cli-8.5.0/arc/define/param/param_tree.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/errors.py` & `arc_cli-8.5.0/arc/errors.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/logging.py` & `arc_cli-8.5.0/arc/logging.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/parser.py` & `arc_cli-8.5.0/arc/parser.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/present/ansi.py` & `arc_cli-8.5.0/arc/present/ansi.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/present/box.py` & `arc_cli-8.5.0/arc/present/box.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/present/console.py` & `arc_cli-8.5.0/arc/present/console.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/present/drawing.py` & `arc_cli-8.5.0/arc/present/drawing.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/present/formatters.py` & `arc_cli-8.5.0/arc/present/formatters.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/present/help_formatter.py` & `arc_cli-8.5.0/arc/present/help_formatter.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/present/joiner.py` & `arc_cli-8.5.0/arc/present/joiner.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/present/markdown/markdown_parser.py` & `arc_cli-8.5.0/arc/present/markdown/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/present/markdown/nodes.py` & `arc_cli-8.5.0/arc/present/markdown/nodes.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/present/out.py` & `arc_cli-8.5.0/arc/present/out.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/present/pager.py` & `arc_cli-8.5.0/arc/present/pager.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/present/table.py` & `arc_cli-8.5.0/arc/present/table.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/present/wrap.py` & `arc_cli-8.5.0/arc/present/wrap.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/prompt/helpers.py` & `arc_cli-8.5.0/arc/prompt/helpers.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/prompt/prompt.py` & `arc_cli-8.5.0/arc/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/prompt/prompts.py` & `arc_cli-8.5.0/arc/prompt/prompts.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/prompt/questions.py` & `arc_cli-8.5.0/arc/prompt/questions.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/runtime/app.py` & `arc_cli-8.5.0/arc/runtime/app.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/runtime/context.py` & `arc_cli-8.5.0/arc/runtime/context.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/runtime/exec.py` & `arc_cli-8.5.0/arc/runtime/exec.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/runtime/init.py` & `arc_cli-8.5.0/arc/runtime/init.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/runtime/middleware.py` & `arc_cli-8.5.0/arc/runtime/middleware.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/runtime/plugin.py` & `arc_cli-8.5.0/arc/runtime/plugin.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/suggest.py` & `arc_cli-8.5.0/arc/suggest.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/types/aliases.py` & `arc_cli-8.5.0/arc/types/aliases.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Module for all Alias types. Alias types are types that handle to conversion for other types.
 All builtin types (int, str, float, etc...) have a corresponding Alias type.
 """
 from __future__ import annotations
 
 import collections
+import datetime
 import enum
 import ipaddress
 import pathlib
 import re
 import types
 import typing as t
 import uuid
@@ -16,15 +17,17 @@
 
 from arc import api, autocompletions, errors, safe
 from arc.autocompletions import Completion, CompletionInfo, CompletionType
 from arc.color import colorize, fg
 from arc.present.joiner import Join
 from arc.prompt.prompts import select_prompt
 from arc.types.convert import convert_type
+from arc.types.dates import DateArgs, DateTimeArgs, TimeArgs
 from arc.types.type_arg import TypeArg
+from arc.types.default import unwrap
 from arc.typing import Annotation, TypeProtocol
 
 if t.TYPE_CHECKING:
     from arc.define.param import Param
     from arc.runtime import Context
     from arc.types.type_info import TypeInfo
 
@@ -430,12 +433,47 @@
         if len(info.annotations) == 0:
             return 0
         return info.annotations[0]
 
 
 class UUIDAlias(Alias, of=uuid.UUID):
     @classmethod
-    def convert(cls, value: str, info: TypeInfo[t.Any]) -> uuid.UUID:
+    def convert(cls, value: str, info: TypeInfo[uuid.UUID]) -> uuid.UUID:
         try:
             return uuid.UUID(value)
         except ValueError as e:
             raise errors.ConversionError(value, "Not a valid UUID", e) from e
+
+
+class DateTimeAlias(Alias, of=datetime.datetime):
+    @classmethod
+    def convert(
+        cls, value: str, info: TypeInfo[datetime.datetime]
+    ) -> datetime.datetime:
+        type_arg: DateTimeArgs = t.cast(DateTimeArgs, info.type_arg) or DateTimeArgs()
+
+        try:
+            return datetime.datetime.strptime(value, unwrap(type_arg.format))
+        except ValueError as e:
+            raise errors.ConversionError(value, "Not a valid datetime", e) from e
+
+
+class DateAlias(Alias, of=datetime.date):
+    @classmethod
+    def convert(cls, value: str, info: TypeInfo[datetime.date]) -> datetime.date:
+        type_arg: DateArgs = t.cast(DateArgs, info.type_arg) or DateArgs()
+
+        try:
+            return datetime.datetime.strptime(value, unwrap(type_arg.format)).date()
+        except ValueError as e:
+            raise errors.ConversionError(value, "Not a valid date", e) from e
+
+
+class TimeAlias(Alias, of=datetime.time):
+    @classmethod
+    def convert(cls, value: str, info: TypeInfo[datetime.time]) -> datetime.time:
+        type_arg: TimeArgs = t.cast(TimeArgs, info.type_arg) or TimeArgs()
+
+        try:
+            return datetime.datetime.strptime(value, unwrap(type_arg.format)).time()
+        except ValueError as e:
+            raise errors.ConversionError(value, "Not a valid time", e) from e
```

### Comparing `arc_cli-8.4.2/arc/types/convert.py` & `arc_cli-8.5.0/arc/types/convert.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/types/default.py` & `arc_cli-8.5.0/arc/types/default.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/types/file.py` & `arc_cli-8.5.0/arc/types/file.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/types/middleware/observers.py` & `arc_cli-8.5.0/arc/types/middleware/observers.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/types/middleware/transformers.py` & `arc_cli-8.5.0/arc/types/middleware/transformers.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/types/middleware/validators.py` & `arc_cli-8.5.0/arc/types/middleware/validators.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/types/network.py` & `arc_cli-8.5.0/arc/types/network.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/types/numbers.py` & `arc_cli-8.5.0/arc/types/numbers.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/types/path.py` & `arc_cli-8.5.0/arc/types/path.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/types/semver.py` & `arc_cli-8.5.0/arc/types/semver.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/types/state.py` & `arc_cli-8.5.0/arc/types/state.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/types/strings.py` & `arc_cli-8.5.0/arc/types/strings.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/types/type_arg.py` & `arc_cli-8.5.0/arc/types/type_arg.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/types/type_info.py` & `arc_cli-8.5.0/arc/types/type_info.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/types/users.py` & `arc_cli-8.5.0/arc/types/users.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/arc/typing.py` & `arc_cli-8.5.0/arc/typing.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.4.2/pyproject.toml` & `arc_cli-8.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arc-cli"
-version = "8.4.2"
+version = "8.5.0"
 description = "Package for creating CLI's with ease."
 authors = ["Sean Collings <me@seancollings.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/seanrcollings/arc"
 documentation = "https://arc.seancollings.dev"
 classifiers= [
```

### Comparing `arc_cli-8.4.2/setup.py` & `arc_cli-8.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'arc.types.middleware']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'arc-cli',
-    'version': '8.4.2',
+    'version': '8.5.0',
     'description': "Package for creating CLI's with ease.",
     'long_description': '# ARC: A Regular CLI\nA tool for building declarative, and highly extendable CLI systems for Python 3.10+\n\n# ARC Features\n- Command line arguments based on python type hints\n- Arbitrary command nesting\n- Automatic `--help` documentation\n- Fully Extensible with custom middlewares,  types, validators, parameter configurations, etc...\n\n# Links\n- [Docs](https://arc.seancollings.dev)\n- [Playground](https://playground.arc.seancollings.dev)\n- [PyPi](https://pypi.org/project/arc-cli/)\n\n\n# Quick Start\n\n```py\nimport arc\n\n@arc.command\ndef hello(name: str):\n    """My first arc program!"""\n    arc.print(f"Hello {name}!")\n\nhello()\n```\n\n```\n$ python hello.py Sean\nHello, Sean!\n```\n\n```\n$ python hello.py --help\nUSAGE\n    hello.py [-h] [--] name\n\nDESCRIPTION\n    My first arc program!\n\nARGUMENTS\n    name\n\nOPTIONS\n    --help (-h)  Displays this help message\n```\n\n# Installation\n\n```\n$ pip install arc-cli\n```\n\nClone for development\n```\n$ git clone https://github.com/seanrcollings/arc\n$ poetry install\n```\n\n# Tests\nTests are written with `pytest`\n```\n$ pytest\n```\n',
     'author': 'Sean Collings',
     'author_email': 'me@seancollings.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/seanrcollings/arc',
```

### Comparing `arc_cli-8.4.2/PKG-INFO` & `arc_cli-8.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arc-cli
-Version: 8.4.2
+Version: 8.5.0
 Summary: Package for creating CLI's with ease.
 Home-page: https://github.com/seanrcollings/arc
 License: MIT
 Author: Sean Collings
 Author-email: me@seancollings.dev
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
```

