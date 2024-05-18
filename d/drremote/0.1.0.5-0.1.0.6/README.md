# Comparing `tmp/drremote-0.1.0.5.tar.gz` & `tmp/drremote-0.1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drremote-0.1.0.5.tar", last modified: Fri May 17 07:38:30 2024, max compression
+gzip compressed data, was "drremote-0.1.0.6.tar", last modified: Sat May 18 12:14:10 2024, max compression
```

## Comparing `drremote-0.1.0.5.tar` & `drremote-0.1.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dieterstockhausen   (501) staff       (20)        0 2024-05-17 07:38:30.370733 drremote-0.1.0.5/
--rw-r--r--   0 dieterstockhausen   (501) staff       (20)     1075 2021-12-24 14:45:06.000000 drremote-0.1.0.5/LICENSE
--rw-r--r--   0 dieterstockhausen   (501) staff       (20)     4135 2024-05-17 07:38:30.370431 drremote-0.1.0.5/PKG-INFO
--rw-r--r--   0 dieterstockhausen   (501) staff       (20)     3728 2021-12-29 17:11:37.000000 drremote-0.1.0.5/README.md
--rw-r--r--   0 dieterstockhausen   (501) staff       (20)       38 2024-05-17 07:38:30.370786 drremote-0.1.0.5/setup.cfg
--rw-r--r--   0 dieterstockhausen   (501) staff       (20)      939 2024-05-14 18:15:10.000000 drremote-0.1.0.5/setup.py
-drwxr-xr-x   0 dieterstockhausen   (501) staff       (20)        0 2024-05-17 07:38:30.364405 drremote-0.1.0.5/src/
-drwxr-xr-x   0 dieterstockhausen   (501) staff       (20)        0 2024-05-17 07:38:30.366668 drremote-0.1.0.5/src/drremote/
--rw-r--r--   0 dieterstockhausen   (501) staff       (20)      143 2023-10-02 18:00:01.000000 drremote-0.1.0.5/src/drremote/__init__.py
--rwxr-xr-x   0 dieterstockhausen   (501) staff       (20)      114 2023-10-02 17:40:21.000000 drremote-0.1.0.5/src/drremote/__main__.py
--rwxr-xr-x   0 dieterstockhausen   (501) staff       (20)     5709 2021-12-29 08:33:05.000000 drremote-0.1.0.5/src/drremote/drremote.py
--rwxr-xr-x   0 dieterstockhausen   (501) staff       (20)     1649 2021-12-21 07:56:39.000000 drremote-0.1.0.5/src/drremote/get_resolve.py
--rw-r--r--   0 dieterstockhausen   (501) staff       (20)      644 2021-12-29 08:30:42.000000 drremote-0.1.0.5/src/drremote/output.py
--rwxr-xr-x   0 dieterstockhausen   (501) staff       (20)     2539 2021-12-29 08:15:44.000000 drremote-0.1.0.5/src/drremote/parse.py
-drwxr-xr-x   0 dieterstockhausen   (501) staff       (20)        0 2024-05-17 07:38:30.370160 drremote-0.1.0.5/src/drremote.egg-info/
--rw-r--r--   0 dieterstockhausen   (501) staff       (20)     4135 2024-05-17 07:38:30.000000 drremote-0.1.0.5/src/drremote.egg-info/PKG-INFO
--rw-r--r--   0 dieterstockhausen   (501) staff       (20)      357 2024-05-17 07:38:30.000000 drremote-0.1.0.5/src/drremote.egg-info/SOURCES.txt
--rw-r--r--   0 dieterstockhausen   (501) staff       (20)        1 2024-05-17 07:38:30.000000 drremote-0.1.0.5/src/drremote.egg-info/dependency_links.txt
--rw-r--r--   0 dieterstockhausen   (501) staff       (20)       47 2024-05-17 07:38:30.000000 drremote-0.1.0.5/src/drremote.egg-info/entry_points.txt
--rw-r--r--   0 dieterstockhausen   (501) staff       (20)        9 2024-05-17 07:38:30.000000 drremote-0.1.0.5/src/drremote.egg-info/top_level.txt
+drwxr-xr-x   0 dieterstockhausen   (501) staff       (20)        0 2024-05-18 12:14:10.332781 drremote-0.1.0.6/
+-rw-r--r--   0 dieterstockhausen   (501) staff       (20)     1075 2021-12-24 14:45:06.000000 drremote-0.1.0.6/LICENSE
+-rw-r--r--   0 dieterstockhausen   (501) staff       (20)     4171 2024-05-18 12:14:10.332351 drremote-0.1.0.6/PKG-INFO
+-rw-r--r--   0 dieterstockhausen   (501) staff       (20)     3764 2024-05-18 12:12:39.000000 drremote-0.1.0.6/README.md
+-rw-r--r--   0 dieterstockhausen   (501) staff       (20)       38 2024-05-18 12:14:10.332851 drremote-0.1.0.6/setup.cfg
+-rw-r--r--   0 dieterstockhausen   (501) staff       (20)      939 2024-05-18 12:12:39.000000 drremote-0.1.0.6/setup.py
+drwxr-xr-x   0 dieterstockhausen   (501) staff       (20)        0 2024-05-18 12:14:10.321482 drremote-0.1.0.6/src/
+drwxr-xr-x   0 dieterstockhausen   (501) staff       (20)        0 2024-05-18 12:14:10.328135 drremote-0.1.0.6/src/drremote/
+-rw-r--r--   0 dieterstockhausen   (501) staff       (20)      143 2024-05-17 07:47:42.000000 drremote-0.1.0.6/src/drremote/__init__.py
+-rwxr-xr-x   0 dieterstockhausen   (501) staff       (20)      114 2024-05-17 07:47:42.000000 drremote-0.1.0.6/src/drremote/__main__.py
+-rwxr-xr-x   0 dieterstockhausen   (501) staff       (20)     5709 2024-05-17 07:47:42.000000 drremote-0.1.0.6/src/drremote/drremote.py
+-rwxr-xr-x   0 dieterstockhausen   (501) staff       (20)     1649 2024-05-17 07:47:42.000000 drremote-0.1.0.6/src/drremote/get_resolve.py
+-rw-r--r--   0 dieterstockhausen   (501) staff       (20)      644 2024-05-17 07:47:42.000000 drremote-0.1.0.6/src/drremote/output.py
+-rwxr-xr-x   0 dieterstockhausen   (501) staff       (20)     2539 2024-05-17 07:47:42.000000 drremote-0.1.0.6/src/drremote/parse.py
+drwxr-xr-x   0 dieterstockhausen   (501) staff       (20)        0 2024-05-18 12:14:10.331921 drremote-0.1.0.6/src/drremote.egg-info/
+-rw-r--r--   0 dieterstockhausen   (501) staff       (20)     4171 2024-05-18 12:14:10.000000 drremote-0.1.0.6/src/drremote.egg-info/PKG-INFO
+-rw-r--r--   0 dieterstockhausen   (501) staff       (20)      357 2024-05-18 12:14:10.000000 drremote-0.1.0.6/src/drremote.egg-info/SOURCES.txt
+-rw-r--r--   0 dieterstockhausen   (501) staff       (20)        1 2024-05-18 12:14:10.000000 drremote-0.1.0.6/src/drremote.egg-info/dependency_links.txt
+-rw-r--r--   0 dieterstockhausen   (501) staff       (20)       47 2024-05-18 12:14:10.000000 drremote-0.1.0.6/src/drremote.egg-info/entry_points.txt
+-rw-r--r--   0 dieterstockhausen   (501) staff       (20)        9 2024-05-18 12:14:10.000000 drremote-0.1.0.6/src/drremote.egg-info/top_level.txt
```

### Comparing `drremote-0.1.0.5/LICENSE` & `drremote-0.1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `drremote-0.1.0.5/PKG-INFO` & `drremote-0.1.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,84 +1,104 @@
 Metadata-Version: 2.1
 Name: drremote
-Version: 0.1.0.5
+Version: 0.1.0.6
 Summary: DRRemote is a python modul which offers access to Davinci Resolve Studio.
 Home-page: 
 Download-URL: https://github.com/sto3014/DRRemote/archive/refs/heads/main.zip
 Author: Dieter Stockhausen
 Author-email: dieter@schwingenhausen.at
 License: MIT
 Keywords: python davinci resolve api
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DRRemote
 
 DRRemote is a python modul which offers access to Davinci Resolve Studio.
-At the time the functionality is very basic. DRRemote is used in conjunction with [LRDavinci](https://github.com/sto3014/LRDavinci).
+At the time the functionality is very basic. DRRemote is used in conjunction
+with [LRDavinci](https://github.com/sto3014/LRDavinci).
 LRDavinci is a Lightroom plug-in for Davinci Resolve Studio
 
 ## Features
+
 * Changes the current timeline
-* Retrieves the attributes for the current timeline 
-  * name, type and ipaddress of database
-  * name of project
-  * name of timeline
+* Retrieves the attributes for the current timeline
+    * name, type and ipaddress of database
+    * name of project
+    * name of timeline
 
 ## Requirements
-* Python 3.6 (not more, not less due to Davinci Resolve restrictions)  
+
+* Python >= 3.6
 * Davinci Resolve Studio (license is needed for Davinci Resolve's Python API).
 
 ## Installation
+
 1. [Python](https://www.python.org/downloads/)  
-    You need to install version 3.6.x.
-2. PIP 
-   * Windows
+   You need to install version >= 3.6
+2. Install/update PIP
+    * Windows
         * python -m pip install --upgrade pip
-   * macOS
-        * curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py  
+    * macOS
+        * curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
         * python get-pip.py
 3. DRRemote
-   * pip install drremote
-4. Davinci Resolve scripting environment  
+    * pip install drremote
+4. Set the Davinci Resolve scripting environment.
    See readme file:  
-  macOS  
-  ```/Library/Application Support/Blackmagic Design/DaVinci Resolve/Developer/Scripting/README.txt```  
-  Windows  
-    ```%PROGRAMDATA%\Blackmagic Design\DaVinci Resolve\Support\Developer\Scripting\README.txt```
+   macOS  
+   ```/Library/Application Support/Blackmagic Design/DaVinci Resolve/Developer/Scripting/README.txt```  
+   Windows  
+   ```%PROGRAMDATA%\Blackmagic Design\DaVinci Resolve\Support\Developer\Scripting\README.txt```
+
 ## Usage
-You must execute __DRRemote__ in a command prompt (Windows) or terminal (macOS).  
-Remarks for Windows:  
-After you installed drremote with PIP, an executable is created as well: 
+
+__DRRemote__ must be executed in a command prompt (Windows) or terminal (macOS) window. You can do so by calling
+the drremote executable/script. To execute drremote you must use the full path or extend your PATH variable.
+
+* Windows:
+
+```
+%APPDATA%\Programs\Python\Python36\Scripts\drremote.exe
+```
+
+* macOS
+
 ```
-%APPDATA%\Programs\Python\Python36\Scripts\drremote.exe.
+/Library/Frameworks/Python.framework/Versions/3.6/bin/drremote
 ```
-To execute drremote.exe you must use the full path or extend your PATH variable.
+
 
 A simple example:
+
 * Start Davinci Resolve Studio, open a project and select a timeline
 * Open a Command Prompt/Terminal and type:
+
 ```
 drremote -m gettimeline -o out.txt
 ```
+
 If successful you find the gathered information in file out.txt in your current directory:
+
 ```
 Success
 project=Snippets
 timeline=2021-12-10-First Snow
 database=2021:Disk
 ```
+
 If you get an error, you may find some more information in the log logfile:
-* MacOS  
-  * $TMPDIR/drremote.log
-* Windows  
-  * %TEMP%/drremote.log
 
+* MacOS
+    * $TMPDIR/drremote.log
+* Windows
+    * %TEMP%/drremote.log
 
 For the commandline arguments see ```drremote --help```:
+
 ```
 usage: drremote [-h] -m {settimeline,gettimeline} [-p PROJECT [PROJECT ...]]
                 [-t TIMELINE [TIMELINE ...]] [-d DATABASE [DATABASE ...]] -o
                 OUTPUT_PATH [OUTPUT_PATH ...] [-w WAIT]
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -95,24 +115,29 @@
   -o OUTPUT_PATH [OUTPUT_PATH ...], --output-path OUTPUT_PATH [OUTPUT_PATH ...]
                         The name and path of the output file. This file holds
                         the result like timeline attributes or error messages.
   -w WAIT, --wait WAIT  Amounts of seconds to wait between the first and
                         second connection attempt
 ```
 
-###Examples  
-#### Set the current timeline in Davinci resolve   
+###Examples
+
+#### Set the current timeline in Davinci resolve
+
 ```
 drremote -m settimeline -t "2021-12-10-First Snow" -p Snippets -d 2021:disk -o out.txt
 ```  
 
-#### Get the current timeline IDs  
+#### Get the current timeline IDs
+
 ```
 drremote -m gettimeline -o out.txt
 ```
+
 The result is written into __out.txt__:
+
 ```
 Success
 project=Snippets
 timeline=2021-12-10-First Snow
 database=2021:Disk
 ```
```

### Comparing `drremote-0.1.0.5/README.md` & `drremote-0.1.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,91 @@
 # DRRemote
 
 DRRemote is a python modul which offers access to Davinci Resolve Studio.
-At the time the functionality is very basic. DRRemote is used in conjunction with [LRDavinci](https://github.com/sto3014/LRDavinci).
+At the time the functionality is very basic. DRRemote is used in conjunction
+with [LRDavinci](https://github.com/sto3014/LRDavinci).
 LRDavinci is a Lightroom plug-in for Davinci Resolve Studio
 
 ## Features
+
 * Changes the current timeline
-* Retrieves the attributes for the current timeline 
-  * name, type and ipaddress of database
-  * name of project
-  * name of timeline
+* Retrieves the attributes for the current timeline
+    * name, type and ipaddress of database
+    * name of project
+    * name of timeline
 
 ## Requirements
-* Python 3.6 (not more, not less due to Davinci Resolve restrictions)  
+
+* Python >= 3.6
 * Davinci Resolve Studio (license is needed for Davinci Resolve's Python API).
 
 ## Installation
+
 1. [Python](https://www.python.org/downloads/)  
-    You need to install version 3.6.x.
-2. PIP 
-   * Windows
+   You need to install version >= 3.6
+2. Install/update PIP
+    * Windows
         * python -m pip install --upgrade pip
-   * macOS
-        * curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py  
+    * macOS
+        * curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
         * python get-pip.py
 3. DRRemote
-   * pip install drremote
-4. Davinci Resolve scripting environment  
+    * pip install drremote
+4. Set the Davinci Resolve scripting environment.
    See readme file:  
-  macOS  
-  ```/Library/Application Support/Blackmagic Design/DaVinci Resolve/Developer/Scripting/README.txt```  
-  Windows  
-    ```%PROGRAMDATA%\Blackmagic Design\DaVinci Resolve\Support\Developer\Scripting\README.txt```
+   macOS  
+   ```/Library/Application Support/Blackmagic Design/DaVinci Resolve/Developer/Scripting/README.txt```  
+   Windows  
+   ```%PROGRAMDATA%\Blackmagic Design\DaVinci Resolve\Support\Developer\Scripting\README.txt```
+
 ## Usage
-You must execute __DRRemote__ in a command prompt (Windows) or terminal (macOS).  
-Remarks for Windows:  
-After you installed drremote with PIP, an executable is created as well: 
+
+__DRRemote__ must be executed in a command prompt (Windows) or terminal (macOS) window. You can do so by calling
+the drremote executable/script. To execute drremote you must use the full path or extend your PATH variable.
+
+* Windows:
+
+```
+%APPDATA%\Programs\Python\Python36\Scripts\drremote.exe
+```
+
+* macOS
+
 ```
-%APPDATA%\Programs\Python\Python36\Scripts\drremote.exe.
+/Library/Frameworks/Python.framework/Versions/3.6/bin/drremote
 ```
-To execute drremote.exe you must use the full path or extend your PATH variable.
+
 
 A simple example:
+
 * Start Davinci Resolve Studio, open a project and select a timeline
 * Open a Command Prompt/Terminal and type:
+
 ```
 drremote -m gettimeline -o out.txt
 ```
+
 If successful you find the gathered information in file out.txt in your current directory:
+
 ```
 Success
 project=Snippets
 timeline=2021-12-10-First Snow
 database=2021:Disk
 ```
+
 If you get an error, you may find some more information in the log logfile:
-* MacOS  
-  * $TMPDIR/drremote.log
-* Windows  
-  * %TEMP%/drremote.log
 
+* MacOS
+    * $TMPDIR/drremote.log
+* Windows
+    * %TEMP%/drremote.log
 
 For the commandline arguments see ```drremote --help```:
+
 ```
 usage: drremote [-h] -m {settimeline,gettimeline} [-p PROJECT [PROJECT ...]]
                 [-t TIMELINE [TIMELINE ...]] [-d DATABASE [DATABASE ...]] -o
                 OUTPUT_PATH [OUTPUT_PATH ...] [-w WAIT]
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -82,24 +102,29 @@
   -o OUTPUT_PATH [OUTPUT_PATH ...], --output-path OUTPUT_PATH [OUTPUT_PATH ...]
                         The name and path of the output file. This file holds
                         the result like timeline attributes or error messages.
   -w WAIT, --wait WAIT  Amounts of seconds to wait between the first and
                         second connection attempt
 ```
 
-###Examples  
-#### Set the current timeline in Davinci resolve   
+###Examples
+
+#### Set the current timeline in Davinci resolve
+
 ```
 drremote -m settimeline -t "2021-12-10-First Snow" -p Snippets -d 2021:disk -o out.txt
 ```  
 
-#### Get the current timeline IDs  
+#### Get the current timeline IDs
+
 ```
 drremote -m gettimeline -o out.txt
 ```
+
 The result is written into __out.txt__:
+
 ```
 Success
 project=Snippets
 timeline=2021-12-10-First Snow
 database=2021:Disk
 ```
```

### Comparing `drremote-0.1.0.5/setup.py` & `drremote-0.1.0.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
-__version__ = '0.1.0.5'
+__version__ = '0.1.0.6'
 setup(
     name='drremote',
     version=__version__,
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     url='',
     license='MIT',
```

### Comparing `drremote-0.1.0.5/src/drremote/drremote.py` & `drremote-0.1.0.6/src/drremote/drremote.py`

 * *Files identical despite different names*

### Comparing `drremote-0.1.0.5/src/drremote/get_resolve.py` & `drremote-0.1.0.6/src/drremote/get_resolve.py`

 * *Files identical despite different names*

### Comparing `drremote-0.1.0.5/src/drremote/output.py` & `drremote-0.1.0.6/src/drremote/output.py`

 * *Files identical despite different names*

### Comparing `drremote-0.1.0.5/src/drremote/parse.py` & `drremote-0.1.0.6/src/drremote/parse.py`

 * *Files identical despite different names*

### Comparing `drremote-0.1.0.5/src/drremote.egg-info/PKG-INFO` & `drremote-0.1.0.6/src/drremote.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,84 +1,104 @@
 Metadata-Version: 2.1
 Name: drremote
-Version: 0.1.0.5
+Version: 0.1.0.6
 Summary: DRRemote is a python modul which offers access to Davinci Resolve Studio.
 Home-page: 
 Download-URL: https://github.com/sto3014/DRRemote/archive/refs/heads/main.zip
 Author: Dieter Stockhausen
 Author-email: dieter@schwingenhausen.at
 License: MIT
 Keywords: python davinci resolve api
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DRRemote
 
 DRRemote is a python modul which offers access to Davinci Resolve Studio.
-At the time the functionality is very basic. DRRemote is used in conjunction with [LRDavinci](https://github.com/sto3014/LRDavinci).
+At the time the functionality is very basic. DRRemote is used in conjunction
+with [LRDavinci](https://github.com/sto3014/LRDavinci).
 LRDavinci is a Lightroom plug-in for Davinci Resolve Studio
 
 ## Features
+
 * Changes the current timeline
-* Retrieves the attributes for the current timeline 
-  * name, type and ipaddress of database
-  * name of project
-  * name of timeline
+* Retrieves the attributes for the current timeline
+    * name, type and ipaddress of database
+    * name of project
+    * name of timeline
 
 ## Requirements
-* Python 3.6 (not more, not less due to Davinci Resolve restrictions)  
+
+* Python >= 3.6
 * Davinci Resolve Studio (license is needed for Davinci Resolve's Python API).
 
 ## Installation
+
 1. [Python](https://www.python.org/downloads/)  
-    You need to install version 3.6.x.
-2. PIP 
-   * Windows
+   You need to install version >= 3.6
+2. Install/update PIP
+    * Windows
         * python -m pip install --upgrade pip
-   * macOS
-        * curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py  
+    * macOS
+        * curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
         * python get-pip.py
 3. DRRemote
-   * pip install drremote
-4. Davinci Resolve scripting environment  
+    * pip install drremote
+4. Set the Davinci Resolve scripting environment.
    See readme file:  
-  macOS  
-  ```/Library/Application Support/Blackmagic Design/DaVinci Resolve/Developer/Scripting/README.txt```  
-  Windows  
-    ```%PROGRAMDATA%\Blackmagic Design\DaVinci Resolve\Support\Developer\Scripting\README.txt```
+   macOS  
+   ```/Library/Application Support/Blackmagic Design/DaVinci Resolve/Developer/Scripting/README.txt```  
+   Windows  
+   ```%PROGRAMDATA%\Blackmagic Design\DaVinci Resolve\Support\Developer\Scripting\README.txt```
+
 ## Usage
-You must execute __DRRemote__ in a command prompt (Windows) or terminal (macOS).  
-Remarks for Windows:  
-After you installed drremote with PIP, an executable is created as well: 
+
+__DRRemote__ must be executed in a command prompt (Windows) or terminal (macOS) window. You can do so by calling
+the drremote executable/script. To execute drremote you must use the full path or extend your PATH variable.
+
+* Windows:
+
+```
+%APPDATA%\Programs\Python\Python36\Scripts\drremote.exe
+```
+
+* macOS
+
 ```
-%APPDATA%\Programs\Python\Python36\Scripts\drremote.exe.
+/Library/Frameworks/Python.framework/Versions/3.6/bin/drremote
 ```
-To execute drremote.exe you must use the full path or extend your PATH variable.
+
 
 A simple example:
+
 * Start Davinci Resolve Studio, open a project and select a timeline
 * Open a Command Prompt/Terminal and type:
+
 ```
 drremote -m gettimeline -o out.txt
 ```
+
 If successful you find the gathered information in file out.txt in your current directory:
+
 ```
 Success
 project=Snippets
 timeline=2021-12-10-First Snow
 database=2021:Disk
 ```
+
 If you get an error, you may find some more information in the log logfile:
-* MacOS  
-  * $TMPDIR/drremote.log
-* Windows  
-  * %TEMP%/drremote.log
 
+* MacOS
+    * $TMPDIR/drremote.log
+* Windows
+    * %TEMP%/drremote.log
 
 For the commandline arguments see ```drremote --help```:
+
 ```
 usage: drremote [-h] -m {settimeline,gettimeline} [-p PROJECT [PROJECT ...]]
                 [-t TIMELINE [TIMELINE ...]] [-d DATABASE [DATABASE ...]] -o
                 OUTPUT_PATH [OUTPUT_PATH ...] [-w WAIT]
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -95,24 +115,29 @@
   -o OUTPUT_PATH [OUTPUT_PATH ...], --output-path OUTPUT_PATH [OUTPUT_PATH ...]
                         The name and path of the output file. This file holds
                         the result like timeline attributes or error messages.
   -w WAIT, --wait WAIT  Amounts of seconds to wait between the first and
                         second connection attempt
 ```
 
-###Examples  
-#### Set the current timeline in Davinci resolve   
+###Examples
+
+#### Set the current timeline in Davinci resolve
+
 ```
 drremote -m settimeline -t "2021-12-10-First Snow" -p Snippets -d 2021:disk -o out.txt
 ```  
 
-#### Get the current timeline IDs  
+#### Get the current timeline IDs
+
 ```
 drremote -m gettimeline -o out.txt
 ```
+
 The result is written into __out.txt__:
+
 ```
 Success
 project=Snippets
 timeline=2021-12-10-First Snow
 database=2021:Disk
 ```
```

