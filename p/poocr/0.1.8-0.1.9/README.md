# Comparing `tmp/poocr-0.1.8.tar.gz` & `tmp/poocr-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poocr-0.1.8.tar", last modified: Wed May  8 13:40:31 2024, max compression
+gzip compressed data, was "poocr-0.1.9.tar", last modified: Wed May 15 16:14:59 2024, max compression
```

## Comparing `poocr-0.1.8.tar` & `poocr-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 13:40:31.609313 poocr-0.1.8/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poocr-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     3823 2024-05-08 13:40:31.608308 poocr-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3145 2024-04-30 17:27:09.000000 poocr-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 13:40:31.528763 poocr-0.1.8/poocr/
--rw-rw-rw-   0        0        0      810 2024-02-26 13:41:46.000000 poocr-0.1.8/poocr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:40:31.576783 poocr-0.1.8/poocr/api/
--rw-rw-rw-   0        0        0      265 2023-03-25 11:08:27.000000 poocr-0.1.8/poocr/api/__init__.py
--rw-rw-rw-   0        0        0    25370 2024-05-06 13:35:11.000000 poocr-0.1.8/poocr/api/ocr.py
--rw-rw-rw-   0        0        0     9452 2024-05-08 13:38:46.000000 poocr-0.1.8/poocr/api/ocr2excel.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:40:31.585307 poocr-0.1.8/poocr/core/
--rw-rw-rw-   0        0        0     1815 2024-05-06 13:38:21.000000 poocr-0.1.8/poocr/core/BaiduOCR.py
--rw-rw-rw-   0        0        0     4271 2023-07-25 15:06:57.000000 poocr-0.1.8/poocr/core/OCR.py
--rw-rw-rw-   0        0        0      223 2023-01-22 06:56:13.000000 poocr-0.1.8/poocr/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:40:31.598303 poocr-0.1.8/poocr/lib/
--rw-rw-rw-   0        0        0     1017 2023-01-28 13:49:56.000000 poocr-0.1.8/poocr/lib/CommonUtils.py
--rw-rw-rw-   0        0        0     1132 2023-01-30 12:39:04.000000 poocr-0.1.8/poocr/lib/Config.py
--rw-rw-rw-   0        0        0      852 2023-01-30 12:39:04.000000 poocr-0.1.8/poocr/lib/Const.py
--rw-rw-rw-   0        0        0        0 2023-01-22 10:20:33.000000 poocr-0.1.8/poocr/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:40:31.606305 poocr-0.1.8/poocr.egg-info/
--rw-rw-rw-   0        0        0     3823 2024-05-08 13:40:31.000000 poocr-0.1.8/poocr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      478 2024-05-08 13:40:31.000000 poocr-0.1.8/poocr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 13:40:31.000000 poocr-0.1.8/poocr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-22 14:21:59.000000 poocr-0.1.8/poocr.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       61 2024-05-08 13:40:31.000000 poocr-0.1.8/poocr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-08 13:40:31.000000 poocr-0.1.8/poocr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      759 2024-05-08 13:40:31.618304 poocr-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poocr-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:40:31.603306 poocr-0.1.8/tests/
--rw-rw-rw-   0        0        0      181 2023-01-30 12:39:04.000000 poocr-0.1.8/tests/__init__.py
--rw-rw-rw-   0        0        0     1150 2024-04-30 17:30:56.000000 poocr-0.1.8/tests/test_tencent.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:14:59.985936 poocr-0.1.9/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poocr-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     3823 2024-05-15 16:14:59.984943 poocr-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3145 2024-04-30 17:27:09.000000 poocr-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 16:14:59.875597 poocr-0.1.9/poocr/
+-rw-rw-rw-   0        0        0      810 2024-02-26 13:41:46.000000 poocr-0.1.9/poocr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:14:59.938137 poocr-0.1.9/poocr/api/
+-rw-rw-rw-   0        0        0      265 2023-03-25 11:08:27.000000 poocr-0.1.9/poocr/api/__init__.py
+-rw-rw-rw-   0        0        0    25712 2024-05-08 14:09:00.000000 poocr-0.1.9/poocr/api/ocr.py
+-rw-rw-rw-   0        0        0     9635 2024-05-08 16:40:05.000000 poocr-0.1.9/poocr/api/ocr2excel.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:14:59.952287 poocr-0.1.9/poocr/core/
+-rw-rw-rw-   0        0        0     1815 2024-05-06 13:38:21.000000 poocr-0.1.9/poocr/core/BaiduOCR.py
+-rw-rw-rw-   0        0        0     4312 2024-05-08 14:08:31.000000 poocr-0.1.9/poocr/core/OCR.py
+-rw-rw-rw-   0        0        0      223 2023-01-22 06:56:13.000000 poocr-0.1.9/poocr/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:14:59.969467 poocr-0.1.9/poocr/lib/
+-rw-rw-rw-   0        0        0     1017 2023-01-28 13:49:56.000000 poocr-0.1.9/poocr/lib/CommonUtils.py
+-rw-rw-rw-   0        0        0     1132 2023-01-30 12:39:04.000000 poocr-0.1.9/poocr/lib/Config.py
+-rw-rw-rw-   0        0        0      852 2023-01-30 12:39:04.000000 poocr-0.1.9/poocr/lib/Const.py
+-rw-rw-rw-   0        0        0        0 2023-01-22 10:20:33.000000 poocr-0.1.9/poocr/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:14:59.982754 poocr-0.1.9/poocr.egg-info/
+-rw-rw-rw-   0        0        0     3823 2024-05-15 16:14:59.000000 poocr-0.1.9/poocr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2024-05-15 16:14:59.000000 poocr-0.1.9/poocr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 16:14:59.000000 poocr-0.1.9/poocr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-22 14:21:59.000000 poocr-0.1.9/poocr.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       61 2024-05-15 16:14:59.000000 poocr-0.1.9/poocr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-15 16:14:59.000000 poocr-0.1.9/poocr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      759 2024-05-15 16:14:59.989932 poocr-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poocr-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:14:59.977750 poocr-0.1.9/tests/
+-rw-rw-rw-   0        0        0      181 2023-01-30 12:39:04.000000 poocr-0.1.9/tests/__init__.py
+-rw-rw-rw-   0        0        0     1150 2024-04-30 17:30:56.000000 poocr-0.1.9/tests/test_tencent.py
```

### Comparing `poocr-0.1.8/LICENSE` & `poocr-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `poocr-0.1.8/PKG-INFO` & `poocr-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poocr
-Version: 0.1.8
+Version: 0.1.9
 Summary: pip install poocr
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poocr/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poocr/blob/main/README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poocr Version: 0.1.8 Summary: pip install poocr
+Metadata-Version: 2.1 Name: poocr Version: 0.1.9 Summary: pip install poocr
 Home-page: https://www.python-office.com/ Author: CoderWanFeng Author-email:
 1957875073@qq.com License: MIT Project-URL: Bug Tracker, https://github.com/
 CoderWanFeng/poocr/issues Project-URL: Documentation, https://github.com/
 CoderWanFeng/poocr/blob/main/README.md Project-URL: Source Code, https://
 github.com/CoderWanFeng/poocr Platform: any Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: toml Requires-
 Dist: tencentcloud-sdk-python Requires-Dist: poprogress Requires-Dist: pofile
```

### Comparing `poocr-0.1.8/README.md` & `poocr-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `poocr-0.1.8/poocr/__init__.py` & `poocr-0.1.9/poocr/__init__.py`

 * *Files identical despite different names*

### Comparing `poocr-0.1.8/poocr/api/ocr.py` & `poocr-0.1.9/poocr/api/ocr.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,35 +2,40 @@
 '''
 @Author  ：程序员晚枫，B站/抖音/微博/小红书/公众号
 @WeChat     ：CoderWanFeng
 @Blog      ：www.python-office.com
 @Date    ：2023/1/22 15:23
 @Description     ：
 '''
-
+import base64
 import sys
 
 from poocr.core.BaiduOCR import BaiduOCR
 from poocr.core.OCR import OCR
 from poocr.lib.CommonUtils import img2base64
 
 
 def get_ocr(configPath, id, key):
     ocr = OCR()
     ocr.set_config(configPath, id, key)
     return ocr
 
 
-def do_api(OCR_NAME, img_path, img_url, configPath, id, key):
+def do_api(OCR_NAME, img_path, img_url, configPath, id, key,pdf_path=None):
     """
     通过类的方法名，直接调用方法
     :return:
     """
     ocr = get_ocr(configPath, id, key)
-    if img_url:
+    if pdf_path:
+        with open(pdf_path, 'rb') as file:
+            pdf_data = file.read()
+            base64_encoded_pdf = base64.b64encode(pdf_data).decode('utf-8')
+            ocr_res = ocr.DoOCR(OCR_NAME, ImageBase64=base64_encoded_pdf, ImageUrl=img_url,IsPdf=True)
+    elif img_url:
         ocr_res = ocr.DoOCR(OCR_NAME, ImageBase64=img_path, ImageUrl=img_url)
     else:
         ImageBase64 = img2base64(img_path)
         ocr_res = ocr.DoOCR(OCR_NAME, ImageBase64=ImageBase64, ImageUrl=img_url)
     return ocr_res
 
 
@@ -550,20 +555,20 @@
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
                   configPath=configPath,
                   id=id, key=key)
 
 
-def VatInvoiceOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
+def VatInvoiceOCR(img_path=None, img_url=None, configPath=None, id=None, key=None, pdf_path=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
                   configPath=configPath,
-                  id=id, key=key)
+                  id=id, key=key, pdf_path=pdf_path)
 
 
 def VatInvoiceVerify(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
                   configPath=configPath,
```

### Comparing `poocr-0.1.8/poocr/api/ocr2excel.py` & `poocr-0.1.9/poocr/api/ocr2excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from poprogress import simple_progress
 
 import poocr
 from poocr.api.ocr import VatInvoiceOCR, IDCardOCR
 
 
 def VatInvoiceOCR2Excel(input_path, output_path=None, output_excel='VatInvoiceOCR2Excel.xlsx', img_url=None,
-                        configPath=None, id=None, key=None, file_name=False, trans=False):
+                        configPath=None, id=None, key=None, file_name=False, trans=False,pdf_path=None):
     """
     批量识别发票，并保存在Excel中
     :param input_path: 发票存放位置，可以填单个文件，也可以填一个目录
     :param output_path:
     :param output_excel:
     :param img_url:
     :param configPath:
@@ -42,15 +42,18 @@
         abs_output_excel = Path(output_path).absolute() / output_excel
     else:  # 指定了，但不是xlsx或者xls结束
         raise BaseException(
             f'输出结果名：output_excel参数，必须以xls或者xlsx结尾，您的输入:{output_excel}有误，请修改后重新运行')
     res_df = []  # 装全部识别的结果
     for vat_img in simple_progress(vat_img_files):
         try:
-            api_res = VatInvoiceOCR(img_path=str(vat_img), img_url=img_url, configPath=configPath, id=id, key=key)
+            if pdf_path:
+                api_res = VatInvoiceOCR(pdf_path=str(vat_img), img_url=img_url, configPath=configPath, id=id, key=key)
+            else:
+                api_res = VatInvoiceOCR(img_path=str(vat_img), img_url=img_url, configPath=configPath, id=id, key=key)
             api_res_json = json.loads(str(api_res))
             VatInvoiceInfos = api_res_json['VatInvoiceInfos']
             dict_pandas = {}  # 存放一行数据
             # 读返回值的第一个key
             beizhu_value = ''
             for VatInvoiceInfo in VatInvoiceInfos:
                 if file_name:
```

### Comparing `poocr-0.1.8/poocr/core/BaiduOCR.py` & `poocr-0.1.9/poocr/core/BaiduOCR.py`

 * *Files identical despite different names*

### Comparing `poocr-0.1.8/poocr/core/OCR.py` & `poocr-0.1.9/poocr/core/OCR.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,21 +57,22 @@
             params = '{\"ImageUrl\":\"%s\"} ' % ImageUrl
         elif ImageBase64:
             params = '{\"ImageBase64\":\"%s\"} ' % ImageBase64
         else:
             return NO_FILE_ERROR
         return params
 
-    def DoOCR(self, OCR_NAME, ImageBase64, ImageUrl):
+    def DoOCR(self, OCR_NAME, ImageBase64, ImageUrl,IsPdf=False):
 
         try:
             ocr_req_func = getattr(models, f'{OCR_NAME}Request', None)
             req = ocr_req_func()
             req.from_json_string(self.get_params(ImageBase64, ImageUrl))
             ocr_func = getattr(self.client, f'{OCR_NAME}', None)
+            req.IsPdf=IsPdf
             resp = ocr_func(req)
             return resp
 
         except TencentCloudSDKException as err:
             print(err)
 
     # def VatInvoiceOCR(self, ImageBase64, ImageUrl):
```

### Comparing `poocr-0.1.8/poocr/lib/CommonUtils.py` & `poocr-0.1.9/poocr/lib/CommonUtils.py`

 * *Files identical despite different names*

### Comparing `poocr-0.1.8/poocr/lib/Config.py` & `poocr-0.1.9/poocr/lib/Config.py`

 * *Files identical despite different names*

### Comparing `poocr-0.1.8/poocr/lib/Const.py` & `poocr-0.1.9/poocr/lib/Const.py`

 * *Files identical despite different names*

### Comparing `poocr-0.1.8/poocr.egg-info/PKG-INFO` & `poocr-0.1.9/poocr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poocr
-Version: 0.1.8
+Version: 0.1.9
 Summary: pip install poocr
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poocr/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poocr/blob/main/README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poocr Version: 0.1.8 Summary: pip install poocr
+Metadata-Version: 2.1 Name: poocr Version: 0.1.9 Summary: pip install poocr
 Home-page: https://www.python-office.com/ Author: CoderWanFeng Author-email:
 1957875073@qq.com License: MIT Project-URL: Bug Tracker, https://github.com/
 CoderWanFeng/poocr/issues Project-URL: Documentation, https://github.com/
 CoderWanFeng/poocr/blob/main/README.md Project-URL: Source Code, https://
 github.com/CoderWanFeng/poocr Platform: any Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: toml Requires-
 Dist: tencentcloud-sdk-python Requires-Dist: poprogress Requires-Dist: pofile
```

### Comparing `poocr-0.1.8/setup.cfg` & `poocr-0.1.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f6f 6372 0d0a 7665 7273 696f   = poocr..versio
-00000020: 6e20 3d20 302e 312e 380d 0a64 6573 6372  n = 0.1.8..descr
+00000020: 6e20 3d20 302e 312e 390d 0a64 6573 6372  n = 0.1.9..descr
 00000030: 6970 7469 6f6e 203d 2070 6970 2069 6e73  iption = pip ins
 00000040: 7461 6c6c 2070 6f6f 6372 0d0a 6c6f 6e67  tall poocr..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
```

### Comparing `poocr-0.1.8/tests/test_tencent.py` & `poocr-0.1.9/tests/test_tencent.py`

 * *Files identical despite different names*

