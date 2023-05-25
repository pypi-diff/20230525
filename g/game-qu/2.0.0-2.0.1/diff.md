# Comparing `tmp/game_qu-2.0.0.tar.gz` & `tmp/game_qu-2.0.1.tar.gz`

## Comparing `game_qu-2.0.0.tar` & `game_qu-2.0.1.tar`

### file list

```diff
@@ -1,49 +1,44 @@
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 game_qu-2.0.0/LISCENCE
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/.idea/.gitignore
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/.idea/misc.xml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/.idea/modules.xml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/.idea/src.iml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/.idea/vcs.xml
--rw-r--r--   0        0        0     7402 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/library_abstraction.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/colors.py
--rw-r--r--   0        0        0     5589 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/engines.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/events.py
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/file_reader.py
--rwxr-xr-x   0        0        0     2183 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/fraction.py
--rwxr-xr-x   0        0        0     4088 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/game_movement.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/game_runner_function.py
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/history_keeper.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/id_creator.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/important_constants.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/important_variables.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/keyboard.py
--rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/library_changer.py
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/library_independant_utility_functions.py
--rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/lines.py
--rw-r--r--   0        0        0     8886 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/paths.py
--rw-r--r--   0        0        0    13204 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/quadratic_equations.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/range.py
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/unique_ids_list.py
--rw-r--r--   0        0        0     9423 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/utility_functions.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/base/velocity_calculator.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/gui_components/component.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/gui_components/dimensions.py
--rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/gui_components/grid.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/gui_components/hud.py
--rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/gui_components/intermediate_screen.py
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/gui_components/navigation_screen.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/gui_components/screen.py
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/gui_components/text_box.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/gui_components/window.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/pygame_abstraction/keys.py
--rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/pygame_abstraction/utility_functions.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/pygame_abstraction/variables.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/pyglet_abstraction/keys.py
--rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/pyglet_abstraction/utility_functions.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 game_qu-2.0.0/src/game_qu/pyglet_abstraction/variables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 game_qu-2.0.0/README.md
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 game_qu-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 game_qu-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 game_qu-2.0.1/LISCENCE
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 game_qu-2.0.1/.idea/workspace.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/__init__.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/game_runner.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/library_abstraction.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/colors.py
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/engines.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/events.py
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/file_reader.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/fraction.py
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/game_movement.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/game_runner_function.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/history_keeper.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/id_creator.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/important_constants.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/important_variables.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/keyboard.py
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/library_changer.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/library_independant_utility_functions.py
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/lines.py
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/paths.py
+-rw-r--r--   0        0        0    13518 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/quadratic_equations.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/range.py
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/unique_ids_list.py
+-rw-r--r--   0        0        0     9677 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/utility_functions.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/velocity_calculator.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/gui_components/component.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/gui_components/dimensions.py
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/gui_components/grid.py
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/gui_components/hud.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/gui_components/intermediate_screen.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/gui_components/navigation_screen.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/gui_components/screen.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/gui_components/text_box.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/gui_components/window.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/pygame_abstraction/keys.py
+-rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/pygame_abstraction/utility_functions.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/pygame_abstraction/variables.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/pyglet_abstraction/keys.py
+-rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/pyglet_abstraction/utility_functions.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/pyglet_abstraction/variables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 game_qu-2.0.1/README.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 game_qu-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 game_qu-2.0.1/PKG-INFO
```

### Comparing `game_qu-2.0.0/LISCENCE` & `game_qu-2.0.1/LISCENCE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `game_qu-2.0.0/src/game_qu/base/engines.py` & `game_qu-2.0.1/src/game_qu/base/engines.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-from game_qu.base.history_keeper import HistoryKeeper
-
-
-class CollisionsEngine:
-    """Provides methods for figuring out if objects have collided"""
-
-    @staticmethod
-    def is_horizontal_collision(object1, object2):
-        """:returns: bool; whether object1 and object2 have collided horizontally (ignores vertical direction- 1D)"""
-
-        return object1.left_edge <= object2.right_edge and object1.right_edge >= object2.left_edge
-
-    @staticmethod
-    def is_vertical_collision(object1, object2):
-        """:returns: bool; whether object1 and object2 have collided vertically (ignores horizontal direction- 1D)"""
-
-        return object1.top_edge <= object2.bottom_edge and object1.bottom_edge >= object2.top_edge
-
-    @staticmethod
-    def is_collision(object1, object2):
-        """:returns: bool; whether object1 and object2 have collided vertically and horizontally"""
-
-        return CollisionsEngine.is_horizontal_collision(object1, object2) and CollisionsEngine.is_vertical_collision(object1, object2)
-
-    @staticmethod
-    def is_left_collision(object1, object2, is_collision=None, last_time=None):
-        """ :returns: bool; if object1 has collided with object2's left edge"""
-
-        objects_are_touching = object1.right_edge == object2.left_edge and CollisionsEngine.is_vertical_collision(
-            object1, object2)
-        is_moving_left_collision = CollisionsEngine.is_moving_left_collision(object1, object2, is_collision, last_time)
-
-        return is_moving_left_collision or objects_are_touching
-
-    @staticmethod
-    def is_right_collision(object1, object2, is_collision=None, last_time=None):
-        """:returns: bool; if object1 has collided with object2's right_edge"""
-
-        is_moving_right_collision = CollisionsEngine.is_moving_right_collision(object1, object2, is_collision,
-                                                                               last_time)
-
-        objects_are_touching = object1.left_edge == object2.right_edge and CollisionsEngine.is_vertical_collision(
-            object1, object2)
-
-        return is_moving_right_collision or objects_are_touching
-
-    @staticmethod
-    def is_moving_right_collision(object1, object2, is_collision=None, last_time=None):
-        """ :returns: bool; if object1 has collided with object2's right_edge because one of the objects has moved
-            (the object1 did not collide with object2 horizontally last cycle)"""
-
-        prev_object1 = HistoryKeeper.get_last(object1.name)
-        prev_object2 = HistoryKeeper.get_last(object2.name)
-
-        if prev_object1 is None or prev_object2 is None:
-            return False
-
-        is_collision = is_collision if is_collision is not None else CollisionsEngine.is_collision(object1, object2)
-        object1_has_moved_into_object2 = (
-                prev_object1.left_edge > prev_object2.right_edge and object1.left_edge < object2.right_edge)
-
-        return is_collision and object1_has_moved_into_object2
-
-    @staticmethod
-    def is_moving_left_collision(object1, object2, is_collision=None, last_time=None):
-        """ :returns: bool; if object1 has hit object2's left_edge because one of the objects has moved
-            (the object1 did not collide with object2 horizontally last cycle)"""
-
-        prev_object1 = HistoryKeeper.get_last(object1.name)
-        prev_object2 = HistoryKeeper.get_last(object2.name)
-
-        if prev_object1 is None or prev_object2 is None:
-            return False
-
-        is_collision = is_collision if is_collision is not None else CollisionsEngine.is_collision(object1, object2)
-
-        object1_has_moved_into_object2 = prev_object1.right_edge < prev_object2.left_edge and object1.right_edge > object2.left_edge
-        return is_collision and object1_has_moved_into_object2
-
-    @staticmethod
-    def is_bottom_collision(object1, object2, is_collision=None, time=None):
-        """ :returns: bool; whether object1 has collided with object2's bottom_edge
-        """
-
-        prev_object1 = HistoryKeeper.get_last(object1.name)
-        prev_object2 = HistoryKeeper.get_last(object2.name)
-
-        if prev_object1 is None or prev_object2 is None:
-            return False
-
-        objects_are_touching = object1.top_edge == object2.bottom_edge and CollisionsEngine.is_horizontal_collision(
-            object1,
-            object2)
-        is_collision = is_collision if is_collision is not None else CollisionsEngine.is_collision(object1, object2)
-
-        # Meaning that it isn't the bottom object anymore
-        return (is_collision and prev_object1.top_edge > prev_object2.bottom_edge and
-                object1.top_edge < object2.bottom_edge) or objects_are_touching
-
-    @staticmethod
-    def is_top_collision(object1, object2, is_collision=None, time=None):
-        """:returns: bool; whether object1 has collided with object2's top_edge"""
-
-        prev_object1 = HistoryKeeper.get_last(object1.name)
-        prev_object2 = HistoryKeeper.get_last(object2.name)
-
-        if prev_object1 is None or prev_object2 is None:
-            return False
-
-        # So rounding doesn't cause any issues
-        objects_are_touching = int(object1.bottom_edge) == int(object2.top_edge) and CollisionsEngine.is_horizontal_collision(object1, object2)
-        is_collision = is_collision if is_collision is not None else CollisionsEngine.is_collision(object1, object2)
-
-        # Meaning that it isn't the bottom object anymore
-        return (is_collision and prev_object1.bottom_edge < prev_object2.top_edge
-                and object1.bottom_edge > object2.top_edge) or objects_are_touching
-
-
+from game_qu.base.history_keeper import HistoryKeeper
+
+
+class CollisionsEngine:
+    """Provides methods for figuring out if objects have collided"""
+
+    @staticmethod
+    def is_horizontal_collision(object1, object2):
+        """:returns: bool; whether object1 and object2 have collided horizontally (ignores vertical direction- 1D)"""
+
+        return object1.left_edge <= object2.right_edge and object1.right_edge >= object2.left_edge
+
+    @staticmethod
+    def is_vertical_collision(object1, object2):
+        """:returns: bool; whether object1 and object2 have collided vertically (ignores horizontal direction- 1D)"""
+
+        return object1.top_edge <= object2.bottom_edge and object1.bottom_edge >= object2.top_edge
+
+    @staticmethod
+    def is_collision(object1, object2):
+        """:returns: bool; whether object1 and object2 have collided vertically and horizontally"""
+
+        return CollisionsEngine.is_horizontal_collision(object1, object2) and CollisionsEngine.is_vertical_collision(object1, object2)
+
+    @staticmethod
+    def is_left_collision(object1, object2, is_collision=None, last_time=None):
+        """ :returns: bool; if object1 has collided with object2's left edge"""
+
+        objects_are_touching = object1.right_edge == object2.left_edge and CollisionsEngine.is_vertical_collision(
+            object1, object2)
+        is_moving_left_collision = CollisionsEngine.is_moving_left_collision(object1, object2, is_collision, last_time)
+
+        return is_moving_left_collision or objects_are_touching
+
+    @staticmethod
+    def is_right_collision(object1, object2, is_collision=None, last_time=None):
+        """:returns: bool; if object1 has collided with object2's right_edge"""
+
+        is_moving_right_collision = CollisionsEngine.is_moving_right_collision(object1, object2, is_collision,
+                                                                               last_time)
+
+        objects_are_touching = object1.left_edge == object2.right_edge and CollisionsEngine.is_vertical_collision(
+            object1, object2)
+
+        return is_moving_right_collision or objects_are_touching
+
+    @staticmethod
+    def is_moving_right_collision(object1, object2, is_collision=None, last_time=None):
+        """ :returns: bool; if object1 has collided with object2's right_edge because one of the objects has moved
+            (the object1 did not collide with object2 horizontally last cycle)"""
+
+        prev_object1 = HistoryKeeper.get_last(object1.name)
+        prev_object2 = HistoryKeeper.get_last(object2.name)
+
+        if prev_object1 is None or prev_object2 is None:
+            return False
+
+        is_collision = is_collision if is_collision is not None else CollisionsEngine.is_collision(object1, object2)
+        object1_has_moved_into_object2 = (
+                prev_object1.left_edge > prev_object2.right_edge and object1.left_edge < object2.right_edge)
+
+        return is_collision and object1_has_moved_into_object2
+
+    @staticmethod
+    def is_moving_left_collision(object1, object2, is_collision=None, last_time=None):
+        """ :returns: bool; if object1 has hit object2's left_edge because one of the objects has moved
+            (the object1 did not collide with object2 horizontally last cycle)"""
+
+        prev_object1 = HistoryKeeper.get_last(object1.name)
+        prev_object2 = HistoryKeeper.get_last(object2.name)
+
+        if prev_object1 is None or prev_object2 is None:
+            return False
+
+        is_collision = is_collision if is_collision is not None else CollisionsEngine.is_collision(object1, object2)
+
+        object1_has_moved_into_object2 = prev_object1.right_edge < prev_object2.left_edge and object1.right_edge > object2.left_edge
+        return is_collision and object1_has_moved_into_object2
+
+    @staticmethod
+    def is_bottom_collision(object1, object2, is_collision=None, time=None):
+        """ :returns: bool; whether object1 has collided with object2's bottom_edge
+        """
+
+        prev_object1 = HistoryKeeper.get_last(object1.name)
+        prev_object2 = HistoryKeeper.get_last(object2.name)
+
+        if prev_object1 is None or prev_object2 is None:
+            return False
+
+        objects_are_touching = object1.top_edge == object2.bottom_edge and CollisionsEngine.is_horizontal_collision(
+            object1,
+            object2)
+        is_collision = is_collision if is_collision is not None else CollisionsEngine.is_collision(object1, object2)
+
+        # Meaning that it isn't the bottom object anymore
+        return (is_collision and prev_object1.top_edge > prev_object2.bottom_edge and
+                object1.top_edge < object2.bottom_edge) or objects_are_touching
+
+    @staticmethod
+    def is_top_collision(object1, object2, is_collision=None, time=None):
+        """:returns: bool; whether object1 has collided with object2's top_edge"""
+
+        prev_object1 = HistoryKeeper.get_last(object1.name)
+        prev_object2 = HistoryKeeper.get_last(object2.name)
+
+        if prev_object1 is None or prev_object2 is None:
+            return False
+
+        # So rounding doesn't cause any issues
+        objects_are_touching = int(object1.bottom_edge) == int(object2.top_edge) and CollisionsEngine.is_horizontal_collision(object1, object2)
+        is_collision = is_collision if is_collision is not None else CollisionsEngine.is_collision(object1, object2)
+
+        # Meaning that it isn't the bottom object anymore
+        return (is_collision and prev_object1.bottom_edge < prev_object2.top_edge
+                and object1.bottom_edge > object2.top_edge) or objects_are_touching
+
+
```

### Comparing `game_qu-2.0.0/src/game_qu/base/file_reader.py` & `game_qu-2.0.1/src/game_qu/base/file_reader.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-import os
-
-class FileReader:
-    """ Reads the contents of a file. The contents of the file must follow this format in order to be read: name:value.
-        For instance, 'high_score:219.0' The value types allowed are int, float, str, bool, float[], and str[]. Generally
-        it would be recommended to use python's built-in json package, but this is also an option for simple file saving and retrieving
-
-        int-format: name:int (high_score:219)
-        float_format: name:float (high_score:219.0)
-        str-format: name:str (name:a)
-        bool_format: name:bool (has_won_game:True)
-        float[]-format: name:[val1,val2,val3] (high_scores:[1.0,2.0,3.0])
-        str[]-format: name:[val1,val2,val3] (names:[a,b,c,d])"""
-
-    name_to_data = {}
-
-    def __init__(self, file_path):
-        """ Initialize the class by reading the file from the 'file_path' and storing the data in 'self.name_to_object'.
-
-            :parameter file_path: str; the path to the file
-
-            :returns: None
-        """
-
-        lines = self.get_lines(file_path)
-
-        for line in lines:
-            delimiter_start = line.index(":")
-
-            name = line[:delimiter_start]
-
-            data = line[delimiter_start + 1:]
-
-            self.name_to_data[name] = data
-
-    def get_lines(self, file_path, new_line_delimiter="\n"):
-        """ Opens the file that was gotten from open(file_path) and uses 'new_line_delimeter' to determine what is a new line
-
-            :parameter file_path: str; the path to the file
-            :parameter new_line_delimiter: str; the delimiter that decides if a new entry in the return_value (lines) should be created
-
-            :returns: str[]; all the lines of the file"""
-
-        file = open(file_path, "r+")
-        lines = file.read().split(new_line_delimiter)
-        file.close()
-        return lines
-
-    def get_int(self, name):
-        """ Retrieves the integer value from 'self.name_to_data' associated with the key 'name'
-
-            :parameter name: str; the name of the key
-
-            :returns: int; the int value associated with the key 'name'
-        """
-
-        return int(self.name_to_data[name])
-
-    def get_float(self, name):
-        """ Retrieves the float value from 'self.name_to_data' associated with the key 'name'
-
-            :parameter name: str; the name of the key
-
-            :returns: float; the float value associated with the key 'name'
-        """
-
-        return float(self.name_to_data[name])
-
-    def get_bool(self, name):
-        """ Retrieves the bool value from 'self.name_to_data' associated with the key 'name'
-
-            :parameter name: str; the name of the key
-
-            :returns: bool; the bool value associated with the key 'name'
-        """
-
-        return self.name_to_data[name] == "True"
-
-    def get_string_list(self, name):
-        """ Retrieves the string list from 'self.name_to_data' associated with the key 'name'
-
-            :parameter name: str; the name of the key
-
-            :returns: str[]; the str[] value associated with the key 'name'
-        """
-
-        return self.name_to_data[name][1:-1].split(",")
-
-    def get_float_list(self, name):
-        """ Retrieves the float list from 'self.name_to_data' associated with the key 'name' (calls get_string_list())
-
-            :parameter name: str; the name of the key
-
-            :returns: float[]; the float[] value associated with the key 'name'
-        """
-
-        string_list = self.get_string_list(name)
-        float_list = []
-
-        for item in string_list:
-            float_list.append(float(item))
-
-        return float_list
-
-    def get_string(self, name):
-        """ Retrieves the string from 'self.name_to_data' associated with the key 'name'
-
-            :parameter name: str; the name of the key
-
-            :returns: str; the str value associated with the key 'name'
-        """
-
-        return self.name_to_data[name]
-
-
-
-
-
+import os
+
+class FileReader:
+    """ Reads the contents of a file. The contents of the file must follow this format in order to be read: name:value.
+        For instance, 'high_score:219.0' The value types allowed are int, float, str, bool, float[], and str[]. Generally
+        it would be recommended to use python's built-in json package, but this is also an option for simple file saving and retrieving
+
+        int-format: name:int (high_score:219)
+        float_format: name:float (high_score:219.0)
+        str-format: name:str (name:a)
+        bool_format: name:bool (has_won_game:True)
+        float[]-format: name:[val1,val2,val3] (high_scores:[1.0,2.0,3.0])
+        str[]-format: name:[val1,val2,val3] (names:[a,b,c,d])"""
+
+    name_to_data = {}
+
+    def __init__(self, file_path):
+        """ Initialize the class by reading the file from the 'file_path' and storing the data in 'self.name_to_object'.
+
+            :parameter file_path: str; the path to the file
+
+            :returns: None
+        """
+
+        lines = self.get_lines(file_path)
+
+        for line in lines:
+            delimiter_start = line.index(":")
+
+            name = line[:delimiter_start]
+
+            data = line[delimiter_start + 1:]
+
+            self.name_to_data[name] = data
+
+    def get_lines(self, file_path, new_line_delimiter="\n"):
+        """ Opens the file that was gotten from open(file_path) and uses 'new_line_delimeter' to determine what is a new line
+
+            :parameter file_path: str; the path to the file
+            :parameter new_line_delimiter: str; the delimiter that decides if a new entry in the return_value (lines) should be created
+
+            :returns: str[]; all the lines of the file"""
+
+        file = open(file_path, "r+")
+        lines = file.read().split(new_line_delimiter)
+        file.close()
+        return lines
+
+    def get_int(self, name):
+        """ Retrieves the integer value from 'self.name_to_data' associated with the key 'name'
+
+            :parameter name: str; the name of the key
+
+            :returns: int; the int value associated with the key 'name'
+        """
+
+        return int(self.name_to_data[name])
+
+    def get_float(self, name):
+        """ Retrieves the float value from 'self.name_to_data' associated with the key 'name'
+
+            :parameter name: str; the name of the key
+
+            :returns: float; the float value associated with the key 'name'
+        """
+
+        return float(self.name_to_data[name])
+
+    def get_bool(self, name):
+        """ Retrieves the bool value from 'self.name_to_data' associated with the key 'name'
+
+            :parameter name: str; the name of the key
+
+            :returns: bool; the bool value associated with the key 'name'
+        """
+
+        return self.name_to_data[name] == "True"
+
+    def get_string_list(self, name):
+        """ Retrieves the string list from 'self.name_to_data' associated with the key 'name'
+
+            :parameter name: str; the name of the key
+
+            :returns: str[]; the str[] value associated with the key 'name'
+        """
+
+        return self.name_to_data[name][1:-1].split(",")
+
+    def get_float_list(self, name):
+        """ Retrieves the float list from 'self.name_to_data' associated with the key 'name' (calls get_string_list())
+
+            :parameter name: str; the name of the key
+
+            :returns: float[]; the float[] value associated with the key 'name'
+        """
+
+        string_list = self.get_string_list(name)
+        float_list = []
+
+        for item in string_list:
+            float_list.append(float(item))
+
+        return float_list
+
+    def get_string(self, name):
+        """ Retrieves the string from 'self.name_to_data' associated with the key 'name'
+
+            :parameter name: str; the name of the key
+
+            :returns: str; the str value associated with the key 'name'
+        """
+
+        return self.name_to_data[name]
+
+
+
+
+
```

### Comparing `game_qu-2.0.0/src/game_qu/base/fraction.py` & `game_qu-2.0.1/src/game_qu/base/fraction.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.0/src/game_qu/base/game_movement.py` & `game_qu-2.0.1/src/game_qu/base/game_movement.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.0/src/game_qu/base/game_runner_function.py` & `game_qu-2.0.1/src/game_qu/base/game_runner_function.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import time
-from game_qu.base.important_variables import *
-from game_qu.base.history_keeper import HistoryKeeper
-from game_qu.base.velocity_calculator import VelocityCalculator
-from game_qu.library_abstraction import utility_functions
-
-def run_game(main_screen):
-    """ Runs all the game code. This will add 'main_screen' to the 'game_window,' so the 'main_screen' components and run
-        function can be called. If there should be multiple screens for this game, game_screen.add_screen() should be called.
-        This function specifically calls game_window.add_screen() and call_every_cycle()"""
-
-    game_window.add_screen(main_screen)
-    utility_functions.call_every_cycle(_run_game_every_cycle)
-
-
-def _run_game_every_cycle(cycle_time, is_start_time, should_render):
-    """ Runs all the code that should be called every game cycle. This function updates all the game components. This
-        function should generally not be called because the run_game method will do that for you"""
-
-    keyboard.run()
-    game_window.run(should_render)
-
-    if is_start_time:
-        cycle_time = time.time() - cycle_time
-
-    HistoryKeeper.set_last_frame_id(VelocityCalculator.current_cycle_number)
-    VelocityCalculator.time = cycle_time
-    VelocityCalculator.current_cycle_number += 1
-
-
-
+import time
+from game_qu.base.important_variables import *
+from game_qu.base.history_keeper import HistoryKeeper
+from game_qu.base.velocity_calculator import VelocityCalculator
+from game_qu.library_abstraction import utility_functions
+
+def run_game(main_screen):
+    """ Runs all the game code. This will add 'main_screen' to the 'game_window,' so the 'main_screen' components and run
+        function can be called. If there should be multiple screens for this game, game_screen.add_screen() should be called.
+        This function specifically calls game_window.add_screen() and call_every_cycle()"""
+
+    game_window.add_screen(main_screen)
+    utility_functions.call_every_cycle(_run_game_every_cycle)
+
+
+def _run_game_every_cycle(cycle_time, is_start_time, should_render):
+    """ Runs all the code that should be called every game cycle. This function updates all the game components. This
+        function should generally not be called because the run_game method will do that for you"""
+
+    keyboard.run()
+    game_window.run(should_render)
+
+    if is_start_time:
+        cycle_time = time.time() - cycle_time
+
+    HistoryKeeper.set_last_frame_id(VelocityCalculator.current_cycle_number)
+    VelocityCalculator.time = cycle_time
+    VelocityCalculator.current_cycle_number += 1
+
+
+
```

### Comparing `game_qu-2.0.0/src/game_qu/base/history_keeper.py` & `game_qu-2.0.1/src/game_qu/base/history_keeper.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-from copy import deepcopy
-
-from game_qu.base.velocity_calculator import VelocityCalculator
-from game_qu.gui_components.dimensions import Dimensions
-from game_qu.base.important_constants import *
-
-
-class HistoryKeeper:
-    last_objects = {}
-    last_frame_id = 0
-
-    @staticmethod
-    def add(history_keeper_object, name, needs_dimensions_only=False, needs_deepcopy=False):
-        """ Adds the object to the HistoryKeeper; IMPORTANT: make sure to provide a unique name for each unique object!
-
-            :parameter history_keeper_object: Object; the object that is going to be added to the HistoryKeeper
-            :parameter name: String; the unique name (identifier) for the object
-            :parameter needs_deepcopy: bool; the object provided is an instance of GameObject
-            :parameter needs_dimensions_only: bool; whether the object stored only needs the dimensions stored for it
-
-            :returns: None
-        """
-
-        if needs_deepcopy:
-            history_keeper_object = deepcopy(history_keeper_object)
-            history_keeper_object.name = name
-
-        if needs_dimensions_only:
-            history_keeper_object = Dimensions(history_keeper_object.left_edge, history_keeper_object.top_edge,
-                                               history_keeper_object.length, history_keeper_object.height)
-            history_keeper_object.name = name
-
-        frame_id = HistoryKeeper.get_frame_id(VelocityCalculator.current_cycle_number)
-        HistoryKeeper.last_objects[f"{name}_{frame_id}"] = history_keeper_object
-
-    @staticmethod
-    def get_last(name):
-        """ Gets the version of that object from the last cycle
-
-            :parameter name: str; the unique name (identifier) given for the object in HistoryKeeper.add() that is used to retrieve the previous version of the object
-
-            :returns: the version of the object from the last cycle
-        """
-
-        return HistoryKeeper.get_last_using_frame_id(name, HistoryKeeper.last_frame_id)
-
-    @staticmethod
-    def get_last_using_frame_id(name, frame_id):
-        """ Gets the version of that object from at that cycle (decided by 'frame_id')
-
-            :parameter name: str; the unique name (identifier) given for the object in HistoryKeeper.add() that is used to get the object at the specific cycle
-            :parameter frame_id: int; the frame_id of the cycle
-
-            :returns: the version of the object from the last cycle
-        """
-        return HistoryKeeper.last_objects.get(f"{name}_{frame_id}")
-
-    @staticmethod
-    def reset():
-        """Resets the HistoryKeeper, so it has no more values of past objects"""
-
-        HistoryKeeper.last_objects = {}
-        HistoryKeeper.times = []
-
-    @staticmethod
-    def set_last_frame_id(cycle_number):
-        """Sets the last time of the HistoryKeeper"""
-
-        HistoryKeeper.last_frame_id = HistoryKeeper.get_frame_id(cycle_number)
-
-    @staticmethod
-    def get_frame_id(cycle_number):
-        """ :returns: int; the identifier for that frame (the number of frames that the HistoryKeeper stores is equal to
-            'FRAMES_HISTORY_KEEPER_STORES' in base/important_variables"""
-        
-        return cycle_number % NUMBER_OF_FRAMES_HISTORY_KEEPER_STORES
-
-    @staticmethod
-    def get_all_of_name(name):
-        """:returns: all the objects in the HistoryKeeper that have the name 'name'"""
-
-        return_value = {}
-
-        for x in range(NUMBER_OF_FRAMES_HISTORY_KEEPER_STORES):
-            key = f"{name}_{x}"
-            value = HistoryKeeper.last_objects.get(key)
-
-            if value is not None:
-                return_value[key] = value
-
-        return return_value
-
-
-
-
-
-
-
-
+from copy import deepcopy
+
+from game_qu.base.velocity_calculator import VelocityCalculator
+from game_qu.gui_components.dimensions import Dimensions
+from game_qu.base.important_constants import *
+
+
+class HistoryKeeper:
+    last_objects = {}
+    last_frame_id = 0
+
+    @staticmethod
+    def add(history_keeper_object, name, needs_dimensions_only=False, needs_deepcopy=False):
+        """ Adds the object to the HistoryKeeper; IMPORTANT: make sure to provide a unique name for each unique object!
+
+            :parameter history_keeper_object: Object; the object that is going to be added to the HistoryKeeper
+            :parameter name: String; the unique name (identifier) for the object
+            :parameter needs_deepcopy: bool; the object provided is an instance of GameObject
+            :parameter needs_dimensions_only: bool; whether the object stored only needs the dimensions stored for it
+
+            :returns: None
+        """
+
+        if needs_deepcopy:
+            history_keeper_object = deepcopy(history_keeper_object)
+            history_keeper_object.name = name
+
+        if needs_dimensions_only:
+            history_keeper_object = Dimensions(history_keeper_object.left_edge, history_keeper_object.top_edge,
+                                               history_keeper_object.length, history_keeper_object.height)
+            history_keeper_object.name = name
+
+        frame_id = HistoryKeeper.get_frame_id(VelocityCalculator.current_cycle_number)
+        HistoryKeeper.last_objects[f"{name}_{frame_id}"] = history_keeper_object
+
+    @staticmethod
+    def get_last(name):
+        """ Gets the version of that object from the last cycle
+
+            :parameter name: str; the unique name (identifier) given for the object in HistoryKeeper.add() that is used to retrieve the previous version of the object
+
+            :returns: the version of the object from the last cycle
+        """
+
+        return HistoryKeeper.get_last_using_frame_id(name, HistoryKeeper.last_frame_id)
+
+    @staticmethod
+    def get_last_using_frame_id(name, frame_id):
+        """ Gets the version of that object from at that cycle (decided by 'frame_id')
+
+            :parameter name: str; the unique name (identifier) given for the object in HistoryKeeper.add() that is used to get the object at the specific cycle
+            :parameter frame_id: int; the frame_id of the cycle
+
+            :returns: the version of the object from the last cycle
+        """
+        return HistoryKeeper.last_objects.get(f"{name}_{frame_id}")
+
+    @staticmethod
+    def reset():
+        """Resets the HistoryKeeper, so it has no more values of past objects"""
+
+        HistoryKeeper.last_objects = {}
+        HistoryKeeper.times = []
+
+    @staticmethod
+    def set_last_frame_id(cycle_number):
+        """Sets the last time of the HistoryKeeper"""
+
+        HistoryKeeper.last_frame_id = HistoryKeeper.get_frame_id(cycle_number)
+
+    @staticmethod
+    def get_frame_id(cycle_number):
+        """ :returns: int; the identifier for that frame (the number of frames that the HistoryKeeper stores is equal to
+            'FRAMES_HISTORY_KEEPER_STORES' in base/important_variables"""
+        
+        return cycle_number % NUMBER_OF_FRAMES_HISTORY_KEEPER_STORES
+
+    @staticmethod
+    def get_all_of_name(name):
+        """:returns: all the objects in the HistoryKeeper that have the name 'name'"""
+
+        return_value = {}
+
+        for x in range(NUMBER_OF_FRAMES_HISTORY_KEEPER_STORES):
+            key = f"{name}_{x}"
+            value = HistoryKeeper.last_objects.get(key)
+
+            if value is not None:
+                return_value[key] = value
+
+        return return_value
+
+
+
+
+
+
+
+
```

### Comparing `game_qu-2.0.0/src/game_qu/base/id_creator.py` & `game_qu-2.0.1/src/game_qu/base/id_creator.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import random
-
-from game_qu.base.unique_ids_list import unique_ids
-from game_qu.base.library_independant_utility_functions import get_string
-
-
-class IDCreator:
-    """A class that creates simple unique identifiers"""
-
-    all_chs = ['1', '2', '3', '4', '5', '6', '7', '8', '9', '0', '-', '=', 'q', 'w', 'e', 'r', 't', 'y', 'u', 'i', 'o', 'p', '[', ']', 'a', 's', 'd', 'f', 'g', 'h', 'j', 'k', 'l', ';', "'", 'z', 'c', 'v', 'b', 'n', 'm', ',', '.', '/', '~', '!', '@', '#', '$', '%', '^', '&', '*', '(', ')', '_', '+', 'Q', 'W', 'E', 'R', 'T', 'Y', 'U', 'I', 'O', 'P', '{', '}', 'A', 'S', 'D', 'F', 'G', 'H', 'J', 'K', 'L', ':', 'Z', 'X', 'C', 'V', 'B', 'N', 'M', '<', '>', '?']
-
-    current_unique_id_index = -1  # So when one is added it goes to index 0
-
-    def get_unique_id_of_length(self, length):
-        """ :returns: str; a unique id with the length 'length.' IMPORTANT: it is recommended to call
-            'self.get_unique_id' because that method will be quicker."""
-
-        random.shuffle(self.all_chs)
-        return get_string(self.all_chs[:length])
-
-    def get_unique_id(self):
-        """:returns: str; a unique identifier"""
-
-        self.current_unique_id_index += 1
-        return_value = None
-
-        if self.current_unique_id_index < len(unique_ids):
-            return_value = unique_ids[self.current_unique_id_index]
-
-        else:
-            return_value = self.get_unique_id_of_length(5)
-
-        return return_value
-
-
-id_creator = IDCreator()
+import random
+
+from game_qu.base.unique_ids_list import unique_ids
+from game_qu.base.library_independant_utility_functions import get_string
+
+
+class IDCreator:
+    """A class that creates simple unique identifiers"""
+
+    all_chs = ['1', '2', '3', '4', '5', '6', '7', '8', '9', '0', '-', '=', 'q', 'w', 'e', 'r', 't', 'y', 'u', 'i', 'o', 'p', '[', ']', 'a', 's', 'd', 'f', 'g', 'h', 'j', 'k', 'l', ';', "'", 'z', 'c', 'v', 'b', 'n', 'm', ',', '.', '/', '~', '!', '@', '#', '$', '%', '^', '&', '*', '(', ')', '_', '+', 'Q', 'W', 'E', 'R', 'T', 'Y', 'U', 'I', 'O', 'P', '{', '}', 'A', 'S', 'D', 'F', 'G', 'H', 'J', 'K', 'L', ':', 'Z', 'X', 'C', 'V', 'B', 'N', 'M', '<', '>', '?']
+
+    current_unique_id_index = -1  # So when one is added it goes to index 0
+
+    def get_unique_id_of_length(self, length):
+        """ :returns: str; a unique id with the length 'length.' IMPORTANT: it is recommended to call
+            'self.get_unique_id' because that method will be quicker."""
+
+        random.shuffle(self.all_chs)
+        return get_string(self.all_chs[:length])
+
+    def get_unique_id(self):
+        """:returns: str; a unique identifier"""
+
+        self.current_unique_id_index += 1
+        return_value = None
+
+        if self.current_unique_id_index < len(unique_ids):
+            return_value = unique_ids[self.current_unique_id_index]
+
+        else:
+            return_value = self.get_unique_id_of_length(5)
+
+        return return_value
+
+
+id_creator = IDCreator()
```

### Comparing `game_qu-2.0.0/src/game_qu/base/important_variables.py` & `game_qu-2.0.1/src/game_qu/base/important_variables.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,89 @@
-"""Holds all the important variables for the game like screen_dimensions, BACKGROUND_COLOR, etc"""
-
-from game_qu.base.library_changer import LibraryChanger
-from game_qu.base.important_constants import *
-
-if not LibraryChanger.get_library_has_been_set():
-    LibraryChanger.set_game_library(DEFAULT_RENDERING_ENGINE)
-
-from game_qu.base.keyboard import Keyboard
-from game_qu.gui_components.window import Window
-from game_qu.library_abstraction import keys
-
-keyboard = Keyboard()
-game_window = Window(SCREEN_LENGTH, SCREEN_HEIGHT, BACKGROUND_COLOR, "Game Basics")
-
-KEY_A = keys.KEY_A
-KEY_B = keys.KEY_B
-KEY_C = keys.KEY_C
-KEY_D = keys.KEY_D
-KEY_E = keys.KEY_E
-KEY_F = keys.KEY_F
-KEY_G = keys.KEY_G
-KEY_H = keys.KEY_H
-KEY_I = keys.KEY_I
-KEY_J = keys.KEY_J
-KEY_K = keys.KEY_K
-KEY_L = keys.KEY_L
-KEY_M = keys.KEY_M
-KEY_N = keys.KEY_N
-KEY_O = keys.KEY_O
-KEY_P = keys.KEY_P
-KEY_Q = keys.KEY_Q
-KEY_R = keys.KEY_R
-KEY_S = keys.KEY_S
-KEY_T = keys.KEY_T
-KEY_U = keys.KEY_U
-KEY_V = keys.KEY_V
-KEY_W = keys.KEY_W
-KEY_X = keys.KEY_X
-KEY_Y = keys.KEY_Y
-KEY_Z = keys.KEY_Z
-KEY_LEFT = keys.KEY_LEFT
-KEY_RIGHT = keys.KEY_RIGHT
-KEY_UP = keys.KEY_UP
-KEY_DOWN = keys.KEY_DOWN
-KEY_QUESTION_MARK = keys.KEY_QUESTION_MARK
-KEY_PERIOD = keys.KEY_PERIOD
-KEY_COMMA = keys.KEY_COMMA
-KEY_COLON = keys.KEY_COLON
-KEY_QUOTATION_MARKS = keys.KEY_QUOTATION_MARKS
-KEY_LEFT_BRACKET = keys.KEY_LEFT_BRACKET
-KEY_RIGHT_BRACKET = keys.KEY_RIGHT_BRACKET
-KEY_ESCAPE = keys.KEY_ESCAPE
-KEY_SLASH = keys.KEY_SLASH
-
-BUTTON_X = 0
-BUTTON_A = 0
-BUTTON_B = 0
-BUTTON_Y = 0
-BUTTON_L = 0
-BUTTON_R = 0
-BUTTON_SELECT = 0
-BUTTON_START = 0
-DPAD_UP = 0
-DPAD_DOWN = 0
-DPAD_LEFT = 0
-DPAD_RIGHT = 0
-
-if LibraryChanger.current_library_name == "pygame":
-    BUTTON_X = keys.BUTTON_X
-    BUTTON_A = keys.BUTTON_A
-    BUTTON_B = keys.BUTTON_B
-    BUTTON_Y = keys.BUTTON_Y
-    BUTTON_L = keys.BUTTON_L
-    BUTTON_R = keys.BUTTON_R
-    BUTTON_SELECT = keys.BUTTON_SELECT
-    BUTTON_START = keys.BUTTON_START
-    DPAD_UP = keys.DPAD_UP
-    DPAD_DOWN = keys.DPAD_DOWN
-    DPAD_LEFT = keys.DPAD_LEFT
+"""Holds all the important variables for the game like screen_dimensions, BACKGROUND_COLOR, etc"""
+
+from game_qu.base.library_changer import LibraryChanger
+from game_qu.base import important_constants
+
+if not LibraryChanger.get_library_has_been_set():
+    LibraryChanger.set_game_library(important_constants.DEFAULT_RENDERING_ENGINE)
+
+if important_constants.IS_FULL_SCREEN and LibraryChanger.current_library_name == "pygame":
+    import pygame
+
+    pygame.display.set_mode(flags=pygame.FULLSCREEN)
+    important_constants.SCREEN_HEIGHT = pygame.display.get_surface().get_height()
+    important_constants.SCREEN_LENGTH = pygame.display.get_surface().get_width()
+
+from game_qu.base.keyboard import Keyboard
+from game_qu.gui_components.window import Window
+from game_qu.library_abstraction import keys
+from game_qu.base.important_constants import *
+
+keyboard = Keyboard()
+game_window = Window(SCREEN_LENGTH, SCREEN_HEIGHT, BACKGROUND_COLOR, "Game Basics")
+
+KEY_A = keys.KEY_A
+KEY_B = keys.KEY_B
+KEY_C = keys.KEY_C
+KEY_D = keys.KEY_D
+KEY_E = keys.KEY_E
+KEY_F = keys.KEY_F
+KEY_G = keys.KEY_G
+KEY_H = keys.KEY_H
+KEY_I = keys.KEY_I
+KEY_J = keys.KEY_J
+KEY_K = keys.KEY_K
+KEY_L = keys.KEY_L
+KEY_M = keys.KEY_M
+KEY_N = keys.KEY_N
+KEY_O = keys.KEY_O
+KEY_P = keys.KEY_P
+KEY_Q = keys.KEY_Q
+KEY_R = keys.KEY_R
+KEY_S = keys.KEY_S
+KEY_T = keys.KEY_T
+KEY_U = keys.KEY_U
+KEY_V = keys.KEY_V
+KEY_W = keys.KEY_W
+KEY_X = keys.KEY_X
+KEY_Y = keys.KEY_Y
+KEY_Z = keys.KEY_Z
+KEY_LEFT = keys.KEY_LEFT
+KEY_RIGHT = keys.KEY_RIGHT
+KEY_UP = keys.KEY_UP
+KEY_DOWN = keys.KEY_DOWN
+KEY_QUESTION_MARK = keys.KEY_QUESTION_MARK
+KEY_PERIOD = keys.KEY_PERIOD
+KEY_COMMA = keys.KEY_COMMA
+KEY_COLON = keys.KEY_COLON
+KEY_QUOTATION_MARKS = keys.KEY_QUOTATION_MARKS
+KEY_LEFT_BRACKET = keys.KEY_LEFT_BRACKET
+KEY_RIGHT_BRACKET = keys.KEY_RIGHT_BRACKET
+KEY_ESCAPE = keys.KEY_ESCAPE
+KEY_SLASH = keys.KEY_SLASH
+
+BUTTON_X = 0
+BUTTON_A = 0
+BUTTON_B = 0
+BUTTON_Y = 0
+BUTTON_L = 0
+BUTTON_R = 0
+BUTTON_SELECT = 0
+BUTTON_START = 0
+DPAD_UP = 0
+DPAD_DOWN = 0
+DPAD_LEFT = 0
+DPAD_RIGHT = 0
+
+if LibraryChanger.current_library_name == "pygame":
+    BUTTON_X = keys.BUTTON_X
+    BUTTON_A = keys.BUTTON_A
+    BUTTON_B = keys.BUTTON_B
+    BUTTON_Y = keys.BUTTON_Y
+    BUTTON_L = keys.BUTTON_L
+    BUTTON_R = keys.BUTTON_R
+    BUTTON_SELECT = keys.BUTTON_SELECT
+    BUTTON_START = keys.BUTTON_START
+    DPAD_UP = keys.DPAD_UP
+    DPAD_DOWN = keys.DPAD_DOWN
+    DPAD_LEFT = keys.DPAD_LEFT
     DPAD_RIGHT = keys.DPAD_RIGHT
```

### Comparing `game_qu-2.0.0/src/game_qu/base/keyboard.py` & `game_qu-2.0.1/src/game_qu/base/keyboard.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-from game_qu.base.events import Event, TimedEvent
-from game_qu.library_abstraction import keys
-from game_qu.library_abstraction import utility_functions
-from game_qu.library_abstraction import variables
-from game_qu.base.important_constants import IS_USING_CONTROLLER
-from game_qu.base.library_changer import LibraryChanger
-
-
-class Keyboard:
-    """ A class that has key_events and key_timed_events that are used to find key states like how long a key was held in,
-        if a key was released, etc. Generally it is recommended to use the functions from game_qu.base/utility_functions.py
-        but the key_events and key_timed_events from this class can also be used."""
-
-    key_events = []
-    key_timed_events = []
-    button_timed_events = {}
-    button_events = {}
-    mouse_clicked_event = Event()
-
-    def __init__(self):
-        """Initializes all the key events"""
-
-        for x in range(len(keys.keys)):
-            self.key_events.append(Event())
-            self.key_timed_events.append(TimedEvent(0))
-
-        # Currently this game engine does not support controllers for pyglet
-        if LibraryChanger.current_library_name == "pygame":
-            self.create_button_events()
-
-    def create_button_events(self):
-        """Creates all the button Events and TimedEvents"""
-
-        for button in keys.buttons:
-            self.button_events[button] = Event()
-            self.button_timed_events[button] = TimedEvent(0)
-
-    def get_key_timed_event(self, key):
-        """:returns: TimedEvent; the TimedEvent associated with that key"""
-
-        return_value = None
-
-        if self.button_timed_events.get(key) is None:
-            return_value = self.key_timed_events[key]
-
-        else:
-            return_value = self.get_button_timed_event(key)
-
-        return return_value
-
-    def get_key_event(self, key):
-        """:returns: Event; the Event associated with that key"""
-
-        return_value = None
-
-        if self.button_events.get(key) is None:
-            return_value = self.key_events[key]
-
-        else:
-            return_value = self.get_button_event(key)
-
-        return return_value
-
-    def get_button_event(self, button):
-        """:returns: Event; the Event associated with that button"""
-
-        return self.button_events[button]
-
-    def get_button_timed_event(self, button):
-        """:returns: TimedEvent; the TimedEvent associated with that button"""
-
-        return self.button_timed_events[button]
-
-    def run(self):
-        """ Runs all the events in key_events and key_timed_events, so attributes about the keys can be viewed. This function
-            SHOULD NOT be called by the user and this library automatically calls it"""
-
-        self.mouse_clicked_event.run(utility_functions.mouse_was_pressed())
-
-        for key in keys.keys:
-            key_was_pressed = utility_functions.key_is_pressed(key)
-
-            self.get_key_event(key).run(key_was_pressed)
-
-            should_reset = not self.get_key_event(key).happened_last_cycle() and not key_was_pressed
-
-            self.get_key_timed_event(key).run(should_reset, key_was_pressed)
-        
-        # If no controller is hooked up, then the buttons should not be run
-        # Currently this game engine does not support controllers for pyglet
-        # TODO make this more general purpose- have it work for multiple controllers
-        if LibraryChanger.current_library_name == "pygame" and variables.joystick is not None and IS_USING_CONTROLLER:
-            self.run_buttons()
-
-    def run_buttons(self):
-        """Runs all the button events, so important information can be gotten from them"""
-
-        for button in keys.buttons:
-
-            button_was_pressed = utility_functions.button_is_pressed(button)
-
-            self.get_button_event(button).run(button_was_pressed)
-
-            should_reset = not self.get_button_event(button).happened_last_cycle() and not button_was_pressed
-
-            self.get_button_timed_event(button).run(should_reset, button_was_pressed)
-
+from game_qu.base.events import Event, TimedEvent
+from game_qu.library_abstraction import keys
+from game_qu.library_abstraction import utility_functions
+from game_qu.library_abstraction import variables
+from game_qu.base.important_constants import IS_USING_CONTROLLER
+from game_qu.base.library_changer import LibraryChanger
+
+
+class Keyboard:
+    """ A class that has key_events and key_timed_events that are used to find key states like how long a key was held in,
+        if a key was released, etc. Generally it is recommended to use the functions from game_qu.base/utility_functions.py
+        but the key_events and key_timed_events from this class can also be used."""
+
+    key_events = []
+    key_timed_events = []
+    button_timed_events = {}
+    button_events = {}
+    mouse_clicked_event = Event()
+
+    def __init__(self):
+        """Initializes all the key events"""
+
+        for x in range(len(keys.keys)):
+            self.key_events.append(Event())
+            self.key_timed_events.append(TimedEvent(0))
+
+        # Currently this game engine does not support controllers for pyglet
+        if LibraryChanger.current_library_name == "pygame":
+            self.create_button_events()
+
+    def create_button_events(self):
+        """Creates all the button Events and TimedEvents"""
+
+        for button in keys.buttons:
+            self.button_events[button] = Event()
+            self.button_timed_events[button] = TimedEvent(0)
+
+    def get_key_timed_event(self, key):
+        """:returns: TimedEvent; the TimedEvent associated with that key"""
+
+        return_value = None
+
+        if self.button_timed_events.get(key) is None:
+            return_value = self.key_timed_events[key]
+
+        else:
+            return_value = self.get_button_timed_event(key)
+
+        return return_value
+
+    def get_key_event(self, key):
+        """:returns: Event; the Event associated with that key"""
+
+        return_value = None
+
+        if self.button_events.get(key) is None:
+            return_value = self.key_events[key]
+
+        else:
+            return_value = self.get_button_event(key)
+
+        return return_value
+
+    def get_button_event(self, button):
+        """:returns: Event; the Event associated with that button"""
+
+        return self.button_events[button]
+
+    def get_button_timed_event(self, button):
+        """:returns: TimedEvent; the TimedEvent associated with that button"""
+
+        return self.button_timed_events[button]
+
+    def run(self):
+        """ Runs all the events in key_events and key_timed_events, so attributes about the keys can be viewed. This function
+            SHOULD NOT be called by the user and this library automatically calls it"""
+
+        self.mouse_clicked_event.run(utility_functions.mouse_was_pressed())
+
+        for key in keys.keys:
+            key_was_pressed = utility_functions.key_is_pressed(key)
+
+            self.get_key_event(key).run(key_was_pressed)
+
+            should_reset = not self.get_key_event(key).happened_last_cycle() and not key_was_pressed
+
+            self.get_key_timed_event(key).run(should_reset, key_was_pressed)
+        
+        # If no controller is hooked up, then the buttons should not be run
+        # Currently this game engine does not support controllers for pyglet
+        # TODO make this more general purpose- have it work for multiple controllers
+        if LibraryChanger.current_library_name == "pygame" and variables.joystick is not None and IS_USING_CONTROLLER:
+            self.run_buttons()
+
+    def run_buttons(self):
+        """Runs all the button events, so important information can be gotten from them"""
+
+        for button in keys.buttons:
+
+            button_was_pressed = utility_functions.button_is_pressed(button)
+
+            self.get_button_event(button).run(button_was_pressed)
+
+            should_reset = not self.get_button_event(button).happened_last_cycle() and not button_was_pressed
+
+            self.get_button_timed_event(button).run(should_reset, button_was_pressed)
+
```

### Comparing `game_qu-2.0.0/src/game_qu/base/library_changer.py` & `game_qu-2.0.1/src/game_qu/base/library_changer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,83 @@
-from game_qu.base import important_constants
-import importlib
-from game_qu import library_abstraction
-
-
-class LibraryChanger:
-    """ A class that allows the user to modify constants and other variables instead of actually modifying the code.
-        IMPORTANT: All the methods of this class must be called from the second line onwards with the first line being
-        from game_qu.base.library_changer import LibraryChanger, so none of the other code is initialized with the old constants."""
-
-    library_has_been_set = False
-    current_library_name = ""
-
-    @staticmethod
-    def set_screen_dimensions(screen_length, screen_height):
-            """Sets the dimensions of the screen. IMPORTANT see class description for details on how to call the methods """
-
-            important_constants.SCREEN_LENGTH = screen_length
-            important_constants.SCREEN_HEIGHT = screen_height
-
-    @staticmethod
-    def set_background_color(background_color):
-        """Sets the background color of the screen (doesn't affect anything if an image is the background)"""
-
-        important_constants.BACKGROUND_COLOR = background_color
-
-    @staticmethod
-    def set_number_of_frames_history_keeper_stores(number_of_frames_history_keeper_stores):
-        """Sets the number of frames the HistoryKeeper keeps in it at one time"""
-
-        important_constants.NUMBER_OF_FRAMES_HISTORY_KEEPER_STORES = number_of_frames_history_keeper_stores
-
-    @staticmethod
-    def set_game_library(library_name):
-        """ Sets the game library that runs all the code. Here are the valid names:
-            'pyglet',
-            'pygame'"""
-
-        valid_library_names = ["pyglet", "pygame"]
-        LibraryChanger.library_has_been_set = True
-
-        if not valid_library_names.__contains__(library_name):
-            raise ValueError(f"Do not recognize 'library_name' {library_name}. Here are the valid values: ['pyglet', 'pygame']")
-
-        if library_name == "pyglet":
-            LibraryChanger.current_library_name = library_name
-            library_abstraction.keys = importlib.import_module("game_qu.pyglet_abstraction.keys")
-            library_abstraction.utility_functions = importlib.import_module("game_qu.pyglet_abstraction.utility_functions")
-            library_abstraction.variables = importlib.import_module("game_qu.pyglet_abstraction.variables")
-
-        else:
-            LibraryChanger.current_library_name = library_name
-            library_abstraction.keys = importlib.import_module("game_qu.pygame_abstraction.keys")
-            library_abstraction.utility_functions = importlib.import_module("game_qu.pygame_abstraction.utility_functions")
-            library_abstraction.variables = importlib.import_module("game_qu.pygame_abstraction.variables")
-
-    @staticmethod
-    def get_library_has_been_set():
-        """:returns: bool; whether the library for the game engine has been set"""
-
-        return LibraryChanger.library_has_been_set
-
-    @staticmethod
-    def set_important_constant(constant_name, constant_value):
-        """Sets the value of the constant with the name 'constant_name' to 'constant_value'"""
-
-        setattr(important_constants, constant_name, constant_value)
-
-    @staticmethod
-    def set_is_using_controller(is_using_controller):
-        """Sets whether the game will be using a controller (important_constants.IS_USING_CONTROLLER) to 'is_using_controller'"""
-
-        important_constants.IS_USING_CONTROLLER = is_using_controller
+from game_qu.base import important_constants
+import importlib
+from game_qu import library_abstraction
+
+
+class LibraryChanger:
+    """ A class that allows the user to modify constants and other variables instead of actually modifying the code.
+        IMPORTANT: All the methods of this class must be called from the second line onwards with the first line being
+        from game_qu.base.library_changer import LibraryChanger, so none of the other code is initialized with the old constants."""
+
+    library_has_been_set = False
+    current_library_name = ""
+
+    @staticmethod
+    def set_screen_dimensions(screen_length, screen_height):
+            """Sets the dimensions of the screen. IMPORTANT see class description for details on how to call the methods """
+
+            important_constants.SCREEN_LENGTH = screen_length
+            important_constants.SCREEN_HEIGHT = screen_height
+
+    @staticmethod
+    def set_background_color(background_color):
+        """Sets the background color of the screen (doesn't affect anything if an image is the background)"""
+
+        important_constants.BACKGROUND_COLOR = background_color
+
+    @staticmethod
+    def set_number_of_frames_history_keeper_stores(number_of_frames_history_keeper_stores):
+        """Sets the number of frames the HistoryKeeper keeps in it at one time"""
+
+        important_constants.NUMBER_OF_FRAMES_HISTORY_KEEPER_STORES = number_of_frames_history_keeper_stores
+
+    @staticmethod
+    def set_game_library(library_name):
+        """ Sets the game library that runs all the code. Here are the valid names:
+            'pyglet',
+            'pygame'"""
+
+        valid_library_names = ["pyglet", "pygame"]
+        LibraryChanger.library_has_been_set = True
+
+        if not valid_library_names.__contains__(library_name):
+            raise ValueError(f"Do not recognize 'library_name' {library_name}. Here are the valid values: ['pyglet', 'pygame']")
+
+        if library_name == "pyglet":
+            LibraryChanger.current_library_name = library_name
+            library_abstraction.keys = importlib.import_module("game_qu.pyglet_abstraction.keys")
+            library_abstraction.utility_functions = importlib.import_module("game_qu.pyglet_abstraction.utility_functions")
+            library_abstraction.variables = importlib.import_module("game_qu.pyglet_abstraction.variables")
+
+        else:
+            LibraryChanger.current_library_name = library_name
+            library_abstraction.keys = importlib.import_module("game_qu.pygame_abstraction.keys")
+            library_abstraction.utility_functions = importlib.import_module("game_qu.pygame_abstraction.utility_functions")
+            library_abstraction.variables = importlib.import_module("game_qu.pygame_abstraction.variables")
+
+    @staticmethod
+    def get_library_has_been_set():
+        """:returns: bool; whether the library for the game engine has been set"""
+
+        return LibraryChanger.library_has_been_set
+
+    @staticmethod
+    def set_important_constant(constant_name, constant_value):
+        """Sets the value of the constant with the name 'constant_name' to 'constant_value'"""
+
+        setattr(important_constants, constant_name, constant_value)
+
+    @staticmethod
+    def set_is_using_controller(is_using_controller):
+        """Sets whether the game will be using a controller (important_constants.IS_USING_CONTROLLER) to 'is_using_controller'"""
+
+        important_constants.IS_USING_CONTROLLER = is_using_controller
+
+    @staticmethod
+    def set_full_screen(is_full_screen):
+        """Makes the size of the application full screen. NOTE: This only works with pygame"""
+
+        if LibraryChanger.current_library_name == "pygame":
+            important_constants.IS_FULL_SCREEN = is_full_screen
+
+        else:
+            raise ValueError("Setting to full screen can only be done when the game engine is pygame")
```

### Comparing `game_qu-2.0.0/src/game_qu/base/lines.py` & `game_qu-2.0.1/src/game_qu/base/lines.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-class Point:
-    """Stores the x and y coordinates of point"""
-
-    x_coordinate = 0
-    y_coordinate = 0
-
-    def __init__(self, x_coordinate, y_coordinate):
-        """ Calls set_point(), so the x_coordinate and y_coordinate can be set
-
-            :parameter x_coordinate: float; the value of the point's x coordinate
-            :parameter y_coordinate: float; the value of the point's y coordinate
-
-            :returns: None
-        """
-
-        self.set_coordinates(x_coordinate, y_coordinate)
-
-    def set_coordinates(self, x_coordinate, y_coordinate):
-        """ Sets the x_coordinate and y_coordinate can be set
-
-            :parameter x_coordinate: float; the value of the point's x coordinate
-            :parameter y_coordinate: float; the value of the point's y coordinate
-
-            :returns: None
-        """
-
-        self.x_coordinate, self.y_coordinate = x_coordinate, y_coordinate
-
-
-class LineSegment:
-    """Uses the equation y = mx + b where m is slope and b is y_intercept"""
-
-    start_point = None
-    end_point = None
-    slope = None
-    y_intercept = None
-
-    def __init__(self, start_point, end_point):
-        """ Sets the start and end point of the lines. It creates a very similar line if the x_coordinate of the start and end
-            point have the same x_coordinate by adding a very small number to the end_point's x_coordinate. This makes
-            finding where two lines collide alot easier. This function will call set_points()
-
-            :parameter start_point: Point; a point on the line (different than end_point)
-            :parameter end_point: Point; a point on the line (different than start_point)
-
-            :returns: None
-        """
-
-        self.set_points(start_point, end_point)
-
-    def set_points(self, start_point, end_point):
-        """ Sets the start and end point of the lines. It creates a very similar line if the x_coordinate of the start and end
-            point have the same x_coordinate by adding a very small number to the end_point's x_coordinate. This makes
-            finding where two lines collide alot easier.
-
-            :parameter start_point: Point; a point on the line (different than end_point)
-            :parameter end_point: Point; a point on the line (different than start_point)
-
-            :returns: None
-        """
-
-        self.start_point, self.end_point = start_point, end_point
-        self.update_line_values()
-
-    def update_line_values(self):
-        """Updates the slope (m) and y_intercept (b) of the line through calculation. Uses the equation y = mx + b"""
-
-        if self.start_point.x_coordinate == self.end_point.x_coordinate:
-            self.end_point.x_coordinate += pow(10, -9)
-
-        self.slope = (self.end_point.y_coordinate - self.start_point.y_coordinate) / (self.end_point.x_coordinate - self.start_point.x_coordinate)
-        self.y_intercept = self.start_point.y_coordinate - self.slope * self.start_point.x_coordinate
-
-    def get_y_coordinate(self, x_coordinate):
-        """:returns: float; the y_coordinate at the x_coordinate"""
-
-        return x_coordinate * self.slope + self.y_intercept
-
-    def get_x_coordinate(self, y_coordinate):
-        """:returns: float; the x_coordinate at the y_coordinate"""
-
-        return (y_coordinate - self.y_intercept) / self.slope
-
-    def contains_x_coordinate(self, x_coordinate):
-        """:returns: bool; if the LineSegment contains the x_coordinate"""
-
-        smaller_x_coordinate = self.start_point.x_coordinate if self.start_point.x_coordinate < self.end_point.x_coordinate else self.end_point.x_coordinate
-        bigger_x_coordinate = self.start_point.x_coordinate if self.start_point.x_coordinate > self.end_point.x_coordinate else self.end_point.x_coordinate
-
-        return x_coordinate >= smaller_x_coordinate and x_coordinate <= bigger_x_coordinate
-
-    def contains_y_coordinate(self, y_coordinate):
-        """:returns: bool; if the LineSegment contains the y_coordinate"""
-
-        smaller_y_coordinate = self.start_point.y_coordinate if self.start_point.y_coordinate < self.end_point.y_coordinate else self.end_point.y_coordinate
-        bigger_y_coordinate = self.start_point.y_coordinate if self.start_point.y_coordinate > self.end_point.y_coordinate else self.end_point.y_coordinate
-
-        return y_coordinate >= smaller_y_coordinate and y_coordinate <= bigger_y_coordinate
-
-    def contains_point(self, point):
-        """:returns: bool; if the LineSegment contains the x_coordinate, y_coordinate, and point"""
-
-        contains_coordinates = self.contains_x_coordinate(point.x_coordinate) and self.contains_y_coordinate(point.y_coordinate)
-        correct_y_coordinate = point.y_coordinate == self.get_y_coordinate(point.x_coordinate)
-
-        return contains_coordinates and correct_y_coordinate
-
-    def slope_is_positive(self):
-        """:returns: bool; if the slope is >= 0"""
-
-        return self.slope >= 0
+class Point:
+    """Stores the x and y coordinates of point"""
+
+    x_coordinate = 0
+    y_coordinate = 0
+
+    def __init__(self, x_coordinate, y_coordinate):
+        """ Calls set_point(), so the x_coordinate and y_coordinate can be set
+
+            :parameter x_coordinate: float; the value of the point's x coordinate
+            :parameter y_coordinate: float; the value of the point's y coordinate
+
+            :returns: None
+        """
+
+        self.set_coordinates(x_coordinate, y_coordinate)
+
+    def set_coordinates(self, x_coordinate, y_coordinate):
+        """ Sets the x_coordinate and y_coordinate can be set
+
+            :parameter x_coordinate: float; the value of the point's x coordinate
+            :parameter y_coordinate: float; the value of the point's y coordinate
+
+            :returns: None
+        """
+
+        self.x_coordinate, self.y_coordinate = x_coordinate, y_coordinate
+
+
+class LineSegment:
+    """Uses the equation y = mx + b where m is slope and b is y_intercept"""
+
+    start_point = None
+    end_point = None
+    slope = None
+    y_intercept = None
+
+    def __init__(self, start_point, end_point):
+        """ Sets the start and end point of the lines. It creates a very similar line if the x_coordinate of the start and end
+            point have the same x_coordinate by adding a very small number to the end_point's x_coordinate. This makes
+            finding where two lines collide alot easier. This function will call set_points()
+
+            :parameter start_point: Point; a point on the line (different than end_point)
+            :parameter end_point: Point; a point on the line (different than start_point)
+
+            :returns: None
+        """
+
+        self.set_points(start_point, end_point)
+
+    def set_points(self, start_point, end_point):
+        """ Sets the start and end point of the lines. It creates a very similar line if the x_coordinate of the start and end
+            point have the same x_coordinate by adding a very small number to the end_point's x_coordinate. This makes
+            finding where two lines collide alot easier.
+
+            :parameter start_point: Point; a point on the line (different than end_point)
+            :parameter end_point: Point; a point on the line (different than start_point)
+
+            :returns: None
+        """
+
+        self.start_point, self.end_point = start_point, end_point
+        self.update_line_values()
+
+    def update_line_values(self):
+        """Updates the slope (m) and y_intercept (b) of the line through calculation. Uses the equation y = mx + b"""
+
+        if self.start_point.x_coordinate == self.end_point.x_coordinate:
+            self.end_point.x_coordinate += pow(10, -9)
+
+        self.slope = (self.end_point.y_coordinate - self.start_point.y_coordinate) / (self.end_point.x_coordinate - self.start_point.x_coordinate)
+        self.y_intercept = self.start_point.y_coordinate - self.slope * self.start_point.x_coordinate
+
+    def get_y_coordinate(self, x_coordinate):
+        """:returns: float; the y_coordinate at the x_coordinate"""
+
+        return x_coordinate * self.slope + self.y_intercept
+
+    def get_x_coordinate(self, y_coordinate):
+        """:returns: float; the x_coordinate at the y_coordinate"""
+
+        return (y_coordinate - self.y_intercept) / self.slope
+
+    def contains_x_coordinate(self, x_coordinate):
+        """:returns: bool; if the LineSegment contains the x_coordinate"""
+
+        smaller_x_coordinate = self.start_point.x_coordinate if self.start_point.x_coordinate < self.end_point.x_coordinate else self.end_point.x_coordinate
+        bigger_x_coordinate = self.start_point.x_coordinate if self.start_point.x_coordinate > self.end_point.x_coordinate else self.end_point.x_coordinate
+
+        return x_coordinate >= smaller_x_coordinate and x_coordinate <= bigger_x_coordinate
+
+    def contains_y_coordinate(self, y_coordinate):
+        """:returns: bool; if the LineSegment contains the y_coordinate"""
+
+        smaller_y_coordinate = self.start_point.y_coordinate if self.start_point.y_coordinate < self.end_point.y_coordinate else self.end_point.y_coordinate
+        bigger_y_coordinate = self.start_point.y_coordinate if self.start_point.y_coordinate > self.end_point.y_coordinate else self.end_point.y_coordinate
+
+        return y_coordinate >= smaller_y_coordinate and y_coordinate <= bigger_y_coordinate
+
+    def contains_point(self, point):
+        """:returns: bool; if the LineSegment contains the x_coordinate, y_coordinate, and point"""
+
+        contains_coordinates = self.contains_x_coordinate(point.x_coordinate) and self.contains_y_coordinate(point.y_coordinate)
+        correct_y_coordinate = point.y_coordinate == self.get_y_coordinate(point.x_coordinate)
+
+        return contains_coordinates and correct_y_coordinate
+
+    def slope_is_positive(self):
+        """:returns: bool; if the slope is >= 0"""
+
+        return self.slope >= 0
```

### Comparing `game_qu-2.0.0/src/game_qu/base/paths.py` & `game_qu-2.0.1/src/game_qu/base/paths.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,255 +1,255 @@
-from game_qu.base.lines import LineSegment, Point
-from game_qu.base.utility_functions import max_value
-from game_qu.base.velocity_calculator import VelocityCalculator
-
-
-class Path:
-    """ Made up of multiple lines that are all connected. The previous point and the next point are connected by a line.
-        For instance, a line looks like: LineSegment(points[0], points[1]). IMPORTANT: no LineSegments can share the same
-        x_coordinate (besides the first x_coordinate between adjacent lines) otherwise the code won't work"""
-
-    lines = []
-    points = []
-    last_point = None
-
-    def __init__(self, start_point, other_points):
-        """Initializes the object with the start_point and other_points. This method calls add_point() for each point in other_points"""
-
-        self.lines = []
-        self.points = [start_point]
-        self.last_point = start_point
-
-        for other_point in other_points:
-            self.add_point(other_point)
-
-    def add_point(self, point):
-        """Adds the point to this path by adding a new line to the path: LineSegment('last_point', 'point')"""
-
-        self.lines.append(LineSegment(self.last_point, point))
-        self.last_point = point
-        self.points.append(point)
-
-    def get_y_coordinate(self, x_coordinate):
-        """ :returns: float; the y_coordinate at that x_coordinate. Or in other words, what the LineSegment that contains
-            the x_coordinate get_y_coordinate() method returns"""
-
-        y_coordinate = 0
-
-        for line in self.lines:
-            if line.contains_x_coordinate(x_coordinate):
-                y_coordinate = line.get_y_coordinate(x_coordinate)
-                break
-
-        return y_coordinate
-
-    def get_lines(self):
-        """:returns: LineSegment[]; the lines of this simple path"""
-
-        return self.lines
-
-    def get_first_line(self):
-        """:returns: LineSegment: the last LineSegment of the Path"""
-
-        return self.lines[0]
-
-    def get_last_line(self):
-        """:returns: LineSegment; the last LineSegment of the Path"""
-
-        last_index = len(self.lines) - 1
-        return self.lines[last_index]
-
-    def __str__(self):
-        """:returns: str; the string representation of the Path"""
-
-        string = ""
-        for x in range(len(self.lines)):
-            string += f"{self.lines[x]} || "
-
-        return string
-
-    def is_moving_down(self, x_coordinate):
-        """:returns: bool; if the slope is negative for the last line that contains this specific 'x_coordinate'"""
-
-        return_value = None
-
-        for line in self.lines:
-            if line.contains_x_coordinate(x_coordinate):
-                return_value = not line.slope_is_positive()
-
-        return return_value
-
-
-class VelocityPath:
-    """A path that takes into account velocity"""
-
-    velocity = 0
-    left_edge_lines = []
-    top_edge_lines = []
-    last_end_time = 0
-
-    times = []  # Stores the times that the get_coordinates() function was called
-    total_time = 0
-    last_point = None
-    is_unending = False
-    previous_time = 0
-
-    def __init__(self, start_point, other_points, velocity):
-        """Initializes the object"""
-
-        self.velocity = velocity
-        self.path_lines = []
-        self.left_edge_lines = []
-        self.top_edge_lines = []
-        self.times = []
-
-        self.last_point = start_point
-
-        for point in other_points:
-            self.add_point(point)
-
-    def add_point(self, point):
-        """Does some calculations to find the time from the start of the last point to the end of the parameter 'point'
-        and then calls add_time_point() to add the point"""
-
-        x_distance = abs(self.last_point.x_coordinate - point.x_coordinate)
-        y_distance = abs(self.last_point.y_coordinate - point.y_coordinate)
-
-        x_time = x_distance / self.velocity
-        y_time = y_distance / self.velocity
-
-        # Whichever one is greater is how long the object will take to travel that distance because it...
-        # can't travel faster than one of its max velocities
-        time_to_travel_distance = max_value(x_time, y_time)
-
-        end_time = time_to_travel_distance + self.last_end_time
-
-        self.add_time_point(point, end_time)
-
-    def add_time_point(self, point, end_time):
-        """Adds the point to the path using the end_time as the x_coordinate for the x and y coordinate lines"""
-
-        left_edge_line = LineSegment(Point(self.last_end_time, self.last_point.x_coordinate),
-                                     Point(end_time, point.x_coordinate))
-
-        top_edge_line = LineSegment(Point(self.last_end_time, self.last_point.y_coordinate),
-                                    Point(end_time, point.y_coordinate))
-
-        self.left_edge_lines.append(left_edge_line)
-        self.top_edge_lines.append(top_edge_line)
-        self.last_end_time = end_time
-
-        # The height for the path_line doesn't matter
-        self.last_point = point
-
-    def get_coordinates(self, should_increase_time=True):
-        """ :returns: float[2] {left_edge, top_edge}; the coordinates at the current time - also updates the current time
-            by calling 'self.update_time' if 'should_increase_time'"""
-
-        if should_increase_time:
-            self.update_time()
-
-        return self.get_coordinates_at_time(self.total_time)
-
-    def update_time(self):
-        """Updates the time variables for this object by the time the last game tick took"""
-
-        # The time should only be increased if it was not called that cycle
-        if self.previous_time != VelocityCalculator.time:
-            self.total_time += VelocityCalculator.time
-            self.previous_time = VelocityCalculator.time
-
-        max_time = self.last_end_time
-
-        if self.total_time > max_time and self.is_unending:
-            self.total_time %= max_time
-
-    def get_coordinates_at_time(self, time):
-        """:returns: float[] {left_edge, top_edge}; the coordinates at that time"""
-
-        index = self.get_index_of_line(time)
-        left_edge_line = self.left_edge_lines[index]
-        top_edge_line = self.top_edge_lines[index]
-
-        return [left_edge_line.get_y_coordinate(time), top_edge_line.get_y_coordinate(time)]
-
-    def get_index_of_line(self, time):
-        """:returns: int; the index of the line that the path is currently on"""
-
-        return_value = len(self.left_edge_lines) - 1
-
-        for x in range(len(self.top_edge_lines)):
-            top_edge_line: LineSegment = self.top_edge_lines[x]
-            start_point = top_edge_line.start_point
-            end_point = top_edge_line.end_point
-
-            if time >= start_point.x_coordinate and time <= end_point.x_coordinate:
-                return_value = x
-
-        return return_value
-
-    def set_time(self, time):
-        """Sets the time to the provided 'time'- if it is greater than the max time it is reduced to a smaller time"""
-
-        self.total_time = time % self.max_time
-
-    @property
-    def max_time(self):
-        return self.last_end_time
-
-    def __str__(self):
-        string = ""
-        for x in range(len(self.top_edge_lines)):
-            top_edge_line = self.top_edge_lines[x]
-            left_edge_line = self.left_edge_lines[x]
-
-            string += f"x {left_edge_line}, y {top_edge_line}\n"
-
-        return string
-
-
-class ActionPath(VelocityPath):
-    """A path that performs an action at each of the points"""
-
-    actions = []
-    is_unending = True
-    index_of_last_line = None
-    object_on_path = None
-
-    def __init__(self, start_point, object_on_path, velocity):
-        """Initializes the object"""
-
-        super().__init__(start_point, [], velocity)
-        self.object_on_path = object_on_path
-        self.actions = []
-
-    def add_point(self, point, action, additional_time=None):
-        """Adds the point to the action path"""
-
-        if additional_time is None:
-            super().add_point(point)
-
-        if additional_time is not None:
-            super().add_time_point(point, self.last_end_time + additional_time)
-
-        self.actions.append(action)
-
-    def run(self):
-        """Runs all the code for the action path"""
-
-        new_index = self.get_index_of_line(self.total_time % self.max_time)
-
-        if new_index != self.index_of_last_line:
-            self.index_of_last_line = new_index
-            self.actions[new_index]()
-
-        self.object_on_path.left_edge, self.object_on_path.top_edge = self.get_coordinates()
-
-    def update_for_side_scrolling(self, amount):
-        """Updates the Path, so side scrolling doesn't cause any issues"""
-
-        for left_edge_line in self.left_edge_lines:
-            # The y_coordinate for the left_edge_line is the 'left_edge' and the x_coordinate is 'time'
-            left_edge_line.start_point.y_coordinate -= amount
-            left_edge_line.end_point.y_coordinate -= amount
-
-            left_edge_line.update_line_values()
+from game_qu.base.lines import LineSegment, Point
+from game_qu.base.utility_functions import max_value
+from game_qu.base.velocity_calculator import VelocityCalculator
+
+
+class Path:
+    """ Made up of multiple lines that are all connected. The previous point and the next point are connected by a line.
+        For instance, a line looks like: LineSegment(points[0], points[1]). IMPORTANT: no LineSegments can share the same
+        x_coordinate (besides the first x_coordinate between adjacent lines) otherwise the code won't work"""
+
+    lines = []
+    points = []
+    last_point = None
+
+    def __init__(self, start_point, other_points):
+        """Initializes the object with the start_point and other_points. This method calls add_point() for each point in other_points"""
+
+        self.lines = []
+        self.points = [start_point]
+        self.last_point = start_point
+
+        for other_point in other_points:
+            self.add_point(other_point)
+
+    def add_point(self, point):
+        """Adds the point to this path by adding a new line to the path: LineSegment('last_point', 'point')"""
+
+        self.lines.append(LineSegment(self.last_point, point))
+        self.last_point = point
+        self.points.append(point)
+
+    def get_y_coordinate(self, x_coordinate):
+        """ :returns: float; the y_coordinate at that x_coordinate. Or in other words, what the LineSegment that contains
+            the x_coordinate get_y_coordinate() method returns"""
+
+        y_coordinate = 0
+
+        for line in self.lines:
+            if line.contains_x_coordinate(x_coordinate):
+                y_coordinate = line.get_y_coordinate(x_coordinate)
+                break
+
+        return y_coordinate
+
+    def get_lines(self):
+        """:returns: LineSegment[]; the lines of this simple path"""
+
+        return self.lines
+
+    def get_first_line(self):
+        """:returns: LineSegment: the last LineSegment of the Path"""
+
+        return self.lines[0]
+
+    def get_last_line(self):
+        """:returns: LineSegment; the last LineSegment of the Path"""
+
+        last_index = len(self.lines) - 1
+        return self.lines[last_index]
+
+    def __str__(self):
+        """:returns: str; the string representation of the Path"""
+
+        string = ""
+        for x in range(len(self.lines)):
+            string += f"{self.lines[x]} || "
+
+        return string
+
+    def is_moving_down(self, x_coordinate):
+        """:returns: bool; if the slope is negative for the last line that contains this specific 'x_coordinate'"""
+
+        return_value = None
+
+        for line in self.lines:
+            if line.contains_x_coordinate(x_coordinate):
+                return_value = not line.slope_is_positive()
+
+        return return_value
+
+
+class VelocityPath:
+    """A path that takes into account velocity"""
+
+    velocity = 0
+    left_edge_lines = []
+    top_edge_lines = []
+    last_end_time = 0
+
+    times = []  # Stores the times that the get_coordinates() function was called
+    total_time = 0
+    last_point = None
+    is_unending = False
+    previous_time = 0
+
+    def __init__(self, start_point, other_points, velocity):
+        """Initializes the object"""
+
+        self.velocity = velocity
+        self.path_lines = []
+        self.left_edge_lines = []
+        self.top_edge_lines = []
+        self.times = []
+
+        self.last_point = start_point
+
+        for point in other_points:
+            self.add_point(point)
+
+    def add_point(self, point):
+        """Does some calculations to find the time from the start of the last point to the end of the parameter 'point'
+        and then calls add_time_point() to add the point"""
+
+        x_distance = abs(self.last_point.x_coordinate - point.x_coordinate)
+        y_distance = abs(self.last_point.y_coordinate - point.y_coordinate)
+
+        x_time = x_distance / self.velocity
+        y_time = y_distance / self.velocity
+
+        # Whichever one is greater is how long the object will take to travel that distance because it...
+        # can't travel faster than one of its max velocities
+        time_to_travel_distance = max_value(x_time, y_time)
+
+        end_time = time_to_travel_distance + self.last_end_time
+
+        self.add_time_point(point, end_time)
+
+    def add_time_point(self, point, end_time):
+        """Adds the point to the path using the end_time as the x_coordinate for the x and y coordinate lines"""
+
+        left_edge_line = LineSegment(Point(self.last_end_time, self.last_point.x_coordinate),
+                                     Point(end_time, point.x_coordinate))
+
+        top_edge_line = LineSegment(Point(self.last_end_time, self.last_point.y_coordinate),
+                                    Point(end_time, point.y_coordinate))
+
+        self.left_edge_lines.append(left_edge_line)
+        self.top_edge_lines.append(top_edge_line)
+        self.last_end_time = end_time
+
+        # The height for the path_line doesn't matter
+        self.last_point = point
+
+    def get_coordinates(self, should_increase_time=True):
+        """ :returns: float[2] {left_edge, top_edge}; the coordinates at the current time - also updates the current time
+            by calling 'self.update_time' if 'should_increase_time'"""
+
+        if should_increase_time:
+            self.update_time()
+
+        return self.get_coordinates_at_time(self.total_time)
+
+    def update_time(self):
+        """Updates the time variables for this object by the time the last game tick took"""
+
+        # The time should only be increased if it was not called that cycle
+        if self.previous_time != VelocityCalculator.time:
+            self.total_time += VelocityCalculator.time
+            self.previous_time = VelocityCalculator.time
+
+        max_time = self.last_end_time
+
+        if self.total_time > max_time and self.is_unending:
+            self.total_time %= max_time
+
+    def get_coordinates_at_time(self, time):
+        """:returns: float[] {left_edge, top_edge}; the coordinates at that time"""
+
+        index = self.get_index_of_line(time)
+        left_edge_line = self.left_edge_lines[index]
+        top_edge_line = self.top_edge_lines[index]
+
+        return [left_edge_line.get_y_coordinate(time), top_edge_line.get_y_coordinate(time)]
+
+    def get_index_of_line(self, time):
+        """:returns: int; the index of the line that the path is currently on"""
+
+        return_value = len(self.left_edge_lines) - 1
+
+        for x in range(len(self.top_edge_lines)):
+            top_edge_line: LineSegment = self.top_edge_lines[x]
+            start_point = top_edge_line.start_point
+            end_point = top_edge_line.end_point
+
+            if time >= start_point.x_coordinate and time <= end_point.x_coordinate:
+                return_value = x
+
+        return return_value
+
+    def set_time(self, time):
+        """Sets the time to the provided 'time'- if it is greater than the max time it is reduced to a smaller time"""
+
+        self.total_time = time % self.max_time
+
+    @property
+    def max_time(self):
+        return self.last_end_time
+
+    def __str__(self):
+        string = ""
+        for x in range(len(self.top_edge_lines)):
+            top_edge_line = self.top_edge_lines[x]
+            left_edge_line = self.left_edge_lines[x]
+
+            string += f"x {left_edge_line}, y {top_edge_line}\n"
+
+        return string
+
+
+class ActionPath(VelocityPath):
+    """A path that performs an action at each of the points"""
+
+    actions = []
+    is_unending = True
+    index_of_last_line = None
+    object_on_path = None
+
+    def __init__(self, start_point, object_on_path, velocity):
+        """Initializes the object"""
+
+        super().__init__(start_point, [], velocity)
+        self.object_on_path = object_on_path
+        self.actions = []
+
+    def add_point(self, point, action, additional_time=None):
+        """Adds the point to the action path"""
+
+        if additional_time is None:
+            super().add_point(point)
+
+        if additional_time is not None:
+            super().add_time_point(point, self.last_end_time + additional_time)
+
+        self.actions.append(action)
+
+    def run(self):
+        """Runs all the code for the action path"""
+
+        new_index = self.get_index_of_line(self.total_time % self.max_time)
+
+        if new_index != self.index_of_last_line:
+            self.index_of_last_line = new_index
+            self.actions[new_index]()
+
+        self.object_on_path.left_edge, self.object_on_path.top_edge = self.get_coordinates()
+
+    def update_for_side_scrolling(self, amount):
+        """Updates the Path, so side scrolling doesn't cause any issues"""
+
+        for left_edge_line in self.left_edge_lines:
+            # The y_coordinate for the left_edge_line is the 'left_edge' and the x_coordinate is 'time'
+            left_edge_line.start_point.y_coordinate -= amount
+            left_edge_line.end_point.y_coordinate -= amount
+
+            left_edge_line.update_line_values()
```

### Comparing `game_qu-2.0.0/src/game_qu/base/quadratic_equations.py` & `game_qu-2.0.1/src/game_qu/base/quadratic_equations.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,314 +1,314 @@
-from game_qu.base.important_variables import SCREEN_HEIGHT
-from game_qu.base.utility_functions import get_kwarg_item, solve_quadratic
-from game_qu.base.velocity_calculator import VelocityCalculator
-
-
-class QuadraticEquation:
-    """A class that defines the necessary variables for a quadratic ax^2 + bx + c"""
-    h = 0
-    k = 0
-    a = 0
-
-    def set_variables(self, h, k, a):
-        """ Sets the variables to the numbers to equation: a(x-h)^2 + k
-
-            :parameter h: float; the first number of the vertex
-            :parameter k: float; the second number of the vertex
-            :parameter a: float; the number that goes before (x-h)^2
-
-            :returns: None
-        """
-
-        self.h = h
-        self.k = k
-        self.a = a
-
-    def get_number(self, x):
-        """ Finds the number by plugging x into the equation ax^2 + bx + c
-
-            :parameter x: float; the variable x that will be used to get the number
-
-            :returns: float; the number that is gotten when x is plugged into the equation
-        """
-
-        return self.a * pow((x - self.h), 2) + self.k
-
-    def points_set_variables(self, vertex, other_point):
-        """ Sets the variables based on both points
-
-            :parameter vertex: Point; the vertex of the quadratic equation
-            :parameter other_point: Point; another point besides the vertex
-
-            :returns: None
-        """
-
-        self.h = vertex.x_coordinate
-        self.k = vertex.y_coordinate
-
-        # Figured this out using algebra
-        self.a = (other_point.y_coordinate - self.k) / pow((other_point.x_coordinate - self.h), 2)
-
-
-class PhysicsEquation:
-    """A class that uses common physics equations for initial_velocity, acceleration, and initial_distance"""
-
-    acceleration = 0
-    initial_velocity = 0
-    initial_distance = 0
-
-    def get_time_to_vertex(self):
-        """ Gets the time it takes to reach the vertex knowing that the final initial_velocity is 0, so the time is -initial_velocity / acceleration
-
-            :returns: float; the time to reach the vertex
-        """
-
-        return -self.initial_velocity / self.acceleration
-
-    def set_acceleration_with_displacement(self, time, displacement):
-        """ Sets the acceleration knowing that d = 1/2 * a * t^2 where d is displacement, a is acceleration, and t is time
-
-            :parameter time: float; the amount of time that it should take to go that amount (displacement)
-            :parameter displacement: float; the distance (up being positive and down being negative) that it should travel
-
-            :returns: None
-        """
-
-        self.acceleration = (2 * displacement) / pow(time, 2)
-
-    def set_acceleration_with_velocity(self, time, velocity_change):
-        """Sets the acceleration knowing that vf = vi + at"""
-
-        self.acceleration = velocity_change / time
-
-    def set_all_variables(self, vertex, time, initial_distance):
-        """ Sets all the variables; calls set_velocity and set_gravity_acceleration
-
-            :parameter vertex: float; the highest/lowest point of the parabola
-            :parameter time: float; the time it takes to get to the vertex/go the acceleration_distance
-            :parameter acceleration_displacement: float; the distance (up being positive and down being negative) that the acceleration in that time
-            :parameter initial_distance: float; the initial distance
-
-            :returns: None
-        """
-
-        self.initial_distance = initial_distance
-
-        # Gotten using math
-        self.initial_velocity = (-2 * initial_distance + 2 * vertex) / time
-        self.acceleration = 2 * (initial_distance - vertex) / pow(time, 2)
-
-    def set_variables(self, **kwargs):
-        """ Sets the variables to the number provided
-
-            possible parameters:
-                acceleration: float; the acceleration (can be positive or negative) | a in 1/2 * ax^2 + bx + c
-                initial_velocity: float; the initial_velocity (can be positive or negative) | b in 1/2 * ax^2 + bx + c
-                initial_distance: float; the starting point (can be positive or negative) | c in 1/2 * ax^2 + bx + c
-
-            :returns: None
-        """
-
-        self.acceleration = get_kwarg_item(kwargs, "acceleration", self.acceleration)
-        self.initial_velocity = get_kwarg_item(kwargs, "initial_velocity", self.initial_velocity)
-        self.initial_distance = get_kwarg_item(kwargs, "initial_distance", self.initial_distance)
-
-    def get_distance(self, time):
-        """ Finds the number by plugging x into the equation 1/2 * at^2 + vt + d
-            where a is acceleration, t is time, v is initial_velocity, and d is initial_distance
-
-            :parameter time: float; the amount of time that has passed
-
-            :returns: float; the number that is gotten when time is plugged into the equation
-        """
-        return 1 / 2 * self.acceleration * pow(time, 2) + self.initial_velocity * time + self.initial_distance
-
-    def get_velocity_using_time(self, time):
-        """ Uses the fact that the initial_velocity is equal to vi - at^2 where vi is the initial initial_velocity, a is acceleration, and t is time
-            to find the initial_velocity
-
-            :parameter time: float; the amount of time that the initial_velocity has been affected by acceleration
-
-            :returns: float; the initial_velocity after affected by acceleration
-        """
-
-        return self.initial_velocity + self.acceleration * time
-
-    def get_velocity_using_displacement(self, displacement):
-        """ Uses the formula vf^2 = vi^2 + 2ax to find the initial_velocity
-            where vf is final initial_velocity, vi is initial initial_velocity, a is acceleration, and x is displacement
-
-            :parameter displacement: float; the amount that the ball has traveled (upwards is positive and downwards is negative)
-
-            :returns: float; the final initial_velocity
-        """
-
-        final_velocity_squared = pow(self.initial_velocity, 2) + 2 * self.acceleration * displacement
-        # Reduces the risk of a rounding error like -1*e^-15 would cause an imaginary number exception
-        return pow(int(final_velocity_squared), 1 / 2)
-
-    def get_vertex(self):
-        """:returns: float; the vertex of this physics equation"""
-
-        return self.get_distance(self.get_time_to_vertex())
-
-    def get_times_to_point(self, distance):
-        """ Finds the number by plugging in 'distance' into the equation 1/2 * at^2 + vt + d
-            where a is acceleration, t is time, v is initial_velocity, and d is initial_distance
-
-            :parameter distance: float; the distance that is wanted
-
-            :returns: float[]; the times that the parabola is at that y coordinate
-        """
-        return solve_quadratic(1 / 2 * self.acceleration, self.initial_velocity, self.initial_distance - distance)
-
-    def get_full_cycle_time(self):
-        """:returns: float; the amount of time it takes the parabola to go from start_location -> start_location"""
-
-        return self.get_time_to_vertex() * 2
-
-    def __str__(self):
-        return f"[{self.acceleration},{self.initial_velocity},{self.initial_distance},]"
-
-    def __eq__(self, other):
-        return (self.acceleration == other.acceleration and self.initial_velocity == other.initial_velocity and
-                self.initial_distance == other.initial_distance)
-
-
-class PhysicsPath(PhysicsEquation):
-    """An extension of physics equation that allows for automatically changing the player's coordinates"""
-
-    game_object = None
-    current_time = 0
-    is_started = False
-    attribute_modifying = None
-    height_of_path = 0
-    time = 0
-    max_time = 0
-    last_time = 0
-    has_max_time = False
-    all_distance = 0
-    last_delta_time = 0
-
-    # def __init__(self, game_object=None, attribute_modifying="", height_of_path=0, initial_distance=0, time=.5):
-    def __init__(self, **kwargs):
-        """ Initializes the object
-
-            :parameter game_object: GameObject; the game object that is following this path
-            :parameter attribute_modifying: String; the name of the attribute this path is modifying
-            :parameter time: float; the time to the vertex of the path
-            :parameter height_of_path: float; the difference between the initial distance and the vertex of the path
-            :parameter max_time: float; the max time of the path - the time the path should end
-
-            :returns: None
-        """
-
-        self.game_object = get_kwarg_item(kwargs, "game_object", None)
-        self.attribute_modifying = get_kwarg_item(kwargs, "attribute_modifying", "")
-        self.time, self.height_of_path = get_kwarg_item(kwargs, "time", .5), get_kwarg_item(kwargs, "height_of_path", 0)
-        self.initial_distance, self.max_time = get_kwarg_item(kwargs, "initial_distance", 0), get_kwarg_item(kwargs,
-                                                                                                             "max_time",
-                                                                                                             0)
-        self.has_max_time = kwargs.get("max_time") is not None
-
-        # Adding the initial_distance, so it that is the height of the parabola
-        self.set_all_variables(self.height_of_path + self.initial_distance, self.time, self.initial_distance)
-
-    def run(self, is_reset_event, is_start_event, is_using_everything=False, is_changing_coordinates=True):
-        """ Runs the code for the game_object following the physics path
-
-            :parameter is_reset_event: bool; if True it will call reset()
-            :parameter is_start_event: bool; if True it will call start()
-            :parameter is_using_everything: bool; if True it will use both velocity and acceleration and if False will just use velocity
-
-            :returns: None
-        """
-
-        self.last_time = self.current_time
-
-        # It should not be started again if it has already been started because starting puts the current_time back to 0
-        if is_start_event and not self.is_started:
-            self.start()
-
-        if is_reset_event:
-            self.reset()
-
-        if self.is_started:
-            self.current_time += VelocityCalculator.time
-
-        can_change_coordinates = self.is_started and self.game_object is not None
-
-        should_change_player_coordinates = can_change_coordinates and is_changing_coordinates
-
-        self.last_delta_time = self.current_time - self.last_time
-
-        # Decides if it is just using the velocity or both velocity and acceleration
-        if should_change_player_coordinates and not is_using_everything:
-            self.game_object.__dict__[self.attribute_modifying] += self.get_velocity_displacement()
-
-        elif should_change_player_coordinates:
-            self.game_object.__dict__[self.attribute_modifying] = self.get_distance(self.current_time)
-
-    def start(self):
-        """Starts the physics path"""
-
-        self.is_started = True
-        self.current_time = 0
-
-    def reset(self):
-        """Ends and reset the physics path"""
-
-        self.is_started = False
-        self.current_time = 0
-        self.last_time = 0
-
-    def set_initial_distance(self, initial_distance):
-        """Sets the initial distance, so the height of the parabola is equal to the vertex"""
-
-        self.initial_distance = initial_distance
-        self.set_all_variables(self.initial_distance + self.height_of_path, self.time, self.initial_distance)
-
-    def get_velocity_displacement(self):
-        """:returns: float; the displacement from velocity (the last_time - start_time)"""
-
-        current_distance = self.initial_velocity * self.current_time
-        last_distance = self.initial_velocity * self.last_time
-
-        return current_distance - last_distance
-
-    def get_acceleration_displacement(self):
-        """:returns: float; the distance from acceleration with gravity"""
-
-        current_distance = 1 / 2 * self.acceleration * pow(self.current_time, 2)
-        last_distance = 1 / 2 * self.acceleration * pow(self.last_time, 2)
-
-        return current_distance - last_distance
-
-    def get_total_displacement(self):
-        """:returns: float; the displacement from both velocity and acceleration"""
-
-        return self.get_velocity_displacement() + self.get_acceleration_displacement()
-
-    def get_acceleration_displacement_from_time(self, time):
-        """:returns: float; the displacement from acceleration at that time"""
-
-        return 1 / 2 * self.acceleration * pow(time, 2)
-
-    def get_final_velocity(self):
-        """:returns: float; the velocity from acceleration (assumes initial_velocity is 0)"""
-
-        return self.acceleration * self.current_time
-
-    def is_done(self, should_reset=False):
-        """:returns: bool; if the path is finished (and if 'should_reset' it will reset it)"""
-
-        return_value = self.current_time >= self.max_time and self.has_max_time
-
-        if should_reset and return_value:
-            self.reset()
-
-        return return_value
-
-    def has_finished(self):
-        """:returns: bool; if the path has either not started or is done"""
-
-        return not self.is_started or self.is_done()
+from game_qu.base.important_variables import SCREEN_HEIGHT
+from game_qu.base.utility_functions import get_kwarg_item, solve_quadratic
+from game_qu.base.velocity_calculator import VelocityCalculator
+
+
+class QuadraticEquation:
+    """A class that defines the necessary variables for a quadratic ax^2 + bx + c"""
+    h = 0
+    k = 0
+    a = 0
+
+    def set_variables(self, h, k, a):
+        """ Sets the variables to the numbers to equation: a(x-h)^2 + k
+
+            :parameter h: float; the first number of the vertex
+            :parameter k: float; the second number of the vertex
+            :parameter a: float; the number that goes before (x-h)^2
+
+            :returns: None
+        """
+
+        self.h = h
+        self.k = k
+        self.a = a
+
+    def get_number(self, x):
+        """ Finds the number by plugging x into the equation ax^2 + bx + c
+
+            :parameter x: float; the variable x that will be used to get the number
+
+            :returns: float; the number that is gotten when x is plugged into the equation
+        """
+
+        return self.a * pow((x - self.h), 2) + self.k
+
+    def points_set_variables(self, vertex, other_point):
+        """ Sets the variables based on both points
+
+            :parameter vertex: Point; the vertex of the quadratic equation
+            :parameter other_point: Point; another point besides the vertex
+
+            :returns: None
+        """
+
+        self.h = vertex.x_coordinate
+        self.k = vertex.y_coordinate
+
+        # Figured this out using algebra
+        self.a = (other_point.y_coordinate - self.k) / pow((other_point.x_coordinate - self.h), 2)
+
+
+class PhysicsEquation:
+    """A class that uses common physics equations for initial_velocity, acceleration, and initial_distance"""
+
+    acceleration = 0
+    initial_velocity = 0
+    initial_distance = 0
+
+    def get_time_to_vertex(self):
+        """ Gets the time it takes to reach the vertex knowing that the final initial_velocity is 0, so the time is -initial_velocity / acceleration
+
+            :returns: float; the time to reach the vertex
+        """
+
+        return -self.initial_velocity / self.acceleration
+
+    def set_acceleration_with_displacement(self, time, displacement):
+        """ Sets the acceleration knowing that d = 1/2 * a * t^2 where d is displacement, a is acceleration, and t is time
+
+            :parameter time: float; the amount of time that it should take to go that amount (displacement)
+            :parameter displacement: float; the distance (up being positive and down being negative) that it should travel
+
+            :returns: None
+        """
+
+        self.acceleration = (2 * displacement) / pow(time, 2)
+
+    def set_acceleration_with_velocity(self, time, velocity_change):
+        """Sets the acceleration knowing that vf = vi + at"""
+
+        self.acceleration = velocity_change / time
+
+    def set_all_variables(self, vertex, time, initial_distance):
+        """ Sets all the variables; calls set_velocity and set_gravity_acceleration
+
+            :parameter vertex: float; the highest/lowest point of the parabola
+            :parameter time: float; the time it takes to get to the vertex/go the acceleration_distance
+            :parameter acceleration_displacement: float; the distance (up being positive and down being negative) that the acceleration in that time
+            :parameter initial_distance: float; the initial distance
+
+            :returns: None
+        """
+
+        self.initial_distance = initial_distance
+
+        # Gotten using math
+        self.initial_velocity = (-2 * initial_distance + 2 * vertex) / time
+        self.acceleration = 2 * (initial_distance - vertex) / pow(time, 2)
+
+    def set_variables(self, **kwargs):
+        """ Sets the variables to the number provided
+
+            possible parameters:
+                acceleration: float; the acceleration (can be positive or negative) | a in 1/2 * ax^2 + bx + c
+                initial_velocity: float; the initial_velocity (can be positive or negative) | b in 1/2 * ax^2 + bx + c
+                initial_distance: float; the starting point (can be positive or negative) | c in 1/2 * ax^2 + bx + c
+
+            :returns: None
+        """
+
+        self.acceleration = get_kwarg_item(kwargs, "acceleration", self.acceleration)
+        self.initial_velocity = get_kwarg_item(kwargs, "initial_velocity", self.initial_velocity)
+        self.initial_distance = get_kwarg_item(kwargs, "initial_distance", self.initial_distance)
+
+    def get_distance(self, time):
+        """ Finds the number by plugging x into the equation 1/2 * at^2 + vt + d
+            where a is acceleration, t is time, v is initial_velocity, and d is initial_distance
+
+            :parameter time: float; the amount of time that has passed
+
+            :returns: float; the number that is gotten when time is plugged into the equation
+        """
+        return 1 / 2 * self.acceleration * pow(time, 2) + self.initial_velocity * time + self.initial_distance
+
+    def get_velocity_using_time(self, time):
+        """ Uses the fact that the initial_velocity is equal to vi - at^2 where vi is the initial initial_velocity, a is acceleration, and t is time
+            to find the initial_velocity
+
+            :parameter time: float; the amount of time that the initial_velocity has been affected by acceleration
+
+            :returns: float; the initial_velocity after affected by acceleration
+        """
+
+        return self.initial_velocity + self.acceleration * time
+
+    def get_velocity_using_displacement(self, displacement):
+        """ Uses the formula vf^2 = vi^2 + 2ax to find the initial_velocity
+            where vf is final initial_velocity, vi is initial initial_velocity, a is acceleration, and x is displacement
+
+            :parameter displacement: float; the amount that the ball has traveled (upwards is positive and downwards is negative)
+
+            :returns: float; the final initial_velocity
+        """
+
+        final_velocity_squared = pow(self.initial_velocity, 2) + 2 * self.acceleration * displacement
+        # Reduces the risk of a rounding error like -1*e^-15 would cause an imaginary number exception
+        return pow(int(final_velocity_squared), 1 / 2)
+
+    def get_vertex(self):
+        """:returns: float; the vertex of this physics equation"""
+
+        return self.get_distance(self.get_time_to_vertex())
+
+    def get_times_to_point(self, distance):
+        """ Finds the number by plugging in 'distance' into the equation 1/2 * at^2 + vt + d
+            where a is acceleration, t is time, v is initial_velocity, and d is initial_distance
+
+            :parameter distance: float; the distance that is wanted
+
+            :returns: float[]; the times that the parabola is at that y coordinate
+        """
+        return solve_quadratic(1 / 2 * self.acceleration, self.initial_velocity, self.initial_distance - distance)
+
+    def get_full_cycle_time(self):
+        """:returns: float; the amount of time it takes the parabola to go from start_location -> start_location"""
+
+        return self.get_time_to_vertex() * 2
+
+    def __str__(self):
+        return f"[{self.acceleration},{self.initial_velocity},{self.initial_distance},]"
+
+    def __eq__(self, other):
+        return (self.acceleration == other.acceleration and self.initial_velocity == other.initial_velocity and
+                self.initial_distance == other.initial_distance)
+
+
+class PhysicsPath(PhysicsEquation):
+    """An extension of physics equation that allows for automatically changing the player's coordinates"""
+
+    game_object = None
+    current_time = 0
+    is_started = False
+    attribute_modifying = None
+    height_of_path = 0
+    time = 0
+    max_time = 0
+    last_time = 0
+    has_max_time = False
+    all_distance = 0
+    last_delta_time = 0
+
+    # def __init__(self, game_object=None, attribute_modifying="", height_of_path=0, initial_distance=0, time=.5):
+    def __init__(self, **kwargs):
+        """ Initializes the object
+
+            :parameter game_object: GameObject; the game object that is following this path
+            :parameter attribute_modifying: String; the name of the attribute this path is modifying
+            :parameter time: float; the time to the vertex of the path
+            :parameter height_of_path: float; the difference between the initial distance and the vertex of the path
+            :parameter max_time: float; the max time of the path - the time the path should end
+
+            :returns: None
+        """
+
+        self.game_object = get_kwarg_item(kwargs, "game_object", None)
+        self.attribute_modifying = get_kwarg_item(kwargs, "attribute_modifying", "")
+        self.time, self.height_of_path = get_kwarg_item(kwargs, "time", .5), get_kwarg_item(kwargs, "height_of_path", 0)
+        self.initial_distance, self.max_time = get_kwarg_item(kwargs, "initial_distance", 0), get_kwarg_item(kwargs,
+                                                                                                             "max_time",
+                                                                                                             0)
+        self.has_max_time = kwargs.get("max_time") is not None
+
+        # Adding the initial_distance, so it that is the height of the parabola
+        self.set_all_variables(self.height_of_path + self.initial_distance, self.time, self.initial_distance)
+
+    def run(self, is_reset_event, is_start_event, is_using_everything=False, is_changing_coordinates=True):
+        """ Runs the code for the game_object following the physics path
+
+            :parameter is_reset_event: bool; if True it will call reset()
+            :parameter is_start_event: bool; if True it will call start()
+            :parameter is_using_everything: bool; if True it will use both velocity and acceleration and if False will just use velocity
+
+            :returns: None
+        """
+
+        self.last_time = self.current_time
+
+        # It should not be started again if it has already been started because starting puts the current_time back to 0
+        if is_start_event and not self.is_started:
+            self.start()
+
+        if is_reset_event:
+            self.reset()
+
+        if self.is_started:
+            self.current_time += VelocityCalculator.time
+
+        can_change_coordinates = self.is_started and self.game_object is not None
+
+        should_change_player_coordinates = can_change_coordinates and is_changing_coordinates
+
+        self.last_delta_time = self.current_time - self.last_time
+
+        # Decides if it is just using the velocity or both velocity and acceleration
+        if should_change_player_coordinates and not is_using_everything:
+            self.game_object.__dict__[self.attribute_modifying] += self.get_velocity_displacement()
+
+        elif should_change_player_coordinates:
+            self.game_object.__dict__[self.attribute_modifying] = self.get_distance(self.current_time)
+
+    def start(self):
+        """Starts the physics path"""
+
+        self.is_started = True
+        self.current_time = 0
+
+    def reset(self):
+        """Ends and reset the physics path"""
+
+        self.is_started = False
+        self.current_time = 0
+        self.last_time = 0
+
+    def set_initial_distance(self, initial_distance):
+        """Sets the initial distance, so the height of the parabola is equal to the vertex"""
+
+        self.initial_distance = initial_distance
+        self.set_all_variables(self.initial_distance + self.height_of_path, self.time, self.initial_distance)
+
+    def get_velocity_displacement(self):
+        """:returns: float; the displacement from velocity (the last_time - start_time)"""
+
+        current_distance = self.initial_velocity * self.current_time
+        last_distance = self.initial_velocity * self.last_time
+
+        return current_distance - last_distance
+
+    def get_acceleration_displacement(self):
+        """:returns: float; the distance from acceleration with gravity"""
+
+        current_distance = 1 / 2 * self.acceleration * pow(self.current_time, 2)
+        last_distance = 1 / 2 * self.acceleration * pow(self.last_time, 2)
+
+        return current_distance - last_distance
+
+    def get_total_displacement(self):
+        """:returns: float; the displacement from both velocity and acceleration"""
+
+        return self.get_velocity_displacement() + self.get_acceleration_displacement()
+
+    def get_acceleration_displacement_from_time(self, time):
+        """:returns: float; the displacement from acceleration at that time"""
+
+        return 1 / 2 * self.acceleration * pow(time, 2)
+
+    def get_final_velocity(self):
+        """:returns: float; the velocity from acceleration (assumes initial_velocity is 0)"""
+
+        return self.acceleration * self.current_time
+
+    def is_done(self, should_reset=False):
+        """:returns: bool; if the path is finished (and if 'should_reset' it will reset it)"""
+
+        return_value = self.current_time >= self.max_time and self.has_max_time
+
+        if should_reset and return_value:
+            self.reset()
+
+        return return_value
+
+    def has_finished(self):
+        """:returns: bool; if the path has either not started or is done"""
+
+        return not self.is_started or self.is_done()
```

### Comparing `game_qu-2.0.0/src/game_qu/base/range.py` & `game_qu-2.0.1/src/game_qu/base/range.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-class Range:
-    """Stores the information for a start and end of a range (1-5)"""
-
-    start = 0
-    end = 0
-
-    def __init__(self, start, end):
-        """Initializes the object"""
-
-        self.start = start
-        self.end = end
-
-    def is_less_than(self, other_range):
-        """:returns: bool; if this range's start is less than the other range's start"""
-
-        starts_are_equal = self.start == other_range.start
-        return_value = None
-
-        if starts_are_equal:
-            return_value = self.end < other_range.end
-
-        else:
-            return_value = self.start < other_range.start
-
-        return return_value
-
-    def get_length(self):
-        """:returns: float; the length of the range (end - start)"""
-
-        return self.end - self.start
-
-    def __str__(self):
-        """Gives the string representation of the range"""
-
-        return f"{self.start} -> {self.end}"
-
-    def __contains__(self, number):
-        """:returns: bool; if the number is within the range- greater than start and less than end"""
-
+class Range:
+    """Stores the information for a start and end of a range (1-5)"""
+
+    start = 0
+    end = 0
+
+    def __init__(self, start, end):
+        """Initializes the object"""
+
+        self.start = start
+        self.end = end
+
+    def is_less_than(self, other_range):
+        """:returns: bool; if this range's start is less than the other range's start"""
+
+        starts_are_equal = self.start == other_range.start
+        return_value = None
+
+        if starts_are_equal:
+            return_value = self.end < other_range.end
+
+        else:
+            return_value = self.start < other_range.start
+
+        return return_value
+
+    def get_length(self):
+        """:returns: float; the length of the range (end - start)"""
+
+        return self.end - self.start
+
+    def __str__(self):
+        """Gives the string representation of the range"""
+
+        return f"{self.start} -> {self.end}"
+
+    def __contains__(self, number):
+        """:returns: bool; if the number is within the range- greater than start and less than end"""
+
         return number >= self.start and number <= self.end
```

### Comparing `game_qu-2.0.0/src/game_qu/base/unique_ids_list.py` & `game_qu-2.0.1/src/game_qu/base/unique_ids_list.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.0/src/game_qu/base/utility_functions.py` & `game_qu-2.0.1/src/game_qu/base/utility_functions.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,255 +1,255 @@
-from math import sqrt
-from game_qu.base.library_changer import LibraryChanger
-
-if not LibraryChanger.get_library_has_been_set():
-    LibraryChanger.set_game_library("pygame")
-
-from game_qu.base.fraction import Fraction
-from game_qu.base.important_variables import keyboard, SCREEN_LENGTH, SCREEN_HEIGHT, IS_USING_CONTROLLER
-import random
-
-from game_qu.library_abstraction import utility_functions
-from game_qu.base.range import Range
-
-# Retrieving the functions from the game library code
-load_image = getattr(utility_functions, "load_image")
-load_text = getattr(utility_functions, "load_text")
-render_text = getattr(utility_functions, "render_text")
-render_image = getattr(utility_functions, "render_image")
-render_rectangle = getattr(utility_functions, "render_rectangle")
-set_up_window = getattr(utility_functions, "set_up_window")
-key_is_pressed = getattr(utility_functions, "key_is_pressed")
-mouse_was_pressed = getattr(utility_functions, "mouse_was_pressed")
-call_every_cycle = getattr(utility_functions, "call_every_cycle")
-is_mouse_collision = getattr(utility_functions, "is_mouse_collision")
-get_time_passed = getattr(utility_functions, "get_time_passed")
-load_and_transform_image = getattr(utility_functions, "load_and_transform_image")
-get_directional_path_to_image = getattr(utility_functions, "get_directional_path_to_image")
-
-def key_is_pressed(key):
-    """:returns: bool; whether that key is currently held down (pressed)"""
-
-    return keyboard.get_key_event(key).happened_this_cycle
-
-
-def key_is_clicked(key):
-    """:returns: bool; whether the key was not held down last cycle and is this cycle (clicked)"""
-
-    return keyboard.get_key_event(key).is_click()
-
-
-def key_has_been_released(key):
-    """:returns: bool; whether the key was held down last cycle and is not this cycle (released)"""
-    return keyboard.get_key_event(key).has_stopped()
-
-
-def get_time_of_key_being_held_in(key):
-    """:returns: float; the amount of time that the key has been held down"""
-
-    return keyboard.get_key_timed_event(key).current_time
-
-def button_is_pressed(button):
-    """:returns: bool; whether that button is currently held down (pressed)"""
-
-    return keyboard.get_button_event(button).happened_this_cycle
-
-
-def button_is_clicked(button):
-    """:returns: bool; whether the button was not held down last cycle and is this cycle (clicked)"""
-
-    return keyboard.get_button_event(button).is_click()
-
-
-def button_has_been_released(button):
-    """:returns: bool; whether the button was held down last cycle and is not this cycle (released)"""
-
-    return keyboard.get_button_event(button).has_stopped()
-
-def get_time_of_button_being_held_in(button):
-    """:returns: float; the amount of time that the button has been held down"""
-
-    return keyboard.get_button_timed_event(button).current_time
-
-def button_is_pressed(button):
-    """:returns: bool; whether that button is currently held down (pressed)"""
-
-    return keyboard.get_button_event(button).happened_this_cycle
-
-def get_game_button_timed_event(game_button):
-    """:returns: TimedEvent; the TimedEvent that is associated with the current state (using the keyboard or controller)"""
-
-    return keyboard.get_button_timed_event(game_button) if IS_USING_CONTROLLER else keyboard.get_key_timed_event(game_button)
-def get_game_button_event(game_button):
-    """:returns: Event; the Event that is associated with the current state (using the keyboard or controller)"""
-
-    return keyboard.get_button_event(game_button) if IS_USING_CONTROLLER else keyboard.get_key_event(game_button)
-
-def game_button_is_pressed(game_button):
-    """:returns: bool; whether that game_button is currently held down (pressed)"""
-
-    return get_game_button_event(game_button).happened_this_cycle
-
-def game_button_is_clicked(game_button):
-    """:returns: bool; whether the game_button was not held down last cycle and is this cycle (clicked)"""
-
-    return get_game_button_event(game_button).is_click()
-
-def game_button_has_been_released(game_button):
-    """:returns: bool; whether the game_button was held down last cycle and is not this cycle (released)"""
-
-    return get_game_button_event(game_button).has_stopped()
-
-def get_time_of_game_button_being_held_in(game_button):
-    """:returns: float; the amount of time that the game_button has been held down"""
-
-    return get_game_button_timed_event(game_button).current_time
-
-
-def mouse_is_clicked():
-    """:returns: bool; whether the mouse was not pressed last cycle and is this cycle (clicked)"""
-
-    return keyboard.mouse_clicked_event.is_click()
-
-
-def get_index_of_range(number, range_lengths=[], ranges=None):
-    """ Finds the index of the range that contains the current number. A range is defined by the numbers between
-        two adjacent indexes (range_lengths[0] -> range_lengths[1])
-
-        :parameter range_lengths: float[]; the lengths of the ranges. For instance, if the range_lengths is [1, 1, 1] then the ranges would be [0 -> 1, 1 -> 2, 2 -> 3]
-        :parameter number: float; the number that is wanted to be within a range
-
-        :returns: int; The index of the range that contains the number and -1 no range contains it"""
-
-    index = -1
-
-    if ranges is None:
-        ranges = get_ranges(range_lengths)
-
-    for x in range(len(ranges)):
-        if ranges[x].__contains__(number):
-            index = x
-            break
-
-    return index
-
-def get_ranges(range_lengths):
-    """:returns: Range[]; the ranges gotten from the range_lengths. A range is defined by two adjacent indexes (range_lengths[0] -> range_lengths[1])"""
-
-    return_value = []
-    current_value = 0
-
-    for range_length in range_lengths:
-        return_value.append(Range(current_value, current_value + range_length))
-        current_value += range_length
-
-    return return_value
-
-def is_within_screen(game_object):
-    """:returns: bool; if the game_object is within the screen (can be seen on the screen)"""
-
-    return (game_object.right_edge > 0 and game_object.left_edge < SCREEN_LENGTH and
-            game_object.bottom_edge > 0 and game_object.top_edge < SCREEN_HEIGHT)
-
-
-def is_random_chance(probability: Fraction):
-    """ Uses the probability for the random chance (for instance if the probability is 7/10 then 7 out of 10
-        times it will return True and the other 3 times it will return False)
-
-        :parameter probability: Fraction; the probability this function will return True
-
-        :returns: bool; if the random number between 1-probability.denominator is >= probability.numerator
-    """
-
-    return random.randint(1, probability.denominator) <= probability.numerator
-
-
-def is_beyond_screen_left(left_edge):
-    """:returns: bool; if the left_edge is beyond the left side of the screen"""
-
-    return left_edge <= 0
-
-
-def is_beyond_screen_right(right_edge):
-    """:returns: bool; if the right_edge is beyond the right side of the screen"""
-
-    return right_edge >= SCREEN_LENGTH
-
-
-def min_value(item1, item2):
-    """:returns: float; the smallest item"""
-
-    if item1 is None:
-        return item2
-
-    if item2 is None:
-        return item1
-
-    return item1 if item1 < item2 else item2
-
-
-def max_value(item1, item2):
-    """returns float; the biggest item"""
-
-    return item1 if item1 > item2 else item2
-
-
-def get_combined_number_values(numbers):
-    """:returns: float or int; all the numbers in 'numbers' added up together in one number"""
-
-    return_value = 0
-
-    for number in numbers:
-        return_value += number
-
-    return return_value
-
-def get_next_index(current_index, max_index):
-    """:returns: int; the index after current_index (it cycles, so once it gets beyond the max_index it goes back to 0)"""
-
-    next_index = current_index + 1
-    return next_index if next_index <= max_index else 0
-
-
-def get_previous_index(current_index, max_index):
-    """:returns: int; the index before current_index (it cycles, so once it gets below 0 it goes to the max_index"""
-
-    prev_index = current_index - 1
-    return prev_index if prev_index >= 0 else max_index
-
-def rounded(number, places):
-    """:returns: float; the number rounded to that many decimal places"""
-
-    rounded_number = int(number * pow(10, places))
-
-    # Converting it back to the proper decimals once it gets rounded from above
-    return rounded_number / pow(10, places)
-
-def get_kwarg_item(kwargs, key, default_value):
-    """ :parameter kwargs: dict; the **kwargs
-        :parameter key: Object; the key for the item
-        :parameter default_value: Object; the value that will be obtained if the kwargs doesn't contain the key
-
-        :returns: Object; kwargs.get(key) if kwargs contains the key otherwise it will return the default_value
-    """
-
-    return kwargs.get(key) if kwargs.__contains__(key) else default_value
-
-def solve_quadratic(a, b, c):
-    """:returns: float[]; [answer1, answer2] the answers to the quadratic
-                and if the answer is an imaginary number it returns float('nan')"""
-
-    number_under_square_root = pow(b, 2) - 4 * a * c
-    number_under_square_root = rounded(number_under_square_root, 4)
-
-    if number_under_square_root < 0:
-        return None
-
-    square_root = sqrt(number_under_square_root)
-
-    answer1 = (-b + square_root) / (2 * a)
-    answer2 = (-b - square_root) / (2 * a)
-
-    answers = [answer2, answer1]
-
-    # If the answers are the same I should only return one of them
+from math import sqrt
+from game_qu.base.library_changer import LibraryChanger
+
+if not LibraryChanger.get_library_has_been_set():
+    LibraryChanger.set_game_library("pygame")
+
+from game_qu.base.fraction import Fraction
+from game_qu.base.important_variables import keyboard, SCREEN_LENGTH, SCREEN_HEIGHT, IS_USING_CONTROLLER
+import random
+
+from game_qu.library_abstraction import utility_functions
+from game_qu.base.range import Range
+
+# Retrieving the functions from the game library code
+load_image = getattr(utility_functions, "load_image")
+load_text = getattr(utility_functions, "load_text")
+render_text = getattr(utility_functions, "render_text")
+render_image = getattr(utility_functions, "render_image")
+render_rectangle = getattr(utility_functions, "render_rectangle")
+set_up_window = getattr(utility_functions, "set_up_window")
+key_is_pressed = getattr(utility_functions, "key_is_pressed")
+mouse_was_pressed = getattr(utility_functions, "mouse_was_pressed")
+call_every_cycle = getattr(utility_functions, "call_every_cycle")
+is_mouse_collision = getattr(utility_functions, "is_mouse_collision")
+get_time_passed = getattr(utility_functions, "get_time_passed")
+load_and_transform_image = getattr(utility_functions, "load_and_transform_image")
+get_directional_path_to_image = getattr(utility_functions, "get_directional_path_to_image")
+
+def key_is_pressed(key):
+    """:returns: bool; whether that key is currently held down (pressed)"""
+
+    return keyboard.get_key_event(key).happened_this_cycle
+
+
+def key_is_clicked(key):
+    """:returns: bool; whether the key was not held down last cycle and is this cycle (clicked)"""
+
+    return keyboard.get_key_event(key).is_click()
+
+
+def key_has_been_released(key):
+    """:returns: bool; whether the key was held down last cycle and is not this cycle (released)"""
+    return keyboard.get_key_event(key).has_stopped()
+
+
+def get_time_of_key_being_held_in(key):
+    """:returns: float; the amount of time that the key has been held down"""
+
+    return keyboard.get_key_timed_event(key).current_time
+
+def button_is_pressed(button):
+    """:returns: bool; whether that button is currently held down (pressed)"""
+
+    return keyboard.get_button_event(button).happened_this_cycle
+
+
+def button_is_clicked(button):
+    """:returns: bool; whether the button was not held down last cycle and is this cycle (clicked)"""
+
+    return keyboard.get_button_event(button).is_click()
+
+
+def button_has_been_released(button):
+    """:returns: bool; whether the button was held down last cycle and is not this cycle (released)"""
+
+    return keyboard.get_button_event(button).has_stopped()
+
+def get_time_of_button_being_held_in(button):
+    """:returns: float; the amount of time that the button has been held down"""
+
+    return keyboard.get_button_timed_event(button).current_time
+
+def button_is_pressed(button):
+    """:returns: bool; whether that button is currently held down (pressed)"""
+
+    return keyboard.get_button_event(button).happened_this_cycle
+
+def get_game_button_timed_event(game_button):
+    """:returns: TimedEvent; the TimedEvent that is associated with the current state (using the keyboard or controller)"""
+
+    return keyboard.get_button_timed_event(game_button) if IS_USING_CONTROLLER else keyboard.get_key_timed_event(game_button)
+def get_game_button_event(game_button):
+    """:returns: Event; the Event that is associated with the current state (using the keyboard or controller)"""
+
+    return keyboard.get_button_event(game_button) if IS_USING_CONTROLLER else keyboard.get_key_event(game_button)
+
+def game_button_is_pressed(game_button):
+    """:returns: bool; whether that game_button is currently held down (pressed)"""
+
+    return get_game_button_event(game_button).happened_this_cycle
+
+def game_button_is_clicked(game_button):
+    """:returns: bool; whether the game_button was not held down last cycle and is this cycle (clicked)"""
+
+    return get_game_button_event(game_button).is_click()
+
+def game_button_has_been_released(game_button):
+    """:returns: bool; whether the game_button was held down last cycle and is not this cycle (released)"""
+
+    return get_game_button_event(game_button).has_stopped()
+
+def get_time_of_game_button_being_held_in(game_button):
+    """:returns: float; the amount of time that the game_button has been held down"""
+
+    return get_game_button_timed_event(game_button).current_time
+
+
+def mouse_is_clicked():
+    """:returns: bool; whether the mouse was not pressed last cycle and is this cycle (clicked)"""
+
+    return keyboard.mouse_clicked_event.is_click()
+
+
+def get_index_of_range(number, range_lengths=[], ranges=None):
+    """ Finds the index of the range that contains the current number. A range is defined by the numbers between
+        two adjacent indexes (range_lengths[0] -> range_lengths[1])
+
+        :parameter range_lengths: float[]; the lengths of the ranges. For instance, if the range_lengths is [1, 1, 1] then the ranges would be [0 -> 1, 1 -> 2, 2 -> 3]
+        :parameter number: float; the number that is wanted to be within a range
+
+        :returns: int; The index of the range that contains the number and -1 no range contains it"""
+
+    index = -1
+
+    if ranges is None:
+        ranges = get_ranges(range_lengths)
+
+    for x in range(len(ranges)):
+        if ranges[x].__contains__(number):
+            index = x
+            break
+
+    return index
+
+def get_ranges(range_lengths):
+    """:returns: Range[]; the ranges gotten from the range_lengths. A range is defined by two adjacent indexes (range_lengths[0] -> range_lengths[1])"""
+
+    return_value = []
+    current_value = 0
+
+    for range_length in range_lengths:
+        return_value.append(Range(current_value, current_value + range_length))
+        current_value += range_length
+
+    return return_value
+
+def is_within_screen(game_object):
+    """:returns: bool; if the game_object is within the screen (can be seen on the screen)"""
+
+    return (game_object.right_edge > 0 and game_object.left_edge < SCREEN_LENGTH and
+            game_object.bottom_edge > 0 and game_object.top_edge < SCREEN_HEIGHT)
+
+
+def is_random_chance(probability: Fraction):
+    """ Uses the probability for the random chance (for instance if the probability is 7/10 then 7 out of 10
+        times it will return True and the other 3 times it will return False)
+
+        :parameter probability: Fraction; the probability this function will return True
+
+        :returns: bool; if the random number between 1-probability.denominator is >= probability.numerator
+    """
+
+    return random.randint(1, probability.denominator) <= probability.numerator
+
+
+def is_beyond_screen_left(left_edge):
+    """:returns: bool; if the left_edge is beyond the left side of the screen"""
+
+    return left_edge <= 0
+
+
+def is_beyond_screen_right(right_edge):
+    """:returns: bool; if the right_edge is beyond the right side of the screen"""
+
+    return right_edge >= SCREEN_LENGTH
+
+
+def min_value(item1, item2):
+    """:returns: float; the smallest item"""
+
+    if item1 is None:
+        return item2
+
+    if item2 is None:
+        return item1
+
+    return item1 if item1 < item2 else item2
+
+
+def max_value(item1, item2):
+    """returns float; the biggest item"""
+
+    return item1 if item1 > item2 else item2
+
+
+def get_combined_number_values(numbers):
+    """:returns: float or int; all the numbers in 'numbers' added up together in one number"""
+
+    return_value = 0
+
+    for number in numbers:
+        return_value += number
+
+    return return_value
+
+def get_next_index(current_index, max_index):
+    """:returns: int; the index after current_index (it cycles, so once it gets beyond the max_index it goes back to 0)"""
+
+    next_index = current_index + 1
+    return next_index if next_index <= max_index else 0
+
+
+def get_previous_index(current_index, max_index):
+    """:returns: int; the index before current_index (it cycles, so once it gets below 0 it goes to the max_index"""
+
+    prev_index = current_index - 1
+    return prev_index if prev_index >= 0 else max_index
+
+def rounded(number, places):
+    """:returns: float; the number rounded to that many decimal places"""
+
+    rounded_number = int(number * pow(10, places))
+
+    # Converting it back to the proper decimals once it gets rounded from above
+    return rounded_number / pow(10, places)
+
+def get_kwarg_item(kwargs, key, default_value):
+    """ :parameter kwargs: dict; the **kwargs
+        :parameter key: Object; the key for the item
+        :parameter default_value: Object; the value that will be obtained if the kwargs doesn't contain the key
+
+        :returns: Object; kwargs.get(key) if kwargs contains the key otherwise it will return the default_value
+    """
+
+    return kwargs.get(key) if kwargs.__contains__(key) else default_value
+
+def solve_quadratic(a, b, c):
+    """:returns: float[]; [answer1, answer2] the answers to the quadratic
+                and if the answer is an imaginary number it returns float('nan')"""
+
+    number_under_square_root = pow(b, 2) - 4 * a * c
+    number_under_square_root = rounded(number_under_square_root, 4)
+
+    if number_under_square_root < 0:
+        return None
+
+    square_root = sqrt(number_under_square_root)
+
+    answer1 = (-b + square_root) / (2 * a)
+    answer2 = (-b - square_root) / (2 * a)
+
+    answers = [answer2, answer1]
+
+    # If the answers are the same I should only return one of them
     return answers if answers[0] != answers[1] else [answers[0]]
```

### Comparing `game_qu-2.0.0/src/game_qu/base/velocity_calculator.py` & `game_qu-2.0.1/src/game_qu/base/velocity_calculator.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-class VelocityCalculator:
-    """A utility class that has methods for figuring out the velocity, distance, and sizes of components"""
-
-    time = 0
-    current_cycle_number = 1
-
-    @staticmethod
-    def get_velocity(unit_of_measurement, amount):
-        """:returns: float; (unit_of_measurement / 1000) * amount- This method breaks the unit_of_measurement into easier units to work with"""
-
-        return (unit_of_measurement / 1000) * amount
-
-    @staticmethod
-    def get_dimension(unit_of_measurement, amount):
-        """:returns: float; (unit_of_measurement / 100) * amount- This method breaks the unit_of_measurement into easier units to work with"""
-        return (unit_of_measurement / 100) * amount
-
-    @staticmethod
-    def get_distance(velocity):
-        """:returns: float; the amount of distance that has been traveled from that velocity since the last cycle (delta time * velocity)"""
-
-        return velocity * VelocityCalculator.time
+class VelocityCalculator:
+    """A utility class that has methods for figuring out the velocity, distance, and sizes of components"""
+
+    time = 0
+    current_cycle_number = 1
+
+    @staticmethod
+    def get_velocity(unit_of_measurement, amount):
+        """:returns: float; (unit_of_measurement / 1000) * amount- This method breaks the unit_of_measurement into easier units to work with"""
+
+        return (unit_of_measurement / 1000) * amount
+
+    @staticmethod
+    def get_dimension(unit_of_measurement, amount):
+        """:returns: float; (unit_of_measurement / 100) * amount- This method breaks the unit_of_measurement into easier units to work with"""
+        return (unit_of_measurement / 100) * amount
+
+    @staticmethod
+    def get_distance(velocity):
+        """:returns: float; the amount of distance that has been traveled from that velocity since the last cycle (delta time * velocity)"""
+
+        return velocity * VelocityCalculator.time
```

### Comparing `game_qu-2.0.0/src/game_qu/gui_components/component.py` & `game_qu-2.0.1/src/game_qu/gui_components/component.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from game_qu.base.history_keeper import HistoryKeeper
-from game_qu.base.velocity_calculator import VelocityCalculator
-from game_qu.gui_components.dimensions import Dimensions
-from game_qu.base.utility_functions import load_image, render_image, render_rectangle, mouse_is_clicked, is_mouse_collision
-from game_qu.base.id_creator import id_creator
-
-
-class Component(Dimensions):
-    """ The components that are added to the game's window. If a screen's get_components() method returns a component,
-        that components run and render methods will be called"""
-
-    color = None
-    path_to_image = None
-    name = ""
-    is_addable = True
-    is_runnable = True  # Sometimes the screen has to run the player, so some components shouldn't be run
-    last_frame_id_when_visible = 0
-    image_length = 1
-    image_height = 1
-
-    def __init__(self, path_to_image=""):
-        """Initializes the object and loads an image if the path_to_image is not empty"""
-
-        self.path_to_image = path_to_image
-
-        if path_to_image != "":
-            self.image_length, self.image_height = load_image(path_to_image)
-
-        self.name = id_creator.get_unique_id()
-
-    def run(self):
-        """Runs everything the component needs every game cycle"""
-
-        pass
-
-    def render(self):
-        """ Renders the component onto the screen- it will either render the image if 'self.path_to_image' is not empty
-            otherwise it will render a rectangle with the color from 'self.color'"""
-
-        if self.path_to_image != "":
-            render_image(self.path_to_image, self.left_edge, self.top_edge, self.length, self.height)
-
-        else:
-            render_rectangle(self.left_edge, self.top_edge, self.length, self.height, self.color)
-
-        self.last_frame_id_when_visible = HistoryKeeper.get_frame_id(VelocityCalculator.current_cycle_number)
-
-    def got_clicked(self):
-        """:returns: bool; the mouse is over the component and the mouse was clicked"""
-
-        was_visible_last_cycle = self.last_frame_id_when_visible == HistoryKeeper.last_frame_id
-        return mouse_is_clicked() and is_mouse_collision(self) and was_visible_last_cycle
-
-    def get_scaled_dimensions(self, unscaled_length, unscaled_height):
-        """ :returns: float[] [scaled_length, scaled_height]; the length and height of the image that is scaled by the
-            smallest of the two, so there is no stretching"""
-
-        horizontal_scale_factor = unscaled_length / self.image_length
-        vertical_scale_factor = unscaled_height / self.image_height
-
-        smaller_scale_factor = horizontal_scale_factor if horizontal_scale_factor < vertical_scale_factor else vertical_scale_factor
-
+from game_qu.base.history_keeper import HistoryKeeper
+from game_qu.base.velocity_calculator import VelocityCalculator
+from game_qu.gui_components.dimensions import Dimensions
+from game_qu.base.utility_functions import load_image, render_image, render_rectangle, mouse_is_clicked, is_mouse_collision
+from game_qu.base.id_creator import id_creator
+
+
+class Component(Dimensions):
+    """ The components that are added to the game's window. If a screen's get_components() method returns a component,
+        that components run and render methods will be called"""
+
+    color = None
+    path_to_image = None
+    name = ""
+    is_addable = True
+    is_runnable = True  # Sometimes the screen has to run the player, so some components shouldn't be run
+    last_frame_id_when_visible = 0
+    image_length = 1
+    image_height = 1
+
+    def __init__(self, path_to_image=""):
+        """Initializes the object and loads an image if the path_to_image is not empty"""
+
+        self.path_to_image = path_to_image
+
+        if path_to_image != "":
+            self.image_length, self.image_height = load_image(path_to_image)
+
+        self.name = id_creator.get_unique_id()
+
+    def run(self):
+        """Runs everything the component needs every game cycle"""
+
+        pass
+
+    def render(self):
+        """ Renders the component onto the screen- it will either render the image if 'self.path_to_image' is not empty
+            otherwise it will render a rectangle with the color from 'self.color'"""
+
+        if self.path_to_image != "":
+            render_image(self.path_to_image, self.left_edge, self.top_edge, self.length, self.height)
+
+        else:
+            render_rectangle(self.left_edge, self.top_edge, self.length, self.height, self.color)
+
+        self.last_frame_id_when_visible = HistoryKeeper.get_frame_id(VelocityCalculator.current_cycle_number)
+
+    def got_clicked(self):
+        """:returns: bool; the mouse is over the component and the mouse was clicked"""
+
+        was_visible_last_cycle = self.last_frame_id_when_visible == HistoryKeeper.last_frame_id
+        return mouse_is_clicked() and is_mouse_collision(self) and was_visible_last_cycle
+
+    def get_scaled_dimensions(self, unscaled_length, unscaled_height):
+        """ :returns: float[] [scaled_length, scaled_height]; the length and height of the image that is scaled by the
+            smallest of the two, so there is no stretching"""
+
+        horizontal_scale_factor = unscaled_length / self.image_length
+        vertical_scale_factor = unscaled_height / self.image_height
+
+        smaller_scale_factor = horizontal_scale_factor if horizontal_scale_factor < vertical_scale_factor else vertical_scale_factor
+
         return [self.image_length * smaller_scale_factor, self.image_height * smaller_scale_factor]
```

### Comparing `game_qu-2.0.0/src/game_qu/gui_components/dimensions.py` & `game_qu-2.0.1/src/game_qu/gui_components/dimensions.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-class Dimensions:
-    """ Gives left_edge, top_edge, height, length and then using those number it provides
-        right_edge, bottom_edge, horizontal_midpoint, and vertical_midpoint"""
-
-    left_edge = 0
-    top_edge = 0
-    length = 0
-    height = 0
-
-    def __init__(self, left_edge, top_edge, length, height):
-        """Initializes all the attributes of the class with the numbers provided (calls self.number_set_dimensions())"""
-
-        self.number_set_dimensions(left_edge, top_edge, length, height)
-
-    @property
-    def right_edge(self):
-        """The left_edge + length is what constitutes the object's right_edge"""
-
-        return self.left_edge + self.length
-
-    @property
-    def bottom_edge(self):
-        """The top_edge + height is what constitutes the object's bottom_edge"""
-
-        return self.top_edge + self.height
-
-    @property
-    def horizontal_midpoint(self):
-        """The left_edge + length / 2 is what constitutes the object's horizontal_midpoint"""
-
-        return self.left_edge + self.length / 2
-
-    @property
-    def vertical_midpoint(self):
-        """The top_edge + height / 2 is what constitutes the object's vertical_midpoint"""
-
-        return self.top_edge + self.height / 2
-
-    def number_set_dimensions(self, left_edge, top_edge, length, height):
-        """Sets the dimensions of this object (does the same thing as __init__)"""
-
-        self.left_edge, self.top_edge, self.length, self.height = left_edge, top_edge, length, height
-
-    def percentage_set_dimensions(self, percent_right, percent_down, percent_length, percent_height, horizontal_number, vertical_number):
-        """ Sets the dimensions based on the values passed into this function
-
-            :parameter percent_right: int; the percent it is to right (percentage of horizontal_number)
-            :parameter percent_down: int; the percent it is down (percentage of horizontal_number)
-            :parameter percent_length: int; the length (percentage of vertical_number)
-            :parameter percent_height: int; the height (percentage of vertical_number)
-            :parameter horizontal_number: int; what percent_right and percent_length are percentages of
-            :parameter vertical_number: int; what percent_down and percent_height are percentages of
-
-            :returns: None
-        """
-
-        self.left_edge = horizontal_number * percent_right / 100
-        self.length = horizontal_number * percent_length / 100
-        self.top_edge = vertical_number * percent_down / 100
+class Dimensions:
+    """ Gives left_edge, top_edge, height, length and then using those number it provides
+        right_edge, bottom_edge, horizontal_midpoint, and vertical_midpoint"""
+
+    left_edge = 0
+    top_edge = 0
+    length = 0
+    height = 0
+
+    def __init__(self, left_edge, top_edge, length, height):
+        """Initializes all the attributes of the class with the numbers provided (calls self.number_set_dimensions())"""
+
+        self.number_set_dimensions(left_edge, top_edge, length, height)
+
+    @property
+    def right_edge(self):
+        """The left_edge + length is what constitutes the object's right_edge"""
+
+        return self.left_edge + self.length
+
+    @property
+    def bottom_edge(self):
+        """The top_edge + height is what constitutes the object's bottom_edge"""
+
+        return self.top_edge + self.height
+
+    @property
+    def horizontal_midpoint(self):
+        """The left_edge + length / 2 is what constitutes the object's horizontal_midpoint"""
+
+        return self.left_edge + self.length / 2
+
+    @property
+    def vertical_midpoint(self):
+        """The top_edge + height / 2 is what constitutes the object's vertical_midpoint"""
+
+        return self.top_edge + self.height / 2
+
+    def number_set_dimensions(self, left_edge, top_edge, length, height):
+        """Sets the dimensions of this object (does the same thing as __init__)"""
+
+        self.left_edge, self.top_edge, self.length, self.height = left_edge, top_edge, length, height
+
+    def percentage_set_dimensions(self, percent_right, percent_down, percent_length, percent_height, horizontal_number, vertical_number):
+        """ Sets the dimensions based on the values passed into this function
+
+            :parameter percent_right: int; the percent it is to right (percentage of horizontal_number)
+            :parameter percent_down: int; the percent it is down (percentage of horizontal_number)
+            :parameter percent_length: int; the length (percentage of vertical_number)
+            :parameter percent_height: int; the height (percentage of vertical_number)
+            :parameter horizontal_number: int; what percent_right and percent_length are percentages of
+            :parameter vertical_number: int; what percent_down and percent_height are percentages of
+
+            :returns: None
+        """
+
+        self.left_edge = horizontal_number * percent_right / 100
+        self.length = horizontal_number * percent_length / 100
+        self.top_edge = vertical_number * percent_down / 100
         self.height = vertical_number * percent_height / 100
```

### Comparing `game_qu-2.0.0/src/game_qu/gui_components/grid.py` & `game_qu-2.0.1/src/game_qu/gui_components/grid.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-from math import ceil, floor
-
-from game_qu.base.important_variables import SCREEN_LENGTH, SCREEN_HEIGHT
-from game_qu.base.velocity_calculator import VelocityCalculator
-
-
-class Grid:
-    """Provides an easy way to put components into a grid"""
-
-    rows = None
-    columns = None
-    dimensions = None
-    length_buffer = VelocityCalculator.get_dimension(SCREEN_LENGTH, 1)
-    height_buffer = VelocityCalculator.get_dimension(SCREEN_HEIGHT, 1)
-    goes_top_to_bottom = True
-    goes_left_to_right = True
-
-    def __init__(self, dimensions, rows, columns, goes_top_to_bottom=True, goes_left_to_right=True):
-        """ Initializes the object | IMPORTANT - columns and rows can't both be None
-
-            :parameter dimensions: Dimensions; the left_edge, top_edge, length, and height of the grid
-            :parameter rows: int; the max amount of rows the grid can have (can be None)
-            :parameter columns: int; the max amount of columns the grid can have (can be None)
-            :parameter goes_top_to_bottom: bool; if the components of the grid start at the top and go down (start at bottom if False)
-            :parameter goes_left_to_right: bool; if the components of the grid start at the left and go right (start at right if False)
-
-            :returns: None
-        """
-
-        self.dimensions = dimensions
-        self.rows, self.columns = rows, columns
-        self.goes_top_to_bottom, self.goes_left_to_right = goes_top_to_bottom, goes_left_to_right
-
-    def turn_into_grid(self, items, item_max_length=None, item_max_height=None, component_stretching_is_allowed=True):
-        """ Turns all the items into a grid format
-
-            :parameter items: Component[]; the items that will be converted into a grid
-            :parameter item_max_length: int; the max length that an item can be (None means there is no max length)
-            :parameter item_max_height: int; the max height than an item can be (None means there is no max height)
-            :parameter component_stretching_is_allowed: bool; whether the component has to be scaled by a specific value
-             before it is rendered (instead of having uneven scales causing stretching)
-
-            :returns: None
-        """
-
-        rows, columns = self.rows, self.columns
-        number_of_items = len(items)
-
-        if rows is None:
-            rows = self.get_grid_dimension(columns, number_of_items)
-
-        if columns is None:
-            columns = self.get_grid_dimension(rows, number_of_items)
-
-        item_height = self.get_item_dimension(self.dimensions.height, rows, item_max_height, self.height_buffer)
-        item_length = self.get_item_dimension(self.dimensions.length, columns, item_max_length, self.length_buffer)
-
-        base_left_edge = self.dimensions.left_edge if self.goes_left_to_right else self.dimensions.right_edge - item_length
-        base_top_edge = self.dimensions.top_edge if self.goes_top_to_bottom else self.dimensions.bottom_edge - item_height
-
-        for x in range(number_of_items):
-            column_number = x % columns
-            row_number = floor(x / columns)
-
-            left_edge = base_left_edge + self.get_dimension_change(column_number, item_length, self.length_buffer)
-            top_edge = base_top_edge + self.get_dimension_change(row_number, item_height, self.height_buffer)
-
-            current_item_length = item_length
-            current_item_height = item_height
-            
-            if not component_stretching_is_allowed:
-                current_item_length, current_item_height = items[x].get_scaled_dimensions(item_length, item_height)
-
-            items[x].number_set_dimensions(left_edge, top_edge, current_item_length, current_item_height)
-
-    def get_grid_dimension(self, other_dimension, number_of_items):
-        """ Finds the number of either rows or columns there should be depending on the value of 'other_dimension' (ceil(number_of_items / other_dimension)
-
-            :parameter other_dimension: float; the grid dimension (number of rows or columns) other than the one that will be returned
-            :parameter number_of_items: int; The number of items in the grid
-
-            :returns: float; either the number of rows or columns depending on the value of 'other_dimension'"""
-
-        return ceil(number_of_items / other_dimension)
-
-    def get_item_dimension(self, grid_dimension_size, grid_dimension, item_dimension_max, buffer_between_items):
-        """ Finds the size of the item that is in 'grid_dimension'- height for rows and length for columns
-
-            :parameter grid_dimension_size: float; the grid's height if the grid item height is wanted and grid's length if the grid item length is wanted
-            :parameter grid_dimension: int; the grid's number of rows if the grid item height is wanted and grid's number of columns if the grid item length is wanted
-            :parameter item_dimension_max: float; the max value this function can return
-            :parameter buffer_between_items: float; the number of pixels between adjacent items
-
-            :returns: float; the size of the item that is in 'grid_dimension'- height for rows and length for columns"""
-
-        remaining_dimension = grid_dimension_size - buffer_between_items * (grid_dimension - 1)
-
-        item_dimension = remaining_dimension / grid_dimension
-
-        if item_dimension_max is not None and item_dimension > item_dimension_max:
-            item_dimension = item_dimension_max
-
-        return item_dimension
-
-    def get_dimension_change(self, grid_dimension, item_dimension, buffer_between_items):
-        """ The amount of pixels that are after the first grid item in the 'grid_dimension'
-
-            :parameter grid_dimension: int; rows if the grid item delta top_edge is wanted and columns if grid item delta left_edge is wanted
-            :parameter item_dimension: float; the height of the grid item if delta top_edge is wanted and length of the grid item if delta left_edge is wanted
-            :parameter buffer_between_items: float; the number of pixels between adjacent items
-
-            :returns: float; the amount of pixels that are after the first grid item in the 'grid_dimension'"""
-
-        dimension_change_amount = grid_dimension * (item_dimension + buffer_between_items)
-
-        # If it starts at the top then the top_edge increases, but if it doesn't then the top_edge decreases
-        return dimension_change_amount if self.goes_top_to_bottom else -dimension_change_amount
+from math import ceil, floor
+
+from game_qu.base.important_variables import SCREEN_LENGTH, SCREEN_HEIGHT
+from game_qu.base.velocity_calculator import VelocityCalculator
+
+
+class Grid:
+    """Provides an easy way to put components into a grid"""
+
+    rows = None
+    columns = None
+    dimensions = None
+    length_buffer = VelocityCalculator.get_dimension(SCREEN_LENGTH, 1)
+    height_buffer = VelocityCalculator.get_dimension(SCREEN_HEIGHT, 1)
+    goes_top_to_bottom = True
+    goes_left_to_right = True
+
+    def __init__(self, dimensions, rows, columns, goes_top_to_bottom=True, goes_left_to_right=True):
+        """ Initializes the object | IMPORTANT - columns and rows can't both be None
+
+            :parameter dimensions: Dimensions; the left_edge, top_edge, length, and height of the grid
+            :parameter rows: int; the max amount of rows the grid can have (can be None)
+            :parameter columns: int; the max amount of columns the grid can have (can be None)
+            :parameter goes_top_to_bottom: bool; if the components of the grid start at the top and go down (start at bottom if False)
+            :parameter goes_left_to_right: bool; if the components of the grid start at the left and go right (start at right if False)
+
+            :returns: None
+        """
+
+        self.dimensions = dimensions
+        self.rows, self.columns = rows, columns
+        self.goes_top_to_bottom, self.goes_left_to_right = goes_top_to_bottom, goes_left_to_right
+
+    def turn_into_grid(self, items, item_max_length=None, item_max_height=None, component_stretching_is_allowed=True):
+        """ Turns all the items into a grid format
+
+            :parameter items: Component[]; the items that will be converted into a grid
+            :parameter item_max_length: int; the max length that an item can be (None means there is no max length)
+            :parameter item_max_height: int; the max height than an item can be (None means there is no max height)
+            :parameter component_stretching_is_allowed: bool; whether the component has to be scaled by a specific value
+             before it is rendered (instead of having uneven scales causing stretching)
+
+            :returns: None
+        """
+
+        rows, columns = self.rows, self.columns
+        number_of_items = len(items)
+
+        if rows is None:
+            rows = self.get_grid_dimension(columns, number_of_items)
+
+        if columns is None:
+            columns = self.get_grid_dimension(rows, number_of_items)
+
+        item_height = self.get_item_dimension(self.dimensions.height, rows, item_max_height, self.height_buffer)
+        item_length = self.get_item_dimension(self.dimensions.length, columns, item_max_length, self.length_buffer)
+
+        base_left_edge = self.dimensions.left_edge if self.goes_left_to_right else self.dimensions.right_edge - item_length
+        base_top_edge = self.dimensions.top_edge if self.goes_top_to_bottom else self.dimensions.bottom_edge - item_height
+
+        for x in range(number_of_items):
+            column_number = x % columns
+            row_number = floor(x / columns)
+
+            left_edge = base_left_edge + self.get_dimension_change(column_number, item_length, self.length_buffer)
+            top_edge = base_top_edge + self.get_dimension_change(row_number, item_height, self.height_buffer)
+
+            current_item_length = item_length
+            current_item_height = item_height
+            
+            if not component_stretching_is_allowed:
+                current_item_length, current_item_height = items[x].get_scaled_dimensions(item_length, item_height)
+
+            items[x].number_set_dimensions(left_edge, top_edge, current_item_length, current_item_height)
+
+    def get_grid_dimension(self, other_dimension, number_of_items):
+        """ Finds the number of either rows or columns there should be depending on the value of 'other_dimension' (ceil(number_of_items / other_dimension)
+
+            :parameter other_dimension: float; the grid dimension (number of rows or columns) other than the one that will be returned
+            :parameter number_of_items: int; The number of items in the grid
+
+            :returns: float; either the number of rows or columns depending on the value of 'other_dimension'"""
+
+        return ceil(number_of_items / other_dimension)
+
+    def get_item_dimension(self, grid_dimension_size, grid_dimension, item_dimension_max, buffer_between_items):
+        """ Finds the size of the item that is in 'grid_dimension'- height for rows and length for columns
+
+            :parameter grid_dimension_size: float; the grid's height if the grid item height is wanted and grid's length if the grid item length is wanted
+            :parameter grid_dimension: int; the grid's number of rows if the grid item height is wanted and grid's number of columns if the grid item length is wanted
+            :parameter item_dimension_max: float; the max value this function can return
+            :parameter buffer_between_items: float; the number of pixels between adjacent items
+
+            :returns: float; the size of the item that is in 'grid_dimension'- height for rows and length for columns"""
+
+        remaining_dimension = grid_dimension_size - buffer_between_items * (grid_dimension - 1)
+
+        item_dimension = remaining_dimension / grid_dimension
+
+        if item_dimension_max is not None and item_dimension > item_dimension_max:
+            item_dimension = item_dimension_max
+
+        return item_dimension
+
+    def get_dimension_change(self, grid_dimension, item_dimension, buffer_between_items):
+        """ The amount of pixels that are after the first grid item in the 'grid_dimension'
+
+            :parameter grid_dimension: int; rows if the grid item delta top_edge is wanted and columns if grid item delta left_edge is wanted
+            :parameter item_dimension: float; the height of the grid item if delta top_edge is wanted and length of the grid item if delta left_edge is wanted
+            :parameter buffer_between_items: float; the number of pixels between adjacent items
+
+            :returns: float; the amount of pixels that are after the first grid item in the 'grid_dimension'"""
+
+        dimension_change_amount = grid_dimension * (item_dimension + buffer_between_items)
+
+        # If it starts at the top then the top_edge increases, but if it doesn't then the top_edge decreases
+        return dimension_change_amount if self.goes_top_to_bottom else -dimension_change_amount
```

### Comparing `game_qu-2.0.0/src/game_qu/gui_components/hud.py` & `game_qu-2.0.1/src/game_qu/gui_components/hud.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-from game_qu.gui_components.grid import Grid
-from game_qu.base.colors import *
-from game_qu.gui_components.component import Component
-from game_qu.base.important_variables import *
-from game_qu.gui_components.text_box import TextBox
-from game_qu.gui_components.dimensions import Dimensions
-
-class HUD(Component):
-    """HUD stands for Heads Up Display. This class provides an easy way to show all the information that the player needs"""
-
-    player_points_fields = []
-    other_fields = []
-    high_score_field = None
-    components = []
-    high_score_is_needed = False
-    rows = 1
-    columns = None
-
-    def __init__(self, number_of_points_fields, other_fields, length, height, rows=1, columns=None, high_score_is_needed=False):
-        """ Initializes the object with the values provided by initializing the TextBox(s) needed.
-            Also fields is just another way of saying TextBox. The HUD uses the Grid class from game_qu.gui_components/grid.py to make the grid pattern
-
-            :parameter number_of_points_fields: int; the number of fields that contain points for players (generally equal to the number of players)
-            :parameter other_fields: Component[]; the other fields that should be displayed
-            :parameter length: float; the length of the HUD (in pixels)
-            :parameter height: float; the height of the HUD (in pixels)
-            :parameter rows: int; the number of rows for the grid of the HUD (see gui_components/grid.py for more information)
-            :parameter columns: int; the number of columns for the grid of the HUD (see gui_components/grid.py for more information)
-            :parameter high_score_is_needed: bool; whether a high score is wanted for the HUD
-
-            :returns: None
-        """
-
-        self.player_points_fields = []
-        self.rows = rows
-        self.columns = columns
-        self.high_score_is_needed = high_score_is_needed
-
-        if high_score_is_needed:
-            self.high_score_field = TextBox("", 28, pleasing_green, white, True)
-            other_fields += [self.high_score_field]
-
-        colors = [blue, red, black, orange, purple, yellow]
-
-        for x in range(number_of_points_fields):
-            self.player_points_fields.append(TextBox("", 28, white, colors[x], True))
-
-        self.components = self.player_points_fields + other_fields
-
-        grid = Grid(Dimensions(0, 0, length, height), rows, columns)
-        grid.turn_into_grid(self.components, None, None)
-
-    def update(self, player_points, high_score=0):
-        """Updates the points in the 'player_points_fields' and if the 'high_score_is_needed' it updates the high score in the 'high_score_field'"""
-
-        for x in range(len(player_points)):
-            self.player_points_fields[x].text = f"Player #{x + 1}: {player_points[x]}"
-
-        if self.high_score_is_needed:
-            self.high_score_field.text = f"High Score: {high_score}"
-
-    def render(self):
-        """Renders the HUD onto the screen"""
-
-        for component in self.components:
-            component.render()
-
-    def set_dimensions(self, left_edge, top_edge, length, height):
-        """Changes the dimensions of the Grid that defines the components layouts"""
-
-        grid = Grid(Dimensions(left_edge, top_edge, length, height), self.rows, self.columns)
-        grid.turn_into_grid(self.components, None, None)
-
-    def set_rows_and_columns(self, rows, columns):
-        """Sets the 'self.rows' and 'self.columns' to the values provided: 'rows' and 'columns'"""
-
-        self.rows = rows
-        self.columns = columns
+from game_qu.gui_components.grid import Grid
+from game_qu.base.colors import *
+from game_qu.gui_components.component import Component
+from game_qu.base.important_variables import *
+from game_qu.gui_components.text_box import TextBox
+from game_qu.gui_components.dimensions import Dimensions
+
+class HUD(Component):
+    """HUD stands for Heads Up Display. This class provides an easy way to show all the information that the player needs"""
+
+    player_points_fields = []
+    other_fields = []
+    high_score_field = None
+    components = []
+    high_score_is_needed = False
+    rows = 1
+    columns = None
+
+    def __init__(self, number_of_points_fields, other_fields, length, height, rows=1, columns=None, high_score_is_needed=False):
+        """ Initializes the object with the values provided by initializing the TextBox(s) needed.
+            Also fields is just another way of saying TextBox. The HUD uses the Grid class from game_qu.gui_components/grid.py to make the grid pattern
+
+            :parameter number_of_points_fields: int; the number of fields that contain points for players (generally equal to the number of players)
+            :parameter other_fields: Component[]; the other fields that should be displayed
+            :parameter length: float; the length of the HUD (in pixels)
+            :parameter height: float; the height of the HUD (in pixels)
+            :parameter rows: int; the number of rows for the grid of the HUD (see gui_components/grid.py for more information)
+            :parameter columns: int; the number of columns for the grid of the HUD (see gui_components/grid.py for more information)
+            :parameter high_score_is_needed: bool; whether a high score is wanted for the HUD
+
+            :returns: None
+        """
+
+        self.player_points_fields = []
+        self.rows = rows
+        self.columns = columns
+        self.high_score_is_needed = high_score_is_needed
+
+        if high_score_is_needed:
+            self.high_score_field = TextBox("", 28, pleasing_green, white, True)
+            other_fields += [self.high_score_field]
+
+        colors = [blue, red, black, orange, purple, yellow]
+
+        for x in range(number_of_points_fields):
+            self.player_points_fields.append(TextBox("", 28, white, colors[x], True))
+
+        self.components = self.player_points_fields + other_fields
+
+        grid = Grid(Dimensions(0, 0, length, height), rows, columns)
+        grid.turn_into_grid(self.components, None, None)
+
+    def update(self, player_points, high_score=0):
+        """Updates the points in the 'player_points_fields' and if the 'high_score_is_needed' it updates the high score in the 'high_score_field'"""
+
+        for x in range(len(player_points)):
+            self.player_points_fields[x].text = f"Player #{x + 1}: {player_points[x]}"
+
+        if self.high_score_is_needed:
+            self.high_score_field.text = f"High Score: {high_score}"
+
+    def render(self):
+        """Renders the HUD onto the screen"""
+
+        for component in self.components:
+            component.render()
+
+    def set_dimensions(self, left_edge, top_edge, length, height):
+        """Changes the dimensions of the Grid that defines the components layouts"""
+
+        grid = Grid(Dimensions(left_edge, top_edge, length, height), self.rows, self.columns)
+        grid.turn_into_grid(self.components, None, None)
+
+    def set_rows_and_columns(self, rows, columns):
+        """Sets the 'self.rows' and 'self.columns' to the values provided: 'rows' and 'columns'"""
+
+        self.rows = rows
+        self.columns = columns
```

### Comparing `game_qu-2.0.0/src/game_qu/gui_components/intermediate_screen.py` & `game_qu-2.0.1/src/game_qu/gui_components/intermediate_screen.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-from game_qu.base.colors import white
-from game_qu.base.utility_functions import get_index_of_range, get_ranges
-from game_qu.gui_components.dimensions import Dimensions
-from game_qu.base.events import TimedEvent
-from game_qu.base.important_variables import BACKGROUND_COLOR, SCREEN_LENGTH, SCREEN_HEIGHT
-from game_qu.gui_components.screen import Screen
-from game_qu.gui_components.text_box import TextBox
-
-from game_qu.base.range import Range
-from game_qu.base.velocity_calculator import VelocityCalculator
-
-
-class IntermediateScreen(Screen):
-    """A screen that displays text(s) for a period of time"""
-
-    time_ranges = []
-    current_time = 0
-    max_time = 0
-    screens = []
-    texts = []
-    set_screen_text_function = None
-    is_being_displayed = False
-
-    def __init__(self, number_of_screens=1, screens=None, texts=[""], times_displayed=[0], set_screen_text_function=None):
-        """Initializes the object"""
-
-        if screens is None:
-            self.create_screens(number_of_screens, texts)
-
-        else:
-            self.screens = screens
-
-        self.set_time_ranges(get_ranges(times_displayed))
-
-        self.set_screen_text_function = self.set_screen_text if set_screen_text_function is None else set_screen_text_function
-
-        Dimensions.__init__(self, 0, 0, SCREEN_LENGTH, SCREEN_HEIGHT)
-
-    def create_screens(self, number_of_screens, texts):
-        """Initializes all the screens (equal to the number_of_screens)"""
-
-        for x in range(number_of_screens):
-            screen = Screen()
-
-            text_box = TextBox(texts[x], 30, BACKGROUND_COLOR, white, True)
-            text_box.number_set_dimensions(0, 0, SCREEN_LENGTH, SCREEN_HEIGHT)
-            screen.components = [text_box]
-            self.screens.append(screen)
-
-    def set_texts(self, texts):
-        """Sets the texts of all the screens in 'self.screens.' It does this by using the method 'self.change_screen_method,' which is set in the __init__ method"""
-
-        for x in range(len(texts)):
-            self.set_screen_text_function(self.screens[x], texts[x])
-    
-    def set_screen_text(self, screen, text):
-        """Sets the text the screen displays (or no text if that is wanted). Calls the 'set_text' method of the screen's first component"""
-
-        # By default, the screen's first component is the TextBox containing the text
-        screen.components[0].set_text(text)
-        
-    def display(self):
-        """Displays all the intermediate screens and sets 'self.current_time' to 0 resetting the screen timers"""
-
-        self.current_time = 0
-        self.is_being_displayed = True
-
-    def get_components(self):
-        """:returns: Component[]; the components that should be displayed"""
-
-        index = get_index_of_range(self.current_time, ranges=self.time_ranges)
-        self.screens[index].render_background()
-        return self.screens[index].get_components()
-
-    def reset(self):
-        """Resets the object back to the start"""
-
-        self.current_time = 0
-        self.is_being_displayed = False
-
-    def set_time_ranges(self, time_ranges):
-        """ Sets the time ranges that each screen is displayed (from 1 second to 3 seconds). If using range_lengths is wanted then
-            it is reccommended to use the function get_ranges in base/utility_functions.py"""
-
-        self.time_ranges = time_ranges
-        self.max_time = 0
-
-        for time_range in time_ranges:
-            self.max_time += time_range.get_length()
-
-    def has_finished(self):
-        """:returns: bool; if the intermediate screens are done being displayed"""
-
-        return self.current_time > self.max_time or not self.is_being_displayed
-
-    def run(self):
-        """Runs all the code necessary to make this object work properly"""
-
-        if not self.has_finished():
-            self.current_time += VelocityCalculator.time
-            index = get_index_of_range(self.current_time, ranges=self.time_ranges)
-            self.screens[index].run()
-
+from game_qu.base.colors import white
+from game_qu.base.utility_functions import get_index_of_range, get_ranges
+from game_qu.gui_components.dimensions import Dimensions
+from game_qu.base.events import TimedEvent
+from game_qu.base.important_variables import BACKGROUND_COLOR, SCREEN_LENGTH, SCREEN_HEIGHT
+from game_qu.gui_components.screen import Screen
+from game_qu.gui_components.text_box import TextBox
+
+from game_qu.base.range import Range
+from game_qu.base.velocity_calculator import VelocityCalculator
+
+
+class IntermediateScreen(Screen):
+    """A screen that displays text(s) for a period of time"""
+
+    time_ranges = []
+    current_time = 0
+    max_time = 0
+    screens = []
+    texts = []
+    set_screen_text_function = None
+    is_being_displayed = False
+
+    def __init__(self, number_of_screens=1, screens=None, texts=[""], times_displayed=[0], set_screen_text_function=None):
+        """Initializes the object"""
+
+        if screens is None:
+            self.create_screens(number_of_screens, texts)
+
+        else:
+            self.screens = screens
+
+        self.set_time_ranges(get_ranges(times_displayed))
+
+        self.set_screen_text_function = self.set_screen_text if set_screen_text_function is None else set_screen_text_function
+
+        Dimensions.__init__(self, 0, 0, SCREEN_LENGTH, SCREEN_HEIGHT)
+
+    def create_screens(self, number_of_screens, texts):
+        """Initializes all the screens (equal to the number_of_screens)"""
+
+        for x in range(number_of_screens):
+            screen = Screen()
+
+            text_box = TextBox(texts[x], 30, BACKGROUND_COLOR, white, True)
+            text_box.number_set_dimensions(0, 0, SCREEN_LENGTH, SCREEN_HEIGHT)
+            screen.components = [text_box]
+            self.screens.append(screen)
+
+    def set_texts(self, texts):
+        """Sets the texts of all the screens in 'self.screens.' It does this by using the method 'self.change_screen_method,' which is set in the __init__ method"""
+
+        for x in range(len(texts)):
+            self.set_screen_text_function(self.screens[x], texts[x])
+    
+    def set_screen_text(self, screen, text):
+        """Sets the text the screen displays (or no text if that is wanted). Calls the 'set_text' method of the screen's first component"""
+
+        # By default, the screen's first component is the TextBox containing the text
+        screen.components[0].set_text(text)
+        
+    def display(self):
+        """Displays all the intermediate screens and sets 'self.current_time' to 0 resetting the screen timers"""
+
+        self.current_time = 0
+        self.is_being_displayed = True
+
+    def get_components(self):
+        """:returns: Component[]; the components that should be displayed"""
+
+        index = get_index_of_range(self.current_time, ranges=self.time_ranges)
+        self.screens[index].render_background()
+        return self.screens[index].get_components()
+
+    def reset(self):
+        """Resets the object back to the start"""
+
+        self.current_time = 0
+        self.is_being_displayed = False
+
+    def set_time_ranges(self, time_ranges):
+        """ Sets the time ranges that each screen is displayed (from 1 second to 3 seconds). If using range_lengths is wanted then
+            it is reccommended to use the function get_ranges in base/utility_functions.py"""
+
+        self.time_ranges = time_ranges
+        self.max_time = 0
+
+        for time_range in time_ranges:
+            self.max_time += time_range.get_length()
+
+    def has_finished(self):
+        """:returns: bool; if the intermediate screens are done being displayed"""
+
+        return self.current_time > self.max_time or not self.is_being_displayed
+
+    def run(self):
+        """Runs all the code necessary to make this object work properly"""
+
+        if not self.has_finished():
+            self.current_time += VelocityCalculator.time
+            index = get_index_of_range(self.current_time, ranges=self.time_ranges)
+            self.screens[index].run()
+
```

### Comparing `game_qu-2.0.0/src/game_qu/gui_components/navigation_screen.py` & `game_qu-2.0.1/src/game_qu/gui_components/navigation_screen.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-from math import sqrt
-
-from game_qu.base.colors import pleasing_green, white
-from game_qu.gui_components.dimensions import Dimensions
-from game_qu.base.utility_functions import button_is_clicked, mouse_is_clicked
-from game_qu.gui_components.grid import Grid
-from game_qu.gui_components.screen import Screen
-from game_qu.gui_components.text_box import TextBox
-from game_qu.base.important_variables import *
-from game_qu.base.utility_functions import game_button_is_clicked
-
-
-class NavigationScreen(Screen):
-    """ A screen that allows you to select different screens (navigate between different screens).
-        By default, hitting escape brings you back to the main screen"""
-
-    buttons = []
-    screens = []
-    selected_screen = None
-    back_to_main_screen_game_button = KEY_ESCAPE
-    button_color = pleasing_green
-    screen_shortcut_game_buttons = {}
-
-    def __init__(self, screen_names, screens, screen_shortcut_game_buttons={}, back_to_main_screen_game_button=KEY_ESCAPE, path_to_background_image="", button_color=button_color):
-        """ Initializes the object with the values provided. It will create a grid with text boxes each containing a screen_name
-            That will link to a specific screen (screen_names[0] -> screens[0])
-
-            :parameter screen_names: str[]; the names of the screens that will be displayed
-            :parameter screens: Screen[]; the screens, which the screen_names are referencing
-            :parameter screen_shortcut_game_buttons: dict {game_button: Screen}. Game button can either be a key or
-            button depending on whether IS_USING_CONTROLLER is true or not (if it is True game_button is a button otherwise it is a key)
-            :parameter back_to_main_screen_game_button: game_button; the game_button that will bring the user back to the main screen
-            :parameter path_to_background_image: str; the path to the background image of the navigation screen
-            :parameter button_color: int[] {red, green, blue}; the rgb values of the buttons
-        """
-
-        super().__init__(path_to_background_image)
-        self.screens = screens
-        self.button_color = button_color
-        self.screen_shortcut_game_buttons = screen_shortcut_game_buttons
-        self.buttons = []
-
-        for screen_name in screen_names:
-            self.buttons.append(TextBox(screen_name, 18, pleasing_green, white, True))
-
-        columns = int(sqrt(len(screen_names)))
-        button_grid = Grid(Dimensions(0, 0, SCREEN_LENGTH, SCREEN_HEIGHT), columns, None)
-        button_grid.turn_into_grid(self.buttons, None, None)
-
-        self.components = self.buttons
-        self.selected_screen = self
-        self.back_to_main_screen_game_button = back_to_main_screen_game_button
-
-    def run(self):
-        """ Changes the currently displayed screen if the buttons were clicked, or the back_to_main_screen_game_button is clicked.
-            It will also run the currently selected_screen's run method"""
-
-        for x in range(len(self.buttons)):
-            if self.buttons[x].got_clicked() and self.selected_screen == self:
-                self.selected_screen = self.screens[x]
-
-        for game_button in self.screen_shortcut_game_buttons.keys():
-            if game_button_is_clicked(game_button):
-                self.selected_screen = self.screen_shortcut_game_buttons.get(game_button)
-
-        if game_button_is_clicked(self.back_to_main_screen_game_button):
-            self.selected_screen = self
-
-        if self.selected_screen != self:
-            self.selected_screen.run()
-
-    def render_background(self):
-        """Renders the background of the currently selected screen"""
-
-        if self.selected_screen != self:
-            self.selected_screen.render_background()
-
-        else:
-            super().render_background()
-
-    def get_components(self):
-        """:returns: Component[]; the components of the currently selected_screen"""
-
-        return self.components if self.selected_screen == self else self.selected_screen.get_components()
-
-    def run_on_close(self):
-        """Makes sure all the screen's run_on_close methods are called"""
-
-        for screen in self.screens:
-            screen.run_on_close()
-
-    def modify_values(self, button_color=button_color, back_to_main_screen_game_button=back_to_main_screen_game_button):
-        """Gives the ability to modify the values of the NavigationScreen"""
-
-        self.button_color = button_color
-        self.back_to_main_screen_game_button = back_to_main_screen_game_button
-
-        for button in self.buttons:
-            button.set_background_color(button_color)
+from math import sqrt
+
+from game_qu.base.colors import pleasing_green, white
+from game_qu.gui_components.dimensions import Dimensions
+from game_qu.base.utility_functions import button_is_clicked, mouse_is_clicked
+from game_qu.gui_components.grid import Grid
+from game_qu.gui_components.screen import Screen
+from game_qu.gui_components.text_box import TextBox
+from game_qu.base.important_variables import *
+from game_qu.base.utility_functions import game_button_is_clicked
+
+
+class NavigationScreen(Screen):
+    """ A screen that allows you to select different screens (navigate between different screens).
+        By default, hitting escape brings you back to the main screen"""
+
+    buttons = []
+    screens = []
+    selected_screen = None
+    back_to_main_screen_game_button = KEY_ESCAPE
+    button_color = pleasing_green
+    screen_shortcut_game_buttons = {}
+
+    def __init__(self, screen_names, screens, screen_shortcut_game_buttons={}, back_to_main_screen_game_button=KEY_ESCAPE, path_to_background_image="", button_color=button_color):
+        """ Initializes the object with the values provided. It will create a grid with text boxes each containing a screen_name
+            That will link to a specific screen (screen_names[0] -> screens[0])
+
+            :parameter screen_names: str[]; the names of the screens that will be displayed
+            :parameter screens: Screen[]; the screens, which the screen_names are referencing
+            :parameter screen_shortcut_game_buttons: dict {game_button: Screen}. Game button can either be a key or
+            button depending on whether IS_USING_CONTROLLER is true or not (if it is True game_button is a button otherwise it is a key)
+            :parameter back_to_main_screen_game_button: game_button; the game_button that will bring the user back to the main screen
+            :parameter path_to_background_image: str; the path to the background image of the navigation screen
+            :parameter button_color: int[] {red, green, blue}; the rgb values of the buttons
+        """
+
+        super().__init__(path_to_background_image)
+        self.screens = screens
+        self.button_color = button_color
+        self.screen_shortcut_game_buttons = screen_shortcut_game_buttons
+        self.buttons = []
+
+        for screen_name in screen_names:
+            self.buttons.append(TextBox(screen_name, 18, pleasing_green, white, True))
+
+        columns = int(sqrt(len(screen_names)))
+        button_grid = Grid(Dimensions(0, 0, SCREEN_LENGTH, SCREEN_HEIGHT), columns, None)
+        button_grid.turn_into_grid(self.buttons, None, None)
+
+        self.components = self.buttons
+        self.selected_screen = self
+        self.back_to_main_screen_game_button = back_to_main_screen_game_button
+
+    def run(self):
+        """ Changes the currently displayed screen if the buttons were clicked, or the back_to_main_screen_game_button is clicked.
+            It will also run the currently selected_screen's run method"""
+
+        for x in range(len(self.buttons)):
+            if self.buttons[x].got_clicked() and self.selected_screen == self:
+                self.selected_screen = self.screens[x]
+
+        for game_button in self.screen_shortcut_game_buttons.keys():
+            if game_button_is_clicked(game_button):
+                self.selected_screen = self.screen_shortcut_game_buttons.get(game_button)
+
+        if game_button_is_clicked(self.back_to_main_screen_game_button):
+            self.selected_screen = self
+
+        if self.selected_screen != self:
+            self.selected_screen.run()
+
+    def render_background(self):
+        """Renders the background of the currently selected screen"""
+
+        if self.selected_screen != self:
+            self.selected_screen.render_background()
+
+        else:
+            super().render_background()
+
+    def get_components(self):
+        """:returns: Component[]; the components of the currently selected_screen"""
+
+        return self.components if self.selected_screen == self else self.selected_screen.get_components()
+
+    def run_on_close(self):
+        """Makes sure all the screen's run_on_close methods are called"""
+
+        for screen in self.screens:
+            screen.run_on_close()
+
+    def modify_values(self, button_color=button_color, back_to_main_screen_game_button=back_to_main_screen_game_button):
+        """Gives the ability to modify the values of the NavigationScreen"""
+
+        self.button_color = button_color
+        self.back_to_main_screen_game_button = back_to_main_screen_game_button
+
+        for button in self.buttons:
+            button.set_background_color(button_color)
```

### Comparing `game_qu-2.0.0/src/game_qu/gui_components/screen.py` & `game_qu-2.0.1/src/game_qu/gui_components/screen.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from game_qu.base.colors import light_gray
-from game_qu.base.utility_functions import render_image
-from game_qu.gui_components.component import Component
-from game_qu.base.important_variables import *
-from game_qu.base.utility_functions import *
-
-screen_sized_component = Component()
-screen_sized_component.number_set_dimensions(0, 0, SCREEN_LENGTH, SCREEN_HEIGHT)
-
-
-class Screen(Component):
-    """ Is the only thing that shows on the window at a time. The Window class (gui_components/window.py) will call the Screen's
-        run() and render_background() method will be called every game frame. It will also the run() and render() method for
-        all the Component(s) that the Screen's get_components() method returns"""
-
-    components = []
-    path_to_background_image = ""
-    is_visible = True
-    background_color = light_gray
-
-    def __init__(self, path_to_background_image="", background_color=light_gray):
-        """ Initializes the object and also loads the image which is at the path 'path_to_background_image.' No image will
-            be loaded if path_to_background_image is ''"""
-
-        self.path_to_background_image = path_to_background_image
-        self.background_color = background_color
-
-        if self.path_to_background_image != "":
-            load_image(path_to_background_image)
-
-    def get_components(self):
-        """:returns: Component[]; the components of the screen"""
-
-        return self.components
-
-    def render_background(self):
-        """Renders the background image that is at the path 'path_to_background_image'"""
-
-        if self.path_to_background_image != "":
-            render_image(self.path_to_background_image, 0, 0, SCREEN_LENGTH, SCREEN_HEIGHT)
-
-        else:
-            screen_sized_component.color = self.background_color
-            screen_sized_component.render()
+from game_qu.base.colors import light_gray
+from game_qu.base.utility_functions import render_image
+from game_qu.gui_components.component import Component
+from game_qu.base.important_variables import *
+from game_qu.base.utility_functions import *
+
+screen_sized_component = Component()
+screen_sized_component.number_set_dimensions(0, 0, SCREEN_LENGTH, SCREEN_HEIGHT)
+
+
+class Screen(Component):
+    """ Is the only thing that shows on the window at a time. The Window class (gui_components/window.py) will call the Screen's
+        run() and render_background() method will be called every game frame. It will also the run() and render() method for
+        all the Component(s) that the Screen's get_components() method returns"""
+
+    components = []
+    path_to_background_image = ""
+    is_visible = True
+    background_color = light_gray
+
+    def __init__(self, path_to_background_image="", background_color=light_gray):
+        """ Initializes the object and also loads the image which is at the path 'path_to_background_image.' No image will
+            be loaded if path_to_background_image is ''"""
+
+        self.path_to_background_image = path_to_background_image
+        self.background_color = background_color
+
+        if self.path_to_background_image != "":
+            load_image(path_to_background_image)
+
+    def get_components(self):
+        """:returns: Component[]; the components of the screen"""
+
+        return self.components
+
+    def render_background(self):
+        """Renders the background image that is at the path 'path_to_background_image'"""
+
+        if self.path_to_background_image != "":
+            render_image(self.path_to_background_image, 0, 0, SCREEN_LENGTH, SCREEN_HEIGHT)
+
+        else:
+            screen_sized_component.color = self.background_color
+            screen_sized_component.render()
```

### Comparing `game_qu-2.0.0/src/game_qu/gui_components/text_box.py` & `game_qu-2.0.1/src/game_qu/gui_components/text_box.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-from game_qu.gui_components.dimensions import Dimensions
-from game_qu.base.important_variables import game_window
-from game_qu.gui_components.component import Component
-from game_qu.base.utility_functions import *
-
-class TextBox(Component):
-    """A box that contains text. The background color, text color, text, font_size, and the text being centered can all be set"""
-
-    text = ""
-    font = None
-    font_size = 0
-    background_color = None
-    text_color = None
-    is_centered = False
-
-    def __init__(self, text, font_size, background_color, text_color, is_centered):
-        """ Initializes the object
-
-            :parameter text: String; the text that is displayed
-            :parameter font_size: int; the size of the font
-            :parameter background_color: tuple; the (Red, Green, Blue) values of the text box's background
-            :parameter text_color: tuple; the (Red, Green, Blue) values of the text's color
-            :parameter is_centered: bool; whether the text inside the text box is centered
-
-            :returns: None
-        """
-
-        super().__init__("")
-
-        self.text, self.font_size = text, font_size
-        self.text_color, self.is_centered = text_color, is_centered
-        self.set_background_color(background_color)
-
-        load_text(self.name, font_size, background_color, text_color)
-
-        Dimensions.__init__(self, 0, 0, 0, 0)
-
-    def render(self):
-        """Renders the TextBox onto the screen"""
-
-        super().render()
-
-        left_edge, top_edge = self.left_edge, self.top_edge
-
-        if self.is_centered:
-            left_edge, top_edge = self.horizontal_midpoint, self.vertical_midpoint
-
-        render_text(left_edge, top_edge, self.text_color, self.background_color, self.text, self.font_size, self.is_centered, self.name)
-    def set_background_color(self, background_color):
-        """Sets the background_color of the TextBox by setting 'self.color' and 'self.background_color' to the value provided ('background_color')"""
-
-        self.color, self.background_color = background_color, background_color
-
-    def set_text(self, text):
-        """Sets TextBox 'self.text' attribute to 'text' """
-
+from game_qu.gui_components.dimensions import Dimensions
+from game_qu.base.important_variables import game_window
+from game_qu.gui_components.component import Component
+from game_qu.base.utility_functions import *
+
+class TextBox(Component):
+    """A box that contains text. The background color, text color, text, font_size, and the text being centered can all be set"""
+
+    text = ""
+    font = None
+    font_size = 0
+    background_color = None
+    text_color = None
+    is_centered = False
+
+    def __init__(self, text, font_size, background_color, text_color, is_centered):
+        """ Initializes the object
+
+            :parameter text: String; the text that is displayed
+            :parameter font_size: int; the size of the font
+            :parameter background_color: tuple; the (Red, Green, Blue) values of the text box's background
+            :parameter text_color: tuple; the (Red, Green, Blue) values of the text's color
+            :parameter is_centered: bool; whether the text inside the text box is centered
+
+            :returns: None
+        """
+
+        super().__init__("")
+
+        self.text, self.font_size = text, font_size
+        self.text_color, self.is_centered = text_color, is_centered
+        self.set_background_color(background_color)
+
+        load_text(self.name, font_size, background_color, text_color)
+
+        Dimensions.__init__(self, 0, 0, 0, 0)
+
+    def render(self):
+        """Renders the TextBox onto the screen"""
+
+        super().render()
+
+        left_edge, top_edge = self.left_edge, self.top_edge
+
+        if self.is_centered:
+            left_edge, top_edge = self.horizontal_midpoint, self.vertical_midpoint
+
+        render_text(left_edge, top_edge, self.text_color, self.background_color, self.text, self.font_size, self.is_centered, self.name)
+    def set_background_color(self, background_color):
+        """Sets the background_color of the TextBox by setting 'self.color' and 'self.background_color' to the value provided ('background_color')"""
+
+        self.color, self.background_color = background_color, background_color
+
+    def set_text(self, text):
+        """Sets TextBox 'self.text' attribute to 'text' """
+
         self.text = text
```

### Comparing `game_qu-2.0.0/src/game_qu/gui_components/window.py` & `game_qu-2.0.1/src/game_qu/gui_components/window.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from game_qu.library_abstraction import utility_functions
-
-
-class Window:
-    """Shows everything onto the users screen through adding components to it and displaying those added components"""
-
-    screens = []
-
-    def __init__(self, length, height, BACKGROUND_COLOR, title):
-        """ Creates a window with the length, height, and title of the values given
-
-            :parameter length: int; the length of the window
-            :parameter height: int; the height of the window
-            :parameter BACKGROUND_COLOR: tuple; the (Red, Green, Blue) values of the window's background
-            :parameter title: String; the title displayed of the window
-
-            :returns: None
-        """
-
-        utility_functions.set_up_window(length, height, BACKGROUND_COLOR, title)
-
-    def add_screen(self, screen):
-        """Adds the screen to 'self.screens' so the Window keeps track of it"""
-
-        self.screens.append(screen)
-
-    def display_screen(self, screen):
-        """ Makes all the other screen's invisible by setting their 'is_visible' attribute to False and makes the 'screen'
-            visible by setting it's 'is_visible' attribute set to True"""
-
-        for other_screen in self.screens:
-            other_screen.is_visible = False
-
-        screen.is_visible = True
-
-    def run(self, should_render):
-        """ Calls the run() and render_background() method of all visible screens. It will also call the run() and render()
-            methods for each of the Component(s) that the get_components() method returns for the visible screens"""
-
-        for screen in self.screens:
-            if not screen.is_visible:
-                continue
-
-            if screen.is_visible:
-                screen.run()
-
-            if screen.is_visible and should_render:
-                screen.render_background()
-
-            for component in screen.get_components():
-
-                if component.is_runnable:
-                    component.run()
-
-                if should_render:
-                    component.render()
+from game_qu.library_abstraction import utility_functions
+
+
+class Window:
+    """Shows everything onto the users screen through adding components to it and displaying those added components"""
+
+    screens = []
+
+    def __init__(self, length, height, BACKGROUND_COLOR, title):
+        """ Creates a window with the length, height, and title of the values given
+
+            :parameter length: int; the length of the window
+            :parameter height: int; the height of the window
+            :parameter BACKGROUND_COLOR: tuple; the (Red, Green, Blue) values of the window's background
+            :parameter title: String; the title displayed of the window
+
+            :returns: None
+        """
+
+        utility_functions.set_up_window(length, height, BACKGROUND_COLOR, title)
+
+    def add_screen(self, screen):
+        """Adds the screen to 'self.screens' so the Window keeps track of it"""
+
+        self.screens.append(screen)
+
+    def display_screen(self, screen):
+        """ Makes all the other screen's invisible by setting their 'is_visible' attribute to False and makes the 'screen'
+            visible by setting it's 'is_visible' attribute set to True"""
+
+        for other_screen in self.screens:
+            other_screen.is_visible = False
+
+        screen.is_visible = True
+
+    def run(self, should_render):
+        """ Calls the run() and render_background() method of all visible screens. It will also call the run() and render()
+            methods for each of the Component(s) that the get_components() method returns for the visible screens"""
+
+        for screen in self.screens:
+            if not screen.is_visible:
+                continue
+
+            if screen.is_visible:
+                screen.run()
+
+            if screen.is_visible and should_render:
+                screen.render_background()
+
+            for component in screen.get_components():
+
+                if component.is_runnable:
+                    component.run()
+
+                if should_render:
+                    component.render()
```

### Comparing `game_qu-2.0.0/src/game_qu/pygame_abstraction/utility_functions.py` & `game_qu-2.0.1/src/game_qu/pygame_abstraction/utility_functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,173 +1,176 @@
-from game_qu.pygame_abstraction import variables
-from game_qu.pygame_abstraction.keys import *
-import pygame
-import time
-
-fonts = {}
-images = {}
-
-def convert_to_int(*args):
-    """:returns: int[len(args)]; the args as int"""
-
-    return_value = []
-
-    for arg in args:
-        return_value.append(int(arg))
-
-    return return_value
-
-def load_image(path_to_image):
-    """ Loads the image from that path_to_image for quick rendering (should be called before the game starts running)
-        :returns: int[] {image_length, image_height}; the length and height of the image"""
-
-    if images.get(path_to_image) is None:
-        images[path_to_image] = pygame.image.load(path_to_image).convert_alpha()
-    return images[path_to_image].get_size()
-
-def load_text(name, font_size, background_color, text_color):
-    """Loads the text for quick rendering (should be called before the game starts running)"""
-
-    if fonts.get(font_size) is None:
-        fonts[font_size] = pygame.font.Font("freesansbold.ttf", font_size)
-
-def render_text(left_edge, top_edge, text_color, background_color, text, font_size, is_centered, name):
-    """Renders the text onto the screen"""
-
-    left_edge, top_edge = convert_to_int(left_edge, top_edge)
-
-    font = fonts.get(font_size)
-    rendered_text = font.render(text, True, text_color, background_color)
-    text_rectangle = rendered_text.get_rect()
-
-    if is_centered:
-        text_rectangle.center = [left_edge, top_edge]
-
-    else:
-        text_rectangle.left = left_edge
-        text_rectangle.top = top_edge
-
-    variables.window.blit(rendered_text, text_rectangle)
-
-def render_image(path_to_image, left_edge, top_edge, length, height):
-    """Renders the image onto the screen"""
-
-    left_edge, top_edge, length, height = convert_to_int(left_edge, top_edge, length, height)
-    image = images.get(path_to_image)
-    image = pygame.transform.scale(image, (length, height))
-    variables.window.blit(image, (left_edge, top_edge))
-
-def render_rectangle(left_edge, top_edge, length, height, color):
-    """Renders the rectangle onto the screen"""
-
-    left_edge, top_edge, length, height = convert_to_int(left_edge, top_edge, length, height)
-    pygame.draw.rect(variables.window, color, [left_edge, top_edge, length, height])
-
-def set_up_window(length, height, background_color, title):
-    """Initializes all the pygame code, so the game be run and rendered"""
-
-    length, height = convert_to_int(length, height)
-    variables.window = pygame.display.set_mode((length, height))
-    pygame.display.set_caption(title)
-    variables.background_color = background_color
-
-
-def key_is_pressed(keyboard_key):
-    """:returns: bool; if the 'keyboard_key' is currently pressed this game cycle"""
-
-    game_engine_key = keyboard_keys_to_game_engine_keys.get(keyboard_key)
-
-    controls = pygame.key.get_pressed()
-    return controls[game_engine_key]
-
-def button_is_pressed(button):
-    game_engine_button = keyboard_keys_to_game_engine_keys.get(button)
-
-    dpad_buttons = {DPAD_UP: 0, DPAD_DOWN: 0, DPAD_LEFT: 0, DPAD_RIGHT: 0}
-    return_value = None
-
-    if dpad_buttons.get(button) is not None:
-        return_value = dpad_is_pressed(button)
-
-    else:
-        return_value = variables.joystick.get_button(game_engine_button)
-
-    return return_value
-
-def dpad_is_pressed(dpad_button):
-    joystick_axis = 0
-    value_wanted = .8
-
-    if dpad_button == DPAD_UP or dpad_button == DPAD_DOWN:
-        joystick_axis = 1
-
-    if dpad_button == DPAD_LEFT or dpad_button == DPAD_UP:
-        value_wanted = -value_wanted
-
-    return_value = None
-
-    if value_wanted < 0:
-        return_value = variables.joystick.get_axis(joystick_axis) <= value_wanted
-
-    else:
-        return_value = variables.joystick.get_axis(joystick_axis) >= value_wanted
-
-    return return_value
-
-
-def mouse_was_pressed():
-    """:returns: bool; whether the mouse is currently held down this game cycle"""
-
-    return pygame.mouse.get_pressed()[0]
-
-
-def call_every_cycle(function):
-    """Makes pygame call the 'function' given every game cycle (60fps)"""
-
-    while True:
-        start_time = time.time()
-        for event in pygame.event.get():
-            if event.type == pygame.QUIT:
-                # on_close_function()
-                pygame.quit()
-
-        variables.window.fill(variables.background_color)
-
-        function(start_time, True, True)
-        pygame.display.update()
-
-def run_checking_closing():
-    """Runs all the pygame code that checks to make sure the game should be closed"""
-
-    pass
-
-
-def is_mouse_collision(dimensions):
-    """:returns: bool; whether the mouse has collided with that rectangle - dimensions (left_edge, top_edge, length, height)"""
-
-    area = pygame.Rect(dimensions.left_edge, dimensions.top_edge, dimensions.length, dimensions.height)
-    mouse_left_edge, mouse_top_edge = pygame.mouse.get_pos()
-    return area.collidepoint(mouse_left_edge, mouse_top_edge)
-
-
-def get_time_passed(start_time):
-    """:returns: bool; the amount of time that has passed between the current time and start time"""
-
-    return time.time() - start_time
-
-
-def load_and_transform_image(image_path):
-    """Loads the image at the 'image_path' then it also loads an image that is the horizontal mirror of the original image"""
-
-    base_image = pygame.image.load(f"{image_path}_right.png").convert_alpha()
-    transformed_image = pygame.transform.flip(base_image, True, False)
-
-    images[f"{image_path}_right.png"] = base_image
-    images[f"{image_path}_left.png"] = transformed_image
-
-
-def get_directional_path_to_image(base_image_path, direction_is_right, additional_path_after_direction):
-    """:returns: str; the path to the image that includes direction"""
-
-    direction_image_path = "right" if direction_is_right else "left"
-
-    return f"{base_image_path}_{direction_image_path}{additional_path_after_direction}.png"
+from game_qu.pygame_abstraction import variables
+from game_qu.pygame_abstraction.keys import *
+import pygame
+from game_qu.base import important_constants
+import time
+
+fonts = {}
+images = {}
+
+def convert_to_int(*args):
+    """:returns: int[len(args)]; the args as int"""
+
+    return_value = []
+
+    for arg in args:
+        return_value.append(int(arg))
+
+    return return_value
+
+def load_image(path_to_image):
+    """ Loads the image from that path_to_image for quick rendering (should be called before the game starts running)
+        :returns: int[] {image_length, image_height}; the length and height of the image"""
+
+    if images.get(path_to_image) is None:
+        images[path_to_image] = pygame.image.load(path_to_image).convert_alpha()
+    return images[path_to_image].get_size()
+
+def load_text(name, font_size, background_color, text_color):
+    """Loads the text for quick rendering (should be called before the game starts running)"""
+
+    if fonts.get(font_size) is None:
+        fonts[font_size] = pygame.font.Font("freesansbold.ttf", font_size)
+
+def render_text(left_edge, top_edge, text_color, background_color, text, font_size, is_centered, name):
+    """Renders the text onto the screen"""
+
+    left_edge, top_edge = convert_to_int(left_edge, top_edge)
+
+    font = fonts.get(font_size)
+    rendered_text = font.render(text, True, text_color, background_color)
+    text_rectangle = rendered_text.get_rect()
+
+    if is_centered:
+        text_rectangle.center = [left_edge, top_edge]
+
+    else:
+        text_rectangle.left = left_edge
+        text_rectangle.top = top_edge
+
+    variables.window.blit(rendered_text, text_rectangle)
+
+def render_image(path_to_image, left_edge, top_edge, length, height):
+    """Renders the image onto the screen"""
+
+    left_edge, top_edge, length, height = convert_to_int(left_edge, top_edge, length, height)
+    image = images.get(path_to_image)
+    image = pygame.transform.scale(image, (length, height))
+    variables.window.blit(image, (left_edge, top_edge))
+
+def render_rectangle(left_edge, top_edge, length, height, color):
+    """Renders the rectangle onto the screen"""
+
+    left_edge, top_edge, length, height = convert_to_int(left_edge, top_edge, length, height)
+    pygame.draw.rect(variables.window, color, [left_edge, top_edge, length, height])
+
+def set_up_window(length, height, background_color, title):
+    """Initializes all the pygame code, so the game be run and rendered"""
+
+    if not important_constants.IS_FULL_SCREEN:
+        length, height = convert_to_int(length, height)
+        variables.window = pygame.display.set_mode((length, height))
+
+    pygame.display.set_caption(title)
+    variables.background_color = background_color
+
+
+def key_is_pressed(keyboard_key):
+    """:returns: bool; if the 'keyboard_key' is currently pressed this game cycle"""
+
+    game_engine_key = keyboard_keys_to_game_engine_keys.get(keyboard_key)
+
+    controls = pygame.key.get_pressed()
+    return controls[game_engine_key]
+
+def button_is_pressed(button):
+    game_engine_button = keyboard_keys_to_game_engine_keys.get(button)
+
+    dpad_buttons = {DPAD_UP: 0, DPAD_DOWN: 0, DPAD_LEFT: 0, DPAD_RIGHT: 0}
+    return_value = None
+
+    if dpad_buttons.get(button) is not None:
+        return_value = dpad_is_pressed(button)
+
+    else:
+        return_value = variables.joystick.get_button(game_engine_button)
+
+    return return_value
+
+def dpad_is_pressed(dpad_button):
+    joystick_axis = 0
+    value_wanted = .8
+
+    if dpad_button == DPAD_UP or dpad_button == DPAD_DOWN:
+        joystick_axis = 1
+
+    if dpad_button == DPAD_LEFT or dpad_button == DPAD_UP:
+        value_wanted = -value_wanted
+
+    return_value = None
+
+    if value_wanted < 0:
+        return_value = variables.joystick.get_axis(joystick_axis) <= value_wanted
+
+    else:
+        return_value = variables.joystick.get_axis(joystick_axis) >= value_wanted
+
+    return return_value
+
+
+def mouse_was_pressed():
+    """:returns: bool; whether the mouse is currently held down this game cycle"""
+
+    return pygame.mouse.get_pressed()[0]
+
+
+def call_every_cycle(function):
+    """Makes pygame call the 'function' given every game cycle (60fps)"""
+
+    while True:
+        start_time = time.time()
+        for event in pygame.event.get():
+            if event.type == pygame.QUIT:
+                # on_close_function()
+                pygame.quit()
+
+        variables.window.fill(variables.background_color)
+
+        function(start_time, True, True)
+        pygame.display.update()
+
+def run_checking_closing():
+    """Runs all the pygame code that checks to make sure the game should be closed"""
+
+    pass
+
+
+def is_mouse_collision(dimensions):
+    """:returns: bool; whether the mouse has collided with that rectangle - dimensions (left_edge, top_edge, length, height)"""
+
+    area = pygame.Rect(dimensions.left_edge, dimensions.top_edge, dimensions.length, dimensions.height)
+    mouse_left_edge, mouse_top_edge = pygame.mouse.get_pos()
+    return area.collidepoint(mouse_left_edge, mouse_top_edge)
+
+
+def get_time_passed(start_time):
+    """:returns: bool; the amount of time that has passed between the current time and start time"""
+
+    return time.time() - start_time
+
+
+def load_and_transform_image(image_path):
+    """Loads the image at the 'image_path' then it also loads an image that is the horizontal mirror of the original image"""
+
+    base_image = pygame.image.load(f"{image_path}_right.png").convert_alpha()
+    transformed_image = pygame.transform.flip(base_image, True, False)
+
+    images[f"{image_path}_right.png"] = base_image
+    images[f"{image_path}_left.png"] = transformed_image
+
+
+def get_directional_path_to_image(base_image_path, direction_is_right, additional_path_after_direction):
+    """:returns: str; the path to the image that includes direction"""
+
+    direction_image_path = "right" if direction_is_right else "left"
+
+    return f"{base_image_path}_{direction_image_path}{additional_path_after_direction}.png"
```

