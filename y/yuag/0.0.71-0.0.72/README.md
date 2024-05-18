# Comparing `tmp/yuag-0.0.71.tar.gz` & `tmp/yuag-0.0.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuag-0.0.71.tar", last modified: Tue May 14 12:01:37 2024, max compression
+gzip compressed data, was "yuag-0.0.72.tar", last modified: Sat May 18 14:47:58 2024, max compression
```

## Comparing `yuag-0.0.71.tar` & `yuag-0.0.72.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 12:01:37.300864 yuag-0.0.71/
--rw-rw-rw-   0        0        0       52 2024-05-14 12:01:37.298867 yuag-0.0.71/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-14 12:01:37.300864 yuag-0.0.71/setup.cfg
--rw-rw-rw-   0        0        0      249 2024-05-14 11:50:18.000000 yuag-0.0.71/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 12:01:37.283172 yuag-0.0.71/yuag/
--rw-rw-rw-   0        0        0     2873 2024-05-13 11:58:51.000000 yuag-0.0.71/yuag/__init__.py
--rw-rw-rw-   0        0        0    44696 2024-05-14 11:50:05.000000 yuag-0.0.71/yuag/yuag.py
-drwxrwxrwx   0        0        0        0 2024-05-14 12:01:37.296866 yuag-0.0.71/yuag.egg-info/
--rw-rw-rw-   0        0        0       52 2024-05-14 12:01:37.000000 yuag-0.0.71/yuag.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2024-05-14 12:01:37.000000 yuag-0.0.71/yuag.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 12:01:37.000000 yuag-0.0.71/yuag.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-14 12:01:37.000000 yuag-0.0.71/yuag.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 14:47:58.551272 yuag-0.0.72/
+-rw-rw-rw-   0        0        0       52 2024-05-18 14:47:58.549275 yuag-0.0.72/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-18 14:47:58.551272 yuag-0.0.72/setup.cfg
+-rw-rw-rw-   0        0        0      249 2024-05-18 14:43:42.000000 yuag-0.0.72/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:47:58.522286 yuag-0.0.72/yuag/
+-rw-rw-rw-   0        0        0     2963 2024-05-18 14:47:11.000000 yuag-0.0.72/yuag/__init__.py
+-rw-rw-rw-   0        0        0    45590 2024-05-18 14:46:18.000000 yuag-0.0.72/yuag/yuag.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:47:58.548275 yuag-0.0.72/yuag.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-05-18 14:47:58.000000 yuag-0.0.72/yuag.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2024-05-18 14:47:58.000000 yuag-0.0.72/yuag.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 14:47:58.000000 yuag-0.0.72/yuag.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-18 14:47:58.000000 yuag-0.0.72/yuag.egg-info/top_level.txt
```

### Comparing `yuag-0.0.71/yuag/__init__.py` & `yuag-0.0.72/yuag/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
 ```
 \n\n
 
 دوال للأرقام:
 -----------------
 ```
 makeZeroNum()
+toTime()
 ```
 \n\n
 
 دوال التقسيم:
 -----------------
 ```
 separate_text()
@@ -200,14 +201,21 @@
 ```
 imageLink_to_dataurl()
 imageFile_to_dataurl()
 videoFile_to_dataurl()
 ```
 \n\n
 
+دوال اليوتيوب:
+-----------------
+```
+video_trans()
+```
+\n\n
+
 رسالة الإنتهاء:
 -----------------
 ```
 doneMessage()
 ```
 """
```

### Comparing `yuag-0.0.71/yuag/yuag.py` & `yuag-0.0.72/yuag/yuag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1157,14 +1157,31 @@
     num = str(num)
     if cells_num > len(num):
         for item in rangeNum(cells_num - len(num)):
             num = zero + num
     
     return num
 
+def toTime(seconds: int):
+    """
+    اللهم صل على سيدنا محمد\n
+    تحويل الثواني لوقت مقسم\n
+
+    ```
+    640 ==> "00:10:40"
+    ```
+    """
+    
+    hours = seconds // 3600
+    remaining_seconds = seconds % 3600
+    minutes = remaining_seconds // 60
+    remaining_seconds = remaining_seconds % 60
+    
+    return f"{hours:02}:{minutes:02}:{remaining_seconds:02}"
+
 # separate defs
 def separate_text(text: str, splitter: list = ["."], joiner: str = "\n", stripping: bool = False, delete_splitter: bool = False): # "line1.line2" ==> "line1.\nline2"
     """
     اللهم صل على سيدنا محمد ﷺ\n
     
     ```
     text = "line1.line2"
@@ -1445,15 +1462,15 @@
 
 # chatGPT
 def chatGPT(user_question: str, api_key: str):
     import openai
 
     openai.api_key = api_key
 
-    response = openai.ChatCompletion.create(
+    response = openai.completions.create(
         model = "gpt-3.5-turbo",
         messages = [
             {
                 "role": "user",
                 "content": user_question
             }
         ]
@@ -1563,11 +1580,25 @@
         # إنشاء Data URL
         data_url = "data:video/mp4;base64," + video_base64.decode('utf-8')
 
         return data_url
     except:
         return error
 
+# youtube
+def video_trans(video_id: str, languages: list = ["ar"]) -> list:
+    """
+    اللهم صل على سيدنا محمد\n
+    دالة لإرجاع ترجمة المقطع على يوتيوب\n\n
+
+    ```
+    ==> [ {"text": "أهلا بكم", "duration": 1.2, "start": 0} ]
+    ```
+    """
+    from youtube_transcript_api import YouTubeTranscriptApi
+    
+    return YouTubeTranscriptApi.list_transcripts(video_id).find_transcript(languages).fetch()
+
 # done message
 def doneMessage(want_clear: int = 1):
     if want_clear > 0: clear()
     print("Done.. Alhamdulillah")
```

