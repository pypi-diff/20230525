# Comparing `tmp/jorun-0.1.0.tar.gz` & `tmp/jorun-0.1.1.tar.gz`

## Comparing `jorun-0.1.0.tar` & `jorun-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/__init__.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/configuration.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/constants.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/errors.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/logger.py
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/main.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/runner.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/scanner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/handler/__init__.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/handler/base.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/handler/docker.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/handler/group.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/handler/shell.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/palette/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/palette/base.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/palette/darcula.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/types/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/types/options.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/types/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/ui/__init__.py
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/ui/application.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/ui/data_signals.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/ui/main_window.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/ui/task_panel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jorun-0.1.0/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 jorun-0.1.0/LICENSE
--rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 jorun-0.1.0/README.md
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jorun-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 jorun-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/__init__.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/configuration.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/constants.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/errors.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/logger.py
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/main.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/runner.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/scanner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/handler/__init__.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/handler/base.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/handler/docker.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/handler/group.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/handler/shell.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/palette/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/palette/base.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/palette/darcula.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/types/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/types/options.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/types/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/ui/__init__.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/ui/application.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/ui/data_signals.py
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/ui/main_window.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/ui/pane.py
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 jorun-0.1.1/src/jorun/ui/task_panel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jorun-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 jorun-0.1.1/LICENSE
+-rw-r--r--   0        0        0     7819 2020-02-02 00:00:00.000000 jorun-0.1.1/README.md
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jorun-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8239 2020-02-02 00:00:00.000000 jorun-0.1.1/PKG-INFO
```

### Comparing `jorun-0.1.0/src/jorun/logger.py` & `jorun-0.1.1/src/jorun/logger.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.0/src/jorun/main.py` & `jorun-0.1.1/src/jorun/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 
 parser = argparse.ArgumentParser(prog="jorun", description="A smart task runner", add_help=True)
 
 parser.add_argument("configuration_file", help="The yml configuration file to run")
 parser.add_argument("--level", help="The log level (DEBUG, INFO, ...)", default="INFO", type=str)
 parser.add_argument("--file-output", help="Log tasks output to files, one per task. "
                                           "This option lets you specify the directory of the log files", type=str)
-parser.add_argument("--gui", help="Run with a graphical interface", action='store_true')
+parser.add_argument("--gui", help="Force running with the graphical interface", action='store_true')
+parser.add_argument("--no-gui", help="Force running without the graphical interface", action='store_true')
 
 running_tasks: List[TaskRunner] = []
 async_tasks: Set[asyncio.Task] = set()
 
 missing_tasks: Dict[str, Task] = {}
 completed_tasks: Set[str] = set()
 
@@ -84,35 +85,38 @@
     global missing_tasks, program_arguments, ui_application, log_handler
 
     register_instance(DarculaColorPalette(), register_for=BaseColorPalette)
 
     program_arguments = parser.parse_args()
     logger.setLevel(program_arguments.level)
 
-    if program_arguments.gui:
+    logger.debug("Loading configuration file")
+    config: TasksConfiguration = load_config(program_arguments.configuration_file)
+
+    gui_config = config.get("gui")
+    show_gui = not program_arguments.no_gui and (program_arguments.gui or gui_config)
+
+    if show_gui:
         logger.debug("Using graphical interface")
         log_handler = QueueHandler(task_streams_queue)
     else:
         logger.debug("Using console output")
         log_handler = NewlineStreamHandler(sys.stdout)
 
-    logger.debug("Loading configuration file")
-    config: TasksConfiguration = load_config(program_arguments.configuration_file)
-
     missing_tasks = config["tasks"].copy()
     loop = asyncio.get_event_loop()
 
-    if program_arguments.gui:
+    if show_gui:
         def on_app_stop():
             logger.info("Main window closed")
             loop.stop()
 
         ui_tasks = [t_name for t_name, t_val in missing_tasks.items() if t_val["type"] != "group"]
 
-        ui_application = UiApplication(ui_tasks, on_app_stop, task_streams_queue, config.get("gui"))
+        ui_application = UiApplication(ui_tasks, on_app_stop, task_streams_queue, gui_config)
         ui_application.start_ui()
 
     try:
         run_missing_tasks()
         loop.run_forever()
     except KeyboardInterrupt:
         logger.info("Requested termination")
@@ -120,15 +124,15 @@
         logger.error("An error occurred")
         traceback.print_exception(e)
     finally:
         logger.info("Terminating the async loop...")
         if loop.is_running():
             loop.stop()
 
-        if program_arguments.gui:
+        if show_gui:
             logger.info("Killing gui...")
             ui_application.stop_ui()
 
         logger.info("Killing async tasks...")
         for t in async_tasks:
             t.cancel()
```

### Comparing `jorun-0.1.0/src/jorun/runner.py` & `jorun-0.1.1/src/jorun/runner.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.0/src/jorun/scanner.py` & `jorun-0.1.1/src/jorun/scanner.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.0/src/jorun/handler/base.py` & `jorun-0.1.1/src/jorun/handler/base.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.0/src/jorun/handler/docker.py` & `jorun-0.1.1/src/jorun/handler/docker.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.0/src/jorun/handler/group.py` & `jorun-0.1.1/src/jorun/handler/group.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.0/src/jorun/handler/shell.py` & `jorun-0.1.1/src/jorun/handler/shell.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.0/src/jorun/types/task.py` & `jorun-0.1.1/src/jorun/types/task.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,21 +12,22 @@
     docker: Optional[DockerTask]
     run_mode: Literal["wait_completion", "indefinite"]
     completion_pattern: Optional[str]
     pattern_in_stderr: Optional[bool]
     depends: Optional[List[str]]
 
 
-class GuiConfiguration(TypedDict):
+class PaneConfiguration(TypedDict):
     columns: int
+    tasks: List[str]
 
 
 class TasksConfiguration(TypedDict):
     tasks: Dict[str, Task]
-    gui: Optional[GuiConfiguration]
+    gui: Optional[Dict[str, PaneConfiguration]]
 
 
 @dataclass
 class TaskNode:
     task: Task
     dependencies: List["TaskNode"]
```

### Comparing `jorun-0.1.0/src/jorun/ui/application.py` & `jorun-0.1.1/src/jorun/ui/application.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import sys
 import time
 from queue import Queue, Empty
 from threading import Thread
-from typing import List, Callable, Optional
+from typing import List, Callable, Optional, Dict
 
 from PyQt6.QtWidgets import QApplication
 
 from .main_window import MainWindow
 from .. import constants
 from ..logger import logger
-from ..types.task import GuiConfiguration
+from ..types.task import PaneConfiguration
 
 
 class UiApplication:
     _ui_thread: Thread
     _running: bool
 
     _app: QApplication
     _window: Optional[MainWindow]
-    _config: Optional[GuiConfiguration]
+    _config: Optional[Dict[str, PaneConfiguration]]
 
     _task_list: List[str]
     _streams_queue: Queue
     _close_handler: Callable
 
     _stream_dequeue_thread: Thread
     _stream_dequeue_running: bool
 
     _trigger_close_handler: bool
 
     def __init__(self, tasks: List[str], close_handler: Callable, task_streams_queue: Queue,
-                 config: Optional[GuiConfiguration]):
+                 config: Optional[Dict[str, PaneConfiguration]]):
         self._window = None
         self._trigger_close_handler = True
         self._config = config
         self._task_list = tasks
         self._close_handler = close_handler
         self._streams_queue = task_streams_queue
 
@@ -64,19 +64,15 @@
             else:
                 time.sleep(.1)
 
     def _run_ui_thread(self):
         self._app = QApplication(sys.argv)
         self._app.setQuitOnLastWindowClosed(True)
 
-        columns = constants.DEFAULT_COLUMNS
-        if self._config and self._config.get('columns'):
-            columns = self._config.get('columns')
-
-        self._window = MainWindow(self._task_list, total_columns=columns)
+        self._window = MainWindow(self._task_list, gui_config=self._config)
         self._window.show()
 
         self._app.exec()
         self._running = False
         self._app_quitting()
 
     def stop_ui(self):
```

### Comparing `jorun-0.1.0/src/jorun/ui/main_window.py` & `jorun-0.1.1/src/jorun/ui/pane.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,60 @@
 from logging import LogRecord
-from typing import Dict, List
+from typing import Optional, List, Dict
 
 from PyQt6.QtCore import Qt
-from PyQt6.QtWidgets import QMainWindow, QSplitter
+from PyQt6.QtWidgets import QWidget, QSplitter, QVBoxLayout
 
 from tinyioc import inject
 
-from .data_signals import DataUpdateSignalEmitter, MainWindowSignals
-from .task_panel import TaskPanel
-from .. import constants
 from ..palette.base import BaseColorPalette
+from .task_panel import TaskPanel
 
 
-class MainWindow(QMainWindow, DataUpdateSignalEmitter):
+class TasksPane(QWidget):
+    _layout: QVBoxLayout
     _central_widget: QSplitter
     _tasks: List[str]
     _total_columns: int
     _task_widgets: Dict[str, TaskPanel]
     _splitters: List[QSplitter]
 
-    signals = MainWindowSignals()
-
     @inject()
-    def __init__(self, tasks: List[str], palette: BaseColorPalette, total_columns=3):
-        super(MainWindow, self).__init__()
-
-        self.signals.app_terminated.connect(self.close)
+    def __init__(self, parent: Optional[QWidget], tasks: List[str], palette: BaseColorPalette, columns: int = 3):
+        super(TasksPane, self).__init__(parent)
 
         self._tasks = tasks
-        self._total_columns = total_columns
+        self._total_columns = columns
         self._task_widgets = {}
         self._splitters = []
 
-        self.setStyleSheet(f"""
-            background-color: {palette.background};
-        """)
-        self.setMinimumSize(300, 300)
-
-        self.setWindowTitle(constants.APP_NAME)
-
         self._central_widget = QSplitter(Qt.Orientation.Vertical, self)
         self._central_widget.setStyleSheet(f"""
             background-color: {palette.background};
         """)
-        self.setCentralWidget(self._central_widget)
+
+        self._layout = QVBoxLayout(self)
+        self.setLayout(self._layout)
         self.setContentsMargins(4, 4, 4, 4)
 
+        self._layout.addWidget(self._central_widget)
+
         col = 0
         for task in self._tasks:
             if col % self._total_columns == 0:
                 last_splitter = QSplitter(Qt.Orientation.Horizontal, self._central_widget)
                 last_splitter.setStyleSheet(f"""
                     background-color: {palette.background};
                 """)
                 self._central_widget.addWidget(last_splitter)
                 self._splitters.append(last_splitter)
 
-            task_panel = TaskPanel(self._splitters[-1], task, self)
+            task_panel = TaskPanel(self._splitters[-1], task)
             self._splitters[-1].addWidget(task_panel)
             self._task_widgets[task] = task_panel
 
             col += 1
 
     # noinspection PyUnresolvedReferences
-    def dispatch_stream_record(self, record: LogRecord):
-        self.signals.data_received.emit(record)
-
-    def dispatch_app_termination(self):
-        self.signals.app_terminated.emit()
+    def dispatch_log_record(self, record: LogRecord):
+        if record.subprocess in self._task_widgets:
+            self._task_widgets[record.subprocess].append_text(record)
```

### Comparing `jorun-0.1.0/src/jorun/ui/task_panel.py` & `jorun-0.1.1/src/jorun/ui/task_panel.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,47 +6,46 @@
 from tinyioc import inject
 
 from .data_signals import DataUpdateSignalEmitter
 from ..palette.base import BaseColorPalette
 
 from .. import constants
 
+
 class TaskPanel(QGroupBox):
     _layout: QVBoxLayout
     _actions_group_widget: QWidget
-    _actions_group_layout: QHBoxLayout
+    _actions_group_layout: QVBoxLayout
     _output_stream_edit_text: QPlainTextEdit
 
     _output_stream: str
 
     _task_name: str
     _task_label: QLabel
 
     _filter_edit_text: QLineEdit
 
     @inject()
-    def __init__(self, parent: Optional[QWidget], task_name: str, signal_emitter: DataUpdateSignalEmitter,
-                 palette: BaseColorPalette):
+    def __init__(self, parent: Optional[QWidget], task_name: str, palette: BaseColorPalette):
         super(TaskPanel, self).__init__(parent)
 
-        signal_emitter.signals.data_received.connect(self.append_text)
-
         self._task_name = task_name
         self._output_stream = ""
 
         self._layout = QVBoxLayout(self)
         self.setLayout(self._layout)
 
         self.setStyleSheet(f"""
             background-color: {palette.current_line};
             border: 0;
         """)
 
         self._actions_group_widget = QWidget(self)
-        self._actions_group_layout = QHBoxLayout(self)
+        self._actions_group_layout = QVBoxLayout(self)
+        self._actions_group_layout.setContentsMargins(0, 0, 0, 0)
         self._actions_group_widget.setLayout(self._actions_group_layout)
 
         self._layout.addWidget(self._actions_group_widget)
 
         self._task_label = QLabel(self)
         self._task_label.setText(self._task_name)
         self._task_label.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Fixed)
@@ -74,27 +73,26 @@
             color: {palette.foreground}; 
             font-family: monospace;
         """)
         self._layout.addWidget(self._output_stream_edit_text, 1)
 
     # noinspection PyUnresolvedReferences
     def append_text(self, record: LogRecord):
-        if record.subprocess == self._task_name:
-            scroll_bottom = False
+        scroll_bottom = False
 
-            if self._output_stream_edit_text.verticalScrollBar().value() > \
-                    self._output_stream_edit_text.verticalScrollBar().maximum() - constants.SCROLL_TOLERANCE:
-                scroll_bottom = True
-
-            self._output_stream += record.message
-            self._update_output_edit_text()
-
-            if scroll_bottom:
-                self._output_stream_edit_text.verticalScrollBar().setValue(
-                    self._output_stream_edit_text.verticalScrollBar().maximum())
+        if self._output_stream_edit_text.verticalScrollBar().value() > \
+                self._output_stream_edit_text.verticalScrollBar().maximum() - constants.SCROLL_TOLERANCE:
+            scroll_bottom = True
+
+        self._output_stream += record.message
+        self._update_output_edit_text()
+
+        if scroll_bottom:
+            self._output_stream_edit_text.verticalScrollBar().setValue(
+                self._output_stream_edit_text.verticalScrollBar().maximum())
 
     def _update_output_edit_text(self):
         filter_input = self._filter_edit_text.text()
 
         if filter_input:
             filtered_text = ""
             for line in self._output_stream.splitlines(keepends=True):
```

### Comparing `jorun-0.1.0/LICENSE` & `jorun-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jorun-0.1.0/README.md` & `jorun-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -15,29 +15,37 @@
 # 
 # A smart task runner
 # 
 # positional arguments:
 #   configuration_file    The yml configuration file to run
 # 
 # options:
-#   -h, --help            show this help message and exit
-#   --level LEVEL         The log level (DEBUG, INFO, ...)
-#   --file-output FILE_OUTPUT
-#                         Log tasks output to files, one per task. This option lets you specify the directory of the log files
-#   --gui                 Run with a graphical interface
-
+#  -h, --help            show this help message and exit
+#  --level LEVEL         The log level (DEBUG, INFO, ...)
+#  --file-output FILE_OUTPUT
+#                        Log tasks output to files, one per task. This option lets you specify the directory of the log files
+#  --gui                 Force running with the graphical interface
+#  --no-gui              Force running without the graphical interface
 
 jorun ./conf.yml
 ```
 
 ## Configuration
 
 ```yml
 gui:
-  columns: 4
+  services:
+    tasks:
+      - db
+      - redis
+  terminals:
+    tasks:
+      - test_1
+      - test_2
+      - test_3
 tasks:
   db:
     type: docker
     docker:
       container_name: test
       image: postgres
       docker_arguments:
@@ -99,36 +107,38 @@
 
 - *completed* (i.e. the task finished executing), by default
 - _the completion pattern is matched_ (the regex pattern matched a line of the task output), if you set a **completion_pattern**
 - _launched_, if you set the **run_mode** to `indefinite`
 
 ## GUI
 
-Through the `--gui` command line option you can run *Jorun* with a graphical interface.
+If you run **Jorun** with the `--gui` command line option, or if you specify the **gui** option
+in the yaml configuration you can start the tool with a graphical interface.
 The GUI is still a prototype, but will let you keep track of the task logs individually and
-even filter the log rows by a substring.
+even filter the log rows.
 
-The YML configuration supports a **gui** section where you can specify the number of columns
-you want the form divided into.
+The **gui** section in the YML configuration is where you can specify the panes you want displayed,
+and for each pane you can set the tasks that belong to it and the maximum number of columns visible in the pane.
 
 ## Reference
 
 The options in **bold** are mandatory, while the others can be omitted.
 
 ### YAML Configuration file
 | Option               | Description                                                                    |
 |----------------------|--------------------------------------------------------------------------------|
 | **tasks** _(object)_ | a mapping between task names and the [task configuration](#task_configuration) |
-| **gui** _(object)_   | the [gui configuration](#gui_configuration)                                    |
+| **gui** _(object)_   | a mapping between pane names and the [pane configuration](#pane_configuration) |
 
-#### <a name="gui_configuration"></a> GUI configuration
+#### <a name="pane_configuration"></a> Pane configuration
 
-| Option              | Description                                                   |
-|---------------------|---------------------------------------------------------------|
-| columns _(integer)_ | the number of columns you want the GUI interface divided into |
+| Option                  | Description                                          |
+|-------------------------|------------------------------------------------------|
+| **tasks** _(array)_     | the tasks that will be displayed in this pane        |
+| **columns** _(integer)_ | the number of columns you want the pane divided into |
 
 #### <a name="task_configuration"></a> Task configuration
 
 | Option                        | Description                                                                                                                                   |
 |-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|
 | **type** _(string)_           | the task type (`shell`, `docker` or `group`)                                                                                                  |
 | **shell** _(object)_          | if **type** is `shell`, the [shell configuration](#shell_configuration)                                                                       |
```

### Comparing `jorun-0.1.0/pyproject.toml` & `jorun-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jorun"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Paolo Infante", email="info@paoloinfante.it" },
 ]
 description = "A customizable task runner"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `jorun-0.1.0/PKG-INFO` & `jorun-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jorun
-Version: 0.1.0
+Version: 0.1.1
 Summary: A customizable task runner
 Project-URL: Homepage, https://github.com/paolo-projects/jorun
 Project-URL: Bug Tracker, https://github.com/paolo-projects/jorun/issues
 Author-email: Paolo Infante <info@paoloinfante.it>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,29 +32,37 @@
 # 
 # A smart task runner
 # 
 # positional arguments:
 #   configuration_file    The yml configuration file to run
 # 
 # options:
-#   -h, --help            show this help message and exit
-#   --level LEVEL         The log level (DEBUG, INFO, ...)
-#   --file-output FILE_OUTPUT
-#                         Log tasks output to files, one per task. This option lets you specify the directory of the log files
-#   --gui                 Run with a graphical interface
-
+#  -h, --help            show this help message and exit
+#  --level LEVEL         The log level (DEBUG, INFO, ...)
+#  --file-output FILE_OUTPUT
+#                        Log tasks output to files, one per task. This option lets you specify the directory of the log files
+#  --gui                 Force running with the graphical interface
+#  --no-gui              Force running without the graphical interface
 
 jorun ./conf.yml
 ```
 
 ## Configuration
 
 ```yml
 gui:
-  columns: 4
+  services:
+    tasks:
+      - db
+      - redis
+  terminals:
+    tasks:
+      - test_1
+      - test_2
+      - test_3
 tasks:
   db:
     type: docker
     docker:
       container_name: test
       image: postgres
       docker_arguments:
@@ -116,36 +124,38 @@
 
 - *completed* (i.e. the task finished executing), by default
 - _the completion pattern is matched_ (the regex pattern matched a line of the task output), if you set a **completion_pattern**
 - _launched_, if you set the **run_mode** to `indefinite`
 
 ## GUI
 
-Through the `--gui` command line option you can run *Jorun* with a graphical interface.
+If you run **Jorun** with the `--gui` command line option, or if you specify the **gui** option
+in the yaml configuration you can start the tool with a graphical interface.
 The GUI is still a prototype, but will let you keep track of the task logs individually and
-even filter the log rows by a substring.
+even filter the log rows.
 
-The YML configuration supports a **gui** section where you can specify the number of columns
-you want the form divided into.
+The **gui** section in the YML configuration is where you can specify the panes you want displayed,
+and for each pane you can set the tasks that belong to it and the maximum number of columns visible in the pane.
 
 ## Reference
 
 The options in **bold** are mandatory, while the others can be omitted.
 
 ### YAML Configuration file
 | Option               | Description                                                                    |
 |----------------------|--------------------------------------------------------------------------------|
 | **tasks** _(object)_ | a mapping between task names and the [task configuration](#task_configuration) |
-| **gui** _(object)_   | the [gui configuration](#gui_configuration)                                    |
+| **gui** _(object)_   | a mapping between pane names and the [pane configuration](#pane_configuration) |
 
-#### <a name="gui_configuration"></a> GUI configuration
+#### <a name="pane_configuration"></a> Pane configuration
 
-| Option              | Description                                                   |
-|---------------------|---------------------------------------------------------------|
-| columns _(integer)_ | the number of columns you want the GUI interface divided into |
+| Option                  | Description                                          |
+|-------------------------|------------------------------------------------------|
+| **tasks** _(array)_     | the tasks that will be displayed in this pane        |
+| **columns** _(integer)_ | the number of columns you want the pane divided into |
 
 #### <a name="task_configuration"></a> Task configuration
 
 | Option                        | Description                                                                                                                                   |
 |-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|
 | **type** _(string)_           | the task type (`shell`, `docker` or `group`)                                                                                                  |
 | **shell** _(object)_          | if **type** is `shell`, the [shell configuration](#shell_configuration)                                                                       |
```

