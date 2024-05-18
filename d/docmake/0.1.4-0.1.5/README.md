# Comparing `tmp/docmake-0.1.4.tar.gz` & `tmp/docmake-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmake-0.1.4.tar", max compression
+gzip compressed data, was "docmake-0.1.5.tar", max compression
```

## Comparing `docmake-0.1.4.tar` & `docmake-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0    11358 2024-05-13 15:11:36.044304 docmake-0.1.4/LICENSE
--rwxr-xr-x   0        0        0     3953 2024-05-13 16:01:03.066258 docmake-0.1.4/README.md
--rwxr-xr-x   0        0        0      421 2024-05-18 03:58:31.013203 docmake-0.1.4/pyproject.toml
--rwxr-xr-x   0        0        0        0 2024-05-13 15:24:15.859574 docmake-0.1.4/src/__init__.py
--rwxr-xr-x   0        0        0    31385 2024-05-18 03:54:45.639907 docmake-0.1.4/src/app.py
--rw-r--r--   0        0        0     4469 1970-01-01 00:00:00.000000 docmake-0.1.4/PKG-INFO
+-rwxr-xr-x   0        0        0    11358 2024-05-13 15:11:36.044304 docmake-0.1.5/LICENSE
+-rwxr-xr-x   0        0        0     4393 2024-05-18 04:07:24.754310 docmake-0.1.5/README.md
+-rwxr-xr-x   0        0        0      421 2024-05-18 04:25:19.382255 docmake-0.1.5/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2024-05-13 15:24:15.859574 docmake-0.1.5/src/__init__.py
+-rwxr-xr-x   0        0        0    31385 2024-05-18 03:54:45.639907 docmake-0.1.5/src/app.py
+-rw-r--r--   0        0        0     4909 1970-01-01 00:00:00.000000 docmake-0.1.5/PKG-INFO
```

### Comparing `docmake-0.1.4/LICENSE` & `docmake-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `docmake-0.1.4/README.md` & `docmake-0.1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,33 +4,41 @@
 
 ## Key Features
 
 - Generate PDFs by combining Markdown, HTML, and CSS.
 - Add custom headers and footers.
 - User-friendly Gradio web interface. 
 
+以下に、より丁寧でわかりやすいREADMEのインストール手順を示します。
+
+---
+
 ## Installation
 
-1. Install Python.
+以下に2～4の手順をまとめた、丁寧に書き直したREADMEのインストールセクションを示します。
 
-2. Clone this repository:
+---
 
-   ```bash
-   git clone https://github.com/morisono/docmaker_webui.git
-   ```
+## Installation
+
+### Prerequisites
 
-3. Navigate to the project directory:
+- Ensure that Python is installed on your system. You can download it from the [official Python website](https://www.python.org/).
+
+### Install via pip
 
    ```bash
-   cd docmaker_webui
+   pip install docmake
    ```
 
-4. Install dependencies:
+### Manual Installation
 
    ```bash
+   git clone https://github.com/morisono/docmaker_webui.git docmake
+   cd docmake
    pip install -r requirements.txt
    ```
 
 ## CLI Usage
 
 ```sh
 usage: 
@@ -44,14 +52,17 @@
         - Encrypt/Decrypto a PDF:
             docmake -i in.[html|pdf] -o out.pdf [options]
 
             For example:
                 docmake -i demo.pdf -o demo.encrypted.pdf --encrypto --autogen
                 docmake -i demo.encrypted.pdf -o demo.decrypted.pdf --decrypto
 
+         - Read remote file:
+            docmake -i $gist --config config.yaml --verbose --qr 40
+
     [Units]
         You can use the following units for width, height, and margin options:
         - px (pixels) - Default unit., in (inches)., cm (centimeters)., mm (millimeters).
 
     [Formats]
         The following paper formats are available for the format option:
         - Letter, Legal, Tabloid, Ledger, A0, A1, A2, A3, A4 (default), A5
```

### Comparing `docmake-0.1.4/src/app.py` & `docmake-0.1.5/src/app.py`

 * *Files identical despite different names*

### Comparing `docmake-0.1.4/PKG-INFO` & `docmake-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docmake
-Version: 0.1.4
+Version: 0.1.5
 Summary: Generate pdf files from other format documents.
 Home-page: https://github.com/morisono/docmaker_webui
 Author: admin
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -18,33 +18,41 @@
 
 ## Key Features
 
 - Generate PDFs by combining Markdown, HTML, and CSS.
 - Add custom headers and footers.
 - User-friendly Gradio web interface. 
 
+以下に、より丁寧でわかりやすいREADMEのインストール手順を示します。
+
+---
+
 ## Installation
 
-1. Install Python.
+以下に2～4の手順をまとめた、丁寧に書き直したREADMEのインストールセクションを示します。
 
-2. Clone this repository:
+---
 
-   ```bash
-   git clone https://github.com/morisono/docmaker_webui.git
-   ```
+## Installation
+
+### Prerequisites
 
-3. Navigate to the project directory:
+- Ensure that Python is installed on your system. You can download it from the [official Python website](https://www.python.org/).
+
+### Install via pip
 
    ```bash
-   cd docmaker_webui
+   pip install docmake
    ```
 
-4. Install dependencies:
+### Manual Installation
 
    ```bash
+   git clone https://github.com/morisono/docmaker_webui.git docmake
+   cd docmake
    pip install -r requirements.txt
    ```
 
 ## CLI Usage
 
 ```sh
 usage: 
@@ -58,14 +66,17 @@
         - Encrypt/Decrypto a PDF:
             docmake -i in.[html|pdf] -o out.pdf [options]
 
             For example:
                 docmake -i demo.pdf -o demo.encrypted.pdf --encrypto --autogen
                 docmake -i demo.encrypted.pdf -o demo.decrypted.pdf --decrypto
 
+         - Read remote file:
+            docmake -i $gist --config config.yaml --verbose --qr 40
+
     [Units]
         You can use the following units for width, height, and margin options:
         - px (pixels) - Default unit., in (inches)., cm (centimeters)., mm (millimeters).
 
     [Formats]
         The following paper formats are available for the format option:
         - Letter, Legal, Tabloid, Ledger, A0, A1, A2, A3, A4 (default), A5
```

