# Comparing `tmp/wheke-0.0.1a9.tar.gz` & `tmp/wheke-0.1.0.tar.gz`

## Comparing `wheke-0.0.1a9.tar` & `wheke-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 wheke-0.0.1a9/.env.example
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 wheke-0.0.1a9/mkdocs.yml
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 wheke-0.0.1a9/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 wheke-0.0.1a9/.github/workflows/test-suite.yml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 wheke-0.0.1a9/docs/api.md
--rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 wheke-0.0.1a9/docs/index.md
--rw-r--r--   0        0        0    24960 2020-02-02 00:00:00.000000 wheke-0.0.1a9/docs/wheke.png
--rw-r--r--   0        0        0   390125 2020-02-02 00:00:00.000000 wheke-0.0.1a9/docs/img/wheke-homepage.png
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 wheke-0.0.1a9/src/wheke/__about__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wheke-0.0.1a9/src/wheke/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 wheke-0.0.1a9/src/wheke/__main__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 wheke-0.0.1a9/src/wheke/cli.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 wheke-0.0.1a9/src/wheke/core.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 wheke-0.0.1a9/src/wheke/demo.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 wheke-0.0.1a9/src/wheke/exceptions.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 wheke-0.0.1a9/src/wheke/pod.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheke-0.0.1a9/src/wheke/py.typed
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 wheke-0.0.1a9/src/wheke/service.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 wheke-0.0.1a9/src/wheke/settings.py
--rw-r--r--   0        0        0    24960 2020-02-02 00:00:00.000000 wheke-0.0.1a9/src/wheke/static/wheke.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheke-0.0.1a9/tests/__init__.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 wheke-0.0.1a9/tests/conftest.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 wheke-0.0.1a9/tests/test_app.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 wheke-0.0.1a9/tests/test_cli.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 wheke-0.0.1a9/tests/test_service.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 wheke-0.0.1a9/tests/example_app/__init__.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 wheke-0.0.1a9/tests/example_app/static/test.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 wheke-0.0.1a9/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 wheke-0.0.1a9/LICENSE.txt
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 wheke-0.0.1a9/README.md
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 wheke-0.0.1a9/pyproject.toml
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 wheke-0.0.1a9/PKG-INFO
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 wheke-0.1.0/.env.example
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 wheke-0.1.0/mkdocs.yml
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 wheke-0.1.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 wheke-0.1.0/.github/workflows/test-suite.yml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 wheke-0.1.0/docs/api.md
+-rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 wheke-0.1.0/docs/index.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 wheke-0.1.0/docs/pods.md
+-rw-r--r--   0        0        0    24960 2020-02-02 00:00:00.000000 wheke-0.1.0/docs/wheke.png
+-rw-r--r--   0        0        0   390125 2020-02-02 00:00:00.000000 wheke-0.1.0/docs/img/wheke-homepage.png
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 wheke-0.1.0/src/wheke/__about__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 wheke-0.1.0/src/wheke/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 wheke-0.1.0/src/wheke/__main__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 wheke-0.1.0/src/wheke/_cli.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 wheke-0.1.0/src/wheke/_core.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 wheke-0.1.0/src/wheke/_demo.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 wheke-0.1.0/src/wheke/_pod.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 wheke-0.1.0/src/wheke/_service.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 wheke-0.1.0/src/wheke/_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheke-0.1.0/src/wheke/py.typed
+-rw-r--r--   0        0        0    24960 2020-02-02 00:00:00.000000 wheke-0.1.0/src/wheke/static/wheke.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheke-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 wheke-0.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 wheke-0.1.0/tests/test_app.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 wheke-0.1.0/tests/test_cli.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 wheke-0.1.0/tests/example_app/__init__.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 wheke-0.1.0/tests/example_app/static/test.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 wheke-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 wheke-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 wheke-0.1.0/README.md
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 wheke-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 wheke-0.1.0/PKG-INFO
```

### Comparing `wheke-0.0.1a9/mkdocs.yml` & `wheke-0.1.0/mkdocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 site_author: Humberto Rocha
 site_description: A cute framework for small self-hosted apps
 
 repo_url: https://github.com/humrochagf/wheke
 
 nav:
   - Introduction: index.md
+  - Pods: pods.md
   - API Docs: api.md
 
 theme:
   name: material
   features:
     - content.code.annotate
     - content.code.copy
```

### Comparing `wheke-0.0.1a9/.github/workflows/docs.yml` & `wheke-0.1.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `wheke-0.0.1a9/.github/workflows/test-suite.yml` & `wheke-0.1.0/.github/workflows/test-suite.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 name: Test Suite
 
 on:
   push:
-    branches: 
+    branches:
     - main
   pull_request:
     branches:
     - main
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.event.pull_request.number || github.sha }}
@@ -22,17 +22,18 @@
         os: [ubuntu-latest, windows-latest, macos-latest]
         python-version: ['3.10', '3.11', '3.12']
 
     steps:
     - uses: actions/checkout@v4
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
+        cache: pip
 
     - name: Ensure latest pip
       run: |
         python -m pip install --upgrade pip
 
     - name: Install dependencies
       run: |
```

### Comparing `wheke-0.0.1a9/docs/index.md` & `wheke-0.1.0/docs/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 ---
 
 # Introduction
 
 **Wheke** is an opinionated framework to build small scale self-hosted applications and it stands on top of well known packages:
 
 - [FastAPI](https://fastapi.tiangolo.com/) to build the web services.
+- [svcs](https://svcs.hynek.me/) to have a robust service registry.
 - [Typer](https://typer.tiangolo.com/) to build great cli.
 - [Pydantic](https://docs.pydantic.dev/latest/) to build schemas and `.env` based settings.
 - [Rich](https://rich.readthedocs.io/en/stable/) to make your app shine.
 
 It aims to provide you:
 
 - An opinionated structure to write you apps.
@@ -67,15 +68,15 @@
 To see how a Wheke app in a single file looks like let's create a `main.py` file and add a route to show a timezone aware clock:
 
 ```python title="File: main.py"
 from datetime import datetime, timezone
 from zoneinfo import ZoneInfo, ZoneInfoNotFoundError
 
 from fastapi import APIRouter, HTTPException, status
-from wheke import Pod, Wheke
+from wheke import Pod, Wheke, demo_pod
 
 router = APIRouter()
 
 
 @router.get("/clock")
 def clock(tz: str | None = None) -> dict:
     try:
@@ -91,14 +92,15 @@
 
     return {"clock": datetime.now(timezone.utc).astimezone(zone_info)}
 
 
 my_pod = Pod("my-pod", router=router)
 
 wheke = Wheke()
+wheke.add_pod(demo_pod)
 wheke.add_pod(my_pod)
 
 app = wheke.create_app()
 ```
 
 To start the server run:
```

### Comparing `wheke-0.0.1a9/docs/wheke.png` & `wheke-0.1.0/docs/wheke.png`

 * *Files identical despite different names*

### Comparing `wheke-0.0.1a9/docs/img/wheke-homepage.png` & `wheke-0.1.0/docs/img/wheke-homepage.png`

 * *Files identical despite different names*

### Comparing `wheke-0.0.1a9/src/wheke/core.py` & `wheke-0.1.0/src/wheke/_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from importlib import import_module
 
 from fastapi import FastAPI
 from fastapi.staticfiles import StaticFiles
 from typer import Typer
 
-from wheke.cli import empty_callback, version
-from wheke.pod import Pod
-from wheke.service import ServiceRegistry
-from wheke.settings import settings
+from ._cli import empty_callback, version
+from ._pod import Pod
+from ._service import get_service_registry
+from ._settings import settings
 
 
 class Wheke:
     """
     The Wheke class is the entry point to build an application.
     """
 
@@ -33,15 +33,15 @@
         if isinstance(pod_to_add, str):
             module_name, pod_name = pod_to_add.rsplit(".", 1)
             pod = getattr(import_module(module_name), pod_name)
         else:
             pod = pod_to_add
 
         for service_type, service_factory in pod.services:
-            ServiceRegistry.register(service_type, service_factory)
+            get_service_registry().register_factory(service_type, service_factory)
 
         self.pods.append(pod)
 
     def create_app(self) -> FastAPI:
         """
         Create a FastAPI app with all plugged pods.
         """
```

### Comparing `wheke-0.0.1a9/src/wheke/demo.py` & `wheke-0.1.0/src/wheke/_demo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 
 from fastapi import APIRouter, Response
 from fastapi.responses import HTMLResponse
 
-from wheke.pod import Pod
+from ._pod import Pod
 
 STATIC_PATH = Path(__file__).resolve().parent / "static"
 
 DEMO_PAGE = """
 <!doctype html>
 <html>
 <head>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path from fastapi import APIRouter, Response from
-fastapi.responses import HTMLResponse from wheke.pod import Pod STATIC_PATH =
-Path(__file__).resolve().parent / "static" DEMO_PAGE = """
+fastapi.responses import HTMLResponse from ._pod import Pod STATIC_PATH = Path
+(__file__).resolve().parent / "static" DEMO_PAGE = """
 ************ WWhheekkee ************
 [Wheke]
 
 AA ccuuttee ffrraammeewwoorrkk ffoorr ssmmaallll sseellff--hhoosstteedd aappppss Made with ❤️ by _H_u_m_b_e_r_t_o_ _R_o_c_h_a
 Illustrated with ❤️ by _G_i_o_v_a_n_n_a_ _B_i_s_s_a_c_o_t
 """ router = APIRouter() @router.get("/", response_class=HTMLResponse,
 include_in_schema=False) async def index() -> Response: return HTMLResponse
```

### Comparing `wheke-0.0.1a9/src/wheke/pod.py` & `wheke-0.1.0/src/wheke/_pod.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from collections.abc import Callable
 from pathlib import Path
 
 from fastapi import APIRouter
 from typer import Typer
 
-from wheke.service import Service
-
-ServiceList = list[tuple[type[Service], Callable]]
+ServiceList = list[tuple[type, Callable]]
 
 
 class Pod:
     """
     A Pod is the base unity that controls a funcionality.
     """
```

### Comparing `wheke-0.0.1a9/src/wheke/static/wheke.png` & `wheke-0.1.0/src/wheke/static/wheke.png`

 * *Files identical despite different names*

### Comparing `wheke-0.0.1a9/tests/test_app.py` & `wheke-0.1.0/tests/test_app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,66 @@
-from fastapi import FastAPI
+from fastapi import FastAPI, status
 from fastapi.testclient import TestClient
 
-from wheke import Wheke
-from wheke.demo import DEMO_PAGE, demo_pod
-from wheke.pod import Pod
-from wheke.settings import settings
+from wheke import Pod, Wheke, demo_pod, settings
+from wheke._demo import DEMO_PAGE
 
 
 def test_create_app() -> None:
     wheke = Wheke()
 
     app = wheke.create_app()
 
     assert type(app) is FastAPI
-    assert demo_pod in wheke.pods
 
 
-def test_create_app_with_empty_pod() -> None:
+def test_create_app_with_demo_pod_in_settings() -> None:
     before_pods = settings.pods.copy()
-    settings.pods = []
+    settings.pods = ["wheke.demo_pod"]
+
+    wheke = Wheke()
+
+    app = wheke.create_app()
 
+    assert type(app) is FastAPI
+    assert demo_pod in wheke.pods
+
+    settings.pods = before_pods
+
+
+def test_create_app_with_empty_pod() -> None:
     empty_pod = Pod("empty")
     wheke = Wheke()
     wheke.add_pod(empty_pod)
 
     app = wheke.create_app()
 
     assert type(app) is FastAPI
     assert wheke.pods == [empty_pod]
 
-    settings.pods = before_pods
-
 
 def test_demo_pod(client: TestClient) -> None:
     response = client.get("/")
 
-    assert response.status_code == 200
+    assert response.status_code == status.HTTP_200_OK
     assert response.text == DEMO_PAGE
 
 
 def test_static(client: TestClient) -> None:
     response = client.get("/static/test.txt")
 
-    assert response.status_code == 200
+    assert response.status_code == status.HTTP_200_OK
     assert response.text.strip() == "test"
 
 
 def test_ping(client: TestClient) -> None:
     response = client.get("/ping")
 
-    assert response.status_code == 200
+    assert response.status_code == status.HTTP_200_OK
+    assert response.json() == {"value": "pong"}
+
+
+def test_aping(client: TestClient) -> None:
+    response = client.get("/aping")
+
+    assert response.status_code == status.HTTP_200_OK
     assert response.json() == {"value": "pong"}
```

### Comparing `wheke-0.0.1a9/tests/test_cli.py` & `wheke-0.1.0/tests/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from typer import Typer
 from typer.testing import CliRunner
 
 from wheke import Wheke
 from wheke.__about__ import __version__
 from wheke.__main__ import cli as main_cli
-from wheke.demo import demo_pod
 
 runner = CliRunner()
 
 
 def test_create_cli() -> None:
     wheke = Wheke()
 
     app = wheke.create_cli()
 
     assert type(app) is Typer
-    assert demo_pod in wheke.pods
 
 
 def test_version() -> None:
     result = runner.invoke(main_cli, "version")
 
     assert result.exit_code == 0
     assert result.stdout.strip() == __version__
```

### Comparing `wheke-0.0.1a9/LICENSE.txt` & `wheke-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wheke-0.0.1a9/README.md` & `wheke-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `wheke-0.0.1a9/pyproject.toml` & `wheke-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -11,26 +11,31 @@
 license = "MIT"
 keywords = []
 authors = [
   { name = "Humberto Rocha", email = "humrochagf@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
-  "Programming Language :: Python",
+  "Framework :: FastAPI",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
+  "Programming Language :: Python",
+  "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
+  "Topic :: Internet :: WWW/HTTP",
+  "Topic :: Internet",
 ]
 dependencies = [
   "fastapi",
   "pydantic",
   "pydantic-settings",
   "rich",
+  "svcs",
   "typer",
 ]
 
 [project.scripts]
 wheke = "wheke.__main__:cli"
 
 [project.urls]
@@ -66,15 +71,27 @@
 [tool.hatch.envs.docs.scripts]
 build = "mkdocs build"
 server = "mkdocs serve"
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.10", "3.11", "3.12"]
 
-[tool.ruff]
+[tool.isort]
+profile = "black"
+skip = [
+  ".env",
+  ".hatch",
+  ".mypy_cache",
+  ".venv",
+  "__pycache__",
+  "env",
+  "venv",
+]
+
+[tool.ruff.lint]
 exclude = [
   ".env",
   ".hatch",
   ".mypy_cache",
   ".venv",
   "__pycache__",
   "env",
@@ -120,21 +137,18 @@
   "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
 ]
 unfixable = [
   # Don't touch unused imports
   "F401",
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["wheke"]
 
-[tool.ruff.flake8-tidy-imports]
-ban-relative-imports = "all"
-
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 [tool.coverage.run]
 source_pkgs = ["wheke", "tests"]
 branch = true
 parallel = true
```

### Comparing `wheke-0.0.1a9/PKG-INFO` & `wheke-0.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: wheke
-Version: 0.0.1a9
+Version: 0.1.0
 Summary: A cute framework for small self-hosted apps
 Project-URL: Documentation, https://wheke.humberto.io/
 Project-URL: Issues, https://github.com/humrochagf/wheke/issues
 Project-URL: Source, https://github.com/humrochagf/wheke
 Author-email: Humberto Rocha <humrochagf@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: FastAPI
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Internet
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Requires-Python: >=3.10
 Requires-Dist: fastapi
 Requires-Dist: pydantic
 Requires-Dist: pydantic-settings
 Requires-Dist: rich
+Requires-Dist: svcs
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
 <h1 align="center" style="font-size: 3rem">
   Wheke
 </h1>
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: wheke Version: 0.0.1a9 Summary: A cute framework
-for small self-hosted apps Project-URL: Documentation, https://
-wheke.humberto.io/ Project-URL: Issues, https://github.com/humrochagf/wheke/
-issues Project-URL: Source, https://github.com/humrochagf/wheke Author-email:
-Humberto Rocha
+Metadata-Version: 2.1 Name: wheke Version: 0.1.0 Summary: A cute framework for
+small self-hosted apps Project-URL: Documentation, https://wheke.humberto.io/
+Project-URL: Issues, https://github.com/humrochagf/wheke/issues Project-URL:
+Source, https://github.com/humrochagf/wheke Author-email: Humberto Rocha
 gmail.com> License-Expression: MIT License-File: LICENSE.txt Classifier:
-Development Status :: 4 - Beta Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
-Python: >=3.10 Requires-Dist: fastapi Requires-Dist: pydantic Requires-Dist:
-pydantic-settings Requires-Dist: rich Requires-Dist: typer Description-Content-
-Type: text/markdown
+Development Status :: 4 - Beta Classifier: Framework :: FastAPI Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python ::
+3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Programming Language :: Python ::
+Implementation :: PyPy Classifier: Topic :: Internet Classifier: Topic ::
+Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
+Requires-Python: >=3.10 Requires-Dist: fastapi Requires-Dist: pydantic
+Requires-Dist: pydantic-settings Requires-Dist: rich Requires-Dist: svcs
+Requires-Dist: typer Description-Content-Type: text/markdown
                               ************ WWhheekkee ************
                                     [Wheke]
                  AA ccuuttee ffrraammeewwoorrkk ffoorr ssmmaallll sseellff--hhoosstteedd aappppss
                              aarrttwwoorrkk bbyy _@@_bb_ii_ss_ss_gg_ii_gg_ii
               _[_T_e_s_t_ _S_u_i_t_e_]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]
 --- **Wheke** is a framework built on top of [FastAPI](https://
 fastapi.tiangolo.com/) that is focussed in small scale self-hosted applications
```

