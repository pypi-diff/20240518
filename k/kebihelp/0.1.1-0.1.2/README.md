# Comparing `tmp/kebihelp-0.1.1.tar.gz` & `tmp/kebihelp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kebihelp-0.1.1.tar", last modified: Fri May 17 10:31:14 2024, max compression
+gzip compressed data, was "kebihelp-0.1.2.tar", last modified: Sat May 18 10:43:11 2024, max compression
```

## Comparing `kebihelp-0.1.1.tar` & `kebihelp-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-17 10:31:14.827013 kebihelp-0.1.1/
--rw-r--r--   0 ju        (1000) ju        (1000)     1067 2024-05-05 11:11:30.000000 kebihelp-0.1.1/LICENSE
--rw-r--r--   0 ju        (1000) ju        (1000)     6552 2024-05-17 10:31:14.827013 kebihelp-0.1.1/PKG-INFO
--rw-r--r--   0 ju        (1000) ju        (1000)     5688 2024-05-17 10:30:40.000000 kebihelp-0.1.1/README.md
--rw-r--r--   0 ju        (1000) ju        (1000)      954 2024-05-17 10:24:15.000000 kebihelp-0.1.1/pyproject.toml
--rw-r--r--   0 ju        (1000) ju        (1000)       38 2024-05-17 10:31:14.830346 kebihelp-0.1.1/setup.cfg
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-17 10:31:14.827013 kebihelp-0.1.1/src/
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-17 10:31:14.827013 kebihelp-0.1.1/src/kebihelp/
--rw-r--r--   0 ju        (1000) ju        (1000)        0 2024-05-05 11:11:30.000000 kebihelp-0.1.1/src/kebihelp/__init__.py
--rw-r--r--   0 ju        (1000) ju        (1000)     4629 2024-05-15 16:44:52.000000 kebihelp-0.1.1/src/kebihelp/config.py
--rw-r--r--   0 ju        (1000) ju        (1000)    10346 2024-05-15 20:08:58.000000 kebihelp-0.1.1/src/kebihelp/gui.py
--rwxr-xr-x   0 ju        (1000) ju        (1000)     1942 2024-05-17 10:24:25.000000 kebihelp-0.1.1/src/kebihelp/main.py
--rw-r--r--   0 ju        (1000) ju        (1000)     2673 2024-05-15 16:41:45.000000 kebihelp-0.1.1/src/kebihelp/parsers.py
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-17 10:31:14.827013 kebihelp-0.1.1/src/kebihelp.egg-info/
--rw-r--r--   0 ju        (1000) ju        (1000)     6552 2024-05-17 10:31:14.000000 kebihelp-0.1.1/src/kebihelp.egg-info/PKG-INFO
--rw-r--r--   0 ju        (1000) ju        (1000)      363 2024-05-17 10:31:14.000000 kebihelp-0.1.1/src/kebihelp.egg-info/SOURCES.txt
--rw-r--r--   0 ju        (1000) ju        (1000)        1 2024-05-17 10:31:14.000000 kebihelp-0.1.1/src/kebihelp.egg-info/dependency_links.txt
--rw-r--r--   0 ju        (1000) ju        (1000)       48 2024-05-17 10:31:14.000000 kebihelp-0.1.1/src/kebihelp.egg-info/entry_points.txt
--rw-r--r--   0 ju        (1000) ju        (1000)       54 2024-05-17 10:31:14.000000 kebihelp-0.1.1/src/kebihelp.egg-info/requires.txt
--rw-r--r--   0 ju        (1000) ju        (1000)        9 2024-05-17 10:31:14.000000 kebihelp-0.1.1/src/kebihelp.egg-info/top_level.txt
+drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-18 10:43:11.070935 kebihelp-0.1.2/
+-rw-r--r--   0 ju        (1000) ju        (1000)     1067 2024-05-05 11:11:30.000000 kebihelp-0.1.2/LICENSE
+-rw-r--r--   0 ju        (1000) ju        (1000)     7359 2024-05-18 10:43:11.070935 kebihelp-0.1.2/PKG-INFO
+-rw-r--r--   0 ju        (1000) ju        (1000)     6495 2024-05-18 10:36:02.000000 kebihelp-0.1.2/README.md
+-rw-r--r--   0 ju        (1000) ju        (1000)      954 2024-05-18 10:41:02.000000 kebihelp-0.1.2/pyproject.toml
+-rw-r--r--   0 ju        (1000) ju        (1000)       38 2024-05-18 10:43:11.070935 kebihelp-0.1.2/setup.cfg
+drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-18 10:43:11.070935 kebihelp-0.1.2/src/
+drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-18 10:43:11.070935 kebihelp-0.1.2/src/kebihelp/
+-rw-r--r--   0 ju        (1000) ju        (1000)        0 2024-05-05 11:11:30.000000 kebihelp-0.1.2/src/kebihelp/__init__.py
+-rw-r--r--   0 ju        (1000) ju        (1000)     4877 2024-05-18 10:26:01.000000 kebihelp-0.1.2/src/kebihelp/config.py
+-rw-r--r--   0 ju        (1000) ju        (1000)    12295 2024-05-18 10:39:37.000000 kebihelp-0.1.2/src/kebihelp/gui.py
+-rwxr-xr-x   0 ju        (1000) ju        (1000)     1942 2024-05-18 10:41:14.000000 kebihelp-0.1.2/src/kebihelp/main.py
+-rw-r--r--   0 ju        (1000) ju        (1000)     2673 2024-05-15 16:41:45.000000 kebihelp-0.1.2/src/kebihelp/parsers.py
+drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-18 10:43:11.070935 kebihelp-0.1.2/src/kebihelp.egg-info/
+-rw-r--r--   0 ju        (1000) ju        (1000)     7359 2024-05-18 10:43:11.000000 kebihelp-0.1.2/src/kebihelp.egg-info/PKG-INFO
+-rw-r--r--   0 ju        (1000) ju        (1000)      363 2024-05-18 10:43:11.000000 kebihelp-0.1.2/src/kebihelp.egg-info/SOURCES.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)        1 2024-05-18 10:43:11.000000 kebihelp-0.1.2/src/kebihelp.egg-info/dependency_links.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)       48 2024-05-18 10:43:11.000000 kebihelp-0.1.2/src/kebihelp.egg-info/entry_points.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)       54 2024-05-18 10:43:11.000000 kebihelp-0.1.2/src/kebihelp.egg-info/requires.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)        9 2024-05-18 10:43:11.000000 kebihelp-0.1.2/src/kebihelp.egg-info/top_level.txt
```

### Comparing `kebihelp-0.1.1/LICENSE` & `kebihelp-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kebihelp-0.1.1/PKG-INFO` & `kebihelp-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kebihelp
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Linux universal keybindings helper written in Python/QT5
 Author-email: Julien Pro <contact@julienpro.com>
 Project-URL: Homepage, https://github.com/juienpro/kebihelp
 Project-URL: Issues, https://github.com/juienpro/kebihelp/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -179,13 +179,52 @@
 
 - Font name and size of any part
 - Colors 
 
 To do that, edit the `kebihelp.json` config file.
 
 
+### Size of the window
+
+The Window layout has a fixed size. You can change it in the config file:
+
+```
+"layout" {
+  "width": 900,
+  "height": 900
+}
+```
+
+These parameters are important: depending of the size of the Window and the number of keybindings, it will enable (or not) the scrollbars.
+
+### Remap default keys
+
+By default, the following keys are configured: 
+
+| Key | Function |
+|-----|----------|
+| Tab | Go to next tab |
+| Shift+Tab | Go to previous tab |
+| Down | Scroll down |
+| Up | Scroll up |
+| Esc | Quit |
+
+You can remap these keys in the config file.
+
+To set-up VIM style keybindings, configure the section `keys` in the `Parameters` of the `kebihelp.json` config file:
+
+```
+"keys": {
+  "tab_previous": "h", 
+  "tab_next": "l",
+  "scroll_down": "j",
+  "scroll_up": "k",
+  "quit": "q"
+}
+```
+
 ## Feedbacks
 
 This tool is not perfect, but it may be useful to build your own "keybinding helper" if your Desktop Environment does not support this feature.
 Your contributions are welcomed!
 
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/juienpro)
```

### Comparing `kebihelp-0.1.1/README.md` & `kebihelp-0.1.2/src/kebihelp.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: kebihelp
+Version: 0.1.2
+Summary: A Linux universal keybindings helper written in Python/QT5
+Author-email: Julien Pro <contact@julienpro.com>
+Project-URL: Homepage, https://github.com/juienpro/kebihelp
+Project-URL: Issues, https://github.com/juienpro/kebihelp/issues
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Topic :: System :: Operating System
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: Desktop Environment
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: prettytable>=3.10.0
+Requires-Dist: PyQt5>=5.15.10
+Requires-Dist: PyQt5_sip>=12.13.0
+
 # Kebihelp - The Universal Linux Key Bindings Helper
 
 Kebihelp is an universal key-bindings helper for Linux, written in Python and initially inspired by AwesomeWM and its "Mod4+s" feature.
 
 ![](docs/kebihelp.gif)
 
 Click on the picture to zoom.
@@ -157,13 +179,52 @@
 
 - Font name and size of any part
 - Colors 
 
 To do that, edit the `kebihelp.json` config file.
 
 
+### Size of the window
+
+The Window layout has a fixed size. You can change it in the config file:
+
+```
+"layout" {
+  "width": 900,
+  "height": 900
+}
+```
+
+These parameters are important: depending of the size of the Window and the number of keybindings, it will enable (or not) the scrollbars.
+
+### Remap default keys
+
+By default, the following keys are configured: 
+
+| Key | Function |
+|-----|----------|
+| Tab | Go to next tab |
+| Shift+Tab | Go to previous tab |
+| Down | Scroll down |
+| Up | Scroll up |
+| Esc | Quit |
+
+You can remap these keys in the config file.
+
+To set-up VIM style keybindings, configure the section `keys` in the `Parameters` of the `kebihelp.json` config file:
+
+```
+"keys": {
+  "tab_previous": "h", 
+  "tab_next": "l",
+  "scroll_down": "j",
+  "scroll_up": "k",
+  "quit": "q"
+}
+```
+
 ## Feedbacks
 
 This tool is not perfect, but it may be useful to build your own "keybinding helper" if your Desktop Environment does not support this feature.
 Your contributions are welcomed!
 
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/juienpro)
```

### Comparing `kebihelp-0.1.1/pyproject.toml` & `kebihelp-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kebihelp"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name="Julien Pro", email="contact@julienpro.com"}
 ]
 description = "A Linux universal keybindings helper written in Python/QT5"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
```

### Comparing `kebihelp-0.1.1/src/kebihelp/config.py` & `kebihelp-0.1.2/src/kebihelp/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,21 @@
                 'cmd_focused_window': "hyprctl activewindow",
                 "importer": {
                       "match_line": ".*::(.+?)::(.+?)::(.+?)::.*",
                       "position_group": 1,
                       "position_keybinding": 2,
                       "position_label": 3
                 },
+                "keys": {
+                    "tab_previous": "Backtab", 
+                    "tab_next": "Tab",
+                    "scroll_down": "Down",
+                    "scroll_up": "Up",
+                    "quit": "Esc"
+                },
                 "layout": {
                     'n_columns': 3,
                     'spacing': 3,
                     'background_color': '#282C34',
                     "opacity": 0.95,
                     "tabs": {
                         "background_color": "#30343D",
```

### Comparing `kebihelp-0.1.1/src/kebihelp/gui.py` & `kebihelp-0.1.2/src/kebihelp/gui.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,48 @@
 
-from PyQt5.QtWidgets import QApplication, QMainWindow, QPushButton, QWidget, QFrame, QLabel, QVBoxLayout, QHBoxLayout, QGridLayout, QScrollArea, QStyle, QLayout, QSizePolicy, QStackedWidget
+from PyQt5.QtWidgets import QApplication, QMainWindow, QPushButton, QWidget, QFrame,  QLabel, QVBoxLayout, QHBoxLayout, QGridLayout, QScrollArea, QStyle, QLayout, QSizePolicy, QStackedWidget
 from PyQt5.QtCore import QSize, Qt
-from PyQt5.QtGui import QFont
+from PyQt5.QtGui import QFont, QKeySequence
 from kebihelp.config import Config
 import subprocess
 from functools import partial
 import sys
 
 class MainWindow(QMainWindow):
     def __init__(self, selected_tab, autodetect):
         super().__init__()
         self.selected_tab = selected_tab
         self.autodetect = autodetect
         self.current_tab_name = None
         self.config = Config()
-
+        
+        self.keymap = self.load_keymap()
         self.keybindings = self.config.config['Keybindings']
         self.set_current_tab()
 
         self.layout = self.config.config['Parameters']['layout']
         # self.all_groups = self.config.get_all_groups()
         self.tab_buttons = []
         self.set_main_window()
         self.set_tabs()
         self.change_tab_by_name(self.current_tab_name)
     
+    def load_keymap(self):
+        default = {
+            'tab_previous': 'Backtab',
+            'tab_next': 'Tab',
+            'scroll_down': 'Down',
+            'scroll_up': 'Up',
+            'quit': 'Esc',
+        }
+        if 'keys' in self.config.config['Parameters']:
+            return self.config.config['Parameters']['keys']
+        else:
+            return default
+
     def set_current_tab(self):
         if self.selected_tab != None:
             if self.selected_tab not in self.keybindings:
                 print("The tab {} does not exist".format(self.selected_tab))
                 sys.exit(1)
             self.current_tab_name = self.selected_tab
 
@@ -57,40 +71,48 @@
         self.setWindowTitle("Kebihelp")
         self.setFont(QFont('Lato'))
         self.setStyleSheet("background-color: {}".format(self.layout['background_color']))
 
         self.setWindowOpacity(self.layout['opacity'])
 
         self.setWindowFlags(Qt.FramelessWindowHint | Qt.WindowStaysOnTopHint)
-
         self.main_widget = QWidget(self)
+
         self.window_layout = QVBoxLayout()
         self.tabs_layout = QHBoxLayout()
         self.stacked_widget = QStackedWidget()
 
         for tab_name, tab_config in self.keybindings.items():
             if '_hidden' in tab_config and tab_config['_hidden'] == True:
                 continue
             # if self.current_tab_name != tab_name:
             #     continue
             widget = self.get_tab_shortcuts(tab_name)
             self.stacked_widget.addWidget(widget)
 
-        # for tab in self.all_groups:
-        #     if self.config.config['Tabs'][tab]['visible'] == False:
-        #         if self.current_tab_name != tab:
-        #             continue
-        #     widget = self.get_tab_shortcuts(tab)
-        #     self.stacked_widget.addWidget(widget)
-
         self.window_layout.addLayout(self.tabs_layout)
         self.window_layout.addWidget(self.stacked_widget)
+        # self.window_layout.setSizeConstraint(QVBoxLayout.SetMinimumSize)
         self.window_layout.addStretch()
         self.main_widget.setLayout(self.window_layout)
-        self.setCentralWidget(self.main_widget)
+        # self.setCentralWidget(self.main_widget)
+        self.scroll_area = QScrollArea()
+        self.scroll_area.setWidget(self.main_widget)
+        self.scroll_area.setFocusPolicy(Qt.NoFocus)
+        self.scroll_area.setWidgetResizable(True)
+        self.scroll_area.setStyleSheet("QScrollBar {width:  0px;}")
+        self.setCentralWidget(self.scroll_area)
+
+        width = 900
+        if 'width' in self.layout:
+            width = self.layout['width']
+        height = 900
+        if 'height' in self.layout:
+            height = self.layout['height']
+        self.setFixedSize(width, height)
 
     def set_tabs(self):
         index = 0
         for tab_name, tab_config in self.keybindings.items():
             if '_hidden' in tab_config and tab_config['_hidden'] == True:
                 continue
             # if self.current_tab_name != tab_name:
@@ -231,22 +253,43 @@
         hbox.addStretch()
         hbox.addWidget(value)
         # hbox.setSpacing(self.layout['shortcut']['spacing'])
         # hbox.setContentsMargins(0, 0, 0, 0)
         return hbox
 
     def keyPressEvent(self, event):
-        if event.key() == Qt.Key_Escape:
+        # if event.key() == Qt.Key_Escape:
+        #     self.close()
+        # if event.key() == Qt.Key_Q:
+        #     self.close()
+        if event.key() == QKeySequence(self.keymap['quit']):
             self.close()
-        if event.key() == Qt.Key_Q:
-            self.close()
-        if event.key() == Qt.Key_Tab:
+
+        if event.key() == QKeySequence(self.keymap['tab_next']):
             current_index = self.stacked_widget.currentIndex()
             n_widgets = self.stacked_widget.count()
             if (current_index == n_widgets - 1):
                 new_index = 0
             else:
                 new_index = current_index + 1
             self.tab_buttons[new_index].setChecked(True)
             self.change_tab(new_index)
 
+        if event.key() == QKeySequence(self.keymap['tab_previous']):
+            current_index = self.stacked_widget.currentIndex()
+            n_widgets = self.stacked_widget.count()
+            if current_index == 0:
+                new_index = n_widgets - 1
+            else:
+                new_index = current_index - 1
+            self.tab_buttons[new_index].setChecked(True)
+            self.change_tab(new_index)
+
+        if event.key() == QKeySequence(self.keymap['scroll_down']):
+            if self.scroll_area.verticalScrollBar().value() < self.scroll_area.verticalScrollBar().maximum():
+                self.scroll_area.verticalScrollBar().setValue(self.scroll_area.verticalScrollBar().value() + self.scroll_area.verticalScrollBar().singleStep())
+
+        if event.key() == QKeySequence(self.keymap['scroll_up']):
+            if self.scroll_area.verticalScrollBar().value() > 0:
+                self.scroll_area.verticalScrollBar().setValue(self.scroll_area.verticalScrollBar().value() - self.scroll_area.verticalScrollBar().singleStep())
+
```

### Comparing `kebihelp-0.1.1/src/kebihelp/main.py` & `kebihelp-0.1.2/src/kebihelp/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from PyQt5.QtWidgets import QApplication
 import sys
 import argparse
 from kebihelp.parsers import Parsers
 from kebihelp.config import Config
 from kebihelp.gui import MainWindow
 
-VERSION="0.1.1"
+VERSION="0.1.2"
 
 def main():
     parser = argparse.ArgumentParser(description="Kebihelp - The universal keybinder helper")
 
     parser.add_argument("-v", "--version", dest="version", action="store_true", help="Show the current version")
     subparsers = parser.add_subparsers(dest="command", help="Main action to perform")
```

### Comparing `kebihelp-0.1.1/src/kebihelp/parsers.py` & `kebihelp-0.1.2/src/kebihelp/parsers.py`

 * *Files identical despite different names*

### Comparing `kebihelp-0.1.1/src/kebihelp.egg-info/PKG-INFO` & `kebihelp-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: kebihelp
-Version: 0.1.1
-Summary: A Linux universal keybindings helper written in Python/QT5
-Author-email: Julien Pro <contact@julienpro.com>
-Project-URL: Homepage, https://github.com/juienpro/kebihelp
-Project-URL: Issues, https://github.com/juienpro/kebihelp/issues
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Topic :: System :: Operating System
-Classifier: Topic :: System :: Systems Administration
-Classifier: Topic :: Desktop Environment
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: prettytable>=3.10.0
-Requires-Dist: PyQt5>=5.15.10
-Requires-Dist: PyQt5_sip>=12.13.0
-
 # Kebihelp - The Universal Linux Key Bindings Helper
 
 Kebihelp is an universal key-bindings helper for Linux, written in Python and initially inspired by AwesomeWM and its "Mod4+s" feature.
 
 ![](docs/kebihelp.gif)
 
 Click on the picture to zoom.
@@ -179,13 +157,52 @@
 
 - Font name and size of any part
 - Colors 
 
 To do that, edit the `kebihelp.json` config file.
 
 
+### Size of the window
+
+The Window layout has a fixed size. You can change it in the config file:
+
+```
+"layout" {
+  "width": 900,
+  "height": 900
+}
+```
+
+These parameters are important: depending of the size of the Window and the number of keybindings, it will enable (or not) the scrollbars.
+
+### Remap default keys
+
+By default, the following keys are configured: 
+
+| Key | Function |
+|-----|----------|
+| Tab | Go to next tab |
+| Shift+Tab | Go to previous tab |
+| Down | Scroll down |
+| Up | Scroll up |
+| Esc | Quit |
+
+You can remap these keys in the config file.
+
+To set-up VIM style keybindings, configure the section `keys` in the `Parameters` of the `kebihelp.json` config file:
+
+```
+"keys": {
+  "tab_previous": "h", 
+  "tab_next": "l",
+  "scroll_down": "j",
+  "scroll_up": "k",
+  "quit": "q"
+}
+```
+
 ## Feedbacks
 
 This tool is not perfect, but it may be useful to build your own "keybinding helper" if your Desktop Environment does not support this feature.
 Your contributions are welcomed!
 
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/juienpro)
```

