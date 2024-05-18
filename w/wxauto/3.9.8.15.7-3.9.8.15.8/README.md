# Comparing `tmp/wxauto-3.9.8.15.7.tar.gz` & `tmp/wxauto-3.9.8.15.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wxauto-3.9.8.15.7.tar", last modified: Wed May 15 15:31:45 2024, max compression
+gzip compressed data, was "dist\wxauto-3.9.8.15.8.tar", last modified: Sat May 18 16:06:14 2024, max compression
```

## Comparing `wxauto-3.9.8.15.7.tar` & `wxauto-3.9.8.15.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 15:31:45.000000 wxauto-3.9.8.15.7/
--rw-rw-rw-   0        0        0     3698 2024-05-15 15:31:45.000000 wxauto-3.9.8.15.7/PKG-INFO
--rw-rw-rw-   0        0        0     3333 2024-05-14 06:00:05.000000 wxauto-3.9.8.15.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-15 15:31:45.000000 wxauto-3.9.8.15.7/setup.cfg
--rw-rw-rw-   0        0        0      732 2024-05-15 15:31:27.000000 wxauto-3.9.8.15.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 15:31:45.000000 wxauto-3.9.8.15.7/wxauto/
--rw-rw-rw-   0        0        0      148 2024-05-14 04:47:09.000000 wxauto-3.9.8.15.7/wxauto/__init__.py
--rw-rw-rw-   0        0        0     8728 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.7/wxauto/color.py
--rw-rw-rw-   0        0        0    24103 2024-05-15 12:26:26.000000 wxauto-3.9.8.15.7/wxauto/elements.py
--rw-rw-rw-   0        0        0       49 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.7/wxauto/errors.py
--rw-rw-rw-   0        0        0     5449 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.7/wxauto/languages.py
--rw-rw-rw-   0        0        0   366752 2024-05-14 04:11:30.000000 wxauto-3.9.8.15.7/wxauto/uiautomation.py
--rw-rw-rw-   0        0        0    11545 2024-05-15 12:23:50.000000 wxauto-3.9.8.15.7/wxauto/utils.py
--rw-rw-rw-   0        0        0    29323 2024-05-15 15:31:36.000000 wxauto-3.9.8.15.7/wxauto/wxauto.py
-drwxrwxrwx   0        0        0        0 2024-05-15 15:31:45.000000 wxauto-3.9.8.15.7/wxauto.egg-info/
--rw-rw-rw-   0        0        0     3698 2024-05-15 15:31:44.000000 wxauto-3.9.8.15.7/wxauto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-05-15 15:31:45.000000 wxauto-3.9.8.15.7/wxauto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 15:31:44.000000 wxauto-3.9.8.15.7/wxauto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-05-15 15:31:44.000000 wxauto-3.9.8.15.7/wxauto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-15 15:31:44.000000 wxauto-3.9.8.15.7/wxauto.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 16:06:14.000000 wxauto-3.9.8.15.8/
+-rw-rw-rw-   0        0        0     3698 2024-05-18 16:06:14.000000 wxauto-3.9.8.15.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3333 2024-05-14 06:00:05.000000 wxauto-3.9.8.15.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-18 16:06:14.000000 wxauto-3.9.8.15.8/setup.cfg
+-rw-rw-rw-   0        0        0      786 2024-05-18 16:05:59.000000 wxauto-3.9.8.15.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:06:14.000000 wxauto-3.9.8.15.8/wxauto/
+-rw-rw-rw-   0        0        0      148 2024-05-14 04:47:09.000000 wxauto-3.9.8.15.8/wxauto/__init__.py
+-r--r--r--   0        0        0    11776 2024-05-13 14:42:39.000000 wxauto-3.9.8.15.8/wxauto/a.dll
+-rw-rw-rw-   0        0        0     8728 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.8/wxauto/color.py
+-rw-rw-rw-   0        0        0    24235 2024-05-17 16:41:17.000000 wxauto-3.9.8.15.8/wxauto/elements.py
+-rw-rw-rw-   0        0        0       49 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.8/wxauto/errors.py
+-rw-rw-rw-   0        0        0     5489 2024-05-17 16:30:23.000000 wxauto-3.9.8.15.8/wxauto/languages.py
+-rw-rw-rw-   0        0        0   366752 2024-05-14 04:11:30.000000 wxauto-3.9.8.15.8/wxauto/uiautomation.py
+-rw-rw-rw-   0        0        0    11545 2024-05-15 12:23:50.000000 wxauto-3.9.8.15.8/wxauto/utils.py
+-rw-rw-rw-   0        0        0    30013 2024-05-18 16:06:05.000000 wxauto-3.9.8.15.8/wxauto/wxauto.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:06:14.000000 wxauto-3.9.8.15.8/wxauto.egg-info/
+-rw-rw-rw-   0        0        0     3698 2024-05-18 16:06:14.000000 wxauto-3.9.8.15.8/wxauto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2024-05-18 16:06:14.000000 wxauto-3.9.8.15.8/wxauto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 16:06:14.000000 wxauto-3.9.8.15.8/wxauto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-05-18 16:06:14.000000 wxauto-3.9.8.15.8/wxauto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-18 16:06:14.000000 wxauto-3.9.8.15.8/wxauto.egg-info/top_level.txt
```

### Comparing `wxauto-3.9.8.15.7/PKG-INFO` & `wxauto-3.9.8.15.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxauto
-Version: 3.9.8.15.7
+Version: 3.9.8.15.8
 Summary: A simple wechat automation tool
 Author: Cluic
 Author-email: tikic@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
```

### Comparing `wxauto-3.9.8.15.7/README.md` & `wxauto-3.9.8.15.8/README.md`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.7/setup.py` & `wxauto-3.9.8.15.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='wxauto',
-    version='3.9.8.15.7',
+    version='3.9.8.15.8',
     author='Cluic',
     author_email='tikic@qq.com',
     description='A simple wechat automation tool',
     long_description=open('README.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
+    # a.dll
+    package_data={'wxauto': ['*.dll']},
     install_requires=[
         'pywin32',
         'pyperclip',
         'Pillow',
         'psutil',
         'typing_extensions',
         'comtypes',
```

### Comparing `wxauto-3.9.8.15.7/wxauto/color.py` & `wxauto-3.9.8.15.8/wxauto/color.py`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.7/wxauto/elements.py` & `wxauto-3.9.8.15.8/wxauto/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,15 @@
         return msgs
     
 
 class ChatWnd(WeChatBase):
     def __init__(self, who, language='cn'):
         self.who = who
         self.language = language
+        self.usedmsgid = []
         self.UiaAPI = uia.WindowControl(searchDepth=1, ClassName='ChatWnd', Name=who)
         self.editbox = self.UiaAPI.EditControl()
         self.C_MsgList = self.UiaAPI.ListControl()
         self.GetAllMessage()
 
         self.savepic = False   # 该参数用于在自动监听的情况下是否自动保存聊天图片
 
@@ -222,37 +223,38 @@
             savepic (bool): 是否自动保存聊天图片
             
         Returns:
             list: 聊天记录信息
         '''
         MsgItems = self.C_MsgList.GetChildren()
         msgs = self._getmsgs(MsgItems, savepic)
-        self.lastmsgid = msgs[-1][-1] if msgs else None
         return msgs
     
     def GetNewMessage(self, savepic=False):
         '''获取当前窗口中加载的新聊天记录
 
         Args:
             savepic (bool): 是否自动保存聊天图片
         
         Returns:
             list: 新聊天记录信息
         '''
-        lastmsgid = self.lastmsgid
-        msgs = self.GetAllMessage()
-        msgids = [i[-1] for i in msgs]
-        if lastmsgid:
-            index = (msgids.index(lastmsgid) if lastmsgid in msgids else -1)+1
-        else:
-            index = 0
-        MsgItems = self.C_MsgList.GetChildren()[index:]
-        newmsgs = self._getmsgs(MsgItems, savepic)
-        self.lastmsgid = newmsgs[-1][-1] if newmsgs else lastmsgid
+        if not self.usedmsgid:
+            self.usedmsgid = [i[-1] for i in self.GetAllMessage()]
+            return []
+        MsgItems = self.C_MsgList.GetChildren()
+        NewMsgItems = [i for i in MsgItems if ''.join([str(i) for i in i.GetRuntimeId()]) not in self.usedmsgid]
+        if not NewMsgItems:
+            return []
+        newmsgs = self._getmsgs(NewMsgItems, savepic)
+        self.usedmsgid = [i[-1] for i in self.GetAllMessage()]
+        if newmsgs[0].type == 'sys' and newmsgs[0].content == self._lang('查看更多消息'):
+            newmsgs = newmsgs[1:]
         return newmsgs
+
     
     def LoadMoreMessage(self):
         """加载当前聊天页面更多聊天信息
         
         Returns:
             bool: 是否成功加载更多聊天信息
         """
```

### Comparing `wxauto-3.9.8.15.7/wxauto/languages.py` & `wxauto-3.9.8.15.8/wxauto/languages.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,17 @@
 '输入': {'cn': '输入', 'cn_t': '輸入', 'en': 'Enter'}, 
 
 # 消息类型
 '链接': {'cn': '链接', 'cn_t': '鏈接', 'en': 'Link'}, 
 '视频': {'cn': '视频', 'cn_t': '視頻', 'en': 'Video'}, 
 '图片': {'cn': '图片', 'cn_t': '圖片', 'en': 'Photo'}, 
 '文件': {'cn': '文件', 'cn_t': '文件', 'en': 'File'}, 
-'': {'cn': '', 'cn_t': '', 'en': ''}}
+'查看更多消息': {'cn': '查看更多消息', 'cn_t': '', 'en': ''}}
+
+
 
 
 IMAGE_LANGUAGE = {
 '上一张': {'cn': '上一张', 'cn_t': '上一張', 'en': 'Previous'}, 
 '下一张': {'cn': '下一张', 'cn_t': '下一張', 'en': 'Next'}, 
 '预览': {'cn': '预览', 'cn_t': '預覽', 'en': 'Preview'}, 
 '放大': {'cn': '放大', 'cn_t': '放大', 'en': 'Zoom'},
```

### Comparing `wxauto-3.9.8.15.7/wxauto/uiautomation.py` & `wxauto-3.9.8.15.8/wxauto/uiautomation.py`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.7/wxauto/utils.py` & `wxauto-3.9.8.15.8/wxauto/utils.py`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.7/wxauto/wxauto.py` & `wxauto-3.9.8.15.8/wxauto/wxauto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Author: Cluic
-Update: 2024-05-15
-Version: 3.9.8.15.7
+Update: 2024-05-19
+Version: 3.9.8.15.8
 """
 
 from . import uiautomation as uia
 from .languages import *
 from .utils import *
 from .elements import *
 from .errors import *
@@ -29,14 +29,15 @@
         self.language = language
         self.lastmsgid = None
         self.listen = dict()
         self._checkversion()
         self.UiaAPI = uia.WindowControl(ClassName='WeChatMainWndForPC', searchDepth=1)
         self._show()
         self.SessionItemList = []
+        self.usedmsgid = []
         MainControl1 = [i for i in self.UiaAPI.GetChildren() if not i.ClassName][0]
         MainControl2 = MainControl1.GetChildren()[0]
         # 三个布局，导航栏(A)、聊天列表(B)、聊天框(C)
         # _______________
         # |■|———|    -□×|
         # | |———|       |
         # |A| B |   C   |   <--- 微信窗口布局简图示意
@@ -108,55 +109,73 @@
         """是否有新消息"""
         self._show()
         return IsRedPixel(self.A_ChatIcon)
     
     def GetNextNewMessage(self, savepic=False):
         """获取下一个新消息"""
         msgs_ = self.GetAllMessage()
-        if self.lastmsgid is None:
-            self.lastmsgid = msgs_[-1][-1]
-            return 
-        if self.lastmsgid is not None and self.lastmsgid in [i[-1] for i in msgs_[:-1]]:
+        msgids = [i[-1] for i in msgs_]
+
+        if not self.usedmsgid:
+            self.usedmsgid = msgids
+        
+        newmsgids = [i for i in msgids if i not in self.usedmsgid]
+        oldmsgids = [i for i in self.usedmsgid if i in msgids]
+        if newmsgids and oldmsgids:
             print('获取当前窗口新消息')
-            idx = [i[-1] for i in msgs_].index(self.lastmsgid)
-            MsgItems = self.C_MsgList.GetChildren()[idx+1:]
-            msgs = self._getmsgs(MsgItems, savepic)
-            self.lastmsgid = msgs[-1][-1]
+            MsgItems = self.C_MsgList.GetChildren()
+            msgids = [''.join([str(i) for i in i.GetRuntimeId()]) for i in MsgItems]
+            new = []
+            for i in range(len(msgids)-1, -1, -1):
+                if msgids[i] in self.usedmsgid:
+                    new = msgids[i+1:]
+                    break
+            NewMsgItems = [
+                i for i in MsgItems 
+                if ''.join([str(i) for i in i.GetRuntimeId()]) in new
+                and i.ControlTypeName == 'ListItemControl'
+            ]
+            if not NewMsgItems:
+                return []
+            msgs = self._getmsgs(NewMsgItems, savepic)
+            self.usedmsgid = msgids
             return {self.CurrentChat(): msgs}
 
         elif self.CheckNewMessage():
             print('获取其他窗口新消息')
             while True:
                 self.A_ChatIcon.DoubleClick(simulateMove=False)
                 sessiondict = self.GetSessionList(newmessage=True)
                 if sessiondict:
                     break
             for session in sessiondict:
                 self.ChatWith(session)
-                MsgItems = self.C_MsgList.GetChildren()[-sessiondict[session]:]
-                msgs = self._getmsgs(MsgItems, savepic)
-                self.lastmsgid = msgs[-1][-1]
+                NewMsgItems = self.C_MsgList.GetChildren()[-sessiondict[session]:]
+                msgs = self._getmsgs(NewMsgItems, savepic)
+                msgs_ = self.GetAllMessage()
+                print(msgs_)
+                self.usedmsgid = [i[-1] for i in msgs_]
                 return {session:msgs}
         else:
             # print('没有新消息')
-            return None
+            return []
     
     def GetAllNewMessage(self):
         """获取所有新消息"""
         newmessages = {}
         while True:
             if self.CheckNewMessage():
                 self.A_ChatIcon.DoubleClick(simulateMove=False)
                 sessiondict = self.GetSessionList(newmessage=True)
                 for session in sessiondict:
                     self.ChatWith(session)
                     newmessages[session] = self.GetAllMessage()[-sessiondict[session]:]
             else:
                 break
-        self.ChatWith(self._lang('文件传输助手'))
+        # self.ChatWith(self._lang('文件传输助手'))
         return newmessages
     
     def GetSessionList(self, reset=False, newmessage=False):
         """获取当前聊天列表中的所有聊天对象
         
         Args:
             reset (bool): 是否重置SessionItemList
@@ -372,15 +391,15 @@
                     break
             editbox.SendKeys('{Enter}')
             return True
         else:
             Warnings.lightred('所有文件都无法成功发送', stacklevel=2)
             return False
             
-    def GetAllMessage(self, savepic=False, n=0):
+    def GetAllMessage(self, savepic=False):
         '''获取当前窗口中加载的所有聊天记录
         
         Args:
             savepic (bool): 是否自动保存聊天图片
             
         Returns:
             list: 聊天记录信息
```

### Comparing `wxauto-3.9.8.15.7/wxauto.egg-info/PKG-INFO` & `wxauto-3.9.8.15.8/wxauto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxauto
-Version: 3.9.8.15.7
+Version: 3.9.8.15.8
 Summary: A simple wechat automation tool
 Author: Cluic
 Author-email: tikic@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
```

