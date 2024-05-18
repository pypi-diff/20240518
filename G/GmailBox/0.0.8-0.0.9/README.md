# Comparing `tmp/gmailbox-0.0.8.tar.gz` & `tmp/gmailbox-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmailbox-0.0.8.tar", last modified: Tue May  7 17:58:21 2024, max compression
+gzip compressed data, was "gmailbox-0.0.9.tar", last modified: Sat May 18 18:23:37 2024, max compression
```

## Comparing `gmailbox-0.0.8.tar` & `gmailbox-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 17:58:21.682180 gmailbox-0.0.8/
-drwxrwxrwx   0        0        0        0 2024-05-07 17:58:21.653319 gmailbox-0.0.8/GmailBox/
--rw-rw-rw-   0        0        0     2328 2024-05-07 17:54:52.000000 gmailbox-0.0.8/GmailBox/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 17:58:21.680184 gmailbox-0.0.8/GmailBox.egg-info/
--rw-rw-rw-   0        0        0     1480 2024-05-07 17:58:21.000000 gmailbox-0.0.8/GmailBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2024-05-07 17:58:21.000000 gmailbox-0.0.8/GmailBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 17:58:21.000000 gmailbox-0.0.8/GmailBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-07 17:58:21.000000 gmailbox-0.0.8/GmailBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-07 17:58:21.000000 gmailbox-0.0.8/GmailBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1480 2024-05-07 17:58:21.681182 gmailbox-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      839 2024-05-07 08:29:09.000000 gmailbox-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-05-07 17:58:21.682180 gmailbox-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      828 2024-05-07 17:57:50.000000 gmailbox-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:23:37.357515 gmailbox-0.0.9/
+drwxrwxrwx   0        0        0        0 2024-05-18 18:23:37.283854 gmailbox-0.0.9/GmailBox/
+-rw-rw-rw-   0        0        0     2818 2024-05-18 15:32:27.000000 gmailbox-0.0.9/GmailBox/__init__.py
+-rw-rw-rw-   0        0        0     1547 2024-05-18 15:26:09.000000 gmailbox-0.0.9/GmailBox/async_session.py
+-rw-rw-rw-   0        0        0     3047 2024-05-18 15:26:09.000000 gmailbox-0.0.9/GmailBox/asyncio.py
+-rw-rw-rw-   0        0        0     1472 2024-05-18 11:56:16.000000 gmailbox-0.0.9/GmailBox/session.py
+-rw-rw-rw-   0        0        0     1090 2024-05-18 11:34:05.000000 gmailbox-0.0.9/GmailBox/types.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:23:37.357515 gmailbox-0.0.9/GmailBox.egg-info/
+-rw-rw-rw-   0        0        0     2474 2024-05-18 18:23:37.000000 gmailbox-0.0.9/GmailBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-18 18:23:37.000000 gmailbox-0.0.9/GmailBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 18:23:37.000000 gmailbox-0.0.9/GmailBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-18 18:23:37.000000 gmailbox-0.0.9/GmailBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-18 18:23:37.000000 gmailbox-0.0.9/GmailBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2474 2024-05-18 18:23:37.357515 gmailbox-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1746 2024-05-18 17:54:48.000000 gmailbox-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-18 18:23:37.357515 gmailbox-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      848 2024-05-18 16:27:59.000000 gmailbox-0.0.9/setup.py
```

### Comparing `gmailbox-0.0.8/GmailBox/__init__.py` & `gmailbox-0.0.9/GmailBox/asyncio.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,70 @@
-import time
 import re
-import requests
 from bs4 import BeautifulSoup
 from urllib.parse import unquote
-from typing import Optional, Dict, Any
+from typing import Optional, List
+from.types import new_emailResult,inboxResult
+import asyncio
+from .async_session import make_request,session_manager
+
+
+__all__ = ["GmailBox"]
+
 
 class GmailBox:
     def __init__(self):
-        self.request = requests.session()
         self.headers = {
             'Pragma': 'no-cache',
             'Accept': '*/*',
             'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36',
         }
-        self.request.get('https://www.emailnator.com/', headers=self.headers)
-        self.token = unquote(self.request.cookies.get_dict()['XSRF-TOKEN'])
-        self.headers["x-xsrf-token"] = self.token
+        self.token = None
         self.email = ""
 
-    def new_email(self) -> Dict[str, str]:
+    async def new_email(self) -> "new_emailResult":
+        req = await make_request('https://www.emailnator.com/', method='get', headers=self.headers, response_type='cookies')
+        self.token = unquote(req['XSRF-TOKEN'])
+        self.headers["x-xsrf-token"] = self.token
         json_data = {'email': ['dotGmail']}
-        response = self.request.post('https://www.emailnator.com/generate-email', headers=self.headers, json=json_data).json()
+        response = await make_request('https://www.emailnator.com/generate-email', method='post', headers=self.headers, json=json_data, response_type='json')
         self.email = response['email'][0]
-        return {'email': self.email}
+        return new_emailResult.parse(self.email)
 
-    def inbox(self, email: Optional[str] = None) -> Dict[str, Any]:
+    async def inbox(self, email: Optional[str] = None, limit: int = None) -> List[inboxResult]:  
+        req = await make_request('https://www.emailnator.com/', method='get', headers=self.headers, response_type='cookies')
+        self.token = unquote(req['XSRF-TOKEN'])
+        self.headers["x-xsrf-token"] = self.token
         email = email or self.email
-        time.sleep(0.20)
+        await asyncio.sleep(0.5)
         json_data = {'email': email}
-        response = self.request.post('https://www.emailnator.com/message-list', headers=self.headers, json=json_data).json()
+        response = await make_request('https://www.emailnator.com/message-list', method='post', headers=self.headers, json=json_data, response_type='json')
+        
         messages = []
-        for item in response['messageData'][1:]:
+        for item in response.get('messageData', [])[1:]:
+            if limit is not None and len(messages) == limit:
+                break
             messageID = item['messageID']
             json_data = {'email': email, 'messageID': messageID}
-            response = self.request.post('https://www.emailnator.com/message-list', headers=self.headers, json=json_data).text
+            response = await make_request('https://www.emailnator.com/message-list', method='post', headers=self.headers, json=json_data, response_type='text')
             soup = BeautifulSoup(response, 'html.parser')
             message = soup.text.strip()
             try:
-                tim, message = re.search(r"Time:\s*\n\s*\n(.+?)([\s\S]+)", message).groups()
-            except:
-                pass
+                time_part, message = re.search(r"Time:\s*\n\s*\n(.+?)([\s\S]+)", message).groups()
+            except AttributeError:
+                time_part = "Unknown"
+            
             sender = item['from']
-            email_sender = re.findall(r'<(.*?)>', sender)[0] if re.findall(r'<(.*?)>', sender) else sender
-            sender_name = re.findall(r'"(.*?)"', sender)[0] if re.findall(r'"(.*?)"', sender) else sender.split(f'<{email_sender}>')[0]
-            messages.append({'from': sender_name, 'email': email_sender, 'subject': item['subject'], 'message': message.strip(), 'time': item['time']})
-        return messages
+            messages.append(inboxResult.parse({
+                'sender': sender,
+                'html': response,
+                'subject': item['subject'],
+                'message': message.strip(),
+                'time': item.get('time', time_part)
+            }))
+        return messages
+
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, *args):
+        session = await session_manager.get_session()
+        await session.close()
```

### Comparing `gmailbox-0.0.8/setup.py` & `gmailbox-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
 	name= "GmailBox",
-	version= "0.0.8",
+	version= "0.0.9",
 	author= "Hamo",
     keywords=["gmail","mail","GmailBox","inbox","email","Tempmail","Tempgmail"],
-    install_requires=['requests','beautifulsoup4'],
+    install_requires=['requests','beautifulsoup4',"aiohttp","asyncio"],
     long_description=readme,
     long_description_content_type="text/markdown",
 	description= "With this library, you can create random Gmail and receive messages",
 	packages=setuptools.find_packages(),
     license="LGPLv3",
 	classifiers=[
         "Development Status :: 3 - Alpha",
```

