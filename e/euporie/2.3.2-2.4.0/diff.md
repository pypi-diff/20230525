# Comparing `tmp/euporie-2.3.2.tar.gz` & `tmp/euporie-2.4.0.tar.gz`

## Comparing `euporie-2.3.2.tar` & `euporie-2.4.0.tar`

### file list

```diff
@@ -1,122 +1,127 @@
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/console/__init__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/console/__main__.py
--rw-r--r--   0        0        0     7655 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/console/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/console/py.typed
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/console/tabs/__init__.py
--rw-r--r--   0        0        0    22732 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/console/tabs/console.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/__init__.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/__main__.py
--rw-r--r--   0        0        0    41099 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/app.py
--rw-r--r--   0        0        0    44698 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/border.py
--rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/commands.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/completion.py
--rw-r--r--   0        0        0    21070 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/config.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/current.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/data_structures.py
--rw-r--r--   0        0        0     8064 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/filters.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/format.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/history.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/io.py
--rw-r--r--   0        0        0    40515 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/kernel.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/keys.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/launch.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/lexers.py
--rw-r--r--   0        0        0    15809 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/log.py
--rw-r--r--   0        0        0    20562 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/margins.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/processors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/py.typed
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/pygments.py
--rw-r--r--   0        0        0    65039 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/reference.py
--rw-r--r--   0        0        0    16092 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/renderer.py
--rw-r--r--   0        0        0    29856 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/style.py
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/suggest.py
--rw-r--r--   0        0        0    14330 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/terminal.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/url.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/utils.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/validation.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/comm/__init__.py
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/comm/base.py
--rw-r--r--   0        0        0    52669 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/comm/ipywidgets.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/comm/registry.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/convert/__init__.py
--rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/convert/base.py
--rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/convert/utils.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/convert/formats/__init__.py
--rw-r--r--   0        0        0    12940 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/convert/formats/ansi.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/convert/formats/base64.py
--rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/convert/formats/common.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/convert/formats/formatted_text.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/convert/formats/html.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/convert/formats/jpeg.py
--rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/convert/formats/markdown.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/convert/formats/pdf.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/convert/formats/pil.py
--rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/convert/formats/png.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/convert/formats/rich.py
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/convert/formats/sixel.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/formatted_text/__init__.py
--rw-r--r--   0        0        0     5830 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/formatted_text/ansi.py
--rw-r--r--   0        0        0   112986 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/formatted_text/html.py
--rw-r--r--   0        0        0     5603 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/formatted_text/markdown.py
--rw-r--r--   0        0        0    40909 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/formatted_text/table.py
--rw-r--r--   0        0        0    27172 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/formatted_text/utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/key_binding/__init__.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/key_binding/key_processor.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/key_binding/micro_state.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/key_binding/registry.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/key_binding/utils.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/key_binding/vi_state.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/key_binding/bindings/__init__.py
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/key_binding/bindings/completion.py
--rw-r--r--   0        0        0    28546 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/key_binding/bindings/micro.py
--rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/key_binding/bindings/mouse.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/tabs/__init__.py
--rw-r--r--   0        0        0    10949 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/tabs/base.py
--rw-r--r--   0        0        0    13915 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/tabs/notebook.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/widgets/__init__.py
--rw-r--r--   0        0        0    29828 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/widgets/cell.py
--rw-r--r--   0        0        0    15741 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/widgets/cell_outputs.py
--rw-r--r--   0        0        0    22472 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/widgets/decor.py
--rw-r--r--   0        0        0    28706 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/widgets/dialog.py
--rw-r--r--   0        0        0    48171 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/widgets/display.py
--rw-r--r--   0        0        0    17525 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/widgets/file_browser.py
--rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/widgets/formatted_text_area.py
--rw-r--r--   0        0        0    81142 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/widgets/forms.py
--rw-r--r--   0        0        0    12793 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/widgets/inputs.py
--rw-r--r--   0        0        0    20628 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/widgets/layout.py
--rw-r--r--   0        0        0    24742 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/widgets/menu.py
--rw-r--r--   0        0        0    41098 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/widgets/page.py
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/widgets/pager.py
--rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/widgets/palette.py
--rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/widgets/search_bar.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/widgets/status_bar.py
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/core/widgets/tree.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/hub/__init__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/hub/__main__.py
--rw-r--r--   0        0        0     6041 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/hub/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/hub/py.typed
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/notebook/__init__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/notebook/__main__.py
--rw-r--r--   0        0        0    21154 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/notebook/app.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/notebook/current.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/notebook/enums.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/notebook/filters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/notebook/py.typed
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/notebook/tabs/__init__.py
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/notebook/tabs/display.py
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/notebook/tabs/edit.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/notebook/tabs/log.py
--rw-r--r--   0        0        0    41043 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/notebook/tabs/notebook.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/notebook/widgets/__init__.py
--rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/notebook/widgets/side_bar.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/preview/__init__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/preview/__main__.py
--rw-r--r--   0        0        0     8741 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/preview/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/preview/py.typed
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/preview/tabs/__init__.py
--rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 euporie-2.3.2/euporie/preview/tabs/notebook.py
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 euporie-2.3.2/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 euporie-2.3.2/LICENSE
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 euporie-2.3.2/README.rst
--rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 euporie-2.3.2/pyproject.toml
--rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 euporie-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/console/__init__.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/console/__main__.py
+-rw-r--r--   0        0        0     7667 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/console/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/console/py.typed
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/console/tabs/__init__.py
+-rw-r--r--   0        0        0    23533 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/console/tabs/console.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/__init__.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/__main__.py
+-rw-r--r--   0        0        0    40124 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/app.py
+-rw-r--r--   0        0        0    46884 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/border.py
+-rw-r--r--   0        0        0     7794 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/commands.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/completion.py
+-rw-r--r--   0        0        0    21438 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/config.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/current.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/data_structures.py
+-rw-r--r--   0        0        0     8064 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/filters.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/format.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/history.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/io.py
+-rw-r--r--   0        0        0    41091 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/kernel.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/keys.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/launch.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/lexers.py
+-rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/log.py
+-rw-r--r--   0        0        0    21206 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/margins.py
+-rw-r--r--   0        0        0     7946 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/path.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/processors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/py.typed
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/pygments.py
+-rw-r--r--   0        0        0    65039 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/reference.py
+-rw-r--r--   0        0        0    16527 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/renderer.py
+-rw-r--r--   0        0        0    30922 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/style.py
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/suggest.py
+-rw-r--r--   0        0        0    14686 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/terminal.py
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/utils.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/validation.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/comm/__init__.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/comm/base.py
+-rw-r--r--   0        0        0    52707 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/comm/ipywidgets.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/comm/registry.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/convert/__init__.py
+-rw-r--r--   0        0        0     8732 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/convert/core.py
+-rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/convert/utils.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/convert/formats/__init__.py
+-rw-r--r--   0        0        0    13555 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/convert/formats/ansi.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/convert/formats/base64.py
+-rw-r--r--   0        0        0     4965 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/convert/formats/common.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/convert/formats/formatted_text.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/convert/formats/html.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/convert/formats/jpeg.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/convert/formats/markdown.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/convert/formats/pdf.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/convert/formats/pil.py
+-rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/convert/formats/png.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/convert/formats/rich.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/convert/formats/sixel.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/formatted_text/__init__.py
+-rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/formatted_text/ansi.py
+-rw-r--r--   0        0        0   143927 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/formatted_text/html.py
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/formatted_text/markdown.py
+-rw-r--r--   0        0        0    41140 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/formatted_text/table.py
+-rw-r--r--   0        0        0    27819 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/formatted_text/utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/key_binding/__init__.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/key_binding/key_processor.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/key_binding/micro_state.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/key_binding/registry.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/key_binding/utils.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/key_binding/vi_state.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/key_binding/bindings/__init__.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/key_binding/bindings/completion.py
+-rw-r--r--   0        0        0    28624 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/key_binding/bindings/micro.py
+-rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/key_binding/bindings/mouse.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/tabs/__init__.py
+-rw-r--r--   0        0        0    13546 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/tabs/base.py
+-rw-r--r--   0        0        0    15648 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/tabs/notebook.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/widgets/__init__.py
+-rw-r--r--   0        0        0    29874 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/widgets/cell.py
+-rw-r--r--   0        0        0    15742 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/widgets/cell_outputs.py
+-rw-r--r--   0        0        0    22153 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/widgets/decor.py
+-rw-r--r--   0        0        0    32257 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/widgets/dialog.py
+-rw-r--r--   0        0        0    49787 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/widgets/display.py
+-rw-r--r--   0        0        0    19842 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/widgets/file_browser.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/widgets/formatted_text_area.py
+-rw-r--r--   0        0        0    82382 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/widgets/forms.py
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/widgets/inputs.py
+-rw-r--r--   0        0        0    20678 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/widgets/layout.py
+-rw-r--r--   0        0        0    30676 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/widgets/menu.py
+-rw-r--r--   0        0        0    42512 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/widgets/page.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/widgets/pager.py
+-rw-r--r--   0        0        0    10814 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/widgets/palette.py
+-rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/widgets/search_bar.py
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/widgets/status_bar.py
+-rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/core/widgets/tree.py
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/data/desktop/euporie-console.desktop
+-rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/data/desktop/euporie-notebook.desktop
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/hub/__init__.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/hub/__main__.py
+-rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/hub/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/hub/py.typed
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/notebook/__init__.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/notebook/__main__.py
+-rw-r--r--   0        0        0    20398 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/notebook/app.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/notebook/current.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/notebook/enums.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/notebook/filters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/notebook/py.typed
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/notebook/tabs/__init__.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/notebook/tabs/display.py
+-rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/notebook/tabs/edit.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/notebook/tabs/json.py
+-rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/notebook/tabs/log.py
+-rw-r--r--   0        0        0    41796 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/notebook/tabs/notebook.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/notebook/widgets/__init__.py
+-rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/notebook/widgets/side_bar.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/preview/__init__.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/preview/__main__.py
+-rw-r--r--   0        0        0     8769 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/preview/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/preview/py.typed
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/preview/tabs/__init__.py
+-rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/preview/tabs/notebook.py
+-rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/web/tabs/web.py
+-rw-r--r--   0        0        0    19186 2020-02-02 00:00:00.000000 euporie-2.4.0/euporie/web/widgets/webview.py
+-rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 euporie-2.4.0/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 euporie-2.4.0/LICENSE
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 euporie-2.4.0/README.rst
+-rw-r--r--   0        0        0     5838 2020-02-02 00:00:00.000000 euporie-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 euporie-2.4.0/PKG-INFO
```

### Comparing `euporie-2.3.2/euporie/console/app.py` & `euporie-2.4.0/euporie/console/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     FloatContainer,
     HSplit,
     VSplit,
     Window,
 )
 from prompt_toolkit.layout.dimension import Dimension
 
-from euporie.console.tabs.console import ConsoleTab
+from euporie.console.tabs.console import Console
 from euporie.core import __logo__
 from euporie.core.app import BaseApp
 from euporie.core.commands import add_cmd
 from euporie.core.config import add_setting
 from euporie.core.filters import buffer_is_code, buffer_is_empty, has_dialog
 from euporie.core.key_binding.registry import register_bindings
 from euporie.core.widgets.dialog import (
@@ -78,15 +78,15 @@
 
         # Initialize the application
         super().__init__(**kwargs)
 
         self.search_bar = SearchBar()
         self.bindings_to_load += ["euporie.console.app.ConsoleApp"]
 
-        self.tabs = [ConsoleTab(self)]
+        self.tabs = []
         self.pager = Pager()
 
         self.config.get_item("mouse_support").event += lambda x: setattr(
             self, "need_mouse_support", x.value
         )
 
     def _get_reserved_height(self) -> Dimension:
@@ -95,14 +95,16 @@
         elif has_completions():
             return Dimension(min=5)
         else:
             return Dimension(min=1)
 
     def load_container(self) -> FloatContainer:
         """Return a container with all opened tabs."""
+        self.tabs = [Console(self)]
+
         assert self.pager is not None
         assert self.search_bar is not None
         assert self.tab is not None
 
         self.dialogs["command-palette"] = CommandPalette(self)
         self.dialogs["about"] = AboutDialog(self)
         self.dialogs["save-as"] = SaveAsDialog(self)
@@ -162,15 +164,15 @@
         """Convert the current console session to a notebook."""
         from euporie.notebook.app import NotebookApp
         from euporie.notebook.tabs.notebook import Notebook
 
         app = get_app()
         nb_app = NotebookApp()
         for tab in app.tabs:
-            if isinstance(tab, ConsoleTab):
+            if isinstance(tab, Console):
                 nb = Notebook(
                     app=nb_app,
                     path=tab.path,
                     kernel=tab.kernel,
                     comms=tab.comms,
                     json=tab.json,
                 )
@@ -191,15 +193,15 @@
     @staticmethod
     @add_cmd()
     def _clear_screen() -> None:
         """Clear the screen and the previous output."""
         app = get_app()
         tab = app.tab
         app.renderer.clear()
-        if isinstance(tab, ConsoleTab):
+        if isinstance(tab, Console):
             tab.reset()
             app.layout.focus(tab.input_box)
 
     add_cmd(
         name="end-of-file",
         filter=buffer_is_code & buffer_is_empty,
         description="Signals the end of the input, causing the console to exit.",
```

### Comparing `euporie-2.3.2/euporie/console/tabs/console.py` & `euporie-2.4.0/euporie/console/tabs/console.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     FloatContainer,
     HSplit,
     VSplit,
     Window,
 )
 from prompt_toolkit.layout.controls import FormattedTextControl
 from prompt_toolkit.layout.layout import Layout
+from upath import UPath
 
 from euporie.core.commands import add_cmd, get_cmd
 from euporie.core.config import add_setting
 from euporie.core.filters import (
     at_end_of_buffer,
     buffer_is_code,
     buffer_is_empty,
@@ -48,47 +49,51 @@
 from euporie.core.validation import KernelValidator
 from euporie.core.widgets.cell_outputs import CellOutputArea
 from euporie.core.widgets.inputs import KernelInput, StdInput
 from euporie.core.widgets.page import PrintingContainer
 from euporie.core.widgets.pager import PagerState
 
 if TYPE_CHECKING:
+    from pathlib import Path
     from typing import Any, Callable, Sequence
 
     from prompt_toolkit.application.application import Application
     from prompt_toolkit.formatted_text import AnyFormattedText, StyleAndTextTuples
     from prompt_toolkit.key_binding.key_bindings import NotImplementedOrNone
     from prompt_toolkit.key_binding.key_processor import KeyPressEvent
     from prompt_toolkit.layout.containers import Float
-    from upath import UPath
 
     from euporie.core.app import BaseApp
 
 log = logging.getLogger(__name__)
 
 
-class ConsoleTab(KernelTab):
+class Console(KernelTab):
     """Interactive console.
 
     An interactive console which connects to a Jupyter kernel.
 
     """
 
+    bg_init = False
+
     def __init__(
         self,
         app: BaseApp,
-        path: UPath | None = None,
+        path: Path | None = None,
         use_kernel_history: bool = True,
+        connection_file: str = "",
     ) -> None:
-        """Create a new :py:class:`ConsoleTab` tab instance.
+        """Create a new :py:class:`Console` tab instance.
 
         Args:
             app: The euporie application the console tab belongs to
             path: A file path to open (not used currently)
             use_kernel_history: If :const:`True`, history will be loaded from the kernel
+            connection_file: The connection file of an existing kernel
         """
         # Kernel setup
         self._metadata = {}
         self.kernel_name = app.config.kernel_name
         self.allow_stdin = True
         self.default_callbacks = MsgCallbacks(
             get_input=lambda prompt, password: self.stdin_box.get_input(
@@ -101,15 +106,20 @@
             set_status=lambda status: self.app.invalidate(),
             set_kernel_info=self.set_kernel_info,
             done=self.complete,
             dead=self.kernel_died,
         )
         self.kernel_tab = self
 
-        super().__init__(app=app, path=path, use_kernel_history=use_kernel_history)
+        super().__init__(
+            app=app,
+            path=path,
+            use_kernel_history=use_kernel_history,
+            connection_file=app.config.connection_file,
+        )
 
         self.lang_info: dict[str, Any] = {}
         self.execution_count = 0
         self.clear_outputs_on_output = False
 
         self.json = nbformat.v4.new_notebook()
         self.json["metadata"] = self._metadata
@@ -473,15 +483,15 @@
         """Receive and processes kernel metadata."""
         self.lang_info = info.get("language_info", {})
 
     def refresh(self, now: bool = True) -> None:
         """Request the output is refreshed (does nothing)."""
         pass
 
-    def statusbar_fields(
+    def __pt_status__(
         self,
     ) -> tuple[Sequence[AnyFormattedText], Sequence[AnyFormattedText]]:
         """Generate the formatted text for the statusbar."""
         assert self.kernel is not None
         return (
             [],
             [
@@ -530,15 +540,15 @@
         assert self.kernel is not None
         self.kernel.inspect(
             code=code,
             cursor_pos=cursor_pos,
             callback=_cb,
         )
 
-    def save(self, path: UPath | None = None, cb: Callable | None = None) -> None:
+    def save(self, path: Path | None = None, cb: Callable | None = None) -> None:
         """Save the console as a notebook."""
         from euporie.core.tabs.notebook import BaseNotebook
 
         if path is not None:
             BaseNotebook.save(cast("BaseNotebook", self), path)
 
     # ################################### Commands ####################################
@@ -569,27 +579,27 @@
         filter=buffer_is_code & buffer_has_focus,
     )
     def _run_input() -> None:
         """Run the console input."""
         from euporie.console.app import get_app
 
         console = get_app().tab
-        assert isinstance(console, ConsoleTab)
+        assert isinstance(console, Console)
         console.run()
 
     @staticmethod
     @add_cmd(
         filter=buffer_is_code & buffer_has_focus & ~has_selection,
     )
     def _show_contextual_help() -> None:
         """Display contextual help."""
         from euporie.console.app import get_app
 
         console = get_app().tab
-        assert isinstance(console, ConsoleTab)
+        assert isinstance(console, Console)
         console.inspect()
 
     @staticmethod
     @add_cmd(
         name="cc-interrupt-kernel",
         hidden=True,
         filter=buffer_is_code & buffer_is_empty,
@@ -640,14 +650,29 @@
         },
         description="""
             Defines the maximum number of executed "cells" to store in case the console
             session is saved to a file or converted into a notebook.
         """,
     )
 
+    add_setting(
+        name="connection_file",
+        flags=["--connection-file", "--kernel-connection-file"],
+        type_=UPath,
+        help_="Attempt to connect to an existing kernel using a JSON connection info file",
+        default=None,
+        description="""
+            If the file does not exist, kernel connection information will be written
+            to the file path provided.
+
+            If the file exists, kernel connection info will be read from the file,
+            allowing euporie to connect to existing kernels.
+        """,
+    )
+
     # ################################# Key Bindings ##################################
 
     register_bindings(
         {
             "euporie.console.tabs.console.Console": {
                 "cc-interrupt-kernel": "c-c",
                 "show-contextual-help": "s-tab",
```

### Comparing `euporie-2.3.2/euporie/core/app.py` & `euporie-2.4.0/euporie/core/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """Contain the main Application class which runs euporie.core."""
 
 from __future__ import annotations
 
 import asyncio
 import json
 import logging
+import signal
+import sys
 from functools import partial
+from pathlib import PurePath
 from typing import TYPE_CHECKING, cast
 from weakref import WeakSet
 
 from prompt_toolkit.application.application import Application, _CombinedRegistry
 from prompt_toolkit.application.current import create_app_session
 from prompt_toolkit.clipboard import InMemoryClipboard
 from prompt_toolkit.clipboard.pyperclip import PyperclipClipboard
 from prompt_toolkit.cursor_shapes import CursorShape, CursorShapeConfig
 from prompt_toolkit.data_structures import Point
 from prompt_toolkit.enums import EditingMode
 from prompt_toolkit.filters import Condition, buffer_has_focus, to_filter
-from prompt_toolkit.formatted_text import to_formatted_text
 from prompt_toolkit.input.defaults import create_input
 from prompt_toolkit.key_binding.bindings.basic import load_basic_bindings
 from prompt_toolkit.key_binding.bindings.cpr import load_cpr_bindings
 from prompt_toolkit.key_binding.bindings.emacs import (
     load_emacs_bindings,
     load_emacs_search_bindings,
     load_emacs_shift_selection_bindings,
@@ -35,15 +37,14 @@
 )
 from prompt_toolkit.key_binding.key_bindings import (
     ConditionalKeyBindings,
     merge_key_bindings,
 )
 from prompt_toolkit.layout.containers import Float, FloatContainer, Window, to_container
 from prompt_toolkit.layout.layout import Layout
-from prompt_toolkit.layout.menus import CompletionsMenu
 from prompt_toolkit.output import ColorDepth
 from prompt_toolkit.output.defaults import create_output
 from prompt_toolkit.output.vt100 import Vt100_Output as PtkVt100_Output
 from prompt_toolkit.styles import (
     BaseStyle,
     ConditionalStyleTransformation,
     DummyStyle,
@@ -57,66 +58,63 @@
 from pygments.styles import STYLE_MAP as pygments_styles
 from pygments.styles import get_style_by_name
 from pyperclip import determine_clipboard
 from upath import UPath
 
 from euporie.core.commands import add_cmd
 from euporie.core.config import Config, add_setting
+from euporie.core.convert.core import get_mime
 from euporie.core.current import get_app
 from euporie.core.filters import in_tmux, insert_mode, replace_mode, tab_has_focus
 from euporie.core.io import Vt100_Output, Vt100Parser
 from euporie.core.key_binding.key_processor import KeyProcessor
 from euporie.core.key_binding.micro_state import MicroState
 from euporie.core.key_binding.registry import (
     load_registered_bindings,
     register_bindings,
 )
 from euporie.core.key_binding.vi_state import ViState
-from euporie.core.log import default_logs, setup_logs
+from euporie.core.log import setup_logs
+from euporie.core.path import parse_path
 from euporie.core.renderer import Renderer
 from euporie.core.style import (
     DEFAULT_COLORS,
     HTML_STYLE,
     IPYWIDGET_STYLE,
     LOG_STYLE,
     MIME_STYLE,
     ColorPalette,
     build_style,
 )
 from euporie.core.terminal import TerminalInfo
-from euporie.core.utils import ChainedList, parse_path
+from euporie.core.utils import ChainedList
 from euporie.core.widgets.decor import Shadow
+from euporie.core.widgets.menu import CompletionsMenu
 
 if TYPE_CHECKING:
     from asyncio import AbstractEventLoop
-    from typing import Any, Callable, Literal, Sequence
+    from pathlib import Path
+    from types import FrameType
+    from typing import Any, Callable
 
     from prompt_toolkit.clipboard import Clipboard
     from prompt_toolkit.contrib.ssh import PromptToolkitSSHSession
     from prompt_toolkit.filters import Filter, FilterOrBool
-    from prompt_toolkit.formatted_text import AnyFormattedText, StyleAndTextTuples
     from prompt_toolkit.input import Input
-    from prompt_toolkit.layout.containers import AnyContainer
     from prompt_toolkit.layout.layout import FocusableElement
     from prompt_toolkit.layout.screen import WritePosition
     from prompt_toolkit.output import Output
 
     from euporie.core.config import Setting
     from euporie.core.tabs.base import Tab
     from euporie.core.terminal import TerminalQuery
     from euporie.core.widgets.dialog import Dialog
     from euporie.core.widgets.pager import Pager
     from euporie.core.widgets.search_bar import SearchBar
 
-    StatusBarFields = tuple[Sequence[AnyFormattedText], Sequence[AnyFormattedText]]
-    ContainerStatusDict = dict[
-        AnyContainer,
-        Callable[[], StatusBarFields],
-    ]
-
 log = logging.getLogger(__name__)
 
 
 _COLOR_DEPTHS = {
     1: ColorDepth.DEPTH_1_BIT,
     4: ColorDepth.DEPTH_4_BIT,
     8: ColorDepth.DEPTH_8_BIT,
@@ -178,15 +176,14 @@
     """
 
     name: str
     color_palette: ColorPalette
     mouse_position: Point
 
     config = Config()
-    status_default: StatusBarFields = ([], [])
     need_mouse_support: bool = False
     log_stdout_level: str = "CRITICAL"
 
     def __init__(
         self,
         title: str | None = None,
         set_title: bool = True,
@@ -251,16 +248,14 @@
         self.dialogs: dict[str, Dialog] = {}
         self.menus: dict[str, Float] = {}
         self.floats = ChainedList(
             self.graphics,
             self.dialogs.values(),
             self.menus.values(),
         )
-        # Mapping of Containers to status field generating functions
-        self.container_statuses: ContainerStatusDict = {}
         # Continue loading when the application has been launched
         # and an event loop has been creeated
         self.pre_run_callables = [self.pre_run]
         self.post_load_callables: list[Callable[[], None]] = []
         # Set default vi input mode to navigate
         self.vi_state = ViState()
         # Set a long timeout for mappings (e.g. dd)
@@ -341,24 +336,20 @@
         # Determine what color depth to use
         self._color_depth = _COLOR_DEPTHS.get(
             self.config.color_depth, self.term_info.depth_of_color.value
         )
         # Set the application's style, and update it when the terminal responds
         self.update_style()
         self.term_info.colors.event += self.update_style
+        # Pause rendering while we load the layout
         self.pause_rendering()
         # Load completions menu. This must be done after the app is initialized, because
         # :py:func:`get_app` is needed to access the config
         self.menus["completions"] = Float(
-            content=Shadow(
-                CompletionsMenu(
-                    max_height=16,
-                    scroll_offset=1,
-                )
-            ),
+            content=Shadow(CompletionsMenu()),
             xcursor=True,
             ycursor=True,
         )
 
         def terminal_ready() -> None:
             """Command here depend on the result of terminal queries."""
             # Open any files we need to
@@ -385,18 +376,15 @@
         else:
             # Otherwise, we query the terminal and wait asynchronously to give it
             # a chance to respond
 
             async def await_terminal_feedback() -> None:
                 try:
                     # Send queries to the terminal if supported
-                    if self.input.__class__.__name__ in (
-                        "Vt100Input",
-                        "PosixPipeInput",
-                    ):
+                    if self.input.__class__.__name__ == "Vt100Input":
                         self.term_info.send_all()
                         # Give the terminal a chance to respond
                         await asyncio.sleep(0.1)
                     # Complete loading the application
                     terminal_ready()
                 except Exception as exception:
                     # Log exceptions, as this runs in the event loop and, exceptions may
@@ -417,14 +405,15 @@
         Ensures the TUI app always tries to run in a TTY.
 
         Returns:
             A prompt-toolkit input instance
 
         """
         input_ = create_input(always_prefer_tty=True)
+
         if stdin := getattr(input_, "stdin", None):
             if not stdin.isatty():
                 from euporie.core.io import IgnoredInput
 
                 input_ = IgnoredInput()
 
         # Use a custom vt100 parser to allow querying the terminal
@@ -511,25 +500,58 @@
         self.term_info.pixel_dimensions.send()
         super()._on_resize()
 
     @classmethod
     def launch(cls) -> None:
         """Launch the app."""
         # Load default logging
-        default_logs()
+        setup_logs()
         # Load the app's configuration
         cls.config.load(cls)
         # Configure the logs
         setup_logs(cls.config)
         # Warn about unrecognised configuration items
         cls.config.warn()
         # Run the application
         with create_app_session(input=cls.load_input(), output=cls.load_output()):
             # Create an instance of the app and run it
-            return cls().run()
+
+            original_sigterm = signal.getsignal(signal.SIGTERM)
+            original_sigint = signal.getsignal(signal.SIGINT)
+
+            app = cls()
+
+            signal.signal(signal.SIGTERM, app.cleanup)
+            signal.signal(signal.SIGINT, app.cleanup)
+
+            result = app.run()
+
+            signal.signal(signal.SIGTERM, original_sigterm)
+            signal.signal(signal.SIGINT, original_sigint)
+
+            return result
+
+    def cleanup(self, signum: int, frame: FrameType | None) -> None:
+        """Restore the state of the terminal on unexpected exit."""
+        log.critical("Unexpected exit signal, restoring terminal")
+        output = self.output
+        self.exit()
+        # Reset terminal state
+        output.quit_alternate_screen()
+        output.disable_mouse_support()
+        output.reset_cursor_key_mode()
+        output.enable_autowrap()
+        output.disable_bracketed_paste()
+        output.clear_title()
+        output.reset_cursor_shape()
+        output.show_cursor()
+        output.reset_attributes()
+        output.flush()
+        # Exit the main thread
+        sys.exit(1)
 
     @classmethod
     async def interact(cls, ssh_session: PromptToolkitSSHSession) -> None:
         """Run the app asynchronously for the hub SSH server."""
         await cls().run_async()
 
     def load_container(self) -> FloatContainer:
@@ -540,35 +562,60 @@
 
         """
         return FloatContainer(
             content=Window(),
             floats=cast("list[Float]", self.floats),
         )
 
-    def get_file_tab(self, path: UPath) -> type[Tab] | None:
+    def get_file_tabs(self, path: Path) -> list[type[Tab]]:
+        """Return the tab to use for a file path."""
+        from euporie.core.tabs.base import Tab
+
+        path_mime = get_mime(path) or "text/plain"
+        log.debug("File %s has mime type: %s", path, path_mime)
+
+        tab_options = set()
+        for tab_cls in Tab._registry:
+            for mime_type in tab_cls.mime_types:
+                if PurePath(path_mime).match(mime_type):
+                    tab_options.add(tab_cls)
+            if path.suffix in tab_cls.file_extensions:
+                tab_options.add(tab_cls)
+
+        return sorted(tab_options, key=lambda x: x.weight, reverse=True)
+
+    def get_file_tab(self, path: Path) -> type[Tab] | None:
         """Return the tab to use for a file path."""
+        if tabs := self.get_file_tabs(path):
+            return tabs[0]
         return None
 
-    def open_file(self, path: UPath, read_only: bool = False) -> None:
+    def open_file(
+        self, path: Path, read_only: bool = False, tab_class: type[Tab] | None = None
+    ) -> None:
         """Create a tab for a file.
 
         Args:
             path: The file path of the notebook file to open
             read_only: If true, the file should be opened read_only
+            tab_class: The tab type to use to open the file
 
         """
         ppath = parse_path(path)
         log.info(f"Opening file {path}")
         for tab in self.tabs:
-            if ppath == getattr(tab, "path", ""):
+            if ppath == getattr(tab, "path", "") and (
+                tab_class is None or isinstance(tab, tab_class)
+            ):
                 log.info(f"File {path} already open, activating")
                 self.layout.focus(tab)
                 break
         else:
-            tab_class = self.get_file_tab(path)
+            if tab_class is None:
+                tab_class = self.get_file_tab(path)
             if tab_class is None:
                 log.error("Unable to display file %s", path)
             else:
                 tab = tab_class(self, ppath)
                 self.tabs.append(tab)
                 # Ensure the opened tab is focused at app start
                 self.focused_element = tab
@@ -753,52 +800,14 @@
 
     def _create_merged_style(
         self, include_default_pygments_style: Filter | None = None
     ) -> BaseStyle:
         """Block default style loading."""
         return DummyStyle()
 
-    def format_status(self, part: Literal["left", "right"]) -> StyleAndTextTuples:
-        """Format the fields in the statusbar generated by the current tab.
-
-        Args:
-            part: ``'left'`` to return the fields on the left side of the statusbar,
-                and ``'right'`` to return the fields on the right
-
-        Returns:
-            A list of style and text tuples for display in the statusbar
-
-        """
-        entries: StatusBarFields = ([], [])
-        for container, status_func in self.container_statuses.items():
-            if self.layout.has_focus(container):
-                entries = status_func()
-                break
-        else:
-            if not self.tabs:
-                entries = self.status_default
-
-        output: StyleAndTextTuples = []
-        # Show the tab's status fields
-        for field in entries[0 if part == "left" else 1]:
-            if field:
-                if isinstance(field, tuple):
-                    ft = [field]
-                else:
-                    ft = to_formatted_text(field, style="class:status.field")
-                output += [
-                    ("class:status.field", " "),
-                    *ft,
-                    ("class:status.field", " "),
-                    ("class:status", " "),
-                ]
-        if output:
-            output.pop()
-        return output
-
     def draw(self, render_as_done: bool = True) -> None:
         """Draw the app without focus, leaving the cursor below the drawn output."""
         # Hide ephemeral containers
         self._redrawing = True
         # Ensure nothing in the layout has focus
         self.layout._stack.append(Window())
         # Re-draw the app
@@ -905,53 +914,14 @@
         },
         description="""
             A list of file paths to open when euporie is launched.
         """,
     )
 
     add_setting(
-        name="log_file",
-        flags=["--log-file"],
-        nargs="?",
-        default="",
-        type_=str,
-        title="the log file path",
-        help_="File path for logs",
-        description="""
-            When set to a file path, the log output will be written to the given path.
-            If no value is given output will be sent to the standard output.
-        """,
-    )
-
-    add_setting(
-        name="log_level",
-        flags=["--log-level"],
-        type_=str,
-        default="",
-        title="the log level",
-        help_="Set the log level",
-        choices=["debug", "info", "warning", "error", "critical"],
-        description="""
-            When set, logging events at the given level are emitted.
-        """,
-    )
-
-    add_setting(
-        name="log_config",
-        flags=["--log-config"],
-        type_=str,
-        default=None,
-        title="additional logging configuration",
-        help_="Additional logging configuration",
-        description="""
-            A JSON string specifying additional logging configuration.
-        """,
-    )
-
-    add_setting(
         name="edit_mode",
         flags=["--edit-mode"],
         type_=str,
         choices=["micro", "emacs", "vi"],
         title="Editor key bindings",
         help_="Key-binding mode for text editing",
         default="micro",
```

### Comparing `euporie-2.3.2/euporie/core/border.py` & `euporie-2.4.0/euporie/core/border.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,30 +271,29 @@
 AsciiThickLine = LineStyle("AsciiDouble", rank=(3, 0), parent=AsciiLine)
 ThickLine = LineStyle("Thick", rank=(3, 4), parent=ThinLine)
 DoubleLine = LineStyle("Double", (3, 5), parent=ThickLine)
 ThickQuadrupleDashedLine = LineStyle("QuadDashed", (3, 1), parent=ThickLine)
 ThickTripleDashedLine = LineStyle("TripleDashed", (3, 2), parent=ThickLine)
 ThickDoubleDashedLine = LineStyle("DoubleDashed", (3, 3), parent=ThickLine)
 
-#  ▂▂▂▂▂▂▂▂▂▂▂▂
-# 🮇Quarter Line▎
-#  🮂🮂🮂🮂🮂🮂🮂🮂🮂🮂🮂🮂
+UpperRightQuarterLine = LineStyle("UpperRightQuarterLine", (4, 2), parent=ThickLine)
+LowerLeftQuarterLine = LineStyle("LowerLeftQuarterLine", (4, 2), parent=ThickLine)
 
-UpperRightHalfLine = LineStyle("UpperRightHalfLine", (4, 2), parent=ThickLine)
-LowerLeftHalfLine = LineStyle("LowerLeftHalfLine", (4, 2), parent=ThickLine)
+UpperRightHalfLine = LineStyle("UpperRightHalfLine", (5, 2), parent=ThickLine)
+LowerLeftHalfLine = LineStyle("LowerLeftHalfLine", (5, 2), parent=ThickLine)
 UpperRightHalfDottedLine = LineStyle(
-    "UpperRightHalfDottedLine", (4, 1), parent=UpperRightHalfLine
+    "UpperRightHalfDottedLine", (5, 1), parent=UpperRightHalfLine
 )
 LowerLeftHalfDottedLine = LineStyle(
-    "LowerLeftHalfDottedLine", (4, 2), parent=LowerLeftHalfLine
+    "LowerLeftHalfDottedLine", (5, 2), parent=LowerLeftHalfLine
 )
 
 
-FullLine = LineStyle("FullLine", (5, 2), parent=ThickLine)
-FullDottedLine = LineStyle("FullDottedLine", (5, 1), parent=ThickLine)
+FullLine = LineStyle("FullLine", (6, 2), parent=ThickLine)
+FullDottedLine = LineStyle("FullDottedLine", (6, 1), parent=ThickLine)
 
 
 class GridChar(NamedTuple):
     """Repreentation of a grid node character.
 
     The four compass points represent the line style joining from the given direction.
     """
@@ -498,14 +497,45 @@
     GridChar(ThinLine,              LowerLeftEighthLine,    NoLine,                 LowerLeftEighthLine ): "▁",
     GridChar(UpperRightEighthLine,  ThinLine,               UpperRightEighthLine,   NoLine              ): "▕",
     GridChar(NoLine,                UpperRightEighthLine,   ThinLine,               UpperRightEighthLine): "▔",
     GridChar(UpperRightEighthLine,  NoLine,                 UpperRightEighthLine,   ThinLine            ): "▕",
     GridChar(ThinLine,              UpperRightEighthLine,   NoLine,                 UpperRightEighthLine): "▔",
     GridChar(NoLine,                NoLine,                 UpperRightEighthLine,   LowerLeftEighthLine ): "▁",
     GridChar(LowerLeftEighthLine,   UpperRightEighthLine,   NoLine,                 NoLine              ): "▔",
+
+    # UpperRightQuarterLine
+    GridChar(UpperRightQuarterLine, NoLine, UpperRightQuarterLine, NoLine): "🮇",
+    GridChar(NoLine, UpperRightQuarterLine, NoLine, UpperRightQuarterLine): "🮂",
+    GridChar(NoLine, UpperRightQuarterLine, UpperRightQuarterLine, NoLine): "🮇",
+    GridChar(UpperRightQuarterLine, NoLine, NoLine, UpperRightQuarterLine): "🮂",
+    GridChar(UpperRightQuarterLine, UpperRightQuarterLine, UpperRightQuarterLine, NoLine): "🮇",
+    GridChar(UpperRightQuarterLine, UpperRightQuarterLine, NoLine, UpperRightQuarterLine): "🮂",
+    # Corners
+    GridChar(NoLine, LowerLeftEighthLine, UpperRightQuarterLine, NoLine): " ",
+    GridChar(NoLine, NoLine, LowerLeftQuarterLine, LowerLeftEighthLine): " ",
+    GridChar(LowerLeftQuarterLine, NoLine, NoLine, UpperRightEighthLine): " ",
+    GridChar(UpperRightQuarterLine, UpperRightEighthLine, NoLine, NoLine): " ",
+
+    # LowerLeftQuarterLine
+    GridChar(LowerLeftQuarterLine, NoLine, LowerLeftQuarterLine, NoLine): "▎",
+    GridChar(NoLine, LowerLeftQuarterLine, NoLine, LowerLeftQuarterLine): "▂",
+    GridChar(NoLine, LowerLeftQuarterLine, LowerLeftQuarterLine, NoLine): "▂",
+    GridChar(LowerLeftQuarterLine, NoLine, NoLine, LowerLeftQuarterLine): "▎",
+    GridChar(NoLine, LowerLeftQuarterLine, LowerLeftQuarterLine, LowerLeftQuarterLine): "▂",
+    GridChar(LowerLeftQuarterLine, NoLine, LowerLeftQuarterLine, LowerLeftQuarterLine): "▎",
+    # Half/ThinLine combos
+    GridChar(LowerLeftQuarterLine, ThinLine, LowerLeftQuarterLine, NoLine): "▎",
+    GridChar(NoLine, LowerLeftQuarterLine, ThinLine, LowerLeftQuarterLine): "▂",
+    GridChar(LowerLeftQuarterLine, NoLine, LowerLeftQuarterLine, ThinLine): "▎",
+    GridChar(ThinLine, LowerLeftQuarterLine, NoLine, LowerLeftQuarterLine): "▂",
+    GridChar(UpperRightQuarterLine, ThinLine, UpperRightQuarterLine, NoLine): "🮇",
+    GridChar(NoLine, UpperRightQuarterLine, ThinLine, UpperRightQuarterLine): "🮂",
+    GridChar(UpperRightQuarterLine, NoLine, UpperRightQuarterLine, ThinLine): "🮇",
+    GridChar(ThinLine, UpperRightQuarterLine, NoLine, UpperRightQuarterLine): "🮂",
+
     # UpperRightHalfLine
     GridChar(UpperRightHalfLine, NoLine, UpperRightHalfLine, NoLine): "▐",
     GridChar(NoLine, UpperRightHalfLine, NoLine, UpperRightHalfLine): "▀",
     GridChar(UpperRightHalfLine, UpperRightHalfLine, NoLine, NoLine): "▝",
     GridChar(NoLine, UpperRightHalfLine, UpperRightHalfLine, NoLine): "▐",
     GridChar(NoLine, NoLine, UpperRightHalfLine, UpperRightHalfLine): "▜",
     GridChar(UpperRightHalfLine, NoLine, NoLine, UpperRightHalfLine): "▀",
@@ -813,23 +843,23 @@
                 for char_key in list(self.grid.values())[i * 4 : (i + 1) * 4]
             )
             for i in range(4)
         )
 
 ThinGrid = ThinLine.grid
 
-InnerEigthGrid = (
-    LowerLeftEighthLine.top_edge
-    + LowerLeftEighthLine.right_edge
-    + UpperRightEighthLine.left_edge
+InsetGrid = (
+    UpperRightQuarterLine.left_edge
+    + LowerLeftQuarterLine.right_edge
     + UpperRightEighthLine.bottom_edge
+    + LowerLeftEighthLine.top_edge
     + ThinLine.inner
 )
 
-OuterEigthGrid = (
+OutsetGrid = (
     LowerLeftEighthLine.top_edge
     + UpperRightEighthLine.right_edge
     + UpperRightEighthLine.bottom_edge
     + LowerLeftEighthLine.left_edge
     + ThinLine.inner
 )
```

### Comparing `euporie-2.3.2/euporie/core/commands.py` & `euporie-2.4.0/euporie/core/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,36 +12,44 @@
 from prompt_toolkit.key_binding.key_bindings import Binding
 from prompt_toolkit.key_binding.key_processor import KeyPressEvent
 
 from euporie.core.key_binding.utils import parse_keys
 from euporie.core.keys import Keys
 
 if TYPE_CHECKING:
-    from typing import Any, Callable, Coroutine, Sequence
+    from typing import Any, Callable, Coroutine
 
     from prompt_toolkit.filters import Filter, FilterOrBool
     from prompt_toolkit.key_binding.key_bindings import (
         KeyBindingsBase,
         KeyHandlerCallable,
+        NotImplementedOrNone,
     )
 
     from euporie.core.widgets.menu import MenuItem
 
     AnyKey = tuple[Keys | str, ...] | Keys | str
     AnyKeys = list[AnyKey] | AnyKey
+    CommandHandlerNoArgs = Callable[
+        ..., Coroutine[Any, Any, None] | NotImplementedOrNone
+    ]
+    CommandHandlerArgs = Callable[
+        [KeyPressEvent], Coroutine[Any, Any, None] | NotImplementedOrNone
+    ]
+    CommandHandler = CommandHandlerNoArgs | CommandHandlerArgs
 
 log = logging.getLogger(__name__)
 
 
 class Command:
     """Wrap a function so it can be used as a key-binding or a menu item."""
 
     def __init__(
         self,
-        handler: Callable[..., Coroutine[Any, Any, None] | None],
+        handler: CommandHandler,
         *,
         filter: FilterOrBool = True,
         hidden: FilterOrBool = False,
         name: str | None = None,
         title: str | None = None,
         menu_title: str | None = None,
         description: str | None = None,
@@ -94,17 +102,14 @@
         self.eager = to_filter(eager)
         self.is_global = to_filter(is_global)
         self.save_before = save_before
         self.record_in_macro = to_filter(record_in_macro)
 
         self.keys: list[tuple[str | Keys, ...]] = []
 
-        self.selected_item = 0
-        self.children: Sequence[MenuItem] = []
-
     def run(self) -> None:
         """Run the command's handler."""
         if self.filter():
             self.key_handler(
                 KeyPressEvent(
                     key_processor_ref=weakref.ref(get_app().key_processor),
                     arg=None,
@@ -113,36 +118,36 @@
                     is_repeat=False,
                 )
             )
 
     @property
     def key_handler(self) -> KeyHandlerCallable:
         """Return a key handler for the command."""
-        sig = signature(self.handler)
+        handler = self.handler
+        sig = signature(handler)
 
         if sig.parameters:
             # The handler already accepts a `KeyPressEvent` argument
-            return cast("KeyHandlerCallable", self.handler)
+            return cast("KeyHandlerCallable", handler)
+
+        if isawaitable(handler):
+
+            async def _key_handler_async(event: KeyPressEvent) -> NotImplementedOrNone:
+                result = cast("CommandHandlerNoArgs", handler)()
+                assert isawaitable(result)
+                return await result
+
+            return _key_handler_async
+
+        else:
 
-        def _key_handler(event: KeyPressEvent) -> None:
-            result = self.handler()
-            # If the handler is a coroutine, create an asyncio task.
-            if isawaitable(result):
-                awaitable = result
-
-                async def bg_task() -> None:
-                    result = await awaitable
-                    if result != NotImplemented:
-                        event.app.invalidate()
-
-                event.app.create_background_task(bg_task())
-            elif result != NotImplemented:
-                event.app.invalidate()
+            def _key_handler(event: KeyPressEvent) -> NotImplementedOrNone:
+                return cast("CommandHandlerNoArgs", handler)()
 
-        return _key_handler
+            return _key_handler
 
     def bind(self, key_bindings: KeyBindingsBase, keys: AnyKeys) -> None:
         """Add the current commands to a set of key bindings.
 
         Args:
             key_bindings: The set of key bindings to bind to
             keys: Additional keys to bind to the command
@@ -169,24 +174,26 @@
         if self.keys:
             return format_keys([self.keys[0]])[0]
         return ""
 
     @property
     def menu_handler(self) -> Callable[[], None]:
         """Return a menu handler for the command."""
-        if isawaitable(self.handler):
+        handler = self.handler
+        if isawaitable(handler):
 
             def _menu_handler() -> None:
-                task = self.handler()
+                task = cast("CommandHandlerNoArgs", handler)()
+                task = cast("Coroutine[Any, Any, None]", task)
                 if task is not None:
                     get_app().create_background_task(task)
 
             return _menu_handler
         else:
-            return cast("Callable[[], None]", self.handler)
+            return cast("Callable[[], None]", handler)
 
     @property
     def menu(self) -> MenuItem:
         """Return a menu item for the command."""
         from euporie.core.widgets.menu import MenuItem
 
         if self._menu is None:
```

### Comparing `euporie-2.3.2/euporie/core/completion.py` & `euporie-2.4.0/euporie/core/completion.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,12 +37,9 @@
     ) -> AsyncGenerator[Completion, None]:
         """Retrieve completions from a :class:`Kernel`."""
         for kwargs in await self.kernel.complete_(
             code=document.text,
             cursor_pos=document.cursor_position,
         ):
             if completion_type := kwargs.get("display_meta"):
-                kwargs["style"] = f"class:completion-menu.completion.{completion_type}"
-                kwargs[
-                    "selected_style"
-                ] = f"class:completion-menu.completion.current.{completion_type}"
+                kwargs["style"] = f"class:completion-{completion_type}"
             yield Completion(**kwargs)
```

### Comparing `euporie-2.3.2/euporie/core/config.py` & `euporie-2.4.0/euporie/core/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 from __future__ import annotations
 
 import argparse
 import json
 import logging
 import os
+import sys
 from ast import literal_eval
 from collections import ChainMap
 from functools import partial
 from pathlib import Path
 from typing import TYPE_CHECKING, Protocol, TextIO, cast
 
 import fastjsonschema
-from appdirs import user_config_dir
+from platformdirs import user_config_dir
 from prompt_toolkit.filters.base import Condition
 from prompt_toolkit.filters.utils import to_filter
 from prompt_toolkit.utils import Event
 from upath import UPath
 
 from euporie.core import __app_name__, __copyright__, __version__
 from euporie.core.commands import add_cmd, get_cmd
-from euporie.core.log import setup_logs
 
 if TYPE_CHECKING:
     from typing import IO, Any, Callable, Optional, Sequence
 
     from prompt_toolkit.filters.base import Filter, FilterOrBool
 
     from euporie.core.widgets.menu import MenuItem
@@ -335,14 +335,16 @@
         if self.valid_user:
             log.debug("Saving setting `%s`", setting)
             with open(self.config_file_path, "w") as f:
                 json.dump(json_data, f, indent=2)
 
     def load(self, cls: type[ConfigurableApp]) -> None:
         """Load the command line, environment, and user configuration."""
+        from euporie.core.log import setup_logs
+
         self.app_cls = cls
         self.app_name = cls.name
         log.debug("Loading config for %s", self.app_name)
 
         user_conf_dir = Path(user_config_dir(__app_name__, appauthor=None))
         user_conf_dir.mkdir(exist_ok=True, parents=True)
         self.config_file_path = (user_conf_dir / self.conf_file_name).with_suffix(
@@ -412,15 +414,19 @@
             args, kwargs = setting.parser_args
             parser.add_argument(*args, **kwargs)
         return parser
 
     def load_args(self) -> dict[str, Any]:
         """Attempt to load configuration settings from commandline flags."""
         result = {}
-        namespace, _ = self.load_parser().parse_known_intermixed_args()
+        # Parse known arguments
+        namespace, remainder = self.load_parser().parse_known_intermixed_args()
+        # Update argv to leave the remaining arguments for subsequent apps
+        sys.argv[1:] = remainder
+        # Validate arguments
         for name, value in vars(namespace).items():
             if value is not None:
                 # Convert to json and back to attain json types
                 json_data = json.loads(_json_encoder.encode({name: value}))
                 try:
                     fastjsonschema.validate(self.schema, json_data)
                 except fastjsonschema.JsonSchemaValueException as error:
@@ -504,25 +510,29 @@
         except fastjsonschema.JsonSchemaValueException as error:
             log.warning(f"Error in config file: `{self.config_file_path}`: {error}")
             self.valid_user = False
         else:
             results.update(json_data)
         return results
 
-    def get(self, name: str) -> Any:
+    def get(self, name: str, default: Any = None) -> Any:
         """Access a configuration value, falling back to the default value if unset.
 
         Args:
             name: The name of the attribute to access.
+            default: The value to return if the name is not found
 
         Returns:
             The configuration variable value.
 
         """
-        return self.settings[name].value
+        if name in self.settings:
+            return self.settings[name].value
+        else:
+            return default
 
     def get_item(self, name: str) -> Any:
         """Access a configuration item.
 
         Args:
             name: The name of the attribute to access.
```

### Comparing `euporie-2.3.2/euporie/core/data_structures.py` & `euporie-2.4.0/euporie/core/data_structures.py`

 * *Files identical despite different names*

### Comparing `euporie-2.3.2/euporie/core/filters.py` & `euporie-2.4.0/euporie/core/filters.py`

 * *Files identical despite different names*

### Comparing `euporie-2.3.2/euporie/core/format.py` & `euporie-2.4.0/euporie/core/format.py`

 * *Files identical despite different names*

### Comparing `euporie-2.3.2/euporie/core/history.py` & `euporie-2.4.0/euporie/core/history.py`

 * *Files identical despite different names*

### Comparing `euporie-2.3.2/euporie/core/io.py` & `euporie-2.4.0/euporie/core/io.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Define custom inputs and outputs, and related methods."""
 
+from __future__ import annotations
+
 import logging
 import re
 from typing import TYPE_CHECKING
 
 from prompt_toolkit.input import vt100_parser
 from prompt_toolkit.input.base import DummyInput, _dummy_context_manager
 from prompt_toolkit.output.vt100 import Vt100_Output as PtkVt100_Output
 
 if TYPE_CHECKING:
-    from typing import Any, Callable, ContextManager, Union
+    from typing import Any, Callable, ContextManager
 
     from prompt_toolkit.keys import Keys
 
 log = logging.getLogger(__name__)
 
 _response_prefix_re = re.compile(
     r"""^\x1b(
@@ -26,15 +28,15 @@
         P[ -~]*(\x1b|x1b\\)?
     )\Z""",
     re.VERBOSE,
 )
 
 
 class _IsPrefixOfLongerMatchCache(vt100_parser._IsPrefixOfLongerMatchCache):
-    def __missing__(self, prefix: "str") -> "bool":
+    def __missing__(self, prefix: str) -> bool:
         """Check if the response might match an OSC or APC code, or DA response."""
         result = super().__missing__(prefix)
         if not result:
             if _response_prefix_re.match(prefix):
                 result = True
                 self[prefix] = result
         return result
@@ -43,57 +45,55 @@
 # Monkey patch the prefix cache
 vt100_parser._IS_PREFIX_OF_LONGER_MATCH_CACHE = _IsPrefixOfLongerMatchCache()
 
 
 class Vt100Parser(vt100_parser.Vt100Parser):
     """A Vt100Parser which checks input against additional key patterns."""
 
-    def __init__(self, *args: "Any", **kwargs: "Any") -> "None":
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         """Create a new VT100 parser."""
         super().__init__(*args, **kwargs)
-        self.queries: "dict[Keys, re.Pattern]" = {}
+        self.queries: dict[Keys, re.Pattern] = {}
 
-    def _get_match(self, prefix: "str") -> "Union[None, Keys, tuple[Keys, ...]]":
+    def _get_match(self, prefix: str) -> None | Keys | tuple[Keys, ...]:
         """Check for additional key matches first."""
         for key, pattern in self.queries.items():
             if pattern.match(prefix):
                 return key
 
         return super()._get_match(prefix)
 
 
 class IgnoredInput(DummyInput):
     """An input which ignores input but does not immediately close the app."""
 
-    def attach(
-        self, input_ready_callback: "Callable[[], None]"
-    ) -> "ContextManager[None]":
+    def attach(self, input_ready_callback: Callable[[], None]) -> ContextManager[None]:
         """Do not call the callback, so the input is never closed."""
         return _dummy_context_manager()
 
 
 class Vt100_Output(PtkVt100_Output):
     """A Vt100 output which enables SGR pixel mouse positioning."""
 
-    def enable_mouse_support(self) -> "None":
+    def enable_mouse_support(self) -> None:
         """Additionally enable SGR-pixel mouse positioning."""
         super().enable_mouse_support()
         self.write_raw("\x1b[?1016h")
 
-    def disable_mouse_support(self) -> "None":
+    def disable_mouse_support(self) -> None:
         """Additionally disable SGR-pixel mouse positioning."""
         super().disable_mouse_support()
         self.write_raw("\x1b[?1016l")
 
-    def enable_extended_keys(self) -> "None":
+    def enable_extended_keys(self) -> None:
         """Request extended keys."""
         # xterm
         self.write_raw("\x1b[>4;1m")
         # kitty
-        self.write_raw("\x1b[>1u")
+        self.write_raw("\x1b[=1u")
 
-    def disable_extended_keys(self) -> "None":
+    def disable_extended_keys(self) -> None:
         """Disable extended keys."""
         # xterm
         self.write_raw("\x1b[>4;0m")
         # kitty
-        self.write_raw("\x1b[<u")
+        self.write_raw("\x1b[=0u")
```

### Comparing `euporie-2.3.2/euporie/core/kernel.py` & `euporie-2.4.0/euporie/core/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 import asyncio
 import concurrent.futures
 import logging
 import threading
 from collections import defaultdict
 from subprocess import DEVNULL  # noqa S404 - Security implications considered
 from typing import TYPE_CHECKING, TypedDict
+from uuid import uuid4
 
 import nbformat
 from _frozen_importlib import _DeadlockError
 from jupyter_client import AsyncKernelManager, KernelManager
 from jupyter_client.kernelspec import NATIVE_KERNEL_NAME, NoSuchKernel
-from jupyter_core.paths import jupyter_path
-
-from euporie.core.config import add_setting
+from jupyter_core.paths import jupyter_path, jupyter_runtime_dir
+from upath import UPath
 
 if TYPE_CHECKING:
+    from pathlib import Path
     from typing import Any, Callable, Coroutine
 
     from jupyter_client import KernelClient
 
     from euporie.core.comm.base import KernelTab
 
 
@@ -46,50 +47,46 @@
 
 class Kernel:
     """Run a notebook kernel and communicates with it asynchronously.
 
     Has the ability to run itself in it's own thread.
     """
 
-    def _setup_loop(self) -> None:
-        """Set the current loop the the kernel's event loop.
-
-        This method is intended to be run in the kernel thread.
-        """
-        asyncio.set_event_loop(self.loop)
-        self.loop.run_forever()
-
     def __init__(
         self,
         kernel_tab: KernelTab,
         threaded: bool = True,
         allow_stdin: bool = False,
         default_callbacks: MsgCallbacks | None = None,
+        connection_file: Path | None = None,
     ) -> None:
         """Call when the :py:class:`Kernel` is initialized.
 
         Args:
             kernel_tab: The notebook this kernel belongs to
             threaded: If :py:const:`True`, run kernel communication in a separate thread
             allow_stdin: Whether the kernel is allowed to request input
             default_callbacks: The default callbacks to use on recipt of a message
+            connection_file: Path to a file from which to load or to hwich to save
+                kernel connection information
 
         """
         self.threaded = threaded
         if threaded:
             self.loop = asyncio.new_event_loop()
             self.thread = threading.Thread(target=self._setup_loop)
             self.thread.daemon = True
             self.thread.start()
         else:
             self.loop = asyncio.get_event_loop()
 
         self.allow_stdin = allow_stdin
 
         self.kernel_tab = kernel_tab
+        self.connection_file = connection_file
         self.kc: KernelClient | None = None
         self.km = AsyncKernelManager(
             kernel_name=str(kernel_tab.kernel_name),
         )
         self._status = "stopped"
         self.error: Exception | None = None
         self.dead = False
@@ -121,15 +118,22 @@
         # purpose of adding the depreciated :file:`.ipython/kernels` folder to the list
         # of kernel search paths. Without this, having IPython installed causes a
         # import race condition error where IPython was imported in the main thread for
         # displaying LaTeX and in the kernel thread to discover kernel paths.
         # Also this speeds up launch since importing IPython is pretty slow.
         self.km.kernel_spec_manager.kernel_dirs = jupyter_path("kernels")
 
+    def _setup_loop(self) -> None:
+        """Set the current loop the the kernel's event loop.
+
+        This method is intended to be run in the kernel thread.
+        """
+        asyncio.set_event_loop(self.loop)
         self.status_change_event = asyncio.Event()
+        self.loop.run_forever()
 
     def _aodo(
         self,
         coro: Coroutine,
         wait: bool = False,
         callback: Callable | None = None,
         timeout: int | float | None = None,
@@ -230,15 +234,15 @@
 
             self._aodo(_wait(), wait=True)
 
     @property
     def missing(self) -> bool:
         """Return True if the requested kernel is not found."""
         try:
-            self.km.kernel_spec
+            self.km.kernel_spec  # noqa B018
         except NoSuchKernel:
             return True
         else:
             return self.km.kernel_spec is None
 
     @property
     def id(self) -> str | None:
@@ -268,24 +272,35 @@
         if self.km.kernel_name is None:
             self.status = "error"
         log.debug("Starting kernel")
         self.status = "starting"
 
         # If we are connecting to an existing kernel, create a kernel client using
         # the given connection file
-        if self.kernel_tab.app.config.kernel_connection_file:
-            connection_file = self.kernel_tab.app.config.kernel_connection_file
-            self.km.load_connection_file(connection_file)
-            kc = self.km.client_factory(connection_file=connection_file)
+        runtime_dir = UPath(jupyter_runtime_dir())
+        if (connection_file := self.connection_file) is None:
+            id_ = str(uuid4())[:8]
+            connection_file = runtime_dir / f"kernel-euporie-{id_}.json"
+        connection_file_str = str(connection_file)
+        self.km.connection_file = connection_file_str
+
+        if connection_file.exists():
+            log.debug(
+                "Connecting to existing kernel using connection file '%s'",
+                connection_file,
+            )
+            self.km.load_connection_file(connection_file_str)
+            kc = self.km.client_factory(connection_file=connection_file_str)
             kc.load_connection_file()
             kc.start_channels()
             self.kc = kc
 
         # Otherwise, start a new kernel using the kernel manager
         else:
+            runtime_dir.mkdir(exist_ok=True, parents=True)
             while True:
                 try:
                     # TODO - send stdout to log
                     await self.km.start_kernel(stdout=DEVNULL, stderr=DEVNULL)
                 except _DeadlockError:
                     # Keep trying if we get an import deadlock
                     continue
@@ -993,39 +1008,47 @@
         """Restart the current kernel."""
         self._aodo(
             self.restart_(),
             wait=wait,
             callback=cb,
         )
 
-    def change(self, name: str, cb: Callable | None = None) -> None:
+    def change(
+        self,
+        name: str | None,
+        connection_file: Path | None = None,
+        cb: Callable | None = None,
+    ) -> None:
         """Change the kernel.
 
         Args:
             name: The name of the kernel to change to
+            connection_file: The path to the connection file to use
             cb: Callback to run once restarted
 
         """
+        self.connection_file = connection_file
         self.status = "starting"
 
         # Update the tab's kernel spec
-        spec = self.specs.get(name, {}).get("spec", {})
+        spec = self.specs.get(name or "", {}).get("spec", {})
         self.kernel_tab.metadata["kernelspec"] = {
             "name": name,
-            "display_name": spec["display_name"],
-            "language": spec["language"],
+            "display_name": spec.get("display_name", ""),
+            "language": spec.get("language", ""),
         }
 
         # Stop the old kernel
         if self.km.has_kernel:
             self.stop()
 
         # Create a new kernel manager instance
         del self.km
-        self.km = AsyncKernelManager(kernel_name=name)
+        kwargs = {} if name is None else {"kernel_name": name}
+        self.km = AsyncKernelManager(**kwargs)
         self.error = None
 
         # Start the kernel
         self.start(cb=cb)
 
     def stop(self, cb: Callable | None = None, wait: bool = False) -> None:
         """Stop the current kernel.
@@ -1049,20 +1072,22 @@
                 self.stop_(),
                 callback=cb,
                 wait=wait,
             )
 
     async def shutdown_(self) -> None:
         """Shut down the kernel and close the event loop if running in a thread."""
+        # Clean up connection file
+        self.km.cleanup_connection_file()
+        # Stop kernel
         if self.km.has_kernel:
             await self.km.shutdown_kernel(now=True)
+        # Stop event loop
         if self.threaded:
             self.loop.stop()
-            self.loop.close()
-            log.debug("Loop closed")
 
     def shutdown(self, wait: bool = False) -> None:
         """Shutdown the kernel and close the kernel's thread.
 
         This is intended to be run when the notebook is closed: the
         :py:class:`~euporie.core.tabs.notebook.Kernel` cannot be restarted after this.
 
@@ -1072,21 +1097,7 @@
         """
         self._aodo(
             self.shutdown_(),
             wait=wait,
         )
         if self.threaded:
             self.thread.join(timeout=5)
-
-    # ################################### Settings ####################################
-
-    add_setting(
-        name="kernel_connection_file",
-        flags=["--kernel-connection-file"],
-        type_=str,
-        help_="Attempt to connect to an existing kernel using a JSON connection info file",
-        default="",
-        description="""
-            Load connection info from JSON dict. This allows euporie to connect to
-            existing kernels.
-        """,
-    )
```

### Comparing `euporie-2.3.2/euporie/core/keys.py` & `euporie-2.4.0/euporie/core/keys.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 from prompt_toolkit.input.ansi_escape_sequences import ANSI_SEQUENCES
 from prompt_toolkit.keys import Keys
 
 # Register additional keys
 extend_enum(Keys, "ControlEnter", "c-enter")
 extend_enum(Keys, "ControlShiftEnter", "c-s-enter")
 extend_enum(Keys, "ShiftEnter", "s-enter")
+extend_enum(Keys, "ControlBackspace", "c-backspace")
 
 # Assign escape sequences to new keys
 ANSI_SEQUENCES["\x1b[27;5;13~"] = Keys.ControlEnter  # type: ignore
 ANSI_SEQUENCES["\x1b[13;5u"] = Keys.ControlEnter  # type: ignore
 
 ANSI_SEQUENCES["\x1b[27;2;13~"] = Keys.ShiftEnter  # type: ignore
 ANSI_SEQUENCES["\x1b[13;2u"] = Keys.ShiftEnter  # type: ignore
 
 ANSI_SEQUENCES["\x1b[27;6;13~"] = Keys.ControlShiftEnter  # type: ignore
 ANSI_SEQUENCES["\x1b[13;6u"] = Keys.ControlShiftEnter  # type: ignore
 
 # CSI-u control+key
+ANSI_SEQUENCES["\x1b[32;5u"] = Keys.ControlSpace  # type: ignore
 ANSI_SEQUENCES["\x1b[97;5u"] = Keys.ControlA  # type: ignore
 ANSI_SEQUENCES["\x1b[98;5u"] = Keys.ControlB  # type: ignore
 ANSI_SEQUENCES["\x1b[99;5u"] = Keys.ControlC  # type: ignore
 ANSI_SEQUENCES["\x1b[100;5u"] = Keys.ControlD  # type: ignore
 ANSI_SEQUENCES["\x1b[101;5u"] = Keys.ControlE  # type: ignore
 ANSI_SEQUENCES["\x1b[102;5u"] = Keys.ControlF  # type: ignore
 ANSI_SEQUENCES["\x1b[103;5u"] = Keys.ControlG  # type: ignore
@@ -42,9 +44,10 @@
 ANSI_SEQUENCES["\x1b[116;5u"] = Keys.ControlT  # type: ignore
 ANSI_SEQUENCES["\x1b[117;5u"] = Keys.ControlU  # type: ignore
 ANSI_SEQUENCES["\x1b[118;5u"] = Keys.ControlV  # type: ignore
 ANSI_SEQUENCES["\x1b[119;5u"] = Keys.ControlW  # type: ignore
 ANSI_SEQUENCES["\x1b[120;5u"] = Keys.ControlX  # type: ignore
 ANSI_SEQUENCES["\x1b[121;5u"] = Keys.ControlY  # type: ignore
 ANSI_SEQUENCES["\x1b[122;5u"] = Keys.ControlZ  # type: ignore
+ANSI_SEQUENCES["\x1b[127;5u"] = Keys.ControlBackspace  # type: ignore
 ANSI_SEQUENCES["\x1b[27;2;9~"] = Keys.BackTab  # type: ignore
 ANSI_SEQUENCES["\x1b[9;2u"] = Keys.BackTab  # type: ignore
```

### Comparing `euporie-2.3.2/euporie/core/launch.py` & `euporie-2.4.0/euporie/core/launch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Define a simple app for launching euporie apps."""
 
 from __future__ import annotations
 
 from importlib.metadata import entry_points
 
 from euporie.core.config import Config, add_setting
-from euporie.core.log import default_logs
+from euporie.core.log import setup_logs
 
 APP_ALIASES = {
     "edit": "notebook",
 }
 
 
 class CoreApp:
@@ -19,20 +19,23 @@
     config = Config()
     log_stdout_level = "error"
 
     @classmethod
     def launch(cls) -> None:
         """Launch the app."""
         # Set up default logging
-        default_logs()
+        setup_logs()
 
         # Load the launcher's configuration
         cls.config.load(cls)
         app = cls.config.app
 
+        # Remove the app setting from the list of known settings
+        del Config.settings["app"]
+
         # Add aliases
         app = APP_ALIASES.get(app, app)
 
         # Run the application
         from euporie.core.__main__ import main
 
         main(app)
```

### Comparing `euporie-2.3.2/euporie/core/lexers.py` & `euporie-2.4.0/euporie/core/lexers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 """Relating to lexers."""
 
+from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
 from pygments.lexers import (
+    get_lexer_by_name,
     get_lexer_for_filename,
     guess_lexer,
     guess_lexer_for_filename,
 )
 from pygments.util import ClassNotFound
 
 if TYPE_CHECKING:
+    from pathlib import Path
+
     from pygments.lexer import Lexer as PygmentsLexerCls
-    from upath import UPath
 
 
-def detect_lexer(text: "str" = "", path: "UPath|None" = None) -> "PygmentsLexerCls":
+def detect_lexer(
+    text: str = "", path: Path | None = None, language: str = ""
+) -> PygmentsLexerCls | None:
     """Detect the pygments lexer for a file."""
     lexer = None
     if path is not None:
         try:
             lexer = get_lexer_for_filename(path)
         except ClassNotFound:
             try:
                 lexer = guess_lexer_for_filename(path, text)
             except ClassNotFound:
                 pass
+    if lexer is None and language:
+        try:
+            lexer = get_lexer_by_name(language)
+        except ClassNotFound:
+            pass
     if lexer is None:
         try:
             lexer = guess_lexer(text)
         except ClassNotFound:
             pass
     return lexer
```

### Comparing `euporie-2.3.2/euporie/core/log.py` & `euporie-2.4.0/euporie/core/log.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,16 +18,18 @@
     print_formatted_text as renderer_print_formatted_text,
 )
 from prompt_toolkit.shortcuts.utils import print_formatted_text
 from prompt_toolkit.styles.pygments import style_from_pygments_cls
 from prompt_toolkit.styles.style import Style, merge_styles
 from pygments.styles import get_style_by_name
 
+from euporie.core.config import add_setting
 from euporie.core.formatted_text.utils import indent, lex, wrap
 from euporie.core.style import LOG_STYLE
+from euporie.core.utils import dict_merge
 
 if TYPE_CHECKING:
     from types import TracebackType
     from typing import Any, Callable, TextIO
 
     from prompt_toolkit.formatted_text.base import StyleAndTextTuples
     from prompt_toolkit.styles.base import BaseStyle
@@ -35,30 +37,16 @@
     from euporie.core.config import Config
 
 log = logging.getLogger(__name__)
 
 LOG_QUEUE: deque = deque(maxlen=1000)
 
 
-def dict_merge(target_dict: dict, input_dict: dict) -> None:
-    """Merge the second dictionary onto the first."""
-    for k in input_dict:
-        if k in target_dict:
-            if isinstance(target_dict[k], dict) and isinstance(input_dict[k], dict):
-                dict_merge(target_dict[k], input_dict[k])
-            elif isinstance(target_dict[k], list) and isinstance(input_dict[k], list):
-                target_dict[k] = [*target_dict[k], *input_dict[k]]
-            else:
-                target_dict[k] = input_dict[k]
-        else:
-            target_dict[k] = input_dict[k]
-
-
 class FtFormatter(logging.Formatter):
-    """Bae class for formatted text logging formatter."""
+    """Base class for formatted text logging formatter."""
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """Create a new formatter instance."""
         super().__init__(*args, **kwargs)
         self.datefmt = self.datefmt or "%H:%M:%S"
 
     def prepare(
@@ -197,24 +185,22 @@
 
     def ft_format(
         self, record: logging.LogRecord, width: int | None = None
     ) -> FormattedText:
         """Format a log record as formatted text."""
         record = self.prepare(record)
         output: StyleAndTextTuples = [
+            ("", "["),
             ("class:pygments.literal.date", f"{record.asctime}"),
-            ("", " "),
+            ("", "] ["),
             (f"class:log.level.{record.levelname}", f"{record.levelname}"),
-            ("", " " * (10 - len(record.levelname))),
+            ("", "] ["),
+            ("class:pygments.comment", f"{record.name}"),
+            ("", "] "),
             ("class:log,msg", record.message),
-            ("", " "),
-            (
-                "class:pygments.comment",
-                f"{record.name}.{record.funcName}:{record.lineno}",
-            ),
             ("", "\n"),
         ]
         if record.exc_text:
             output += self.format_traceback(record.exc_text) + [("", "\n")]
         return FormattedText(output)
 
 
@@ -279,90 +265,14 @@
                 ),
                 margin=" " * msg_pad,
             )
         output += [("", "\n")]
         return FormattedText(output)
 
 
-def setup_logs(config: Config) -> None:
-    """Configure the logger for euporie."""
-    log_file_is_stdout = config.log_file in ("-", "/dev/stdout")
-
-    log_config = {
-        "version": 1,
-        "disable_existing_loggers": False,
-        "formatters": {
-            "file_format": {
-                "format": "{asctime} {levelname:<7} [{name}.{funcName}:{lineno}] {message}",
-                "style": "{",
-                "datefmt": "%Y-%m-%d %H:%M:%S",
-            },
-            "stdout_format": {
-                "()": "euporie.core.log.StdoutFormatter",
-            },
-            "log_tab_format": {
-                "()": "euporie.core.log.LogTabFormatter",
-            },
-        },
-        "handlers": {
-            **(
-                {
-                    "file": {
-                        "level": config.log_level.upper() or "ERROR",
-                        "class": "logging.FileHandler",
-                        "filename": Path(config.log_file).expanduser(),
-                        "formatter": "file_format",
-                    }
-                }
-                if config.log_file and not log_file_is_stdout
-                else {}
-            ),
-            "stdout": {
-                "level": config.log_level.upper()
-                if config.log_level and log_file_is_stdout
-                else (
-                    "critical"
-                    if (app_cls := config.app_cls) is None
-                    else app_cls.log_stdout_level
-                ),
-                "class": "euporie.core.log.FormattedTextHandler",
-                "pygments_theme": config.syntax_theme,
-                "formatter": "stdout_format",
-                "stream": sys.stdout,
-            },
-            "log_tab": {
-                "level": config.log_level.upper() or "INFO",
-                "class": "euporie.core.log.QueueHandler",
-                "formatter": "log_tab_format",
-                "queue": LOG_QUEUE,
-            },
-        },
-        "loggers": {
-            "euporie": {
-                "level": config.log_level.upper() or "INFO",
-                "handlers": ["log_tab", "stdout"]
-                + (["file"] if not log_file_is_stdout and config.log_file else []),
-                "propagate": False,
-            },
-        },
-        # Log everything to the internal logger
-        "root": {"handlers": ["log_tab"]},
-    }
-    # Update log_config based additional config provided
-    if config.log_config:
-        import json
-
-        extra_config = json.loads(config.log_config)
-        dict_merge(log_config, extra_config)
-    # Configure the logger
-    # Pytype used TypedDicts to validate the dictionary structure, but I cannot get
-    # this to work for some reason...
-    logging.config.dictConfig(log_config)  # type: ignore
-
-
 class stdout_to_log:
     """A decorator which captures standard output and logs it."""
 
     def __init__(
         self, log: logging.Logger, output: str = "Literal['stdout','stderr']"
     ) -> None:
         """Create a new instance of the capturing context manager.
@@ -421,57 +331,143 @@
     if issubclass(exc_type, KeyboardInterrupt):
         sys.__excepthook__(exc_type, exc_value, exc_traceback)
         return
     # Log the exception
     log.critical("Uncaught exception", exc_info=(exc_type, exc_value, exc_traceback))
 
 
-def default_logs() -> None:
-    """Apply the default logging configuration before euporie's config is loaded."""
-    logging.config.dictConfig(
-        {
-            "version": 1,
-            "disable_existing_loggers": False,
-            "formatters": {
-                "file_format": {
-                    "format": "{asctime} {levelname:<7} [{name}.{funcName}:{lineno}] {message}",
-                    "style": "{",
-                    "datefmt": "%Y-%m-%d %H:%M:%S",
-                },
-                "stdout_format": {
-                    "()": StdoutFormatter,
-                },
-                "log_tab_format": {
-                    "()": LogTabFormatter,
-                },
+def setup_logs(config: Config | None = None) -> None:
+    """Configure the logger for euporie."""
+    # Default log config
+    log_config: dict[str, Any] = {
+        "version": 1,
+        "disable_existing_loggers": False,
+        "formatters": {
+            "file_format": {
+                "format": "{asctime} {levelname:<7} [{name}.{funcName}:{lineno}] {message}",
+                "style": "{",
+                "datefmt": "%Y-%m-%d %H:%M:%S",
+            },
+            "stdout_format": {
+                "()": StdoutFormatter,
             },
-            "handlers": {
-                "stdout": {
-                    "level": "INFO",
-                    "()": FormattedTextHandler,
-                    "formatter": "stdout_format",
-                    "stream": sys.stdout,
-                },
-                "log_tab": {
-                    "level": "INFO",
-                    "()": QueueHandler,
-                    "formatter": "log_tab_format",
-                    "queue": LOG_QUEUE,
-                },
+            "log_tab_format": {
+                "()": LogTabFormatter,
             },
-            "loggers": {
-                "euporie": {
-                    "level": "INFO",
-                    "handlers": ["log_tab", "stdout"],
-                    "propagate": False,
-                },
+        },
+        "handlers": {
+            "stdout": {
+                "level": "INFO",
+                "()": FormattedTextHandler,
+                "formatter": "stdout_format",
+                "stream": sys.stdout,
+            },
+            "log_tab": {
+                "level": "INFO",
+                "()": QueueHandler,
+                "formatter": "log_tab_format",
+                "queue": LOG_QUEUE,
+            },
+        },
+        "loggers": {
+            "euporie": {
+                "level": "INFO",
+                "handlers": ["log_tab", "stdout"],
+                "propagate": False,
             },
-            # Log everything to the internal logger
-            "root": {"handlers": ["log_tab"]},
-        }
-    )  # type: ignore
+        },
+        # Log everything to the internal logger
+        "root": {"handlers": ["log_tab"]},
+    }
+
+    if config is not None:
+        log_file = config.get("log_file", "")
+        log_file_is_stdout = log_file in {"-", "/dev/stdout"}
+        log_level = config.log_level.upper()
+
+        # Configure file handler
+        if log_file and not log_file_is_stdout:
+            log_config["handlers"]["file"] = {
+                "level": log_level,
+                "class": "logging.FileHandler",
+                "filename": Path(config.log_file).expanduser(),
+                "formatter": "file_format",
+            }
+            log_config["loggers"]["euporie"]["handlers"].append("file")
+
+        # Configure stdout handler
+        if log_file_is_stdout:
+            stdout_level = log_level
+        elif (app_cls := config.app_cls) is not None and (
+            log_stdout_level := app_cls.log_stdout_level
+        ):
+            stdout_level = log_stdout_level.upper()
+        else:
+            stdout_level = "CRITICAL"
+        log_config["handlers"]["stdout"]["level"] = stdout_level
+        log_config["handlers"]["stdout"]["pygments_theme"] = config.get(
+            "syntax_theme", "euporie"
+        )
+
+        # Configure euporie logger
+        log_config["loggers"]["euporie"]["level"] = config.log_level.upper()
+
+        # Update log_config based on additional config dict provided
+        if config.log_config:
+            import json
+
+            extra_config = json.loads(config.log_config)
+            dict_merge(log_config, extra_config)
+
+    # Configure the logger
+    # Pytype used TypedDicts to validate the dictionary structure, but I cannot get
+    # this to work for some reason...
+    logging.config.dictConfig(log_config)  # type: ignore
 
     # Capture warnings so they show up in the logs
     logging.captureWarnings(True)
 
     # Log uncaught exceptions
     sys.excepthook = handle_exception
+
+
+# ################################### Settings ########################################
+
+
+add_setting(
+    name="log_file",
+    flags=["--log-file"],
+    nargs="?",
+    default="",
+    type_=str,
+    title="the log file path",
+    help_="File path for logs",
+    description="""
+        When set to a file path, the log output will be written to the given path.
+        If no value is given output will be sent to the standard output.
+    """,
+)
+
+add_setting(
+    name="log_level",
+    flags=["--log-level"],
+    type_=str,
+    default="warning",
+    title="the log level",
+    help_="Set the log level",
+    choices=["debug", "info", "warning", "error", "critical"],
+    description="""
+        When set, logging events at the given level are emitted.
+    """,
+)
+
+add_setting(
+    name="log_config",
+    flags=["--log-config"],
+    type_=str,
+    default=None,
+    title="additional logging configuration",
+    help_="Additional logging configuration",
+    description="""
+        A JSON string specifying additional logging configuration.
+    """,
+)
```

### Comparing `euporie-2.3.2/euporie/core/margins.py` & `euporie-2.4.0/euporie/core/margins.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     from prompt_toolkit.layout.controls import UIContent
     from prompt_toolkit.layout.mouse_handlers import MouseHandlers
     from prompt_toolkit.layout.screen import Screen, WritePosition
 
     class ScrollableContainer(Protocol):
         """Protocol for a scrollable container."""
 
-        render_info: WindowRenderInfo
+        render_info: WindowRenderInfo | None
         vertical_scroll: int
 
 
 log = logging.getLogger(__name__)
 
 
 class ClickableMargin(Margin, metaclass=ABCMeta):
@@ -61,25 +61,31 @@
         self.target = target
         self.render_info: WindowRenderInfo | None = None
         self.content = FormattedTextControl(self.create_fragments)
 
     def create_fragments(self) -> StyleAndTextTuples:
         """Generate text fragments to display."""
         return self.margin.create_margin(
-            self.target.render_info,
+            cast("WindowRenderInfo", self.target.render_info),  # Minor type hack
             self.write_position.width,
             self.write_position.height,
         )
 
     def reset(self) -> None:
         """Reet the state of this container and all the children."""
 
     def preferred_width(self, max_available_width: int) -> Dimension:
         """Return a the desired width for this container."""
-        width = self.margin.get_width(lambda: self.target.render_info.ui_content)
+
+        def _get_ui_content() -> UIContent:
+            render_info = self.target.render_info
+            assert render_info is not None
+            return render_info.ui_content
+
+        width = self.margin.get_width(_get_ui_content)
         return Dimension(min=width, max=width)
 
     def preferred_height(self, width: int, max_available_height: int) -> Dimension:
         """Return a thedesired height for this container."""
         return Dimension()
 
     def write_to_screen(
@@ -182,15 +188,15 @@
     eighths = "█▇▆▅▄▃▂▁ "
 
     def __init__(
         self,
         display_arrows: FilterOrBool = True,
         up_arrow_symbol: str = "▴",
         down_arrow_symbol: str = "▾",
-        autohide: FilterOrBool = True,
+        autohide: FilterOrBool = False,
         smooth: bool = True,
         style: str = "",
     ) -> None:
         """Create a new scrollbar instance."""
         self.display_arrows = to_filter(display_arrows)
         self.up_arrow_symbol = up_arrow_symbol
         self.down_arrow_symbol = down_arrow_symbol
@@ -210,41 +216,50 @@
 
     def get_width(self, get_ui_content: Callable[[], UIContent]) -> int:
         """Return the scrollbar width: always 1."""
         return 1
 
     def create_margin(
         self,
-        window_render_info: WindowRenderInfo,
+        window_render_info: WindowRenderInfo | None,
         width: int,
         height: int,
         margin_render_info: WindowRenderInfo | None = None,
     ) -> StyleAndTextTuples:
         """Create the margin's formatted text."""
         result: StyleAndTextTuples = []
 
         self.window_render_info = window_render_info
         self.margin_render_info = margin_render_info
 
-        if window_render_info is None or not width:
+        # If this is the first time the target is being drawn, it may not yet have a
+        # render_info yet. Thus, invalidate the app so we can immediately redraw the
+        # scroll-bar with the render_info
+        if window_render_info is None:
+            get_app().invalidate()
+
+        if not width:
             return result
 
         # Show we render the arrow buttons?
         display_arrows = self.display_arrows()
 
         # The height of the scrollbar, excluding the optional buttons
-        self.track_height = window_render_info.window_height
+        self.track_height = (
+            window_render_info.window_height if window_render_info else height
+        )
         if display_arrows:
             self.track_height -= 2
 
         # Height of all text in the output: If there is none, we cannot divide
         # by zero so we hide the thumb
-        content_height = window_render_info.content_height
-        if content_height == 0 or content_height <= len(
-            window_render_info.displayed_lines
+        if (
+            window_render_info is None
+            or (content_height := window_render_info.content_height) == 0
+            or content_height <= len(window_render_info.displayed_lines)
         ):
             self.thumb_size = 0
         else:
             # The thumb is the part which moves, floating on the track: calculate its size
             fraction_visible = len(window_render_info.displayed_lines) / (
                 content_height
             )
@@ -255,15 +270,17 @@
                 )
                 / 8
             )
         if not self.smooth:
             self.thumb_size = int(self.thumb_size)
 
         # Calculate the position of the thumb
-        if content_height <= len(window_render_info.displayed_lines):
+        if window_render_info is None or content_height <= len(
+            window_render_info.displayed_lines
+        ):
             fraction_above = 0.0
         else:
             fraction_above = window_render_info.vertical_scroll / (
                 content_height - len(window_render_info.displayed_lines)
             )
         self.thumb_top = max(
             0,
@@ -377,15 +394,16 @@
 
         Returns:
             :py:const:`NotImplemented` is eturned when the mouse event is unhandled;
             :py:const:`None` is returned when the mouse event is handled successfully
 
         """
         render_info = self.window_render_info
-        assert render_info is not None
+        if render_info is None:
+            return NotImplemented
 
         content_height = render_info.content_height
         if isinstance(mouse_event, MouseEvent):
             cell_position = mouse_event.cell_position
         else:
             cell_position = RelativePosition(0.5, 0.5)
         row = mouse_event.position.y + cell_position.y
@@ -406,17 +424,17 @@
             # Use the window's current vertical scroll as it may have changed since the
             # window_render_info was generated
             window = render_info.window
             delta = window.vertical_scroll - target_scroll
 
             if isinstance(window, Window):
                 if delta < 0:
-                    func = window._scroll_up
-                else:
                     func = window._scroll_down
+                else:
+                    func = window._scroll_up
                 for _ in range(abs(delta)):
                     func()
             elif hasattr(window, "scrolling"):
                 render_info.window.scrolling = delta
 
         # Mouse down events
         elif mouse_event.event_type == MouseEventType.MOUSE_DOWN:
```

### Comparing `euporie-2.3.2/euporie/core/processors.py` & `euporie-2.4.0/euporie/core/processors.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """Buffer processors."""
 
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
+from prompt_toolkit.data_structures import Point
 from prompt_toolkit.layout.processors import (
     AppendAutoSuggestion,
     Processor,
     Transformation,
 )
 from prompt_toolkit.layout.utils import explode_text_fragments
+from prompt_toolkit.utils import get_cwidth
 
 if TYPE_CHECKING:
+    from typing import Callable
+
     from prompt_toolkit.layout.processors import TransformationInput
 
 
 log = logging.getLogger(__name__)
 
 
 class AppendLineAutoSuggestion(AppendAutoSuggestion):
@@ -57,7 +61,38 @@
             for i in range(len(fragments) - 1, -1, -1):
                 style, char, *_ = fragments[i]
                 if char == " ":
                     fragments[i] = (f"{style} {self.style}", new_char)
                 else:
                     break
         return Transformation(fragments)
+
+
+class CursorProcessor(Processor):
+    """Show a mouse cursor."""
+
+    def __init__(
+        self,
+        get_cursor_position: Callable[[], Point],
+        char: str = "🮰",
+        style: str = "class:mouse",
+    ) -> None:
+        """Create a new processor instance."""
+        self.char = char
+        self.style = style
+        self.get_cursor_position = get_cursor_position
+
+    def apply_transformation(self, ti: TransformationInput) -> Transformation:
+        """Replace character at the cursor position."""
+        pos = self.get_cursor_position()
+        fragments = ti.fragments
+        if ti.lineno == pos.y:
+            fragments = explode_text_fragments(fragments)
+            if (length := len(fragments)) < (x := pos.x):
+                fragments.append(("", " " * (x - length)))
+            frag = fragments[x]
+            char = self.char.ljust(get_cwidth(frag[1]))
+            fragments[x] = (
+                f"{frag[0]} {self.style}",
+                char,
+            )
+        return Transformation(fragments)
```

### Comparing `euporie-2.3.2/euporie/core/pygments.py` & `euporie-2.4.0/euporie/core/pygments.py`

 * *Files identical despite different names*

### Comparing `euporie-2.3.2/euporie/core/reference.py` & `euporie-2.4.0/euporie/core/reference.py`

 * *Files identical despite different names*

### Comparing `euporie-2.3.2/euporie/core/renderer.py` & `euporie-2.4.0/euporie/core/renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,38 +259,54 @@
         full_screen: bool = False,
         mouse_support: FilterOrBool = False,
         cpr_not_supported_callback: Callable[[], None] | None = None,
         extend_height: FilterOrBool = False,
         extend_width: FilterOrBool = False,
     ) -> None:
         """Create a new :py:class:`Renderer` instance."""
+        self.app: Application[Any] | None = None
         super().__init__(
             style, output, full_screen, mouse_support, cpr_not_supported_callback
         )
         self.extend_height = to_filter(extend_height)
         self.extend_width = to_filter(extend_width)
 
     def reset(self, _scroll: bool = False, leave_alternate_screen: bool = True) -> None:
         """Disable extended keys before resetting the output."""
+        from euporie.core.app import BaseApp
+
+        super().reset(_scroll, leave_alternate_screen)
+
         output = self.output
 
         # Disable extended keys
-        if isinstance(output, Vt100_Output):
-            cast(Vt100_Output, self.output).disable_extended_keys()
-
-        super().reset(_scroll, leave_alternate_screen)
+        app = self.app
+        if (
+            app
+            and isinstance(app, BaseApp)
+            and app.term_info.csiu_status.value
+            and isinstance(output, Vt100_Output)
+        ):
+            cast("Vt100_Output", self.output).disable_extended_keys()
 
     def render(
         self, app: Application[Any], layout: Layout, is_done: bool = False
     ) -> None:
         """Render the current interface to the output."""
+        from euporie.core.app import BaseApp
+
         output = self.output
+        self.app = app
 
         # Enable extended keys
-        if isinstance(output, Vt100_Output):
+        if (
+            isinstance(app, BaseApp)
+            and app.term_info.csiu_status.value
+            and isinstance(output, Vt100_Output)
+        ):
             output.enable_extended_keys()
 
         # Enter alternate screen.
         if self.full_screen and not self._in_alternate_screen:
             self._in_alternate_screen = True
             output.enter_alternate_screen()
```

### Comparing `euporie-2.3.2/euporie/core/style.py` & `euporie-2.4.0/euporie/core/style.py`

 * *Files 2% similar despite different names*

```diff
@@ -394,14 +394,16 @@
         "app-tab-bar": f"bg:{cp.bg.less(0.15)}",
         "app-tab-bar border": f"fg:{cp.bg.more(0.1)}",
         "app-tab-bar tab inactive": f"fg:{cp.fg.more(0.5)}",
         "app-tab-bar tab inactive border": f"fg:{cp.bg.more(0.15)}",
         "app-tab-bar tab active": "bold fg:default bg:default",
         "app-tab-bar tab active close": "fg:darkred",
         "app-tab-bar tab active border top": f"fg:{cp.hl} bg:{cp.bg.less(0.15)}",
+        # Tabs
+        "loading": "fg:#888888",
         # Buffer
         "line-number": f"fg:{cp.fg.more(0.5)} bg:{cp.bg.more(0.05)}",
         "line-number.current": f"bold orange bg:{cp.bg.more(0.1)}",
         "line-number edge": f"fg:{cp.bg.darker(0.1)}",
         "line-number.current edge": f"fg:{cp.bg.darker(0.1)}",
         "cursor-line": f"bg:{cp.bg.more(0.05)}",
         "cursor-line search": f"bg:{cp.bg.more(0.02)}",
@@ -430,44 +432,47 @@
         "cell input prompt": "fg:blue",
         "cell output prompt": "fg:red",
         "cell show outputs": "bg:#888",
         "cell show inputs": "bg:#888",
         # Scrollbars
         "scrollbar": f"fg:{cp.bg.more(0.75)} bg:{cp.bg.more(0.15)}",
         "scrollbar.background": f"fg:{cp.bg.more(0.75)} bg:{cp.bg.more(0.15)}",
-        "scrollbar.arrow": f"fg:{cp.bg.more(0.75)} bg:{cp.bg.more(0.15)}",
+        "scrollbar.arrow": f"fg:{cp.bg.more(0.75)} bg:{cp.bg.more(0.20)}",
         "scrollbar.start": "",
         # "scrollbar.start": f"fg:{cp.bg.more(0.75)} bg:{cp.bg.more(0.25)}",
         "scrollbar.button": f"fg:{cp.bg.more(0.75)} bg:{cp.bg.more(0.75)}",
         "scrollbar.end": f"fg:{cp.bg.more(0.15)} bg:{cp.bg.more(0.75)}",
         # Overflow margin
         "overflow": f"fg:{cp.fg.more(0.5)}",
         # Dialogs
-        "dialog title": f"fg:white bg:{cp.hl.darker(0.25)} bold",
-        "dialog title border": "fg:ansired",
+        "dialog dialog-title": f"fg:white bg:{cp.hl.darker(0.25)} bold",
         "dialog": f"fg:{cp.fg.base} bg:{cp.bg.darker(0.1)}",
         "dialog text-area": f"bg:{cp.bg.lighter(0.05)}",
         "dialog input text text-area": f"fg:default bg:{cp.bg.less(0.1)}",
         "dialog text-area last-line": "nounderline",
         "dialog border": f"fg:{cp.bg.darker(0.1).more(0.1)}",
         # Horizontals rule
         "hr": "fg:ansired",
         # Completions menu
-        "completion-menu.completion.keyword": "fg:#d700af",
-        "completion-menu.completion.current.keyword": "fg:#fff bg:#d700ff",
-        "completion-menu.completion.function": "fg:#005faf",
-        "completion-menu.completion.current.function": "fg:#fff bg:#005fff",
-        "completion-menu.completion.class": "fg:#008700",
-        "completion-menu.completion.current.class": "fg:#fff bg:#00af00",
-        "completion-menu.completion.statement": "fg:#5f0000",
-        "completion-menu.completion.current.statement": "fg:#fff bg:#5f0000",
-        "completion-menu.completion.instance": "fg:#d75f00",
-        "completion-menu.completion.current.instance": "fg:#fff bg:#d78700",
-        "completion-menu.completion.module": "fg:#d70000",
-        "completion-menu.completion.current.module": "fg:#fff bg:#d70000",
+        "menu completion-keyword": "fg:#d700af",
+        "menu completion-function": "fg:#005faf",
+        "menu completion-class": "fg:#008700",
+        "menu completion-statement": "fg:#5f0000",
+        "menu completion-instance": "fg:#d75f00",
+        "menu completion-module": "fg:#d70000",
+        "menu completion-magic": "fg:#888888",
+        "menu completion-path": "fg:#aa8800",
+        "menu selection completion-keyword": f"fg:{ColorPaletteColor('#d700af').lighter(0.75)}",
+        "menu selection completion-function": f"fg:{ColorPaletteColor('#005faf').lighter(0.75)}",
+        "menu selection completion-class": f"fg:{ColorPaletteColor('#008700').lighter(0.75)}",
+        "menu selection completion-statement": f"fg:{ColorPaletteColor('#5f0000').lighter(0.75)}",
+        "menu selection completion-instance": f"fg:{ColorPaletteColor('#d75f00').lighter(0.75)}",
+        "menu selection completion-module": f"fg:{ColorPaletteColor('#d70000').lighter(0.75)}",
+        "menu selection completion-magic": f"fg:{ColorPaletteColor('#888888').lighter(0.75)}",
+        "menu selection completion-path": f"fg:{ColorPaletteColor('#aa8800').lighter(0.75)}",
         # Log
         "log.level.nonset": "fg:grey",
         "log.level.debug": "fg:green",
         "log.level.info": "fg:blue",
         "log.level.warning": "fg:yellow",
         "log.level.error": "fg:red",
         "log.level.critical": "fg:red bold",
@@ -508,19 +513,29 @@
         "side_bar buttons": f"bg:{cp.bg.less(0.15)}",
         "side_bar buttons hovered": f"fg:{cp.hl}",
         "side_bar buttons selection": f"fg:{cp.fg} bg:{cp.hl}",
         "side_bar buttons separator": f"fg:{cp.bg.less(0.15)} bg:{cp.bg.less(0.15)}",
         "side_bar buttons separator selection before": f"fg:{cp.bg.less(0.15)} bg:{cp.hl}",
         "side_bar buttons separator selection after": f"fg:{cp.hl} bg:{cp.bg.less(0.15)}",
         # Tabbed split
-        "tabbed-split tab-bar tab inactive": f"fg:{cp.bg.more(0.1)}",
-        "tabbed-split tab-bar tab inactive border": f"fg:{cp.bg.more(0.15)}",
+        "tabbed-split border": f"fg:{cp.bg.more(0.2)}",
+        "tabbed-split border left": f"bg:{cp.bg.more(0.025)}",
+        "tabbed-split border right": f"bg:{cp.bg.more(0.025)}",
+        "tabbed-split border bottom left": f"bg:{cp.bg}",
+        "tabbed-split border bottom right": f"bg:{cp.bg}",
+        "tabbed-split page": f"bg:{cp.bg.more(0.025)}",
+        "dialog tabbed-split border bottom right": f"bg:{cp.bg.darker(0.1)}",
+        "dialog tabbed-split border bottom left": f"bg:{cp.bg.darker(0.1)}",
+        "tabbed-split tab-bar tab inactive": f"fg:{cp.bg.more(0.3)}",
+        "tabbed-split tab-bar tab inactive title": f"bg:{cp.bg.darker(0.05)}",
+        "tabbed-split tab-bar tab inactive border left": f"bg:{cp.bg.darker(0.05)}",
+        "tabbed-split tab-bar tab inactive border right": f"bg:{cp.bg.darker(0.05)}",
         "tabbed-split tab-bar tab active": f"bold fg:{cp.fg}",
+        "tabbed-split tab-bar tab active title": f"bg:{cp.bg.more(0.025)}",
         "tabbed-split tab-bar tab active close": "fg:darkred",
-        "tabbed-split border": f"fg:{cp.bg.more(0.2)}",
         # Ipywidgets
         "ipywidget focused": f"bg:{cp.bg.more(0.05)}",
         "ipywidget slider track": f"fg:{cp.fg.darker(0.5)}",
         "ipywidget slider arrow": f"fg:{cp.fg.darker(0.25)}",
         "ipywidget slider handle": f"fg:{cp.fg.darker(0.25)}",
         "ipywidget accordion border default": f"fg:{cp.bg.more(0.2)}",
         ## Styled borders
@@ -607,15 +622,15 @@
         "input inset border top selection": f"fg:{cp.bg.lighter(0.5)}",
         "input inset border left selection": f"fg:{cp.bg.lighter(0.5)}",
         "input inset border bottom selection focused": f"fg:{cp.hl.darker(0.5)}",
         "input inset border right selection focused": f"fg:{cp.hl.darker(0.5)}",
         "input inset border top selection focused": f"fg:{cp.hl.lighter(0.5)}",
         "input inset border left selection focused": f"fg:{cp.hl.lighter(0.5)}",
         "input text placeholder": f"fg:{cp.fg.more(0.6)}",
-        "input text text-area": f"bg:{cp.bg.lighter(0.1)}",
+        "input text text-area": f"fg:default bg:{cp.bg.lighter(0.1)}",
         "input text border top": f"fg:{cp.bg.darker(0.5)}",
         "input text border right": f"fg:{cp.bg.lighter(0.25)}",
         "input text border bottom": f"fg:{cp.bg.lighter(0.25)}",
         "input text border left": f"fg:{cp.bg.darker(0.5)}",
         "input text border top focused": f"fg:{cp.hl.darker(0.5)}",
         "input text border right focused": f"fg:{cp.hl.lighter(0.5)}",
         "input text border bottom focused": f"fg:{cp.hl.lighter(0.5)}",
```

### Comparing `euporie-2.3.2/euporie/core/suggest.py` & `euporie-2.4.0/euporie/core/suggest.py`

 * *Files identical despite different names*

### Comparing `euporie-2.3.2/euporie/core/terminal.py` & `euporie-2.4.0/euporie/core/terminal.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,32 +128,14 @@
         Returns:
             The last value received, or the default value.
 
         """
         return self._value or self.default
 
 
-class ColorQueryMixin:
-    """A mixin for terminal queries which check a terminal colour."""
-
-    pattern: re.Pattern
-
-    def verify(self, data: str) -> str | None:
-        """Verify the response contains a colour."""
-        if match := self.pattern.match(data):
-            if colors := match.groupdict():
-                r, g, b = (
-                    colors.get("r", "00"),
-                    colors.get("g", "00"),
-                    colors.get("b", "00"),
-                )
-                return f"#{r[:2]}{g[:2]}{b[:2]}"
-        return None
-
-
 class Colors(TerminalQuery):
     """A terminal query to retrieve colours as hex codes."""
 
     _color_names = {
         "10": "fg",
         "11": "bg",
         "4;0": "ansiblack",
@@ -233,14 +215,15 @@
     default = False
     cache = True
     cmd = "\x1b_Gi=4294967295,s=1,v=1,a=q,t=d,f=24;AAAA\x1b\\"
     # Konsole responds with 'i=0' - I'll allow it
     pattern = re.compile(r"^\x1b_Gi=(4294967295|0);(?P<status>OK)\x1b\\\Z")
 
     def _cmd(self) -> str:
+        """Hide the command in case the terminal does not support this sequence."""
         return "\x1b[s" + tmuxify(self.cmd) + "\x1b[u\x1b[2K"
 
     def verify(self, data: str) -> bool:
         """Verify the terminal response means kitty graphics are supported."""
         if match := self.pattern.match(data):
             if values := match.groupdict():
                 if values.get("status") == "OK":
@@ -324,84 +307,109 @@
 
 
 class SgrPixelStatus(TerminalQuery):
     """A terminal query to check for Pixel SGR support."""
 
     default = False
     cache = True
-    cmd = "\x1b[?1016$p"
+    cmd = "\x1b[?1016h\x1b[?1016$p\x1b[?1016l"  # Enable, check, disable
     pattern = re.compile(r"^\x1b\[\?1016;(?P<Pm>\d)\$\Z")
 
     def verify(self, data: str) -> bool:
         """Verify the terminal response means sixel graphics are supported."""
         if match := self.pattern.match(data):
             if values := match.groupdict():
-                if values.get("Pm") != 0:
+                if values.get("Pm") in {"1", "3"}:
                     return True
         return False
 
 
+class CsiUStatus(TerminalQuery):
+    """A terminal query to check for CSI-u support."""
+
+    default = False
+    cache = True
+    cmd = "\x1b[?u"
+    pattern = re.compile(r"^\x1b\[\?\d+u")
+
+    def verify(self, data: str) -> bool:
+        """Verify the terminal responds."""
+        if match := self.pattern.match(data):
+            if match:
+                return True
+        return False
+
+
 class TerminalInfo:
     """A class to gather and hold information about the terminal."""
 
     input: Input
     output: Output
 
+    _queries: dict[type[TerminalQuery], TerminalQuery] = {}
+
     def __init__(self, input_: Input, output: Output, config: Config) -> None:
         """Instantiate the terminal information class."""
         self.input = input_
         self.output = output
         self.config = config
-        self._queries: list[TerminalQuery] = []
 
         self.colors = self.register(Colors)
         self.pixel_dimensions = self.register(PixelDimensions)
         self.sixel_graphics_status = self.register(SixelGraphicsStatus)
         self.kitty_graphics_status = self.register(KittyGraphicsStatus)
         self.iterm_graphics_status = self.register(ItermGraphicsStatus)
         self.depth_of_color = self.register(DepthOfColor)
         self.sgr_pixel_status = self.register(SgrPixelStatus)
+        self.csiu_status = self.register(CsiUStatus)
 
     def register(self, query: type[TerminalQuery]) -> TerminalQuery:
         """Instantiate and registers a query's response with the input parser."""
         # Create an instance of this query
-        query_inst = query(self.output, config=self.config)
-        self._queries.append(query_inst)
+        query_inst: TerminalQuery | None
 
-        # If the query expects a response from the terminal, we need to add a
-        # key-binding for it and register it with the input parser
-        if query.pattern:
-            name = re.sub(r"(?<!^)(?=[A-Z])", "-", query.__name__).lower()
-            title = name.replace("-", " ")
-
-            # Add a "key" definition for this query
-            key_name = f"{query.__name__}Response"
-            key_code = f"<{name}-response>"
-            # Do not register the same key multiple times
-            if not hasattr(Keys, key_name):
-                extend_enum(Keys, key_name, key_code)
-            key = getattr(Keys, key_name)
-
-            # Register this key with the parser if supported
-            if parser := getattr(self.input, "vt100_parser", None):
-                # Register the key
-                parser.queries[key] = query.pattern
-
-            # Add a command for the query's key-binding
-            add_cmd(name=name, title=title, hidden=True)(query_inst._handle_response)
-            # Add key-binding
-            register_bindings({"euporie.core.app.BaseApp": {name: key}})
+        if (query_inst := self._queries.get(query)) is None:
+            query_inst = query(self.output, config=self.config)
+            self._queries[query] = query_inst
+
+            # If the query expects a response from the terminal, we need to add a
+            # key-binding for it and register it with the input parser
+            if query.pattern:
+                name = re.sub(r"(?<!^)(?=[A-Z])", "-", query.__name__).lower()
+                title = name.replace("-", " ")
+
+                # Add a "key" definition for this query
+                key_name = f"{query.__name__}Response"
+                key_code = f"<{name}-response>"
+                # Do not register the same key multiple times
+                if not hasattr(Keys, key_name):
+                    extend_enum(Keys, key_name, key_code)
+                key = getattr(Keys, key_name)
+
+                # Register this key with the parser if supported
+                if (parser := getattr(self.input, "vt100_parser", None)) and hasattr(
+                    parser, "queries"
+                ):
+                    # Register the key
+                    parser.queries[key] = query.pattern
+
+                # Add a command for the query's key-binding
+                add_cmd(name=name, title=title, hidden=True)(
+                    query_inst._handle_response
+                )
+                # Add key-binding
+                register_bindings({"euporie.core.app.BaseApp": {name: key}})
 
         return query_inst
 
     def send_all(self) -> None:
         """Send the command for all queries."""
         # Ensure line wrapping is off before sending queries
         self.output.disable_autowrap()
-        for query in self._queries:
+        for query in self._queries.values():
             query.send()
 
     def _tiocgwnsz(self) -> tuple[int, int, int, int]:
         """Get the size and pixel dimensions of the terminal with `termios`."""
         output = array.array("H", [0, 0, 0, 0])
         if _have_termios_tty_fcntl():
             import fcntl
```

### Comparing `euporie-2.3.2/euporie/core/validation.py` & `euporie-2.4.0/euporie/core/validation.py`

 * *Files identical despite different names*

### Comparing `euporie-2.3.2/euporie/core/comm/base.py` & `euporie-2.4.0/euporie/core/comm/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import TYPE_CHECKING
 from weakref import WeakKeyDictionary
 
 from euporie.core.current import get_app
 from euporie.core.widgets.display import Display
 
 if TYPE_CHECKING:
-    from typing import Any, Callable, Sequence
+    from typing import Any, Callable, Mapping, Sequence
 
     from prompt_toolkit.layout.containers import AnyContainer
 
     from euporie.core.kernel import Kernel
     from euporie.core.tabs.base import KernelTab
     from euporie.core.widgets.cell_outputs import OutputParent
 
@@ -25,25 +25,25 @@
 
 class CommView:
     """Hold a container and methods to update its attributes."""
 
     def __init__(
         self,
         container: AnyContainer,
-        setters: dict[str, Callable[..., None]] | None = None,
+        setters: Mapping[str, Callable[..., None]] | None = None,
     ) -> None:
         """Create a new instance of the Comm vieew.
 
         Args:
             container: The main container to display when this Comm is to be visualised
             setters: A dictionary mapping state names to callback functions which should
                 be called when the named state value changed.
         """
         self.container = container
-        self.setters = setters or {}
+        self.setters: dict[str, Callable[..., None]] = dict(setters or {})
         self.kernel: Kernel | None = None
 
     def update(self, changes: dict[str, Any]) -> None:
         """Update the view to reflect changes in the Comm.
 
         Calls any setter functions defined for the changed keys with the changed values
         as arguments.
@@ -113,8 +113,9 @@
 
 
 class UnimplementedComm(Comm):
     """Represent a Comm object which is not implemented in euporie.core."""
 
     def process_data(self, data: dict, buffers: Sequence[bytes]) -> None:
         """Doe nothing when data is received."""
-        return None
+        self.data = data
+        self.buffers = buffers
```

### Comparing `euporie-2.3.2/euporie/core/comm/ipywidgets.py` & `euporie-2.4.0/euporie/core/comm/ipywidgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     Text,
     ToggleButton,
     ToggleButtons,
 )
 from euporie.core.widgets.layout import AccordionSplit, ReferencedSplit, TabbedSplit
 
 if TYPE_CHECKING:
-    from typing import Any, Iterable, Sequence
+    from typing import Any, Iterable, MutableSequence, Sequence
 
     from prompt_toolkit.buffer import Buffer
     from prompt_toolkit.formatted_text.base import AnyFormattedText
     from prompt_toolkit.layout.containers import AnyContainer, _Split
 
     from euporie.core.comm.base import KernelTab
     from euporie.core.widgets.cell_outputs import OutputParent
@@ -62,15 +62,15 @@
 WIDGET_MODELS: dict[str, type[IpyWidgetComm]] = {}
 
 
 def _separate_buffers(
     substate: dict | list | tuple,
     path: list[str | int],
     buffer_paths: list[list[str | int]],
-    buffers: list[memoryview | bytearray | bytes],
+    buffers: MutableSequence[memoryview | bytearray | bytes],
 ) -> dict | list | tuple:
     """Remove binary types from dicts and lists, but keep track of their paths.
 
     Any part of the dict/list that needs modification will be cloned, so the original
     stays untouched.
 
     Args:
@@ -114,15 +114,15 @@
                 vnew = _separate_buffers(v, path + [k], buffer_paths, buffers)
                 if v is not vnew:  # only assign when value changed
                     if cloned_substrate is None:
                         cloned_substrate = dict(substate)  # clone list/tuple
                     cloned_substrate[k] = vnew
     else:
         raise ValueError("expected state to be a list or dict, not %r" % substate)
-    return cloned_substrate or substate
+    return cloned_substrate if cloned_substrate is not None else substate
 
 
 class IpyWidgetComm(Comm, metaclass=ABCMeta):
     """A Comm object which represents ipython widgets."""
 
     target_name = "jupyter.widget"
 
@@ -186,15 +186,15 @@
         state = _separate_buffers(self.data["state"], [], buffer_paths, buffers)
         assert isinstance(state, dict)
         output = {
             "model_name": state.get("_model_name"),
             "model_module": state.get("_model_module"),
             "model_module_version": state.get("_model_module_version"),
             "state": {
-                **{key: value for key, value in state.items()},
+                **dict(state.items()),
                 "buffers": [
                     {
                         "encoding": "base64",
                         "path": p,
                         "data": standard_b64encode(d).decode("ascii"),
                     }
                     for p, d in zip(buffer_paths, buffers)
@@ -288,15 +288,15 @@
                         ]
                 self.prev_msg_id = msg_id
 
         super().process_data(data, buffers)
 
 
 class LayoutIpyWidgetComm(IpyWidgetComm, metaclass=ABCMeta):
-    """Bae class for layout widgets with children."""
+    """Base class for layout widgets with children."""
 
     def render_children(
         self, models: list[str], parent: OutputParent
     ) -> list[AnyContainer]:
         """Create views for the child Comms in the layout."""
         return [
             self.comm_container.comms[
@@ -640,15 +640,15 @@
         value = self.data["state"].get("value", 0.0)
         if value not in options:
             bisect.insort(options, value)
         return options
 
 
 class SliderIpyWidgetComm(IpyWidgetComm, metaclass=ABCMeta):
-    """Bae class for slider ipywidgets."""
+    """Base class for slider ipywidgets."""
 
     def normalize(self, x: Any) -> Any:
         """Convert the internal widget's value to one compatible with the ipywidget."""
         return x
 
     @property
     @abstractmethod
@@ -718,15 +718,15 @@
         """Set the selected index when the ipywidget's selected value changes."""
         if value in slider.options:
             slider.index = slider.options.index(value)
             slider.value_changed()
 
 
 class RangeSliderIpyWidgetComm(SliderIpyWidgetComm):
-    """Bae class for range slider ipywidgets."""
+    """Base class for range slider ipywidgets."""
 
     @property
     def indices(self) -> list[int]:
         """Return the first and last selected indices."""
         output = []
         for value in self.data["state"]["value"]:
             if value in self.options:
@@ -769,15 +769,15 @@
 
 
 class FloatRangeSliderModel(FloatOptionsMixin, RangeSliderIpyWidgetComm):
     """A slider ipywidget that accepts a range of float values."""
 
 
 class NumberTextBoxIpyWidgetComm(TextBoxIpyWidgetComm, metaclass=ABCMeta):
-    """Bae class for text-box ipywidgets with numerical values."""
+    """Base class for text-box ipywidgets with numerical values."""
 
     def create_view(self, parent: OutputParent) -> CommView:
         """Create a new view of the numerical text-box ipywidget."""
         disabled = disabled = Condition(
             lambda: self.data["state"].get("disabled", False)
         )
 
@@ -895,15 +895,15 @@
 
 
 class FloatProgressModel(FloatOptionsMixin, ProgressIpyWidgetComm):
     """A progress bar ipywidget that accepts float values."""
 
 
 class ToggleableIpyWidgetComm(IpyWidgetComm, metaclass=ABCMeta):
-    """Bae class for toggleable ipywidgets."""
+    """Base class for toggleable ipywidgets."""
 
     def normalize(self, x: Any) -> float | None:
         """Cat the container's selected value to a bool if possible."""
         try:
             value = bool(x)
         except ValueError:
             return None
@@ -990,15 +990,15 @@
                 ),
             ),
             setters={"value": partial(setattr, checkbox, "selected")},
         )
 
 
 class SelectableIpyWidgetComm(IpyWidgetComm, metaclass=ABCMeta):
-    """Bae class for selectable ipywidgets."""
+    """Base class for selectable ipywidgets."""
 
     def update_index(self, container: SelectableWidget) -> None:
         """Send a ``comm_message`` updating the selected index when it changes."""
         self.set_state("index", container.index)
 
 
 class DropdownModel(SelectableIpyWidgetComm):
@@ -1094,15 +1094,15 @@
 
     def create_view(self, parent: OutputParent) -> CommView:
         """Create a new view of the multiple select widget."""
         select = Select(
             options=self.data["state"].get("_options_labels", []),
             indices=self.data["state"]["index"],
             on_change=self.update_index,
-            style="class:select,face",
+            style="class:select",
             multiple=True,
             rows=self.data["state"]["rows"],
             disabled=Condition(lambda: self.data["state"].get("disabled", False)),
         )
         return CommView(
             FocusedStyle(
                 LabelledWidget(
```

### Comparing `euporie-2.3.2/euporie/core/comm/registry.py` & `euporie-2.4.0/euporie/core/comm/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 
 from typing import TYPE_CHECKING
 
 from euporie.core.comm.base import UnimplementedComm
 from euporie.core.comm.ipywidgets import open_comm_ipywidgets
 
 if TYPE_CHECKING:
-    from typing import Any, Sequence
+    from typing import Any, Callable, Sequence
 
     from euporie.core.comm.base import Comm, KernelTab
 
-TARGET_CLASSES = {"jupyter.widget": open_comm_ipywidgets}
+TARGET_CLASSES: dict[str, Callable[[KernelTab, str, dict, Sequence[bytes]], Comm]] = {
+    "jupyter.widget": open_comm_ipywidgets
+}
 
 
 def open_comm(
     comm_container: KernelTab,
     content: dict[str, Any],
     buffers: Sequence[bytes],
 ) -> Comm:
@@ -32,12 +34,16 @@
 
     Returns:
         A class representing the comm
 
     """
     target_name = content.get("target_name", "")
     return TARGET_CLASSES.get(target_name, UnimplementedComm)(
-        comm_container=comm_container,
-        comm_id=str(content.get("comm_id")),
-        data=content.get("data", {}),
-        buffers=buffers,
+        # comm_container=
+        comm_container,
+        # comm_id=
+        str(content.get("comm_id")),
+        # data=
+        content.get("data", {}),
+        # buffers=
+        buffers,
     )
```

### Comparing `euporie-2.3.2/euporie/core/convert/utils.py` & `euporie-2.4.0/euporie/core/convert/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from importlib import import_module
 from shutil import which
 from typing import TYPE_CHECKING
 
 import imagesize
 from prompt_toolkit.filters import Condition, to_filter
 
-from euporie.core.convert.base import convert
+from euporie.core.convert.core import convert
 from euporie.core.current import get_app
 
 if TYPE_CHECKING:
     from typing import Any
 
     from prompt_toolkit.filters import Filter
```

### Comparing `euporie-2.3.2/euporie/core/convert/formats/ansi.py` & `euporie-2.4.0/euporie/core/convert/formats/ansi.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from __future__ import annotations
 
 import logging
 from functools import partial
 from math import ceil
 from typing import TYPE_CHECKING
 
-from euporie.core.convert.base import register
+from euporie.core.convert.core import register
 from euporie.core.convert.formats.common import chafa_convert_cmd, chafa_convert_py
 from euporie.core.convert.formats.pil import set_background
 from euporie.core.convert.utils import call_subproc, commands_exist, have_modules
 from euporie.core.current import get_app
 
 if TYPE_CHECKING:
+    from pathlib import Path
     from typing import Any
 
     from PIL.Image import Image as PilImage
     from rich.console import RenderableType
-    from upath import UPath
 
 log = logging.getLogger(__name__)
 
 
 @register(
     from_="html",
     to="ansi",
@@ -30,15 +30,15 @@
 )
 def html_to_ansi_w3m(
     data: str,
     width: int | None = None,
     height: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert HTML text to formatted ANSI using :command:`w3m`."""
     cmd: list[Any] = ["w3m", "-T", "text/html"]
     if width is not None:
         cmd += ["-cols", str(width)]
     return call_subproc(data.encode(), cmd).decode()
 
@@ -50,15 +50,15 @@
 )
 def html_to_ansi_elinks(
     data: str,
     width: int | None = None,
     height: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert HTML text to formatted ANSI using :command:`elinks`."""
     cmd: list[Any] = [
         "elinks",
         "-dump",
         "-dump-color-mode",
         "3",
@@ -78,15 +78,15 @@
 )
 def html_to_ansi_lynx(
     data: str,
     width: int | None = None,
     height: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert HTML text to formatted ANSI using :command:`lynx`."""
     cmd: list[Any] = ["lynx", "-dump", "-stdin"]
     if width is not None:
         cmd += [f"-width={width}"]
     return call_subproc(data.encode(), cmd).decode()
 
@@ -98,15 +98,15 @@
 )
 def html_to_ansi_links(
     data: str,
     width: int | None = None,
     height: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert HTML text to formatted ANSI using :command:`links`."""
     cmd: list[Any] = ["links", "-dump"]
     if width is not None:
         cmd += ["-width", width]
     return call_subproc(data.encode(), cmd, use_tempfile=True).decode()
 
@@ -118,15 +118,15 @@
 )
 def html_to_ansi_py_htmlparser(
     data: str,
     width: int | None = None,
     height: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert HTML tables to ANSI text using :py:mod:`HTMLParser`."""
     import io
     import re
     from html.parser import HTMLParser
 
     class HTMLStripper(HTMLParser):
@@ -175,15 +175,15 @@
 )
 def latex_to_ansi_py_flatlatex(
     data: str,
     width: int | None = None,
     height: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert LaTeX to ANSI using :py:mod:`flatlatex`."""
     import flatlatex
 
     return flatlatex.converter().convert(data.strip().strip("$").strip())
 
 
@@ -194,15 +194,15 @@
 )
 def latex_to_ansi_py_pylatexenc(
     data: str,
     width: int | None = None,
     height: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert LaTeX to ANSI using :py:mod:`pylatexenc`."""
     from pylatexenc.latex2text import LatexNodes2Text
 
     return LatexNodes2Text().latex_to_text(data.strip().strip("$").strip())
 
 
@@ -213,15 +213,15 @@
 )
 def latex_to_ansi_py_sympy(
     data: str,
     width: int | None = None,
     height: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert LaTeX to ANSI using :py:mod:`sympy`."""
     from sympy import pretty
     from sympy.parsing.latex import parse_latex
     from sympy.parsing.latex.errors import LaTeXParsingError
 
     from euporie.core.log import stdout_to_log
@@ -237,22 +237,38 @@
 @register(from_="pil", to="ansi", filter_=have_modules("timg"), weight=2)
 def pil_to_ansi_py_timg(
     data: PilImage,
     cols: int | None = None,
     rows: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert a PIL image to ANSI text using :py:mod:`timg`."""
     import timg
 
+    px, py = get_app().term_info.cell_size_px
+
+    # Calculate rows based on image aspect ratio
     w, h = data.size
-    if cols is not None:
-        data = data.resize((cols, ceil(cols / w * h)))
+    if rows is None and cols is not None:
+        w, h = data.size
+        rows = ceil(cols / w * h)
+    elif cols is None and rows is not None:
+        w, h = data.size
+        cols = ceil(rows / h * w)
+    elif rows is None and cols is None:
+        cols = ceil(w / px)
+        rows = ceil(h / py)
+    assert rows is not None and cols is not None
+
+    # `timg` assumes a 2x1 terminal cell aspect ratio, so we correct for while
+    # resizing the image
+    data = data.resize((cols, ceil(rows * 2 * (px / py) / 0.5)))
+
     bg = bg or get_app().color_palette.bg.base_hex
     if bg:
         data = set_background(data, bg)
     data = set_background(data, bg)
     return timg.Ansi24HblockMethod(data).to_string()
 
 
@@ -263,15 +279,15 @@
 )
 def pil_to_ansi_py_img2unicode(
     data: PilImage,
     cols: int | None = None,
     rows: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert a PIL image to ANSI text using :py:mod:`img2unicode`."""
     import io
 
     from img2unicode import FastQuadDualOptimizer, Renderer
 
     output = io.StringIO()
@@ -301,15 +317,15 @@
 )
 def image_to_ansi_timg(
     data: bytes,
     cols: int | None = None,
     rows: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert image data to ANSI text using :command:`timg`."""
     cmd: list[Any] = ["timg"]
     if cols is not None and rows is not None:
         cmd += [f"-g{cols}x{cols}"]
     cmd += ["--compress", "-pq", "--threads=-1", "-"]
     return call_subproc(data, cmd).decode()
@@ -322,15 +338,15 @@
 )
 def image_to_ansi_catimg(
     data: bytes,
     cols: int | None = None,
     rows: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert image data to ANSI text using :command:`catimg`."""
     cmd: list[Any] = ["catimg"]
     if cols is not None and rows is not None:
         cmd += ["-w", cols * 2]
     cmd += ["-"]
     return call_subproc(data, cmd).decode()
@@ -343,15 +359,15 @@
 )
 def image_to_ansi_icat(
     data: bytes,
     cols: int | None = None,
     rows: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert image data to ANSI text using :command:`icat`."""
     cmd: list[Any] = ["icat"]
     if cols is not None and rows is not None:
         cmd += ["-w", cols]
     cmd += ["--mode", "24bit", "-"]
     return call_subproc(data, cmd).decode()
@@ -364,15 +380,15 @@
 )
 def image_to_ansi_tiv(
     data: bytes,
     cols: int | None = None,
     rows: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert image data to ANSI text using :command:`tiv`."""
     cmd: list[Any] = ["tiv"]
     if cols is not None and rows is not None:
         cmd += ["-w", cols, "-h", rows]
     return call_subproc(data, cmd, use_tempfile=True).decode()
 
@@ -384,15 +400,15 @@
 )
 def image_to_ansi_viu(
     data: bytes,
     cols: int | None = None,
     rows: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert image data to ANSI text using :command:`viu`."""
     cmd: list[Any] = ["viu"]
     if cols is not None and rows is not None:
         cmd += ["-w", cols]
     cmd += ["-s", "-"]
     return call_subproc(data, cmd).decode()
@@ -405,15 +421,15 @@
 )
 def image_to_ansi_jp2a(
     data: bytes,
     cols: int | None = None,
     rows: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert image data to ANSI text using :command:`jp2a`."""
     cmd: list[Any] = ["jp2a", "--color"]
     if cols is not None and rows is not None:
         cmd += [f"--height={rows}"]
     cmd += ["-"]
     return call_subproc(data, cmd).decode()
@@ -426,35 +442,40 @@
 )
 def png_to_ansi_img2txt(
     data: bytes,
     cols: int | None = None,
     rows: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert PNG data to ANSI text using :command:`img2txt`."""
     cmd: list[Any] = ["img2txt"]
     if cols is not None and rows is not None:
         cmd += ["-W", cols, "-H", rows]
     return call_subproc(data, cmd, use_tempfile=True).decode()
 
 
 @register(from_=("png", "jpeg", "svg"), to="ansi", filter_=True, weight=99)
 def png_to_ansi_py_placeholder(
     data: bytes,
-    cols: int = 7,
-    rows: int = 3,
+    cols: int | None = None,
+    rows: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Draw placeholder ANSI text."""
     from euporie.core.border import RoundedLine
 
+    if cols is None:
+        cols = 7
+    if rows is None:
+        rows = 3
+
     lines = []
     B = RoundedLine.grid
     lines.append(f"{B.TOP_LEFT}{B.TOP_MID * max(5, (cols - 2))}{B.TOP_RIGHT}")
     lines += [f"{B.MID_LEFT}{B.MID_MID * (cols - 2)}{B.MID_RIGHT}"] * ((rows - 3) // 2)
     lines.append(f"{B.MID_LEFT}{'Image'.center(cols - 2)}{B.MID_RIGHT}")
     lines += [f"{B.MID_LEFT}{B.MID_MID * (cols - 2)}{B.MID_RIGHT}"] * (
         (rows - 3) - (rows - 3) // 2
@@ -470,15 +491,15 @@
 )
 def rich_to_ansi_py(
     data: RenderableType,
     width: int | None = None,
     height: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert rich objects to formatted ANSI text."""
     import rich
 
     console = rich.get_console()
     options = console.options
     if width is not None:
```

### Comparing `euporie-2.3.2/euporie/core/convert/formats/common.py` & `euporie-2.4.0/euporie/core/convert/formats/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,67 +6,70 @@
 import logging
 from typing import TYPE_CHECKING
 
 from euporie.core.convert.utils import call_subproc
 from euporie.core.current import get_app
 
 if TYPE_CHECKING:
+    from pathlib import Path
     from typing import Any, Literal
 
     from PIL.Image import Image as PilImage
-    from upath import UPath
 
 log = logging.getLogger(__name__)
 
 
 def base64_to_bytes_py(
     data: str | bytes,
     width: int | None = None,
     height: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> bytes:
     """Convert base64 encoded data to bytes."""
     data_str = data.decode() if isinstance(data, bytes) else data
     return base64.b64decode(data_str)
 
 
 def imagemagick_convert(
     output_format: str,
     data: str | bytes,
     cols: int | None = None,
     rows: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str | bytes:
     """Convert image data to PNG bytes using ``imagemagick``."""
     cmd: list[Any] = ["convert"]  # , "-density", "300"]
-    if cols is not None:
-        px, _ = get_app().term_info.cell_size_px
+    app = get_app()
+    if cols is not None and hasattr(app, "term_info"):
+        px, _ = app.term_info.cell_size_px
         cmd += ["-geometry", f"{int(cols * px)}"]
-    bg = bg or get_app().color_palette.bg.base_hex
-    if bg is not None:
+    if not bg and hasattr(app, "color_palette"):
+        bg = app.color_palette.bg.base_hex
+    if bg:
         cmd += ["-background", bg]
     cmd += ["-[0]", f"{output_format}:-"]
     result: bytes | str = call_subproc(data, cmd)
+
     if output_format in {"sixel", "svg"} and isinstance(result, bytes):
         result = result.decode()
     return result
 
 
 def chafa_convert_cmd(
     output_format: str,
     data: str | bytes,
     cols: int | None = None,
     rows: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str | bytes:
     """Convert image data to ANSI text using :command:`chafa`."""
     cmd: list[Any] = ["chafa", f"--format={output_format}"]
     if cols is not None or rows is not None:
         cmd += [f"--size={cols or '1'}x{rows or '1'}"]
     if bg:
         cmd += ["--bg", bg]
@@ -77,15 +80,15 @@
 def chafa_convert_py(
     output_format: Literal["symbols", "sixels", "kitty", "iterm2"],
     data: PilImage,
     cols: int | None = None,
     rows: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str | bytes:
     """Convert image data to ANSI text using ::`chafa.py`."""
     from chafa.chafa import Canvas, CanvasConfig, PixelMode, PixelType
 
     pil_mode_to_pixel_type = {
         "RGBa": PixelType.CHAFA_PIXEL_RGBA8_PREMULTIPLIED,
         "RGBA": PixelType.CHAFA_PIXEL_RGBA8_UNASSOCIATED,
@@ -105,20 +108,42 @@
 
         data = data.convert("RGBA", palette=Image.Palette.ADAPTIVE, colors=16)
 
     # Init canvas config
     config = CanvasConfig()
     # Set output mode
     config.pixel_mode = str_to_pixel_mode[output_format]
-    # Set canvas height and width
-    config.height = rows or 20
-    config.width = cols or 80
     # Configure the canvas geometry based on our cell size
-    config.cell_width, config.cell_height = get_app().term_info.cell_size_px
+    if hasattr(app := get_app(), "term_info"):
+        px, py = app.term_info.cell_size_px
+    else:
+        px, py = 10, 20
+    config.cell_width, config.cell_height = px, py
+    # Set canvas height and width
+    if cols:
+        config.width = cols
+        if rows:
+            config.height = max(1, rows)
+        # If we don't have specified, use the image's aspect
+        else:
+            config.height = max(1, int(cols / data.size[0] * data.size[1] * px / py))
+
+    # Set the foreground color
+    if not fg and hasattr(app, "color_palette"):
+        fg = app.color_palette.fg.base_hex
+    if fg and (color := fg.lstrip("#")):
+        config.fg_color = (
+            int(color[0:2], 16),
+            int(color[2:4], 16),
+            int(color[4:6], 16),
+        )
+
     # Set the background color
+    if not bg and hasattr(app, "color_palette"):
+        bg = app.color_palette.bg.base_hex
     if bg and (color := bg.lstrip("#")):
         config.bg_color = (
             int(color[0:2], 16),
             int(color[2:4], 16),
             int(color[4:6], 16),
         )
```

### Comparing `euporie-2.3.2/euporie/core/convert/formats/html.py` & `euporie-2.4.0/euporie/core/convert/formats/html.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 from markdown_it import MarkdownIt
 from mdit_py_plugins.amsmath import amsmath_plugin
 from mdit_py_plugins.dollarmath.index import dollarmath_plugin
 from mdit_py_plugins.texmath.index import texmath_plugin
 from pygments import highlight
 from pygments.formatters import HtmlFormatter
-from pygments.lexers import get_lexer_by_name
 
-from euporie.core.convert.base import register
+from euporie.core.convert.core import register
 from euporie.core.current import get_app
+from euporie.core.lexers import detect_lexer
 
 if TYPE_CHECKING:
-    from upath import UPath
+    from pathlib import Path
 
 log = logging.getLogger(__name__)
 
 
 class MarkdownParser(MarkdownIt):
     """Subclas the markdown parser to allow ``file:`` URIs."""
 
@@ -32,15 +32,15 @@
 
 markdown_parser = (
     (
         MarkdownParser(
             options_update={
                 "highlight": lambda text, language, lang_args: highlight(
                     text,
-                    get_lexer_by_name(language),
+                    detect_lexer(text, language=language),
                     HtmlFormatter(
                         nowrap=True,
                         noclasses=True,
                         style=app.config.syntax_theme
                         if hasattr((app := get_app()), "config")
                         else "default",
                     ),
@@ -61,13 +61,13 @@
 @register(from_="markdown", to="html")
 def markdown_to_html_markdown_it(
     data: str | bytes,
     width: int | None = None,
     height: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert markdown to HTML using :py:mod:`markdownit_py`."""
     assert markdown_parser is not None
     markup = data.decode() if isinstance(data, bytes) else data
     return markdown_parser.render(markup)
```

### Comparing `euporie-2.3.2/euporie/core/convert/formats/markdown.py` & `euporie-2.4.0/euporie/core/convert/formats/markdown.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Contain functions which convert data to markdown format."""
 
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
-from euporie.core.convert.base import register
+from euporie.core.convert.core import register
 from euporie.core.convert.utils import have_modules
 
 if TYPE_CHECKING:
-    from upath import UPath
+    from pathlib import Path
 
 log = logging.getLogger(__name__)
 
 _HTML2TEXT_TABLE_RE = r"(?:(?:.*\|)+[^|]*?(?:\n|$))+"
 
 
 @register(
@@ -23,15 +23,15 @@
 )
 def html_to_markdown_py_html2text(
     data: str | bytes,
     width: int | None = None,
     height: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert HTML to markdown tables using :py:mod:`html2text`."""
     import re
 
     from html2text import HTML2Text
 
     parser = HTML2Text(bodywidth=0)
@@ -69,14 +69,14 @@
 )
 def html_to_markdown_py_mtable(
     data: str | bytes,
     width: int | None = None,
     height: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert HTML tables to markdown tables using :py:mod:`mtable`."""
     from mtable import MarkupTable
 
     markup = data.decode() if isinstance(data, bytes) else data
     return "\n\n".join([table.to_md() for table in MarkupTable.from_html(markup)])
```

### Comparing `euporie-2.3.2/euporie/core/convert/formats/pil.py` & `euporie-2.4.0/euporie/core/convert/formats/pil.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Contain functions which convert data to PIL format."""
 
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
-from euporie.core.convert.base import register
+from euporie.core.convert.core import register
 from euporie.core.convert.utils import have_modules
 
 if TYPE_CHECKING:
+    from pathlib import Path
+
     from PIL.Image import Image as PilImage
-    from upath import UPath
 
 log = logging.getLogger(__name__)
 
 
 def set_background(image: PilImage, bg_color: str | None = None) -> PilImage:
     """Remove the alpha channel from an image and set the background colour."""
     from PIL import Image
@@ -39,21 +40,22 @@
 )
 def png_to_pil_py(
     data: bytes,
     cols: int | None = None,
     rows: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> PilImage:
     """Convert PNG to a pillow image using :py:mod:`PIL`."""
     import io
 
     from PIL import Image
 
     try:
         image = Image.open(io.BytesIO(data))
+        image.load()
     except OSError:
         log.error("Could not load image.")
         return Image.new(mode="P", size=(1, 1))
     else:
         return image
```

### Comparing `euporie-2.3.2/euporie/core/convert/formats/png.py` & `euporie-2.4.0/euporie/core/convert/formats/png.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Contain functions which convert data to png format."""
 
 from __future__ import annotations
 
 from functools import partial
 from typing import TYPE_CHECKING
 
-from euporie.core.convert.base import register
+from euporie.core.convert.core import register
 from euporie.core.convert.formats.common import base64_to_bytes_py, imagemagick_convert
 from euporie.core.convert.utils import commands_exist, have_modules
 
 if TYPE_CHECKING:
+    from pathlib import Path
+
     from PIL.Image import Image as PilImage
-    from upath import UPath
 
 
 register(
     from_="base64-png",
     to="png",
 )(base64_to_bytes_py)
 
@@ -27,15 +28,15 @@
 )
 def latex_to_png_dvipng(
     data: str,
     width: int | None = None,
     height: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> bytes | None:
     """Render LaTeX as a png image using :command:`dvipng`.
 
     Borrowed from IPython.
     """
     import shutil
     import subprocess
@@ -108,15 +109,15 @@
 )
 def latex_to_png_py_mpl(
     data: str,
     width: int | None = None,
     height: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> bytes:
     """Render LaTeX as a png image using :py:module:`matplotlib`.
 
     Borrowed from IPython.
     """
     from io import BytesIO
 
@@ -151,15 +152,15 @@
 )
 def pil_to_png_py_pil(
     data: PilImage,
     cols: int | None = None,
     rows: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> bytes:
     """Convert a pillow image to sixels :py:mod:`teimpy`."""
     import io
 
     with io.BytesIO() as output:
         data.save(output, format="PNG")
         contents = output.getvalue()
@@ -173,14 +174,14 @@
 )
 def svg_to_png_py_cairosvg(
     data: str | bytes,
     width: int | None = None,
     height: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert SVG to PNG using :py:mod:`cairosvg`."""
     import cairosvg
 
     markup = data.decode() if isinstance(data, bytes) else data
     return cairosvg.surface.PNGSurface.convert(markup, write_to=None)
```

### Comparing `euporie-2.3.2/euporie/core/convert/formats/rich.py` & `euporie-2.4.0/euporie/core/convert/formats/rich.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """Contain function which convert data to rich format."""
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from euporie.core.convert.base import register
+from euporie.core.convert.core import register
 from euporie.core.convert.utils import have_modules
 
 if TYPE_CHECKING:
+    from pathlib import Path
+
     from rich.markdown import Markdown
-    from upath import UPath
 
 
 @register(
     from_="markdown",
     to="rich",
     filter_=have_modules("rich"),
 )
 def markdown_to_rich_py(
     data: str | bytes,
     width: int | None = None,
     height: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> Markdown:
     """Convert base64 encoded data to bytes."""
     from rich.markdown import Markdown
 
     markup = data.decode() if isinstance(data, bytes) else data
     return Markdown(
         markup,
```

### Comparing `euporie-2.3.2/euporie/core/convert/formats/sixel.py` & `euporie-2.4.0/euporie/core/convert/formats/sixel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Contain function which convert data to sixel format."""
 
 from __future__ import annotations
 
 from functools import partial
 from typing import TYPE_CHECKING
 
-from euporie.core.convert.base import register
+from euporie.core.convert.core import register
 from euporie.core.convert.formats.common import (
     chafa_convert_cmd,
     chafa_convert_py,
     imagemagick_convert,
 )
 from euporie.core.convert.utils import call_subproc, commands_exist, have_modules
 from euporie.core.current import get_app
 
 if TYPE_CHECKING:
+    from pathlib import Path
     from typing import Any
 
     from PIL.Image import Image as PilImage
-    from upath import UPath
 
 
 register(
     from_=("png", "jpeg", "svg", "pdf"),
     to="sixel",
     filter_=commands_exist("chafa"),
 )(partial(chafa_convert_cmd, "sixel"))
@@ -42,15 +42,15 @@
 )
 def png_to_sixel_img2sixel(
     data: bytes,
     cols: int | None = None,
     rows: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert PNG data to sixels :command:`img2sixel`."""
     bg = bg or get_app().color_palette.bg.base_hex
     cmd: list[Any] = ["img2sixel", "-I"]
     if bg:
         cmd += [f"--bgcolor={bg}"]
     if cols is not None:
@@ -73,15 +73,15 @@
 )
 def pil_to_sixel_py_timg(
     data: PilImage,
     cols: int | None = None,
     rows: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert a pillow image to sixels :py:mod:`timg`."""
     import timg
 
     return timg.SixelMethod(data).to_string()
 
 
@@ -92,14 +92,14 @@
 )
 def pil_to_sixel_py_teimpy(
     data: PilImage,
     cols: int | None = None,
     rows: int | None = None,
     fg: str | None = None,
     bg: str | None = None,
-    path: UPath | None = None,
+    path: Path | None = None,
 ) -> str:
     """Convert a pillow image to sixels :py:mod:`teimpy`."""
     import numpy as np
     import teimpy
 
     return teimpy.get_drawer(teimpy.Mode.SIXEL).draw(np.asarray(data))
```

### Comparing `euporie-2.3.2/euporie/core/formatted_text/ansi.py` & `euporie-2.4.0/euporie/core/formatted_text/ansi.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,33 +13,34 @@
 
 log = logging.getLogger(__name__)
 
 
 class ANSI(PTANSI):
     """Convert ANSI text into formatted text, preserving all control sequences."""
 
-    def __init__(self, value: str, tab_size: int = 4) -> None:
+    def __init__(self, value: str, tab_size: int = 8) -> None:
         """Initiate the ANSI processor instance.
 
         This replaces carriage returns to emulate terminal output.
 
         Args:
             value: The ANSI string to process.
             tab_size: The number of spaces to use to represent a tab
 
         """
-        self.tab_size = tab_size
+        # Replace tabs with spaces
+        value = value.expandtabs(tabsize=tab_size)
         # Replace windows style newlines
         value = value.replace("\r\n", "\n")
         # Remove anything before a carriage return if there is something after it to
         # emulate a carriage return in the output
         value = re.sub(r"^.*\r(?!\n)", "", value, 0, re.MULTILINE)
         # Clear line by deleting previous characters
         value = re.sub(r".*\x1b\[2K", "", value, 0)
-        # Ignore cursor hide / show request
+        # Remove hide & show cursor commands
         value = re.sub(r"\x1b\[\?25[hl]", "", value, 0)
 
         super().__init__(value)
 
     def _parse_corot(self) -> Generator[None, str, None]:
         """Coroutine that parses the ANSI escape sequences.
 
@@ -71,19 +72,14 @@
 
             # Check for backspace
             elif char == "\x08":
                 # TODO - remove last character from last non-ZeroWidthEscape fragment
                 formatted_text.pop()
                 continue
 
-            # Check for tabs
-            elif char == "\t":
-                formatted_text.append(("", " " * self.tab_size))
-                continue
-
             elif char in ("\x1b", "\x9b"):
                 # Got a CSI sequence, try to compile a control sequence
                 char = yield
 
                 # Check for sixels
                 if char == "P":
                     # Got as DEC code
```

### Comparing `euporie-2.3.2/euporie/core/formatted_text/html.py` & `euporie-2.4.0/euporie/core/formatted_text/html.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,23 +3,28 @@
 from __future__ import annotations
 
 import logging
 import re
 from ast import literal_eval
 from bisect import bisect_right
 from collections.abc import Mapping
-from functools import cached_property, lru_cache
+from functools import cached_property, lru_cache, partial
 from html.parser import HTMLParser
 from itertools import zip_longest
 from math import ceil
-from typing import TYPE_CHECKING, NamedTuple
+from operator import eq, ge, gt, le, lt
+from typing import TYPE_CHECKING, NamedTuple, cast
+from urllib.parse import urljoin
 
 from flatlatex.data import subscript, superscript
 from prompt_toolkit.application.current import get_app_session
-from prompt_toolkit.cache import SimpleCache
+from prompt_toolkit.data_structures import Size
+from prompt_toolkit.filters.base import Condition
+from prompt_toolkit.filters.utils import _always as always
+from prompt_toolkit.filters.utils import _never as never
 from prompt_toolkit.formatted_text.base import StyleAndTextTuples
 from prompt_toolkit.formatted_text.utils import split_lines
 from prompt_toolkit.layout.dimension import Dimension
 from upath import UPath
 
 from euporie.core.border import (
     DiLineStyle,
@@ -38,15 +43,15 @@
     ThinDoubleDashedLine,
     ThinLine,
     ThinQuadrupleDashedLine,
     UpperRightEighthLine,
     UpperRightHalfDottedLine,
     UpperRightHalfLine,
 )
-from euporie.core.convert.base import convert, get_format
+from euporie.core.convert.core import convert, get_format
 from euporie.core.convert.utils import data_pixel_size, pixels_to_cell_size
 from euporie.core.current import get_app
 from euporie.core.data_structures import DiBool, DiInt, DiStr
 from euporie.core.formatted_text.table import Table, compute_padding
 from euporie.core.formatted_text.utils import (
     FormattedTextAlign,
     add_border,
@@ -58,18 +63,16 @@
     fragment_list_width,
     join_lines,
     last_char,
     max_line_width,
     pad,
     paste,
     strip,
-    strip_one_trailing_newline,
     truncate,
 )
-from euporie.core.url import load_url
 
 
 class CssSelector(NamedTuple):
     """A named tuple to hold CSS selector data."""
 
     comb: str | None = None
     item: str | None = None
@@ -82,23 +85,24 @@
         attrs = ", ".join(
             f"{k}={v!r}" for k, v in self._asdict().items() if v != defaults[k]
         )
         return f"{self.__class__.__name__}({attrs})"
 
 
 if TYPE_CHECKING:
-    from typing import (
-        Any,
-        Callable,
-        Generator,
-        Hashable,
-        Iterator,
-    )
+    from pathlib import Path
+    from typing import Any, Callable, Generator, Iterator
 
-    CssSelectors = dict[tuple[tuple[CssSelector, ...], ...], dict[str, str]]
+    from prompt_toolkit.filters.base import Filter
+    from prompt_toolkit.key_binding.key_bindings import NotImplementedOrNone
+    from prompt_toolkit.mouse_events import MouseEvent
+
+    CssSelectors = dict[
+        Filter, dict[tuple[tuple[CssSelector, ...], ...], dict[str, str]]
+    ]
 
 log = logging.getLogger(__name__)
 
 
 class Direction(NamedTuple):
     """A description of a direction."""
 
@@ -115,14 +119,46 @@
         (?P<item>(?:::)?[^\s>+~:[\]]+)?
         (?P<attr>\[[^\s>+~:]+\])?
         (?P<pseudo>\:[^:][^\s>+~]*)?
     """,
     re.VERBOSE,
 )
 
+_AT_RULE_RE = re.compile(
+    r"""
+    (
+        @(?:color-profile|container|counter-style|document|font-face|font-feature-values|font-palette-values|keyframes|layer|media|page|supports)
+        [^@{]+
+        (?:
+            {[^{}]*}
+            |
+            {(?:[^{]+?{(?:[^{}]|{[^}]+?})+?}\s*)*?}
+        )
+        |
+        @(?:charset|import|namespace)[^;]*;
+    )
+    """,
+    re.VERBOSE,
+)
+
+_NESTED_AT_RULE_RE = re.compile(
+    r"@(?P<identifier>[\w-]+)\s+(?P<rule>[^{]*?)\s*{\s*(?P<part>.*)\s*}"
+)
+
+_MEDIA_QUERY_TARGET_RE = re.compile(
+    r"""
+        (?:
+            (?P<invert>not\s+)?
+            (?:only\s+)?  # Ignore this
+            (?P<type>all|print|screen) |
+            (?:\((?P<feature>[^)]+)\))
+        )
+    """,
+    re.VERBOSE,
+)
 
 # List of elements which might not have a close tag
 _VOID_ELEMENTS = (
     "area",
     "base",
     "br",
     "col",
@@ -326,14 +362,18 @@
                 rule = pseudo[:end]
                 pseudo = pseudo[end + 1 :]
                 matched = sibling_element_index is not None and (
                     (rule == "odd" and sibling_element_index % 2 == 1)
                     or (rule == "even" and sibling_element_index % 2 == 0)
                 )
                 continue
+        if pseudo.startswith(":link"):
+            pseudo = pseudo[5:]
+            matched = bool(element_attrs.get("href"))
+            continue
         return False
 
     if not matched:
         return False
 
     while selector and matched:
         # Universal selector
@@ -439,15 +479,15 @@
         return f"#{hexes}"
     elif value.startswith("rgb"):
         # Ignore alpha for now - TODO
         color_values = value.strip("rgba()").split(",")[:3]
         hexes = []
         for color_value in color_values:
             if (int_value := get_integer(color_value)) is not None:
-                hexes.append(hex(int_value)[2:])
+                hexes.append(f"{hex(int_value)[2:]:02}")
             else:
                 return ""
         return "#" + "".join(hexes)
     else:
         from euporie.core.reference import KNOWN_COLORS
 
         if value == "transparent" or value in KNOWN_COLORS:
@@ -500,15 +540,15 @@
     units = units[::-1]
 
     # Calculate size based on units
 
     # TODO - process view-width units
     # https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Values_and_units
 
-    if units == "%":
+    if units in {"%", "vh", "vw"}:
         assert available is not None
         return number / 100 * available
 
     # Get cell pixel dimensions
     app = get_app()
     if hasattr(app, "term_info"):
         cell_px, cell_py = get_app().term_info.cell_size_px
@@ -537,15 +577,15 @@
     theme: dict[str, str] = {}
 
     if not content:
         return theme
 
     for declaration in content.split(";"):
         name, _, value = declaration.partition(":")
-        name = name.strip()
+        name = name.strip().lower()
 
         # Ignore "!important" tags for now - TODO
         value = value.replace("!important", "").strip()
 
         # Helpers
 
         def _split_quad(value: str) -> tuple[str, str, str, str]:
@@ -557,14 +597,16 @@
                 left = right = values[1]
             elif len(values) == 3:
                 top = values[0]
                 right = left = values[1]
                 bottom = values[2]
             elif len(values) >= 4:
                 top, right, bottom, left, *_ = values
+            else:
+                top = right = bottom = left = ""
             return top, right, bottom, left
 
         # Compute values
 
         if name == "background":
             # TODO - needs work
             for part in value.split():
@@ -655,14 +697,23 @@
         elif name == "list-style":
             for each_value in value.split():
                 if each_value in {"inside", "outside"}:
                     theme["list_style_position"] = each_value
                 elif each_value in _LIST_STYLE_TYPES:
                     theme["list_style_type"] = each_value
 
+        elif name == "flex-flow":
+            values = set(value.split(" "))
+            directions = {"row", "row-reverse", "column", "column-reverse"}
+            wraps = {"nowrap", "wrap", "wrap-reverse"}
+            for value in values.intersection(directions):
+                theme["flex_direction"] = value
+            for value in values.intersection(wraps):
+                theme["flex_wrap"] = value
+
         else:
             name = name.replace("-", "_")
             theme[name] = value
 
     return theme
 
 
@@ -719,20 +770,23 @@
     "border_left_style": "none",
     "border_bottom_style": "none",
     "border_right_style": "none",
     "border_top_color": "",
     "border_left_color": "",
     "border_bottom_color": "",
     "border_right_color": "",
+    # Flex
+    "flex_direction": "row",
+    "align_content": "normal",
     # Position
     "position": "static",
-    "top": "0",
-    "right": "0",
-    "bottom": "0",
-    "left": "0",
+    "top": "unset",
+    "right": "unset",
+    "bottom": "unset",
+    "left": "unset",
     "z_index": "0",
     # Lists
     "list_style_type": "none",
     "list_style_position": "inside",
 }
 
 
@@ -767,54 +821,85 @@
 
     def update_space(
         self,
         available_width: int,
         available_height: int,
     ) -> None:
         """Set the space available to the element for rendering."""
-        self.available_width = available_width
-        self.available_height = available_height
+        if self.theme["position"] == "fixed":
+            # Space is given by position
+            position = self.position
+            dom = self.element.dom
+            assert dom.width is not None and dom.height is not None
+            self.available_width = (dom.width - position.right) - position.left
+            self.available_height = (dom.height - position.bottom) - position.top
+
+        # elif parent_theme := self.parent_theme:
+        #     self.available_width = parent_theme.content_width
+        #     self.available_height = parent_theme.content_height
+
+        else:
+            self.available_width = available_width
+            self.available_height = available_height
 
     # Theme calculation methods
 
     @cached_property
     def inherited_browser_css_theme(self) -> dict[str, str]:
         """Get the inherited parts from the browser CSS."""
         if (parent_theme := self.parent_theme) is not None:
             return {
                 k: v
                 for k, v in {
                     **parent_theme.inherited_browser_css_theme,
                     **parent_theme.browser_css_theme,
                 }.items()
-                if k in _HERITABLE_PROPS
+                if k in _HERITABLE_PROPS or k.startswith("__")
             }
 
         else:
             return {}
 
     @cached_property
     def inherited_theme(self) -> dict[str, str]:
         """Calculate the theme inherited from the element's parent."""
+        theme: dict[str, str] = {}
+        parent = self.element.parent
+
+        # Text elements inherit from direct inline parents
+        if self.element.name == "text" and parent is not None:
+            inline_parent_themes = []
+            while parent.theme.d_inline:
+                inline_parent_themes.append(parent.theme.theme)
+                parent = parent.parent
+                if parent is None:
+                    break
+            for inherited_theme in inline_parent_themes:
+                theme.update(inherited_theme)
+
+        # Inherit heritable properties from the parent element's theme
+        # unless the default value is unset
         if (parent_theme := self.parent_theme) is not None:
             browser_css = self.browser_css_theme
-            return {
-                k: v
-                for part in (
-                    parent_theme.inherited_theme,
-                    parent_theme.dom_css_theme,
-                    parent_theme.attributes_theme,
-                    parent_theme.style_attribute_theme,
-                )
-                for k, v in part.items()
-                if k in _HERITABLE_PROPS and browser_css.get(k) != "unset"
-            }
+            theme.update(
+                {
+                    k: v
+                    for part in (
+                        parent_theme.inherited_theme,
+                        parent_theme.dom_css_theme,
+                        parent_theme.attributes_theme,
+                        parent_theme.style_attribute_theme,
+                    )
+                    for k, v in part.items()
+                    if (k in _HERITABLE_PROPS or k.startswith("__"))
+                    and browser_css.get(k) != "unset"
+                }
+            )
 
-        else:
-            return {}
+        return theme
 
     @cached_property
     def style_attribute_theme(self) -> dict[str, str]:
         """Calculate the theme defined by the element's style attribute."""
         return parse_css_content(self.element.attrs.get("style", ""))
 
     @cached_property
@@ -851,78 +936,84 @@
         # cellpadding # TODO
         return theme
 
     def _css_theme(self, css: CssSelectors) -> dict[str, str]:
         """Calculate the theme defined in CSS."""
         specificity_rules = []
         element = self.element
-        for selectors, rule in css.items():
-            for selector_parts in selectors:
-                # Last selector item should match the current element
-                selector = selector_parts[-1]
-                if not match_css_selector(
-                    selector.item or "",
-                    selector.attr or "",
-                    selector.pseudo or "",
-                    element.name,
-                    element.is_first_child_element,
-                    element.is_last_child_element,
-                    element.sibling_element_index,
-                    **element.attrs,
-                ):
-                    continue
-
-                # All of the parent selectors should match a separate parent in order
-                # TODO - combinators
-                # https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors#combinators
-                unmatched_parents: list[Node] = [x for x in element.parents[::-1] if x]
-
-                _unmatched_parents: list[Node]
-                parent = element.parent
-                if parent and (
-                    (selector.comb == ">" and parent)
-                    # Pseudo-element selectors only match direct ancestors
-                    or ((item := selector.item) and item.startswith("::"))
-                ):
-                    _unmatched_parents = [parent]
-                else:
-                    _unmatched_parents = unmatched_parents
-
-                # TODO investigate caching element / selector chains so we don't have to
-                # iterate through every parent every time
-
-                # Iterate through selector items in reverse, skipping the last
-                for selector in selector_parts[-2::-1]:
-                    for i, parent in enumerate(_unmatched_parents):
-                        if parent and match_css_selector(
+        for condition, css_block in css.items():
+            if condition():
+                for selectors, rule in css_block.items():
+                    for selector_parts in selectors:
+                        # Last selector item should match the current element
+                        selector = selector_parts[-1]
+                        if not match_css_selector(
                             selector.item or "",
                             selector.attr or "",
                             selector.pseudo or "",
-                            parent.name,
-                            parent.is_first_child_element,
-                            parent.is_last_child_element,
-                            parent.sibling_element_index,
-                            **parent.attrs,
+                            element.name,
+                            element.is_first_child_element,
+                            element.is_last_child_element,
+                            element.sibling_element_index,
+                            **element.attrs,
                         ):
-                            if selector.comb == ">" and (parent := parent.parent):
-                                _unmatched_parents = [parent]
+                            continue
+
+                        # All of the parent selectors should match a separate parent in order
+                        # TODO - combinators
+                        # https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors#combinators
+                        unmatched_parents: list[Node] = [
+                            x for x in element.parents[::-1] if x
+                        ]
+
+                        _unmatched_parents: list[Node]
+                        parent = element.parent
+                        if parent and (
+                            (selector.comb == ">" and parent)
+                            # Pseudo-element selectors only match direct ancestors
+                            or ((item := selector.item) and item.startswith("::"))
+                        ):
+                            _unmatched_parents = [parent]
+                        else:
+                            _unmatched_parents = unmatched_parents
+
+                        # TODO investigate caching element / selector chains so we don't have to
+                        # iterate through every parent every time
+
+                        # Iterate through selector items in reverse, skipping the last
+                        for selector in selector_parts[-2::-1]:
+                            for i, parent in enumerate(_unmatched_parents):
+                                if parent and match_css_selector(
+                                    selector.item or "",
+                                    selector.attr or "",
+                                    selector.pseudo or "",
+                                    parent.name,
+                                    parent.is_first_child_element,
+                                    parent.is_last_child_element,
+                                    parent.sibling_element_index,
+                                    **parent.attrs,
+                                ):
+                                    if selector.comb == ">" and (
+                                        parent := parent.parent
+                                    ):
+                                        _unmatched_parents = [parent]
+                                    else:
+                                        _unmatched_parents = unmatched_parents[i + 1 :]
+                                    break
                             else:
-                                _unmatched_parents = unmatched_parents[i + 1 :]
-                            break
-                    else:
-                        break
+                                break
 
-                else:
-                    # Calculate selector specificity score
-                    specificity_rules.append(
-                        (selector_specificity(selector_parts), rule)
-                    )
-                    # We have already matched this rule, we don't need to keep checking
-                    # the rest of the selectors for this rule
-                    break
+                        else:
+                            # Calculate selector specificity score
+                            specificity_rules.append(
+                                (selector_specificity(selector_parts), rule)
+                            )
+                            # We have already matched this rule, we don't need to keep checking
+                            # the rest of the selectors for this rule
+                            break
 
         return {
             k: v
             for specificity_rule in sorted(specificity_rules, key=lambda x: x[0])
             for k, v in specificity_rule[1].items()
         }
 
@@ -937,40 +1028,87 @@
         return self._css_theme(css=self.element.dom.css)
 
     # Computed properties
 
     @cached_property
     def d_block(self) -> bool:
         """If the element a block element."""
-        return self.theme["display"] == "block" and self.theme["float"] == "none"
+        theme = self.theme
+        parent_theme = self.parent_theme
+        return theme["display"] in {"block", "flex"} and (
+            parent_theme is None
+            or (self.floated is None and not parent_theme.d_flex)
+            or (
+                parent_theme.d_flex and parent_theme["flex_direction"].startswith("col")
+            )
+        )
 
     @cached_property
     def d_inline(self) -> bool:
         """If the element an inline element."""
-        return self.theme["display"] == "inline" and self.theme["float"] == "none"
+        return self.theme["display"] == "inline" and self.floated is None
 
     @cached_property
     def d_inline_block(self) -> bool:
         """If the element an inline element."""
-        return self.theme["display"] == "inline-block" or self.theme["float"] != "none"
+        theme = self.theme
+        parent_theme = self.parent_theme
+        return (
+            # Is an actual inline block
+            theme["display"] == "inline-block"
+            # Is floated
+            or self.floated is not None
+            # If flexed in the row direction
+            or (
+                parent_theme is not None
+                and parent_theme.d_flex
+                and parent_theme["flex_direction"].startswith("row")
+            )
+        )
+
+    @cached_property
+    def d_flex(self) -> bool:
+        """If the element a block element."""
+        return self.theme["display"] == "flex"
+
+    @cached_property
+    def d_image(self) -> bool:
+        """If the element is an image."""
+        return self.element.name in {"img", "svg"}
 
     @cached_property
     def d_table(self) -> bool:
         """If the element a block element."""
         return self.theme["display"] == "table"
 
     @cached_property
+    def d_table_cell(self) -> bool:
+        """If the element a block element."""
+        return self.theme["display"] == "table-cell"
+
+    @cached_property
     def d_list_item(self) -> bool:
         """If the element an inline element."""
-        return self.theme["display"] == "list-item" and self.theme["float"] == "none"
+        return self.theme["display"] == "list-item" and self.floated is None
 
     @cached_property
     def d_blocky(self) -> bool:
         """If the element an inline element."""
-        return self.d_block or self.d_table or self.d_list_item
+        return self.d_block or self.d_table or self.d_table_cell or self.d_list_item
+
+    @cached_property
+    def floated(self) -> str | None:
+        """The float status of the element."""
+        value = self.theme["float"]
+        # Float property does not apply to flex-level boxes
+        if value == "none" or (
+            (parent_theme := self.parent_theme) and parent_theme.d_flex
+        ):
+            return None
+        return value
 
     @property
     def min_width(self) -> int | None:
         """The minimum permitted width."""
         if value := self.get("min_width"):
             theme_width = css_dimension(
                 value, vertical=False, available=self.available_width
@@ -978,89 +1116,202 @@
             if theme_width is not None:
                 return int(theme_width)
         return None
 
     @property
     def width(self) -> int | None:
         """The pescribed width."""
-        if value := self.theme.get("width"):
-            theme_width = css_dimension(
-                value, vertical=False, available=self.available_width
-            )
+        value = self.theme.get("width")
+
+        theme_width: int | float | None
+        if value:
+            if value == "min-content":
+                theme_width = self.min_content_width
+            elif value == "max-content":
+                theme_width = self.max_content_width
+            else:
+                theme_width = css_dimension(
+                    value, vertical=False, available=self.available_width
+                )
             if theme_width is not None:
-                return int(theme_width)
+                return min(int(theme_width), self.available_width)
 
-        else:
-            element = self.element
+        elif (element := self.element).name == "input":
             attrs = element.attrs
-            if element.name == "input" and attrs.get("type") in {
+            if attrs.get("type") in {
                 "text",
                 "password",
                 "email",
                 "number",
                 "search",
                 "tel",
                 "url",
             }:
                 return try_eval(size) if (size := attrs.get("size")) else 20
 
+        elif element.name == "text":
+            return len(element.text)
+
         return None
 
     @property
     def max_width(self) -> int | None:
         """The maximum permitted width."""
         if value := self.get("max_width"):
             theme_width = css_dimension(
                 value, vertical=False, available=self.available_width
             )
             if theme_width is not None:
                 return int(theme_width)
         return None
 
-    @property
-    def height(self) -> int:
-        """The perscribed height."""
-        # TODO - process min-/max-height
-        if value := self.get("height"):
-            theme_height = css_dimension(
-                value, vertical=True, available=self.available_height
+    @cached_property
+    def min_content_width(self) -> int:
+        """Get maximum absolute child width."""
+        if self.element.name == "text":
+            return max([len(x) for x in self.element.text.split()] or [0])
+        else:
+            return max(
+                [
+                    child.theme.min_content_width
+                    for child in self.element.renderable_contents
+                ]
+                or [0]
+            )
+
+    @cached_property
+    def max_content_width(self) -> int:
+        """Get maximum absolute child width."""
+        if self.element.name == "text":
+            return max([len(x) for x in self.element.text.split("\n")] or [0])
+        else:
+            return sum(
+                [
+                    child.theme.max_content_width
+                    for child in self.element.renderable_contents
+                ]
+                or [0]
             )
-            if theme_height is not None:
-                return int(theme_height)
-        assert self.available_height is not None
-        return self.available_height
 
     @property
     def content_width(self) -> int:
         """Return the width available for rendering the element's content."""
         value = self.width
-        # Set content width to the available width for blocks
+
+        border_box = self.theme.get("box_sizing") == "border-box"
+
+        # Use max-content-width as default for inline-blocks
+        if value is None and self.d_inline_block and not self.d_image:
+            value = self.max_content_width
+            # Do not use border-box for inline-blocks if no width is given
+            border_box = False
+
+        # If we do not have a value, use the available space
         if value is None:
-            value = (self.available_width or 0) - self.margin.left - self.margin.right
+            margin = self.margin
+            value = (self.available_width or 0) - margin.left - margin.right
+
+            # Blocks without a set with are rendered with border-box box-sizing
+            if self.d_blocky or self.d_inline_block:
+                border_box = True
+
+        # Ignore box-sizing for table cells, as they include padding and borders
+        if self.d_table_cell:
+            border_box = False
+
+        # Remove padding and borders from available space if we are using box-sizing
+        if border_box:
+            padding = self.padding
+            border_visibility = self.border_visibility
+            value -= padding.left + padding.right
+            value -= border_visibility.left + border_visibility.right
+
         # Apply min / max width constraints
         if (max_width := self.max_width) is not None and max_width < value:
             value = max_width
         elif (min_width := self.min_width) is not None and min_width > value:
             value = min_width
-        # Remove padding and borders from content width for blocks
-        if value and (self.d_blocky or self.d_inline_block):
-            value -= self.padding.left + self.padding.right
-            value -= self.border_visibility.left + self.border_visibility.right
 
         return max(0, value)
 
     @property
+    def min_height(self) -> int | None:
+        """The minimum permitted height."""
+        if value := self.get("min_height"):
+            theme_height = css_dimension(
+                value, vertical=True, available=self.available_height
+            )
+            if theme_height is not None:
+                return int(theme_height)
+        return None
+
+    @property
+    def height(self) -> int | None:
+        """The perscribed height."""
+        # TODO - process min-/max-height
+        if value := self.get("height"):
+            theme_height = css_dimension(
+                value, vertical=True, available=self.available_height
+            )
+            if theme_height is not None:
+                return int(theme_height)
+        return None
+
+    @property
+    def max_height(self) -> int | None:
+        """The maximum permitted height."""
+        if value := self.get("max_height"):
+            theme_height = css_dimension(
+                value, vertical=True, available=self.available_height
+            )
+            if theme_height is not None:
+                return int(theme_height)
+        return None
+
+    @property
     def content_height(self) -> int:
         """Return the height available for rendering the element's content."""
         value = self.height
-        if value and self.d_blocky:
-            value -= self.padding.top + self.padding.bottom
-            value -= self.border_visibility.top + self.border_visibility.bottom
-            value -= self.margin.top + self.margin.bottom
-        return max(value, 0)
+
+        border_box = self.theme.get("box_sizing") == "border-box"
+
+        # Use max-content-height as default for inline-blocks
+        # if value is None and self.d_inline_block and not self.d_image:
+        #     value = self.max_content_height
+        #     # Do not use border-box for inline-blocks if no height is given
+        #     border_box = False
+
+        # If we do not have a value, use the available space
+        if value is None:
+            margin = self.margin
+            value = (self.available_height or 0) - margin.top - margin.bottom
+
+            # Blocks without a set with are rendered with border-box box-sizing
+            # (but not rendered tables as they include padding and borders)
+            if self.d_blocky or self.d_inline_block:
+                border_box = True
+
+        # Ignore box-sizing for table cells, as they include padding and borders
+        if self.d_table_cell:
+            border_box = False
+
+        # Remove padding and borders from available space if we are using box-sizing
+        if border_box:
+            padding = self.padding
+            border_visibility = self.border_visibility
+            value -= padding.top + padding.bottom
+            value -= border_visibility.top + border_visibility.bottom
+
+        # Apply min / max height constraints
+        if (max_height := self.max_height) is not None and max_height < value:
+            value = max_height
+        elif (min_height := self.min_height) is not None and min_height > value:
+            value = min_height
+
+        return max(0, value)
 
     @cached_property
     def padding(self) -> DiInt:
         """Calculate the padding box."""
         output = {}
         a_w = self.available_width
         for direction, vertical in (
@@ -1140,27 +1391,29 @@
                     and not parent_border_visibility.bottom
                 ):
                     values["bottom"] = 0
 
             # Replace the margin on the parent
             if (
                 (first_child := element.first_child_element)
+                and first_child.prev_node_in_flow is None
                 and not self.border_visibility.top
                 and not self.padding.top
             ):
                 child_theme = first_child.theme
                 if child_theme.d_blocky:
                     # TODO - check this
                     if child_theme.available_width is None:
                         child_theme.update_space(
                             self.available_width, self.available_height
                         )
                     values["top"] = max(child_theme.base_margin.top, values["top"])
             if (
                 (last_child := element.last_child_element)
+                and last_child.next_node_in_flow is None
                 and not self.padding.bottom
                 and not self.border_visibility.bottom
             ):
                 child_theme = last_child.theme
                 if child_theme.d_blocky:
                     # TODO - check this
                     if child_theme.available_width is None:
@@ -1179,17 +1432,26 @@
         if self.d_inline:
             values["top"] = 0
             values["bottom"] = 0
 
         return DiInt(**values)
 
     @cached_property
-    def margin_auto(self) -> bool:
+    def block_align(self) -> FormattedTextAlign:
         """Determine if the left and right margins are set to auto."""
-        return self.theme["margin_left"] == self.theme["margin_right"] == "auto"
+        # Temporarily use "justify_self" until flex / grid are implemented (TODO)
+        if (self.theme["margin_left"] == self.theme["margin_right"] == "auto") or (
+            self.d_inline_block and self.theme.get("justify_self") == "center"
+        ):
+            return FormattedTextAlign.CENTER
+        elif (self.theme["margin_left"] == "auto") or (
+            self.d_inline_block and self.theme.get("justify_self") == "right"
+        ):
+            return FormattedTextAlign.RIGHT
+        return FormattedTextAlign.LEFT
 
     @cached_property
     def border_style(self) -> DiStr:
         """Calculate the visibility of the element's borders."""
         if parent_theme := self.parent_theme:
             parent_style = parent_theme.style
         else:
@@ -1204,19 +1466,19 @@
 
             color_str = get_color(self.theme[f"border_{direction}_color"])
             if color_str == "transparent" and parent_theme:
                 style += f" fg:{parent_theme.background_color}"
             elif border_color := get_color(color_str):
                 style += f" fg:{border_color}"
 
-            if getattr(self.border_line, direction) in {
-                UpperRightEighthLine,
-                LowerLeftEighthLine,
-            }:
-                style += f" bg:{self.background_color}"
+            # if getattr(self.border_line, direction) in {
+            #     UpperRightEighthLine,
+            #     LowerLeftEighthLine,
+            # }:
+            style += f" bg:{self.background_color}"
 
             output[direction] = style
 
         return DiStr(**output)
 
     @cached_property
     def border_visibility(self) -> DiBool:
@@ -1239,15 +1501,14 @@
 
         return DiBool(**output)
 
     @cached_property
     def border_line(self) -> DiLineStyle:
         """Calculate the line style."""
         a_w = self.available_width
-        self.d_inline
         output = {}
         for direction in ("top", "right", "bottom", "left"):
             border_width = self.theme[f"border_{direction}_width"]
             size = (
                 _BORDER_WIDTHS.get(
                     border_width,
                     css_dimension(border_width, vertical=False, available=a_w),
@@ -1290,31 +1551,44 @@
         return self.theme.get("border_collapse") == "collapse"
 
     @cached_property
     def color(self) -> str:
         """Get the computed theme foreground color."""
         # TODO - transparency
         color_str = self.theme["color"]
-        if color_str == "transparent":
+        # Use black as the default color if a bg color is set
+        if color_str.startswith("var("):
+            var = color_str[4:-1].replace("-", "_")
+            color_str = self.theme.get(var, color_str)
+        if color_str == "default" and self.theme["background_color"] != "default":
+            color_str = "#000000"
+        elif color_str == "transparent":
             return self.background_color
         if fg := get_color(color_str):
             return fg
         elif self.parent_theme:
             return self.parent_theme.color
         else:
             return ""
 
     @cached_property
     def background_color(self) -> str:
         """Get the computed theme background color."""
         # TODO - transparency
         color_str = self.theme["background_color"]
+        # Use white as the default bg color if a fg color is set
+        # if color_str == "default" and self.theme["color"] != "default":
+        # color_str = "#ffffff"
+        if color_str.startswith("var("):
+            var = color_str[4:-1].replace("-", "_")
+            color_str = self.theme.get(var, color_str)
         if color_str == "transparent":
             if parent_theme := self.parent_theme:
                 return parent_theme.background_color
+            color_str = ""
         if bg := get_color(color_str):
             return bg
         elif self.parent_theme:
             return self.parent_theme.background_color
         else:
             return ""
 
@@ -1377,14 +1651,27 @@
     def text_align(self) -> FormattedTextAlign:
         """The text alignment direction."""
         return _TEXT_ALIGNS.get(self.theme["text_align"], FormattedTextAlign.LEFT)
 
     @cached_property
     def vertical_align(self) -> float:
         """The vertical alignment direction."""
+        if (parent_theme := self.parent_theme) and parent_theme.d_flex:
+            if self.theme.get("align_content") in {
+                "normal",
+                "flex-start",
+                "start",
+                "baseline",
+            }:
+                return 0
+            elif self.theme.get("align_content") == "center":
+                return 0.5
+            else:
+                return 1
+
         return _VERTICAL_ALIGNS.get(self.theme["vertical_align"], 1)
 
     @cached_property
     def list_style_type(self) -> str:
         """The bullet character to use for the list."""
         return _LIST_STYLE_TYPES.get(
             self.theme["list_style_type"], self.theme["list_style_type"]
@@ -1414,50 +1701,61 @@
         """The z-index of the element."""
         return get_integer(self.theme["z_index"]) or 0
 
     @cached_property
     def position(self) -> DiInt:
         """The position of an element with a relative, absolute or fixed position."""
         # TODO - calculate position based on top, left, bottom,right, width, height
+        soup_theme = self.element.dom.soup.theme
         return DiInt(
             top=int(
                 css_dimension(
                     self.theme["top"],
                     vertical=True,
-                    available=self.element.dom.soup.theme.available_height,
+                    available=soup_theme.available_height,
                 )
                 or 0
             ),
             right=int(
                 css_dimension(
                     self.theme["right"],
                     vertical=False,
-                    available=self.element.dom.soup.theme.available_width,
+                    available=soup_theme.available_width,
                 )
                 or 0
             ),
             bottom=int(
                 css_dimension(
                     self.theme["bottom"],
                     vertical=True,
-                    available=self.element.dom.soup.theme.available_height,
+                    available=soup_theme.available_height,
                 )
                 or 0
             ),
             left=int(
                 css_dimension(
                     self.theme["left"],
                     vertical=False,
-                    available=self.element.dom.soup.theme.available_width,
+                    available=soup_theme.available_width,
                 )
                 or 0
             ),
         )
 
     @cached_property
+    def anchors(self) -> DiBool:
+        """Which position directions are set."""
+        return DiBool(
+            top=self.theme["top"] not in {"unset"},
+            right=self.theme["right"] not in {"unset"},
+            bottom=self.theme["bottom"] not in {"unset"},
+            left=self.theme["left"] not in {"unset"},
+        )
+
+    @cached_property
     def skip(self) -> bool:
         """Determine if the element should not be displayed."""
         return (
             "none" in self.theme["display"]
             or (
                 (element := self.element).name == "text"
                 and not self.preformatted
@@ -1477,15 +1775,15 @@
         )
 
     @cached_property
     def in_flow(self) -> bool:
         """Determine if the element is "in-flow"."""
         return (
             not self.skip
-            and self.theme["float"] == "none"
+            and self.floated is None
             and self.theme["position"] not in {"absolute", "fixed"}
             and self.element.name != "html"
         )
 
     # Mapping methods - these are passed on to the unerlying theme dictionary
 
     def __getitem__(self, key: str) -> Any:
@@ -1497,426 +1795,506 @@
         return self.theme.__iter__()
 
     def __len__(self) -> int:
         """Get the length of the mapping."""
         return self.theme.__len__()
 
 
-_BROWSER_CSS = {
-    # Non-rendered elements
-    (
-        (CssSelector(item="head"),),
-        (CssSelector(item="base"),),
-        (CssSelector(item="command"),),
-        (CssSelector(item="link"),),
-        (CssSelector(item="meta"),),
-        (CssSelector(item="noscript"),),
-        (CssSelector(item="script"),),
-        (CssSelector(item="style"),),
-        (CssSelector(item="title"),),
-        (CssSelector(item="option"),),
-        (CssSelector(item="input", attr="[type=hidden]"),),
-    ): {"display": "none"},
-    # Inline elements
-    (
-        (CssSelector(item="::before"),),
-        (CssSelector(item="::after"),),
-        (CssSelector(item="text"),),
-        (CssSelector(item="abbr"),),
-        (CssSelector(item="acronym"),),
-        (CssSelector(item="audio"),),
-        (CssSelector(item="bdi"),),
-        (CssSelector(item="bdo"),),
-        (CssSelector(item="big"),),
-        (CssSelector(item="br"),),
-        (CssSelector(item="canvas"),),
-        (CssSelector(item="data"),),
-        (CssSelector(item="datalist"),),
-        (CssSelector(item="embed"),),
-        (CssSelector(item="iframe"),),
-        (CssSelector(item="label"),),
-        (CssSelector(item="map"),),
-        (CssSelector(item="meter"),),
-        (CssSelector(item="object"),),
-        (CssSelector(item="output"),),
-        (CssSelector(item="picture"),),
-        (CssSelector(item="progress"),),
-        (CssSelector(item="q"),),
-        (CssSelector(item="ruby"),),
-        (CssSelector(item="select"),),
-        (CssSelector(item="slot"),),
-        (CssSelector(item="small"),),
-        (CssSelector(item="span"),),
-        (CssSelector(item="template"),),
-        (CssSelector(item="textarea"),),
-        (CssSelector(item="time"),),
-        (CssSelector(item="tt"),),
-        (CssSelector(item="video"),),
-        (CssSelector(item="wbr"),),
-    ): {"display": "inline"},
-    # Formatted inlines
-    ((CssSelector(item="a"),),): {
-        "display": "inline",
-        "text_decoration": "underline",
-        "color": "ansibrightblue",
-    },
-    ((CssSelector(item="b"),), (CssSelector(item="strong"),)): {
-        "display": "inline",
-        "font_weight": "bold",
-    },
-    (
-        (CssSelector(item="cite"),),
-        (CssSelector(item="dfn"),),
-        (CssSelector(item="em"),),
-        (CssSelector(item="i"),),
-        (CssSelector(item="var"),),
-    ): {"display": "inline", "font_style": "italic"},
-    ((CssSelector(item="code"),),): {
-        "display": "inline",
-    },
-    ((CssSelector(item="del"),), (CssSelector(item="s"),)): {
-        "display": "inline",
-        "text_decoration": "line-through",
-    },
-    ((CssSelector(item="img"),), (CssSelector(item="svg"),)): {
-        "display": "inline-block",
-        "overflow_x": "hidden",
-        "overflow_y": "hidden",
-    },
-    ((CssSelector(item="ins"),), (CssSelector(item="u"),)): {
-        "display": "inline",
-        "text_decoration": "underline",
-    },
-    ((CssSelector(item="kbd"),),): {
-        "display": "inline",
-        "background_color": "#333344",
-        "color": "#FFFFFF",
-    },
-    ((CssSelector(item="mark"),),): {
-        "display": "inline",
-        "color": "black",
-        "background_color": "#FFFF00",
-    },
-    ((CssSelector(item="samp"),),): {
-        "display": "inline",
-        "background_color": "#334433",
-        "color": "#FFFFFF",
-    },
-    ((CssSelector(item="sub"),),): {"display": "inline", "vertical_align": "sub"},
-    ((CssSelector(item="sup"),),): {"display": "inline", "vertical_align": "super"},
-    (
+_BROWSER_CSS: CssSelectors = {
+    always: {
+        # Set body background to white
+        ((CssSelector(item="body"),),): {"background_color": "#FFFFFF"},
+        # Non-rendered elements
         (
-            CssSelector(item="q"),
-            CssSelector(item="::before"),
-        ),
-    ): {"content": "“"},
-    (
+            (CssSelector(item="head"),),
+            (CssSelector(item="base"),),
+            (CssSelector(item="command"),),
+            (CssSelector(item="link"),),
+            (CssSelector(item="meta"),),
+            (CssSelector(item="noscript"),),
+            (CssSelector(item="script"),),
+            (CssSelector(item="style"),),
+            (CssSelector(item="title"),),
+            (CssSelector(item="option"),),
+            (CssSelector(item="input", attr="[type=hidden]"),),
+        ): {"display": "none"},
+        # Inline elements
         (
-            CssSelector(item="q"),
-            CssSelector(item="::after"),
-        ),
-    ): {"content": "”"},
-    # Images
-    (
-        (CssSelector(item="img", attr="[_missing]"),),
-        (CssSelector(item="svg", attr="[_missing]"),),
-    ): {
-        "border_top_style": "solid",
-        "border_right_style": "solid",
-        "border_bottom_style": "solid",
-        "border_left_style": "solid",
-        "border_top_width": "1px",
-        "border_right_width": "1px",
-        "border_bottom_width": "1px",
-        "border_left_width": "1px",
-    },
-    # Alignment
-    ((CssSelector(item="center"),), (CssSelector(item="caption"),)): {
-        "text_align": "center",
-        "display": "block",
-    },
-    # Tables
-    ((CssSelector(item="table"),),): {
-        "display": "table",
-        "border_collapse": "collapse",
-    },
-    ((CssSelector(item="td"),),): {"display": "table-cell", "text_align": "unset"},
-    ((CssSelector(item="th"),),): {
-        "display": "table-cell",
-        "font_weight": "bold",
-        "text_align": "center",
-    },
-    # Forms
-    ((CssSelector(item="input"),),): {
-        "display": "inline-block",
-        "white_space": "pre",
-        "color": "#000000",
-        "border_top_style": "inset",
-        "border_right_style": "inset",
-        "border_bottom_style": "inset",
-        "border_left_style": "inset",
-        "border_top_width": "2px",
-        "border_right_width": "2px",
-        "border_bottom_width": "2px",
-        "border_left_width": "2px",
-        "vertical_align": "middle",
-    },
-    ((CssSelector(item="input", attr="[type=text]"),),): {
-        "background_color": "#FFFFFF",
-        "border_top_color": "#606060",
-        "border_right_color": "#E9E7E3",
-        "border_bottom_color": "#E9E7E3",
-        "border_left_color": "#606060",
-        "overflow_x": "hidden",
-    },
-    (
-        (CssSelector(item="input", attr="[type=button]"),),
-        (CssSelector(item="input", attr="[type=submit]"),),
-        (CssSelector(item="input", attr="[type=reset]"),),
-    ): {
-        "background_color": "#d4d0c8",
-        "border_right": "#606060",
-        "border_bottom": "#606060",
-        "border_left": "#ffffff",
-        "border_top": "#ffffff",
-    },
-    ((CssSelector(item="button"),),): {
-        "display": "inline-block",
-        "color": "#000000",
-        "border_top_style": "outset",
-        "border_right_style": "outset",
-        "border_bottom_style": "outset",
-        "border_left_style": "outset",
-        "border_top_width": "2px",
-        "border_right_width": "2px",
-        "border_bottom_width": "2px",
-        "border_left_width": "2px",
-        "background_color": "#d4d0c8",
-        "border_right": "#606060",
-        "border_bottom": "#606060",
-        "border_left": "#ffffff",
-        "border_top": "#ffffff",
-    },
-    # Headings
-    ((CssSelector(item="h1"),),): {
-        "font_weight": "bold",
-        "text_decoration": "underline",
-        "border_bottom_style": "solid",
-        "border_bottom_width": "thick",
-        "padding_bottom": "2rem",
-        "margin_top": "2rem",
-        "margin_bottom": "2em",
-    },
-    ((CssSelector(item="h2"),),): {
-        "font_weight": "bold",
-        "border_bottom_style": "double",
-        "border_bottom_width": "thick",
-        "padding_bottom": "1.5rem",
-        "margin_top": "1.5rem",
-        "margin_bottom": "1.5rem",
-    },
-    ((CssSelector(item="h3"),),): {
-        "font_weight": "bold",
-        "font_style": "italic",
-        "border_bottom_style": ":lower-left",
-        "border_bottom_width": "thin",
-        "padding_top": "1rem",
-        "padding_bottom": "1rem",
-        "margin_bottom": "1.5rem",
-    },
-    ((CssSelector(item="h4"),),): {
-        "text_decoration": "underline",
-        "border_bottom_style": "solid",
-        "border_bottom_width": "thin",
-        "padding_top": "1rem",
-        "padding_bottom": "1rem",
-        "margin_bottom": "1.5rem",
-    },
-    ((CssSelector(item="h5"),),): {
-        "border_bottom_style": "dashed",
-        "border_bottom_width": "thin",
-        "margin_bottom": "1.5rem",
-    },
-    ((CssSelector(item="h6"),),): {
-        "font_style": "italic",
-        "border_bottom_style": "dotted",
-        "border_bottom_width": "thin",
-        "margin_bottom": "1.5rem",
-    },
-    # Misc blocks
-    ((CssSelector(item="blockquote"),),): {
-        "margin_top": "1em",
-        "margin_bottom": "1em",
-        "margin_right": "2em",
-        "margin_left": "2em",
-    },
-    ((CssSelector(item="hr"),),): {
-        "margin_top": "1rem",
-        "margin_bottom": "1rem",
-        "border_top_width": "thin",
-        "border_top_style": "solid",
-        "border_top_color": "ansired",
-    },
-    ((CssSelector(item="p"),),): {"margin_top": "1em", "margin_bottom": "1em"},
-    ((CssSelector(item="pre"),),): {
-        "margin_top": "1em",
-        "margin_bottom": "1em",
-        "white_space": "pre",
-    },
-    # Lists
-    ((CssSelector(item="::marker"),),): {
-        "display": "inline",
-        "padding_right": "1em",
-        "text_align": "right",
-    },
-    ((CssSelector(item="ol"),),): {
-        "list_style_type": "decimal",
-        "list_style_position": "outside",
-        "padding_left": "4em",
-        "margin_top": "1em",
-        "margin_bottom": "1em",
-    },
-    (
-        (CssSelector(item="ul"),),
-        (CssSelector(item="menu"),),
-        (CssSelector(item="dir"),),
-    ): {
-        "list_style_type": "disc",
-        "list_style_position": "outside",
-        "padding_left": "3em",
-        "margin_top": "1em",
-        "margin_bottom": "1em",
-    },
-    (
-        (CssSelector(item="dir"), CssSelector(item="dir")),
-        (CssSelector(item="dir"), CssSelector(item="menu")),
-        (CssSelector(item="dir"), CssSelector(item="ul")),
-        (CssSelector(item="ol"), CssSelector(item="dir")),
-        (CssSelector(item="ol"), CssSelector(item="menu")),
-        (CssSelector(item="ol"), CssSelector(item="ul")),
-        (CssSelector(item="menu"), CssSelector(item="dir")),
-        (CssSelector(item="menu"), CssSelector(item="menu")),
-        (CssSelector(item="ul"), CssSelector(item="dir")),
-        (CssSelector(item="ul"), CssSelector(item="menu")),
-        (CssSelector(item="ul"), CssSelector(item="ul")),
-    ): {"margin_top": "0em", "margin_bottom": "0em", "list_style_type": "circle"},
-    (
-        (CssSelector(item="dir"), CssSelector(item="dl")),
-        (CssSelector(item="dir"), CssSelector(item="ol")),
-        (CssSelector(item="dl"), CssSelector(item="dir")),
-        (CssSelector(item="dl"), CssSelector(item="dl")),
-        (CssSelector(item="dl"), CssSelector(item="ol")),
-        (CssSelector(item="dl"), CssSelector(item="menu")),
-        (CssSelector(item="dl"), CssSelector(item="ul")),
-        (CssSelector(item="ol"), CssSelector(item="dl")),
-        (CssSelector(item="ol"), CssSelector(item="ol")),
-        (CssSelector(item="menu"), CssSelector(item="dl")),
-        (CssSelector(item="menu"), CssSelector(item="ol")),
-        (CssSelector(item="ul"), CssSelector(item="dl")),
-        (CssSelector(item="ul"), CssSelector(item="ol")),
-    ): {"margin_top": "0em", "margin_bottom": "0em"},
-    ((CssSelector(item="menu"), CssSelector(item="ul")),): {
-        "list_style_type": "circle",
-        "margin_top": "0em",
-        "margin_bottom": "0em",
-    },
-    (
-        (CssSelector(item="dir"), CssSelector(item="dir"), CssSelector(item="dir")),
-        (CssSelector(item="dir"), CssSelector(item="dir"), CssSelector(item="menu")),
-        (CssSelector(item="dir"), CssSelector(item="dir"), CssSelector(item="ul")),
-        (CssSelector(item="dir"), CssSelector(item="menu"), CssSelector(item="dir")),
-        (CssSelector(item="dir"), CssSelector(item="menu"), CssSelector(item="menu")),
-        (CssSelector(item="dir"), CssSelector(item="menu"), CssSelector(item="ul")),
-        (CssSelector(item="dir"), CssSelector(item="ol"), CssSelector(item="dir")),
-        (CssSelector(item="dir"), CssSelector(item="ol"), CssSelector(item="menu")),
-        (CssSelector(item="dir"), CssSelector(item="ol"), CssSelector(item="ul")),
-        (CssSelector(item="dir"), CssSelector(item="ul"), CssSelector(item="dir")),
-        (CssSelector(item="dir"), CssSelector(item="ul"), CssSelector(item="menu")),
-        (CssSelector(item="dir"), CssSelector(item="ul"), CssSelector(item="ul")),
-        (CssSelector(item="menu"), CssSelector(item="dir"), CssSelector(item="dir")),
-        (CssSelector(item="menu"), CssSelector(item="dir"), CssSelector(item="menu")),
-        (CssSelector(item="menu"), CssSelector(item="dir"), CssSelector(item="ul")),
-        (CssSelector(item="menu"), CssSelector(item="menu"), CssSelector(item="dir")),
-        (CssSelector(item="menu"), CssSelector(item="menu"), CssSelector(item="menu")),
-        (CssSelector(item="menu"), CssSelector(item="menu"), CssSelector(item="ul")),
-        (CssSelector(item="menu"), CssSelector(item="ol"), CssSelector(item="dir")),
-        (CssSelector(item="menu"), CssSelector(item="ol"), CssSelector(item="menu")),
-        (CssSelector(item="menu"), CssSelector(item="ol"), CssSelector(item="ul")),
-        (CssSelector(item="menu"), CssSelector(item="ul"), CssSelector(item="dir")),
-        (CssSelector(item="menu"), CssSelector(item="ul"), CssSelector(item="menu")),
-        (CssSelector(item="menu"), CssSelector(item="ul"), CssSelector(item="ul")),
-        (CssSelector(item="ol"), CssSelector(item="dir"), CssSelector(item="dir")),
-        (CssSelector(item="ol"), CssSelector(item="dir"), CssSelector(item="menu")),
-        (CssSelector(item="ol"), CssSelector(item="dir"), CssSelector(item="ul")),
-        (CssSelector(item="ol"), CssSelector(item="menu"), CssSelector(item="dir")),
-        (CssSelector(item="ol"), CssSelector(item="menu"), CssSelector(item="menu")),
-        (CssSelector(item="ol"), CssSelector(item="menu"), CssSelector(item="ul")),
-        (CssSelector(item="ol"), CssSelector(item="ol"), CssSelector(item="dir")),
-        (CssSelector(item="ol"), CssSelector(item="ol"), CssSelector(item="menu")),
-        (CssSelector(item="ol"), CssSelector(item="ol"), CssSelector(item="ul")),
-        (CssSelector(item="ol"), CssSelector(item="ul"), CssSelector(item="dir")),
-        (CssSelector(item="ol"), CssSelector(item="ul"), CssSelector(item="menu")),
-        (CssSelector(item="ol"), CssSelector(item="ul"), CssSelector(item="ul")),
-        (CssSelector(item="ul"), CssSelector(item="dir"), CssSelector(item="dir")),
-        (CssSelector(item="ul"), CssSelector(item="dir"), CssSelector(item="menu")),
-        (CssSelector(item="ul"), CssSelector(item="dir"), CssSelector(item="ul")),
-        (CssSelector(item="ul"), CssSelector(item="menu"), CssSelector(item="dir")),
-        (CssSelector(item="ul"), CssSelector(item="menu"), CssSelector(item="menu")),
-        (CssSelector(item="ul"), CssSelector(item="menu"), CssSelector(item="ul")),
-        (CssSelector(item="ul"), CssSelector(item="ol"), CssSelector(item="dir")),
-        (CssSelector(item="ul"), CssSelector(item="ol"), CssSelector(item="menu")),
-        (CssSelector(item="ul"), CssSelector(item="ol"), CssSelector(item="ul")),
-        (CssSelector(item="ul"), CssSelector(item="ul"), CssSelector(item="dir")),
-        (CssSelector(item="ul"), CssSelector(item="ul"), CssSelector(item="menu")),
-        (CssSelector(item="ul"), CssSelector(item="ul"), CssSelector(item="ul")),
-    ): {"list_style_type": "square"},
-    ((CssSelector(item="li"),),): {"display": "list-item"},
-    ((CssSelector(item="details"),),): {
-        "list_style_type": "disclosure-closed",
-        "list_style_position": "inside",
-    },
-    ((CssSelector(item="details", attr="[open]"), CssSelector(item="summary")),): {
-        "list_style_type": "disclosure-open"
-    },
-    ((CssSelector(item="summary"),),): {"display": "list-item", "font_weight": "bold"},
-    # Dataframes for Jupyter
-    ((CssSelector(item=".dataframe"),),): {"_pt_class": "dataframe"},
-    (
-        (CssSelector(item=".dataframe"), CssSelector(item="td")),
-        (CssSelector(item=".dataframe"), CssSelector(item="th")),
-    ): {
-        "border_top_style": "hidden",
-        "border_left_style": "hidden",
-        "border_bottom_style": "hidden",
-        "border_right_style": "hidden",
-        "padding_left": "1em",
-    },
-    (
+            (CssSelector(item="::before"),),
+            (CssSelector(item="::after"),),
+            (CssSelector(item="text"),),
+            (CssSelector(item="abbr"),),
+            (CssSelector(item="acronym"),),
+            (CssSelector(item="audio"),),
+            (CssSelector(item="bdi"),),
+            (CssSelector(item="bdo"),),
+            (CssSelector(item="big"),),
+            (CssSelector(item="br"),),
+            (CssSelector(item="canvas"),),
+            (CssSelector(item="data"),),
+            (CssSelector(item="datalist"),),
+            (CssSelector(item="embed"),),
+            (CssSelector(item="iframe"),),
+            (CssSelector(item="label"),),
+            (CssSelector(item="map"),),
+            (CssSelector(item="meter"),),
+            (CssSelector(item="object"),),
+            (CssSelector(item="output"),),
+            (CssSelector(item="picture"),),
+            (CssSelector(item="progress"),),
+            (CssSelector(item="q"),),
+            (CssSelector(item="ruby"),),
+            (CssSelector(item="select"),),
+            (CssSelector(item="slot"),),
+            (CssSelector(item="small"),),
+            (CssSelector(item="span"),),
+            (CssSelector(item="template"),),
+            (CssSelector(item="textarea"),),
+            (CssSelector(item="time"),),
+            (CssSelector(item="tt"),),
+            (CssSelector(item="video"),),
+            (CssSelector(item="wbr"),),
+        ): {"display": "inline"},
+        # Formatted inlines
+        ((CssSelector(item="a"),),): {
+            "display": "inline",
+            "text_decoration": "underline",
+            "color": "ansibrightblue",
+        },
+        ((CssSelector(item="b"),), (CssSelector(item="strong"),)): {
+            "display": "inline",
+            "font_weight": "bold",
+        },
         (
-            CssSelector(item=".dataframe"),
-            CssSelector(item="th"),
-        ),
-    ): {
-        "_pt_class": "dataframe,th",
-    },
-    (
-        (CssSelector(item=".dataframe"), CssSelector(item="th", pseudo=":first-child")),
-        (CssSelector(item=".dataframe"), CssSelector(item="th", pseudo=":last-child")),
-        (CssSelector(item=".dataframe"), CssSelector(item="td", pseudo=":last-child")),
-    ): {"padding_right": "1em"},
-    ((CssSelector(item=".dataframe"), CssSelector(item="td")),): {
-        "_pt_class": "dataframe,td bg:default"
-    },
-    (
+            (CssSelector(item="cite"),),
+            (CssSelector(item="dfn"),),
+            (CssSelector(item="em"),),
+            (CssSelector(item="i"),),
+            (CssSelector(item="var"),),
+        ): {"display": "inline", "font_style": "italic"},
+        ((CssSelector(item="code"),),): {
+            "display": "inline",
+        },
+        ((CssSelector(item="del"),), (CssSelector(item="s"),)): {
+            "display": "inline",
+            "text_decoration": "line-through",
+        },
+        (
+            (CssSelector(item="img", attr="[width=0]"),),
+            (CssSelector(item="img", attr="[height=0]"),),
+            (CssSelector(item="svg", attr="[width=0]"),),
+            (CssSelector(item="svg", attr="[height=0]"),),
+        ): {"display": "none"},
+        ((CssSelector(item="img"),), (CssSelector(item="svg"),)): {
+            "display": "inline-block",
+            "overflow_x": "hidden",
+            "overflow_y": "hidden",
+        },
+        ((CssSelector(item="ins"),), (CssSelector(item="u"),)): {
+            "display": "inline",
+            "text_decoration": "underline",
+        },
+        ((CssSelector(item="kbd"),),): {
+            "display": "inline",
+            "background_color": "#333344",
+            "color": "#FFFFFF",
+        },
+        ((CssSelector(item="mark"),),): {
+            "display": "inline",
+            "color": "black",
+            "background_color": "#FFFF00",
+        },
+        ((CssSelector(item="samp"),),): {
+            "display": "inline",
+            "background_color": "#334433",
+            "color": "#FFFFFF",
+        },
+        ((CssSelector(item="sub"),),): {"display": "inline", "vertical_align": "sub"},
+        ((CssSelector(item="sup"),),): {"display": "inline", "vertical_align": "super"},
+        (
+            (
+                CssSelector(item="q"),
+                CssSelector(item="::before"),
+            ),
+        ): {"content": "“"},
+        (
+            (
+                CssSelector(item="q"),
+                CssSelector(item="::after"),
+            ),
+        ): {"content": "”"},
+        # Images
+        (
+            (CssSelector(item="img", attr="[_missing]"),),
+            (CssSelector(item="svg", attr="[_missing]"),),
+        ): {
+            "border_top_style": "solid",
+            "border_right_style": "solid",
+            "border_bottom_style": "solid",
+            "border_left_style": "solid",
+            "border_top_width": "1px",
+            "border_right_width": "1px",
+            "border_bottom_width": "1px",
+            "border_left_width": "1px",
+        },
+        # Alignment
+        ((CssSelector(item="center"),), (CssSelector(item="caption"),)): {
+            "text_align": "center",
+            "display": "block",
+        },
+        # Tables
+        ((CssSelector(item="table"),),): {
+            "display": "table",
+            "border_collapse": "collapse",
+        },
+        (
+            (CssSelector(item="td"),),
+            (CssSelector(item="th"),),
+        ): {
+            "border_top_width": "0px",
+            "border_right_width": "0px",
+            "border_bottom_width": "0px",
+            "border_left_width": "0px",
+        },
+        ((CssSelector(item="td"),),): {"display": "table-cell", "text_align": "unset"},
+        ((CssSelector(item="th"),),): {
+            "display": "table-cell",
+            "font_weight": "bold",
+            "text_align": "center",
+        },
+        # Forms
+        ((CssSelector(item="input"),),): {
+            "display": "inline-block",
+            "white_space": "pre",
+            "color": "#000000",
+            "border_top_style": "inset",
+            "border_right_style": "inset",
+            "border_bottom_style": "inset",
+            "border_left_style": "inset",
+            "border_top_width": "2px",
+            "border_right_width": "2px",
+            "border_bottom_width": "2px",
+            "border_left_width": "2px",
+            "vertical_align": "middle",
+        },
+        ((CssSelector(item="input", attr="[type=text]"),),): {
+            "background_color": "#FAFAFA",
+            "border_top_color": "#606060",
+            "border_right_color": "#E9E7E3",
+            "border_bottom_color": "#E9E7E3",
+            "border_left_color": "#606060",
+            "overflow_x": "hidden",
+        },
+        (
+            (CssSelector(item="input", attr="[type=button]"),),
+            (CssSelector(item="input", attr="[type=submit]"),),
+            (CssSelector(item="input", attr="[type=reset]"),),
+        ): {
+            "background_color": "#d4d0c8",
+            "border_right": "#606060",
+            "border_bottom": "#606060",
+            "border_left": "#ffffff",
+            "border_top": "#ffffff",
+        },
+        ((CssSelector(item="button"),),): {
+            "display": "inline-block",
+            "color": "#000000",
+            "border_top_style": "outset",
+            "border_right_style": "outset",
+            "border_bottom_style": "outset",
+            "border_left_style": "outset",
+            "border_top_width": "2px",
+            "border_right_width": "2px",
+            "border_bottom_width": "2px",
+            "border_left_width": "2px",
+            "background_color": "#d4d0c8",
+            "border_right": "#606060",
+            "border_bottom": "#606060",
+            "border_left": "#ffffff",
+            "border_top": "#ffffff",
+        },
+        # Headings
+        ((CssSelector(item="h1"),),): {
+            "font_weight": "bold",
+            "text_decoration": "underline",
+            "border_bottom_style": "solid",
+            "border_bottom_width": "thick",
+            "padding_bottom": "2rem",
+            "margin_top": "2rem",
+            "margin_bottom": "2em",
+        },
+        ((CssSelector(item="h2"),),): {
+            "font_weight": "bold",
+            "border_bottom_style": "double",
+            "border_bottom_width": "thick",
+            "padding_bottom": "1.5rem",
+            "margin_top": "1.5rem",
+            "margin_bottom": "1.5rem",
+        },
+        ((CssSelector(item="h3"),),): {
+            "font_weight": "bold",
+            "font_style": "italic",
+            "border_bottom_style": ":lower-left",
+            "border_bottom_width": "thin",
+            "padding_top": "1rem",
+            "padding_bottom": "1rem",
+            "margin_bottom": "1.5rem",
+        },
+        ((CssSelector(item="h4"),),): {
+            "text_decoration": "underline",
+            "border_bottom_style": "solid",
+            "border_bottom_width": "thin",
+            "padding_top": "1rem",
+            "padding_bottom": "1rem",
+            "margin_bottom": "1.5rem",
+        },
+        ((CssSelector(item="h5"),),): {
+            "border_bottom_style": "dashed",
+            "border_bottom_width": "thin",
+            "margin_bottom": "1.5rem",
+        },
+        ((CssSelector(item="h6"),),): {
+            "font_style": "italic",
+            "border_bottom_style": "dotted",
+            "border_bottom_width": "thin",
+            "margin_bottom": "1.5rem",
+        },
+        # Misc blocks
+        ((CssSelector(item="blockquote"),),): {
+            "margin_top": "1em",
+            "margin_bottom": "1em",
+            "margin_right": "2em",
+            "margin_left": "2em",
+        },
+        ((CssSelector(item="hr"),),): {
+            "margin_top": "1rem",
+            "margin_bottom": "1rem",
+            "border_top_width": "thin",
+            "border_top_style": "solid",
+            "border_top_color": "ansired",
+            "width": "100%",
+        },
+        ((CssSelector(item="p"),),): {"margin_top": "1em", "margin_bottom": "1em"},
+        ((CssSelector(item="pre"),),): {
+            "margin_top": "1em",
+            "margin_bottom": "1em",
+            "white_space": "pre",
+        },
+        # Lists
+        ((CssSelector(item="::marker"),),): {
+            "display": "inline",
+            "padding_right": "1em",
+            "text_align": "right",
+        },
+        ((CssSelector(item="ol"),),): {
+            "list_style_type": "decimal",
+            "list_style_position": "outside",
+            "padding_left": "4em",
+            "margin_top": "1em",
+            "margin_bottom": "1em",
+        },
+        (
+            (CssSelector(item="ul"),),
+            (CssSelector(item="menu"),),
+            (CssSelector(item="dir"),),
+        ): {
+            "list_style_type": "disc",
+            "list_style_position": "outside",
+            "padding_left": "3em",
+            "margin_top": "1em",
+            "margin_bottom": "1em",
+        },
+        (
+            (CssSelector(item="dir"), CssSelector(item="dir")),
+            (CssSelector(item="dir"), CssSelector(item="menu")),
+            (CssSelector(item="dir"), CssSelector(item="ul")),
+            (CssSelector(item="ol"), CssSelector(item="dir")),
+            (CssSelector(item="ol"), CssSelector(item="menu")),
+            (CssSelector(item="ol"), CssSelector(item="ul")),
+            (CssSelector(item="menu"), CssSelector(item="dir")),
+            (CssSelector(item="menu"), CssSelector(item="menu")),
+            (CssSelector(item="ul"), CssSelector(item="dir")),
+            (CssSelector(item="ul"), CssSelector(item="menu")),
+            (CssSelector(item="ul"), CssSelector(item="ul")),
+        ): {"margin_top": "0em", "margin_bottom": "0em", "list_style_type": "circle"},
+        (
+            (CssSelector(item="dir"), CssSelector(item="dl")),
+            (CssSelector(item="dir"), CssSelector(item="ol")),
+            (CssSelector(item="dl"), CssSelector(item="dir")),
+            (CssSelector(item="dl"), CssSelector(item="dl")),
+            (CssSelector(item="dl"), CssSelector(item="ol")),
+            (CssSelector(item="dl"), CssSelector(item="menu")),
+            (CssSelector(item="dl"), CssSelector(item="ul")),
+            (CssSelector(item="ol"), CssSelector(item="dl")),
+            (CssSelector(item="ol"), CssSelector(item="ol")),
+            (CssSelector(item="menu"), CssSelector(item="dl")),
+            (CssSelector(item="menu"), CssSelector(item="ol")),
+            (CssSelector(item="ul"), CssSelector(item="dl")),
+            (CssSelector(item="ul"), CssSelector(item="ol")),
+        ): {"margin_top": "0em", "margin_bottom": "0em"},
+        ((CssSelector(item="menu"), CssSelector(item="ul")),): {
+            "list_style_type": "circle",
+            "margin_top": "0em",
+            "margin_bottom": "0em",
+        },
         (
-            CssSelector(item=".dataframe"),
-            CssSelector(item="tr", pseudo=":nth-child(odd)"),
-            CssSelector(item="td"),
-        ),
-    ): {"_pt_class": "dataframe,row-odd,td"},
+            (CssSelector(item="dir"), CssSelector(item="dir"), CssSelector(item="dir")),
+            (
+                CssSelector(item="dir"),
+                CssSelector(item="dir"),
+                CssSelector(item="menu"),
+            ),
+            (CssSelector(item="dir"), CssSelector(item="dir"), CssSelector(item="ul")),
+            (
+                CssSelector(item="dir"),
+                CssSelector(item="menu"),
+                CssSelector(item="dir"),
+            ),
+            (
+                CssSelector(item="dir"),
+                CssSelector(item="menu"),
+                CssSelector(item="menu"),
+            ),
+            (CssSelector(item="dir"), CssSelector(item="menu"), CssSelector(item="ul")),
+            (CssSelector(item="dir"), CssSelector(item="ol"), CssSelector(item="dir")),
+            (CssSelector(item="dir"), CssSelector(item="ol"), CssSelector(item="menu")),
+            (CssSelector(item="dir"), CssSelector(item="ol"), CssSelector(item="ul")),
+            (CssSelector(item="dir"), CssSelector(item="ul"), CssSelector(item="dir")),
+            (CssSelector(item="dir"), CssSelector(item="ul"), CssSelector(item="menu")),
+            (CssSelector(item="dir"), CssSelector(item="ul"), CssSelector(item="ul")),
+            (
+                CssSelector(item="menu"),
+                CssSelector(item="dir"),
+                CssSelector(item="dir"),
+            ),
+            (
+                CssSelector(item="menu"),
+                CssSelector(item="dir"),
+                CssSelector(item="menu"),
+            ),
+            (CssSelector(item="menu"), CssSelector(item="dir"), CssSelector(item="ul")),
+            (
+                CssSelector(item="menu"),
+                CssSelector(item="menu"),
+                CssSelector(item="dir"),
+            ),
+            (
+                CssSelector(item="menu"),
+                CssSelector(item="menu"),
+                CssSelector(item="menu"),
+            ),
+            (
+                CssSelector(item="menu"),
+                CssSelector(item="menu"),
+                CssSelector(item="ul"),
+            ),
+            (CssSelector(item="menu"), CssSelector(item="ol"), CssSelector(item="dir")),
+            (
+                CssSelector(item="menu"),
+                CssSelector(item="ol"),
+                CssSelector(item="menu"),
+            ),
+            (CssSelector(item="menu"), CssSelector(item="ol"), CssSelector(item="ul")),
+            (CssSelector(item="menu"), CssSelector(item="ul"), CssSelector(item="dir")),
+            (
+                CssSelector(item="menu"),
+                CssSelector(item="ul"),
+                CssSelector(item="menu"),
+            ),
+            (CssSelector(item="menu"), CssSelector(item="ul"), CssSelector(item="ul")),
+            (CssSelector(item="ol"), CssSelector(item="dir"), CssSelector(item="dir")),
+            (CssSelector(item="ol"), CssSelector(item="dir"), CssSelector(item="menu")),
+            (CssSelector(item="ol"), CssSelector(item="dir"), CssSelector(item="ul")),
+            (CssSelector(item="ol"), CssSelector(item="menu"), CssSelector(item="dir")),
+            (
+                CssSelector(item="ol"),
+                CssSelector(item="menu"),
+                CssSelector(item="menu"),
+            ),
+            (CssSelector(item="ol"), CssSelector(item="menu"), CssSelector(item="ul")),
+            (CssSelector(item="ol"), CssSelector(item="ol"), CssSelector(item="dir")),
+            (CssSelector(item="ol"), CssSelector(item="ol"), CssSelector(item="menu")),
+            (CssSelector(item="ol"), CssSelector(item="ol"), CssSelector(item="ul")),
+            (CssSelector(item="ol"), CssSelector(item="ul"), CssSelector(item="dir")),
+            (CssSelector(item="ol"), CssSelector(item="ul"), CssSelector(item="menu")),
+            (CssSelector(item="ol"), CssSelector(item="ul"), CssSelector(item="ul")),
+            (CssSelector(item="ul"), CssSelector(item="dir"), CssSelector(item="dir")),
+            (CssSelector(item="ul"), CssSelector(item="dir"), CssSelector(item="menu")),
+            (CssSelector(item="ul"), CssSelector(item="dir"), CssSelector(item="ul")),
+            (CssSelector(item="ul"), CssSelector(item="menu"), CssSelector(item="dir")),
+            (
+                CssSelector(item="ul"),
+                CssSelector(item="menu"),
+                CssSelector(item="menu"),
+            ),
+            (CssSelector(item="ul"), CssSelector(item="menu"), CssSelector(item="ul")),
+            (CssSelector(item="ul"), CssSelector(item="ol"), CssSelector(item="dir")),
+            (CssSelector(item="ul"), CssSelector(item="ol"), CssSelector(item="menu")),
+            (CssSelector(item="ul"), CssSelector(item="ol"), CssSelector(item="ul")),
+            (CssSelector(item="ul"), CssSelector(item="ul"), CssSelector(item="dir")),
+            (CssSelector(item="ul"), CssSelector(item="ul"), CssSelector(item="menu")),
+            (CssSelector(item="ul"), CssSelector(item="ul"), CssSelector(item="ul")),
+        ): {"list_style_type": "square"},
+        ((CssSelector(item="li"),),): {"display": "list-item"},
+        ((CssSelector(item="details"),),): {
+            "list_style_type": "disclosure-closed",
+            "list_style_position": "inside",
+        },
+        ((CssSelector(item="details", attr="[open]"), CssSelector(item="summary")),): {
+            "list_style_type": "disclosure-open"
+        },
+        ((CssSelector(item="summary"),),): {
+            "display": "list-item",
+            "font_weight": "bold",
+        },
+        # Dataframes for Jupyter
+        ((CssSelector(item=".dataframe"),),): {"_pt_class": "dataframe"},
+        (
+            (CssSelector(item=".dataframe"), CssSelector(item="td")),
+            (CssSelector(item=".dataframe"), CssSelector(item="th")),
+        ): {
+            "border_top_style": "hidden",
+            "border_left_style": "hidden",
+            "border_bottom_style": "hidden",
+            "border_right_style": "hidden",
+            "padding_left": "1em",
+        },
+        (
+            (
+                CssSelector(item=".dataframe"),
+                CssSelector(item="th"),
+            ),
+        ): {
+            "_pt_class": "dataframe,th",
+        },
+        (
+            (
+                CssSelector(item=".dataframe"),
+                CssSelector(item="th", pseudo=":first-child"),
+            ),
+            (
+                CssSelector(item=".dataframe"),
+                CssSelector(item="th", pseudo=":last-child"),
+            ),
+            (
+                CssSelector(item=".dataframe"),
+                CssSelector(item="td", pseudo=":last-child"),
+            ),
+        ): {"padding_right": "1em"},
+        ((CssSelector(item=".dataframe"), CssSelector(item="td")),): {
+            "_pt_class": "dataframe,td bg:default"
+        },
+        (
+            (
+                CssSelector(item=".dataframe"),
+                CssSelector(item="tr", pseudo=":nth-child(odd)"),
+                CssSelector(item="td"),
+            ),
+        ): {"_pt_class": "dataframe,row-odd,td"},
+    }
 }
 
 
 class Node:
     """Represent an node in the DOM."""
 
     theme: Theme
@@ -1938,16 +2316,15 @@
         self.attrs: dict[str, Any] = {k: v for k, v in (attrs or []) if v is not None}
         self.contents: list[Node] = contents or []
         self.closed = False
         self.marker: Node | None = None
         self.before: Node | None = None
         self.after: Node | None = None
 
-        parent_theme = parent.theme if parent else None
-        self.theme = Theme(self, parent_theme=parent_theme)
+        self.theme = Theme(self, parent_theme=parent.theme if parent else None)
 
     def _outer_html(self, d: int = 0, attrs: bool = True) -> str:
         dd = " " * d
         s = ""
         if self.name != "text":
             s += f"{dd}<{self.name}"
             if attrs:
@@ -1963,52 +2340,155 @@
                     s += f"\n{dd}{dd}"
                 s += f"</{self.name}>"
         else:
             s += f"{dd}{self.text}"
         return s
 
     @cached_property
+    def preceding_text(self) -> str:
+        """Return the text preceding this element."""
+        s = ""
+        parent = self.parent
+        while parent and not parent.theme.d_blocky:
+            parent = parent.parent
+        if parent:
+            for node in parent.renderable_descendents:
+                if node is self:
+                    break
+                s += node.text
+        return s
+
+    @cached_property
     def text(self) -> str:
         """Get the element's computed text."""
         if text := self._text:
             if callable(transform := self.theme.text_transform):
                 text = transform(text)
 
-            if not self.theme.preformatted:
-                # Strip whitespace
-                strippable = True
-                for i in text:
-                    if i not in "\x20\x0a\x09\x0c\x0d":
-                        strippable = False
-                        break
-                if strippable:
-                    if "\n" in text:
-                        text = "\n"
-                    else:
-                        text = " "
+            # if False and not (preformatted := self.theme.preformatted):
+            if not (preformatted := self.theme.preformatted):
+                # 1. All spaces and tabs immediately before and after a line break are ignored
+                text = re.sub(r"(\s+(?=\n)|(?<=\n)\s+)", "", text, re.MULTILINE)
+                # 2. All tab characters are handled as space characters
+                text = text.replace("\t", " ")
+                # 3. Line breaks are converted to spaces
+                text = text.replace("\n", " ")
+                # 4. any space immediately following another space is ignored
+                # (even across two separate inline elements)
+                text = re.sub(r"\s\s+", " ", text)
+                if not (
+                    preceding_text := self.preceding_text
+                ) or preceding_text.endswith(" "):
+                    text = text.lstrip(" ")
+                # 5. Sequences of spaces at the beginning and end of an element are removed
+                if text:
+                    parent = self.parent
+                    while (
+                        parent
+                        and parent.is_first_child_element
+                        and not parent.theme.d_blocky
+                    ):
+                        parent = parent.parent
+                    if parent and parent.theme.d_blocky:
+                        if text[0] == " " and (self.is_first_child_node):
+                            text = text[1:]
+                if text:
+                    parent = self.parent
+                    while (
+                        parent
+                        and parent.is_last_child_element
+                        and not parent.theme.d_blocky
+                    ):
+                        parent = parent.parent
+                    if text[-1] == " " and (self.is_last_child_node):
+                        text = text[:-1]
+
+                # Remove space around text in block contexts
+                if (
+                    text
+                    and (node := self.prev_node)
+                    and (node.theme.d_blocky or node.name == "br")
+                ):
+                    text = text.lstrip("\x20\x0a\x09\x0c\x0d")
+                if (
+                    text
+                    and (node := self.next_node)
+                    and (node.theme.d_blocky or node.name == "br")
+                ):
+                    text = text.rstrip(" \t\r\n\x0c")
 
-                # Collapse whitespace
-                text = re.sub(r"\s+", " ", text.strip("\n").replace("\n", " "))
+            elif preformatted and self.is_last_child_node:
+                # TODO - align tabstops
+                text = text.replace("\t", "    ")
+                # Remove one trailing newline
+                if text[-1] == "\n":
+                    text = text[:-1]
 
         return text
 
     def find_all(self, tag: str, recursive: bool = False) -> list[Node]:
         """Find all child elements of a given tag type."""
         return [element for element in self.contents if element.name == tag]
 
+    @cached_property
+    def renderable_contents(self) -> list[Node]:
+        """List the node's contents including '::before' and '::after' elements."""
+        # Do not add '::before' and '::after' elements to themselves
+        if self.name.startswith("::") or self.name == "text":
+            return self.contents
+
+        contents = []
+
+        # Add ::before node
+        before_node = Node(dom=self.dom, name="::before", parent=self)
+        if text := before_node.theme.theme.get("content", "").strip('"').strip("'"):
+            before_node.contents.append(
+                Node(dom=self.dom, name="text", parent=before_node, text=text)
+            )
+            contents.append(before_node)
+
+        contents.extend(self.contents)
+
+        # Add ::after node
+        after_node = Node(dom=self.dom, name="::after", parent=self)
+        if text := after_node.theme.theme.get("content", "").strip('"').strip("'"):
+            after_node.contents.append(
+                Node(dom=self.dom, name="text", parent=after_node, text=text)
+            )
+            contents.append(after_node)
+
+        return contents
+
     @property
     def descendents(self) -> Generator[Node, None, None]:
         """Yield all descendent elements."""
         for child in self.contents:
             yield child
             yield from child.descendents
 
+    @property
+    def renderable_descendents(self) -> Generator[Node, None, None]:
+        """Yield descendents, including pseudo and skipping inline elements."""
+        for child in self.renderable_contents:
+            if (
+                child.theme.d_inline
+                and child.renderable_contents
+                and child.name != "text"
+            ):
+                yield from child.renderable_descendents
+            # elif (
+            #     child.name == "text" and self.name != "::block" and self.theme.d_blocky
+            # ):
+            #     yield Node(dom=self.dom, name="::block", parent=self, contents=[child])
+            else:
+                yield child
+
     @cached_property
     def parents(self) -> list[Node]:
-        """Yield all descendent elements."""
+        """Yield all parent elements."""
         parents = []
         parent = self.parent
         while parent is not None:
             parents.append(parent)
             parent = parent.parent
         return parents[::-1]
 
@@ -2153,25 +2633,28 @@
         parts = [self.name, *[f'{k}="{v}"' for k, v in self.attrs.items()]]
         return f"<{' '.join(parts)}>"
 
 
 class CustomHTMLParser(HTMLParser):
     """An HTML parser."""
 
+    soup: Node
+    curr: Node
+
     def __init__(self, dom: HTML) -> None:
         """Create a new parser instance."""
         super().__init__()
         self.dom = dom
-        self.curr = self.soup = Node(name="::root", dom=dom, parent=None, attrs=[])
 
     def parse(self, markup: str) -> Node:
         """Pare HTML markup."""
-        self.curr = self.soup = Node(dom=self.dom, name="::root", parent=None, attrs=[])
+        soup = Node(name="::root", dom=self.dom, parent=None, attrs=[])
+        self.curr = soup
         self.feed(markup)
-        return self.soup
+        return soup
 
     def handle_starttag(self, tag: str, attrs: list[tuple[str, str | None]]) -> None:
         """Open a new element."""
         self.autoclose()
         element = Node(dom=self.dom, name=tag, parent=self.curr, attrs=attrs)
         self.curr.contents.append(element)
         self.curr = element
@@ -2183,93 +2666,40 @@
             if self.curr.parent:
                 self.curr = self.curr.parent
 
     def handle_data(self, data: str) -> None:
         """Create data (text) elements."""
         self.autoclose()
         self.curr.contents.append(
-            Node(
-                dom=self.dom,
-                name="text",
-                parent=self.curr,
-                text=data,
-                attrs=[],
-            )
+            Node(dom=self.dom, name="text", text=data, parent=self.curr, attrs=[])
         )
 
     def handle_endtag(self, tag: str) -> None:
         """Handle end tags: close the currently opened element."""
         if tag != self.curr.name:
             self.autoclose()
         self.curr.closed = True
         if self.curr.parent:
             self.curr = self.curr.parent
 
 
-def parse_styles(soup: Node, base_url: UPath) -> CssSelectors:
+def parse_style_sheet(css_str: str, dom: HTML) -> None:
     """Collect all CSS styles from style tags."""
-    rules: CssSelectors = {}
-    for child in soup.descendents:
-        css_str = ""
-
-        # In case of a <link> style, load the url
-        if (
-            child.name == "link"
-            and child.attrs.get("rel") == "stylesheet"
-            and (href := child.attrs.get("href"))
-        ):
-            if css_bytes := load_url(href, base_url):
-                css_str = css_bytes.decode()
+    dom_css = dom.css
+    # Remove whitespace and newlines
+    # css_str = css_str.strip().replace("\n", "")
+    css_str = re.sub(r"\s*\n\s*", " ", css_str)
+    # Remove comments
+    css_str = re.sub(r"\/\*[^\*]+\*\/", "", css_str)
+    # Replace ':before' and ':after' with '::before' and '::after'
+    # for compatibility with old CSS and to make root selector work
+    css_str = re.sub("(?<!:):(?=before|after|root)", "::", css_str)
 
-        # In case of a <style> tab, load first child's text
-        elif child.name == "style":
-            if child.contents:
-                css_str = child.contents[0].text
-        else:
-            continue
-        # Remove whitespace and newlines
-        # css_str = css_str.strip().replace("\n", "")
-        css_str = re.sub(r"\s*\n\s*", " ", css_str)
-        # Remove comments
-        css_str = re.sub(r"\/\*[^\*]+\*\/", "", css_str)
-        # Replace ':before' and ':after' with '::before' and '::after'
-        css_str = re.sub("(?<!:):(?=before|after)", "::", css_str)
-        # Allow plain '@media screen' queries
-        css_str = re.sub(
-            r"""
-            @media\s+screen\s*{\s*
-              (.+? {
-                (?:[^:}]+\s*:\s*[^;}]+\s*;\s*)*
-                (?:[^:}]+\s*:\s*[^;}]+\s*;?\s*)?
-              })
-              \s*
-            }
-            """,
-            "\\1",
-            css_str,
-            0,
-            flags=re.DOTALL | re.VERBOSE,
-        )
-        # Remove other media queries for now - TODO
-        # TODO - Far too slow sometimes!
-        css_str = re.sub(
-            r"""
-            @media.+?{\s*
-              (.+? {
-                (?:[^:}]+\s*:\s*[^;}]+\s*;\s*)*
-                (?:[^:}]+\s*:\s*[^;}]+\s*;?\s*)?
-              })
-              \s*
-            }
-            """,
-            "",
-            css_str,
-            0,
-            flags=re.DOTALL | re.VERBOSE,
-        )
+    def parse_part(condition: Filter, css_str: str) -> None:
+        """Parse a group of CSS rules."""
         if css_str:
             css_str = css_str.replace("\n", "").strip()
             if css_str:
                 for rule in css_str.rstrip("}").split("}"):
                     selectors, _, content = rule.partition("{")
                     content = content.strip().rstrip(";")
                     rule_content = parse_css_content(content)
@@ -2277,187 +2707,377 @@
                         parsed_selectors = tuple(
                             tuple(
                                 CssSelector(**m.groupdict())
                                 for m in _SELECTOR_RE.finditer(selector.strip())
                             )
                             for selector in map(str.strip, selectors.split(","))
                         )
+                        rules = dom_css.setdefault(condition, {})
                         if parsed_selectors in rules:
                             rules[parsed_selectors].update(rule_content)
                         else:
                             rules[parsed_selectors] = rule_content
 
-    return rules
+    # Split out nested at-rules - we need to process them separately
+    for part in _AT_RULE_RE.split(css_str):
+        if (
+            part
+            and part[0] == "@"
+            and (m := _NESTED_AT_RULE_RE.match(part)) is not None
+        ):
+            m_dict = m.groupdict()
+            # Process '@media' queries
+            if m_dict["identifier"] == "media":
+                # Split each query - separated by "or" or ","
+                queries = re.split("(?: or |,)", m_dict["rule"])
+                query_conditions: Filter = never
+                for query in queries:
+                    # Each query can be the logical sum of multiple targets
+                    target_conditions: Filter = always
+                    for target in query.split(" and "):
+                        if (
+                            target_m := _MEDIA_QUERY_TARGET_RE.match(target)
+                        ) is not None:
+                            target_m_dict = target_m.groupdict()
+                            # Check for media type conditions
+                            if (media_type := target_m_dict["type"]) is not None:
+                                target_conditions &= (
+                                    always if media_type in {"all", "screen"} else never
+                                )
+                            # Check for media feature confitions
+                            elif (
+                                media_feature := target_m_dict["feature"]
+                            ) is not None:
+                                target_conditions &= parse_media_condition(
+                                    media_feature, dom
+                                )
+                            # Check for logical 'NOT' inverting the target condition
+                            if target_m_dict["invert"]:
+                                target_conditions = ~target_conditions
+                    # Logical OR of all media queries
+                    query_conditions |= target_conditions
+                # Parse the @media CSS block
+                parse_part(query_conditions, m_dict["part"])
+        # If we are outinside an at-rule block, parse the CSS and always use it
+        else:
+            parse_part(always, part)
+
+
+def parse_media_condition(condition: str, dom: HTML) -> Filter:
+    """Convert media rules to conditions."""
+    condition = condition.replace(" ", "")
+    result: Filter
+
+    for op_str, op_func in (("<=", le), (">=", ge), ("<", lt), (">", gt), ("=", eq)):
+        if op_str in condition:
+            operator = op_func
+            feature, _, value = condition.partition(op_str)
+            break
+    else:
+        feature, _, value = condition.partition(":")
+        if feature.startswith("max-"):
+            operator = le
+            feature = feature[4:]
+        elif feature.startswith("min-"):
+            operator = ge
+            feature = feature[4:]
+        else:
+            operator = eq
+
+    if feature == "width":
+        result = Condition(
+            lambda: operator(
+                width := dom.width or 80,
+                css_dimension(value, vertical=False, available=width) or 80,
+            )
+        )
+    elif feature == "height":
+        result = Condition(
+            lambda: operator(
+                height := dom.height or 24,
+                css_dimension(value, vertical=True, available=height) or 24,
+            )
+        )
+    elif feature == "aspect":
+        result = Condition(
+            lambda: operator(
+                (width := (dom.width or 80)) / (height := (dom.height or 24)),
+                (
+                    80
+                    if (dim := css_dimension(value, vertical=False, available=width))
+                    is None
+                    else dim
+                )
+                / (
+                    24
+                    if (dim := css_dimension(value, vertical=True, available=height))
+                    is None
+                    else dim
+                ),
+            )
+        )
+
+    elif feature == "device-width":
+        result = Condition(
+            lambda: operator(
+                (
+                    output.get_size()
+                    if (output := get_app_session()._output)
+                    else Size(24, 80)
+                ).columns,
+                css_dimension(value, vertical=False, available=dom.width) or 80,
+            )
+        )
+    elif feature == "device-height":
+        result = Condition(
+            lambda: operator(
+                (
+                    output.get_size()
+                    if (output := get_app_session()._output)
+                    else Size(24, 80)
+                ).rows,
+                css_dimension(value, vertical=True, available=dom.height) or 24,
+            )
+        )
+    elif feature == "device-aspect":
+        result = Condition(
+            lambda: operator(
+                (
+                    size := (
+                        output.get_size()
+                        if (output := get_app_session()._output)
+                        else Size(24, 80)
+                    )
+                ).columns
+                / size.rows,
+                (css_dimension(value, vertical=False, available=dom.width) or 1)
+                / (css_dimension(value, vertical=True, available=dom.height) or 1),
+            )
+        )
+
+    # elif feature == "color":
+    #     Check output color depth
+
+    else:
+        result = always
+
+    return result
 
 
 class HTML:
     """A HTML formatted text renderer.
 
     Accepts a HTML string and renders it at a given width.
     """
 
-    formatted_text: StyleAndTextTuples
-
-    def render_ol_content(
-        self,
-        element: Node,
-        left: int = 0,
-        fill: bool = True,
-        align_content: bool = True,
-    ) -> StyleAndTextTuples:
-        """Render lists, adding item numbers to child <li> elements."""
-        # Assign a list index to each item. This can be set via the 'value' attributed
-        _curr = 0
-        for item in element.find_all("li"):
-            _curr += 1
-            _curr = int(item.attrs.setdefault("value", str(_curr)))
-        # Render list as normal
-        return self.render_node_content(
-            element=element,
-            left=left,
-            fill=fill,
-            align_content=align_content,
-        )
-
-    render_ul_content = render_ol_content
-
     def __init__(
         self,
         markup: str,
-        base: UPath | str | None = None,
+        base: Path | str | None = None,
         width: int | None = None,
         height: int | None = None,
         collapse_root_margin: bool = False,
         fill: bool = True,
+        css: CssSelectors | None = None,
         browser_css: CssSelectors | None = None,
+        mouse_handler: Callable[[Node, MouseEvent], NotImplementedOrNone] | None = None,
+        paste_fixed: bool = True,
     ) -> None:
         """Initialize the markdown formatter.
 
         Args:
             markup: The markdown text to render
             base: The base url for the HTML dom
             width: The width in characters available for rendering. If :py:const:`None`
                 the terminal width will be used
             height: The width in characters available for rendering. If :py:const:`None`
                 the terminal height will be used
             collapse_root_margin: If :py:const:`True`, margins of the root element will
                 be collapsed
             fill: Whether remaining space in block elements should be filled
+            css: Base CSS to apply when rendering the HTML
             browser_css: The browser CSS to use
+            mouse_handler: A mouse handler function to use when links are clicked
+            paste_fixed: Whether fixed elements should be pasted over the output
 
         """
-        self.browser_css: CssSelectors = {
-            **(_BROWSER_CSS if browser_css is None else browser_css)
-        }
-        self.css: CssSelectors = {}
-
-        self.markup = markup
+        self.markup = markup.strip()
         self.base = UPath(base or ".")
-        self.width: int | None = None
-        self.height: int | None = None
-        self.collapse_root_margin = collapse_root_margin
+        self.title = ""
+
+        self.browser_css = browser_css or _BROWSER_CSS
+        self.css: CssSelectors = css or {}
+
+        self.render_count = 0
+        self.width = width
+        self.height = height
+
         self.fill = fill
+        self.collapse_root_margin = collapse_root_margin
+        self.paste_fixed = paste_fixed
 
-        self.parser = CustomHTMLParser(self)
+        self.mouse_handler = mouse_handler
 
-        self.element_theme_cache: SimpleCache[Hashable, dict[str, Any]] = SimpleCache()
+        self.formatted_text: StyleAndTextTuples = []
+        self.floats: dict[tuple[int, DiBool, DiInt], StyleAndTextTuples] = {}
+        self.fixed: dict[tuple[int, DiBool, DiInt], StyleAndTextTuples] = {}
+        self.fixed_mask: StyleAndTextTuples = []
+        # self.images = []
+        # self.anchors = []
 
-        # Parse the markup
-        self.soup = self.parser.parse(markup.strip())
+        self.assets_loaded = False
 
-        # Parse the styles
-        self.css.update(parse_styles(self.soup, self.base))
+    # Lazily load attributes
 
-        # Load images
+    @cached_property
+    def parser(self) -> CustomHTMLParser:
+        """Load the HTML parser."""
+        return CustomHTMLParser(self)
+
+    @cached_property
+    def soup(self) -> Node:
+        """Parse the markup."""
+        return self.parser.parse(self.markup)
+
+    def load_assets(self) -> None:
+        """Load CSS styles and image resources.
+
+        Do not touch element's themes!
+        """
         for child in self.soup.descendents:
-            if child.name == "img" and (src := child.attrs.get("src")):
-                if data := load_url(src, self.base):
-                    child.attrs["_data"] = data
+            # Set title
+            if child.name == "title":
+                if contents := child.contents:
+                    self.title = contents[0].text
+
+            # In case of a <link> style, load the url
+            elif (
+                child.name == "link"
+                and (
+                    (attrs := child.attrs).get("rel") == "stylesheet"
+                    or (attrs.get("rel") == "preload" and attrs.get("as") == "style")
+                )
+                and (href := attrs.get("href", ""))
+            ):
+                css_path = UPath(urljoin(str(self.base), href))
+                try:
+                    css_str = css_path.read_text()
+                except Exception:
+                    log.debug("Could not load file %s", css_path)
                 else:
-                    child.attrs["_missing"] = "true"
-
-        self.floats: dict[tuple[int, DiInt], StyleAndTextTuples] = {}
-        self.fixes: dict[tuple[int, DiInt], StyleAndTextTuples] = {}
+                    parse_style_sheet(css_str, self)
 
-        # Render the markup
-        self.render(width, height)
+            # In case of a <style> tab, load first child's text
+            elif child.name == "style":
+                if child.contents:
+                    # Use unprocess text attribute to avoid loading the element's theme
+                    css_str = child.contents[0]._text
+                    parse_style_sheet(css_str, self)
+
+            # Load images
+            elif child.name == "img" and (src := child.attrs.get("src")):
+                data_path = UPath(urljoin(str(self.base), src))
+                if data_path.exists():
+                    try:
+                        data = data_path.read_bytes()
+                    except Exception:
+                        log.info("Error loading file '%s'", data_path)
+                    else:
+                        if data:
+                            child.attrs["_data"] = data
+                else:
+                    child.attrs["_missing"] = "true"
 
-    def render_list_item_content(
-        self,
-        element: Node,
-        left: int = 0,
-        fill: bool = True,
-        align_content: bool = True,
-    ) -> StyleAndTextTuples:
-        """Render a list item."""
-        # Get element theme
-        theme = element.theme
-        # Get the bullet style
-        list_style = theme.list_style_type
-        bullet = list_style
-        if list_style == "decimal":
-            bullet = f"{element.attrs['value']}."
-        # Add bullet element
-        if bullet:
-            bullet_element = Node(
-                dom=self,
-                name="::marker",
-                parent=element,
-                contents=[Node(dom=self, name="text", parent=element, text=bullet)],
-            )
-            if theme.list_style_position == "inside":
-                element.contents.insert(0, bullet_element)
-            else:
-                element.marker = bullet_element
-        # Render the list item
-        ft = self.render_node_content(
-            element,
-            left=left,
-            fill=fill,
-            align_content=align_content,
-        )
-        return ft
+        self.assets_loaded = True
 
-    def render(self, width: int | None, height: int | None) -> None:
+    def render(self, width: int | None, height: int | None) -> StyleAndTextTuples:
         """Render the current markup at a given size."""
-        if not width or not height:
+        no_w = width is None and self.width is None
+        no_h = height is None and self.height is None
+        if no_w or no_h:
             size = get_app_session().output.get_size()
-        self.width = width or size.columns
-        self.height = height or size.rows
+            if no_w:
+                width = size.columns
+            if no_h:
+                height = size.rows
+        if width is not None:
+            self.width = width
+        if height is not None:
+            self.height = height
+        assert self.width is not None
+        assert self.height is not None
+
+        if not self.assets_loaded:
+            self.load_assets()
 
         ft = self.render_element(
             self.soup,
             available_width=self.width,
             available_height=self.height,
             fill=self.fill,
         )
 
-        # Draw floats
-        for (_, position), float_ft in sorted(self.floats.items()):
-            row = col = 0
-            if (top := position.top) is not None:
-                row = top
-            elif (bottom := position.bottom) is not None:
-                row = (
-                    sum(1 for _ in split_lines(ft))
-                    - sum(1 for _ in split_lines(float_ft))
-                    - bottom
-                )
-            if (left := position.left) is not None:
-                col = left
-            elif (right := position.right) is not None:
-                row = max_line_width(ft) - max_line_width(float_ft) - right
-
-            ft = paste(ft, float_ft, row, col)
-
         # Apply "ReverseOverwrite"s
         ft = apply_reverse_overwrites(ft)
 
+        # Apply floats and fixed elements
+
+        def _paste_floats(
+            floats: dict[tuple[int, DiBool, DiInt], StyleAndTextTuples],
+            lower_ft: StyleAndTextTuples,
+        ) -> StyleAndTextTuples:
+            """Paste floats on top of rendering."""
+            lower_ft_height = None
+            for (_, anchors, position), float_ft in sorted(floats.items()):
+                row = col = 0
+                if anchors.top:
+                    row = position.top
+                elif anchors.bottom:
+                    if lower_ft_height is None:
+                        lower_ft_height = sum(1 for _ in split_lines(lower_ft))
+                    row = (
+                        lower_ft_height
+                        - sum(1 for _ in split_lines(float_ft))
+                        - position.bottom
+                    )
+                if anchors.left:
+                    col = position.left
+                elif anchors.right:
+                    row = (
+                        max_line_width(lower_ft)
+                        - max_line_width(float_ft)
+                        - position.right
+                    )
+                lower_ft = paste(float_ft, lower_ft, row, col)
+            return lower_ft
+
+        # Draw floats
+        if self.floats:
+            ft = _paste_floats(self.floats, ft)
+
+        # Paste floats onto a mask, then onto the rendering if required
+        if self.fixed:
+            assert self.width is not None
+            assert self.height is not None
+            fixed_mask = cast(
+                "StyleAndTextTuples", [("", (" " * self.width) + "\n")] * self.height
+            )
+            fixed_mask = _paste_floats(self.fixed, fixed_mask)
+            fixed_mask = apply_reverse_overwrites(fixed_mask)
+            if self.paste_fixed:
+                ft = paste(fixed_mask, ft, 0, 0, transparent=True)
+            self.fixed_mask = fixed_mask
+        else:
+            self.fixed_mask = []
+
+        self.render_count += 1
         self.formatted_text = ft
 
+        return ft
+
     def render_element(
         self,
         element: Node,
         available_width: int,
         available_height: int,
         left: int = 0,
         fill: bool = True,
@@ -2512,22 +3132,79 @@
             if parent_theme := element.theme.parent_theme:
                 style = parent_theme.style
             else:
                 style = ""
             ft = [(style, text)]
         return ft
 
+    def render_ol_content(
+        self,
+        element: Node,
+        left: int = 0,
+        fill: bool = True,
+        align_content: bool = True,
+    ) -> StyleAndTextTuples:
+        """Render lists, adding item numbers to child <li> elements."""
+        # Assign a list index to each item. This can be set via the 'value' attributed
+        _curr = 0
+        for item in element.find_all("li"):
+            _curr += 1
+            _curr = int(item.attrs.setdefault("value", str(_curr)))
+        # Render list as normal
+        return self.render_node_content(
+            element=element,
+            left=left,
+            fill=fill,
+            align_content=align_content,
+        )
+
+    render_ul_content = render_ol_content
+
+    def render_list_item_content(
+        self,
+        element: Node,
+        left: int = 0,
+        fill: bool = True,
+        align_content: bool = True,
+    ) -> StyleAndTextTuples:
+        """Render a list item."""
+        # Get element theme
+        theme = element.theme
+        # Get the bullet style
+        list_style = theme.list_style_type
+        bullet = list_style
+        if list_style == "decimal":
+            bullet = f"{element.attrs['value']}."
+        # Add bullet element
+        if bullet:
+            bullet_element = Node(dom=self, name="::marker", parent=element)
+            bullet_element.contents.append(
+                Node(dom=self, name="text", parent=bullet_element, text=bullet)
+            )
+            if theme.list_style_position == "inside":
+                element.contents.insert(0, bullet_element)
+            else:
+                element.marker = bullet_element
+        # Render the list item
+        ft = self.render_node_content(
+            element,
+            left=left,
+            fill=fill,
+            align_content=align_content,
+        )
+        return ft
+
     def render_table_content(
         self,
         element: Node,
         left: int = 0,
         fill: bool = True,
         align_content: bool = True,
     ) -> StyleAndTextTuples:
-        """Render a list of parsed markdown elements representing a table element.
+        """Render a HTML table element.
 
         Args:
             element: The list of parsed elements to render
             left: The position on the current line at which to render the output - used
                 to indent subsequent lines when rendering inline blocks like images
             fill: Whether to fill the remainder of the rendered space with whitespace
             align_content: Whether to align the element's content
@@ -2538,15 +3215,15 @@
         """
         ft = []
 
         table_theme = element.theme
         table_x_dim = Dimension(
             min=table_theme.min_width,
             preferred=table_theme.content_width if "width" in table_theme else None,
-            max=table_theme.max_width or table_theme.available_width,
+            max=table_theme.max_width or table_theme.content_width,
         )
         table = Table(
             align=table_theme.text_align,
             style=table_theme.style,
             border_line=table_theme.border_line,
             border_style=table_theme.border_style,
             padding=DiInt(0, 0, 0, 0),
@@ -2575,15 +3252,14 @@
                             td_theme.update_space(
                                 table_theme.content_width
                                 or table_theme.available_width,
                                 table_theme.content_height
                                 or table_theme.available_width,
                             )
                             cell = row.new_cell(
-                                # text=" ",
                                 text=self.render_node_content(
                                     td,
                                     left=0,
                                     align_content=False,
                                     fill=False,
                                 ),
                                 padding=td_theme.padding,
@@ -2606,26 +3282,27 @@
         for child in element.find_all("tbody", recursive=False):
             render_rows(child.contents)
         # Render rows not in a head / body / foot as part of the body
         render_rows(element.contents)
         for child in element.find_all("tfoot", recursive=False):
             render_rows(child.contents)
 
+        # TODO - process <colgroup> elements
+
         # Add cell contents
         if td_map:
             col_widths = table.calculate_col_widths()
-
             for row in table.rows:
                 for col_width, cell in zip(col_widths, row.cells):
                     if td := td_map.get(cell):
                         cell_padding = compute_padding(cell)
                         available_width = (
-                            (table_x_dim.max if cell.colspan > 1 else col_width)
-                            - cell_padding.left
-                            - cell_padding.right
+                            table_x_dim.max
+                            if cell.colspan > 1
+                            else col_width - cell_padding.left - cell_padding.right
                         )
                         td.theme.update_space(
                             available_width, table_theme.available_height
                         )
                         cell.text = self.render_node_content(
                             td,
                             # TODO - get actual colspan cell widths properly
@@ -2663,17 +3340,17 @@
         align_content: bool = True,
     ) -> StyleAndTextTuples:
         """Render an image's content."""
         theme = element.theme
         content_width = theme.content_width
         # content_height = theme.content_height
         src = str(element.attrs.get("src", ""))
-        path = UPath(src)
+        path = self.base / src
 
-        if data := element.attrs.get("_data"):
+        if not element.attrs.get("_missing") and (data := element.attrs.get("_data")):
             # Display it graphically
             format_ = get_format(path, default="png")
             cols, aspect = pixels_to_cell_size(*data_pixel_size(data, format_=format_))
             # Manually set a value if we don't have one
             cols = cols or 20
             aspect = aspect or 0.5
             # Scale down the image to fit to width
@@ -2684,37 +3361,41 @@
             ft = (
                 convert(
                     data,
                     from_=format_,
                     to="formatted_text",
                     cols=cols,
                     rows=rows,
+                    fg=theme.color,
                     bg=theme.background_color,
                     path=path,
                 )
                 or []
             )
             # Remove trailing new-lines
             ft = strip(ft, chars="\n", left=False)
             # Set default background color on generated content
             ft = [(f"{theme.style} {x[0]}", *x[1:]) for x in ft]
 
         else:
-            ft = []
-
-            if (alt := element.attrs.get("alt")) != "":
-                style = f"class:image,placeholder {theme.style}"
-                ft.append((style, "🌄"))
-                if content_width and content_width >= 7:
-                    ft.extend(
-                        [
-                            (style, " "),
-                            (style, (alt or (path.name if path else "Image"))),
-                        ]
-                    )
+            style = f"class:image,placeholder {theme.style}"
+            ft = [(style, "🌄")]
+            if content_width and content_width >= 7:
+                ft.extend(
+                    [
+                        (style, " "),
+                        (
+                            style,
+                            (
+                                element.attrs.get("alt")
+                                or (path.name if path else "Image")
+                            ),
+                        ),
+                    ]
+                )
 
         return ft
 
     def render_svg_content(
         self,
         element: Node,
         left: int = 0,
@@ -2722,20 +3403,31 @@
         align_content: bool = True,
     ) -> StyleAndTextTuples:
         """Display images rendered as ANSI art."""
         theme = element.theme
         # HTMLParser clobber the case of element attributes
         # We fix the SVG viewBox here
         data = element._outer_html().replace(" viewbox=", " viewBox=")
-        # Render the image
+        # Display it graphically
+        cols, aspect = pixels_to_cell_size(*data_pixel_size(data, format_="svg"))
+        # Scale down the image to fit to width
+        if content_width := theme.content_width:
+            if cols == 0:
+                cols = content_width
+            else:
+                cols = min(content_width, cols)
+        rows = int(cols * aspect)
+        # Convert the image to formatted-text
         ft = convert(
             data=data,
             from_="svg",
             to="formatted_text",
-            cols=theme.content_width,
+            cols=cols,
+            rows=rows or None,
+            fg=theme.color,
             bg=theme.background_color,
         )
         # Remove trailing new-lines
         ft = strip(ft, chars="\n", left=False)
         # Set default background color on generated content
         ft = [(f"{theme.style} {x[0]}", *x[1:]) for x in ft]
         return ft
@@ -2751,35 +3443,25 @@
         attrs = element.attrs
         element.contents.insert(
             0,
             Node(
                 dom=self,
                 name="text",
                 parent=element,
-                text=attrs.get("value", attrs.get("placeholder", "")),
+                text=attrs.get("value", attrs.get("placeholder", " ")) or " ",
             ),
         )
         ft = self.render_node_content(
             element,
             left=left,
             fill=fill,
             align_content=align_content,
         )
         return ft
 
-    def render_br_content(
-        self,
-        element: Node,
-        left: int = 0,
-        fill: bool = True,
-        align_content: bool = True,
-    ) -> StyleAndTextTuples:
-        """Render line breaks."""
-        return [("", "\n")]
-
     def render_node_content(
         self,
         element: Node,
         left: int = 0,
         fill: bool = True,
         align_content: bool = True,
     ) -> StyleAndTextTuples:
@@ -2790,95 +3472,107 @@
         ft_middle: StyleAndTextTuples
         ft_right: StyleAndTextTuples
         empty: StyleAndTextTuples = []
 
         line_height = 1
         baseline = 0
 
-        # Add "::before"  and "::after" nodes
-        # TODO - do we have to do this for every element?
-        for name, pos in (("::before", 0), ("::after", 1)):
-            if not element.name.startswith("::"):
-                content_node = Node(dom=element.dom, name=name, parent=element)
-                if text := content_node.theme.get("content", "").strip('"'):
-                    content_node.contents.append(
-                        Node(
-                            dom=element.dom, name="text", parent=content_node, text=text
-                        )
-                    )
-                    element.contents.insert(pos * len(element.contents), content_node)
-
         parent_theme = element.theme
 
         d_blocky = d_inline = d_inline_block = False
 
         float_lines_left: list[StyleAndTextTuples] = []
         float_width_left = 0
         float_lines_right: list[StyleAndTextTuples] = []
         float_width_right = 0
 
         content_width = parent_theme.content_width
 
-        new_line = []
+        new_line: StyleAndTextTuples = []
+
+        def flush() -> None:
+            """Add the current line to the rendered output."""
+            nonlocal new_line, ft, left, line_height, baseline
+            if new_line:
+                # Pad the new-line to form an alignable block
+                new_line = pad(new_line, style=parent_theme.style)
+                if ft:
+                    # Combine with the output
+                    ft = join_lines([ft, new_line]) if ft else new_line
+                else:
+                    ft = new_line
+            # Reset the new line
+            left = 0
+            line_height = 1
+            baseline = 0
+            new_line = []
 
         # Render each child node
-        for child in element.contents:
+        for child in element.renderable_descendents:
             theme = child.theme
 
             if theme.skip:
                 continue
 
+            # Start a new line if we encounter a <br> element
+            if child.name == "br":
+                flush()
+                continue
+
             # We will start a new line if the previous item was a block
             if ft and d_blocky and last_char(ft) != "\n":
                 line_height = 1
                 left = 0
                 baseline = 0
 
             d_blocky = theme.d_blocky
             d_inline = theme.d_inline
             d_inline_block = theme.d_inline_block
+            preformatted = theme.preformatted
+
+            available_width = parent_theme.content_width
+            available_height = parent_theme.content_height
 
             # Render the element
             rendering = self.render_element(
                 child,
-                available_width=parent_theme.content_width,
-                available_height=parent_theme.content_height,
+                available_width=available_width,
+                available_height=available_height,
                 left=0 if d_blocky or d_inline_block else left,
                 fill=fill,
                 align_content=align_content,
             )
 
             # If the rendering was empty, move on
             if not rendering:
                 continue
 
             # If the rendering was a positioned absolutely or fixed, store it and draw it later
             if theme.theme["position"] == "fixed":
-                # self.fixes[(theme.z_index, theme.position)] = rendering
-                self.floats[(theme.z_index, theme.position)] = rendering
+                self.fixed[(theme.z_index, theme.anchors, theme.position)] = rendering
 
             # if theme.theme["position"] == "absolute":
-            # self.floats[(theme.z_index, theme.position)] = rendering
+            #     self.floats[(theme.z_index, theme.anchors, theme.position)] = rendering
 
             # if theme.theme["position"] == "relative":
             # ... TODO ..
 
-            elif theme.theme["float"] == "right":
+            elif theme.floated == "right":
                 lines = []
                 for ft_left, ft_right in zip_longest(
                     split_lines(pad(rendering, style=theme.style)),
                     float_lines_right,
                     fillvalue=empty,
                 ):
                     lines.append([*ft_left, *ft_right])
                 float_lines_right = lines
                 float_width_right = fragment_list_width(float_lines_right[0])
                 continue
 
-            elif theme.theme["float"] == "left":
+            elif theme.floated == "left":
                 lines = []
                 for ft_left, ft_right in zip_longest(
                     lines,
                     split_lines(pad(rendering, style=theme.style)),
                     fillvalue=empty,
                 ):
                     lines.append([*ft_left, *ft_right])
@@ -2887,47 +3581,53 @@
                 continue
 
             # If the rendering was inline, add it to the end of the last line of the
             # current output. This might involve re-aligning the last line in the
             # output, which could have been an inline-block
 
             elif d_inline and (
+                # parent_theme.d_inline or parent_theme.d_inline_block or preformatted
                 parent_theme.d_inline
-                or parent_theme.d_inline_block
-                or theme.preformatted
+                or preformatted
             ):
                 new_line.extend(rendering)
 
             elif d_inline or d_inline_block:
                 if d_inline:
-                    tokens = fragment_list_to_words(rendering)
+                    tokens = list(fragment_list_to_words(rendering))
                 else:
                     tokens = [rendering]
 
-                tokens = list(tokens)
-
                 for token in tokens:
                     token_lines = list(split_lines(token))
                     token_width = max(fragment_list_width(line) for line in token_lines)
                     token_height = len(token_lines)
 
+                    # Deal with floats
+
                     float_width_right = (
                         fragment_list_width(float_lines_right[0])
                         if float_lines_right
                         else 0
                     )
                     float_width_left = (
                         fragment_list_width(float_lines_left[0])
                         if float_lines_left
                         else 0
                     )
 
+                    # If we have floats, transform the current new line and add one row
+                    # from each active float
                     if (
-                        content_width - float_width_left - float_width_right
-                    ) - left - token_width < 0:
+                        new_line
+                        and (content_width - float_width_left - float_width_right)
+                        - left
+                        - token_width
+                        < 0
+                    ):
                         new_rows = list(split_lines(new_line))
                         new_line_width = max(
                             fragment_list_width(line) for line in new_rows
                         )
 
                         transformed_rows = []
                         for ft_left, ft_middle, ft_right in zip_longest(
@@ -2953,35 +3653,39 @@
                                 [
                                     *ft_left,
                                     *align(
                                         ft_middle,
                                         how=parent_theme.text_align,
                                         width=line_width,
                                         style=parent_theme.style,
+                                        placeholder="",
                                     ),
                                     *ft_right,
                                 ]
                             )
 
-                        ft = join_lines([ft, *transformed_rows]) if ft else new_line
-
                         float_lines_left = float_lines_left[line_height:]
                         float_lines_right = float_lines_right[line_height:]
 
+                        # Manually flush the transformed lines
+                        if ft:
+                            ft = join_lines([ft, *transformed_rows])
+                        else:
+                            ft = join_lines(transformed_rows)
+                        baseline = 0
                         new_rows = [[]]
-                        new_line = []
-                        line_height = 1
                         left = 0
-                        baseline = 0
+                        line_height = 1
+                        new_line = []
 
                     if line_height == token_height == 1 or not new_line:
                         new_line.extend(token)
                         new_rows = [new_line]
                         baseline = int(theme.vertical_align * (token_height - 1))
-
+                        line_height = max(line_height, token_height)
                     else:
                         new_line, baseline = concat(
                             ft_a=new_line,
                             ft_b=token,
                             baseline_a=baseline,
                             baseline_b=int(theme.vertical_align * (token_height - 1)),
                             style=parent_theme.style,
@@ -2991,17 +3695,15 @@
 
                     left += token_width
 
             # Otherwise we are rendering a block-like element, which gets added to the
             # end of the output
             else:
                 # Flush the latest line
-                if new_line:
-                    ft = join_lines([ft, new_line]) if ft else new_line
-                    new_line = []
+                flush()
                 # Start block elements on a new line
                 if ft and d_blocky and last_char(ft) != "\n":
                     ft.append(("", "\n"))
 
                 ft.extend(rendering)
 
                 # line_height = len(list(split_lines(rendering)))
@@ -3041,23 +3743,23 @@
                 row = [
                     *ft_left,
                     *align(
                         ft_middle,
                         how=parent_theme.text_align,
                         width=line_width,
                         style=parent_theme.style + " nounderline",
+                        placeholder="",
                     ),
                     *ft_right,
                 ]
                 ft = join_lines([ft, row]) if ft else row
             new_line = []
 
         # Flush any current lines
-        if new_line:
-            ft = join_lines([ft, new_line]) if ft else new_line
+        flush()
 
         # Draw flex elements
         # if parent_theme.get("flex") and parent_theme.get("flex-direction") == "column":
         # table = Table(border=Invisible, collapse_empty_borders=True)
         # row = table.new_row()
         # for output in outputs:
         # row.new_cell(output)
@@ -3088,80 +3790,100 @@
         content_width = theme.content_width
         content_height = theme.content_height
 
         # Apply style to inline elements
         if d_inline:
             ft = apply_style(ft, theme.style)
 
-        # Remove trailing newline from the contents of pre-formatted elements
-        if preformatted and (
-            (parent_theme and not parent_theme.preformatted) or d_blocky
-        ):
-            ft = strip_one_trailing_newline(ft)
-
         # If an element should not overflow it's width / height, truncate it
         if not d_inline and not preformatted:
             if theme.get("overflow_x") == "hidden":
                 ft = truncate(ft, content_width, placeholder="", ignore_whitespace=True)
             elif theme.get("overflow_x") == "auto":
                 ft = truncate(
                     ft,
                     content_width,
                     placeholder="▹",
                     ignore_whitespace=True,
                     style=theme.style,
                 )
             else:
                 ft = truncate(
-                    ft, content_width, ignore_whitespace=True, style=theme.style
+                    ft,
+                    content_width,
+                    placeholder="",
+                    ignore_whitespace=True,
+                    style=theme.style,
                 )
 
-        if theme.get("overflow_y") in {"hidden", "auto"}:
-            lines = []
-            for i, line in enumerate(split_lines(ft)):
-                if i <= content_height:
-                    lines.append(line)
-            ft = join_lines(lines)
+        # Truncate or expand the height
+        overflow_y = theme.get("overflow_y") in {"hidden", "auto"}
+        pad_height = d_blocky and theme.height is not None
+        if overflow_y or pad_height:
+            target_height = None
+            if (min_height := theme.min_height) and min_height > content_height:
+                target_height = min_height
+            if (max_height := theme.max_height) and max_height < content_height:
+                target_height = max_height
+            elif height := theme.height:
+                target_height = height
+
+            if target_height is not None:
+                # Truncate elements with hidden overflows
+                if overflow_y:
+                    lines = []
+                    for i, line in enumerate(split_lines(ft)):
+                        if i <= target_height:
+                            lines.append(line)
+                else:
+                    lines = list(split_lines(ft))
+
+                # Pad height of block elements to theme height
+                if pad_height and len(lines) < target_height:
+                    lines.extend([[]] * (target_height - len(lines)))
+
+                ft = join_lines(lines)
 
         # Align content
-        if align_content and (d_blocky or d_inline_block):
+        if align_content and d_blocky:
             alignment = theme.text_align
-
             if alignment != FormattedTextAlign.LEFT:
                 ft = align(
                     ft,
                     alignment,
                     width=None if d_inline_block else content_width,
                     style=theme.style,
                     ignore_whitespace=True,
+                    placeholder="",
                 )
 
         # # Fill space around block elements so they fill the content width
-        if ft and (fill and d_blocky) or d_inline_block:
+        if ft and ((fill and d_blocky and not theme.d_table) or d_inline_block):
             pad_width = None
             if d_blocky:
                 pad_width = content_width
             elif d_inline_block:
                 if theme.width is None:
                     pad_width = max_line_width(ft)
                 else:
                     pad_width = content_width
+            style = theme.style
             ft = pad(
                 ft,
                 width=pad_width,
                 char=" ",
-                style=theme.style,
+                style=style,
             )
 
         # Use the rendered content width from now on for inline elements
         if d_inline_block or d_inline:
             content_width = max_line_width(ft)
 
         # Add padding & border
-        if d_blocky or d_inline_block or d_inline:
+        if d_blocky or d_inline_block:
             padding = theme.padding
             border_visibility = theme.border_visibility
             if (any(padding) or any(border_visibility)) and not (
                 theme.d_table and theme.border_collapse
             ):
                 ft = add_border(
                     ft,
@@ -3169,14 +3891,41 @@
                     border_grid=theme.border_grid,
                     width=content_width if not ft else None,
                     border_visibility=border_visibility,
                     border_style=theme.border_style,
                     padding=padding,
                 )
 
+        # Draw borders and padding on text inside inline elements
+        elif element.name == "text":
+            padding = theme.padding
+            border_visibility = theme.border_visibility
+            if (
+                padding.left
+                or padding.right
+                or border_visibility.left
+                or border_visibility.right
+            ):
+                if not element.is_first_child_node:
+                    border_visibility = border_visibility._replace(left=False)
+                    padding = padding._replace(left=0)
+                if not element.is_last_child_node:
+                    border_visibility = border_visibility._replace(right=False)
+                    padding = padding._replace(right=0)
+                if any(padding) or any(border_visibility):
+                    ft = add_border(
+                        ft,
+                        style=f"{theme.style} nounderline",
+                        border_grid=theme.border_grid,
+                        width=content_width if not ft else None,
+                        border_visibility=border_visibility,
+                        border_style=theme.border_style,
+                        padding=padding,
+                    )
+
         # The "::marker" element is drawn in the margin, before any padding
         # If the element has no margin, it can end up in the parent's padding
         # We use [ReverseOverwrite] fragments to ensure the marker is ignored
         # now and written over the margin later.
         if element.marker is not None:
             marker_ft = self.render_element(
                 element.marker,
@@ -3190,65 +3939,90 @@
                 *apply_style(marker_ft, "[ReverseOverwrite]"),
                 *ft,
             ]
 
         parent_style = parent_theme.style if parent_theme else ""
 
         # Render the margin
-        if d_blocky and theme.margin_auto:
+        # if d_blocky and (alignment := theme.block_align) != FormattedTextAlign.LEFT:
+        if (alignment := theme.block_align) != FormattedTextAlign.LEFT:
             # Center block contents if margin_left and margin_right are "auto"
             ft = align(
                 ft,
-                how=FormattedTextAlign.CENTER,
+                how=alignment,
                 width=theme.available_width,
                 style=parent_style,
+                placeholder="",
             )
 
         elif any(margin := theme.margin):
             ft = add_border(
                 ft=ft,
                 style=f"{parent_style} nounderline",
                 border_visibility=DiBool.from_value(False),
                 padding=margin,
                 padding_style=parent_style,
             )
 
         # Ensure hidden content is blank and styled like the parent
         if theme.hidden:
-            ft = [
-                (
-                    parent_style,
-                    "\n".join([" " * len(x) for x in text.split("\n")]),
-                )
-                for style, text, *_ in ft
-            ]
+            ft = cast(
+                "StyleAndTextTuples",
+                [
+                    (
+                        parent_style,
+                        "\n".join([" " * len(x) for x in text.split("\n")]),
+                        *rest,
+                    )
+                    for style, text, *rest in ft
+                ],
+            )
+
+        # Apply mouse handler to links
+        if (
+            (parent := element.parent)
+            and parent.name == "a"
+            and callable(handler := self.mouse_handler)
+            and (href := parent.attrs.get("href"))
+        ):
+            element.attrs["_link_path"] = self.base / href
+            ft = cast(
+                "StyleAndTextTuples",
+                [
+                    (style, text, *(rest or [partial(handler, element)]))
+                    for style, text, *rest in ft
+                ],
+            )
 
         return ft
 
     def __pt_formatted_text__(self) -> StyleAndTextTuples:
         """Return formatted text."""
+        if not self.formatted_text:
+            self.render(width=None, height=None)
         return self.formatted_text
 
 
 if __name__ == "__main__":
     import sys
 
     from prompt_toolkit.application.current import create_app_session, set_app
     from prompt_toolkit.shortcuts.utils import print_formatted_text
     from prompt_toolkit.styles.style import Style
 
     from euporie.core.app import BaseApp
+    from euporie.core.path import parse_path
     from euporie.core.style import HTML_STYLE
 
-    path = UPath(sys.argv[1])
+    path = parse_path(sys.argv[1])
 
     with create_app_session(input=BaseApp.load_input(), output=BaseApp.load_output()):
         with set_app(BaseApp()):
-            with path.open() as f:
-                html = HTML(
-                    path.open().read(),
+            print_formatted_text(
+                HTML(
+                    path.read_text(),
                     base=path,
                     collapse_root_margin=False,
                     fill=True,
-                )
-
-                print_formatted_text(html, style=Style(HTML_STYLE))
+                ),
+                style=Style(HTML_STYLE),
+            )
```

### Comparing `euporie-2.3.2/euporie/core/formatted_text/markdown.py` & `euporie-2.4.0/euporie/core/formatted_text/markdown.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,176 +1,187 @@
 """Contain the browser CSS for formatting markdown."""
 
+from prompt_toolkit.filters.utils import _always
+
 from .html import CssSelector
 
 _MARKDOWN_CSS = {
-    (
-        (CssSelector(item="h1"),),
-        (CssSelector(item="h2"),),
-        (CssSelector(item="h3"),),
-        (CssSelector(item="h4"),),
-        (CssSelector(item="h5"),),
-        (CssSelector(item="h6"),),
-    ): {
-        "text_align": "center",
-    },
-    ((CssSelector(item="h1"),),): {
-        "font_weight": "bold",
-        "text_decoration": "underline",
-        "border_top_style": "double",
-        "border_right_style": "double",
-        "border_bottom_style": "double",
-        "border_left_style": "double",
-        "border_top_width": "0.34em",
-        "border_right_width": "0.34em",
-        "border_bottom_width": "0.34em",
-        "border_left_width": "0.34em",
-        "border_top_color": "ansiyellow",
-        "border_right_color": "ansiyellow",
-        "border_bottom_color": "ansiyellow",
-        "border_left_color": "ansiyellow",
-    },
-    ((CssSelector(item="h2"),),): {
-        "font_weight": "bold",
-        "border_top_style": "solid",
-        "border_right_style": "solid",
-        "border_bottom_style": "solid",
-        "border_left_style": "solid",
-        "border_top_width": "0.34em",
-        "border_right_width": "0.34em",
-        "border_bottom_width": "0.34em",
-        "border_left_width": "0.34em",
-        "border_top_color": "#888888",
-        "border_right_color": "#888888",
-        "border_bottom_color": "#888888",
-        "border_left_color": "#888888",
-    },
-    ((CssSelector(item="h3"),),): {
-        "font_weight": "bold",
-        "font_style": "italic",
-        "border_top_style": "solid",
-        "border_right_style": "solid",
-        "border_bottom_style": "solid",
-        "border_left_style": "solid",
-        "border_top_width": "0.1em",
-        "border_right_width": "0.1em",
-        "border_bottom_width": "0.1em",
-        "border_left_width": "0.1em",
-        "border_top_color": "#888888",
-        "border_right_color": "#888888",
-        "border_bottom_color": "#888888",
-        "border_left_color": "#888888",
-        "margin_left": "auto",
-        "margin_right": "auto",
-        "padding_left": "1em",
-        "padding_right": "1em",
-    },
-    ((CssSelector(item="h4"),),): {
-        "text_weight": "bold",
-        "text_decoration": "underline",
-        "margin_top": "1rem",
-        "margin_bottom": "1rem",
-    },
-    ((CssSelector(item="h5"),),): {
-        "font_weight": "bold",
-        "margin_top": "1rem",
-        "margin_bottom": "1rem",
-    },
-    ((CssSelector(item="h6"),),): {
-        "font_style": "italic",
-        "margin_top": "1rem",
-        "margin_bottom": "1rem",
-    },
-    (
+    _always: {
+        (
+            (CssSelector(item="h1"),),
+            (CssSelector(item="h2"),),
+            (CssSelector(item="h3"),),
+            (CssSelector(item="h4"),),
+            (CssSelector(item="h5"),),
+            (CssSelector(item="h6"),),
+        ): {
+            "text_align": "center",
+        },
+        ((CssSelector(item="h1"),),): {
+            "font_weight": "bold",
+            "text_decoration": "underline",
+            "border_top_style": "double",
+            "border_right_style": "double",
+            "border_bottom_style": "double",
+            "border_left_style": "double",
+            "border_top_width": "0.34em",
+            "border_right_width": "0.34em",
+            "border_bottom_width": "0.34em",
+            "border_left_width": "0.34em",
+            "border_top_color": "ansiyellow",
+            "border_right_color": "ansiyellow",
+            "border_bottom_color": "ansiyellow",
+            "border_left_color": "ansiyellow",
+            "padding_bottom": "0",
+        },
+        ((CssSelector(item="h2"),),): {
+            "font_weight": "bold",
+            "border_top_style": "solid",
+            "border_right_style": "solid",
+            "border_bottom_style": "solid",
+            "border_left_style": "solid",
+            "border_top_width": "0.34em",
+            "border_right_width": "0.34em",
+            "border_bottom_width": "0.34em",
+            "border_left_width": "0.34em",
+            "border_top_color": "#888888",
+            "border_right_color": "#888888",
+            "border_bottom_color": "#888888",
+            "border_left_color": "#888888",
+            "padding_bottom": "0",
+        },
+        ((CssSelector(item="h3"),),): {
+            "font_weight": "bold",
+            "font_style": "italic",
+            "border_top_style": "solid",
+            "border_right_style": "solid",
+            "border_bottom_style": "solid",
+            "border_left_style": "solid",
+            "border_top_width": "0.1em",
+            "border_right_width": "0.1em",
+            "border_bottom_width": "0.1em",
+            "border_left_width": "0.1em",
+            "border_top_color": "#888888",
+            "border_right_color": "#888888",
+            "border_bottom_color": "#888888",
+            "border_left_color": "#888888",
+            "margin_left": "auto",
+            "margin_right": "auto",
+            "padding_top": "0",
+            "padding_right": "1em",
+            "padding_bottom": "0",
+            "padding_left": "1em",
+        },
+        ((CssSelector(item="h4"),),): {
+            "text_weight": "bold",
+            "text_decoration": "underline",
+            "border_bottom_color": "#888888",
+            "margin_top": "1rem",
+            "margin_bottom": "1rem",
+        },
+        ((CssSelector(item="h5"),),): {
+            "font_weight": "bold",
+            "border_bottom_color": "#888888",
+            "margin_top": "1rem",
+            "margin_bottom": "1rem",
+        },
+        ((CssSelector(item="h6"),),): {
+            "font_style": "italic",
+            "border_bottom_color": "#888888",
+            "margin_top": "1rem",
+            "margin_bottom": "1rem",
+        },
         (
-            CssSelector(item="ol"),
-            CssSelector(item="li"),
-            CssSelector(item="::marker"),
-        ),
-    ): {"color": "ansicyan"},
-    (
+            (
+                CssSelector(item="ol"),
+                CssSelector(item="li"),
+                CssSelector(item="::marker"),
+            ),
+        ): {"color": "ansicyan"},
         (
-            CssSelector(item="ul"),
-            CssSelector(item="li"),
-            CssSelector(item="::marker"),
-        ),
-    ): {"color": "ansiyellow"},
-    ((CssSelector(item="blockquote"),),): {
-        "margin_top": "1em",
-        "margin_bottom": "1em",
-        "padding_left": "1em",
-        "border_left_width": "thick",
-        "border_left_style": "solid",
-        "border_left_color": "darkmagenta",
-    },
-    ((CssSelector(item=".block"),),): {"display": "block"},
-    ((CssSelector(item="td"),),): {
-        "display": "table-cell",
-        "border_top_style": "solid",
-        "border_right_style": "solid",
-        "border_bottom_style": "solid",
-        "border_left_style": "solid",
-        "border_top_width": "0.1em",
-        "border_right_width": "0.1em",
-        "border_bottom_width": "0.1em",
-        "border_left_width": "0.1em",
-        "padding_left": "1em",
-        "padding_right": "1em",
-        # "_pt_class": "markdown,table,border",
-    },
-    ((CssSelector(item="th"),),): {
-        "display": "table-cell",
-        "border_top_style": "solid",
-        "border_right_style": "solid",
-        "border_bottom_style": "solid",
-        "border_left_style": "solid",
-        "border_top_width": "0.34em",
-        "border_right_width": "0.34em",
-        "border_bottom_width": "0.34em",
-        "border_left_width": "0.34em",
-        "padding_left": "1em",
-        "padding_right": "1em",
-        "font_weight": "bold",
-        # "_pt_class": "markdown,table,border",
-    },
-    ((CssSelector(item="code"),),): {
-        "display": "inline",
-        "_pt_class": "markdown,code",
-    },
-    ((CssSelector(item=".math"),),): {"text_transform": "latex"},
-    ((CssSelector(item=".block"),),): {"display": "block"},
-    ((CssSelector(item=".math.block"),),): {
-        "text_align": "center",
-    },
-    (
+            (
+                CssSelector(item="ul"),
+                CssSelector(item="li"),
+                CssSelector(item="::marker"),
+            ),
+        ): {"color": "ansiyellow"},
+        ((CssSelector(item="blockquote"),),): {
+            "margin_top": "1em",
+            "margin_bottom": "1em",
+            "padding_left": "1em",
+            "border_left_width": "thick",
+            "border_left_style": "solid",
+            "border_left_color": "darkmagenta",
+        },
+        ((CssSelector(item=".block"),),): {"display": "block"},
+        ((CssSelector(item="td"),),): {
+            "display": "table-cell",
+            "border_top_style": "solid",
+            "border_right_style": "solid",
+            "border_bottom_style": "solid",
+            "border_left_style": "solid",
+            "border_top_width": "0.1em",
+            "border_right_width": "0.1em",
+            "border_bottom_width": "0.1em",
+            "border_left_width": "0.1em",
+            "padding_left": "1em",
+            "padding_right": "1em",
+            # "_pt_class": "markdown,table,border",
+        },
+        ((CssSelector(item="th"),),): {
+            "display": "table-cell",
+            "border_top_style": "solid",
+            "border_right_style": "solid",
+            "border_bottom_style": "solid",
+            "border_left_style": "solid",
+            "border_top_width": "0.34em",
+            "border_right_width": "0.34em",
+            "border_bottom_width": "0.34em",
+            "border_left_width": "0.34em",
+            "padding_left": "1em",
+            "padding_right": "1em",
+            "font_weight": "bold",
+            # "_pt_class": "markdown,table,border",
+        },
+        ((CssSelector(item="code"),),): {
+            "display": "inline",
+            "_pt_class": "markdown,code",
+        },
+        ((CssSelector(item=".math"),),): {"text_transform": "latex"},
+        ((CssSelector(item=".block"),),): {"display": "block"},
+        ((CssSelector(item=".math.block"),),): {
+            "text_align": "center",
+        },
         (
-            CssSelector(item="pre"),
-            CssSelector(comb=">", item="code"),
-        ),
-    ): {
-        "display": "block",
-        "border_top_style": "solid",
-        "border_top_width": "1px",
-        "border_right_style": "solid",
-        "border_right_width": "1px",
-        "border_bottom_style": "solid",
-        "border_bottom_width": "1px",
-        "border_left_style": "solid",
-        "border_left_width": "1px",
-        "_pt_class": "markdown,code,block",
-    },
-    (
+            (
+                CssSelector(item="pre"),
+                CssSelector(comb=">", item="code"),
+            ),
+        ): {
+            "display": "block",
+            "border_top_style": "solid",
+            "border_top_width": "1px",
+            "border_right_style": "solid",
+            "border_right_width": "1px",
+            "border_bottom_style": "solid",
+            "border_bottom_width": "1px",
+            "border_left_style": "solid",
+            "border_left_width": "1px",
+            "_pt_class": "markdown,code,block",
+        },
         (
-            CssSelector(item="pre"),
-            CssSelector(comb=">", item="code"),
-            CssSelector(item="*"),
-        ),
-    ): {
-        "pt_class": "markdown,code,block",
-    },
-    ((CssSelector(item="img"),), (CssSelector(item="svg"),)): {
-        "display": "inline-block",
-        "overflow_x": "hidden",
-        "overflow_y": "hidden",
-        "vertical_align": "middle",
-    },
+            (
+                CssSelector(item="pre"),
+                CssSelector(comb=">", item="code"),
+                CssSelector(item="*"),
+            ),
+        ): {
+            "pt_class": "markdown,code,block",
+        },
+        ((CssSelector(item="img"),), (CssSelector(item="svg"),)): {
+            "display": "inline-block",
+            "overflow_x": "hidden",
+            "overflow_y": "hidden",
+            "vertical_align": "middle",
+        },
+    }
 }
```

### Comparing `euporie-2.3.2/euporie/core/formatted_text/table.py` & `euporie-2.4.0/euporie/core/formatted_text/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,15 @@
 
     def __repr__(self) -> str:
         """Represent the cell instance as a string."""
         return f"{self.__class__.__name__}()"
 
 
 class RowCol:
-    """Bae class for table rows and columns."""
+    """Base class for table rows and columns."""
 
     type_: str
     span_type: str
 
     def __init__(
         self,
         table: Table | None = None,
@@ -509,14 +509,17 @@
 
 @lru_cache
 def compute_border_width(cell: Cell, render_count: int = 0) -> DiInt:
     """Compute the width od a cell's borders."""
     if isinstance(cell, DummyCell):
         return DiInt(0, 0, 0, 0)
 
+    if isinstance(cell, SpacerCell):
+        cell = cell.expands
+
     output = {"top": 1, "right": 1, "bottom": 1, "left": 1}
 
     row = cell.row
     col = cell.col
     table = col.table
 
     if row not in table._rows.values():
@@ -664,20 +667,20 @@
     # Determine whether to expand or contract the table
     current_width = total_width(col_widths)
     if width.preferred_specified:
         if current_width < width.preferred:
             expand(width.preferred)
         elif current_width > width.preferred:
             contract(width.preferred)
-    elif width.max_specified:
+    if width.max_specified:
         if current_width > width.max:
             contract(width.max)
         if current_width < width.max and expand_to_width:
             expand(width.max)
-    elif width.min_specified and current_width < width.min:
+    if width.min_specified and current_width < width.min:
         expand(width.min)
 
     return col_widths
 
 
 @lru_cache
 def get_node(
@@ -734,23 +737,25 @@
         A list of lines of formatted text
     """
     padding = compute_padding(cell, render_count)
     return split_lines(
         align(
             wrap(
                 [
-                    ("", "\n" * (padding.top or 0)),
+                    *([("", "\n" * padding.top)] if padding.top else []),
                     *compute_text(cell, render_count),
-                    ("", "\n" * (padding.bottom or 0)),
+                    *([("", "\n" * padding.bottom)] if padding.bottom else []),
                 ],
                 width=width,
+                placeholder="",
             ),
             compute_align(cell, render_count),
             width=width,
             style=compute_style(cell, render_count),
+            placeholder="",
         )
     )
 
 
 @lru_cache
 def compute_border_style(cell: Cell, render_count: int = 0) -> DiStr:
     """Compute the cell's final style for each of a cell's borders."""
@@ -956,15 +961,15 @@
     def add_row(self, row: Row) -> None:
         """Add a row to the table."""
         row.table = self
 
         unfilled = [
             i
             for i, row in self._rows.items()
-            if all([isinstance(cell, SpacerCell) for cell in row._cells.values()])
+            if all(isinstance(cell, SpacerCell) for cell in row._cells.values())
         ]
 
         index = min(
             min(unfilled + [len(self._rows)]),
             max([-1] + list(self._rows)) + 1,
         )
 
@@ -987,15 +992,15 @@
     def add_col(self, col: Col) -> None:
         """Add a column to the table."""
         col.table = self
 
         unfilled = [
             i
             for i, col in self._cols.items()
-            if all([isinstance(cell, SpacerCell) for cell in col._cells.values()])
+            if all(isinstance(cell, SpacerCell) for cell in col._cells.values())
         ]
 
         index = min(
             min(unfilled + [len(self._cols)]),
             max([-1] + list(self._cols)) + 1,
         )
 
@@ -1053,21 +1058,21 @@
             sw_bs = compute_border_style(sw, render_count)
             ne_bs = compute_border_style(ne, render_count)
             se_bs = compute_border_style(se, render_count)
             nw_bs = compute_border_style(nw, render_count)
 
             node_style = " ".join(
                 (
-                    sw_bs.top,
-                    sw_bs.right,
                     ne_bs.bottom,
+                    sw_bs.right,
+                    sw_bs.top,
                     ne_bs.left,
-                    se_bs.top,
-                    se_bs.left,
                     nw_bs.bottom,
+                    se_bs.left,
+                    se_bs.top,
                     nw_bs.right,
                 )
             )
             node_char = get_node(
                 compute_border_line(nw, render_count),
                 ne_bl := compute_border_line(ne, render_count),
                 se_bl := compute_border_line(se, render_count),
@@ -1107,16 +1112,16 @@
         if row:
             # Calculate borders
             borders = []
             render_count = self.render_count
             for w, e in zip([DummyCell(), *row.cells], [*row.cells, DummyCell()]):
                 border_style = " ".join(
                     (
-                        compute_border_style(w, render_count).right,
                         compute_border_style(e, render_count).left,
+                        compute_border_style(w, render_count).right,
                     )
                 )
                 border_char = get_vertical_edge(
                     compute_border_line(w, render_count),
                     compute_border_line(e, render_count),
                 )
 
@@ -1162,30 +1167,31 @@
                 output_line: StyleAndTextTuples = []
                 for i, (line, cell) in enumerate(zip(row_line, row.cells)):
                     # Skip spacer cells
                     if isinstance(cell, SpacerCell) and cell.expands.colspan > 1:
                         continue
                     output_line.append(borders[i])
 
-                    padding_style = f"{cell.style} nounderline"
+                    cell_style = compute_style(cell, render_count)
+                    padding_style = f"{cell_style} nounderline"
                     padding = compute_padding(cell, render_count)
                     padding_left, padding_right = padding.left, padding.right
 
                     excess = (
                         sum(col_widths[i : i + cell.colspan])
                         - padding_left
                         - fragment_list_width(line or [])
                         - padding_right
                     )
 
                     output_line.extend(
                         [
                             (padding_style, " " * (padding.left or 0)),
                             *(line or []),
-                            (cell.style, " " * excess),
+                            (cell_style, " " * excess),
                             (padding_style, " " * (padding.right or 0)),
                         ]
                     )
                 output_line.append(borders[i + 1])
                 output_lines.append(output_line)
 
         return join_lines(output_lines)
```

### Comparing `euporie-2.3.2/euporie/core/formatted_text/utils.py` & `euporie-2.4.0/euporie/core/formatted_text/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from prompt_toolkit.formatted_text.base import OneStyleAndTextTuple, StyleAndTextTuples
 from prompt_toolkit.formatted_text.utils import (
     fragment_list_to_text,
     split_lines,
     to_plain_text,
 )
+from prompt_toolkit.layout.utils import explode_text_fragments
 from prompt_toolkit.utils import get_cwidth
 from pygments.lexers import get_lexer_by_name
 from pygments.util import ClassNotFound
 
 from euporie.core.border import GridStyle, ThinGrid
 from euporie.core.data_structures import DiBool, DiInt, DiStr
 
@@ -97,24 +98,24 @@
 
 
 def fragment_list_to_words(
     fragments: StyleAndTextTuples, sep: str = " "
 ) -> Iterable[StyleAndTextTuples]:
     """Split formatted text into a list of word fragments which form words."""
     word: StyleAndTextTuples = []
-    for style, string, *_ in fragments:
+    for style, string, *rest in fragments:
         parts = re.split(r"(?<=[\s\-])", string)
         if len(parts) == 1:
-            word.append((style, parts[0]))
+            word.append(cast("OneStyleAndTextTuple", (style, parts[0], *rest)))
         else:
             for part in parts[:-1]:
-                word.append((style, part))
+                word.append(cast("OneStyleAndTextTuple", (style, part, *rest)))
                 yield word[:]
                 word.clear()
-            word.append((style, parts[-1]))
+            word.append(cast("OneStyleAndTextTuple", (style, parts[-1], *rest)))
     if word:
         yield word
 
 
 def apply_style(ft: StyleAndTextTuples, style: str) -> StyleAndTextTuples:
     """Apply a style to formatted text."""
     return [
@@ -194,15 +195,15 @@
         ignore_whitespace: Do not use placeholder when truncating whitespace
 
     Returns:
         The truncated formatted text
 
     """
     lines = split_lines(ft)
-    if max(fragment_list_width(line) for line in lines) < width:
+    if max(fragment_list_width(line) for line in lines) <= width:
         return ft
     result: StyleAndTextTuples = []
     phw = sum(get_cwidth(c) for c in placeholder)
     for line in split_lines(ft):
         used_width = 0
         for i, item in enumerate(line):
             fragment_width = sum(
@@ -456,30 +457,40 @@
         if (remaining := (width - fragment_list_width(line))) > 0:
             line.append((style + " nounderline", (char * remaining)))
         filled_output.append(line)
     return join_lines(filled_output)
 
 
 def paste(
-    ft_bottom: StyleAndTextTuples,
     ft_top: StyleAndTextTuples,
+    ft_bottom: StyleAndTextTuples,
     row: int = 0,
     col: int = 0,
+    transparent: bool = False,
 ) -> StyleAndTextTuples:
     """Pate formatted text on top of other formatted text."""
     ft: StyleAndTextTuples = []
-
     top_lines = dict(enumerate(split_lines(ft_top), start=row))
     for y, line_b in enumerate(split_lines(ft_bottom)):
         if y in top_lines:
-            # x = 0
             line_t = top_lines[y]
             line_t_width = fragment_list_width(line_t)
             ft += substring(line_b, 0, col)
-            ft += substring(line_t)
+            if transparent:
+                chars_t = explode_text_fragments(line_t)
+                chars_b = explode_text_fragments(
+                    substring(line_b, col, col + line_t_width)
+                )
+                for char_t, char_b in zip(chars_t, chars_b):
+                    if char_t[0] == "" and char_t[1] == " ":
+                        ft.append(char_b)
+                    else:
+                        ft.append(char_t)
+            else:
+                ft += line_t
             ft += substring(line_b, col + line_t_width)
         else:
             ft += line_b
         ft.append(("", "\n"))
 
     if ft:
         ft.pop()
@@ -525,16 +536,16 @@
 
     if rows_a - baseline_a < rows_b - baseline_b:
         ft_a = [*ft_a, ("", lines_below * "\n")]
     elif rows_a - baseline_a > rows_b - baseline_b:
         ft_b = [*ft_b, ("", lines_below * "\n")]
 
     ft = paste(
-        pad(ft_a, style=style),
         ft_b,
+        pad(ft_a, style=style),
         row=0,
         col=cols_a,
     )
 
     new_baseline = max(baseline_a, baseline_b)
 
     return ft, new_baseline
```

### Comparing `euporie-2.3.2/euporie/core/key_binding/key_processor.py` & `euporie-2.4.0/euporie/core/key_binding/key_processor.py`

 * *Files identical despite different names*

### Comparing `euporie-2.3.2/euporie/core/key_binding/micro_state.py` & `euporie-2.4.0/euporie/core/key_binding/micro_state.py`

 * *Files identical despite different names*

### Comparing `euporie-2.3.2/euporie/core/key_binding/registry.py` & `euporie-2.4.0/euporie/core/key_binding/registry.py`

 * *Files identical despite different names*

### Comparing `euporie-2.3.2/euporie/core/key_binding/utils.py` & `euporie-2.4.0/euporie/core/key_binding/utils.py`

 * *Files identical despite different names*

### Comparing `euporie-2.3.2/euporie/core/key_binding/vi_state.py` & `euporie-2.4.0/euporie/core/key_binding/vi_state.py`

 * *Files identical despite different names*

### Comparing `euporie-2.3.2/euporie/core/key_binding/bindings/completion.py` & `euporie-2.4.0/euporie/core/key_binding/bindings/completion.py`

 * *Files identical despite different names*

### Comparing `euporie-2.3.2/euporie/core/key_binding/bindings/micro.py` & `euporie-2.4.0/euporie/core/key_binding/bindings/micro.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,19 @@
         "euporie.core.key_binding.bindings.micro.EditMode": {
             "type-key": "<any>",
             "move-cursor-right": "right",
             "move-cursor-left": "left",
             "newline": "enter",
             "accept-line": "enter",
             "backspace": ["backspace", "c-h"],
-            "backward-kill-word": [("escape", "backspace"), ("escape", "c-h")],
+            "backward-kill-word": [
+                "c-backspace",
+                ("escape", "backspace"),
+                ("escape", "c-h"),
+            ],
             "start-selection": [
                 "s-up",
                 "s-down",
                 "s-right",
                 "s-left",
                 ("escape", "s-left"),
                 ("escape", "s-right"),
```

### Comparing `euporie-2.3.2/euporie/core/key_binding/bindings/mouse.py` & `euporie-2.4.0/euporie/core/key_binding/bindings/mouse.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,19 +150,19 @@
             # Save global mouse position
             event.app.mouse_position = Point(x=x, y=y)
 
             # Apply limits to mouse position if enabled
             if (mouse_limits := event.app.mouse_limits) is not None:
                 x = max(
                     mouse_limits.xpos,
-                    min(x, mouse_limits.xpos + mouse_limits.width - 1),
+                    min(x, mouse_limits.xpos + (mouse_limits.width - 1)),
                 )
                 y = max(
                     mouse_limits.ypos,
-                    min(y, mouse_limits.ypos + mouse_limits.height - 1),
+                    min(y, mouse_limits.ypos + (mouse_limits.height - 1)),
                 )
 
             # Call the mouse handler from the renderer.
             # Note: This can return `NotImplemented` if no mouse handler was
             #       found for this position, or if no repainting needs to
             #       happen. this way, we avoid excessive repaints during mouse
             #       movements.
```

### Comparing `euporie-2.3.2/euporie/core/tabs/base.py` & `euporie-2.4.0/euporie/core/tabs/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,60 +4,76 @@
 
 import logging
 from abc import ABCMeta
 from collections import deque
 from functools import partial
 from typing import TYPE_CHECKING
 
+from prompt_toolkit.eventloop.utils import run_in_executor_with_context
 from prompt_toolkit.history import InMemoryHistory
-from prompt_toolkit.layout.containers import Window
+from prompt_toolkit.layout.containers import Window, WindowAlign
+from prompt_toolkit.layout.controls import FormattedTextControl
 
 from euporie.core.comm.registry import open_comm
 from euporie.core.commands import add_cmd
 from euporie.core.completion import KernelCompleter
 from euporie.core.config import add_setting
 from euporie.core.current import get_app
 from euporie.core.filters import kernel_tab_has_focus, tab_has_focus
 from euporie.core.history import KernelHistory
 from euporie.core.kernel import Kernel, MsgCallbacks
+from euporie.core.key_binding.registry import (
+    register_bindings,
+)
 from euporie.core.suggest import HistoryAutoSuggest
 
 if TYPE_CHECKING:
+    from pathlib import Path
     from typing import Any, Callable, Deque, Sequence
 
     from prompt_toolkit.auto_suggest import AutoSuggest
     from prompt_toolkit.completion.base import Completer
-    from prompt_toolkit.formatted_text import AnyFormattedText
     from prompt_toolkit.history import History
     from prompt_toolkit.layout.containers import AnyContainer
-    from upath import UPath
 
     from euporie.core.app import BaseApp
     from euporie.core.comm.base import Comm
+    from euporie.core.widgets.status_bar import StatusBarFields
 
 log = logging.getLogger(__name__)
 
 
 class Tab(metaclass=ABCMeta):
-    """Bae class for interface tabs."""
+    """Base class for interface tabs."""
+
+    _registry: set[type[Tab]] = set()
+    name: str | None = None
+    weight: int = 0
+    mime_types: set[str] = set()
+    file_extensions: set[str] = set()
 
     container: AnyContainer
 
-    def __init__(self, app: BaseApp, path: UPath | None = None) -> None:
+    def __init_subclass__(cls, *args: Any, **kwargs: Any) -> None:
+        """Compile a registry of named tabs."""
+        super().__init_subclass__(**kwargs)
+        if cls.name:
+            Tab._registry.add(cls)
+
+    def __init__(self, app: BaseApp, path: Path | None = None) -> None:
         """Call when the tab is created."""
         self.app = app
         self.path = path
-        self.app.container_statuses[self] = self.statusbar_fields
-        self.container = Window()
+        self.container = Window(
+            FormattedTextControl([("fg:#888888", "\nLoading…")], focusable=True),
+            align=WindowAlign.CENTER,
+        )
 
-    def statusbar_fields(
-        self,
-    ) -> tuple[Sequence[AnyFormattedText], Sequence[AnyFormattedText]]:
-        """Return a list of statusbar field values shown then this tab is active."""
-        return ([], [])
+        self.dirty = False
+        self.saving = False
 
     @property
     def title(self) -> str:
         """Return the tab title."""
         return ""
 
     def reset(self) -> "None":  # noqa B027
@@ -67,81 +83,149 @@
     def close(self, cb: Callable | None = None) -> None:
         """Close a tab with a callback.
 
         Args:
             cb: A function to call after the tab is closed.
 
         """
-        if self in self.app.container_statuses:
-            del self.app.container_statuses[self]
+        # Run callback
         if callable(cb):
             cb()
 
     def focus(self) -> None:
         """Focus the tab (or make it visible)."""
         self.app.focus_tab(self)
 
-    def save(self, path: UPath | None = None, cb: Callable | None = None) -> None:
+    def _save(self, path: Path | None = None, cb: Callable | None = None) -> None:
+        """Perform the file save in a background thread."""
+        run_in_executor_with_context(self.save, path, cb)
+
+    def save(self, path: Path | None = None, cb: Callable | None = None) -> None:
         """Save the current notebook."""
         raise NotImplementedError
 
+    def __pt_status__(self) -> StatusBarFields | None:
+        """Return a list of statusbar field values shown then this tab is active."""
+        return ([], [])
+
     def __pt_container__(self) -> AnyContainer:
         """Return the main container object."""
         return self.container
 
     # ################################### Commands ####################################
 
     @staticmethod
     @add_cmd(filter=tab_has_focus, title="Reset the current tab")
     def _reset_tab() -> None:
         """Reet the current tab, reloading contents from source."""
         if (tab := get_app().tab) is not None:
             tab.reset()
 
+    @staticmethod
+    @add_cmd(filter=tab_has_focus)
+    def _save_file() -> None:
+        """Save the current file."""
+        if (tab := get_app().tab) is not None:
+            try:
+                tab._save()
+            except NotImplementedError:
+                pass
+
+    # ################################# Key Bindings ##################################
+
+    register_bindings(
+        {
+            "euporie.core.tabs.base.Tab": {
+                "save-file": "c-s",
+                "reset-tab": "f5",
+            }
+        }
+    )
+
 
 class KernelTab(Tab, metaclass=ABCMeta):
     """A Tab which connects to a kernel."""
 
     kernel: Kernel
     kernel_language: str
     _metadata: dict[str, Any]
+    bg_init = True
 
     default_callbacks: MsgCallbacks
     allow_stdin: bool
 
     def __init__(
         self,
         app: BaseApp,
-        path: UPath | None = None,
+        path: Path | None = None,
         kernel: Kernel | None = None,
         comms: dict[str, Comm] | None = None,
         use_kernel_history: bool = False,
+        connection_file: Path | None = None,
     ) -> None:
         """Create a new instance of a tab with a kernel."""
+        # Init tab
         super().__init__(app, path)
 
+        if self.bg_init:
+            # Load kernel in a background thread
+            run_in_executor_with_context(
+                partial(
+                    self.init_kernel, kernel, comms, use_kernel_history, connection_file
+                )
+            )
+        else:
+            self.init_kernel(kernel, comms, use_kernel_history, connection_file)
+
+    def pre_init_kernel(self) -> None:
+        """Run stuff before the kernel is loaded."""
+        pass
+
+    def post_init_kernel(self) -> None:
+        """Run stuff after the kernel is loaded."""
+        pass
+
+    def init_kernel(
+        self,
+        kernel: Kernel | None = None,
+        comms: dict[str, Comm] | None = None,
+        use_kernel_history: bool = False,
+        connection_file: Path | None = None,
+    ) -> None:
+        """Set up the tab's kernel and related components."""
+        self.pre_init_kernel()
+
         self.kernel_queue: Deque[Callable] = deque()
 
         if kernel:
             self.kernel = kernel
             self.kernel.default_callbacks = self.default_callbacks
         else:
             self.kernel = Kernel(
                 kernel_tab=self,
                 allow_stdin=self.allow_stdin,
                 default_callbacks=self.default_callbacks,
+                connection_file=connection_file,
             )
         self.comms: dict[str, Comm] = comms or {}  # The client-side comm states
         self.completer: Completer = KernelCompleter(self.kernel)
         self.use_kernel_history = use_kernel_history
         self.history: History = (
             KernelHistory(self.kernel) if use_kernel_history else InMemoryHistory()
         )
         self.suggester: AutoSuggest = HistoryAutoSuggest(self.history)
 
+        self.post_init_kernel()
+
+    def close(self, cb: Callable | None = None) -> None:
+        """Shut down kernel when tab is closed."""
+        if hasattr(self, "kernel"):
+            self.kernel.shutdown()
+        super().close(cb)
+
     def interrupt_kernel(self) -> None:
         """Interrupt the current `Notebook`'s kernel."""
         self.kernel.interrupt()
 
     def restart_kernel(self, cb: Callable | None = None) -> None:
         """Restart the current `Notebook`'s kernel."""
 
@@ -289,15 +373,15 @@
         if isinstance(kt := get_app().tab, KernelTab):
             kt.change_kernel()
 
     # ################################### Settings ####################################
 
     add_setting(
         name="kernel_name",
-        flags=["--kernel-name"],
+        flags=["--kernel-name", "--kernel"],
         type_=str,
         help_="The name of the kernel to start by default",
         default="python3",
         description="""
             The name of the kernel selected automatically by the console app or in new
             notebooks. If set to an empty string, the user will be asked which kernel
             to launch.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `euporie-2.3.2/euporie/core/tabs/notebook.py` & `euporie-2.4.0/euporie/core/tabs/notebook.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,24 +11,31 @@
 import nbformat
 from prompt_toolkit.filters import Never, buffer_has_focus
 
 from euporie.core.comm.registry import open_comm
 from euporie.core.commands import get_cmd
 from euporie.core.config import add_setting
 from euporie.core.kernel import MsgCallbacks
+from euporie.core.path import parse_path
 from euporie.core.tabs.base import KernelTab
-from euporie.core.utils import parse_path
 from euporie.core.widgets.cell import Cell, get_cell_id
 
+try:
+    from jupytext import read as read_nb
+    from jupytext import write as write_nb
+except ModuleNotFoundError:
+    from nbformat import read as read_nb
+    from nbformat import write as write_nb
+
 if TYPE_CHECKING:
+    from pathlib import Path
     from typing import Any, Callable
 
     from prompt_toolkit.filters import Filter
     from prompt_toolkit.layout.containers import AnyContainer
-    from upath import UPath
 
     from euporie.core.app import BaseApp
     from euporie.core.comm.base import Comm
     from euporie.core.kernel import Kernel
 
 log = logging.getLogger(__name__)
 
@@ -38,15 +45,15 @@
 
     allow_stdin = False
     edit_mode = False
 
     def __init__(
         self,
         app: BaseApp,
-        path: UPath | None = None,
+        path: Path | None = None,
         kernel: Kernel | None = None,
         comms: dict[str, Comm] | None = None,
         use_kernel_history: bool = False,
         json: dict[str, Any] | None = None,
     ) -> None:
         """Instantiate a Notebook container, using a notebook at a given path.
 
@@ -69,74 +76,90 @@
                 "clear_output": lambda wait: self.cell.clear_output(wait),
                 "set_metadata": lambda path, data: self.cell.set_metadata(path, data),
                 "set_status": self.set_status,
                 "set_kernel_info": self.set_kernel_info,
                 "dead": self.kernel_died,
             }
         )
-
-        # Load the notebook file
-        self.path = parse_path(path)
-        log.debug("Loading notebooks %s", self.path)
-
-        self.load(json)
+        self.json = json or {}
+        self._rendered_cells: dict[str, Cell] = {}
+        self.multiple_cells_selected: Filter = Never()
+        self.path = parse_path(path) if path else None
+        self.loaded = False
 
         super().__init__(
             app, path, kernel=kernel, comms=comms, use_kernel_history=use_kernel_history
         )
 
-        self._rendered_cells: dict[str, Cell] = {}
-        self.load_widgets_from_metadata()
-        self.dirty = False
-        self.saving = False
-        self.multiple_cells_selected: Filter = Never()
-
-        self.container = self.load_container()
-
     # Tab stuff
 
     def reset(self) -> None:
         """Reload the notebook file from the disk and re-render."""
         # Restore selection after reset
         if self.path is not None:
             self._rendered_cells = {}
             self.load()
         self.refresh()
 
     # KernelTab stuff
 
+    def pre_init_kernel(self) -> None:
+        """Run stuff before the kernel is loaded."""
+        # Load notebook file
+        self.load()
+
+    def post_init_kernel(self) -> None:
+        """Load the notebook container after the kernel has been loaded."""
+        # Replace the tab's container
+        prev = self.container
+        self.container = self.load_container()
+        self.loaded = True
+        self.app.invalidate()
+
+        # Update the focus if the old container had focus
+        if (layout := self.app.layout).has_focus(prev):
+
+            async def _focus_new_container() -> None:
+                layout.focus(self.container)
+
+            self.app.create_background_task(_focus_new_container())
+
+        # Load widgets
+        self.load_widgets_from_metadata()
+
     @property
     def metadata(self) -> dict[str, Any]:
         """Return a dictionary to hold notebook / kernel metadata."""
         return self.json.setdefault("metadata", {})
 
     def kernel_started(self, result: dict[str, Any] | None = None) -> None:
         """Task to run when the kernel has started."""
         super().kernel_started(result)
 
     def kernel_died(self) -> None:
         """Call if the kernel dies."""
         if confirm := self.app.dialogs.get("confirm"):
             confirm.show(
                 title="Kernel connection lost",
-                message="The kernel appears to have died\nas it can no longer be reached.\n\n"
+                message="The kernel appears to have died\n"
+                "as it can no longer be reached.\n\n"
                 "Do you want to restart the kernel?",
                 cb=self.kernel.restart,
             )
 
     # Notebook stuff
 
-    def load(self, json: dict[str, Any] | None = None) -> None:
+    def load(self) -> None:
         """Load the notebook file from the file-system."""
         # Open json file, or load from passed json object
         if self.path is not None and self.path.exists():
             with self.path.open() as f:
-                self.json = nbformat.read(f, as_version=4)
+                self.json = read_nb(f, as_version=4)
         else:
-            self.json = json or nbformat.v4.new_notebook()
+            self.json = self.json or nbformat.v4.new_notebook()
         # Ensure there is always at least one cell
         if not self.json.setdefault("cells", []):
             self.json["cells"] = [nbformat.v4.new_code_cell()]
 
     def set_status(self, status: str) -> None:
         """Call when kernel status changes."""
         self.cell.set_status(status)
@@ -238,15 +261,15 @@
             unsaved.show(
                 tab=self,
                 cb=cb,
             )
         else:
             super().close(cb)
 
-    def save(self, path: UPath | None = None, cb: Callable | None = None) -> None:
+    def save(self, path: Path | None = None, cb: Callable | None = None) -> None:
         """Write the notebook's JSON to the current notebook's file.
 
         Additionally save the widget state to the notebook metadata.
 
         Args:
             path: An optional new path at which to save the tab
             cb: A callback to run if after saving the notebook.
@@ -263,32 +286,51 @@
                         comm_id: comm._get_embed_state()
                         for comm_id, comm in self.comms.items()
                         if comm.data.get("state", {}).get("__unlinked__") is not True
                     },
                 }
             }
         if self.path is None:
-            # get_cmd("save-as").run()
             if dialog := self.app.dialogs.get("save-as"):
                 dialog.show(tab=self, cb=cb)
         else:
             log.debug("Saving notebook..")
             self.saving = True
             self.app.invalidate()
+
+            # Save to a temp file, then replace the original
+            temp_path = self.path.parent / f".{self.path.stem}.tmp{self.path.suffix}"
+            log.debug("Using temporary file %s", temp_path.name)
             try:
-                open_file = self.path.open("w")
+                open_file = temp_path.open("w")
             except NotImplementedError:
                 get_cmd("save-as").run()
             else:
-                with open_file as f:
-                    nbformat.write(nb=nbformat.from_dict(self.json), fp=f)
-                self.dirty = False
-                self.saving = False
-                self.app.invalidate()
-                log.debug("Notebook saved")
+                try:
+                    try:
+                        with open_file as f:
+                            write_nb(nb=nbformat.from_dict(self.json), fp=f)
+                    except AssertionError:
+                        # Jupytext requires a filename if we don't give it a format
+                        write_nb(nb=nbformat.from_dict(self.json), fp=temp_path)
+                except Exception:
+                    if dialog := self.app.dialogs.get("save-as"):
+                        dialog.show(tab=self, cb=cb)
+                else:
+                    open_file.close()
+                    try:
+                        temp_path.rename(self.path)
+                    except Exception:
+                        if dialog := self.app.dialogs.get("save-as"):
+                            dialog.show(tab=self, cb=cb)
+                    else:
+                        self.dirty = False
+                        self.saving = False
+                        self.app.invalidate()
+                        log.debug("Notebook saved")
             # Run the callback
             if callable(cb):
                 cb()
 
     def run_cell(
         self,
         cell: Cell,
```

### Comparing `euporie-2.3.2/euporie/core/widgets/cell.py` & `euporie-2.4.0/euporie/core/widgets/cell.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,18 @@
                     pager.hide()
 
             # Tell the scrolling container to scroll the cursor into view on the next render
             weak_self.kernel_tab.page.scroll_to_cursor = True
 
         # Now we generate the main container used to represent a kernel_tab cell
 
+        source_hidden = Condition(
+            lambda: self.json["metadata"].get("jupyter", {}).get("source_hidden", False)
+        )
+
         self.input_box = KernelInput(
             kernel_tab=self.kernel_tab,
             text=self.input,
             complete_while_typing=self.is_code,
             autosuggest_while_typing=self.is_code,
             wrap_lines=Condition(lambda: weak_self.json.get("cell_type") == "markdown"),
             on_text_changed=on_text_changed,
@@ -166,14 +170,15 @@
                         if cell.cell_type != "raw"
                         else SimpleLexer()
                     ),
                     weakref.proxy(self),
                 )
             ),
             accept_handler=lambda buffer: self.run_or_render() or True,
+            focusable=show_input & ~source_hidden,
         )
         self.input_box.buffer.name = self.cell_type
 
         def border_char(name: str) -> Callable[..., str]:
             """Return a function which returns the cell border character to display."""
 
             def _inner() -> str:
@@ -224,18 +229,14 @@
                 ),
                 fill(char=border_char("TOP_MID"), height=1),
                 fill(width=1, height=1, char=border_char("TOP_RIGHT")),
             ],
             height=1,
         )
 
-        source_hidden = Condition(
-            lambda: self.json["metadata"].get("jupyter", {}).get("source_hidden", False)
-        )
-
         input_row = ConditionalContainer(
             VSplit(
                 [
                     fill(width=1, char=border_char("MID_LEFT")),
                     ConditionalContainer(
                         content=Window(
                             FormattedTextControl(
@@ -584,15 +585,15 @@
 
     @property
     def language(self) -> str:
         """Return the cell's code language."""
         if self.cell_type == "markdown":
             return "markdown"
         elif self.cell_type == "code":
-            lang_info = self.kernel_tab.json.metadata.get("language_info", {})
+            lang_info = self.kernel_tab.metadata.get("language_info", {})
             return lang_info.get("name", lang_info.get("pygments_lexer", "python"))
         else:
             return "raw"
 
     def reformat(self) -> None:
         """Reformat the cell's input."""
         config = get_app().config
```

### Comparing `euporie-2.3.2/euporie/core/widgets/cell_outputs.py` & `euporie-2.4.0/euporie/core/widgets/cell_outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import PurePath
 from typing import TYPE_CHECKING
 
 from prompt_toolkit.cache import SimpleCache
 from prompt_toolkit.layout.containers import DynamicContainer, HSplit, to_container
 from prompt_toolkit.widgets.base import Box
 
-from euporie.core.convert.base import BASE64_FORMATS, MIME_FORMATS, find_route
+from euporie.core.convert.core import BASE64_FORMATS, MIME_FORMATS, find_route
 from euporie.core.current import get_app
 from euporie.core.widgets.display import Display
 from euporie.core.widgets.tree import JsonView
 
 if TYPE_CHECKING:
     from typing import Any, Protocol, TypeVar
 
@@ -35,15 +35,15 @@
             ...
 
 
 log = logging.getLogger(__name__)
 
 
 class CellOutputElement(metaclass=ABCMeta):
-    """Bae class for the various types of cell outputs (display data or widgets)."""
+    """Base class for the various types of cell outputs (display data or widgets)."""
 
     data: Any
 
     def __init__(
         self,
         mime: str,
         data: Any,
```

### Comparing `euporie-2.3.2/euporie/core/widgets/decor.py` & `euporie-2.4.0/euporie/core/widgets/decor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Decorative widgets."""
 
-# from __future__ import annotations
+from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
 from prompt_toolkit.cache import FastDictCache
 from prompt_toolkit.filters import has_focus, to_filter
 from prompt_toolkit.layout.containers import (
@@ -26,15 +26,15 @@
 from euporie.core.border import ThinLine
 from euporie.core.config import add_setting
 from euporie.core.current import get_app
 from euporie.core.data_structures import DiBool
 from euporie.core.style import ColorPaletteColor
 
 if TYPE_CHECKING:
-    from typing import Callable, Optional, Union
+    from typing import Callable
 
     from prompt_toolkit.key_binding.key_bindings import NotImplementedOrNone
     from prompt_toolkit.layout.containers import AnyContainer
     from prompt_toolkit.mouse_events import MouseEvent
 
     from euporie.core.border import GridStyle
 
@@ -44,20 +44,20 @@
 
 
 class Line(Container):
     """Draw a horizontal or vertical line."""
 
     def __init__(
         self,
-        char: "Optional[str]" = None,
-        width: "Optional[int]" = None,
-        height: "Optional[int]" = None,
-        collapse: "bool" = False,
-        style: "str" = "class:grid-line",
-    ) -> "None":
+        char: str | None = None,
+        width: int | None = None,
+        height: int | None = None,
+        collapse: bool = False,
+        style: str = "class:grid-line",
+    ) -> None:
         """Initialize a grid line.
 
         Args:
             char: The character to draw. If unset, the relevant character from
                 :py:class:`euporie.core.box.grid` is used
             width: The length of the line. If specified, the line will be horizontal
             height: The height of the line. If specified, the line will be vertical
@@ -74,36 +74,34 @@
         self.width = width
         self.height = height
         if char is None:
             char = ThinLine.grid.VERTICAL if width else ThinLine.grid.HORIZONTAL
         self.char = Char(char, style)
         self.collapse = collapse
 
-    def reset(self) -> "None":
+    def reset(self) -> None:
         """Reet the state of the line. Does nothing."""
 
-    def preferred_width(self, max_available_width: "int") -> "Dimension":
+    def preferred_width(self, max_available_width: int) -> Dimension:
         """Return the preferred width of the line."""
         return Dimension(min=int(not self.collapse), max=self.width)
 
-    def preferred_height(
-        self, width: "int", max_available_height: "int"
-    ) -> "Dimension":
+    def preferred_height(self, width: int, max_available_height: int) -> Dimension:
         """Return the preferred height of the line."""
         return Dimension(min=int(not self.collapse), max=self.height)
 
     def write_to_screen(
         self,
-        screen: "Screen",
-        mouse_handlers: "MouseHandlers",
-        write_position: "WritePosition",
-        parent_style: "str",
-        erase_bg: "bool",
-        z_index: "Optional[int]",
-    ) -> "None":
+        screen: Screen,
+        mouse_handlers: MouseHandlers,
+        write_position: WritePosition,
+        parent_style: str,
+        erase_bg: bool,
+        z_index: int | None,
+    ) -> None:
         """Draw a continuous line in the ``write_position`` area.
 
         Args:
             screen: The :class:`~prompt_toolkit.layout.screen.Screen` class to which
                 the output has to be written.
             mouse_handlers: :class:`prompt_toolkit.layout.mouse_handlers.MouseHandlers`.
             write_position: A :class:`prompt_toolkit.layout.screen.WritePosition` object
@@ -120,55 +118,53 @@
         xpos = write_position.xpos
 
         for y in range(ypos, ypos + write_position.height):
             row = screen.data_buffer[y]
             for x in range(xpos, xpos + write_position.width):
                 row[x] = self.char
 
-    def get_children(self) -> "list":
+    def get_children(self) -> list:
         """Return an empty list of the container's children."""
         return []
 
 
 class Pattern(Container):
     """Fill an area with a repeating background pattern."""
 
     def __init__(
         self,
-        char: "Union[str, Callable[[], str]]",
-        pattern: "Union[int, Callable[[], int]]" = 1,
-    ) -> "None":
+        char: str | Callable[[], str],
+        pattern: int | Callable[[], int] = 1,
+    ) -> None:
         """Initialize the :class:`Pattern`."""
         self.bg = Char(" ", "class:pattern")
         self.char = char
         self.pattern = pattern
 
-    def reset(self) -> "None":
+    def reset(self) -> None:
         """Reet the pattern. Does nothing."""
         pass
 
-    def preferred_width(self, max_available_width: "int") -> "Dimension":
+    def preferred_width(self, max_available_width: int) -> Dimension:
         """Return an empty dimension (expand to available width)."""
         return Dimension()
 
-    def preferred_height(
-        self, width: "int", max_available_height: "int"
-    ) -> "Dimension":
+    def preferred_height(self, width: int, max_available_height: int) -> Dimension:
         """Return an empty dimension (expand to available height)."""
         return Dimension()
 
     def write_to_screen(
         self,
-        screen: "Screen",
-        mouse_handlers: "MouseHandlers",
-        write_position: "WritePosition",
-        parent_style: "str",
-        erase_bg: "bool",
-        z_index: "Optional[int]",
-    ) -> "None":
+        screen: Screen,
+        mouse_handlers: MouseHandlers,
+        write_position: WritePosition,
+        parent_style: str,
+        erase_bg: bool,
+        z_index: int | None,
+    ) -> None:
         """Fill the whole area of write_position with a pattern.
 
         Args:
             screen: The :class:`~prompt_toolkit.layout.screen.Screen` class to which
                 the output has to be written.
             mouse_handlers: :class:`prompt_toolkit.layout.mouse_handlers.MouseHandlers`.
             write_position: A :class:`prompt_toolkit.layout.screen.WritePosition` object
@@ -204,29 +200,29 @@
                     or (pattern == 4 and (x + y) % 3 == 0)
                     or (pattern == 5 and ((x + y % 2 * 3) % 6) % 4 == 0)
                 ):
                     row[x] = char
                 else:
                     row[x] = bg
 
-    def get_children(self) -> "list":
+    def get_children(self) -> list:
         """Return an empty list of the container's children."""
         return []
 
 
 class Border:
     """Draw a border around any container."""
 
     def __init__(
         self,
-        body: "AnyContainer",
-        border: "Optional[GridStyle]" = ThinLine.grid,
-        style: "Union[str, Callable[[], str]]" = "class:border",
-        show_borders: "Optional[DiBool]" = None,
-    ) -> "None":
+        body: AnyContainer,
+        border: GridStyle | None = ThinLine.grid,
+        style: str | Callable[[], str] = "class:border",
+        show_borders: DiBool | None = None,
+    ) -> None:
         """Create a new border widget which wraps another container.
 
         Args:
             body: The container to surround with a border
             border: The grid style to use
             style: The style to apply to the border
             show_borders: Which of the four borders should be displayed
@@ -240,15 +236,15 @@
         else:
             show_borders = DiBool(True, True, True, True)
         border_top = to_filter(show_borders.top)
         border_right = to_filter(show_borders.right)
         border_bottom = to_filter(show_borders.bottom)
         border_left = to_filter(show_borders.left)
 
-        self.container: "AnyContainer"
+        self.container: AnyContainer
         if border is not None and any(show_borders):
             self.container = HSplit(
                 [
                     ConditionalContainer(
                         VSplit(
                             [
                                 ConditionalContainer(
@@ -340,75 +336,73 @@
                         filter=border_bottom,
                     ),
                 ],
             )
         else:
             self.container = body
 
-    def add_style(self, extra: "str") -> "Callable[[], str]":
+    def add_style(self, extra: str) -> Callable[[], str]:
         """Return a function which adds a style string to the border style."""
 
-        def _style() -> "str":
+        def _style() -> str:
             if callable(self.style):
                 return f"{self.style()} {extra}"
             else:
                 return f"{self.style} {extra}"
 
         return _style
 
-    def __pt_container__(self) -> "AnyContainer":
+    def __pt_container__(self) -> AnyContainer:
         """Return the border widget's container."""
         return self.container
 
 
 class FocusedStyle(Container):
     """Apply a style to child containers when focused or hovered."""
 
     def __init__(
         self,
-        body: "AnyContainer",
-        style_focus: "Union[str, Callable[[], str]]" = "class:focused",
-        style_hover: "Union[str, Callable[[], str]]" = "class:hovered",
-    ) -> "None":
+        body: AnyContainer,
+        style_focus: str | Callable[[], str] = "class:focused",
+        style_hover: str | Callable[[], str] = "",
+    ) -> None:
         """Create a new instance of the widget.
 
         Args:
             body: The container to act on
             style_focus: The style to apply when the body has focus
             style_hover: The style to apply when the body is hovered
         """
         self.body = body
         self.style_focus = style_focus
         self.style_hover = style_hover
         self.hover = False
         self.has_focus = has_focus(self.body)
 
-    def reset(self) -> "None":
+    def reset(self) -> None:
         """Reet the wrapped container."""
         to_container(self.body).reset()
 
-    def preferred_width(self, max_available_width: "int") -> "Dimension":
+    def preferred_width(self, max_available_width: int) -> Dimension:
         """Return the wrapped container's preferred width."""
         return to_container(self.body).preferred_width(max_available_width)
 
-    def preferred_height(
-        self, width: "int", max_available_height: "int"
-    ) -> "Dimension":
+    def preferred_height(self, width: int, max_available_height: int) -> Dimension:
         """Return the wrapped container's preferred height."""
         return to_container(self.body).preferred_height(width, max_available_height)
 
     def write_to_screen(
         self,
-        screen: "Screen",
-        mouse_handlers: "MouseHandlers",
-        write_position: "WritePosition",
-        parent_style: "str",
-        erase_bg: "bool",
-        z_index: "Optional[int]",
-    ) -> "None":
+        screen: Screen,
+        mouse_handlers: MouseHandlers,
+        write_position: WritePosition,
+        parent_style: str,
+        erase_bg: bool,
+        z_index: int | None,
+    ) -> None:
         """Draw the wrapped container with the additional style."""
         to_container(self.body).write_to_screen(
             screen,
             mouse_handlers,
             write_position,
             f"{parent_style} {self.get_style()}",
             erase_bg,
@@ -418,18 +412,18 @@
         if self.style_hover:
             x_min = write_position.xpos
             x_max = x_min + write_position.width
             y_min = write_position.ypos
             y_max = y_min + write_position.height
 
             # Wrap mouse handlers to add "hover" class on hover
-            def _wrap_mouse_handler(handler: "Callable") -> "MouseHandler":
+            def _wrap_mouse_handler(handler: Callable) -> MouseHandler:
                 def wrapped_mouse_handler(
-                    mouse_event: "MouseEvent",
-                ) -> "NotImplementedOrNone":
+                    mouse_event: MouseEvent,
+                ) -> NotImplementedOrNone:
                     result = handler(mouse_event)
 
                     if mouse_event.event_type == MouseEventType.MOUSE_MOVE:
                         app = get_app()
                         if (
                             mouse_event.position.x,
                             mouse_event.position.y,
@@ -448,64 +442,62 @@
                 tuple[Callable], MouseHandler
             ] = FastDictCache(get_value=_wrap_mouse_handler)
             for y in range(y_min, y_max):
                 row = mouse_handlers.mouse_handlers[y]
                 for x in range(x_min, x_max):
                     row[x] = mouse_handler_wrappers[(row[x],)]
 
-    def get_style(self) -> "str":
+    def get_style(self) -> str:
         """Determine the style to apply depending on the focus status."""
         style = ""
         if self.has_focus():
             style += (
                 self.style_focus() if callable(self.style_focus) else self.style_focus
             )
         if self.hover:
             style += " " + (
                 self.style_hover() if callable(self.style_hover) else self.style_hover
             )
         return style
 
-    def get_children(self) -> "list[Container]":
+    def get_children(self) -> list[Container]:
         """Return the list of child :class:`.Container` objects."""
         return [to_container(self.body)]
 
 
 class DropShadow(Container):
     """A transparent container which makes the background darker."""
 
     def __init__(self, amount: float = 0.5) -> None:
         """Create a new instance."""
         self.amount = amount
         app = get_app()
         self.cp = app.color_palette
         self.renderer = app.renderer
 
-    def reset(self) -> "None":
+    def reset(self) -> None:
         """Reet the wrapped container - here, do nothing."""
 
-    def preferred_width(self, max_available_width: "int") -> "Dimension":
+    def preferred_width(self, max_available_width: int) -> Dimension:
         """Return the wrapped container's preferred width."""
         return Dimension(weight=1)
 
-    def preferred_height(
-        self, width: "int", max_available_height: "int"
-    ) -> "Dimension":
+    def preferred_height(self, width: int, max_available_height: int) -> Dimension:
         """Return the wrapped container's preferred height."""
         return Dimension(weight=1)
 
     def write_to_screen(
         self,
-        screen: "Screen",
-        mouse_handlers: "MouseHandlers",
-        write_position: "WritePosition",
-        parent_style: "str",
-        erase_bg: "bool",
-        z_index: "Optional[int]",
-    ) -> "None":
+        screen: Screen,
+        mouse_handlers: MouseHandlers,
+        write_position: WritePosition,
+        parent_style: str,
+        erase_bg: bool,
+        z_index: int | None,
+    ) -> None:
         """Draw the wrapped container with the additional style."""
         attr_cache = self.renderer._attrs_for_style
         if attr_cache is not None:
             ypos = write_position.ypos
             xpos = write_position.xpos
             amount = self.amount
             for y in range(ypos, ypos + write_position.height):
@@ -547,15 +539,15 @@
 class Shadow:
     """Draw a shadow underneath/behind this container.
 
     This is a globally configurable version of the
     :py:class:`prompt_toolkit.widows.base.Shadow` class.
     """
 
-    def __init__(self, body: "AnyContainer") -> "None":
+    def __init__(self, body: AnyContainer) -> None:
         """Initialize a new drop-shadow container.
 
         Args:
             body: Another container object.
         """
         filter_ = get_app().config.filter("show_shadows")
         shadow = FloatContainer(
@@ -576,23 +568,23 @@
                     right=-1,
                     transparent=True,
                     content=DropShadow(),
                 ),
             ],
         )
 
-        def get_contents() -> "AnyContainer":
+        def get_contents() -> AnyContainer:
             if filter_():
                 return shadow
             else:
                 return body
 
         self.container = DynamicContainer(get_contents)
 
-    def __pt_container__(self) -> "AnyContainer":
+    def __pt_container__(self) -> AnyContainer:
         """Return the container's content."""
         return self.container
 
     # ################################### Settings ####################################
 
     add_setting(
         name="show_shadows",
```

### Comparing `euporie-2.3.2/euporie/core/widgets/dialog.py` & `euporie-2.4.0/euporie/core/widgets/dialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,27 @@
 
 from __future__ import annotations
 
 import logging
 import traceback
 from abc import ABCMeta, abstractmethod
 from functools import partial
+from pathlib import Path
 from typing import TYPE_CHECKING
 
 from prompt_toolkit.cache import SimpleCache
 from prompt_toolkit.clipboard import ClipboardData
 from prompt_toolkit.completion import PathCompleter
 from prompt_toolkit.data_structures import Point
-from prompt_toolkit.filters import Condition, has_completions, has_focus
+from prompt_toolkit.filters import (
+    Condition,
+    buffer_has_focus,
+    has_completions,
+    has_focus,
+)
 from prompt_toolkit.formatted_text import AnyFormattedText, to_formatted_text
 from prompt_toolkit.formatted_text.utils import split_lines
 from prompt_toolkit.key_binding.bindings.focus import focus_next, focus_previous
 from prompt_toolkit.key_binding.key_bindings import DynamicKeyBindings, KeyBindings
 from prompt_toolkit.layout.containers import (
     ConditionalContainer,
     DynamicContainer,
@@ -27,14 +33,15 @@
 )
 from prompt_toolkit.layout.controls import FormattedTextControl, UIContent, UIControl
 from prompt_toolkit.layout.dimension import Dimension
 from prompt_toolkit.layout.screen import WritePosition
 from prompt_toolkit.mouse_events import MouseButton, MouseEventType
 from prompt_toolkit.widgets.base import Box, Label
 
+from euporie.core.app import get_app
 from euporie.core.border import (
     FullLine,
     LowerLeftHalfLine,
     UpperRightHalfLine,
 )
 from euporie.core.commands import add_cmd
 from euporie.core.filters import tab_has_focus
@@ -54,14 +61,15 @@
     from prompt_toolkit.key_binding.key_processor import KeyPressEvent
     from prompt_toolkit.layout.containers import AnyContainer
     from prompt_toolkit.layout.layout import FocusableElement
     from prompt_toolkit.mouse_events import MouseEvent
 
     from euporie.core.app import BaseApp
     from euporie.core.tabs.base import KernelTab
+    from euporie.core.widgets.file_browser import FileBrowserControl
 
 log = logging.getLogger(__name__)
 
 
 DialogGrid = (
     FullLine.left_edge
     + FullLine.right_edge
@@ -180,22 +188,31 @@
 
         # Set default body & buttons
         self.body: AnyContainer = Window()
         self.buttons: dict[str, Callable | None] = {"OK": None}
         self.button_widgets: list[AnyContainer] = []
 
         # Create key-bindings
-        self.kb = KeyBindings()
-        self.kb.add("escape")(lambda event: self.hide())
-        self.kb.add("tab", filter=~has_completions)(focus_next)
-        self.kb.add("s-tab", filter=~has_completions)(focus_previous)
+        kb = KeyBindings()
+        kb.add("escape")(lambda event: self.hide())
+        kb.add("tab", filter=~has_completions)(focus_next)
+        kb.add("s-tab", filter=~has_completions)(focus_previous)
+
+        @kb.add("enter", filter=~has_completions & ~buffer_has_focus)
+        def _focus_button(event: KeyPressEvent) -> NotImplementedOrNone:
+            if self.button_widgets:
+                app.layout.focus(self.button_widgets[0])
+                return None
+            return NotImplemented
+
+        self.kb = kb
         self.buttons_kb = KeyBindings()
 
         # Create title row
-        title_window = Window(height=1, style="class:dialog,title")
+        title_window = Window(height=1, style="class:dialog,dialog-title")
         title_window.content = DialogTitleControl(
             lambda: self.title, self, title_window
         )
         title_row = ConditionalContainer(
             title_window, filter=Condition(lambda: bool(self.title))
         )
 
@@ -230,15 +247,15 @@
                         [
                             title_row,
                             body_row,
                             buttons_row,
                         ],
                         style="class:dialog,body",
                         key_bindings=self.kb,
-                        modal=True,
+                        modal=False,
                     ),
                     border=DialogGrid,
                     style="class:dialog,border",
                 ),
             ),
             filter=self.visible,
         )
@@ -448,14 +465,15 @@
             "OK": partial(self.validate, self.filepath.buffer, tab=tab, cb=cb),
             "Cancel": None,
         }
         self.file_browser.control.on_open._handlers.clear()
         self.file_browser.control.on_open += lambda path: self.validate(
             self.filepath.buffer, tab=tab, cb=cb
         )
+        self.file_browser.control.selected = None
         self.error = error
         self.to_focus = self.filepath
 
     def validate(
         self, buffer: Buffer, tab: Tab | None, cb: Callable | None = None
     ) -> None:
         """Validate the input."""
@@ -463,31 +481,73 @@
 
 
 class OpenFileDialog(FileDialog):
     """A dialog which prompts the user for a filepath to open."""
 
     title = "Select a File to Open"
 
+    def __init__(self, app: BaseApp) -> None:
+        """Additional body components."""
+        from euporie.core.widgets.forms import Dropdown
+
+        super().__init__(app)
+
+        self.tab_dd = tab_dd = Dropdown(options=[])
+
+        def _update_options(fb: FileBrowserControl) -> None:
+            tabs = get_app().get_file_tabs(path) if (path := fb.path).is_file() else []
+            tab_dd.options = tabs
+            tab_dd.labels = [tab.name for tab in tabs]
+
+        self.file_browser.control.on_select += _update_options
+
+        if isinstance(self.body, HSplit):
+            self.body.children.append(
+                ConditionalContainer(
+                    FocusedStyle(LabelledWidget(tab_dd, "Open with:")),
+                    filter=Condition(lambda: len(tab_dd.options) > 1),
+                )
+            )
+
+    def load(
+        self,
+        text: str = "",
+        tab: Tab | None = None,
+        error: str = "",
+        cb: Callable | None = None,
+    ) -> None:
+        """Load the dialog body."""
+        super().load(text=text, tab=tab, error=error, cb=cb)
+        self.tab_dd.options = []
+        self.tab_dd.labels = []
+
     def validate(
         self, buffer: Buffer, tab: Tab | None, cb: Callable | None = None
     ) -> None:
         """Validate the the file to open exists."""
-        from euporie.core.utils import parse_path
+        from upath import UPath
+
+        from euporie.core.path import parse_path
 
         path = parse_path(self.file_browser.control.dir / buffer.text)
         if path is not None:
-            if str(path).startswith("http") or path.is_file():
-                self.hide()
-                self.app.open_file(path)
-            elif not path.exists():
+            if not path.exists():
+                path = UPath(buffer.text)
+
+            if path.exists():
+                if path.is_dir():
+                    self.file_browser.control.dir = path
+                elif path.is_file():
+                    self.hide()
+                    self.app.open_file(path, tab_class=self.tab_dd.value)
+                return
+            else:
                 self.show(
                     error="The file path specified does not exist", text=buffer.text
                 )
-            elif path.is_dir():
-                self.file_browser.control.dir = path
 
     # ################################### Commands ####################################
 
     @staticmethod
     @add_cmd(menu_title="Open File…")
     def _open_file() -> None:
         """Open a file."""
@@ -512,15 +572,15 @@
 
     title = "Select a Path to Save"
 
     def validate(
         self, buffer: Buffer, tab: Tab | None, cb: Callable | None = None
     ) -> None:
         """Validate the the file to open exists."""
-        from euporie.core.utils import parse_path
+        from euporie.core.path import parse_path
 
         path = parse_path(self.file_browser.control.dir / buffer.text)
         if tab and path is not None:
             if path.is_dir():
                 self.file_browser.control.dir = path
             else:
                 tab.save(path=path)
@@ -585,48 +645,84 @@
     """A dialog which allows the user to select a kernel."""
 
     title = "Select Kernel"
 
     def load(
         self,
         kernel_specs: dict[str, Any] | None = None,
+        runtime_dirs: dict[str, Path] | None = None,
         tab: KernelTab | None = None,
         message: str = "",
     ) -> None:
         """Load dialog body & buttons."""
+        from jupyter_core.paths import jupyter_runtime_dir
+
+        from euporie.core.widgets.layout import TabbedSplit
+
         kernel_specs = kernel_specs or {}
+        runtime_dirs = runtime_dirs or {}
 
-        options = Select(
+        options_specs = Select(
             options=list(kernel_specs.keys()),
             labels=[
                 kernel_spec.get("spec", {}).get("display_name", kernel_name)
                 for kernel_name, kernel_spec in kernel_specs.items()
             ],
             style="class:input,radio-buttons",
             prefix=("○", "◉"),
             multiple=False,
             border=None,
             rows=5,
             dont_extend_width=False,
         )
+        self.to_focus = options_specs
 
-        msg_ft = (f"{message}\n" if message else "") + "Please select a kernel:\n"
+        connection_files = {
+            path.name: path
+            for path in Path(jupyter_runtime_dir()).glob("kernel-*.json")
+        }
+        options_files = Select(
+            options=list(connection_files.values()),
+            labels=list(connection_files.keys()),
+            style="class:input,radio-buttons",
+            prefix=("○", "◉"),
+            multiple=False,
+            border=None,
+            rows=5,
+            dont_extend_width=False,
+        )
+
+        msg_ft = (f"{message}\n\n" if message else "") + "Please select a kernel:"
 
         self.body = HSplit(
             [
                 Label(msg_ft),
-                FocusedStyle(options),
+                tabs := TabbedSplit(
+                    [
+                        FocusedStyle(options_specs),
+                        FocusedStyle(options_files),
+                    ],
+                    titles=["New", "Existing"],
+                    width=Dimension(min=30),
+                ),
             ]
         )
 
         def _change_kernel() -> None:
             self.hide()
             assert tab is not None
-            name = options.options[options.index or 0]
-            tab.kernel.change(name, cb=tab.kernel_started)
+            if tabs.active == 0:
+                name = options_specs.value
+                connection_file = None
+            else:
+                name = None
+                connection_file = options_files.value
+            tab.kernel.change(
+                name=name, connection_file=connection_file, cb=tab.kernel_started
+            )
 
         self.buttons = {
             "Select": _change_kernel,
             "Cancel": None,
         }
 
 
@@ -668,14 +764,15 @@
 class ErrorDialog(Dialog):
     """A dialog to show unhandled exceptions."""
 
     title = "Error"
 
     def load(self, exception: Exception | None = None, when: str = "") -> None:
         """Load dialog body & buttons."""
+        from euporie.core.margins import MarginContainer, ScrollbarMargin
         from euporie.core.widgets.formatted_text_area import FormattedTextArea
         from euporie.core.widgets.forms import Checkbox
 
         if exception is None:
             exception = Exception("Unspecified Error")
 
         checkbox = Checkbox(
@@ -701,20 +798,25 @@
                         ]
                     )
                 ),
                 FocusedStyle(
                     Box(checkbox, padding_left=0),
                 ),
                 ConditionalContainer(
-                    FormattedTextArea(
-                        lex([("", tb_text)], "pytb"),
-                        width=80,
-                        height=Dimension(min=10),
-                        wrap_lines=False,
-                        style="",
+                    VSplit(
+                        [
+                            fta := FormattedTextArea(
+                                lex([("", tb_text)], "pytb"),
+                                width=80,
+                                height=Dimension(min=10),
+                                wrap_lines=False,
+                                style="",
+                            ),
+                            MarginContainer(ScrollbarMargin(), target=fta.window),
+                        ]
                     ),
                     filter=Condition(lambda: checkbox.selected),
                 ),
             ]
         )
 
         def _copy_traceback() -> None:
@@ -771,29 +873,31 @@
         """Create a new shortcuts dialog instance."""
         super().__init__(app)
         self.details: StyleAndTextTuples | None = None
 
     def load(self, *args: Any, **kwargs: Any) -> None:
         """Load the dialog body."""
         from euporie.core.formatted_text.utils import max_line_width
+        from euporie.core.margins import MarginContainer, ScrollbarMargin
         from euporie.core.widgets.formatted_text_area import FormattedTextArea
 
         if not self.details:
             self.details = self.format_key_info()
         assert self.details is not None
 
         width = max_line_width(self.details)
 
-        self.body = FormattedTextArea(
+        fta = FormattedTextArea(
             formatted_text=self.details,
             multiline=True,
             focusable=True,
             wrap_lines=False,
-            width=width,
+            width=width - 2,
         )
+        self.body = VSplit([fta, MarginContainer(ScrollbarMargin(), target=fta.window)])
 
     def format_key_info(self) -> StyleAndTextTuples:
         """Generate a table with the current key bindings."""
         import importlib
         from textwrap import dedent
 
         from prompt_toolkit.formatted_text.base import to_formatted_text
```

### Comparing `euporie-2.3.2/euporie/core/widgets/display.py` & `euporie-2.4.0/euporie/core/widgets/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,53 +12,52 @@
 from prompt_toolkit.cache import SimpleCache
 from prompt_toolkit.data_structures import Point
 from prompt_toolkit.filters.app import has_completions
 from prompt_toolkit.filters.base import Condition
 from prompt_toolkit.filters.utils import to_filter
 from prompt_toolkit.formatted_text.base import to_formatted_text
 from prompt_toolkit.formatted_text.utils import fragment_list_width, split_lines
-from prompt_toolkit.layout.containers import Float, Window
+from prompt_toolkit.layout.containers import ConditionalContainer, Float, VSplit, Window
 from prompt_toolkit.layout.controls import GetLinePrefixCallable, UIContent, UIControl
-from prompt_toolkit.layout.margins import ConditionalMargin
 from prompt_toolkit.layout.mouse_handlers import MouseHandlers
 from prompt_toolkit.layout.screen import Char, WritePosition
 from prompt_toolkit.mouse_events import MouseEvent, MouseEventType
 from prompt_toolkit.utils import Event
 
 from euporie.core.commands import add_cmd
-from euporie.core.convert.base import convert, find_route
+from euporie.core.convert.core import convert, find_route
 from euporie.core.convert.utils import data_pixel_size, pixels_to_cell_size
 from euporie.core.current import get_app
 from euporie.core.data_structures import DiInt
 from euporie.core.filters import (
     display_has_focus,
     has_dialog,
     has_menus,
     in_tmux,
     scrollable,
 )
 from euporie.core.key_binding.registry import (
     load_registered_bindings,
     register_bindings,
 )
-from euporie.core.margins import ScrollbarMargin
+from euporie.core.margins import MarginContainer, ScrollbarMargin
 from euporie.core.terminal import tmuxify
 from euporie.core.widgets.page import BoundedWritePosition
 
 if TYPE_CHECKING:
+    from pathlib import Path
     from typing import Any, Callable, Iterable
 
     from prompt_toolkit.filters import FilterOrBool
     from prompt_toolkit.formatted_text import StyleAndTextTuples
     from prompt_toolkit.key_binding import KeyBindingsBase
     from prompt_toolkit.key_binding.key_bindings import NotImplementedOrNone
-    from prompt_toolkit.layout.containers import AnyContainer, WindowRenderInfo
+    from prompt_toolkit.layout.containers import AnyContainer
     from prompt_toolkit.layout.dimension import AnyDimension
     from prompt_toolkit.layout.screen import Screen
-    from upath import UPath
 
 
 log = logging.getLogger(__name__)
 
 
 class DisplayControl(UIControl):
     """A data formatter, which displays cell output data.
@@ -67,15 +66,15 @@
     events - i.e. images are downscaled to fit, markdown is re-flowed, etc.
     """
 
     def __init__(
         self,
         data: Any,
         format_: str,
-        path: UPath | None = None,
+        path: Path | None = None,
         fg_color: str | None = None,
         bg_color: str | None = None,
         sizing_func: Callable[[], tuple[int, float]] | None = None,
         focusable: FilterOrBool = False,
         focus_on_click: FilterOrBool = False,
     ) -> None:
         """Create a new data formatter control.
@@ -98,19 +97,20 @@
         self.fg_color = fg_color
         self.bg_color = bg_color
         self.focusable = to_filter(focusable)
         self.focus_on_click = to_filter(focus_on_click)
         self.key_bindings = load_registered_bindings(
             "euporie.core.widgets.display.Display"
         )
+        self._cursor_position = Point(x=0, y=0)
+        self.dy = 0
         self.app = get_app()
 
+        self.on_data_changed = Event(self)
         self.on_cursor_position_changed = Event(self)
-        self._cursor_position = Point(x=0, y=0)
-        self.dy = 0
 
         self.sizing_func = sizing_func or (lambda: (0, 0))
         self._max_cols = 0
         self._aspect = 0.0
 
         self.rendered_lines: list[StyleAndTextTuples] = []
         self._format_cache: SimpleCache = SimpleCache(maxsize=50)
@@ -129,14 +129,15 @@
         return self._data
 
     @data.setter
     def data(self, value: Any) -> None:
         """Set the control's data."""
         self._data = value
         self.reset()
+        self.on_data_changed.fire()
 
     def get_key_bindings(self) -> KeyBindingsBase | None:
         """Return the control's key bindings."""
         return self.key_bindings
 
     @property
     def cursor_position(self) -> Point:
@@ -272,14 +273,15 @@
             self.app.layout.current_control = self
             return None
         return NotImplemented
 
     def get_invalidate_events(self) -> Iterable[Event[object]]:
         """Return the Window invalidate events."""
         # Whenever the cursor position changes, the UI has to be updated.
+        yield self.on_data_changed
         yield self.on_cursor_position_changed
 
     @property
     def content_width(self) -> int:
         """Return the maximum line length of the content."""
         return max(fragment_list_width(line) for line in self.rendered_lines)
 
@@ -289,15 +291,14 @@
             self.hide()
 
 
 class DisplayWindow(Window):
     """A window sub-class which can scroll left and right."""
 
     content: DisplayControl
-    render_info: WindowRenderInfo
     vertical_scroll: int
 
     def _write_to_screen_at_index(
         self,
         screen: Screen,
         mouse_handlers: MouseHandlers,
         write_position: WritePosition,
@@ -384,15 +385,15 @@
 class GraphicControl(DisplayControl, metaclass=ABCMeta):
     """A base-class for display controls which render terminal graphics."""
 
     def __init__(
         self,
         data: Any,
         format_: str,
-        path: UPath | None = None,
+        path: Path | None = None,
         fg_color: str | None = None,
         bg_color: str | None = None,
         sizing_func: Callable[[], tuple[int, float]] | None = None,
         focusable: FilterOrBool = False,
         focus_on_click: FilterOrBool = False,
         scale: float = 0,
         bbox: DiInt | None = None,
@@ -628,15 +629,15 @@
 class KittyGraphicControl(GraphicControl):
     """A graphic control which displays images using Kitty's graphics protocol."""
 
     def __init__(
         self,
         data: Any,
         format_: str,
-        path: UPath | None = None,
+        path: Path | None = None,
         fg_color: str | None = None,
         bg_color: str | None = None,
         sizing_func: Callable[[], tuple[int, float]] | None = None,
         focusable: FilterOrBool = False,
         focus_on_click: FilterOrBool = False,
         scale: float = 0,
         bbox: DiInt | None = None,
@@ -953,15 +954,15 @@
     """A :py:class:`Float` which displays a graphic."""
 
     def __init__(
         self,
         target_window: Window,
         data: Any,
         format_: str,
-        path: UPath | None = None,
+        path: Path | None = None,
         fg_color: str | None = None,
         bg_color: str | None = None,
         sizing_func: Callable[[], tuple[int, float]] | None = None,
         filter: FilterOrBool = True,
     ) -> None:
         """Create a new instance.
 
@@ -1049,27 +1050,53 @@
     def data(self, value: Any) -> None:
         """Set the graphic float's data."""
         self._data = value
         if self.control is not None:
             self.control.data = value
             self.control.reset()
 
+    @property
+    def format_(self) -> str:
+        """Return the graphic's current data format."""
+        if self.control is not None:
+            return self.control.format_
+        return ""
+
+    @format_.setter
+    def format_(self, value: str) -> None:
+        """Set the graphic float's data format."""
+        if self.control is not None:
+            self.control.format_ = value
+
+    @property
+    def path(self) -> Path | None:
+        """Return the graphic's current data path."""
+        if self.control is not None:
+            return self.control.path
+        return None
+
+    @path.setter
+    def path(self, value: Path | None) -> None:
+        """Set the graphic float's data path."""
+        if self.control is not None:
+            self.control.path = value
+
 
 class Display:
     """Rich output displays.
 
     A container for displaying rich output data.
 
     """
 
     def __init__(
         self,
         data: Any,
         format_: str,
-        path: UPath | None = None,
+        path: Path | None = None,
         fg_color: str | None = None,
         bg_color: str | None = None,
         height: AnyDimension = None,
         width: AnyDimension = None,
         px: int | None = None,
         py: int | None = None,
         focusable: FilterOrBool = False,
@@ -1134,24 +1161,27 @@
             wrap_lines=wrap_lines,
             always_hide_cursor=always_hide_cursor,
             dont_extend_height=dont_extend_height,
             style=self.style,
             char=" ",
         )
 
-        self.window.right_margins = [
-            ConditionalMargin(
-                ScrollbarMargin(),
-                filter=to_filter(scrollbar)
-                & (
-                    ~to_filter(scrollbar_autohide)
-                    | (to_filter(scrollbar_autohide) & scrollable(self.window))
+        self.container = VSplit(
+            [
+                self.window,
+                ConditionalContainer(
+                    MarginContainer(ScrollbarMargin(), target=self.window),
+                    filter=to_filter(scrollbar)
+                    & (
+                        ~to_filter(scrollbar_autohide)
+                        | (to_filter(scrollbar_autohide) & scrollable(self.window))
+                    ),
                 ),
-            )
-        ]
+            ]
+        )
 
         # Add graphic
         app = get_app()
         self.graphic_float = GraphicFloat(
             target_window=self.window,
             data=data,
             format_=format_,
@@ -1171,14 +1201,36 @@
 
     @data.setter
     def data(self, value: Any) -> None:
         """Set the display container's data."""
         self.control.data = value
         self.graphic_float.data = value
 
+    @property
+    def format_(self) -> str:
+        """Return the display's current data format."""
+        return self.control.format_
+
+    @format_.setter
+    def format_(self, value: str) -> None:
+        """Set the display container's data format."""
+        self.control.format_ = value
+        self.graphic_float.format_ = value
+
+    @property
+    def path(self) -> Path | None:
+        """Return the display's current data path."""
+        return self.control.path
+
+    @path.setter
+    def path(self, value: Path | None) -> None:
+        """Set the display container's data path."""
+        self.control.path = value
+        self.graphic_float.path = value
+
     def make_sizing_func(
         self, data: Any, format_: str, fg: str | None, bg: str | None
     ) -> Callable[[], tuple[int, float]]:
         """Create a function to recalculate the data's dimensions in terminal cells."""
         px, py = self.px, self.py
         if px is None or py is None:
             px, py = data_pixel_size(data, format_, fg=fg, bg=bg)
@@ -1218,15 +1270,15 @@
         self.control.reset()
         if self.graphic_float.control is not None:
             self.graphic_float.control.sizing_func = sizing_func
             self.graphic_float.control.reset()
 
     def __pt_container__(self) -> AnyContainer:
         """Return the content of this output."""
-        return self.window
+        return self.container
 
     # ################################### Commands ####################################
 
     @staticmethod
     @add_cmd(filter=display_has_focus)
     def _scroll_display_left() -> None:
         """Scroll the display up one line."""
```

### Comparing `euporie-2.3.2/euporie/core/widgets/file_browser.py` & `euporie-2.4.0/euporie/core/widgets/file_browser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 """Define a file browser widget."""
 
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
-from prompt_toolkit.application.current import get_app
 from prompt_toolkit.buffer import Buffer
 from prompt_toolkit.cache import FastDictCache
 from prompt_toolkit.completion import PathCompleter
 from prompt_toolkit.data_structures import Point
 from prompt_toolkit.filters.utils import to_filter
 from prompt_toolkit.key_binding.key_bindings import KeyBindings, KeyBindingsBase
 from prompt_toolkit.key_binding.key_processor import KeyPressEvent
 from prompt_toolkit.layout.containers import (
     ConditionalContainer,
     HSplit,
     VSplit,
     Window,
 )
 from prompt_toolkit.layout.controls import UIContent, UIControl
-from prompt_toolkit.mouse_events import MouseEvent, MouseEventType
+from prompt_toolkit.layout.screen import WritePosition
+from prompt_toolkit.mouse_events import MouseButton, MouseEvent, MouseEventType
 from prompt_toolkit.utils import Event
 from upath import UPath
 
-from euporie.core.border import InnerEigthGrid
-from euporie.core.margins import ScrollbarMargin
+from euporie.core.app import get_app
+from euporie.core.border import InsetGrid
+from euporie.core.margins import MarginContainer, ScrollbarMargin
 from euporie.core.widgets.decor import Border, FocusedStyle
 from euporie.core.widgets.forms import Button, Text
 
 if TYPE_CHECKING:
+    from pathlib import Path
     from typing import Callable
 
     from prompt_toolkit.filters.base import FilterOrBool
     from prompt_toolkit.formatted_text import StyleAndTextTuples
     from prompt_toolkit.key_binding.key_bindings import NotImplementedOrNone
     from prompt_toolkit.layout.containers import AnyContainer
     from prompt_toolkit.layout.dimension import AnyDimension
     from upath.core import PT
 
+    from euporie.core.widgets.status_bar import StatusBarFields
+
 log = logging.getLogger(__name__)
 
 
 FILE_ICONS = {
     # default
     "file": "",
     "dir": "",
@@ -345,44 +349,47 @@
     ".pdf": "",
     ".doc": "",
     ".docx": "",
     ".ipynb": "ﴬ",
 }
 
 
-def is_dir(path: str | UPath) -> bool | None:
+def is_dir(path: str | Path) -> bool | None:
     """Check if a path is a directory."""
     test_path = UPath(path)
     try:
         return test_path.is_dir()
     except (ValueError, PermissionError, TypeError):
         return None
 
 
 class FileBrowserControl(UIControl):
     """A control for browsing a filesystem."""
 
     def __init__(
         self,
-        path: UPath | None = None,
+        path: Path | None = None,
         on_chdir: Callable[[FileBrowserControl], None] | None = None,
         on_select: Callable[[FileBrowserControl], None] | None = None,
         on_open: Callable[[FileBrowserControl], None] | None = None,
+        window: Window | None = None,
     ) -> None:
         """Initialize a new file browser instance."""
         self.dir = path or UPath(".")
-        self.hovered: int = 0
+        self.hovered: int | None = None
         self.selected: int | None = None
         self._dir_cache: FastDictCache[
-            tuple[UPath], list[tuple[bool, UPath]]
+            tuple[Path], list[tuple[bool, Path]]
         ] = FastDictCache(get_value=self.load_path, size=1)
         self.on_select = Event(self, on_select)
         self.on_chdir = Event(self, on_chdir)
         self.on_open = Event(self, on_open)
 
+        self.window = window
+
         self.on_chdir.fire()
 
         self.key_bindings = kb = KeyBindings()
 
         @kb.add("up")
         @kb.add("<scroll-up>")
         def _move_up(event: KeyPressEvent) -> None:
@@ -408,20 +415,20 @@
         @kb.add("space")
         @kb.add("enter")
         @kb.add("right")
         def _open(event: KeyPressEvent) -> None:
             return self.open_path()
 
     @property
-    def contents(self) -> list[tuple[bool, UPath]]:
+    def contents(self) -> list[tuple[bool, Path]]:
         """Return the contents of the current folder."""
         return self._dir_cache[(self.dir,)]
 
     @property
-    def dir(self) -> UPath:
+    def dir(self) -> Path:
         """Return the current folder path."""
         return self._dir
 
     @dir.setter
     def dir(self, value: PT) -> None:
         """Set the current folder path."""
         dir_path = UPath(value)
@@ -431,20 +438,20 @@
             pass
         if is_dir(dir_path):
             self._dir = dir_path
         else:
             log.warning("'%s' is not a directory, not changing directory", value)
 
     @property
-    def path(self) -> UPath:
+    def path(self) -> Path:
         """Return the current selected path."""
         return self.contents[self.selected or 0][1]
 
     @staticmethod
-    def load_path(path: UPath) -> list[tuple[bool, UPath]]:
+    def load_path(path: Path) -> list[tuple[bool, Path]]:
         """Return the contents of a folder."""
         paths = [] if path.parent == path else [path / ".."]
         try:
             paths += list(path.iterdir())
         except PermissionError:
             pass
         is_dirs = []
@@ -485,19 +492,50 @@
             cursor_position=Point(0, self.selected or 0),
             show_cursor=False,
         )
 
     def mouse_handler(self, mouse_event: MouseEvent) -> NotImplementedOrNone:
         """Handle mouse events."""
         row = mouse_event.position.y
-        if mouse_event.event_type == MouseEventType.MOUSE_DOWN:
-            get_app().layout.current_control = self
+        app = get_app()
+        if (
+            mouse_event.button == MouseButton.LEFT
+            and mouse_event.event_type == MouseEventType.MOUSE_DOWN
+        ):
+            app.layout.current_control = self
+            app.mouse_limits = None
+            self.hovered = None
             return self.select(row, open_file=True)
         elif mouse_event.event_type == MouseEventType.MOUSE_MOVE:
-            return self.hover(row)
+            # Mark item as hovered if mouse is over the control
+            if (
+                self.window is not None
+                and (info := self.window.render_info) is not None
+            ):
+                rowcol_to_yx = info._rowcol_to_yx
+                abs_mouse_pos = (
+                    mouse_event.position.x + info._x_offset,
+                    mouse_event.position.y + info._y_offset - info.vertical_scroll,
+                )
+                if abs_mouse_pos == app.mouse_position:
+                    row_col_vals = rowcol_to_yx.values()
+                    y_min, x_min = min(row_col_vals)
+                    y_max, x_max = max(row_col_vals)
+                    app.mouse_limits = WritePosition(
+                        xpos=x_min,
+                        ypos=y_min,
+                        width=x_max - x_min + 1,
+                        height=y_max - y_min + 1,
+                    )
+                    return self.hover(row)
+                else:
+                    # Clear mouse limits if mouse is outside control
+                    app.mouse_limits = None
+                    self.hovered = None
+                    return None
 
         return NotImplemented
 
     def select(self, row: int | None, open_file: bool = False) -> NotImplementedOrNone:
         """Select a file in the browser."""
         if row is None:
             row = 0
@@ -505,20 +543,21 @@
         if self.selected != row:
             self.selected = row
             self.on_select.fire()
         elif open_file:
             self.open_path()
         return None
 
-    def hover(self, row: int) -> NotImplementedOrNone:
+    def hover(self, row: int | None) -> NotImplementedOrNone:
         """Hover a file in the browser."""
-        row = min(max(0, row), len(self.contents) - 1)
-        if self.hovered != row:
-            self.hovered = row
-            return None
+        if row is not None:
+            row = min(max(0, row), len(self.contents) - 1)
+            if self.hovered != row:
+                self.hovered = row
+                return None
         return NotImplemented
 
     def open_path(self) -> None:
         """Open the selected file."""
         if self.selected is not None:
             is_dir, path = self.contents[self.selected]
             if is_dir:
@@ -551,48 +590,55 @@
         """Key bindings specific to this user control."""
         return self.key_bindings
 
     def is_focusable(self) -> bool:
         """Determine that the file_browser is focusable."""
         return True
 
+    def __pt_status__(self) -> StatusBarFields:
+        """Show the selected or hovered path in the statusbar."""
+        if self.hovered is not None:
+            return [[("", str(self.contents[self.hovered][1]))]], []
+        elif self.selected is not None:
+            return [[("", str(self.contents[self.selected][1]))]], []
+        return [], []
+
 
 class FileBrowser:
     """A file browser."""
 
     completer = PathCompleter(only_directories=True)
 
     def __init__(
         self,
-        path: UPath | None = None,
-        on_select: Callable[[UPath], None] | None = None,
-        on_open: Callable[[UPath], None] | None = None,
-        on_chdir: Callable[[UPath], None] | None = None,
+        path: Path | None = None,
+        on_select: Callable[[Path], None] | None = None,
+        on_open: Callable[[Path], None] | None = None,
+        on_chdir: Callable[[Path], None] | None = None,
         width: AnyDimension = None,
         height: AnyDimension = None,
         style: str = "",
         show_address_bar: FilterOrBool = True,
     ) -> None:
         """Create a new instance."""
 
         def _accept_path(buffer: Buffer) -> bool:
-            control.dir = UPath(buffer.text)
+            control.dir = Path(buffer.text)
             return True
 
         def _validate_path(path: str) -> bool:
             return is_dir(path) or False
 
         text = Text(
             validation=_validate_path,
             accept_handler=_accept_path,
             completer=self.completer,
         )
         self.control = control = FileBrowserControl(
             path=path,
-            on_open=lambda x: log.debug(x.path),
             on_chdir=lambda x: setattr(text, "text", str(x.dir)),
         )
         if on_select is not None:
             control.on_select += (
                 lambda x: on_select(x.path) if callable(on_select) else None
             )
         if on_chdir is not None:
@@ -618,26 +664,36 @@
                             ),
                         ]
                     ),
                     filter=to_filter(show_address_bar),
                 ),
                 FocusedStyle(
                     Border(
-                        Window(
-                            control,
-                            style="class:face",
-                            right_margins=[ScrollbarMargin()],
+                        VSplit(
+                            [
+                                window := Window(
+                                    control,
+                                    style="class:face",
+                                ),
+                                MarginContainer(ScrollbarMargin(), target=window),
+                            ]
                         ),
-                        border=InnerEigthGrid,
+                        border=InsetGrid,
                         style="class:input,inset,border",
                     ),
                     style_hover="",
                 ),
             ],
             style="class:file-browser " + style,
             width=width,
             height=height,
         )
+        # Set control's window so it can determine it's position for mouse-over
+        control.window = window
 
     def __pt_container__(self) -> AnyContainer:
         """Return the tree-view container's content."""
         return self.container
+
+    def __pt_status__(self) -> StatusBarFields:
+        """Show the selected or hovered path in the statusbar."""
+        return self.control.__pt_status__()
```

### Comparing `euporie-2.3.2/euporie/core/widgets/formatted_text_area.py` & `euporie-2.4.0/euporie/core/widgets/formatted_text_area.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     split_lines,
     to_formatted_text,
 )
 from prompt_toolkit.layout.margins import ConditionalMargin
 from prompt_toolkit.layout.processors import DynamicProcessor, Processor, Transformation
 from prompt_toolkit.widgets import TextArea
 
-from euporie.core.margins import NumberedDiffMargin, ScrollbarMargin
+from euporie.core.margins import NumberedDiffMargin
 
 if TYPE_CHECKING:
     from typing import Any
 
     from prompt_toolkit.filters import FilterOrBool
     from prompt_toolkit.formatted_text import AnyFormattedText, StyleAndTextTuples
     from prompt_toolkit.layout.processors import TransformationInput
@@ -94,16 +94,14 @@
         # Set the left margins
         self.window.left_margins = [
             ConditionalMargin(
                 NumberedDiffMargin(),
                 self.line_numbers,
             )
         ]
-        # Add auto scrollbar
-        self.window.right_margins = [ScrollbarMargin(display_arrows=False)]
         # Set the formatted text to display
         self._set_formatted_text(formatted_text)
 
     @property
     def formatted_text(self) -> StyleAndTextTuples:
         """The formatted text."""
         ft = to_formatted_text(self._formatted_text)
```

### Comparing `euporie-2.3.2/euporie/core/widgets/forms.py` & `euporie-2.4.0/euporie/core/widgets/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import asyncio
 import logging
 from abc import ABCMeta, abstractmethod
 from collections import deque
 from functools import partial
 from math import ceil, floor
-from typing import TYPE_CHECKING, cast
+from typing import TYPE_CHECKING, Dict, cast
 from weakref import finalize
 
 from prompt_toolkit.buffer import ValidationState
 from prompt_toolkit.cache import SimpleCache
 from prompt_toolkit.completion.base import ConditionalCompleter
 from prompt_toolkit.completion.word_completer import WordCompleter
 from prompt_toolkit.filters import (
@@ -26,15 +26,15 @@
 from prompt_toolkit.formatted_text.base import to_formatted_text
 from prompt_toolkit.formatted_text.utils import fragment_list_len, fragment_list_width
 from prompt_toolkit.key_binding.key_bindings import (
     ConditionalKeyBindings,
     KeyBindings,
     merge_key_bindings,
 )
-from prompt_toolkit.layout.containers import ConditionalContainer, Float, Window
+from prompt_toolkit.layout.containers import ConditionalContainer, Float, VSplit, Window
 from prompt_toolkit.layout.controls import (
     BufferControl,
     FormattedTextControl,
     UIContent,
     UIControl,
 )
 from prompt_toolkit.layout.dimension import Dimension
@@ -42,19 +42,19 @@
 from prompt_toolkit.layout.screen import WritePosition
 from prompt_toolkit.layout.utils import explode_text_fragments
 from prompt_toolkit.mouse_events import MouseButton, MouseEvent, MouseEventType
 from prompt_toolkit.utils import Event
 from prompt_toolkit.validation import Validator
 from prompt_toolkit.widgets.base import Box, TextArea
 
-from euporie.core.border import InnerEigthGrid
+from euporie.core.border import InsetGrid
 from euporie.core.current import get_app
 from euporie.core.data_structures import DiBool
 from euporie.core.formatted_text.utils import FormattedTextAlign, align
-from euporie.core.margins import ScrollbarMargin
+from euporie.core.margins import MarginContainer, ScrollbarMargin
 from euporie.core.widgets.decor import Border, Shadow
 from euporie.core.widgets.layout import ConditionalSplit
 
 if TYPE_CHECKING:
     from typing import Any, Callable, Sequence
 
     from prompt_toolkit.buffer import Buffer, BufferAcceptHandler
@@ -91,15 +91,15 @@
 
     def __init__(
         self,
         color: str | Callable[[], str] = "#FFFFFF",
         width: int = 2,
         height: int = 1,
         style: str = "class:swatch",
-        border: GridStyle = InnerEigthGrid,
+        border: GridStyle = InsetGrid,
         show_borders: DiBool | None = None,
     ) -> None:
         """Create a new instance of the color swatch.
 
         Args:
             color: A function or string which gives color to display
             width: The width of the color swatch (excluding the border)
@@ -139,15 +139,15 @@
         self,
         text: AnyFormattedText,
         on_click: Callable[[Button], None] | None = None,
         on_mouse_down: Callable[[Button], None] | None = None,
         disabled: FilterOrBool = False,
         width: int | None = None,
         style: str | Callable[[], str] = "class:input",
-        border: GridStyle | None = InnerEigthGrid,
+        border: GridStyle | None = InsetGrid,
         show_borders: DiBool | None = None,
         selected: bool = False,
         key_bindings: KeyBindingsBase | None = None,
         mouse_handler: Callable[[MouseEvent], NotImplementedOrNone] | None = None,
     ) -> None:
         """Create a new button widget instance.
 
@@ -255,15 +255,19 @@
                         ypos=y_min,
                         width=x_max - x_min,
                         height=y_max - y_min,
                     )
                 self.on_mouse_down.fire()
 
                 if not self.has_focus():
-                    get_app().layout.focus(self)
+                    app = get_app()
+                    app.layout.focus(self)
+                    # Invalidate the app - we don't do it by returning None so the
+                    # event can bubble
+                    app.invalidate()
                     # We want this event to bubble if unfocused
                     return NotImplemented
                 else:
                     return None
 
             elif mouse_event.event_type == MouseEventType.MOUSE_UP:
                 get_app().mouse_limits = None
@@ -301,15 +305,15 @@
 
     def __pt_container__(self) -> AnyContainer:
         """Return the button's container."""
         return self.container
 
 
 class ToggleableWidget(metaclass=ABCMeta):
-    """Bae class for toggleable widgets."""
+    """Base class for toggleable widgets."""
 
     container: AnyContainer
     on_click: Event
     selected: bool
     disabled: Filter
     key_bindings: KeyBindingsBase | None
 
@@ -321,15 +325,17 @@
     def mouse_handler(self, mouse_event: MouseEvent) -> NotImplementedOrNone:
         """Focus on mouse down and toggle state on mouse up."""
         if self.disabled():
             return NotImplemented
         elif mouse_event.event_type == MouseEventType.MOUSE_DOWN:
             layout = get_app().layout
             if not layout.has_focus(self):
-                get_app().layout.focus(self)
+                app = get_app()
+                app.layout.focus(self)
+                app.invalidate()
                 return NotImplemented
             else:
                 return None
         elif mouse_event.event_type == MouseEventType.MOUSE_UP:
             self.toggle()
             return None
         else:
@@ -359,15 +365,15 @@
 
     def __init__(
         self,
         text: AnyFormattedText,
         on_click: Callable[[ToggleButton], None] | None = None,
         width: int | None = None,
         style: str | Callable[[], str] = "class:input",
-        border: GridStyle | None = InnerEigthGrid,
+        border: GridStyle | None = InsetGrid,
         show_borders: DiBool | None = None,
         selected: bool = False,
         disabled: FilterOrBool = False,
         key_bindings: KeyBindingsBase | None = None,
     ) -> None:
         """Create a new toggle-button instance.
 
@@ -529,15 +535,15 @@
 
     def __init__(
         self,
         text: str = "",
         style: str = "class:input",
         height: int = 1,
         min_height: int = 1,
-        multiline: bool = False,
+        multiline: FilterOrBool = False,
         expand: FilterOrBool = True,
         width: int | None = None,
         completer: Completer | None = None,
         options: list[str] | Callable[[], list[str]] | None = None,
         show_borders: DiBool | None = None,
         on_text_changed: Callable[[Buffer], None] | None = None,
         validation: Callable[[str], bool] | None = None,
@@ -633,26 +639,31 @@
             menu_position=self.text_area.control.menu_position,
             focus_on_click=self.text_area.control.focus_on_click,
             key_bindings=self.text_area.control.key_bindings,
             expand=expand,
         )
         self.text_area.window.content = self.text_area.control
 
-        if multiline:
-            self.text_area.window.right_margins = [
-                *self.text_area.window.right_margins,
-                ScrollbarMargin(),
-            ]
         if on_text_changed:
             self.text_area.buffer.on_text_changed += on_text_changed
         if validation:
             self.text_area.buffer.validate_while_typing = Always()
         self.container = Border(
-            self.text_area,
-            border=InnerEigthGrid,
+            VSplit(
+                [
+                    self.text_area,
+                    ConditionalContainer(
+                        MarginContainer(
+                            ScrollbarMargin(), target=self.text_area.window
+                        ),
+                        filter=to_filter(multiline),
+                    ),
+                ]
+            ),
+            border=InsetGrid,
             style=self.border_style,
             show_borders=show_borders,
         )
 
     def border_style(self) -> str:
         """Calculate the style to apply to the widget's border."""
         if self.text_area.buffer.validation_state == ValidationState.INVALID:
@@ -901,15 +912,15 @@
                     self.control,
                     style=self.add_style("class:progress"),
                     dont_extend_width=self.vertical,
                     # dont_extend_height=~self.vertical,
                     height=lambda: None if self.vertical() else 1,
                     width=lambda: 1 if self.vertical() else None,
                 ),
-                border=InnerEigthGrid,
+                border=InsetGrid,
                 style=self.add_style("class:progress,border"),
             ),
             # width=lambda: 1 if self.vertical() else None,
         )
 
     @property
     def value(self) -> float | int:
@@ -933,16 +944,16 @@
         return _style
 
     def __pt_container__(self) -> AnyContainer:
         """Return the progress-bar's container."""
         return self.container
 
 
-class SizedMask(dict[int, bool]):
-    """Mak with restricted number of True items."""
+class SizedMask(Dict[int, bool]):
+    """Mask with restricted number of True items."""
 
     def __init__(self, size: int | None = None) -> None:
         """Initialize a new sized default dict."""
         self.size = size
         self._keys: deque[int] = deque()
 
     def clear(self) -> None:
@@ -970,15 +981,15 @@
 
     def __missing__(self, key: int) -> bool:
         """Return ``False`` for unknown items."""
         return False
 
 
 class SelectableWidget(metaclass=ABCMeta):
-    """Bae class for widgets where one or more items can be selected."""
+    """Base class for widgets where one or more items can be selected."""
 
     def __init__(
         self,
         options: list[Any],
         labels: Sequence[AnyFormattedText] | None = None,
         index: int | None = None,
         indices: list[int] | None = None,
@@ -1129,24 +1140,42 @@
     @indices.setter
     def indices(self, values: tuple[int]) -> None:
         """Set the selected indices."""
         self._selected.clear()
         for i in range(len(self.options)):
             self._selected[i] = i in values
 
+    @property
+    def value(self) -> Any:
+        """Return the selected value."""
+        if self.options:
+            return self.options[self.index or 0]
+        else:
+            return None
+
+    @property
+    def values(self) -> list[Any]:
+        """Return a list of the selected values."""
+        if self.options:
+            return [self.options[i] for i in self.indices]
+        else:
+            return [None for i in self.indices]
+
     def mouse_handler(self, i: int, mouse_event: MouseEvent) -> NotImplementedOrNone:
         """Handle mouse events."""
         if self.disabled():
             return NotImplemented
         if mouse_event.event_type == MouseEventType.MOUSE_MOVE:
             self.hovered = i
             return None
         elif mouse_event.event_type == MouseEventType.MOUSE_DOWN:
             if not self.has_focus():
+                app = get_app()
                 get_app().layout.focus(self)
+                app.invalidate()
                 # We want this event to bubble if unfocused
                 return NotImplemented
             else:
                 return None
         elif mouse_event.event_type == MouseEventType.MOUSE_UP:
             self.toggle_item(i)
             return None
@@ -1197,15 +1226,15 @@
         n_values: int | None = None,
         multiple: FilterOrBool = False,
         max_count: int | None = None,
         on_change: Callable[[SelectableWidget], None] | None = None,
         style: str | Callable[[], str] = "class:input,select",
         rows: int | None = 3,
         prefix: tuple[str, str] = ("", ""),
-        border: GridStyle | None = InnerEigthGrid,
+        border: GridStyle | None = InsetGrid,
         show_borders: DiBool | None = None,
         disabled: FilterOrBool = False,
         dont_extend_width: FilterOrBool = True,
         dont_extend_height: FilterOrBool = True,
     ) -> None:
         """Create a new select widget instance.
 
@@ -1248,15 +1277,20 @@
             style=style,
             disabled=disabled,
         )
 
     def text_fragments(self) -> StyleAndTextTuples:
         """Create a list of formatted text fragments to display."""
         ft: StyleAndTextTuples = []
-        max_width = max(fragment_list_width(to_formatted_text(x)) for x in self.labels)
+        if self.labels:
+            max_width = max(
+                fragment_list_width(to_formatted_text(x)) for x in self.labels
+            )
+        else:
+            max_width = 1
         for i, label in enumerate(self.labels):
             label = to_formatted_text(label)
             label = align(label, FormattedTextAlign.LEFT, width=max_width)
             if self.multiple():
                 cursor = "[SetCursorPosition]" if i == self.hovered else ""
             else:
                 cursor = "[SetCursorPosition]" if self.mask[i] else ""
@@ -1273,34 +1307,39 @@
             handler = cast(
                 "Callable[[MouseEvent], None]", partial(self.mouse_handler, i)
             )
             ft += [
                 (f"{fragment_style} {style}", text, handler)
                 for fragment_style, text, *_ in ft_option
             ]
-        ft.pop()
+        if ft:
+            ft.pop()
         return ft
 
     def load_container(self) -> AnyContainer:
         """Load the widget's container."""
         return Box(
             Border(
-                Window(
-                    FormattedTextControl(
-                        self.text_fragments,
-                        focusable=True,
-                        show_cursor=False,
-                        key_bindings=self.key_bindings(),
-                    ),
-                    height=lambda: self.rows,
-                    dont_extend_width=self.dont_extend_width,
-                    dont_extend_height=self.dont_extend_height,
-                    style=f"class:face"
-                    f"{' class:disabled' if self.disabled() else ''}",
-                    right_margins=[ScrollbarMargin(style=self.style)],
+                VSplit(
+                    [
+                        window := Window(
+                            FormattedTextControl(
+                                self.text_fragments,
+                                focusable=True,
+                                show_cursor=False,
+                                key_bindings=self.key_bindings(),
+                            ),
+                            height=lambda: self.rows,
+                            dont_extend_width=self.dont_extend_width,
+                            dont_extend_height=self.dont_extend_height,
+                            style=f"class:face"
+                            f"{' class:disabled' if self.disabled() else ''}",
+                        ),
+                        MarginContainer(ScrollbarMargin(), target=window),
+                    ]
                 ),
                 border=self.border,
                 show_borders=self.show_borders,
                 style="class:inset,border",
             ),
             padding=0,
             style=self.style,
@@ -1506,15 +1545,15 @@
         index: int | None = None,
         indices: list[int] | None = None,
         n_values: int | None = None,
         multiple: FilterOrBool = False,
         max_count: int | None = None,
         on_change: Callable[[SelectableWidget], None] | None = None,
         style: str | Callable[[], str] = "class:input",
-        border: GridStyle | None = InnerEigthGrid,
+        border: GridStyle | None = InsetGrid,
         disabled: FilterOrBool = False,
         vertical: FilterOrBool = False,
     ) -> None:
         """Create a new select widget instance.
 
         Args:
             options: List of permitted values
@@ -2051,15 +2090,15 @@
         index: int | None = None,
         indices: list[int] | None = None,
         n_values: int | None = None,
         multiple: FilterOrBool = False,
         max_count: int | None = None,
         on_change: Callable[[SelectableWidget], None] | None = None,
         style: str | Callable[[], str] = "class:input",
-        border: GridStyle = InnerEigthGrid,
+        border: GridStyle = InsetGrid,
         show_borders: DiBool | None = None,
         vertical: FilterOrBool = False,
         show_arrows: FilterOrBool = True,
         arrows: tuple[AnyFormattedText, AnyFormattedText] = ("-", "+"),
         show_readout: FilterOrBool = True,
         disabled: FilterOrBool = False,
     ) -> None:
```

### Comparing `euporie-2.3.2/euporie/core/widgets/inputs.py` & `euporie-2.4.0/euporie/core/widgets/inputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,14 @@
         left_margins: Sequence[Margin] | None = None,
         right_margins: Sequence[Margin] | None = None,
         on_text_changed: Callable[[Buffer], None] | None = None,
         on_cursor_position_changed: Callable[[Buffer], None] | None = None,
         tempfile_suffix: str | Callable[[], str] = "",
         key_bindings: KeyBindingsBase | None = None,
         enable_history_search: FilterOrBool | None = False,
-        focusable: FilterOrBool = True,
         wrap_lines: FilterOrBool = False,
         complete_while_typing: FilterOrBool = True,
         autosuggest_while_typing: FilterOrBool = True,
         validate_while_typing: FilterOrBool | None = None,
         **kwargs: Any,
     ) -> None:
         """Initiate the cell input box."""
@@ -91,14 +90,15 @@
         app = kernel_tab.app
 
         kwargs.setdefault("wrap_lines", wrap_lines)
         kwargs.setdefault("style", "class:kernel-input")
         kwargs.setdefault("history", kernel_tab.history)
         kwargs.setdefault("search_field", app.search_bar)
         kwargs.setdefault("focus_on_click", True)
+        kwargs.setdefault("preview_search", True)
         kwargs.setdefault(
             "input_processors",
             [
                 ConditionalProcessor(
                     HighlightIncrementalSearchProcessor(),
                     filter=is_searching,
                 ),
@@ -164,26 +164,36 @@
         # Set style
         style = kwargs.get("style", "")
         self.window.style = lambda: (
             "class:text-area " + ("class:focused " if self.has_focus() else "") + style
         )
 
         # Add configurable line numbers
-        self.window.left_margins = left_margins or [
-            ConditionalMargin(
-                NumberedDiffMargin(),
-                Condition(lambda: self.kernel_tab.app.config.line_numbers),
-            )
-        ]
-        self.window.right_margins = right_margins or [
-            OverflowMargin(),
-            ConditionalMargin(
-                ScrollbarMargin(display_arrows=False), filter=scrollable(self.window)
-            ),
-        ]
+        self.window.left_margins = (
+            left_margins
+            if left_margins is not None
+            else [
+                ConditionalMargin(
+                    NumberedDiffMargin(),
+                    Condition(lambda: self.kernel_tab.app.config.line_numbers),
+                )
+            ]
+        )
+
+        self.window.right_margins = (
+            right_margins
+            if right_margins is not None
+            else [
+                OverflowMargin(),
+                ConditionalMargin(
+                    ScrollbarMargin(display_arrows=False),
+                    filter=scrollable(self.window),
+                ),
+            ]
+        )
 
         self.window.cursorline = self.has_focus
 
         # Set extra key-bindings
         widgets_key_bindings = load_registered_bindings(
             "euporie.core.widgets.inputs.KernelInput"
         )
```

### Comparing `euporie-2.3.2/euporie/core/widgets/layout.py` & `euporie-2.4.0/euporie/core/widgets/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     UIContent,
     UIControl,
 )
 from prompt_toolkit.mouse_events import MouseButton, MouseEventType
 from prompt_toolkit.utils import Event
 from prompt_toolkit.widgets import Box
 
-from euporie.core.border import OuterEigthGrid
+from euporie.core.border import OutsetGrid
 from euporie.core.data_structures import DiBool
 from euporie.core.widgets.decor import Border
 
 if TYPE_CHECKING:
     from typing import Any, Callable, Sequence
 
     from prompt_toolkit.filters import FilterOrBool
@@ -336,15 +336,15 @@
                 if callable(activate := tabs[index].on_activate):
                     activate()
                 return None
         return NotImplemented
 
 
 class StackedSplit(metaclass=ABCMeta):
-    """Bae class for containers with selectable children."""
+    """Base class for containers with selectable children."""
 
     def __init__(
         self,
         children: Sequence[AnyContainer],
         titles: Sequence[AnyFormattedText],
         active: int = 0,
         style: str | Callable[[], str] = "class:tab-split",
@@ -450,15 +450,15 @@
         children: Sequence[AnyContainer],
         titles: Sequence[AnyFormattedText],
         active: int = 0,
         style: str | Callable[[], str] = "class:tab-split",
         on_change: Callable[[StackedSplit], None] | None = None,
         width: AnyDimension = None,
         height: AnyDimension = None,
-        border: GridStyle = OuterEigthGrid,
+        border: GridStyle = OutsetGrid,
         show_borders: DiBool | None = None,
     ) -> None:
         """Initialize a new tabbed container."""
         self.border = border
         self.show_borders = show_borders or DiBool(False, True, True, True)
         super().__init__(
             children=children,
@@ -489,14 +489,15 @@
                 ),
                 Border(
                     Box(
                         DynamicContainer(self.active_child),
                         padding=0,
                         padding_top=1,
                         padding_bottom=1,
+                        style="class:tabbed-split,page",
                     ),
                     border=self.border,
                     show_borders=self.show_borders,
                 ),
             ],
             style="class:tabbed-split",
             width=self.width,
```

### Comparing `euporie-2.3.2/euporie/core/widgets/menu.py` & `euporie-2.4.0/euporie/core/widgets/menu.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,29 +2,37 @@
 
 from __future__ import annotations
 
 import logging
 from functools import partial
 from typing import TYPE_CHECKING
 
-from prompt_toolkit.filters import Condition, to_filter
+from prompt_toolkit.data_structures import Point
+from prompt_toolkit.filters import Condition, has_completions, is_done, to_filter
 from prompt_toolkit.formatted_text.base import to_formatted_text
 from prompt_toolkit.formatted_text.utils import (
     fragment_list_to_text,
     fragment_list_width,
     to_plain_text,
 )
 from prompt_toolkit.key_binding.key_bindings import KeyBindings
 from prompt_toolkit.layout.containers import (
     ConditionalContainer,
     Container,
     Float,
+    HSplit,
+    ScrollOffsets,
+    VSplit,
     Window,
 )
-from prompt_toolkit.layout.controls import FormattedTextControl
+from prompt_toolkit.layout.controls import FormattedTextControl, UIContent
+from prompt_toolkit.layout.dimension import Dimension
+from prompt_toolkit.layout.menus import (
+    CompletionsMenuControl as PtkCompletionsMenuControl,
+)
 from prompt_toolkit.layout.utils import explode_text_fragments
 from prompt_toolkit.mouse_events import MouseEvent, MouseEventType
 from prompt_toolkit.utils import get_cwidth
 
 from euporie.core.border import OuterHalfGrid
 from euporie.core.current import get_app
 from euporie.core.widgets.decor import Shadow
@@ -34,19 +42,21 @@
 
     from prompt_toolkit.filters import Filter, FilterOrBool
     from prompt_toolkit.formatted_text.base import (
         AnyFormattedText,
         OneStyleAndTextTuple,
         StyleAndTextTuples,
     )
+    from prompt_toolkit.key_binding.key_bindings import NotImplementedOrNone
     from prompt_toolkit.key_binding.key_processor import KeyPressEvent
 
     from euporie.core.app import BaseApp
     from euporie.core.border import GridStyle
     from euporie.core.commands import Command
+    from euporie.core.widgets.status_bar import StatusBarFields
 
 
 log = logging.getLogger(__name__)
 
 
 class MenuItem:
     """A prompt-toolkit compatible menu item with more advanced capabilities.
@@ -250,211 +260,14 @@
             widths.append(width)
         return max(widths)
 
 
 class MenuBar:
     """A container to hold the menubar and main application body."""
 
-    def _get_menu(self, level: int) -> MenuItem:
-        menu = self.menu_items[self.selected_menu[0]]
-
-        for i, index in enumerate(self.selected_menu[1:]):
-            if i < level:
-                try:
-                    menu = menu.children[index]
-                except IndexError:
-                    return MenuItem("debug")
-
-        return menu
-
-    def _get_menu_fragments(self) -> StyleAndTextTuples:
-        focused = get_app().layout.has_focus(self.window)
-
-        # This is called during the rendering. When we discover that this
-        # widget doesn't have the focus anymore. Reset menu state.
-        if not focused:
-            self.selected_menu = [0]
-
-        def mouse_handler(index: int, mouse_event: MouseEvent) -> None:
-            hover = mouse_event.event_type == MouseEventType.MOUSE_MOVE
-            if mouse_event.event_type == MouseEventType.MOUSE_DOWN or hover and focused:
-                # Toggle focus.
-                app = get_app()
-                if not hover:
-                    if app.layout.has_focus(self.window):
-                        if self.selected_menu == [index]:
-                            app.layout.focus_last()
-                    else:
-                        app.layout.focus(self.window)
-                self.selected_menu = [index]
-
-        results: StyleAndTextTuples = []
-        used_keys = set()
-
-        for i, item in enumerate(self.menu_items):
-            # Add shortcut key hints
-            key = to_plain_text(item.formatted_text)[0].lower()
-            ft: StyleAndTextTuples
-            if key not in used_keys:
-                ft = explode_text_fragments(item.formatted_text)
-                ft = [(f"underline {ft[0][0]}", ft[0][1]), *ft[1:]]
-                used_keys |= {key}
-            else:
-                ft = item.formatted_text
-
-            mh = partial(mouse_handler, i)
-            selected = i == self.selected_menu[0] and focused
-            style = "class:selection" if selected else ""
-            first_style = f"{style} [SetMenuPosition]" if selected else style
-
-            results.extend(
-                [
-                    (first_style, " ", mh),
-                    *[(f"{style} {style_}", text, mh) for style_, text, *_ in ft],
-                    (style, " ", mh),
-                ]
-            )
-
-        return results
-
-    def _submenu(self, level: int = 0) -> Window:
-        def get_text_fragments() -> StyleAndTextTuples:
-            result: StyleAndTextTuples = []
-            if level < len(self.selected_menu):
-                menu = self._get_menu(level)
-
-                if menu.children:
-                    result.extend(
-                        [
-                            ("class:menu,border", self.grid.TOP_LEFT),
-                            ("class:menu,border", self.grid.TOP_MID * menu.width),
-                            ("class:menu,border", self.grid.TOP_RIGHT),
-                            ("", "\n"),
-                        ]
-                    )
-
-                    try:
-                        selected_item = self.selected_menu[level + 1]
-                    except IndexError:
-                        selected_item = -1
-
-                    def one_item(
-                        i: int, item: MenuItem
-                    ) -> Iterable[OneStyleAndTextTuple]:
-                        assert isinstance(item, MenuItem)
-                        assert isinstance(menu, MenuItem)
-
-                        def mouse_handler(mouse_event: MouseEvent) -> None:
-                            if item.disabled:
-                                # The arrow keys can't interact with menu items that
-                                # are disabled. The mouse shouldn't be able to either.
-                                return
-                            hover = mouse_event.event_type == MouseEventType.MOUSE_MOVE
-                            if (
-                                mouse_event.event_type == MouseEventType.MOUSE_UP
-                                or hover
-                            ):
-                                app = get_app()
-                                if not hover and item.handler:
-                                    app.layout.focus_last()
-                                    item.handler()
-                                else:
-                                    self.selected_menu = self.selected_menu[
-                                        : level + 1
-                                    ] + [i]
-
-                        if item.separator:
-                            # Show a connected line with no mouse handler
-                            yield (
-                                "class:menu,border",
-                                self.grid.SPLIT_LEFT
-                                + (self.grid.SPLIT_MID * menu.width)
-                                + self.grid.SPLIT_RIGHT,
-                            )
-
-                        else:
-                            # Show the right edge
-                            style = ""
-                            # Set the style if disabled
-                            if item.disabled:
-                                style += "class:menu,disabled"
-                            # Set the style and cursor if selected
-                            if i == selected_item:
-                                style += "class:menu,selection"
-                            yield (f"{style} class:menu,border", self.grid.MID_LEFT)
-                            if i == selected_item:
-                                yield ("[SetCursorPosition]", "")
-                            # Construct the menu item contents
-                            prefix_padding = " " * (
-                                0
-                                if menu.collapse_prefix
-                                else menu.prefix_width
-                                - fragment_list_width(item.prefix)
-                            )
-                            suffix_padding = " " * (
-                                menu.width
-                                - fragment_list_width(item.prefix)
-                                - len(prefix_padding)
-                                - fragment_list_width(item.formatted_text)
-                                - (
-                                    fragment_list_width(item.suffix)
-                                    if menu.collapse_suffix
-                                    else menu.suffix_width
-                                )
-                            )
-                            text_padding = " " * (
-                                menu.width
-                                - fragment_list_width(item.prefix)
-                                - len(prefix_padding)
-                                - fragment_list_width(item.formatted_text)
-                                - fragment_list_width(item.suffix)
-                                - len(suffix_padding)
-                            )
-                            menu_formatted_text: StyleAndTextTuples = to_formatted_text(
-                                [
-                                    *item.prefix,
-                                    ("", prefix_padding),
-                                    *item.formatted_text,
-                                    ("", text_padding),
-                                    ("", suffix_padding),
-                                    *item.suffix,
-                                ],
-                                style=style,
-                            )
-                            # Apply mouse handler to all fragments
-                            menu_formatted_text = [
-                                (fragment[0], fragment[1], mouse_handler)
-                                for fragment in menu_formatted_text
-                            ]
-                            # Show the menu item contents
-                            yield from menu_formatted_text
-                            # Position the sub-menu
-                            if i == selected_item:
-                                yield ("[SetMenuPosition]", "")
-                            # Show the right edge
-                            yield (f"{style} class:menu,border", self.grid.MID_RIGHT)
-
-                        yield ("", "\n")
-
-                    for i, item in enumerate(menu.children):
-                        if not item.hidden():
-                            result.extend(one_item(i, item))
-
-                    result.extend(
-                        [
-                            ("class:menu,border", self.grid.BOTTOM_LEFT),
-                            ("class:menu,border", self.grid.BOTTOM_MID * menu.width),
-                            ("class:menu,border", self.grid.BOTTOM_RIGHT),
-                        ]
-                    )
-
-            return result
-
-        return Window(FormattedTextControl(get_text_fragments), style="class:menu")
-
     def __init__(
         self,
         app: BaseApp,
         menu_items: Sequence[MenuItem],
         grid: GridStyle = OuterHalfGrid,
     ) -> None:
         """Initiate the menu bar.
@@ -491,15 +304,18 @@
         def _right(event: KeyPressEvent) -> None:
             self.selected_menu[0] = min(
                 len(self.menu_items) - 1, self.selected_menu[0] + 1
             )
 
         @kb.add("down", filter=in_main_menu)
         def _down(event: KeyPressEvent) -> None:
-            self.selected_menu.append(0)
+            menu = self._get_menu(len(self.selected_menu) - 2)
+            indices = [i for i, item in enumerate(menu.children) if not item.disabled]
+            if indices:
+                self.selected_menu.append(indices[0])
 
         @kb.add("c-c", filter=in_main_menu)
         @kb.add("c-g", filter=in_main_menu)
         def _cancel(event: KeyPressEvent) -> None:
             """Leave menu."""
             event.app.layout.focus_last()
 
@@ -536,15 +352,15 @@
             # Look for previous enabled items in this sub menu.
             menu = self._get_menu(len(self.selected_menu) - 2)
             index = self.selected_menu[-1]
 
             previous_indexes = [
                 i
                 for i, item in enumerate(menu.children)
-                if i < index and not item.disabled
+                if i < index and not item.disabled and not item.hidden()
             ]
 
             if previous_indexes:
                 self.selected_menu[-1] = previous_indexes[-1]
             elif len(self.selected_menu) == 2:
                 # Return to main menu.
                 self.selected_menu.pop()
@@ -554,15 +370,15 @@
             """Select next (enabled) menu item."""
             menu = self._get_menu(len(self.selected_menu) - 2)
             index = self.selected_menu[-1]
 
             next_indexes = [
                 i
                 for i, item in enumerate(menu.children)
-                if i > index and not item.disabled
+                if i > index and not item.disabled and not item.hidden()
             ]
 
             if next_indexes:
                 self.selected_menu[-1] = next_indexes[0]
 
         @kb.add("enter")
         def _click(event: KeyPressEvent) -> None:
@@ -603,17 +419,15 @@
         self.control = FormattedTextControl(
             self._get_menu_fragments,
             key_bindings=kb,
             focusable=True,
             show_cursor=False,
         )
         self.window: Window = Window(
-            height=1,
-            content=self.control,
-            style="class:menu,bar",
+            height=1, content=self.control, style="class:menu,bar"
         )
 
         submenu = self._submenu(0)
         submenu2 = self._submenu(1)
         submenu3 = self._submenu(2)
 
         @Condition
@@ -624,42 +438,380 @@
             xcursor=True,
             ycursor=True,
             content=ConditionalContainer(
                 content=Shadow(body=submenu), filter=has_focus
             ),
         )
         self.app.menus["menu-2"] = Float(
-            attach_to_window=submenu,
+            attach_to_window=submenu.get_children()[1],
             xcursor=True,
             ycursor=True,
             allow_cover_cursor=True,
             content=ConditionalContainer(
                 content=Shadow(body=submenu2),
-                filter=has_focus & Condition(lambda: len(self.selected_menu) >= 1),
+                filter=has_focus
+                & Condition(lambda: len(self.selected_menu) > 1)
+                & Condition(lambda: bool(self._get_menu(1).children)),
             ),
         )
         self.app.menus["menu-3"] = Float(
-            attach_to_window=submenu2,
+            attach_to_window=submenu2.get_children()[1],
             xcursor=True,
             ycursor=True,
             allow_cover_cursor=True,
             content=ConditionalContainer(
                 content=Shadow(body=submenu3),
-                filter=has_focus & Condition(lambda: len(self.selected_menu) >= 2),
+                filter=has_focus
+                & Condition(lambda: len(self.selected_menu) > 2)
+                & Condition(lambda: bool(self._get_menu(2).children)),
             ),
         )
 
-        get_app().container_statuses[self.window] = self.statusbar_fields
+    def _get_menu(self, level: int) -> MenuItem:
+        menu = self.menu_items[self.selected_menu[0]]
+        for i, index in enumerate(self.selected_menu[1:]):
+            if i < level:
+                try:
+                    menu = menu.children[index]
+                except IndexError:
+                    return MenuItem("debug")
+        return menu
+
+    def _get_menu_fragments(self) -> StyleAndTextTuples:
+        focused = get_app().layout.has_focus(self.window)
 
-    def statusbar_fields(
-        self,
-    ) -> tuple[list[AnyFormattedText], list[AnyFormattedText]]:
+        # This is called during the rendering. When we discover that this
+        # widget doesn't have the focus anymore. Reset menu state.
+        if not focused:
+            self.selected_menu = [0]
+
+        def mouse_handler(index: int, mouse_event: MouseEvent) -> NotImplementedOrNone:
+            hover = mouse_event.event_type == MouseEventType.MOUSE_MOVE
+            if mouse_event.event_type == MouseEventType.MOUSE_DOWN or hover and focused:
+                # Toggle focus.
+                app = get_app()
+                if not hover:
+                    if app.layout.has_focus(self.window):
+                        if self.selected_menu == [index]:
+                            app.layout.focus_last()
+                    else:
+                        app.layout.focus(self.window)
+                self.selected_menu = [index]
+                return None
+            return NotImplemented
+
+        results: StyleAndTextTuples = []
+        used_keys = set()
+
+        for i, item in enumerate(self.menu_items):
+            # Add shortcut key hints
+            key = to_plain_text(item.formatted_text)[0].lower()
+            ft: StyleAndTextTuples
+            if key not in used_keys:
+                ft = explode_text_fragments(item.formatted_text)
+                ft = [(f"underline {ft[0][0]}", ft[0][1]), *ft[1:]]
+                used_keys |= {key}
+            else:
+                ft = item.formatted_text
+
+            mh = partial(mouse_handler, i)
+            selected = i == self.selected_menu[0] and focused
+            style = "class:selection" if selected else ""
+            first_style = f"{style} [SetMenuPosition]" if selected else style
+
+            results.extend(
+                [
+                    (first_style, " ", mh),
+                    *[(f"{style} {style_}", text, mh) for style_, text, *_ in ft],
+                    (style, " ", mh),
+                ]
+            )
+
+        return results
+
+    def _submenu(self, level: int = 0) -> Container:
+        grid = self.grid
+
+        def get_text_fragments() -> StyleAndTextTuples:
+            result: StyleAndTextTuples = []
+            if level < len(self.selected_menu):
+                menu = self._get_menu(level)
+
+                if menu.children:
+                    try:
+                        selected_item = self.selected_menu[level + 1]
+                    except IndexError:
+                        selected_item = -1
+
+                    def one_item(
+                        i: int, item: MenuItem
+                    ) -> Iterable[OneStyleAndTextTuple]:
+                        assert isinstance(item, MenuItem)
+                        assert isinstance(menu, MenuItem)
+
+                        def mouse_handler(mouse_event: MouseEvent) -> None:
+                            if item.disabled:
+                                # The arrow keys can't interact with menu items that
+                                # are disabled. The mouse shouldn't be able to either.
+                                return
+                            hover = mouse_event.event_type == MouseEventType.MOUSE_MOVE
+                            if (
+                                mouse_event.event_type == MouseEventType.MOUSE_UP
+                                or hover
+                            ):
+                                app = get_app()
+                                if not hover and item.handler:
+                                    app.layout.focus_last()
+                                    item.handler()
+                                else:
+                                    self.selected_menu = self.selected_menu[
+                                        : level + 1
+                                    ] + [i]
+
+                        if item.separator:
+                            # Show a connected line with no mouse handler
+                            yield (
+                                "class:menu,border",
+                                grid.SPLIT_LEFT
+                                + (grid.SPLIT_MID * menu.width)
+                                + grid.SPLIT_RIGHT,
+                            )
+
+                        else:
+                            # Show the right edge
+                            style = ""
+                            # Set the style if disabled
+                            if item.disabled:
+                                style += "class:menu,disabled"
+                            # Set the style and cursor if selected
+                            if i == selected_item:
+                                style += "class:menu,selection"
+                            yield (f"{style} class:menu,border", grid.MID_LEFT)
+                            if i == selected_item:
+                                yield ("[SetCursorPosition]", "")
+                            # Construct the menu item contents
+                            prefix_padding = " " * (
+                                0
+                                if menu.collapse_prefix
+                                else menu.prefix_width
+                                - fragment_list_width(item.prefix)
+                            )
+                            suffix_padding = " " * (
+                                menu.width
+                                - fragment_list_width(item.prefix)
+                                - len(prefix_padding)
+                                - fragment_list_width(item.formatted_text)
+                                - (
+                                    fragment_list_width(item.suffix)
+                                    if menu.collapse_suffix
+                                    else menu.suffix_width
+                                )
+                            )
+                            text_padding = " " * (
+                                menu.width
+                                - fragment_list_width(item.prefix)
+                                - len(prefix_padding)
+                                - fragment_list_width(item.formatted_text)
+                                - fragment_list_width(item.suffix)
+                                - len(suffix_padding)
+                            )
+                            menu_formatted_text: StyleAndTextTuples = to_formatted_text(
+                                [
+                                    *item.prefix,
+                                    ("", prefix_padding),
+                                    *item.formatted_text,
+                                    ("", text_padding),
+                                    ("", suffix_padding),
+                                    *item.suffix,
+                                ],
+                                style=style,
+                            )
+                            # Apply mouse handler to all fragments
+                            menu_formatted_text = [
+                                (fragment[0], fragment[1], mouse_handler)
+                                for fragment in menu_formatted_text
+                            ]
+                            # Show the menu item contents
+                            yield from menu_formatted_text
+                            # Position the sub-menu
+                            if i == selected_item:
+                                yield ("[SetMenuPosition]", "")
+                            # Show the right edge
+                            yield (f"{style} class:menu,border", grid.MID_RIGHT)
+
+                    for i, item in enumerate(menu.children):
+                        if not item.hidden():
+                            result.extend(one_item(i, item))
+                            if i < len(menu.children) - 1:
+                                result.append(("", "\n"))
+
+            return result
+
+        return HSplit(
+            [
+                VSplit(
+                    [
+                        Window(char=grid.TOP_LEFT, width=1, height=1),
+                        Window(char=grid.TOP_MID, height=1),
+                        Window(char=grid.TOP_RIGHT, width=1, height=1),
+                    ],
+                    style="class:border",
+                ),
+                Window(
+                    FormattedTextControl(get_text_fragments),
+                    scroll_offsets=ScrollOffsets(top=1, bottom=1),
+                ),
+                VSplit(
+                    [
+                        Window(char=grid.BOTTOM_LEFT, width=1, height=1),
+                        Window(char=grid.BOTTOM_MID, height=1),
+                        # Window(char="🭑🭆", height=1),
+                        Window(char=grid.BOTTOM_RIGHT, width=1, height=1),
+                    ],
+                    style="class:border",
+                ),
+            ],
+            style="class:menu",
+        )
+
+    def __pt_container__(self) -> Container:
+        """Return the menu bar container's content."""
+        return self.window
+
+    def __pt_status__(self) -> StatusBarFields:
         """Return the description of the currently selected menu item."""
         selected_item = self._get_menu(len(self.selected_menu) - 1)
         if isinstance(selected_item, MenuItem):
             return (["", selected_item.description], [])
         else:
             return (["", ""], [])
 
-    def __pt_container__(self) -> Container:
-        """Return the menu bar container's content."""
-        return self.window
+
+class CompletionsMenuControl(PtkCompletionsMenuControl):
+    """A custom completions menu control."""
+
+    def create_content(self, width: int, height: int) -> UIContent:
+        """Create a UIContent object for this control."""
+        complete_state = get_app().current_buffer.complete_state
+        if complete_state:
+            completions = complete_state.completions
+            index = complete_state.complete_index  # Can be None!
+
+            # Calculate width of completions menu.
+            menu_width = self._get_menu_width(width, complete_state)
+            menu_meta_width = self._get_menu_meta_width(
+                width - menu_width, complete_state
+            )
+            total_width = menu_width + menu_meta_width
+
+            grid = OuterHalfGrid
+
+            def get_line(i: int) -> StyleAndTextTuples:
+                c = completions[i]
+                selected_item = i == index
+                output: StyleAndTextTuples = []
+
+                style = "class:menu"
+                if selected_item:
+                    style += ",selection"
+
+                output.append((f"{style},border", grid.MID_LEFT))
+                if selected_item:
+                    output.append(("[SetCursorPosition]", ""))
+                # Construct the menu item contents
+                padding = " " * (
+                    total_width
+                    - fragment_list_width(c.display)
+                    - fragment_list_width(c.display_meta)
+                    - 2
+                )
+                output.extend(
+                    to_formatted_text(
+                        [
+                            *c.display,
+                            ("", padding),
+                            *to_formatted_text(
+                                c.display_meta, style=f"{style} {c.style}"
+                            ),
+                        ],
+                        style=style,
+                    )
+                )
+                output.append((f"{style},border", grid.MID_RIGHT))
+
+                # Apply mouse handler
+                output = [
+                    (fragment[0], fragment[1], self.mouse_handler)
+                    for fragment in output
+                ]
+
+                return output
+
+            return UIContent(
+                get_line=get_line,
+                cursor_position=Point(x=0, y=index or 0),
+                line_count=len(completions),
+            )
+
+        return UIContent()
+
+    def mouse_handler(self, mouse_event: MouseEvent) -> NotImplementedOrNone:
+        """Handle mouse events: clicking and scrolling."""
+        if mouse_event.event_type == MouseEventType.MOUSE_MOVE:
+            # Set completion
+            complete_state = get_app().current_buffer.complete_state
+            if complete_state:
+                complete_state.complete_index = mouse_event.position.y
+                return None
+
+        return super().mouse_handler(mouse_event)
+
+
+class CompletionsMenu(ConditionalContainer):
+    """A custom completions menu."""
+
+    def __init__(
+        self,
+        max_height: int | None = 16,
+        scroll_offset: int | Callable[[], int] = 1,
+        extra_filter: FilterOrBool = True,
+        z_index: int = 10**8,
+    ) -> None:
+        """Create a completions menu with borders."""
+        extra_filter = to_filter(extra_filter)
+        grid = OuterHalfGrid
+        super().__init__(
+            content=HSplit(
+                [
+                    VSplit(
+                        [
+                            Window(char=grid.TOP_LEFT, width=1, height=1),
+                            Window(char=grid.TOP_MID, height=1),
+                            Window(char=grid.TOP_RIGHT, width=1, height=1),
+                        ],
+                        style="class:border",
+                    ),
+                    Window(
+                        content=CompletionsMenuControl(),
+                        width=Dimension(min=8),
+                        height=Dimension(min=1, max=max_height),
+                        scroll_offsets=ScrollOffsets(
+                            top=scroll_offset, bottom=scroll_offset
+                        ),
+                        dont_extend_width=True,
+                        z_index=z_index,
+                    ),
+                    VSplit(
+                        [
+                            Window(char=grid.BOTTOM_LEFT, width=1, height=1),
+                            Window(char=grid.BOTTOM_MID, height=1),
+                            Window(char=grid.BOTTOM_RIGHT, width=1, height=1),
+                        ],
+                        style="class:border",
+                    ),
+                ],
+                style="class:menu",
+            ),
+            # Show when there are completions but not at the point we are
+            # returning the input.
+            filter=has_completions & ~is_done & extra_filter,
+        )
```

### Comparing `euporie-2.3.2/euporie/core/widgets/page.py` & `euporie-2.4.0/euporie/core/widgets/page.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 """Contain containers which display children at full height vertially stacked."""
 
 from __future__ import annotations
 
-import asyncio
-import contextvars
 import logging
 import weakref
 from typing import TYPE_CHECKING, cast
 
 from prompt_toolkit.application.current import get_app
 from prompt_toolkit.data_structures import Point
+from prompt_toolkit.eventloop.utils import run_in_executor_with_context
 from prompt_toolkit.filters import is_searching
 from prompt_toolkit.layout.containers import (
     Container,
     ScrollOffsets,
     Window,
     WindowRenderInfo,
     to_container,
 )
 from prompt_toolkit.layout.controls import UIContent
 from prompt_toolkit.layout.dimension import Dimension, to_dimension
+from prompt_toolkit.layout.layout import walk
 from prompt_toolkit.layout.mouse_handlers import MouseHandlers
 from prompt_toolkit.layout.screen import Char, Screen, WritePosition
 from prompt_toolkit.mouse_events import MouseEvent, MouseEventType, MouseModifier
 
 from euporie.core.data_structures import DiInt
 
 if TYPE_CHECKING:
-    from typing import Callable, Sequence
+    from typing import Callable, Iterable, Sequence
 
     from prompt_toolkit.key_binding.key_bindings import (
         KeyBindingsBase,
         NotImplementedOrNone,
     )
     from prompt_toolkit.layout.containers import AnyContainer
     from prompt_toolkit.layout.dimension import AnyDimension
+    from prompt_toolkit.utils import Event
 
     MouseHandler = Callable[[MouseEvent], object]
 
 log = logging.getLogger(__name__)
 
 
 class BoundedWritePosition(WritePosition):
@@ -80,18 +81,32 @@
         self.parent = parent
         self.child = weakref.proxy(child)
         self.container = to_container(child)
 
         self.screen = Screen(default_char=Char(char=" "))
         self.mouse_handlers = MouseHandlers()
 
+        self.render_counter = -1
+        self._invalid = True
+        self._invalidate_events: list[Event[object]] = []
+        self._layout_hash = 0
         self.height = 0
         self.width = 0
 
-        self.refresh = True
+    def invalidate(self) -> None:
+        """Flag the child's rendering as out-of-date."""
+        self._invalid = True
+
+    def _invalidate_handler(self, sender: object) -> None:
+        self.invalidate()
+
+    @property
+    def layout_hash(self) -> int:
+        """Return a hash of the child's current layout."""
+        return sum(hash(container) for container in walk(self.container))
 
     def render(
         self,
         available_width: int,
         available_height: int,
         style: str = "",
     ) -> None:
@@ -99,17 +114,32 @@
 
         Args:
             available_width: The height available for rendering
             available_height: The width available for rendering
             style: The parent style to apply when rendering
 
         """
-        if self.refresh:
-            self.refresh = False
+        # Check if refresh is needed
+        refresh = False
+        new_layout_hash = self.layout_hash
+        if self.render_counter != (new_render_counter := get_app().render_counter):
+            if (
+                self._invalid
+                or self.width != available_width
+                or self._layout_hash != (new_layout_hash := self.layout_hash)
+            ):
+                self.render_counter = new_render_counter
+                refresh = True
+
+        # Refresh if needed
+        if refresh:
+            self._invalid = False
+            self._layout_hash = new_layout_hash
             # log.debug("Re-rendering cell %s", self.child.index)
+            self.width = available_width
             self.height = self.container.preferred_height(
                 available_width, available_height
             ).preferred
             # TODO - allow horizontal scrolling too
             # self.width = self.container.preferred_width(available_width).width
             self.width = available_width
 
@@ -124,14 +154,28 @@
                 ),
                 style,
                 erase_bg=True,
                 z_index=0,
             )
             self.screen.draw_all_floats()
 
+            # Collect invalidation events
+            def gather_events() -> Iterable[Event[object]]:
+                for container in walk(self.container):
+                    if isinstance(container, Window):
+                        for event in container.content.get_invalidate_events():
+                            event += self._invalidate_handler
+                            yield event
+
+            # Remove all the original event handlers
+            for event in self._invalidate_events:
+                event -= self._invalidate_handler
+            # Update the list of handlers
+            self._invalidate_events = list(gather_events())
+
     def blit(
         self,
         screen: Screen,
         mouse_handlers: MouseHandlers,
         left: int,
         top: int,
         cols: slice,
@@ -234,15 +278,15 @@
                         response = self.parent.scroll(1)
 
                     else:
                         response = handler(new_event)
 
                     # Refresh the child if there was a response
                     if response is None:
-                        self.refresh = True
+                        self.invalidate()
                         return response
 
                     # This would work if windows returned NotImplemented when scrolled
                     # to the start or end
                     # if response is NotImplemented:
                     #     if mouse_event.event_type == MouseEventType.SCROLL_DOWN:
                     #         response = self.parent.scroll(-1)
@@ -256,15 +300,15 @@
                             MouseModifier.SHIFT,
                             MouseModifier.CONTROL,
                         }:
                             self.parent.select(index, extend=True)
                         else:
                             self.parent.select(index, extend=False)
                         response = None
-                        self.refresh = True
+                        self.invalidate()
 
                         # Attempt to focus the container
                         layout.focus(self.child)
 
                     return response
 
                 mouse_handler_wrappers[handler] = wrapped_mouse_handler
@@ -312,14 +356,16 @@
         for window, point in self.screen.menu_positions.items():
             screen.menu_positions[window] = Point(x=left + point.x, y=top + point.y)
 
 
 class ScrollingContainer(Container):
     """A scrollable container which renders only the currently visible children."""
 
+    render_info: WindowRenderInfo | None
+
     def __init__(
         self,
         children: Callable[[], Sequence[AnyContainer]] | Sequence[AnyContainer],
         height: AnyDimension = None,
         width: AnyDimension = None,
         style: str | Callable[[], str] = "",
     ) -> None:
@@ -357,49 +403,35 @@
         self.style = style
 
         self.scroll_to_cursor = False
         self.scrolling = 0
 
     def pre_render_children(self, width: int, height: int) -> None:
         """Render all unrendered children in a background thread."""
-        # Copy the current context so ``get_app()`` works in the thread
-        ctx = contextvars.copy_context()
+        # Prevent multiple calls
+        self.pre_rendered = 0.00001
 
         def render_in_thread() -> None:
-            """Create a new event loop in the thread."""
-            loop = asyncio.new_event_loop()
-            asyncio.set_event_loop(loop)
-
-            async def render_run_in_loop() -> None:
-                """Render all children sequentially."""
-                n_children = len(self.children)
-                for i in range(n_children):
-                    if i < len(self.children):
-                        self.get_child_render_info(i).render(width, height)
-                        self.pre_rendered = i / n_children
-                    get_app().invalidate()
-                self.pre_rendered = 1.0
+            """Render children in  thread."""
+            n_children = len(self.children)
+            for i in range(n_children):
+                if i < len(self.children):
+                    self.get_child_render_info(i).render(width, height)
+                    self.pre_rendered = i / n_children
                 get_app().invalidate()
+            self.pre_rendered = 1.0
+            get_app().invalidate()
 
-            loop.run_until_complete(render_run_in_loop())
-
-        async def trigger_render() -> None:
-            """Use an executor thread from the current event loop."""
-            await asyncio.get_event_loop().run_in_executor(
-                None, ctx.run, render_in_thread
-            )
-
-        get_app().create_background_task(trigger_render())
+        run_in_executor_with_context(render_in_thread)
 
     def reset(self) -> None:
         """Reet the state of this container and all the children."""
-        meta_data = list(self.child_render_infos.values())
-        for meta in meta_data:
+        for meta in self.child_render_infos.values():
             meta.container.reset()
-            meta.refresh = True
+            meta.invalidate()
 
     def preferred_width(self, max_available_width: int) -> Dimension:
         """Do not provide a preferred width - grow to fill the available space."""
         if self.width is not None:
             return Dimension(min=1, preferred=self.width, weight=1)
         return Dimension(weight=1)
 
@@ -442,23 +474,23 @@
             # Scroll into view
             if scroll:
                 self.scroll_to(new_slice.start)
             # Request a refresh of the previously selected children
             render_info: ChildRenderInfo | None
             for render_info in self._selected_child_render_infos:
                 if render_info:
-                    render_info.refresh = True
+                    render_info.invalidate()
             # If a child currently has focus, request to refresh it
-            for child in self.children:
-                if (
-                    render_info := self.child_render_infos.get(hash(child))
-                ) is not None:
-                    if app.layout.has_focus(render_info.child):
-                        render_info.refresh = True
-                        break
+            # for child in self.children:
+            #     if (
+            #         render_info := self.child_render_infos.get(hash(child))
+            #     ) is not None:
+            #         if app.layout.has_focus(render_info.child):
+            #             render_info.invalidate()
+            #             break
             # Get the first selected child and focus it
             child = self.children[new_slice.start]
             if not app.layout.has_focus(child):
                 try:
                     app.layout.focus(child)
                 except ValueError:
                     pass
@@ -561,15 +593,19 @@
         Returns:
             :py:const:`NotImplemented` is scrolling is not allowed, otherwise
                 :py:const:`None`
 
         """
         # self.refresh_children = True
         if n > 0:
-            if min(self.visible_indicies) == 0 and self.index_positions[0] is not None:
+            if (
+                min(self.visible_indicies) == 0
+                and self.index_positions
+                and self.index_positions[0] is not None
+            ):
                 n = min(n, 0 - self.index_positions[0] - self.scrolling)
                 if self.index_positions[0] + self.scrolling + n > 0:
                     return NotImplemented
         elif n < 0:
             bottom_index = len(self.children) - 1
             if bottom_index in self.visible_indicies:
                 bottom_child = self.get_child_render_info(bottom_index)
@@ -632,54 +668,46 @@
         """
         ypos = write_position.ypos
         xpos = write_position.xpos
 
         available_width = write_position.width
         available_height = write_position.height
 
-        # Trigger pre-rendering of children
-        if not self.pre_rendered:
-            self.pre_render_children(available_width, available_height)
-
         # Update screen height
         screen.height = max(screen.height, ypos + write_position.height)
 
         # Record children which are currently visible
         visible_indicies = set()
 
         # Force the selected children to refresh
         selected_indices = self.selected_indices
         self._selected_child_render_infos = []
         for index in selected_indices:
             render_info = self.get_child_render_info(index)
-            # Do not bother to re-render children if we are scrolling
+            # Do not bother to re-render selected children if we are scrolling
             if not self.scrolling:
-                render_info.refresh = True
+                render_info.invalidate()
             self._selected_child_render_infos.append(render_info)
             self.index_positions[index] = None
 
-        # Refresh all children if the width has changed
-        if self.last_write_position.width != write_position.width:
-            for child_render_info in self.child_render_infos.values():
-                child_render_info.refresh = True
-
         # Refresh visible children if searching
         if is_searching():
             for index in self.visible_indicies:
-                self.get_child_render_info(index).refresh = True
+                self.get_child_render_info(index).invalidate()
 
         # Scroll to make the cursor visible
+        layout = get_app().layout
         if self.scroll_to_cursor:
             selected_child_render_info = self._selected_child_render_infos[0]
             selected_child_render_info.render(
                 available_width=available_width,
                 available_height=available_height,
                 style=f"{parent_style} {self.style}",
             )
-            current_window = get_app().layout.current_window
+            current_window = layout.current_window
             cursor_position = selected_child_render_info.screen.cursor_positions.get(
                 current_window
             )
             if cursor_position:
                 cursor_row = self.selected_child_position + cursor_position.y
                 if cursor_row < 0:
                     self.selected_child_position -= cursor_row
@@ -801,21 +829,30 @@
         # screen.draw_all_floats()
 
         # Ensure the focused child is always in the layout
         visible_indicies.add(self._selected_slice.start)
 
         # Update which children will appear in the layout
         self.visible_indicies = visible_indicies
+
+        # Update parent relations in layout
+        def _walk(e: Container) -> None:
+            for c in e.get_children():
+                layout._child_to_parent[c] = e
+                _walk(c)
+
+        _walk(self)
+
         # Record where the contain was last drawn so we can determine if cell outputs
         # are partially obscured
         self.last_write_position = write_position
 
         # Calculate scrollbar info
         sizes = self.known_sizes
-        avg_size = sum(sizes.values()) / len(sizes)
+        avg_size = sum(sizes.values()) / len(sizes) if sizes else 0
         n_children = len(self.children)
         for i in range(n_children):
             if i not in sizes:
                 sizes[i] = int(avg_size)
         content_height = max(sum(sizes.values()), 1)
 
         # Mock up a WindowRenderInfo so we can draw a scrollbar margin
@@ -832,14 +869,18 @@
             x_offset=xpos,
             y_offset=ypos,
             wrap_lines=False,
         )
         # Signal that we are no longer scrolling
         self.scrolling = 0
 
+        # Trigger pre-rendering of children
+        if not self.pre_rendered:
+            self.pre_render_children(available_width, available_height)
+
     @property
     def vertical_scroll(self) -> int:
         """The best guess at the absolute vertical scroll position."""
         return (
             sum(list(self.known_sizes.values())[: self._selected_slice.start])
             - self.selected_child_position
         )
```

### Comparing `euporie-2.3.2/euporie/core/widgets/pager.py` & `euporie-2.4.0/euporie/core/widgets/pager.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     ConditionalContainer,
     DynamicContainer,
     HSplit,
 )
 from prompt_toolkit.widgets import Box
 
 from euporie.core.commands import add_cmd
-from euporie.core.convert.base import BASE64_FORMATS, MIME_FORMATS, find_route
+from euporie.core.convert.core import BASE64_FORMATS, MIME_FORMATS, find_route
 from euporie.core.current import get_app
 from euporie.core.filters import pager_has_focus
 from euporie.core.key_binding.registry import (
     load_registered_bindings,
     register_bindings,
 )
 from euporie.core.widgets.cell_outputs import CellOutput, CellOutputDataElement
```

### Comparing `euporie-2.3.2/euporie/core/widgets/palette.py` & `euporie-2.4.0/euporie/core/widgets/palette.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,27 +13,29 @@
 from prompt_toolkit.layout.containers import HSplit, ScrollOffsets, VSplit, Window
 from prompt_toolkit.layout.controls import UIContent, UIControl
 from prompt_toolkit.mouse_events import MouseEvent, MouseEventType
 
 from euporie.core.commands import Command, add_cmd, commands
 from euporie.core.current import get_app
 from euporie.core.key_binding.registry import register_bindings
-from euporie.core.margins import ScrollbarMargin
+from euporie.core.margins import MarginContainer, ScrollbarMargin
 from euporie.core.widgets.decor import FocusedStyle
 from euporie.core.widgets.dialog import Dialog
 from euporie.core.widgets.forms import Text
+from euporie.core.widgets.status_bar import StatusContainer
 
 if TYPE_CHECKING:
     from prompt_toolkit.buffer import Buffer
     from prompt_toolkit.formatted_text import StyleAndTextTuples
     from prompt_toolkit.key_binding.key_bindings import NotImplementedOrNone
     from prompt_toolkit.key_binding.key_processor import KeyPressEvent
     from prompt_toolkit.layout.controls import GetLinePrefixCallable
 
-    from euporie.core.app import BaseApp, StatusBarFields
+    from euporie.core.app import BaseApp
+    from euporie.core.widgets.status_bar import StatusBarFields
 
 log = logging.getLogger(__name__)
 
 
 class _CommandMatch(NamedTuple):
     length: int
     position: int
@@ -188,47 +190,42 @@
             multiline=False,
             accept_handler=self.accept,
             style="class:input",
             expand=False,
             placeholder="  Type to search…",
         )
         self.text_area.buffer.on_text_changed += self.text_changed
-        scroll_bar_margin = ScrollbarMargin(display_arrows=False)
 
-        self.body = HSplit(
-            [
-                VSplit(
-                    [FocusedStyle(self.text_area)],
-                    padding=1,
-                ),
-                Window(
-                    CommandMenuControl(self),
-                    scroll_offsets=ScrollOffsets(bottom=1),
-                    right_margins=[scroll_bar_margin],
-                ),
-            ],
+        self.body = StatusContainer(
+            body=HSplit(
+                [
+                    VSplit(
+                        [FocusedStyle(self.text_area)],
+                        padding=1,
+                    ),
+                    VSplit(
+                        [
+                            window := Window(
+                                CommandMenuControl(self),
+                                scroll_offsets=ScrollOffsets(bottom=1),
+                            ),
+                            MarginContainer(ScrollbarMargin(), target=window),
+                        ]
+                    ),
+                ],
+            ),
+            status=self.__pt_status__,
         )
         self.buttons = {}
 
-        get_app().container_statuses[self.container] = self.statusbar_fields
-
     def load(self) -> None:
         """Reset the dialog ready for display."""
         self.text_area.buffer.text = ""
         self.to_focus = self.text_area
 
-    def statusbar_fields(
-        self,
-    ) -> StatusBarFields:
-        """Return a list of statusbar field values shown then this tab is active."""
-        if self.matches:
-            return ([self.matches[self.index].command.description], [])
-        else:
-            return ([], [])
-
     def select(self, n: int, event: KeyPressEvent | None = None) -> None:
         """Change the index of the selected command.
 
         Args:
             n: The relative amount by which to change the selected index
             event: Ignored
 
@@ -263,14 +260,20 @@
         if self.matches:
             self.hide()
             self.matches[self.index].command.run()
             return True
         else:
             return False
 
+    def __pt_status__(self) -> StatusBarFields | None:
+        """Return a list of statusbar field values shown then this tab is active."""
+        if self.matches:
+            return ([self.matches[self.index].command.description], [])
+        return None
+
     # ################################### Commands ####################################
 
     @staticmethod
     @add_cmd()
     def _toggle_command_palette() -> None:
         """Show the command palette."""
         if command_palette := get_app().dialogs.get("command-palette"):
```

### Comparing `euporie-2.3.2/euporie/core/widgets/search_bar.py` & `euporie-2.4.0/euporie/core/widgets/search_bar.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import logging
 from typing import TYPE_CHECKING
 
 from prompt_toolkit.filters.app import is_searching
 from prompt_toolkit.key_binding.vi_state import InputMode
 from prompt_toolkit.layout.controls import BufferControl, SearchBufferControl
 from prompt_toolkit.search import SearchDirection
+from prompt_toolkit.selection import SelectionState
 from prompt_toolkit.widgets import SearchToolbar as PtkSearchToolbar
 
 from euporie.core.commands import add_cmd
 from euporie.core.current import get_app
 from euporie.core.key_binding.registry import (
     load_registered_bindings,
     register_bindings,
@@ -53,14 +54,28 @@
                 ("", " "),
             ],
         )
         self.control.key_bindings = load_registered_bindings(
             "euporie.core.widgets.search_bar.SearchBar"
         )
 
+    register_bindings(
+        {
+            "euporie.core.app.BaseApp": {
+                "find": ["c-f", "f3", "f7"],
+                "find-next": "c-g",
+                "find-previous": "c-p",
+            },
+            "euporie.core.widgets.search_bar.SearchBar": {
+                "accept-search": "enter",
+                "stop-search": "escape",
+            },
+        }
+    )
+
 
 def start_global_search(
     buffer_control: BufferControl | None = None,
     direction: SearchDirection = SearchDirection.FORWARD,
 ) -> None:
     """Start a search through all searchable `buffer_controls` in the layout."""
     app = get_app()
@@ -90,14 +105,15 @@
             isinstance(control, BufferControl)
             and control.search_buffer_control == search_buffer_control
         ):
             # Set its search direction
             control.search_state.direction = direction
             # Add it to our list
             searchable_controls.append(control)
+
     # Stop the search if we did not find any searchable controls
     if not searchable_controls:
         return
 
     # If the current control is searchable, link it
     if current_control in searchable_controls:
         assert isinstance(current_control, BufferControl)
@@ -109,18 +125,15 @@
         ]
     # Make sure to focus the search BufferControl
     layout.focus(search_buffer_control)
     # If we're in Vi mode, make sure to go into insert mode.
     app.vi_state.input_mode = InputMode.INSERT
 
 
-@add_cmd(
-    menu_title="Find",
-    # filter=control_is_searchable,
-)
+@add_cmd(menu_title="Find")
 def find() -> None:
     """Enter search mode."""
     start_global_search(direction=SearchDirection.FORWARD)
 
 
 def find_prev_next(direction: SearchDirection) -> None:
     """Find the previous or next search match."""
@@ -138,18 +151,21 @@
     elif app.search_bar is not None:
         search_buffer_control = app.search_bar.control
     if isinstance(control, BufferControl) and search_buffer_control is not None:
         # Update search_state.
         search_state = control.search_state
         search_state.direction = direction
         # Apply search to buffer
-        control.buffer.apply_search(
-            search_state, include_current_position=False, count=1
+        buffer = control.buffer
+        buffer.apply_search(search_state, include_current_position=False, count=1)
+        # Set selection
+        buffer.selection_state = SelectionState(
+            buffer.cursor_position + len(search_state.text)
         )
-    # break
+        buffer.selection_state.enter_shift_mode()
 
 
 @add_cmd()
 def find_next() -> None:
     """Find the next search match."""
     find_prev_next(SearchDirection.FORWARD)
 
@@ -166,16 +182,16 @@
 def stop_search() -> None:
     """Abort the search."""
     layout = get_app().layout
     buffer_control = layout.search_target_buffer_control
     if buffer_control is None:
         return
     search_buffer_control = buffer_control.search_buffer_control
-    # Focus the original buffer again.
-    layout.focus(buffer_control)
+    # Focus the previous control
+    layout.focus(layout.previous_control)
     # Close the search toolbar
     if search_buffer_control is not None:
         del layout.search_links[search_buffer_control]
         # Reset content of search control.
         search_buffer_control.buffer.reset()
     # Redraw everything
     get_app().refresh()
@@ -198,27 +214,24 @@
             and control.search_buffer_control == search_buffer_control
         ):
             search_state = control.search_state
             # Update search state.
             if search_buffer_control.buffer.text:
                 search_state.text = search_buffer_control.buffer.text
             # Apply search.
-            control.buffer.apply_search(search_state, include_current_position=True)
+            control.buffer.apply_search(
+                search_state, include_current_position=True, count=1
+            )
+
+    # Set selection on target control
+    buffer_control = layout.search_target_buffer_control
+    if buffer_control and control.is_focusable():
+        buffer = buffer_control.buffer
+        buffer.selection_state = SelectionState(
+            buffer.cursor_position + len(search_state.text)
+        )
+        buffer.selection_state.enter_shift_mode()
+
     # Add query to history of search line.
     search_buffer_control.buffer.append_to_history()
     # Stop the search
     stop_search()
-
-
-register_bindings(
-    {
-        "euporie.core.app.BaseApp": {
-            "find": ["c-f", "f3", "f7"],
-            "find-next": "c-g",
-            "find-previous": "c-p",
-        },
-        "euporie.core.widgets.search_bar.SearchBar": {
-            "accept-search": "enter",
-            "stop-search": "escape",
-        },
-    }
-)
```

### Comparing `euporie-2.3.2/euporie/core/widgets/status_bar.py` & `euporie-2.4.0/euporie/notebook/tabs/display.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,81 @@
-"""Define a status-bar widget."""
+"""Contain a tab for displaying files."""
 
 from __future__ import annotations
 
+import logging
 from typing import TYPE_CHECKING
 
-from prompt_toolkit.filters.utils import to_filter
-from prompt_toolkit.layout.containers import (
-    ConditionalContainer,
-    VSplit,
-    Window,
-    WindowAlign,
-)
-from prompt_toolkit.layout.controls import FormattedTextControl
-
-from euporie.core.config import add_setting
-from euporie.core.current import get_app
-from euporie.core.filters import is_searching
+from prompt_toolkit.eventloop.utils import run_in_executor_with_context
+from prompt_toolkit.layout.containers import VSplit
+from prompt_toolkit.layout.dimension import Dimension
+
+from euporie.core.convert.core import MIME_FORMATS, get_format
+from euporie.core.margins import MarginContainer, ScrollbarMargin
+from euporie.core.tabs.base import Tab
+from euporie.core.widgets.display import Display
 
 if TYPE_CHECKING:
-    from prompt_toolkit.filters.base import FilterOrBool
+    from pathlib import Path
+
     from prompt_toolkit.layout.containers import AnyContainer
 
+    from euporie.core.app import BaseApp
+    from euporie.core.widgets.status_bar import StatusBarFields
 
-class StatusBar:
-    """A status bar which shows the status of the current tab."""
+log = logging.getLogger(__name__)
 
-    def __init__(self, extra_filter: FilterOrBool = True) -> None:
-        """Create a new status bar instance."""
-        self.app = get_app()
-        self.container = ConditionalContainer(
-            content=VSplit(
-                [
-                    Window(
-                        FormattedTextControl(
-                            lambda: self.app.format_status(part="left")
-                        ),
-                        style="class:status",
-                    ),
-                    Window(
-                        FormattedTextControl(
-                            lambda: self.app.format_status(part="right")
-                        ),
-                        style="class:status.right",
-                        align=WindowAlign.RIGHT,
-                    ),
-                ],
-                height=1,
-            ),
-            filter=get_app().config.filter("show_status_bar")
-            & ~is_searching
-            & to_filter(extra_filter),
-        )
 
-    def __pt_container__(self) -> AnyContainer:
-        """Return the widget's container."""
-        return self.container
-
-    # ################################### Settings ####################################
-
-    add_setting(
-        name="show_status_bar",
-        flags=["--show-status-bar"],
-        type_=bool,
-        title="status bar",
-        help_="Show the status bar",
-        default=True,
-        schema={
-            "type": "boolean",
-        },
-        description="""
-            Whether the status bar should be shown at the bottom of the screen.
-        """,
-    )
+class DisplayTab(Tab):
+    """Tab class for displaying files."""
+
+    name = "File Viewer"
+    mime_types = set(MIME_FORMATS.keys())
+
+    def __init__(self, app: BaseApp, path: Path | None = None) -> None:
+        """Call when the tab is created."""
+        super().__init__(app, path)
+
+        # Load file and container in background
+        if self.path is not None:
+
+            def _load() -> None:
+                self.container = self.load_container()
+                self.app.layout.focus(self.container)
+                self.app.invalidate()
+
+            run_in_executor_with_context(_load)
+
+    def __pt_status__(self) -> StatusBarFields | None:
+        """Return a list of statusbar field values shown then this tab is active."""
+        return ([str(self.path)], [])
+
+    @property
+    def title(self) -> str:
+        """Return the tab title."""
+        if self.path is not None:
+            return str(self.path.name) or str(self.path)
+        else:
+            return "<file>"
+
+    def load_container(self) -> AnyContainer:
+        """Abcract method for loading the notebook's main container."""
+        assert self.path is not None
+
+        self.display = Display(
+            data=self.path.read_bytes(),
+            format_=get_format(self.path),
+            path=self.path,
+            focusable=True,
+            focus_on_click=True,
+            always_hide_cursor=True,
+            dont_extend_height=False,
+            scrollbar=False,
+        )
+        return VSplit(
+            [
+                self.display,
+                MarginContainer(ScrollbarMargin(), target=self.display.window),
+            ],
+            width=Dimension(weight=1),
+            height=Dimension(weight=1),
+        )
```

### Comparing `euporie-2.3.2/euporie/core/widgets/tree.py` & `euporie-2.4.0/euporie/core/widgets/tree.py`

 * *Files identical despite different names*

### Comparing `euporie-2.3.2/euporie/hub/app.py` & `euporie-2.4.0/euporie/hub/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     def __init__(self, app_cls: type[BaseApp]) -> None:
         """Set the interaction function for the SSH session."""
         self.app_cls = app_cls
 
     def begin_auth(self, username: str) -> bool | Awaitable[bool]:
         """Perform authentication in the SSH server."""
-        if self.app_cls.config.no_auth:
+        if not self.app_cls.config.auth:
             # No authentication.
             return False
         return super().begin_auth(username)
 
     def session_requested(self) -> PromptToolkitSSHSession:
         """Return an SSH session."""
         # Not sure why mypy gives an error here
@@ -64,26 +64,28 @@
     """
 
     name = "hub"
 
     @classmethod
     def launch(cls) -> None:
         """Launch the HubApp SSH server."""
+        # Default logging configuration
+        setup_logs()
+
         # Configure some setting defaults
         cls.config.settings["log_file"].value = "-"
+        cls.config.settings["log_level"].value = "info"
         cls.config.settings[
             "log_config"
         ].value = '{"loggers": {"asyncssh": {"handlers":["stdout"], "level": "DEBUG"}}}'
 
         # Load the app's configuration
         cls.config.load(cls)
-        # Configure the logs
-        setup_logs(cls.config)
 
-        if cls.config.no_auth:
+        if not cls.config.auth:
             log.warning(
                 "This server has been configured without SSH authentication, "
                 "meaning anyone can connect"
             )
 
         # Import the hubbed app
         if entry_point := {
@@ -184,19 +186,19 @@
         description="""
             One or more OpenSSH-style :file:`authorized_keys` files, containing
             public keys for authorized clients.
         """,
     )
 
     add_setting(
-        name="no_auth",
-        flags=["--no-auth"],
+        name="auth",
+        flags=["--auth"],
         type_=bool,
         help_="Allow unauthenticated access to euporie hub",
-        default=False,
+        default=True,
         description="""
             When set, users will be able to access euporie hub without authentication.
 
             .. warning::
 
                This option is dangerous, as arbitrary code can be executed through
                euporie apps.
```

### Comparing `euporie-2.3.2/euporie/notebook/app.py` & `euporie-2.4.0/euporie/notebook/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from prompt_toolkit.layout.dimension import Dimension
 
 from euporie.core import __logo__
 from euporie.core.app import BaseApp
 from euporie.core.commands import add_cmd, get_cmd
 from euporie.core.config import add_setting
 from euporie.core.key_binding.registry import register_bindings
+from euporie.core.tabs.base import Tab
 from euporie.core.widgets.decor import Pattern
 from euporie.core.widgets.dialog import (
     AboutDialog,
     ConfirmDialog,
     ErrorDialog,
     MsgBoxDialog,
     NoKernelsDialog,
@@ -51,18 +52,17 @@
 
 if TYPE_CHECKING:
     from asyncio import AbstractEventLoop
     from typing import Any, Callable, Sequence
 
     from prompt_toolkit.formatted_text import StyleAndTextTuples
     from prompt_toolkit.layout.containers import AnyContainer, Float
-    from upath import UPath
 
-    from euporie.core.tabs.base import Tab
     from euporie.core.widgets.cell import Cell
+    from euporie.core.widgets.status_bar import StatusBarFields
 
 log = logging.getLogger(__name__)
 
 
 class NotebookApp(BaseApp):
     """Notebook app.
 
@@ -77,54 +77,32 @@
 
     def __init__(self, **kwargs: Any) -> None:
         """Create a new euporie text user interface application instance."""
         kwargs.setdefault("title", "euporie-notebook")
         kwargs.setdefault("full_screen", True)
         kwargs.setdefault("leave_graphics", False)
         super().__init__(**kwargs)
-        self.search_bar = SearchBar()
         self.bindings_to_load.append("euporie.notebook.app.NotebookApp")
-        self.pre_run_callables.append(self.load_default_statusbar_fields)
 
         # Register config hooks
         self.config.get_item("show_cell_borders").event += lambda x: self.refresh()
 
-    def load_default_statusbar_fields(self) -> None:
+    def statusbar_defaults(self) -> StatusBarFields | None:
         """Load the default statusbar fields (run after keybindings are loaded)."""
-        self.status_default = (
+        return (
             [
                 [
                     ("", "Press "),
                     ("bold", get_cmd("new-notebook").key_str()),
                     ("", " to start a new notebook"),
                 ],
             ],
             [[("", "Press "), ("bold", get_cmd("quit").key_str()), ("", " to quit")]],
         )
 
-    def get_file_tab(self, path: UPath) -> type[Tab]:
-        """Return the tab to use for a file path."""
-        if path.suffix == ".ipynb":
-            return Notebook
-        else:
-            import mimetypes
-
-            from euporie.core.convert.base import MIME_FORMATS
-
-            mime, _ = mimetypes.guess_type(path)
-            log.debug("File %s has mime type: %s", path, mime)
-            if (mime or "").startswith("text/") and mime not in MIME_FORMATS:
-                from euporie.notebook.tabs.edit import EditorTab
-
-                return EditorTab
-            else:
-                from euporie.notebook.tabs.display import DisplayTab
-
-                return DisplayTab
-
     async def _poll_terminal_colors(self) -> None:
         """Repeatedly query the terminal for its background and foreground colours."""
         while self.config.terminal_polling_interval:
             await asyncio.sleep(self.config.terminal_polling_interval)
             self.term_info.colors.send()
 
     def post_load(self) -> None:
@@ -217,16 +195,15 @@
             filter=Condition(
                 lambda: (len(self.tabs) > 1 or self.config.always_show_tab_bar)
                 and TabMode(self.config.tab_mode) == TabMode.STACK
             ),
         )
 
         self.pager = Pager()
-
-        assert self.search_bar is not None
+        self.search_bar = SearchBar()
 
         self.dialogs["command-palette"] = CommandPalette(self)
         self.dialogs["about"] = AboutDialog(self)
         self.dialogs["open-file"] = OpenFileDialog(self)
         self.dialogs["save-as"] = SaveAsDialog(self)
         self.dialogs["no-kernels"] = NoKernelsDialog(self)
         self.dialogs["change-kernel"] = SelectKernelDialog(self)
@@ -278,15 +255,15 @@
                                 ],
                                 width=Dimension(weight=1),
                             ),
                         ],
                         height=Dimension(min=1),
                     ),
                     self.search_bar,
-                    StatusBar(),
+                    StatusBar(default=self.statusbar_defaults()),
                 ],
                 style="class:body",
             ),
             floats=cast("list[Float]", self.floats),
         )
 
         return self.container
@@ -381,15 +358,15 @@
         return [
             MenuItem(
                 "File",
                 children=[
                     get_cmd("new-notebook").menu,
                     get_cmd("open-file").menu,
                     separator,
-                    get_cmd("save-notebook").menu,
+                    get_cmd("save-file").menu,
                     get_cmd("save-as").menu,
                     get_cmd("close-tab").menu,
                     separator,
                     get_cmd("quit").menu,
                 ],
             ),
             MenuItem(
```

### Comparing `euporie-2.3.2/euporie/notebook/filters.py` & `euporie-2.4.0/euporie/notebook/filters.py`

 * *Files identical despite different names*

### Comparing `euporie-2.3.2/euporie/notebook/tabs/display.py` & `euporie-2.4.0/euporie/notebook/tabs/json.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,55 @@
-"""Contain a tab for displaying files."""
+"""Contain a tab for displaying JSON data."""
 
 from __future__ import annotations
 
+import json
 import logging
 from typing import TYPE_CHECKING
 
+from prompt_toolkit.eventloop.utils import run_in_executor_with_context
 from prompt_toolkit.layout.containers import VSplit
 from prompt_toolkit.layout.dimension import Dimension
 
-from euporie.core.convert.base import get_format
-from euporie.core.margins import MarginContainer, ScrollbarMargin
 from euporie.core.tabs.base import Tab
-from euporie.core.widgets.display import Display
+from euporie.core.widgets.tree import JsonView
 
 if TYPE_CHECKING:
-    from typing import Sequence
+    from pathlib import Path
 
-    from prompt_toolkit.formatted_text import AnyFormattedText
     from prompt_toolkit.layout.containers import AnyContainer
-    from upath import UPath
 
     from euporie.core.app import BaseApp
+    from euporie.core.widgets.status_bar import StatusBarFields
 
 log = logging.getLogger(__name__)
 
 
-class DisplayTab(Tab):
-    """Tab class for displaying files."""
+class JsonTab(Tab):
+    """Tab class for JSON data."""
 
-    def __init__(self, app: BaseApp, path: UPath | None = None) -> None:
+    name = "JSON Viewer"
+    mime_types = {"*json"}
+    filte_types = {".json"}
+
+    def __init__(self, app: BaseApp, path: Path | None = None) -> None:
         """Call when the tab is created."""
         super().__init__(app, path)
+
+        # Load file and container in background
         if self.path is not None:
-            self.container = self.load_container()
 
-    def statusbar_fields(
-        self,
-    ) -> tuple[Sequence[AnyFormattedText], Sequence[AnyFormattedText]]:
+            def _load() -> None:
+                self.container = self.load_container()
+                self.app.layout.focus(self.container)
+                self.app.invalidate()
+
+            run_in_executor_with_context(_load)
+
+    def __pt_status__(self) -> StatusBarFields | None:
         """Return a list of statusbar field values shown then this tab is active."""
         return ([str(self.path)], [])
 
     @property
     def title(self) -> str:
         """Return the tab title."""
         if self.path is not None:
@@ -48,25 +57,17 @@
         else:
             return "<file>"
 
     def load_container(self) -> AnyContainer:
         """Abcract method for loading the notebook's main container."""
         assert self.path is not None
 
-        self.display = Display(
-            data=self.path.read_bytes(),
-            format_=get_format(self.path),
-            path=self.path,
-            focusable=True,
-            focus_on_click=True,
-            always_hide_cursor=True,
-            dont_extend_height=False,
-            scrollbar=False,
-        )
+        data = json.load(self.path.open())
+
         return VSplit(
             [
-                self.display,
-                MarginContainer(ScrollbarMargin(), target=self.display.window),
+                JsonView(data, title=self.path.name, expanded=True),
+                # MarginContainer(ScrollbarMargin(), target=self.display.window),
             ],
             width=Dimension(weight=1),
             height=Dimension(weight=1),
         )
```

### Comparing `euporie-2.3.2/euporie/notebook/tabs/edit.py` & `euporie-2.4.0/euporie/core/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,74 @@
-"""Contain a tab for displaying files."""
+"""Miscellaneou utility classes."""
 
 from __future__ import annotations
 
-import logging
-from typing import TYPE_CHECKING
+from itertools import chain
+from typing import TYPE_CHECKING, Sequence, TypeVar, overload
 
-from prompt_toolkit.layout.containers import VSplit
-from prompt_toolkit.layout.dimension import Dimension
+from prompt_toolkit.mouse_events import MouseButton, MouseEventType
 
-from euporie.core.kernel import Kernel, MsgCallbacks
-from euporie.core.lexers import detect_lexer
+if TYPE_CHECKING:
+    from typing import Callable, Iterable
 
-# from euporie.core.margins import MarginContainer
-from euporie.core.tabs.base import KernelTab
-from euporie.core.widgets.inputs import KernelInput
+    from prompt_toolkit.key_binding.key_bindings import NotImplementedOrNone
+    from prompt_toolkit.layout.mouse_handlers import MouseHandler
+    from prompt_toolkit.mouse_events import MouseEvent
 
-if TYPE_CHECKING:
-    from typing import Sequence
+T = TypeVar("T")
 
-    from prompt_toolkit.formatted_text import AnyFormattedText
-    from prompt_toolkit.layout.containers import AnyContainer
-    from upath import UPath
-
-    from euporie.core.app import BaseApp
-    from euporie.core.comm.base import Comm
-
-log = logging.getLogger(__name__)
-
-
-class EditorTab(KernelTab):
-    """Tab class for editing text files."""
-
-    allow_stdin = True
-    _metadata = {}
-
-    def __init__(
-        self,
-        app: BaseApp,
-        path: UPath | None = None,
-        kernel: Kernel | None = None,
-        comms: dict[str, Comm] | None = None,
-        use_kernel_history: bool = False,
-    ) -> None:
-        """Call when the tab is created."""
-        self.default_callbacks = MsgCallbacks({})
-        super().__init__(app, path, kernel, comms, use_kernel_history)
-
-        # Load file
-        if self.path is not None:
-            text = self.path.read_text()
-        else:
-            text = ""
 
-        # Detect language
-        lexer = detect_lexer(text, path)
-        self._metadata = {"kernelspec": {"language": lexer.name}}
-
-        # Load UI
-        self.container = self.load_container()
-
-        self.input_box.text = text
-
-    def statusbar_fields(
-        self,
-    ) -> tuple[Sequence[AnyFormattedText], Sequence[AnyFormattedText]]:
-        """Return a list of statusbar field values shown then this tab is active."""
-        return ([str(self.path)], [])
+class ChainedList(Sequence[T]):
+    """A list-like class which chains multiple lists."""
+
+    def __init__(self, *lists: Iterable[T]) -> None:
+        """Create a new instance."""
+        self.lists = lists
 
     @property
-    def title(self) -> str:
-        """Return the tab title."""
-        if self.path is not None:
-            return str(self.path.name)
+    def data(self) -> list[T]:
+        """Return the list data."""
+        return list(chain.from_iterable(self.lists))
+
+    @overload
+    def __getitem__(self, i: int) -> T:
+        ...
+
+    @overload
+    def __getitem__(self, i: slice) -> list[T]:
+        ...
+
+    def __getitem__(self, i):
+        """Get an item from the chained lists."""
+        return self.data[i]
+
+    def __len__(self) -> int:
+        """Return the length of the chained lists."""
+        return len(self.data)
+
+
+def dict_merge(target_dict: dict, input_dict: dict) -> None:
+    """Merge the second dictionary onto the first."""
+    for k in input_dict:
+        if k in target_dict:
+            if isinstance(target_dict[k], dict) and isinstance(input_dict[k], dict):
+                dict_merge(target_dict[k], input_dict[k])
+            elif isinstance(target_dict[k], list) and isinstance(input_dict[k], list):
+                target_dict[k] = [*target_dict[k], *input_dict[k]]
+            else:
+                target_dict[k] = input_dict[k]
         else:
-            return "<New File>"
+            target_dict[k] = input_dict[k]
+
+
+def on_click(func: Callable) -> MouseHandler:
+    """Return a mouse handler which call a given function on click."""
+
+    def _mouse_handler(mouse_event: MouseEvent) -> NotImplementedOrNone:
+        if (
+            mouse_event.button == MouseButton.LEFT
+            and mouse_event.event_type == MouseEventType.MOUSE_UP
+        ):
+            return func()
+        return NotImplemented
 
-    def load_container(self) -> AnyContainer:
-        """Abcract method for loading the notebook's main container."""
-        assert self.path is not None
-
-        self.input_box = KernelInput(kernel_tab=self)
-
-        return VSplit(
-            [
-                self.input_box,
-                # MarginContainer(ScrollbarMargin(), target=self.input_box.window),
-            ],
-            width=Dimension(weight=1),
-            height=Dimension(weight=1),
-        )
+    return _mouse_handler
```

### Comparing `euporie-2.3.2/euporie/notebook/tabs/log.py` & `euporie-2.4.0/euporie/notebook/tabs/log.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,66 @@
 """Initiate logging for euporie.core."""
 
 from __future__ import annotations
 
-from pathlib import Path
 from typing import TYPE_CHECKING
 
 from prompt_toolkit.filters import Condition, has_focus
 from prompt_toolkit.formatted_text.base import FormattedText
-from prompt_toolkit.layout.containers import HSplit
+from prompt_toolkit.layout.containers import HSplit, VSplit
 from prompt_toolkit.layout.dimension import Dimension
 from prompt_toolkit.widgets import SearchToolbar
 
 from euporie.core.commands import add_cmd
 from euporie.core.current import get_app
 from euporie.core.log import LOG_QUEUE, QueueHandler
+from euporie.core.margins import MarginContainer, ScrollbarMargin
+from euporie.core.path import parse_path
 from euporie.core.tabs.base import Tab
 from euporie.core.widgets.formatted_text_area import FormattedTextArea
 
 if TYPE_CHECKING:
+    from pathlib import Path
     from typing import Callable
 
-    from upath import UPath
-
     from euporie.core.app import BaseApp
 
 
 class LogView(Tab):
     """A tab which allows you to view log entries."""
 
-    def __init__(self, app: BaseApp, path: UPath | None = None) -> None:
+    def __init__(self, app: BaseApp, path: Path | None = None) -> None:
         """Create a new log view tab instance."""
         super().__init__(app, path)
         # Build the container
         self.search_field = SearchToolbar(
             text_if_not_searching=[("class:not-searching", "Press '/' to search.")]
         )
         self.text_area = FormattedTextArea(
             formatted_text=[],
             read_only=True,
-            scrollbar=True,
+            scrollbar=False,
             line_numbers=Condition(lambda: self.app.config.line_numbers),
             search_field=self.search_field,
             focus_on_click=True,
             wrap_lines=False,
             dont_extend_width=False,
         )
         self.container = HSplit(
-            [self.text_area, self.search_field],
+            [
+                VSplit(
+                    [
+                        self.text_area,
+                        MarginContainer(
+                            ScrollbarMargin(), target=self.text_area.window
+                        ),
+                    ]
+                ),
+                self.search_field,
+            ],
             width=Dimension(weight=1),
             height=Dimension(weight=1),
         )
         self.hook_id = QueueHandler.hook(self.add_record)
         # Add text to the textarea
         for record in LOG_QUEUE:
             self.add_record(record)
@@ -68,15 +78,15 @@
         self.text_area.formatted_text += message
         self.text_area.buffer.cursor_position = cp
 
     @property
     def title(self) -> str:
         """Return the title of this tab."""
         suffix = (
-            f" ({Path(self.app.config.log_file).name})"
+            f" ({parse_path(self.app.config.log_file).name})"
             if self.app.config.log_file
             else ""
         )
         return f"Logs{suffix}"
 
     def close(self, cb: Callable | None = None) -> None:
         """Remove log queue handler hook on close."""
```

### Comparing `euporie-2.3.2/euporie/notebook/tabs/notebook.py` & `euporie-2.4.0/euporie/notebook/tabs/notebook.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,41 +50,53 @@
     cell_has_focus,
     code_cell_selected,
     deleted_cells,
     notebook_has_focus,
 )
 
 if TYPE_CHECKING:
+    from pathlib import Path
     from typing import Any, Deque, MutableSequence, Sequence
 
-    from prompt_toolkit.formatted_text.base import AnyFormattedText, StyleAndTextTuples
+    from prompt_toolkit.formatted_text.base import StyleAndTextTuples
     from prompt_toolkit.key_binding.key_bindings import NotImplementedOrNone
     from prompt_toolkit.layout.containers import AnyContainer
     from prompt_toolkit.mouse_events import MouseEvent
-    from upath import UPath
 
     from euporie.core.app import BaseApp
     from euporie.core.comm.base import Comm
     from euporie.core.kernel import Kernel
+    from euporie.core.widgets.status_bar import StatusBarFields
 
 log = logging.getLogger(__name__)
 
 
 class Notebook(BaseNotebook):
     """Interactive notebooks.
 
     A tab which allows running and editing a notebook.
     """
 
+    name = "Notebook Editor"
+    weight = 3
+    mime_types = {"application/x-ipynb+json"}
+    file_extensions = {".ipynb"}
+    try:
+        from jupytext.formats import NOTEBOOK_EXTENSIONS
+    except ModuleNotFoundError:
+        pass
+    else:
+        file_extensions |= set(NOTEBOOK_EXTENSIONS)
+
     allow_stdin = True
 
     def __init__(
         self,
         app: BaseApp,
-        path: UPath | None = None,
+        path: Path | None = None,
         kernel: Kernel | None = None,
         comms: dict[str, Comm] | None = None,
         use_kernel_history: bool = True,
         json: dict[str, Any] | None = None,
     ) -> None:
         """Load a editable notebook."""
         super().__init__(
@@ -98,50 +110,63 @@
 
         self.edit_mode = False
         self.in_edit_mode = Condition(self.check_edit_mode)
         self.multiple_cells_selected = multiple_cells_selected
         self.clipboard: list[Cell] = []
         self.undo_buffer: Deque[tuple[int, list[Cell]]] = deque(maxlen=10)
 
-        if not kernel:
-            self.kernel.start(cb=self.kernel_started, wait=False)
-
     # Tab stuff
 
     def _statusbar_kernel_handeler(self, event: MouseEvent) -> NotImplementedOrNone:
         """Event handler for kernel name field in statusbar."""
         if event.event_type == MouseEventType.MOUSE_UP:
             get_cmd("change-kernel").run()
             return None
         else:
             return NotImplemented
 
-    def statusbar_fields(
-        self,
-    ) -> tuple[Sequence[AnyFormattedText], Sequence[AnyFormattedText]]:
+    def __pt_status__(self) -> StatusBarFields | None:
         """Generate the formatted text for the statusbar."""
-        rendered = self.page.pre_rendered
-        return (
-            [
-                self.mode(),
-                f"Cell {self.page.selected_slice.start+1}",
-                f"Rendering… ({rendered:.0%})" if rendered < 1 else "",
-                "Saving…" if self.saving else "",
-            ],
-            [
-                lambda: cast(
-                    "StyleAndTextTuples",
-                    [("", self.kernel_display_name, self._statusbar_kernel_handeler)],
-                ),
-                KERNEL_STATUS_REPR[self.kernel.status] if self.kernel else ".",
-            ],
-        )
+        if self.loaded:
+            rendered = self.page.pre_rendered
+            return (
+                [
+                    self.mode(),
+                    f"Cell {self.page.selected_slice.start+1}",
+                    f"Rendering… ({rendered:.0%})" if rendered < 1 else "",
+                    "Saving…" if self.saving else "",
+                ],
+                [
+                    lambda: cast(
+                        "StyleAndTextTuples",
+                        [
+                            (
+                                "",
+                                self.kernel_display_name,
+                                self._statusbar_kernel_handeler,
+                            )
+                        ],
+                    ),
+                    KERNEL_STATUS_REPR[self.kernel.status] if self.kernel else ".",
+                ],
+            )
+        else:
+            return ([], [])
 
     # Notebook stuff
 
+    def post_init_kernel(self) -> None:
+        """Start the kernel after if has been loaded."""
+        # Start kernel
+        if self.kernel._status == "stopped":
+            self.kernel.start(cb=self.kernel_started, wait=False)
+
+        # Load container
+        super().post_init_kernel()
+
     @property
     def selected_indices(self) -> list[int]:
         """Return a list of the currently selected cell indices."""
         return self.page.selected_indices
 
     def kernel_started(self, result: dict[str, Any] | None = None) -> None:
         """Run when the kernel has started."""
@@ -215,15 +240,16 @@
                     MarginContainer(ScrollbarMargin(), target=self.page),
                     filter=Condition(lambda: self.app.config.show_scroll_bar),
                 ),
             ],
             width=Dimension(weight=1),
             height=Dimension(min=1, weight=2),
             key_bindings=load_registered_bindings(
-                "euporie.notebook.tabs.notebook.Notebook"
+                "euporie.core.tabs.base.Tab",
+                "euporie.notebook.tabs.notebook.Notebook",
             ),
         )
 
     @property
     def cell(self) -> Cell:
         """Return the currently selected `Cell` in this `Notebook`."""
         cell = self.page.get_child()
@@ -311,15 +337,15 @@
             slice_ = self.page._selected_slice
         # This triggers another redraw of the selected cell
         self.page._set_selected_slice(slice_, force=True, scroll=scroll)
         self.page.reset()
 
     def refresh_cell(self, cell: Cell) -> None:
         """Trigger the refresh of a notebook cell."""
-        self.page.get_child_render_info(cell.index).refresh = True
+        self.page.get_child_render_info(cell.index).invalidate()
 
     def add_cell_above(self) -> None:
         """Inert a cell above the current selection."""
         index = self.page.selected_slice.start + 0
         self.add(index)
         self.refresh(slice_=slice(index, index + 1), scroll=False)
 
@@ -566,24 +592,14 @@
         """,
     )
 
     # ################################### Commands ####################################
 
     @staticmethod
     @add_cmd(
-        filter=notebook_has_focus,
-    )
-    def _save_notebook() -> None:
-        """Save the current notebook."""
-        tab = get_app().tab
-        if isinstance(tab, Notebook):
-            tab.save()
-
-    @staticmethod
-    @add_cmd(
         filter=cell_has_focus & ~buffer_has_focus,
     )
     def _enter_cell_edit_mode() -> None:
         """Enter cell edit mode."""
         nb = get_app().tab
         if isinstance(nb, Notebook):
             nb.enter_edit_mode()
@@ -926,14 +942,19 @@
     )
     def _cells_to_markdown() -> None:
         """Change selected cells to markdown cells."""
         nb = get_app().tab
         if isinstance(nb, Notebook):
             for cell in nb.cells:
                 cell.set_cell_type("markdown", clear=True)
+                # Remove unallowed additional properties
+                json = cell.json
+                json.pop("execution_count", None)
+                json.pop("outputs", None)
+                cell.run_or_render()
 
     @staticmethod
     @add_cmd(
         filter=cell_has_focus & ~buffer_has_focus,
     )
     def _cells_to_code() -> None:
         """Change selected cells to code cells."""
@@ -989,15 +1010,15 @@
 
     @staticmethod
     @add_cmd(
         filter=cell_has_focus & ~buffer_has_focus,
         title="Collapse cell inputs",
     )
     def _hide_cell_inputs() -> None:
-        """Collape the selected cells' inputs."""
+        """Collapse the selected cells' inputs."""
         nb = get_app().tab
         if isinstance(nb, Notebook):
             for cell in nb.cells:
                 cell.hide_input()
 
     @staticmethod
     @add_cmd(
@@ -1024,15 +1045,15 @@
 
     @staticmethod
     @add_cmd(
         filter=cell_has_focus & ~buffer_has_focus,
         title="Collapse cell outputs",
     )
     def _hide_cell_outputs() -> None:
-        """Collape the selected cells' outputs."""
+        """Collapse the selected cells' outputs."""
         nb = get_app().tab
         if isinstance(nb, Notebook):
             for cell in nb.cells:
                 cell.hide_output()
 
     @staticmethod
     @add_cmd(
@@ -1183,15 +1204,14 @@
         get_cmd("toggle-line-numbers").run()
 
     # ################################# Key Bindings ##################################
 
     register_bindings(
         {
             "euporie.notebook.tabs.notebook.Notebook": {
-                "save-notebook": "c-s",
                 "enter-cell-edit-mode": "enter",
                 "exit-edit-mode": "escape",
                 "run-selected-cells": ["c-enter", "c-e"],
                 "run-and-select-next": ["s-enter", "c-r"],
                 "run-cell-and-insert-below": ("escape", "enter"),
                 "add-cell-above": "a",
                 "add-cell-below": "b",
@@ -1230,11 +1250,10 @@
                 "split-cell": "c-\\",
                 "edit-previous-cell": "up",
                 "edit-next-cell": "down",
                 "scroll-output-left": "left",
                 "scroll-output-right": "right",
                 "toggle-expand": "w",
                 "notebook-toggle-line-numbers": "l",
-                "reset-tab": "f5",
             }
         }
     )
```

### Comparing `euporie-2.3.2/euporie/notebook/widgets/side_bar.py` & `euporie-2.4.0/euporie/notebook/widgets/side_bar.py`

 * *Files identical despite different names*

### Comparing `euporie-2.3.2/euporie/preview/app.py` & `euporie-2.4.0/euporie/preview/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from euporie.core.app import BaseApp, get_app
 from euporie.core.config import add_setting
 from euporie.core.key_binding.registry import register_bindings
 from euporie.preview.tabs.notebook import PreviewNotebook
 
 if TYPE_CHECKING:
+    from pathlib import Path
     from typing import IO, Any, TextIO
 
     from prompt_toolkit.application.application import _AppResult
     from prompt_toolkit.layout.containers import Float
     from prompt_toolkit.output import Output
 
     from euporie.core.tabs.base import Tab
@@ -87,15 +88,15 @@
         # We want the app to close when rendering is complete
         # self.after_render += self.pre_exit
         # Do not load any key bindings
         self.bindings_to_load.append("euporie.preview.app.PreviewApp")
         # Select the first tab after files are opened
         self.post_load_callables.append(partial(setattr, self, "tab_idx", 0))
 
-    def get_file_tab(self, path: UPath) -> type[Tab]:
+    def get_file_tab(self, path: Path) -> type[Tab]:
         """Return the tab to use for a file path."""
         return PreviewNotebook
 
     def exit(
         self,
         result: _AppResult | None = None,
         exception: BaseException | type[BaseException] | None = None,
```

### Comparing `euporie-2.3.2/euporie/preview/tabs/notebook.py` & `euporie-2.4.0/euporie/preview/tabs/notebook.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,74 +17,87 @@
 
 from euporie.core.config import add_setting
 from euporie.core.tabs.notebook import BaseNotebook
 from euporie.core.widgets.cell import Cell
 from euporie.core.widgets.page import PrintingContainer
 
 if TYPE_CHECKING:
+    from pathlib import Path
     from typing import Any, Callable
 
     from prompt_toolkit.application.application import Application
     from prompt_toolkit.formatted_text.base import StyleAndTextTuples
     from prompt_toolkit.layout.containers import AnyContainer
-    from upath import UPath
 
     from euporie.core.app import BaseApp
 
 log = logging.getLogger(__name__)
 
 
 class PreviewNotebook(BaseNotebook):
     """A notebook tab which renders cells sequentially."""
 
+    bg_init = False
+
     def __init__(
         self,
         app: BaseApp,
-        path: UPath | None = None,
+        path: Path | None = None,
         use_kernel_history: bool = False,
     ) -> None:
         """Create a new instance."""
-        super().__init__(app, path, use_kernel_history=use_kernel_history)
         self.cell_index = 0
-        self.app.before_render += self.before_render
-        self.app.after_render += self.after_render
         self.cells: FastDictCache[tuple[int], Cell] = FastDictCache(
             get_value=self.get_cell
         )
 
-        # If we are running the notebook, pause rendering util the kernel has started
-        if self.app.config.run:
-            self.app.pause_rendering()
-            self.kernel.start(cb=self.kernel_started, wait=True)
+        super().__init__(app, path, use_kernel_history=use_kernel_history)
+
+        self.app.before_render += self.before_render
+        self.app.after_render += self.after_render
+
+    def pre_init_kernel(self) -> None:
+        """Filter cells before kernel is loaded."""
+        super().pre_init_kernel()
 
         # Filter the cells to be shown
         n_cells = len(self.json["cells"]) - 1
         start: int | None = None
         stop: int | None = None
         if self.app.config.cell_start is not None:
             start = min(max(self.app.config.cell_start, -n_cells), n_cells)
         if self.app.config.cell_stop is not None:
             stop = min(max(self.app.config.cell_stop, -n_cells), n_cells)
         log.debug("Showing cells %s to %s", start, stop)
         self.json["cells"] = self.json["cells"][start:stop]
 
+    def post_init_kernel(self) -> None:
+        """Optionally start kernel after it is loaded."""
+        super().post_init_kernel()
+        # If we are running the notebook, pause rendering util the kernel has started
+        if self.app.config.run:
+            self.app.pause_rendering()
+            self.kernel.start(cb=self.kernel_started, wait=True)
+
     def print_title(self) -> None:
         """Print a notebook's filename."""
+        from euporie.core.border import DoubleLine
         from euporie.core.formatted_text.utils import (
             FormattedTextAlign,
             add_border,
             align,
             wrap,
         )
 
         width = self.app.output.get_size().columns
         ft: StyleAndTextTuples = [("bold", str(self.path))]
         ft = wrap(ft, width - 4)
         ft = align(ft, how=FormattedTextAlign.CENTER, width=width - 4)
-        ft = add_border(ft, width=width)
+        ft = add_border(ft, width=width, border_grid=DoubleLine.grid)
+        ft.append(("", "\n"))
         self.app.print_text(ft)
 
     def kernel_started(self, result: dict | None = None) -> None:
         """Resume rendering the app when the kernel has started."""
         self.app.resume_rendering()
 
     def close(self, cb: Callable | None = None) -> None:
```

### Comparing `euporie-2.3.2/.gitignore` & `euporie-2.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `euporie-2.3.2/LICENSE` & `euporie-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `euporie-2.3.2/README.rst` & `euporie-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `euporie-2.3.2/pyproject.toml` & `euporie-2.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -30,40 +30,33 @@
   "prompt-toolkit~=3.0.36",
   "Pygments~=2.11",
   "nbformat~=5.0",
   "jupyter_client~=7.1",
   "aenum~=3.1",
   "typing-extensions~=4.2",
   "fastjsonschema~=2.15",
-  "appdirs~=1.4",
+  "platformdirs~=3.5",
   "pyperclip~=1.8",
   "imagesize~=1.3",
   "markdown-it-py~=2.1.0",
   "linkify-it-py~=1.0",
   "mdit-py-plugins~=0.3.0",
   "flatlatex~=0.15",
   "timg~=1.1",
   "Pillow~=9.0",
   "sixelcrop~=0.1.3",
-  "universal-pathlib~=0.0.19",
+  "universal-pathlib~=0.0.23",
   "fsspec[http]>=2022.8.0",
 ]
 
 [project.optional-dependencies]
-hub = [
-  "asyncssh~=2.10.1",
-]
-format = [
-  "black>=19.3.b0",
-  "isort~=5.10.1",
-  "ssort~=0.11.6",
-]
-chafa = [
-  "chafa.py>=1.0.2",
-]
+hub = ["asyncssh~=2.10.1"]
+format = ["black>=19.3.b0", "isort~=5.10.1"]
+chafa = ["chafa.py>=1.0.2"]
+jupytext = ["jupytext>=1.14.0"]
 
 [project.urls]
 Documentation = "https://euporie.readthedocs.io/en/latest"
 Issues = "https://github.com/joouha/euporie/issues"
 Source = "https://github.com/joouha/euporie"
 Changelog = "https://euporie.readthedocs.io/en/latest/pages/changelog.html"
 
@@ -83,14 +76,16 @@
 
 [project.entry-points."pygments.lexers"]
 argparse = 'euporie.core.pygments:ArgparseLexer'
 
 [project.entry-points."pygments.styles"]
 euporie = 'euporie.core.pygments:EuporiePygmentsStyle'
 
+[tool.hatch.build.targets.wheel.shared-data]
+"euporie/data/desktop" = "share/applications/"
 
 [tool.hatch.version]
 path = "euporie/core/__init__.py"
 
 [tool.hatch.build]
 packages = ["euporie"]
 
@@ -108,32 +103,29 @@
 
 [tool.hatch.envs.check]
 description = "Check and lint the codebase."
 detached = true
 dependencies = [
   "pre-commit",
   "pre-commit-hooks",
-  "ssort",
   "black",
   "ruff",
   "codespell", "tomli",
 ]
 
 [tool.hatch.envs.check.scripts]
 check = [
-    "ssort --check {args:euporie tests scripts}",
     "black --check {args:euporie tests scripts}",
-    "codespell {args:euporie tests scripts}",
     "ruff {args:euporie tests scripts}",
+    "codespell {args:euporie tests scripts docs/pages}",
 ]
 fix = [
-    "ssort {args:euporie tests scripts}",
     "black {args:euporie tests scripts}",
-    "codespell {args:-- euporie tests scripts}",
     "ruff --fix {args:euporie tests scripts}",
+    "codespell -i 3 -w {args:euporie tests scripts docs/pages}",
 ]
 
 [tool.hatch.envs.type]
 description = "Type check the codebase."
 dependencies = [
   "mypy",
   # Dependencies
@@ -147,17 +139,17 @@
 [tool.hatch.envs.type.scripts]
 run = "mypy {args:--namespace-packages -p euporie -p tests -p scripts}"
 
 [tool.hatch.envs.test]
 description = "Run tests."
 detached = false
 dependencies = [
-  "pytest",
+  "pytest", "pytest-cov", "coverage",
   # Optional non-dependencies
-  "html2text"
+  "python-magic", "html2text",
 ]
 [[tool.hatch.envs.test.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "pypy3"]
 
 [tool.hatch.envs.test.scripts]
 run = "pytest {args}"
 cov = "coverage run --parallel -m pytest {args}"
@@ -194,14 +186,16 @@
     "E501",
     # Google style docstrings
     "D203", "D204", "D213", "D215", "D400", "D404", "D406", "D407", "D408", "D409", "D413",
     # Allow empty functions in ABCs
     "B027",
     # zip() without an explicit strict= parameter
     "B905",
+    # Ignore subprocess warnings
+    "S603", "S607"
 ]
 
 [tool.ruff.per-file-ignores]
 "scripts/*.py" = ["T201"]
 
 [tool.codespell]
 ignore-words-list = "iterm,edn,controll,controle"
@@ -212,11 +206,14 @@
 # pretty = true
 show_error_codes = true
 
 [[tool.mypy.overrides]]
 module = [
   "_frozen_importlib", "ipykernel", "fastjsonschema",
   "pyperclip", "upath.*", "chafa.*", "timg", "pylatexenc.*", "aenum", "pygments.*",
+  "jupytext.*",
   "ssort",
-  "flatlatex.*", "timg", "img2unicode", "cairosvg", "teimpy", "numpy", "mtable", "imagesize", "matplotlib.*"
+  "flatlatex.*", "timg", "img2unicode", "cairosvg", "teimpy", "numpy", "mtable", "imagesize", "matplotlib.*",
+  "magic", "fsspec.*",
+  "pytest.*",
 ]
 ignore_missing_imports = true
```

### Comparing `euporie-2.3.2/PKG-INFO` & `euporie-2.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: euporie
-Version: 2.3.2
+Version: 2.4.0
 Summary: Euporie is a suite of terminal applications for interacting with Jupyter kernels
 Project-URL: Documentation, https://euporie.readthedocs.io/en/latest
 Project-URL: Issues, https://github.com/joouha/euporie/issues
 Project-URL: Source, https://github.com/joouha/euporie
 Project-URL: Changelog, https://euporie.readthedocs.io/en/latest/pages/changelog.html
 Author-email: Josiah Outram Halstead <josiah@halstead.email>
 License-File: LICENSE
@@ -18,40 +18,41 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Requires-Dist: aenum~=3.1
-Requires-Dist: appdirs~=1.4
 Requires-Dist: fastjsonschema~=2.15
 Requires-Dist: flatlatex~=0.15
 Requires-Dist: fsspec[http]>=2022.8.0
 Requires-Dist: imagesize~=1.3
 Requires-Dist: jupyter-client~=7.1
 Requires-Dist: linkify-it-py~=1.0
 Requires-Dist: markdown-it-py~=2.1.0
 Requires-Dist: mdit-py-plugins~=0.3.0
 Requires-Dist: nbformat~=5.0
 Requires-Dist: pillow~=9.0
+Requires-Dist: platformdirs~=3.5
 Requires-Dist: prompt-toolkit~=3.0.36
 Requires-Dist: pygments~=2.11
 Requires-Dist: pyperclip~=1.8
 Requires-Dist: sixelcrop~=0.1.3
 Requires-Dist: timg~=1.1
 Requires-Dist: typing-extensions~=4.2
-Requires-Dist: universal-pathlib~=0.0.19
+Requires-Dist: universal-pathlib~=0.0.23
 Provides-Extra: chafa
 Requires-Dist: chafa-py>=1.0.2; extra == 'chafa'
 Provides-Extra: format
 Requires-Dist: black>=19.3.b0; extra == 'format'
 Requires-Dist: isort~=5.10.1; extra == 'format'
-Requires-Dist: ssort~=0.11.6; extra == 'format'
 Provides-Extra: hub
 Requires-Dist: asyncssh~=2.10.1; extra == 'hub'
+Provides-Extra: jupytext
+Requires-Dist: jupytext>=1.14.0; extra == 'jupytext'
 Description-Content-Type: text/x-rst
 
 |logo|
 
 .. |logo| image:: https://user-images.githubusercontent.com/12154190/160670889-c6fc4cd8-413d-49f0-b105-9c0e03117032.svg
    :alt: <Logo>
```

