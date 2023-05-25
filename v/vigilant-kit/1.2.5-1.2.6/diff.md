# Comparing `tmp/vigilant_kit-1.2.5.tar.gz` & `tmp/vigilant_kit-1.2.6.tar.gz`

## Comparing `vigilant_kit-1.2.5.tar` & `vigilant_kit-1.2.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/.vigilant.env.example
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/vigilant.json.example
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/bin/doc_generator.py
--rw-r--r--   0        0        0    28724 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/docs/actions.md
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/docs/browser_options.md
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/docs/configuration.md
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/docs/native_selenium.md
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/docs/selenium_install.md
--rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/docs/tutorial_pytest.md
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/docs/vigilant_pytest.md
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/docs/vigilant_unittest.md
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/src/vgl_cli/install_dev_kit_command.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/src/vgl_cli/install_standalone_command.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/src/vgl_cli/install_webdriver_command.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/src/vgl_cli/run_selenium_command.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/src/vgl_cli/vgl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/src/vigilant/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/src/vigilant/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/src/vigilant/actions/__init__.py
--rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/src/vigilant/actions/assertions.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/src/vigilant/actions/finder.py
--rw-r--r--   0        0        0    11684 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/src/vigilant/actions/vigilant_actions.py
--rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/src/vigilant/actions/waiter.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/src/vigilant/driver/__init__.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/src/vigilant/driver/vigilant_driver.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/.gitignore
--rw-r--r--   0        0        0    35125 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/LICENSE
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/README.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 vigilant_kit-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/.vigilant.env.example
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/vigilant.json.example
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/bin/doc_generator.py
+-rw-r--r--   0        0        0    30712 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/docs/actions.md
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/docs/browser_options.md
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/docs/configuration.md
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/docs/native_selenium.md
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/docs/selenium_install.md
+-rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/docs/tutorial_pytest.md
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/docs/vigilant_pytest.md
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/docs/vigilant_unittest.md
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vgl_cli/install_dev_kit_command.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vgl_cli/install_standalone_command.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vgl_cli/install_webdriver_command.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vgl_cli/run_selenium_command.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vgl_cli/vgl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vigilant/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vigilant/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vigilant/actions/__init__.py
+-rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vigilant/actions/assertions.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vigilant/actions/finder.py
+-rw-r--r--   0        0        0    13552 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vigilant/actions/vigilant_actions.py
+-rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vigilant/actions/waiter.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vigilant/driver/__init__.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vigilant/driver/vigilant_driver.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/.gitignore
+-rw-r--r--   0        0        0    35125 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/LICENSE
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/README.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/PKG-INFO
```

### Comparing `vigilant_kit-1.2.5/bin/doc_generator.py` & `vigilant_kit-1.2.6/bin/doc_generator.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/docs/actions.md` & `vigilant_kit-1.2.6/docs/actions.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 - [get_base_url](#get_base_url)
 - [get_cookie](#get_cookie)
 - [get_page_title](#get_page_title)
 - [get_text_from_element](#get_text_from_element)
 - [get_timeout](#get_timeout)
 - [maximize_window](#maximize_window)
 - [move_mouse_on_element](#move_mouse_on_element)
+- [open_new_tab](#open_new_tab)
+- [open_new_window](#open_new_window)
 - [page_back](#page_back)
 - [page_forward](#page_forward)
 - [page_refresh](#page_refresh)
 - [press_key](#press_key)
 - [quit](#quit)
 - [resize_window](#resize_window)
 - [scroll_to](#scroll_to)
@@ -44,14 +46,17 @@
 - [see_text](#see_text)
 - [send_keys](#send_keys)
 - [set_cookie](#set_cookie)
 - [strict_wait](#strict_wait)
 - [submit_form](#submit_form)
 - [switch_to_default](#switch_to_default)
 - [switch_to_frame](#switch_to_frame)
+- [switch_to_next_tab](#switch_to_next_tab)
+- [switch_to_previous_tab](#switch_to_previous_tab)
+- [switch_to_window](#switch_to_window)
 - [type_in_alert](#type_in_alert)
 - [wait_for_alert_](#wait_for_alert_)
 - [wait_for_element_to_be_present_in_dom](#wait_for_element_to_be_present_in_dom)
 - [wait_for_element_to_be_visible](#wait_for_element_to_be_visible)
 - [wait_for_element_to_disappear](#wait_for_element_to_disappear)
 - [wait_for_text_to_be_present_in_element](#wait_for_text_to_be_present_in_element)
 - [wait_for_text_to_be_present_in_element_attribute](#wait_for_text_to_be_present_in_element_attribute)
@@ -103,15 +108,15 @@
         Clears a field after it becomes visible.
 
         :param selector: The field to clear
         :return: self
         
 
 ```python
-# src/vigilant/actions/vigilant_actions.py (line 376)
+# src/vigilant/actions/vigilant_actions.py (line 433)
 def clear_field(self, selector) -> return_type:
     """
         Clears a field after it becomes visible.
 
         :param selector: The field to clear
         :return: self
         """
@@ -371,15 +376,15 @@
 
         :param selector: The field to fill
         :param value: The value to fill in the field
         :return: self
         
 
 ```python
-# src/vigilant/actions/vigilant_actions.py (line 301)
+# src/vigilant/actions/vigilant_actions.py (line 317)
 def fill_field(self, selector, value) -> return_type:
     """
         Fills a field with a specified value after the field becomes visible.
 
         :param selector: The field to fill
         :param value: The value to fill in the field
         :return: self
@@ -393,15 +398,15 @@
         Fills multiple fields in a form using a dictionary of selectors and values.
 
         :param selector_data: A dictionary of selectors and values
         :return: self
         
 
 ```python
-# src/vigilant/actions/vigilant_actions.py (line 314)
+# src/vigilant/actions/vigilant_actions.py (line 330)
 def fill_form(self, selector_data) -> return_type:
     """
         Fills multiple fields in a form using a dictionary of selectors and values.
 
         :param selector_data: A dictionary of selectors and values
         :return: self
         """
@@ -574,15 +579,15 @@
         Gets the text from an element after it becomes visible.
 
         :param selector: The element to get text from
         :return: The text of the element
         
 
 ```python
-# src/vigilant/actions/vigilant_actions.py (line 290)
+# src/vigilant/actions/vigilant_actions.py (line 306)
 def get_text_from_element(self, selector) -> return_type:
     """
         Gets the text from an element after it becomes visible.
 
         :param selector: The element to get text from
         :return: The text of the element
         """
@@ -635,25 +640,63 @@
         Moves the mouse cursor over an element after the element becomes visible.
 
         :param selector: The element to move the mouse cursor over
         :return: self
         
 
 ```python
-# src/vigilant/actions/vigilant_actions.py (line 328)
+# src/vigilant/actions/vigilant_actions.py (line 344)
 def move_mouse_on_element(self, selector) -> return_type:
     """
         Moves the mouse cursor over an element after the element becomes visible.
 
         :param selector: The element to move the mouse cursor over
         :return: self
         """
     # Function code goes here
 ```
 
+## open_new_tab
+
+
+        Opens a new tab and switches to it
+
+        :return: self
+        
+
+```python
+# src/vigilant/actions/vigilant_actions.py (line 287)
+def open_new_tab(self) -> return_type:
+    """
+        Opens a new tab and switches to it
+
+        :return: self
+        """
+    # Function code goes here
+```
+
+## open_new_window
+
+
+        Opens a new window and switches to new window
+
+        :return: self
+        
+
+```python
+# src/vigilant/actions/vigilant_actions.py (line 279)
+def open_new_window(self) -> return_type:
+    """
+        Opens a new window and switches to new window
+
+        :return: self
+        """
+    # Function code goes here
+```
+
 ## page_back
 
 
         Goes one step backward in the browser history.
 
         :return: self
         
@@ -713,15 +756,15 @@
         Presses a specified key.
 
         :param key: The key to press
         :return: self
         
 
 ```python
-# src/vigilant/actions/vigilant_actions.py (line 341)
+# src/vigilant/actions/vigilant_actions.py (line 357)
 def press_key(self, key) -> return_type:
     """
         Presses a specified key.
 
         :param key: The key to press
         :return: self
         """
@@ -776,15 +819,15 @@
         Scrolls to an element.
 
         :param selector: The element to scroll to
         :return: self
         
 
 ```python
-# src/vigilant/actions/vigilant_actions.py (line 279)
+# src/vigilant/actions/vigilant_actions.py (line 295)
 def scroll_to(self, selector) -> return_type:
     """
         Scrolls to an element.
 
         :param selector: The element to scroll to
         :return: self
         """
@@ -914,15 +957,15 @@
 
         :param selector: The field to send keys to
         :param keys: The keys to send
         :return: self
         
 
 ```python
-# src/vigilant/actions/vigilant_actions.py (line 353)
+# src/vigilant/actions/vigilant_actions.py (line 369)
 def send_keys(self, selector, keys) -> return_type:
     """
         Sends keys to a specified field.
 
         :param selector: The field to send keys to
         :param keys: The keys to send
         :return: self
@@ -976,15 +1019,15 @@
         Submits a form using a specified selector.
 
         :param selector: The form to submit
         :return: self
         
 
 ```python
-# src/vigilant/actions/vigilant_actions.py (line 365)
+# src/vigilant/actions/vigilant_actions.py (line 381)
 def submit_form(self, selector) -> return_type:
     """
         Submits a form using a specified selector.
 
         :param selector: The form to submit
         :return: self
         """
@@ -1027,14 +1070,73 @@
 
         :param frame_id: The ID of the frame to switch to
         :return: self
         """
     # Function code goes here
 ```
 
+## switch_to_next_tab
+
+
+        Switch to the next tab
+
+        :return: self
+        
+
+```python
+# src/vigilant/actions/vigilant_actions.py (line 392)
+def switch_to_next_tab(self) -> return_type:
+    """
+        Switch to the next tab
+
+        :return: self
+        """
+    # Function code goes here
+```
+
+## switch_to_previous_tab
+
+
+        Switch to the previous tab
+
+        :return: self
+        
+
+```python
+# src/vigilant/actions/vigilant_actions.py (line 405)
+def switch_to_previous_tab(self) -> return_type:
+    """
+        Switch to the previous tab
+
+        :return: self
+        """
+    # Function code goes here
+```
+
+## switch_to_window
+
+
+        Switch to the window identify by window name(title).
+
+        :param  window_name: Window title to switch on
+        :return: self
+        
+
+```python
+# src/vigilant/actions/vigilant_actions.py (line 418)
+def switch_to_window(self, window_name: str) -> return_type:
+    """
+        Switch to the window identify by window name(title).
+
+        :param  window_name: Window title to switch on
+        :return: self
+        """
+    # Function code goes here
+```
+
 ## type_in_alert
 
 
         Types the specified value in the alert.
 
         :param value: The value to type in the alert
         :return: self
```

### Comparing `vigilant_kit-1.2.5/docs/browser_options.md` & `vigilant_kit-1.2.6/docs/browser_options.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/docs/configuration.md` & `vigilant_kit-1.2.6/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/docs/native_selenium.md` & `vigilant_kit-1.2.6/docs/native_selenium.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/docs/selenium_install.md` & `vigilant_kit-1.2.6/docs/selenium_install.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/docs/tutorial_pytest.md` & `vigilant_kit-1.2.6/docs/tutorial_pytest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/docs/vigilant_pytest.md` & `vigilant_kit-1.2.6/docs/vigilant_pytest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/docs/vigilant_unittest.md` & `vigilant_kit-1.2.6/docs/vigilant_unittest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/src/vgl_cli/install_dev_kit_command.py` & `vigilant_kit-1.2.6/src/vgl_cli/install_dev_kit_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/src/vgl_cli/install_standalone_command.py` & `vigilant_kit-1.2.6/src/vgl_cli/install_standalone_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/src/vgl_cli/install_webdriver_command.py` & `vigilant_kit-1.2.6/src/vgl_cli/install_webdriver_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/src/vgl_cli/run_selenium_command.py` & `vigilant_kit-1.2.6/src/vgl_cli/run_selenium_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/src/vgl_cli/vgl.py` & `vigilant_kit-1.2.6/src/vgl_cli/vgl.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/src/vigilant/actions/assertions.py` & `vigilant_kit-1.2.6/src/vigilant/actions/assertions.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/src/vigilant/actions/finder.py` & `vigilant_kit-1.2.6/src/vigilant/actions/finder.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/src/vigilant/actions/vigilant_actions.py` & `vigilant_kit-1.2.6/src/vigilant/actions/vigilant_actions.py`

 * *Files 15% similar despite different names*

```diff
@@ -272,14 +272,32 @@
         :param selector: The element to click on
         :return: self
         """
         self.waiter.wait_for_element_to_be_visible(selector)
         log.info(f'Clicking on element: {selector}')
         self.finder.find(selector).click()
 
+    def open_new_window(self):
+        """
+        Opens a new window and switches to new window
+
+        :return: self
+        """
+        log.info(f'Opening new window')
+        self.driver.switch_to.new_window('window')
+
+    def open_new_tab(self):
+        """
+        Opens a new tab and switches to it
+
+        :return: self
+        """
+        log.info(f'Opening new tab')
+        self.driver.switch_to.new_window('tab')
+
     def scroll_to(self, selector):
         """
         Scrolls to an element.
 
         :param selector: The element to scroll to
         :return: self
         """
@@ -369,14 +387,55 @@
         :param selector: The form to submit
         :return: self
         """
         log.info(f'Submitting form: {selector}')
         self.finder.find(selector).submit()
         return self
 
+    def switch_to_next_tab(self):
+        """
+        Switch to the next tab
+
+        :return: self
+        """
+        window_handles = self.driver.window_handles
+        current_tab_index = window_handles.index(self.driver.current_window_handle)
+        next_tab_index = (current_tab_index + 1) % len(window_handles)
+        log.info(f'Switching to the next tab')
+        self.driver.switch_to.window(window_handles[next_tab_index])
+        return self
+
+    def switch_to_previous_tab(self):
+        """
+        Switch to the previous tab
+
+        :return: self
+        """
+        window_handles = self.driver.window_handles
+        current_tab_index = window_handles.index(self.driver.current_window_handle)
+        next_tab_index = (current_tab_index - 1) % len(window_handles)
+        log.info(f'Switching to the previous tab')
+        self.driver.switch_to.window(window_handles[next_tab_index])
+        return self
+
+    def switch_to_window(self, window_name: str):
+        """
+        Switch to the window identify by window name(title).
+
+        :param  window_name: Window title to switch on
+        :return: self
+        """
+        # Iterate through all window handles
+        for handle in self.driver.window_handles:
+            self.driver.switch_to.window(handle)
+            if self.driver.title == window_name:
+                log.info(f'Switching to the window {window_name}')
+                break
+        return self
+
     def clear_field(self, selector):
         """
         Clears a field after it becomes visible.
 
         :param selector: The field to clear
         :return: self
         """
```

### Comparing `vigilant_kit-1.2.5/src/vigilant/actions/waiter.py` & `vigilant_kit-1.2.6/src/vigilant/actions/waiter.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/src/vigilant/driver/__init__.py` & `vigilant_kit-1.2.6/src/vigilant/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/src/vigilant/driver/vigilant_driver.py` & `vigilant_kit-1.2.6/src/vigilant/driver/vigilant_driver.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/.gitignore` & `vigilant_kit-1.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/LICENSE` & `vigilant_kit-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/README.md` & `vigilant_kit-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.5/pyproject.toml` & `vigilant_kit-1.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vigilant_kit"
-version = "1.2.5"
+version = "1.2.6"
 authors = [
   { name="Pelykh Ivan", email="ivan.pelykh@protonmail.com" },
 ]
 description = "Library that makes functional testing with Selenium WebDriver fast and easy. "
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `vigilant_kit-1.2.5/PKG-INFO` & `vigilant_kit-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vigilant_kit
-Version: 1.2.5
+Version: 1.2.6
 Summary: Library that makes functional testing with Selenium WebDriver fast and easy. 
 Project-URL: Homepage, https://github.com/ivpel/vigilant
 Project-URL: Bug Tracker, https://github.com/ivpel/vigilant/issues
 Author-email: Pelykh Ivan <ivan.pelykh@protonmail.com>
 License-File: LICENSE
 Keywords: bdd,functional,functional-testing,pytest,selenium,tdd,testing,unittest,webdriver
 Requires-Python: >=3.7
```

