# Comparing `tmp/arclet-alconna-1.7.6.tar.gz` & `tmp/arclet-alconna-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-1.7.6.tar", last modified: Sat May 20 12:06:18 2023, max compression
+gzip compressed data, was "arclet-alconna-1.7.7.tar", last modified: Thu May 25 17:54:03 2023, max compression
```

## Comparing `arclet-alconna-1.7.6.tar` & `arclet-alconna-1.7.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.6/LICENSE
--rw-r--r--   0        0        0     2810 2023-05-11 05:55:21.918053 arclet-alconna-1.7.6/pyproject.toml
--rw-r--r--   0        0        0     6702 2023-05-11 05:55:23.383958 arclet-alconna-1.7.6/README-EN.md
--rw-r--r--   0        0        0     1084 2023-05-20 11:27:26.756981 arclet-alconna-1.7.6/src/arclet/alconna/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 05:53:44.746150 arclet-alconna-1.7.6/src/arclet/alconna/_internal/__init__.py
--rw-r--r--   0        0        0    17897 2023-05-20 11:20:33.572115 arclet-alconna-1.7.6/src/arclet/alconna/_internal/_analyser.py
--rw-r--r--   0        0        0     8476 2023-05-11 05:53:44.748144 arclet-alconna-1.7.6/src/arclet/alconna/_internal/_argv.py
--rw-r--r--   0        0        0    23361 2023-05-19 14:58:51.599030 arclet-alconna-1.7.6/src/arclet/alconna/_internal/_handlers.py
--rw-r--r--   0        0        0     9971 2023-05-19 14:58:51.600030 arclet-alconna-1.7.6/src/arclet/alconna/_internal/_header.py
--rw-r--r--   0        0        0      837 2023-05-11 05:53:44.749146 arclet-alconna-1.7.6/src/arclet/alconna/_internal/_util.py
--rw-r--r--   0        0        0     1543 2023-05-11 05:54:34.441719 arclet-alconna-1.7.6/src/arclet/alconna/action.py
--rw-r--r--   0        0        0    14429 2023-05-11 05:55:00.317381 arclet-alconna-1.7.6/src/arclet/alconna/args.py
--rw-r--r--   0        0        0     1499 2023-05-11 05:53:44.752371 arclet-alconna-1.7.6/src/arclet/alconna/argv.py
--rw-r--r--   0        0        0    15660 2023-05-11 05:55:01.638197 arclet-alconna-1.7.6/src/arclet/alconna/arparma.py
--rw-r--r--   0        0        0    13248 2023-05-11 05:55:02.886909 arclet-alconna-1.7.6/src/arclet/alconna/base.py
--rw-r--r--   0        0        0     1889 2023-05-11 05:55:04.954858 arclet-alconna-1.7.6/src/arclet/alconna/builtin.py
--rw-r--r--   0        0        0     4867 2023-05-11 05:53:44.757144 arclet-alconna-1.7.6/src/arclet/alconna/completion.py
--rw-r--r--   0        0        0     4465 2023-05-11 05:55:07.597153 arclet-alconna-1.7.6/src/arclet/alconna/config.py
--rw-r--r--   0        0        0    14061 2023-05-19 14:58:51.601035 arclet-alconna-1.7.6/src/arclet/alconna/core.py
--rw-r--r--   0        0        0     2617 2023-05-11 05:55:14.716787 arclet-alconna-1.7.6/src/arclet/alconna/duplication.py
--rw-r--r--   0        0        0     1009 2023-05-11 05:55:16.833416 arclet-alconna-1.7.6/src/arclet/alconna/exceptions.py
--rw-r--r--   0        0        0    11287 2023-05-11 05:55:17.442184 arclet-alconna-1.7.6/src/arclet/alconna/formatter.py
--rw-r--r--   0        0        0       99 2023-05-11 05:53:44.763145 arclet-alconna-1.7.6/src/arclet/alconna/i18n/.config.json
--rw-r--r--   0        0        0     3638 2023-05-19 14:58:51.602031 arclet-alconna-1.7.6/src/arclet/alconna/i18n/en-US.json
--rw-r--r--   0        0        0     3687 2023-05-19 14:58:51.603034 arclet-alconna-1.7.6/src/arclet/alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0    17034 2023-05-20 11:18:12.523446 arclet-alconna-1.7.6/src/arclet/alconna/manager.py
--rw-r--r--   0        0        0     1484 2023-05-11 05:55:18.667097 arclet-alconna-1.7.6/src/arclet/alconna/model.py
--rw-r--r--   0        0        0     1943 2023-05-11 05:55:19.651541 arclet-alconna-1.7.6/src/arclet/alconna/model.pyi
--rw-r--r--   0        0        0     3940 2023-05-11 05:55:20.308191 arclet-alconna-1.7.6/src/arclet/alconna/output.py
--rw-r--r--   0        0        0        0 2023-05-11 05:53:44.769149 arclet-alconna-1.7.6/src/arclet/alconna/py.typed
--rw-r--r--   0        0        0     5815 2023-05-11 05:55:25.933152 arclet-alconna-1.7.6/src/arclet/alconna/stub.py
--rw-r--r--   0        0        0     3586 2023-05-11 05:55:26.563876 arclet-alconna-1.7.6/src/arclet/alconna/typing.py
--rw-r--r--   0        0        0     3246 2023-05-11 05:53:44.772143 arclet-alconna-1.7.6/tests/analyser_test.py
--rw-r--r--   0        0        0     7583 2023-05-11 05:53:44.773143 arclet-alconna-1.7.6/tests/args_test.py
--rw-r--r--   0        0        0     2167 2023-05-11 05:55:03.459296 arclet-alconna-1.7.6/tests/base_test.py
--rw-r--r--   0        0        0     3113 2023-05-11 05:53:44.774144 arclet-alconna-1.7.6/tests/components_test.py
--rw-r--r--   0        0        0     1199 2023-05-11 05:53:44.774144 arclet-alconna-1.7.6/tests/config_test.py
--rw-r--r--   0        0        0    23993 2023-05-20 11:16:57.405551 arclet-alconna-1.7.6/tests/core_test.py
--rw-r--r--   0        0        0      505 2023-05-11 05:53:44.775105 arclet-alconna-1.7.6/tests/util_test.py
--rw-r--r--   0        0        0     7363 1970-01-01 00:00:00.000000 arclet-alconna-1.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.7/LICENSE
+-rw-r--r--   0        0        0     2810 2023-05-25 16:57:28.459958 arclet-alconna-1.7.7/pyproject.toml
+-rw-r--r--   0        0        0     6702 2023-05-25 16:37:15.089363 arclet-alconna-1.7.7/README-EN.md
+-rw-r--r--   0        0        0     1084 2023-05-25 16:37:15.105359 arclet-alconna-1.7.7/src/arclet/alconna/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:37:15.106361 arclet-alconna-1.7.7/src/arclet/alconna/_internal/__init__.py
+-rw-r--r--   0        0        0    17705 2023-05-25 17:31:34.682918 arclet-alconna-1.7.7/src/arclet/alconna/_internal/_analyser.py
+-rw-r--r--   0        0        0     8476 2023-05-25 16:37:15.107359 arclet-alconna-1.7.7/src/arclet/alconna/_internal/_argv.py
+-rw-r--r--   0        0        0    23280 2023-05-25 17:07:20.959020 arclet-alconna-1.7.7/src/arclet/alconna/_internal/_handlers.py
+-rw-r--r--   0        0        0    10053 2023-05-25 17:28:18.129401 arclet-alconna-1.7.7/src/arclet/alconna/_internal/_header.py
+-rw-r--r--   0        0        0     1333 2023-05-25 17:53:21.656271 arclet-alconna-1.7.7/src/arclet/alconna/_internal/_util.py
+-rw-r--r--   0        0        0     1543 2023-05-25 16:37:15.110384 arclet-alconna-1.7.7/src/arclet/alconna/action.py
+-rw-r--r--   0        0        0    14323 2023-05-25 17:43:52.094619 arclet-alconna-1.7.7/src/arclet/alconna/args.py
+-rw-r--r--   0        0        0     1499 2023-05-25 16:37:15.112359 arclet-alconna-1.7.7/src/arclet/alconna/argv.py
+-rw-r--r--   0        0        0    15488 2023-05-25 17:37:16.116622 arclet-alconna-1.7.7/src/arclet/alconna/arparma.py
+-rw-r--r--   0        0        0    13248 2023-05-25 16:37:15.114361 arclet-alconna-1.7.7/src/arclet/alconna/base.py
+-rw-r--r--   0        0        0     2715 2023-05-25 17:37:16.076621 arclet-alconna-1.7.7/src/arclet/alconna/builtin.py
+-rw-r--r--   0        0        0     4867 2023-05-25 16:37:15.116360 arclet-alconna-1.7.7/src/arclet/alconna/completion.py
+-rw-r--r--   0        0        0     4465 2023-05-25 16:37:15.117360 arclet-alconna-1.7.7/src/arclet/alconna/config.py
+-rw-r--r--   0        0        0    14061 2023-05-25 16:37:15.117360 arclet-alconna-1.7.7/src/arclet/alconna/core.py
+-rw-r--r--   0        0        0     2014 2023-05-25 17:41:01.475077 arclet-alconna-1.7.7/src/arclet/alconna/duplication.py
+-rw-r--r--   0        0        0     1009 2023-05-25 16:37:15.119359 arclet-alconna-1.7.7/src/arclet/alconna/exceptions.py
+-rw-r--r--   0        0        0    11287 2023-05-25 16:37:15.120361 arclet-alconna-1.7.7/src/arclet/alconna/formatter.py
+-rw-r--r--   0        0        0       99 2023-05-21 05:43:33.502836 arclet-alconna-1.7.7/src/arclet/alconna/i18n/.config.json
+-rw-r--r--   0        0        0     3638 2023-05-21 05:43:33.503837 arclet-alconna-1.7.7/src/arclet/alconna/i18n/en-US.json
+-rw-r--r--   0        0        0     3687 2023-05-21 05:43:33.504836 arclet-alconna-1.7.7/src/arclet/alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0    17039 2023-05-25 17:37:16.096623 arclet-alconna-1.7.7/src/arclet/alconna/manager.py
+-rw-r--r--   0        0        0     1484 2023-05-25 16:37:15.122358 arclet-alconna-1.7.7/src/arclet/alconna/model.py
+-rw-r--r--   0        0        0     1943 2023-05-25 16:37:15.123407 arclet-alconna-1.7.7/src/arclet/alconna/model.pyi
+-rw-r--r--   0        0        0     3940 2023-05-25 16:37:15.124599 arclet-alconna-1.7.7/src/arclet/alconna/output.py
+-rw-r--r--   0        0        0        0 2023-05-21 05:43:33.513926 arclet-alconna-1.7.7/src/arclet/alconna/py.typed
+-rw-r--r--   0        0        0     5815 2023-05-25 16:37:15.125359 arclet-alconna-1.7.7/src/arclet/alconna/stub.py
+-rw-r--r--   0        0        0     3586 2023-05-25 16:37:15.125704 arclet-alconna-1.7.7/src/arclet/alconna/typing.py
+-rw-r--r--   0        0        0     3246 2023-05-25 16:37:15.127191 arclet-alconna-1.7.7/tests/analyser_test.py
+-rw-r--r--   0        0        0     7583 2023-05-25 16:37:15.127710 arclet-alconna-1.7.7/tests/args_test.py
+-rw-r--r--   0        0        0     2167 2023-05-25 16:37:15.128711 arclet-alconna-1.7.7/tests/base_test.py
+-rw-r--r--   0        0        0     3119 2023-05-25 17:37:16.085622 arclet-alconna-1.7.7/tests/components_test.py
+-rw-r--r--   0        0        0     1199 2023-05-25 16:37:15.130711 arclet-alconna-1.7.7/tests/config_test.py
+-rw-r--r--   0        0        0    24318 2023-05-25 17:21:11.641086 arclet-alconna-1.7.7/tests/core_test.py
+-rw-r--r--   0        0        0      505 2023-05-25 16:37:15.132710 arclet-alconna-1.7.7/tests/util_test.py
+-rw-r--r--   0        0        0     7363 1970-01-01 00:00:00.000000 arclet-alconna-1.7.7/PKG-INFO
```

### Comparing `arclet-alconna-1.7.6/LICENSE` & `arclet-alconna-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/pyproject.toml` & `arclet-alconna-1.7.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 name = "arclet-alconna"
 description = "A High-performance, Generality, Humane Command Line Arguments Parser Library."
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "typing-extensions>=4.5.0",
-    "nepattern<0.6.0, >=0.5.6",
+    "nepattern<0.6.0, >=0.5.8",
     "tarina>=0.3.3",
 ]
 dynamic = []
 requires-python = ">=3.8"
 readme = "README-EN.md"
 keywords = [
     "command",
@@ -34,15 +34,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
-version = "1.7.6"
+version = "1.7.7"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 documentation = "https://arcletproject.github.io/docs/alconna/tutorial"
 repository = "https://github.com/ArcletProject/Alconna"
```

### Comparing `arclet-alconna-1.7.6/README-EN.md` & `arclet-alconna-1.7.7/README-EN.md`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/__init__.py` & `arclet-alconna-1.7.7/src/arclet/alconna/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 from .builtin import set_default
 from .model import OptionResult, SubcommandResult, HeadResult
 from .output import output_manager
 from .formatter import TextFormatter
 from .duplication import Duplication
 from .stub import ArgsStub, OptionStub, SubcommandStub
 
-__version__ = "1.7.6"
+__version__ = "1.7.7"
 
 # backward compatibility
 Arpamar = Arparma
 DataCollectionContainer = Argv
```

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/_internal/_analyser.py` & `arclet-alconna-1.7.7/src/arclet/alconna/_internal/_analyser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 from __future__ import annotations
 
 import re
-import traceback
 from dataclasses import dataclass, field
 from re import Match
 from typing import TYPE_CHECKING, Any, Callable, Generic, Set
 
 from tarina import lang
 from typing_extensions import Self, TypeAlias
 
 from ..action import Action
 from ..args import Args
 from ..arparma import Arparma
 from ..base import Option, Subcommand
 from ..completion import comp_ctx
-from ..config import Namespace, config
+from ..config import config
 from ..exceptions import (
     ArgumentMissing, FuzzyMatchSuccess, ParamsUnmatched, PauseTriggered, SpecialOptionTriggered
 )
 from ..manager import ShortcutArgs, command_manager
 from ..model import HeadResult, OptionResult, Sentence, SubcommandResult
 from ..output import output_manager
 from ..typing import TDC
 from ._handlers import (
     analyse_args, analyse_header, analyse_param,
     handle_completion, handle_help, handle_opt_default,
     handle_shortcut, prompt
 )
 from ._header import Header
-from ._util import levenshtein
+from ._util import levenshtein, escape, unescape
 
 if TYPE_CHECKING:
     from ..core import Alconna
     from ._argv import Argv
 
 _SPECIAL = {
     "help": handle_help,
@@ -60,51 +59,47 @@
                 continue
             else:
                 data[alias] = sorted([li, option], key=lambda x: x.priority, reverse=True)
         else:
             data[alias] = option
 
 
-def default_compiler(analyser: SubAnalyser, _config: Namespace, pids: set[str]):
+def default_compiler(analyser: SubAnalyser, pids: set[str]):
     """默认的编译方法
 
     Args:
         analyser (SubAnalyser): 任意子解析器
-        _config (Namespace): 命名空间配置
         pids (set[str]): 节点名集合
     """
-    require_len = 0
     for opts in analyser.command.options:
         if isinstance(opts, Option):
             if opts.compact or opts.action.type == 2 or not set(analyser.command.separators).issuperset(opts.separators):
                 analyser.compact_params.append(opts)
             _compile_opts(opts, analyser.compile_params)  # type: ignore
             if opts.default:
                 analyser.default_opt_result[opts.dest] = (opts.default, opts.action)
             pids.update(opts.aliases)
         elif isinstance(opts, Subcommand):
             sub = SubAnalyser(opts)
             analyser.compile_params[opts.name] = sub
             pids.add(opts.name)
-            default_compiler(sub, _config, pids)
+            default_compiler(sub, pids)
             if not set(analyser.command.separators).issuperset(opts.separators):
                 analyser.compact_params.append(sub)
             if sub.command.default:
                 analyser.default_sub_result[opts.dest] = sub.command.default
         if opts.requires:
             pids.update(opts.requires)
-            require_len = max(len(opts.requires), require_len)
             for k in opts.requires:
                 analyser.compile_params.setdefault(k, Sentence(name=k))
 
 
 @dataclass
 class SubAnalyser(Generic[TDC]):
     """子解析器, 用于子命令的解析"""
-
     command: Subcommand
     """子命令"""
     default_main_only: bool = field(default=False)
     """命令是否只有主参数"""
     need_main_args: bool = field(default=False)
     """是否需要主参数"""
     compile_params: dict[str, Sentence | Option | list[Option] | SubAnalyser[TDC]] = field(default_factory=dict)
@@ -251,15 +246,14 @@
         super().__init__(alconna)
         self.fuzzy_match = alconna.meta.fuzzy_match
         self.used_tokens = set()
         self.command_header = Header.generate(alconna.command, alconna.prefixes, alconna.meta.compact)
         compiler = compiler or default_compiler
         compiler(
             self,
-            alconna.namespace_config,
             command_manager.resolve(self.command).param_ids
         )
 
     def _clr(self):
         self.used_tokens.clear()
         super()._clr()
 
@@ -294,38 +288,40 @@
             return self.export(argv, True, exc)
         data_index = 0
         for i, unit in enumerate(argv.raw_data):
             if not data:
                 break
             if not isinstance(unit, str):
                 continue
+            unit = escape(unit)
             if unit == f"{{%{data_index}}}":
                 argv.raw_data[i] = data.pop(0)
                 data_index += 1
             elif f"{{%{data_index}}}" in unit:
-                argv.raw_data[i] = unit.replace(f"{{%{data_index}}}", str(data.pop(0)))
+                argv.raw_data[i] = unescape(unit.replace(f"{{%{data_index}}}", str(data.pop(0))))
                 data_index += 1
             elif mat := re.search(r"\{\*(.*)\}", unit, re.DOTALL):
                 sep = mat[1]
-                argv.raw_data[i] = unit.replace(f"{{*{sep}}}", (sep or ' ').join(map(str, data)))
+                argv.raw_data[i] = unescape(unit.replace(f"{{*{sep}}}", (sep or ' ').join(map(str, data))))
                 data.clear()
 
         argv.bak_data = argv.raw_data.copy()
         argv.addon(data).addon(short.get('args', []))
         if reg:
             groups: tuple[str, ...] = reg.groups()
             gdict: dict[str, str] = reg.groupdict()
             for j, unit in enumerate(argv.raw_data):
                 if not isinstance(unit, str):
                     continue
+                unit = escape(unit)
                 for i, c in enumerate(groups):
                     unit = unit.replace(f"{{{i}}}", c)
                 for k, v in gdict.items():
                     unit = unit.replace(f"{{{k}}}", v)
-                argv.raw_data[j] = unit
+                argv.raw_data[j] = unescape(unit)
         if argv.message_cache:
             argv.token = argv.generate_token(argv.raw_data)
         return self.process(argv)
 
     def process(self, argv: Argv[TDC]) -> Arparma[TDC]:
         """主体解析函数, 应针对各种情况进行解析
 
@@ -420,29 +416,26 @@
                 raise
             return self.export(argv, True, e1)
 
         if self.default_main_only and not self.args_result:
             self.args_result = analyse_args(argv, self.self_args)
 
     def export(
-        self,
-        argv: Argv[TDC],
-        fail: bool = False,
-        exception: BaseException | None = None,
+        self, argv: Argv[TDC], fail: bool = False, exception: BaseException | None = None,
     ) -> Arparma[TDC]:
         """创建 `Arparma` 解析结果, 其一定是一次解析的最后部分
 
         Args:
             argv (Argv[TDC]): 命令行参数
             fail (bool, optional): 是否解析失败. Defaults to False.
             exception (BaseException | None, optional): 解析失败时的异常. Defaults to None.
         """
         result = Arparma(self.command.path, argv.origin, not fail, self.header_result)
         if fail:
-            result.error_info = exception or repr(traceback.format_exc(limit=1))
+            result.error_info = exception
             result.error_data = argv.release()
         else:
             if self.default_opt_result:
                 handle_opt_default(self.default_opt_result, self.options_result)
             if self.default_sub_result:
                 for k, v in self.default_sub_result.items():
                     if k not in self.subcommands_result:
@@ -454,8 +447,8 @@
             if argv.message_cache:
                 command_manager.record(argv.token, result)
                 self.used_tokens.add(argv.token)
         self.reset()
         return result  # type: ignore
 
 
-TCompile: TypeAlias = Callable[[SubAnalyser, Namespace, Set[str]], None]
+TCompile: TypeAlias = Callable[[SubAnalyser, Set[str]], None]
```

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/_internal/_argv.py` & `arclet-alconna-1.7.7/src/arclet/alconna/_internal/_argv.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/_internal/_handlers.py` & `arclet-alconna-1.7.7/src/arclet/alconna/_internal/_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,21 +71,15 @@
             raise ParamsUnmatched(*res.error.args)
         result_dict[_kwarg[1]] = res._value  # type: ignore
         return
     argv.rollback(may_arg)
     raise ParamsUnmatched(lang.require("args", "key_missing").format(target=may_arg, key=key))
 
 
-def _loop_kw(
-    argv: Argv,
-    _loop: int,
-    seps: tuple[str, ...],
-    value: MultiVar,
-    default: Any
-):
+def _loop_kw(argv: Argv, _loop: int, seps: tuple[str, ...], value: MultiVar, default: Any):
     """循环关键字参数"""
     result = {}
     for _ in range(_loop):
         _m_arg, _m_str = argv.next(seps)
         if not _m_arg:
             continue
         if _m_str and _m_arg in argv.param_ids:
@@ -99,20 +93,15 @@
         if value.flag == '+':
             raise ParamsUnmatched
         result = [default] if default else []
     return result
 
 
 def _loop(
-    argv: Argv,
-    _loop: int,
-    seps: tuple[str, ...],
-    value: MultiVar,
-    default: Any,
-    kw: KeyWordVar | None
+    argv: Argv, _loop: int, seps: tuple[str, ...], value: MultiVar, default: Any, kw: KeyWordVar | None
 ):
     """循环参数"""
     result = []
     for _ in range(_loop):
         _m_arg, _m_str = argv.next(seps)
         if not _m_arg:
             continue
@@ -129,20 +118,15 @@
     if not result:
         if value.flag == '+':
             raise ParamsUnmatched
         result = [default] if default else []
     return tuple(result)
 
 
-def multi_arg_handler(
-    argv: Argv,
-    args: Args,
-    arg: Arg,
-    result_dict: dict[str, Any],
-):
+def multi_arg_handler(argv: Argv, args: Args, arg: Arg, result_dict: dict[str, Any],):
     """处理可变参数
 
     Args:
         argv (Argv): 命令行参数
         args (Args): 参数集合
         arg (Arg): 参数单元
         result_dict (dict[str, Any]): 结果字典
@@ -218,20 +202,18 @@
                 result, default_val, arg.optional, key, argv.fuzzy_match  # type: ignore
             )
         elif value == AllParam:
             argv.rollback(may_arg)
             result[key] = argv.converter(argv.release(arg.separators))
             argv.current_index = argv.ndata
             return result
-        elif value == AnyOne:
+        elif value == AnyOne or (value == STRING and _str):
             result[key] = may_arg
         elif value == AnyString:
             result[key] = str(may_arg)
-        elif value == STRING and _str:
-            result[key] = may_arg
         else:
             res = (
                 value.invalidate(may_arg, default_val)
                 if value.anti
                 else value.validate(may_arg, default_val)
             )
             if res.flag != 'valid':
@@ -290,14 +272,15 @@
         return target
     if param.action.type == 2:
         if not param.nargs:
             source.value += target.value
             return source
         return target
     if not param.nargs:
+        source.value = source.value[:]
         source.value.extend(target.value)
     else:
         for key, value in target.args.items():
             if key in source.args:
                 source.args[key].append(value)
             else:
                 source.args[key] = [value]
```

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/_internal/_header.py` & `arclet-alconna-1.7.7/src/arclet/alconna/_internal/_header.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 from inspect import isclass
 from typing import Any, Callable
 
 from nepattern import BasePattern, UnionPattern, all_patterns, type_parser
 from nepattern.util import TPattern
 from tarina import Empty, lang
 
+from ._util import escape, unescape
 from ..typing import TPrefixes
 
 
 def handle_bracket(name: str, mapping: dict):
     """处理字符串中的括号对并转为正则表达式"""
     pattern_map = all_patterns()
+    name = escape(name)
     if len(parts := re.split(r"(\{.*?})", name)) <= 1:
-        return name, False
+        return unescape(name), False
     for i, part in enumerate(parts):
         if not part:
             continue
         if part.startswith("{") and part.endswith("}"):
             res = part[1:-1].split(":")
             if not res or (len(res) > 1 and not res[1] and not res[0]):
                 parts[i] = ".+?"
@@ -31,15 +33,15 @@
                     i
                 ] = f"{pattern_map[res[1]].pattern if res[1] in pattern_map else res[1]}"
             elif res[1] in pattern_map:
                 mapping[res[0]] = pattern_map[res[1]]
                 parts[i] = f"(?P<{res[0]}>{pattern_map[res[1]].pattern})"
             else:
                 parts[i] = f"(?P<{res[0]}>{res[1]})"
-    return "".join(parts), True
+    return unescape("".join(parts)), True
 
 
 class Pair:
     """用于匹配前缀和命令的配对"""
     __slots__ = ("prefix", "pattern", "is_prefix_pat", "gd_supplier", "_match")
 
     def __init__(self, prefix: Any, pattern: TPattern | str):
```

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/action.py` & `arclet-alconna-1.7.7/src/arclet/alconna/action.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/args.py` & `arclet-alconna-1.7.7/src/arclet/alconna/args.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,17 +207,15 @@
             if param.kind == param.VAR_POSITIONAL:
                 anno = MultiVar(anno, "*")
             if param.kind == param.VAR_KEYWORD:
                 anno = MultiVar(KeyWordVar(anno), "*")
             _args.add(name, value=anno, default=de)
         return _args, method
 
-    def __init__(
-        self, *args: Arg, separators: str | Iterable[str] | None = None, **kwargs: TAValue
-    ):
+    def __init__(self, *args: Arg, separators: str | Iterable[str] | None = None, **kwargs: TAValue):
         """
         构造一个 `Args`
 
         Args:
             *args (Arg): 参数单元
             separators (str | Iterable[str] | None, optional): 可选的为所有参数单元指定分隔符
             **kwargs (TAValue): 剩余的参数单元值
@@ -295,33 +293,31 @@
             if arg.name in _visit:
                 continue
             _tmp.append(arg)
             _visit.add(arg.name)
             if arg.name in self._visit:
                 continue
             self._visit.add(arg.name)
-            _limit = False
-            if isinstance(arg.value, MultiVar) and not _limit:
+            if isinstance(arg.value, MultiVar):
                 if isinstance(arg.value.base, KeyWordVar):
                     if self.var_keyword:
                         raise InvalidParam(lang.require("args", "duplicate_kwargs"))
                     self.var_keyword = arg.value
                 elif self.var_positional:
                     raise InvalidParam(lang.require("args", "duplicate_varargs"))
                 else:
                     self.var_positional = arg.value
-                _limit = True
             if isinstance(arg.value, KeyWordVar):
                 if self.var_keyword or self.var_positional:
                     raise InvalidParam(lang.require("args", "exclude_mutable_args"))
                 self.keyword_only.append(arg.name)
                 if arg.value.sep in arg.separators:
                     _tmp.insert(-1, Arg(f"_key_{arg.name}", value=f"-*{arg.name}"))
                     _tmp[-1].value = arg.value.base
-            if ArgFlag.OPTIONAL in arg.flag:
+            if arg.optional:
                 if self.var_keyword or self.var_positional:
                     raise InvalidParam(lang.require("args", "exclude_mutable_args"))
                 self.optional_count += 1
         self.argument.clear()
         self.argument.extend(_tmp)
         del _tmp
         del _visit
```

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/argv.py` & `arclet-alconna-1.7.7/src/arclet/alconna/argv.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/arparma.py` & `arclet-alconna-1.7.7/src/arclet/alconna/arparma.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,33 +76,33 @@
 
     def __init__(
         self,
         source: str,
         origin: TDC,
         matched: bool = False,
         header_match: HeadResult | None = None,
-        error_info: type[BaseException] | BaseException | str = '',
+        error_info: type[BaseException] | BaseException | None = None,
         error_data: list[str | Any] | None = None,
         main_args: dict[str, Any] | None = None,
         options: dict[str, OptionResult] | None = None,
         subcommands: dict[str, SubcommandResult] | None = None,
     ):
         """初始化 `Arparma`
         Args:
             source (str): 命令源
             origin (TDC): 原始数据
             matched (bool, optional): 是否匹配
             header_match (HeadResult | None, optional): 命令头匹配结果
-            error_info (type[BaseException] | BaseException | str, optional): 错误信息
+            error_info (type[BaseException] | BaseException | None, optional): 错误信息
             error_data (list[str | Any] | None, optional): 错误数据
             main_args (dict[str, Any] | None, optional): 主参数匹配结果
             options (dict[str, OptionResult] | None, optional): 选项匹配结果
             subcommands (dict[str, SubcommandResult] | None, optional): 子命令匹配结果
         """
-        self._source = source
+        self.source = source
         self.origin = origin
         self.matched = matched
         self.header_match = header_match or HeadResult()
         self.error_info = error_info
         self.error_data = error_data or []
         self.main_args = main_args or {}
         self.other_args = {}
@@ -111,20 +111,14 @@
 
     def _clr(self):
         ks = list(self.__dict__.keys())
         for k in ks:
             delattr(self, k)
 
     @property
-    def source(self):
-        """返回命令源"""
-        from .manager import command_manager
-        return command_manager.get_command(self._source)
-
-    @property
     def header(self) -> dict[str, Any]:
         """返回可能解析到的命令头中的组信息"""
         return self.header_match.groups
 
     @property
     def head_matched(self):
         """返回命令头是否匹配"""
```

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/base.py` & `arclet-alconna-1.7.7/src/arclet/alconna/base.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/builtin.py` & `arclet-alconna-1.7.7/src/arclet/alconna/builtin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,36 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Any, Callable, overload
+from typing import Any, Callable, overload, cast
 
 from .arparma import Arparma, ArparmaBehavior
+from .core import Alconna
+from .duplication import Duplication
+from .stub import ArgsStub, OptionStub, SubcommandStub
 from .exceptions import BehaveCancelled
 
-__all__ = ["set_default"]
+__all__ = ["set_default", "generate_duplication"]
+
+
+def generate_duplication(alc: Alconna) -> type[Duplication]:
+    """依据给定的命令生成一个解析结果的检查类。"""
+    from .base import Option, Subcommand
+    options = filter(lambda x: isinstance(x, Option), alc.options)
+    subcommands = filter(lambda x: isinstance(x, Subcommand), alc.options)
+    return cast(type[Duplication], type(
+        f"{alc.name.strip('/.-:')}Interface",
+        (Duplication,), {
+            "__annotations__": {
+                "args": ArgsStub,
+                **{opt.dest: OptionStub for opt in options},
+                **{sub.dest: SubcommandStub for sub in subcommands},
+            }
+        }
+    ))
 
 
 class _MISSING_TYPE: pass
 MISSING = _MISSING_TYPE()
 
 
 @dataclass(init=True, eq=True, unsafe_hash=True)
```

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/completion.py` & `arclet-alconna-1.7.7/src/arclet/alconna/completion.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/config.py` & `arclet-alconna-1.7.7/src/arclet/alconna/config.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/core.py` & `arclet-alconna-1.7.7/src/arclet/alconna/core.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/duplication.py` & `arclet-alconna-1.7.7/src/arclet/alconna/duplication.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 
 class Duplication:
     """`副本`, 用以更方便的检查、调用解析结果的类。"""
     header: dict[str, str]
 
     def __init__(self, target: Arparma):
         from .base import Option, Subcommand
+        from .manager import command_manager
+        source = command_manager.get_command(target.source)
         self.header = target.header.copy()
         for key, value in self.__annotations__.items():
             if isclass(value) and issubclass(value, BaseStub):
                 if value is ArgsStub:
-                    setattr(self, key, ArgsStub(target.source.args).set_result(target.main_args))
+                    setattr(self, key, ArgsStub(source.args).set_result(target.main_args))
                 elif value is SubcommandStub:
-                    for subcommand in filter(lambda x: isinstance(x, Subcommand), target.source.options):
+                    for subcommand in filter(lambda x: isinstance(x, Subcommand), source.options):
                         if subcommand.dest == key:
                             setattr(self, key, SubcommandStub(subcommand).set_result(target.subcommands.get(key, None)))
                 elif value is OptionStub:
-                    for option in filter(lambda x: isinstance(x, Option), target.source.options):
+                    for option in filter(lambda x: isinstance(x, Option), source.options):
                         if option.dest == key:
                             setattr(self, key, OptionStub(option).set_result(target.options.get(key, None)))
             elif key != 'header':
                 setattr(self, key, target.all_matched_args.get(key, Empty))
 
     def __repr__(self):
         return f'{self.__class__.__name__}({self.__annotations__})'
@@ -37,24 +39,7 @@
     def option(self, name: str) -> OptionStub | None:
         """获取指定名称的选项存根。"""
         return cast(OptionStub, getattr(self, name, None))
 
     def subcommand(self, name: str) -> SubcommandStub | None:
         """获取指定名称的子命令存根。"""
         return cast(SubcommandStub, getattr(self, name, None))
-
-
-def generate_duplication(arp: Arparma) -> Duplication:
-    """依据给定的命令生成一个解析结果的检查类。"""
-    from .base import Option, Subcommand
-    options = filter(lambda x: isinstance(x, Option), arp.source.options)
-    subcommands = filter(lambda x: isinstance(x, Subcommand), arp.source.options)
-    return cast(Duplication, type(
-        f"{arp.source.name.strip('/.-:')}Interface",
-        (Duplication,), {
-            "__annotations__": {
-                "args": ArgsStub,
-                **{opt.dest: OptionStub for opt in options},
-                **{sub.dest: SubcommandStub for sub in subcommands},
-            }
-        }
-    )(arp))
```

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/exceptions.py` & `arclet-alconna-1.7.7/src/arclet/alconna/exceptions.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/formatter.py` & `arclet-alconna-1.7.7/src/arclet/alconna/formatter.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/i18n/en-US.json` & `arclet-alconna-1.7.7/src/arclet/alconna/i18n/en-US.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/i18n/zh-CN.json` & `arclet-alconna-1.7.7/src/arclet/alconna/i18n/zh-CN.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/manager.py` & `arclet-alconna-1.7.7/src/arclet/alconna/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,15 @@
 
     def get_token(self, result: Arparma) -> int:
         """获取某个命令的 `token`"""
         return next((token for token, res in self.__record.items() if res == result), 0)
 
     def get_result(self, command: Alconna) -> list[Arparma]:
         """获取某个命令的所有 `Arparma` 对象"""
-        return [v for v in self.__record.values() if v.source == command]
+        return [v for v in self.__record.values() if v.source == command.path]
 
     @property
     def recent_message(self) -> DataCollection[str | Any] | None:
         """获取最近一次使用的命令"""
         if rct := self.__record.peek_first_item():
             return rct[1].origin  # type: ignore
```

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/model.py` & `arclet-alconna-1.7.7/src/arclet/alconna/model.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/model.pyi` & `arclet-alconna-1.7.7/src/arclet/alconna/model.pyi`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/output.py` & `arclet-alconna-1.7.7/src/arclet/alconna/output.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/stub.py` & `arclet-alconna-1.7.7/src/arclet/alconna/stub.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/src/arclet/alconna/typing.py` & `arclet-alconna-1.7.7/src/arclet/alconna/typing.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/tests/analyser_test.py` & `arclet-alconna-1.7.7/tests/analyser_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/tests/args_test.py` & `arclet-alconna-1.7.7/tests/args_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/tests/base_test.py` & `arclet-alconna-1.7.7/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/tests/components_test.py` & `arclet-alconna-1.7.7/tests/components_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from arclet.alconna import Alconna, Option, Args, Subcommand, Arparma, ArparmaBehavior
-from arclet.alconna.builtin import set_default
-from arclet.alconna.duplication import Duplication, generate_duplication
+from arclet.alconna.builtin import set_default, generate_duplication
+from arclet.alconna.duplication import Duplication
 from arclet.alconna.stub import ArgsStub, OptionStub, SubcommandStub
 from arclet.alconna.output import output_manager
 from arclet.alconna.model import OptionResult
 
 
 def test_behavior():
     com = Alconna("comp", Args["bar", int]) + Option("foo", default=321)
@@ -53,26 +53,25 @@
     assert isinstance(duplication1, Demo1)
     assert isinstance(duplication1.foo, int)
     assert isinstance(duplication1.bar, str)
     assert isinstance(duplication1.baz, str)
 
     com4_1 = Alconna(["!", "！"], "yiyu", Args["value;OH", str])
     res = com4_1.parse("!yiyu")
-    dup = generate_duplication(res)
+    dup = generate_duplication(com4_1)(res)
     assert isinstance(dup, Duplication)
 
+
 def test_output():
     print("")
     output_manager.set_action(lambda x: {'bar': f'{x}!'}, "foo")
     output_manager.set(lambda: "123", "foo")
     assert output_manager.send("foo") == {"bar": "123!"}
     assert output_manager.send("foo", lambda: "321") == {"bar": "321!"}
 
-
-
     com5 = Alconna("comp5", Args["foo", int], Option("--bar", Args["bar", str]))
     output_manager.set_action(lambda x: x, "comp5")
     with output_manager.capture("comp5") as output:
         res = com5.parse("comp5 --help")
         assert res.matched is False
         assert output.get("output")
         print("")
```

### Comparing `arclet-alconna-1.7.6/tests/config_test.py` & `arclet-alconna-1.7.7/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.6/tests/core_test.py` & `arclet-alconna-1.7.7/tests/core_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,17 @@
 
 def test_bracket_header():
     alc2 = Alconna("RD{r:int}?=={e:int}")
     res = alc2.parse("RD100==36")
     assert res.matched is True
     assert res.header["r"] == 100
     assert res.header["e"] == 36
+    alc2_1 = Alconna(r"RD\{r:int\}")
+    assert not alc2_1.parse("RD100").matched
+    assert alc2_1.parse("RD{r:int}").matched
 
 
 def test_formatter():
     from tarina import lang
     alc3 = Alconna(
         "/pip",
         Subcommand(
@@ -598,16 +601,21 @@
     assert res.query("i.foo") == 5
     assert res.query("a.value") == [1, 1]
     assert res.query("flag.flag") == ["abc", "def", "xyz"]
     assert res.query("v.value") == 3
     assert res.query("xyz.value") == 4
     assert res.query("foo_bar_q.value") == 3
 
+    alc24_3 = Alconna(
+        "core24_3", Option("-t", default=False, action=append_value(True))
+    )
+    assert alc24_3.parse("core24_3 -t -t -t").query("t.value") == [True, True, True]
+
 
-def test_defualt():
+def test_default():
     from arclet.alconna import store_value, OptionResult, append, store_true
 
     alc25 = Alconna(
         "core25",
         Option("--foo", action=store_value(123), default=423),
         Option("bar", Args["baz;?", int]["qux", float, 1.0], default=OptionResult(args={"baz": 321})),
     )
```

### Comparing `arclet-alconna-1.7.6/PKG-INFO` & `arclet-alconna-1.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna
-Version: 1.7.6
+Version: 1.7.7
 Summary: A High-performance, Generality, Humane Command Line Arguments Parser Library.
 License: MIT
 Keywords: command,argparse,fast,alconna,cli,command-line,parsing,optparse
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

