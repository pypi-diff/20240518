# Comparing `tmp/flexidata-0.0.1.tar.gz` & `tmp/flexidata-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexidata-0.0.1.tar", last modified: Fri May 17 18:26:04 2024, max compression
+gzip compressed data, was "flexidata-0.0.2.tar", last modified: Sat May 18 19:51:11 2024, max compression
```

## Comparing `flexidata-0.0.1.tar` & `flexidata-0.0.2.tar`

### file list

```diff
@@ -1,33 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 18:26:04.540242 flexidata-0.0.1/
--rw-rw-rw-   0        0        0    11558 2024-05-01 19:03:09.000000 flexidata-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       26 2024-05-17 18:22:13.000000 flexidata-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0    15381 2024-05-17 18:26:04.538236 flexidata-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      766 2024-05-17 13:37:32.000000 flexidata-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 18:26:04.504599 flexidata-0.0.1/flexidata/
--rw-rw-rw-   0        0        0     1838 2024-05-05 15:00:12.000000 flexidata-0.0.1/flexidata/Logger.py
--rw-rw-rw-   0        0        0        0 2024-05-02 08:52:21.000000 flexidata-0.0.1/flexidata/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 18:26:04.524322 flexidata-0.0.1/flexidata/models/
--rw-rw-rw-   0        0        0        0 2024-05-02 06:01:08.000000 flexidata-0.0.1/flexidata/models/__init__.py
--rw-rw-rw-   0        0        0      562 2024-05-02 08:41:23.000000 flexidata-0.0.1/flexidata/models/base.py
--rw-rw-rw-   0        0        0     3117 2024-05-02 08:39:53.000000 flexidata-0.0.1/flexidata/models/detectron2.py
-drwxrwxrwx   0        0        0        0 2024-05-17 18:26:04.527324 flexidata-0.0.1/flexidata/parser/
--rw-rw-rw-   0        0        0        0 2024-05-02 06:00:51.000000 flexidata-0.0.1/flexidata/parser/__init__.py
--rw-rw-rw-   0        0        0    21772 2024-05-17 12:54:03.000000 flexidata-0.0.1/flexidata/parser/pdf.py
-drwxrwxrwx   0        0        0        0 2024-05-17 18:26:04.533237 flexidata-0.0.1/flexidata/utils/
--rw-rw-rw-   0        0        0        0 2024-05-02 06:00:39.000000 flexidata-0.0.1/flexidata/utils/__init__.py
--rw-rw-rw-   0        0        0      266 2024-05-11 09:04:55.000000 flexidata-0.0.1/flexidata/utils/common.py
--rw-rw-rw-   0        0        0     2001 2024-05-11 14:11:32.000000 flexidata-0.0.1/flexidata/utils/constants.py
--rw-rw-rw-   0        0        0     4740 2024-05-05 14:05:40.000000 flexidata-0.0.1/flexidata/utils/pdf.py
--rw-rw-rw-   0        0        0    10010 2024-05-08 18:00:49.000000 flexidata-0.0.1/flexidata/utils/text.py
-drwxrwxrwx   0        0        0        0 2024-05-17 18:26:04.536237 flexidata-0.0.1/flexidata.egg-info/
--rw-rw-rw-   0        0        0    15381 2024-05-17 18:26:04.000000 flexidata-0.0.1/flexidata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      562 2024-05-17 18:26:04.000000 flexidata-0.0.1/flexidata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 18:26:04.000000 flexidata-0.0.1/flexidata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      424 2024-05-17 18:26:04.000000 flexidata-0.0.1/flexidata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-17 18:26:04.000000 flexidata-0.0.1/flexidata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      800 2024-05-17 18:17:28.000000 flexidata-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      467 2024-05-13 16:14:08.000000 flexidata-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 18:26:04.540242 flexidata-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      360 2024-05-17 18:24:25.000000 flexidata-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 18:26:04.535270 flexidata-0.0.1/tests/
--rw-rw-rw-   0        0        0     2724 2024-05-13 09:24:41.000000 flexidata-0.0.1/tests/test_pdf.py
+drwxrwxrwx   0        0        0        0 2024-05-18 19:51:11.895890 flexidata-0.0.2/
+-rw-rw-rw-   0        0        0    11558 2024-05-01 19:03:09.000000 flexidata-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       26 2024-05-17 18:22:13.000000 flexidata-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    15381 2024-05-18 19:51:11.894770 flexidata-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      766 2024-05-17 13:37:32.000000 flexidata-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 19:51:11.820452 flexidata-0.0.2/flexidata/
+-rw-rw-rw-   0        0        0     1838 2024-05-05 15:00:12.000000 flexidata-0.0.2/flexidata/Logger.py
+-rw-rw-rw-   0        0        0        0 2024-05-02 08:52:21.000000 flexidata-0.0.2/flexidata/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 19:51:11.863612 flexidata-0.0.2/flexidata/models/
+-rw-rw-rw-   0        0        0        0 2024-05-02 06:01:08.000000 flexidata-0.0.2/flexidata/models/__init__.py
+-rw-rw-rw-   0        0        0      562 2024-05-02 08:41:23.000000 flexidata-0.0.2/flexidata/models/base.py
+-rw-rw-rw-   0        0        0     3117 2024-05-02 08:39:53.000000 flexidata-0.0.2/flexidata/models/detectron2.py
+drwxrwxrwx   0        0        0        0 2024-05-18 19:51:11.867213 flexidata-0.0.2/flexidata/ocr/
+-rw-rw-rw-   0        0        0        0 2024-05-18 19:45:25.000000 flexidata-0.0.2/flexidata/ocr/__init__.py
+-rw-rw-rw-   0        0        0     1804 2024-05-11 18:01:28.000000 flexidata-0.0.2/flexidata/ocr/agent.py
+-rw-rw-rw-   0        0        0     1354 2024-05-13 16:13:08.000000 flexidata-0.0.2/flexidata/ocr/google_vision.py
+-rw-rw-rw-   0        0        0     5193 2024-05-12 07:05:47.000000 flexidata-0.0.2/flexidata/ocr/paddle.py
+-rw-rw-rw-   0        0        0     1739 2024-05-11 16:52:17.000000 flexidata-0.0.2/flexidata/ocr/tesseract.py
+drwxrwxrwx   0        0        0        0 2024-05-18 19:51:11.867213 flexidata-0.0.2/flexidata/parser/
+-rw-rw-rw-   0        0        0        0 2024-05-02 06:00:51.000000 flexidata-0.0.2/flexidata/parser/__init__.py
+-rw-rw-rw-   0        0        0    21772 2024-05-17 12:54:03.000000 flexidata-0.0.2/flexidata/parser/pdf.py
+drwxrwxrwx   0        0        0        0 2024-05-18 19:51:11.883998 flexidata-0.0.2/flexidata/reader/
+-rw-rw-rw-   0        0        0        0 2024-05-18 19:45:52.000000 flexidata-0.0.2/flexidata/reader/__init__.py
+-rw-rw-rw-   0        0        0      749 2024-05-10 16:16:39.000000 flexidata-0.0.2/flexidata/reader/factory.py
+-rw-rw-rw-   0        0        0      311 2024-05-10 16:10:37.000000 flexidata-0.0.2/flexidata/reader/file_reader.py
+-rw-rw-rw-   0        0        0      965 2024-05-10 16:16:34.000000 flexidata-0.0.2/flexidata/reader/google_drive.py
+-rw-rw-rw-   0        0        0      804 2024-05-10 16:16:29.000000 flexidata-0.0.2/flexidata/reader/local.py
+-rw-rw-rw-   0        0        0     1112 2024-05-10 16:16:24.000000 flexidata-0.0.2/flexidata/reader/s3.py
+-rw-rw-rw-   0        0        0      930 2024-05-10 16:16:14.000000 flexidata-0.0.2/flexidata/reader/web.py
+drwxrwxrwx   0        0        0        0 2024-05-18 19:51:11.891548 flexidata-0.0.2/flexidata/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-02 06:00:39.000000 flexidata-0.0.2/flexidata/utils/__init__.py
+-rw-rw-rw-   0        0        0      266 2024-05-11 09:04:55.000000 flexidata-0.0.2/flexidata/utils/common.py
+-rw-rw-rw-   0        0        0     2001 2024-05-11 14:11:32.000000 flexidata-0.0.2/flexidata/utils/constants.py
+-rw-rw-rw-   0        0        0     4740 2024-05-05 14:05:40.000000 flexidata-0.0.2/flexidata/utils/pdf.py
+-rw-rw-rw-   0        0        0    10010 2024-05-08 18:00:49.000000 flexidata-0.0.2/flexidata/utils/text.py
+drwxrwxrwx   0        0        0        0 2024-05-18 19:51:11.893641 flexidata-0.0.2/flexidata.egg-info/
+-rw-rw-rw-   0        0        0    15381 2024-05-18 19:51:11.000000 flexidata-0.0.2/flexidata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      888 2024-05-18 19:51:11.000000 flexidata-0.0.2/flexidata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 19:51:11.000000 flexidata-0.0.2/flexidata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      424 2024-05-18 19:51:11.000000 flexidata-0.0.2/flexidata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-18 19:51:11.000000 flexidata-0.0.2/flexidata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      800 2024-05-18 19:50:21.000000 flexidata-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      467 2024-05-13 16:14:08.000000 flexidata-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 19:51:11.896424 flexidata-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      360 2024-05-17 18:24:25.000000 flexidata-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 19:51:11.892071 flexidata-0.0.2/tests/
+-rw-rw-rw-   0        0        0     2724 2024-05-13 09:24:41.000000 flexidata-0.0.2/tests/test_pdf.py
```

### Comparing `flexidata-0.0.1/LICENSE` & `flexidata-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.1/PKG-INFO` & `flexidata-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexidata
-Version: 0.0.1
+Version: 0.0.2
 Summary: FlexiData is an open-source Python package designed for processing unstructured data.
 Author-email: Kalyanakannan Padivasu <Kalyanakannan.p@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -201,16 +201,16 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
-Project-URL: Homepage, https://github.com/kalyanakannan/flexidata
-Project-URL: Issues, https://github.com/kalyanakannan/flexidata/issues
+Project-URL: Homepage, https://github.com/flexidatalabs/flexidata
+Project-URL: Issues, https://github.com/flexidatalabs/flexidata/issues
 Keywords: PDF,DOCX document parsing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `flexidata-0.0.1/README.md` & `flexidata-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.1/flexidata/Logger.py` & `flexidata-0.0.2/flexidata/Logger.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.1/flexidata/models/base.py` & `flexidata-0.0.2/flexidata/models/base.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.1/flexidata/models/detectron2.py` & `flexidata-0.0.2/flexidata/models/detectron2.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.1/flexidata/parser/pdf.py` & `flexidata-0.0.2/flexidata/parser/pdf.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.1/flexidata/utils/constants.py` & `flexidata-0.0.2/flexidata/utils/constants.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.1/flexidata/utils/pdf.py` & `flexidata-0.0.2/flexidata/utils/pdf.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.1/flexidata/utils/text.py` & `flexidata-0.0.2/flexidata/utils/text.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.1/flexidata.egg-info/PKG-INFO` & `flexidata-0.0.2/flexidata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexidata
-Version: 0.0.1
+Version: 0.0.2
 Summary: FlexiData is an open-source Python package designed for processing unstructured data.
 Author-email: Kalyanakannan Padivasu <Kalyanakannan.p@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -201,16 +201,16 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
-Project-URL: Homepage, https://github.com/kalyanakannan/flexidata
-Project-URL: Issues, https://github.com/kalyanakannan/flexidata/issues
+Project-URL: Homepage, https://github.com/flexidatalabs/flexidata
+Project-URL: Issues, https://github.com/flexidatalabs/flexidata/issues
 Keywords: PDF,DOCX document parsing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `flexidata-0.0.1/pyproject.toml` & `flexidata-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "flexidata"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Kalyanakannan Padivasu", email="Kalyanakannan.p@gmail.com" },
 ]
 description = "FlexiData is an open-source Python package designed for processing unstructured data."
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["PDF,DOCX document parsing"]
@@ -14,13 +14,13 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-Homepage = "https://github.com/kalyanakannan/flexidata"
-Issues = "https://github.com/kalyanakannan/flexidata/issues"
+Homepage = "https://github.com/flexidatalabs/flexidata"
+Issues = "https://github.com/flexidatalabs/flexidata/issues"
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `flexidata-0.0.1/tests/test_pdf.py` & `flexidata-0.0.2/tests/test_pdf.py`

 * *Files identical despite different names*

