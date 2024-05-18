# Comparing `tmp/QEasyWidgets-0.1.8.tar.gz` & `tmp/QEasyWidgets-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QEasyWidgets-0.1.8.tar", last modified: Tue May 14 15:27:43 2024, max compression
+gzip compressed data, was "QEasyWidgets-0.1.9.tar", last modified: Sat May 18 01:46:20 2024, max compression
```

## Comparing `QEasyWidgets-0.1.8.tar` & `QEasyWidgets-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 15:27:43.103299 QEasyWidgets-0.1.8/
--rw-rw-rw-   0        0        0    35823 2023-12-07 09:28:12.000000 QEasyWidgets-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       82 2024-04-05 05:40:54.000000 QEasyWidgets-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1759 2024-05-14 15:27:43.103299 QEasyWidgets-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-14 15:27:43.100190 QEasyWidgets-0.1.8/QEasyWidgets/
--rw-rw-rw-   0        0        0    23435 2024-05-14 14:01:25.000000 QEasyWidgets-0.1.8/QEasyWidgets/ComponentsCustomizer.py
--rw-rw-rw-   0        0        0    15667 2024-05-14 09:59:56.000000 QEasyWidgets-0.1.8/QEasyWidgets/QFunctions.py
--rw-rw-rw-   0        0        0     4305 2024-04-01 00:18:06.000000 QEasyWidgets-0.1.8/QEasyWidgets/QTasks.py
--rw-rw-rw-   0        0        0    70976 2024-05-08 10:24:53.000000 QEasyWidgets-0.1.8/QEasyWidgets/Sources.py
--rw-rw-rw-   0        0        0    29197 2024-05-08 03:09:46.000000 QEasyWidgets-0.1.8/QEasyWidgets/Utils.py
--rw-rw-rw-   0        0        0    22606 2024-05-08 02:30:45.000000 QEasyWidgets-0.1.8/QEasyWidgets/WindowCustomizer.py
--rw-rw-rw-   0        0        0       22 2024-04-01 00:18:06.000000 QEasyWidgets-0.1.8/QEasyWidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 15:27:43.103299 QEasyWidgets-0.1.8/QEasyWidgets.egg-info/
--rw-rw-rw-   0        0        0     1759 2024-05-14 15:27:43.000000 QEasyWidgets-0.1.8/QEasyWidgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2024-05-14 15:27:43.000000 QEasyWidgets-0.1.8/QEasyWidgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 15:27:43.000000 QEasyWidgets-0.1.8/QEasyWidgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-05-14 15:27:43.000000 QEasyWidgets-0.1.8/QEasyWidgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-14 15:27:43.000000 QEasyWidgets-0.1.8/QEasyWidgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1135 2024-04-01 15:15:08.000000 QEasyWidgets-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2024-05-14 15:27:43.103299 QEasyWidgets-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1570 2024-05-14 10:04:20.000000 QEasyWidgets-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 01:46:20.487784 QEasyWidgets-0.1.9/
+-rw-rw-rw-   0        0        0    35823 2023-12-07 09:28:12.000000 QEasyWidgets-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       82 2024-04-05 05:40:54.000000 QEasyWidgets-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1908 2024-05-18 01:46:20.487784 QEasyWidgets-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-18 01:46:20.483498 QEasyWidgets-0.1.9/QEasyWidgets/
+-rw-rw-rw-   0        0        0    23460 2024-05-18 01:45:51.000000 QEasyWidgets-0.1.9/QEasyWidgets/ComponentsCustomizer.py
+-rw-rw-rw-   0        0        0    15667 2024-05-18 01:45:53.000000 QEasyWidgets-0.1.9/QEasyWidgets/QFunctions.py
+-rw-rw-rw-   0        0        0     4305 2024-04-01 00:18:06.000000 QEasyWidgets-0.1.9/QEasyWidgets/QTasks.py
+-rw-rw-rw-   0        0        0    70976 2024-05-08 10:24:53.000000 QEasyWidgets-0.1.9/QEasyWidgets/Sources.py
+-rw-rw-rw-   0        0        0    29202 2024-05-17 06:15:06.000000 QEasyWidgets-0.1.9/QEasyWidgets/Utils.py
+-rw-rw-rw-   0        0        0    22606 2024-05-08 02:30:45.000000 QEasyWidgets-0.1.9/QEasyWidgets/WindowCustomizer.py
+-rw-rw-rw-   0        0        0       22 2024-04-01 00:18:06.000000 QEasyWidgets-0.1.9/QEasyWidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 01:46:20.486325 QEasyWidgets-0.1.9/QEasyWidgets.egg-info/
+-rw-rw-rw-   0        0        0     1908 2024-05-18 01:46:20.000000 QEasyWidgets-0.1.9/QEasyWidgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2024-05-18 01:46:20.000000 QEasyWidgets-0.1.9/QEasyWidgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 01:46:20.000000 QEasyWidgets-0.1.9/QEasyWidgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-18 01:46:20.000000 QEasyWidgets-0.1.9/QEasyWidgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-18 01:46:20.000000 QEasyWidgets-0.1.9/QEasyWidgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1135 2024-04-01 15:15:08.000000 QEasyWidgets-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-18 01:46:20.488784 QEasyWidgets-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1570 2024-05-14 15:33:05.000000 QEasyWidgets-0.1.9/setup.py
```

### Comparing `QEasyWidgets-0.1.8/LICENSE` & `QEasyWidgets-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.8/PKG-INFO` & `QEasyWidgets-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 2.1
 Name: QEasyWidgets
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple widget library based on PySide6
 Home-page: https://github.com/Spr-Aachen/QEasyWidgets
 Author: Spr_Aachen
 Author-email: 2835946988@qq.com
 License: GPLv3
 Project-URL: Source Code, https://github.com/Spr-Aachen/QEasyWidgets
 Project-URL: Bug Tracker, https://github.com/Spr-Aachen/QEasyWidgets/issues
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PySide6
+Requires-Dist: darkdetect
+Requires-Dist: tqdm
+Requires-Dist: psutil
+Requires-Dist: nvidia-ml-py
+Requires-Dist: PyGithub
 
 <div align = "center">
 
 # QEasyWidgets
 
 [![Releases](https://img.shields.io/github/v/release/Spr-Aachen/QEasyWidgets?color=green&label=Release&logo=Github&logoColor=white&style=for-the-badge)](https://github.com/Spr-Aachen/QEasyWidgets/releases/latest)&nbsp;
```

### Comparing `QEasyWidgets-0.1.8/QEasyWidgets/ComponentsCustomizer.py` & `QEasyWidgets-0.1.9/QEasyWidgets/ComponentsCustomizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -473,27 +473,31 @@
     '''
     textChanged = Signal(str)
     cursorPositionChanged = Signal(int, int)
 
     focusedIn = Signal()
     focusedOut = Signal()
 
+    interacted = Signal()
+
     rectChanged = Signal(QRect)
 
     def __init__(self, parent: QWidget = None):
         super().__init__(parent)
 
         self.LineEdit = LineEdit()
         self.LineEdit.textChanged.connect(self.textChanged.emit)
+        self.LineEdit.textChanged.connect(lambda: self.interacted.emit())
         #self.LineEdit.cursorPositionChanged.connect(self.cursorPositionChanged.emit)
         self.LineEdit.focusedIn.connect(self.focusInEvent)
         self.LineEdit.focusedOut.connect(self.focusOutEvent)
 
         self.Button = ButtonBase()
         self.Button.setIcon(IconBase.OpenedFolder)
+        self.Button.clicked.connect(self.interacted.emit)
 
         HBoxLayout = QHBoxLayout(self)
         HBoxLayout.setSpacing(0)
         HBoxLayout.setContentsMargins(0, 0, 0, 0)
         HBoxLayout.addWidget(self.LineEdit)
         HBoxLayout.addWidget(self.Button, alignment = Qt.AlignRight)
 
@@ -515,18 +519,15 @@
 
     def hideToolTip(self) -> None:
         self.ToolTip.hideText() if self.ToolTip.isVisible() else None
 
     def mouseMoveEvent(self, event: QMouseEvent) -> None:
         position = event.position()
         self.cursorPositionChanged.emit(position.x(), position.y())
-        if 0 < position.x() < self.width() and 0 < position.y() < self.height():
-            pass #self.focusInEvent()
-        else:
-            self.focusOutEvent()
+        self.interacted.emit()
 
     def moveEvent(self, event: QMoveEvent) -> None:
         self.rectChanged.emit(self.rect())
 
     def resizeEvent(self, event: QResizeEvent) -> None:
         self.rectChanged.emit(self.rect())
```

### Comparing `QEasyWidgets-0.1.8/QEasyWidgets/QFunctions.py` & `QEasyWidgets-0.1.9/QEasyWidgets/QFunctions.py`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.8/QEasyWidgets/QTasks.py` & `QEasyWidgets-0.1.9/QEasyWidgets/QTasks.py`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.8/QEasyWidgets/Sources.py` & `QEasyWidgets-0.1.9/QEasyWidgets/Sources.py`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.8/QEasyWidgets/Utils.py` & `QEasyWidgets-0.1.9/QEasyWidgets/Utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -766,41 +766,42 @@
     '''
     def __init__(self,
         Config_Path: Optional[str] = None
     ):
         self.Config_Path = NormPath(Path(os.getenv('SystemDrive')).joinpath('Config.ini')) if Config_Path == None else Config_Path
         os.makedirs(Path(self.Config_Path).parent, exist_ok = True)
 
-    def ReadConfig(self):
-        ConfigParser = configparser.ConfigParser()
-        ConfigParser.read(self.Config_Path)
-        return ConfigParser
+        self.ConfigParser = configparser.ConfigParser()
+        self.ConfigParser.read(self.Config_Path)
+
+    def Parser(self):
+        return self.ConfigParser
 
     def EditConfig(self,
         Section: str = ...,
         Option: str = ...,
         Value: str = ...,
         ConfigParser: Optional[configparser.ConfigParser] = None
     ):
-        ConfigParser = self.ReadConfig() if ConfigParser == None else ConfigParser
+        ConfigParser = self.Parser() if ConfigParser == None else ConfigParser
         try:
             ConfigParser.add_section(Section)
         except:
             pass
         ConfigParser.set(Section, Option, Value)
         with open(self.Config_Path, 'w') as Config:
             ConfigParser.write(Config)
 
     def GetValue(self,
         Section: str = ...,
         Option: str = ...,
         InitValue: Optional[str] = None,
         ConfigParser: Optional[configparser.ConfigParser] = None
     ):
-        ConfigParser = self.ReadConfig() if ConfigParser == None else ConfigParser
+        ConfigParser = self.Parser() if ConfigParser == None else ConfigParser
         try:
             Value = ConfigParser.get(Section, Option)
         except:
             if InitValue != None:
                 self.EditConfig(Section, Option, InitValue, ConfigParser)
                 return InitValue
             else:
```

### Comparing `QEasyWidgets-0.1.8/QEasyWidgets/WindowCustomizer.py` & `QEasyWidgets-0.1.9/QEasyWidgets/WindowCustomizer.py`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.8/QEasyWidgets.egg-info/PKG-INFO` & `QEasyWidgets-0.1.9/QEasyWidgets.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 2.1
 Name: QEasyWidgets
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple widget library based on PySide6
 Home-page: https://github.com/Spr-Aachen/QEasyWidgets
 Author: Spr_Aachen
 Author-email: 2835946988@qq.com
 License: GPLv3
 Project-URL: Source Code, https://github.com/Spr-Aachen/QEasyWidgets
 Project-URL: Bug Tracker, https://github.com/Spr-Aachen/QEasyWidgets/issues
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PySide6
+Requires-Dist: darkdetect
+Requires-Dist: tqdm
+Requires-Dist: psutil
+Requires-Dist: nvidia-ml-py
+Requires-Dist: PyGithub
 
 <div align = "center">
 
 # QEasyWidgets
 
 [![Releases](https://img.shields.io/github/v/release/Spr-Aachen/QEasyWidgets?color=green&label=Release&logo=Github&logoColor=white&style=for-the-badge)](https://github.com/Spr-Aachen/QEasyWidgets/releases/latest)&nbsp;
```

### Comparing `QEasyWidgets-0.1.8/README.md` & `QEasyWidgets-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.8/setup.py` & `QEasyWidgets-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open('./README.md', encoding = 'utf-8') as f:
     LongDescription = f.read()
 
 ##############################################################################################################################
 
 setup(
     name = "QEasyWidgets",
-    version = '0.1.8',
+    version = '0.1.9',
     description = 'A simple widget library based on PySide6',
     long_description = LongDescription,
     long_description_content_type = 'text/markdown',
     license = 'GPLv3',
     author = "Spr_Aachen",
     author_email = '2835946988@qq.com',
     url = 'https://github.com/Spr-Aachen/QEasyWidgets',
```

