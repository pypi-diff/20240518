# Comparing `tmp/streamlit-eidos-0.1.0.tar.gz` & `tmp/streamlit-eidos-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-eidos-0.1.0.tar", last modified: Mon May 13 09:56:48 2024, max compression
+gzip compressed data, was "streamlit-eidos-0.2.0.tar", last modified: Sat May 18 05:19:34 2024, max compression
```

## Comparing `streamlit-eidos-0.1.0.tar` & `streamlit-eidos-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,37 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-05-13 09:56:48.133217 streamlit-eidos-0.1.0/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1066 2024-05-07 02:53:06.000000 streamlit-eidos-0.1.0/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)       83 2024-05-07 04:11:10.000000 streamlit-eidos-0.1.0/MANIFEST.in
--rw-r--r--   0 dave      (1000) dave      (1000)     2706 2024-05-13 09:56:48.133217 streamlit-eidos-0.1.0/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     2354 2024-05-12 23:06:44.000000 streamlit-eidos-0.1.0/README.md
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2024-05-13 09:56:48.133217 streamlit-eidos-0.1.0/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)      695 2024-05-12 23:05:38.000000 streamlit-eidos-0.1.0/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-05-13 09:56:48.113216 streamlit-eidos-0.1.0/src/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-05-13 09:56:48.129217 streamlit-eidos-0.1.0/src/streamlit_eidos/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1544 2024-05-13 01:27:50.000000 streamlit-eidos-0.1.0/src/streamlit_eidos/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-05-13 09:56:48.133217 streamlit-eidos-0.1.0/src/streamlit_eidos/frontend/
--rw-rw-r--   0 dave      (1000) dave      (1000)      466 2024-05-07 04:14:11.000000 streamlit-eidos-0.1.0/src/streamlit_eidos/frontend/index.html
--rw-rw-r--   0 dave      (1000) dave      (1000)     1990 2024-05-13 08:50:20.000000 streamlit-eidos-0.1.0/src/streamlit_eidos/frontend/main.js
--rw-rw-r--   0 dave      (1000) dave      (1000)   230931 2024-05-07 02:53:06.000000 streamlit-eidos-0.1.0/src/streamlit_eidos/frontend/streamlit-component-lib.js
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2024-05-07 02:53:06.000000 streamlit-eidos-0.1.0/src/streamlit_eidos/frontend/style.css
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-05-13 09:56:48.133217 streamlit-eidos-0.1.0/src/streamlit_eidos.egg-info/
--rw-r--r--   0 dave      (1000) dave      (1000)     2706 2024-05-13 09:56:47.000000 streamlit-eidos-0.1.0/src/streamlit_eidos.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      456 2024-05-13 09:56:47.000000 streamlit-eidos-0.1.0/src/streamlit_eidos.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2024-05-13 09:56:47.000000 streamlit-eidos-0.1.0/src/streamlit_eidos.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       23 2024-05-13 09:56:47.000000 streamlit-eidos-0.1.0/src/streamlit_eidos.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       16 2024-05-13 09:56:47.000000 streamlit-eidos-0.1.0/src/streamlit_eidos.egg-info/top_level.txt
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-05-18 05:19:34.158002 streamlit-eidos-0.2.0/
+-rw-rw-r--   0 dave      (1000) dave      (1000)       46 2024-05-13 09:56:02.000000 streamlit-eidos-0.2.0/.gitignore
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-05-18 05:19:34.154002 streamlit-eidos-0.2.0/.vscode/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      622 2024-05-18 00:09:04.000000 streamlit-eidos-0.2.0/.vscode/launch.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1066 2024-05-07 02:53:06.000000 streamlit-eidos-0.2.0/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)      131 2024-05-18 05:12:03.000000 streamlit-eidos-0.2.0/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1734 2024-05-18 05:04:35.000000 streamlit-eidos-0.2.0/Makefile
+-rw-r--r--   0 dave      (1000) dave      (1000)     2721 2024-05-18 05:19:34.158002 streamlit-eidos-0.2.0/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2354 2024-05-12 23:06:44.000000 streamlit-eidos-0.2.0/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-05-18 05:19:34.154002 streamlit-eidos-0.2.0/examples/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1874 2024-05-18 04:43:22.000000 streamlit-eidos-0.2.0/examples/test.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)       18 2024-05-12 23:04:43.000000 streamlit-eidos-0.2.0/requirements.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2024-05-18 05:19:34.158002 streamlit-eidos-0.2.0/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)      743 2024-05-18 05:19:28.000000 streamlit-eidos-0.2.0/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-05-18 05:19:34.154002 streamlit-eidos-0.2.0/streamlit_eidos/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1536 2024-05-18 03:46:57.000000 streamlit-eidos-0.2.0/streamlit_eidos/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-05-18 05:19:34.158002 streamlit-eidos-0.2.0/streamlit_eidos/frontend/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      566 2024-05-18 03:30:31.000000 streamlit-eidos-0.2.0/streamlit_eidos/frontend/.eslintrc.cjs
+-rw-rw-r--   0 dave      (1000) dave      (1000)      253 2024-05-18 03:30:31.000000 streamlit-eidos-0.2.0/streamlit_eidos/frontend/.gitignore
+-rw-rw-r--   0 dave      (1000) dave      (1000)       43 2024-05-18 05:17:34.000000 streamlit-eidos-0.2.0/streamlit_eidos/frontend/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-05-18 05:19:34.158002 streamlit-eidos-0.2.0/streamlit_eidos/frontend/dist/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-05-18 05:19:34.158002 streamlit-eidos-0.2.0/streamlit_eidos/frontend/dist/assets/
+-rw-rw-r--   0 dave      (1000) dave      (1000)   322333 2024-05-18 04:18:35.000000 streamlit-eidos-0.2.0/streamlit_eidos/frontend/dist/assets/index-Sp77uM4B.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)      317 2024-05-18 04:18:35.000000 streamlit-eidos-0.2.0/streamlit_eidos/frontend/dist/index.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)      292 2024-05-18 03:53:39.000000 streamlit-eidos-0.2.0/streamlit_eidos/frontend/index.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)   162845 2024-05-18 03:32:04.000000 streamlit-eidos-0.2.0/streamlit_eidos/frontend/package-lock.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)      694 2024-05-18 03:32:04.000000 streamlit-eidos-0.2.0/streamlit_eidos/frontend/package.json
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-05-18 05:19:34.158002 streamlit-eidos-0.2.0/streamlit_eidos/frontend/src/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1764 2024-05-18 04:18:26.000000 streamlit-eidos-0.2.0/streamlit_eidos/frontend/src/Component.jsx
+-rw-rw-r--   0 dave      (1000) dave      (1000)      235 2024-05-18 03:54:11.000000 streamlit-eidos-0.2.0/streamlit_eidos/frontend/src/main.jsx
+-rw-rw-r--   0 dave      (1000) dave      (1000)      180 2024-05-18 03:32:36.000000 streamlit-eidos-0.2.0/streamlit_eidos/frontend/vite.config.js
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-05-18 05:19:34.158002 streamlit-eidos-0.2.0/streamlit_eidos.egg-info/
+-rw-r--r--   0 dave      (1000) dave      (1000)     2721 2024-05-18 05:19:33.000000 streamlit-eidos-0.2.0/streamlit_eidos.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      778 2024-05-18 05:19:34.000000 streamlit-eidos-0.2.0/streamlit_eidos.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2024-05-18 05:19:33.000000 streamlit-eidos-0.2.0/streamlit_eidos.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       37 2024-05-18 05:19:33.000000 streamlit-eidos-0.2.0/streamlit_eidos.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       16 2024-05-18 05:19:33.000000 streamlit-eidos-0.2.0/streamlit_eidos.egg-info/top_level.txt
```

### Comparing `streamlit-eidos-0.1.0/LICENSE` & `streamlit-eidos-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-eidos-0.1.0/PKG-INFO` & `streamlit-eidos-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: streamlit-eidos
-Version: 0.1.0
+Version: 0.2.0
 Summary: Streamlit component for EIDOS framework
 Author: Oceanum
 Author-email: developers@oceanum.science
 Keywords: streamlit,oceanum,eidos,visualisation
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit>=1.2
-Requires-Dist: oceanum
+Requires-Dist: oceanum[eidos]>=0.1.0
 
 # streamlit-eidos
 
 Streamlit component for EIDOS visualisation with bi-directional transport for events.
 
 ## Installation instructions
```

### Comparing `streamlit-eidos-0.1.0/README.md` & `streamlit-eidos-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-eidos-0.1.0/setup.py` & `streamlit-eidos-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-eidos",
-    version="0.1.0",
+    version="0.2.0",
     author="Oceanum",
     author_email="developers@oceanum.science",
     description="Streamlit component for EIDOS framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["streamlit_eidos"],
-    package_dir={"": "src"},
     include_package_data=True,
-    python_requires=">=3.7",
+    package_data={"streamlit_eidos": ["frontend/dist/**/*"]},
+    python_requires=">=3.10",
     keywords=["streamlit", "oceanum", "eidos", "visualisation"],
-    install_requires=["streamlit>=1.2", "oceanum"],
+    install_requires=["streamlit>=1.2", "oceanum[eidos]>=0.1.0"],
     entry_points={},
 )
```

### Comparing `streamlit-eidos-0.1.0/src/streamlit_eidos/__init__.py` & `streamlit-eidos-0.2.0/streamlit_eidos/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import streamlit.components.v1 as components
 
 from oceanum.eidos import Eidos
 
 
 # Tell streamlit that there is a component called streamlit_eidos,
 # and that the code to display that component is in the "frontend" folder
-frontend_dir = (Path(__file__).parent / "frontend").absolute()
+frontend_dir = (Path(__file__).parent / "frontend" / "dist").absolute()
 _component_func = components.declare_component(
     "streamlit_eidos", path=str(frontend_dir)
 )
 
 
 # Create the python function that will be called
 def st_eidos(eidos=None, height=500, events=None):
@@ -37,18 +37,18 @@
         A dictionary containing the dictionary of an EIDOS event.
     """
 
     if eidos is None or not isinstance(eidos, Eidos):
         raise ValueError("First argument must be an instance of Eidos")
 
     renderer = os.environ.get("EIDOS_RENDERER", "https://render.eidos.oceanum.io")
-    print(f"Using renderer at {renderer}")
 
     component_value = _component_func(
         key=eidos.id,
         height=height,
-        spec=eidos.model_dump(),
+        eidos=eidos.model_dump(),
+        spectype="spec",
         events=events if events else ["click"],
         renderer=renderer,
     )
 
     return component_value
```

### Comparing `streamlit-eidos-0.1.0/src/streamlit_eidos.egg-info/PKG-INFO` & `streamlit-eidos-0.2.0/streamlit_eidos.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: streamlit-eidos
-Version: 0.1.0
+Version: 0.2.0
 Summary: Streamlit component for EIDOS framework
 Author: Oceanum
 Author-email: developers@oceanum.science
 Keywords: streamlit,oceanum,eidos,visualisation
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit>=1.2
-Requires-Dist: oceanum
+Requires-Dist: oceanum[eidos]>=0.1.0
 
 # streamlit-eidos
 
 Streamlit component for EIDOS visualisation with bi-directional transport for events.
 
 ## Installation instructions
```

