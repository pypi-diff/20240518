# Comparing `tmp/autilsy-0.1.3.1.tar.gz` & `tmp/autilsy-0.1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autilsy-0.1.3.1.tar", last modified: Thu Apr 18 14:12:07 2024, max compression
+gzip compressed data, was "autilsy-0.1.3.2.tar", last modified: Sat May 18 01:48:02 2024, max compression
```

## Comparing `autilsy-0.1.3.1.tar` & `autilsy-0.1.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-04-18 14:12:07.381859 autilsy-0.1.3.1/
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)      176 2024-04-18 14:12:07.381859 autilsy-0.1.3.1/PKG-INFO
-drwxrwxr-x   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-04-18 14:12:07.377859 autilsy-0.1.3.1/autilsy/
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-03-17 09:58:08.000000 autilsy-0.1.3.1/autilsy/__init__.py
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)     2790 2024-03-24 08:13:18.000000 autilsy-0.1.3.1/autilsy/annots.py
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)    22376 2024-04-18 14:09:17.000000 autilsy-0.1.3.1/autilsy/common.py
-drwxrwxr-x   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-04-18 14:12:07.377859 autilsy-0.1.3.1/autilsy/resource/
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-04-04 13:46:33.000000 autilsy-0.1.3.1/autilsy/resource/__init__.py
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)   705306 2024-04-04 13:46:33.000000 autilsy-0.1.3.1/autilsy/resource/image_bytes.py
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)     9995 2024-04-04 14:04:14.000000 autilsy-0.1.3.1/autilsy/ui.py
-drwxrwxr-x   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-04-18 14:12:07.377859 autilsy-0.1.3.1/autilsy.egg-info/
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)      176 2024-04-18 14:12:06.000000 autilsy-0.1.3.1/autilsy.egg-info/PKG-INFO
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)      293 2024-04-18 14:12:07.000000 autilsy-0.1.3.1/autilsy.egg-info/SOURCES.txt
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)        1 2024-04-18 14:12:06.000000 autilsy-0.1.3.1/autilsy.egg-info/dependency_links.txt
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)      121 2024-04-18 14:12:06.000000 autilsy-0.1.3.1/autilsy.egg-info/requires.txt
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)        8 2024-04-18 14:12:07.000000 autilsy-0.1.3.1/autilsy.egg-info/top_level.txt
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)       38 2024-04-18 14:12:07.381859 autilsy-0.1.3.1/setup.cfg
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)      416 2024-04-18 14:11:55.000000 autilsy-0.1.3.1/setup.py
+drwxrwxr-x   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-05-18 01:48:02.942638 autilsy-0.1.3.2/
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)      176 2024-05-18 01:48:02.942638 autilsy-0.1.3.2/PKG-INFO
+drwxrwxr-x   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-05-18 01:48:02.942638 autilsy-0.1.3.2/autilsy/
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-03-17 09:58:08.000000 autilsy-0.1.3.2/autilsy/__init__.py
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)     2790 2024-03-24 08:13:18.000000 autilsy-0.1.3.2/autilsy/annots.py
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)    22273 2024-05-18 01:43:20.000000 autilsy-0.1.3.2/autilsy/common.py
+drwxrwxr-x   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-05-18 01:48:02.942638 autilsy-0.1.3.2/autilsy/resource/
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-04-04 13:46:33.000000 autilsy-0.1.3.2/autilsy/resource/__init__.py
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)   705306 2024-04-04 13:46:33.000000 autilsy-0.1.3.2/autilsy/resource/image_bytes.py
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)     9995 2024-04-04 14:04:14.000000 autilsy-0.1.3.2/autilsy/ui.py
+drwxrwxr-x   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-05-18 01:48:02.942638 autilsy-0.1.3.2/autilsy.egg-info/
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)      176 2024-05-18 01:48:02.000000 autilsy-0.1.3.2/autilsy.egg-info/PKG-INFO
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)      293 2024-05-18 01:48:02.000000 autilsy-0.1.3.2/autilsy.egg-info/SOURCES.txt
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)        1 2024-05-18 01:48:02.000000 autilsy-0.1.3.2/autilsy.egg-info/dependency_links.txt
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)       97 2024-05-18 01:48:02.000000 autilsy-0.1.3.2/autilsy.egg-info/requires.txt
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)        8 2024-05-18 01:48:02.000000 autilsy-0.1.3.2/autilsy.egg-info/top_level.txt
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)       38 2024-05-18 01:48:02.942638 autilsy-0.1.3.2/setup.cfg
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)      386 2024-05-18 01:46:01.000000 autilsy-0.1.3.2/setup.py
```

### Comparing `autilsy-0.1.3.1/autilsy/annots.py` & `autilsy-0.1.3.2/autilsy/annots.py`

 * *Files identical despite different names*

### Comparing `autilsy-0.1.3.1/autilsy/common.py` & `autilsy-0.1.3.2/autilsy/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -588,16 +588,15 @@
             text_size: text size.
         return:
             numpy array image.
         """
         if isinstance(img, np.ndarray):
             img = Image.fromarray(cv2.cvtColor(img, cv2.COLOR_BGR2RGB))
         draw = ImageDraw.Draw(img)
-        font_path = os.path.join(os.path.dirname(__file__), "font/simsun.ttc") 
-        font = ImageFont.truetype(font_path, text_size, encoding='utf-8')
+        font = ImageFont.truetype("simsun.ttc", text_size, encoding='utf-8')
         draw.text(pos, text, color, font=font)
 
         return cv2.cvtColor(np.array(img), cv2.COLOR_RGB2BGR)
 
     def RandColor(self,)->tuple:
         """
         return:
@@ -691,9 +690,8 @@
                 break
             else:
                 print("Invalid key!")
                 continue
 
 if __name__ == "__main__":
     autil = Autils()
-    autil.ReadYMLFile("")
```

### Comparing `autilsy-0.1.3.1/autilsy/resource/image_bytes.py` & `autilsy-0.1.3.2/autilsy/resource/image_bytes.py`

 * *Files identical despite different names*

### Comparing `autilsy-0.1.3.1/autilsy/ui.py` & `autilsy-0.1.3.2/autilsy/ui.py`

 * *Files identical despite different names*

