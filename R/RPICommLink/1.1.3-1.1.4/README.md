# Comparing `tmp/RPICommLink-1.1.3.tar.gz` & `tmp/rpicommlink-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RPICommLink-1.1.3.tar", last modified: Wed May 15 06:59:57 2024, max compression
+gzip compressed data, was "rpicommlink-1.1.4.tar", last modified: Sat May 18 06:17:38 2024, max compression
```

## Comparing `RPICommLink-1.1.3.tar` & `rpicommlink-1.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 06:59:57.825827 RPICommLink-1.1.3/
--rw-rw-rw-   0        0        0     1070 2024-05-07 16:58:39.000000 RPICommLink-1.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1920 2024-05-15 06:59:57.822693 RPICommLink-1.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-15 06:59:57.786776 RPICommLink-1.1.3/RPICommLink/
--rw-rw-rw-   0        0        0    21233 2024-05-15 06:59:20.000000 RPICommLink-1.1.3/RPICommLink/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:59:57.818690 RPICommLink-1.1.3/RPICommLink.egg-info/
--rw-rw-rw-   0        0        0     1920 2024-05-15 06:59:57.000000 RPICommLink-1.1.3/RPICommLink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2024-05-15 06:59:57.000000 RPICommLink-1.1.3/RPICommLink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 06:59:57.000000 RPICommLink-1.1.3/RPICommLink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-15 06:59:57.000000 RPICommLink-1.1.3/RPICommLink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 06:59:57.825827 RPICommLink-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     2433 2024-05-15 06:59:20.000000 RPICommLink-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 06:17:38.448778 rpicommlink-1.1.4/
+-rw-rw-rw-   0        0        0     1070 2024-05-07 16:58:39.000000 rpicommlink-1.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     2030 2024-05-18 06:17:38.448778 rpicommlink-1.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-18 06:17:38.444788 rpicommlink-1.1.4/RPICommLink/
+-rw-rw-rw-   0        0        0    22616 2024-05-18 06:15:24.000000 rpicommlink-1.1.4/RPICommLink/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 06:17:38.447780 rpicommlink-1.1.4/RPICommLink.egg-info/
+-rw-rw-rw-   0        0        0     2030 2024-05-18 06:17:38.000000 rpicommlink-1.1.4/RPICommLink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2024-05-18 06:17:38.000000 rpicommlink-1.1.4/RPICommLink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 06:17:38.000000 rpicommlink-1.1.4/RPICommLink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-18 06:17:38.000000 rpicommlink-1.1.4/RPICommLink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 06:17:38.449775 rpicommlink-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     2568 2024-05-18 06:16:51.000000 rpicommlink-1.1.4/setup.py
```

### Comparing `RPICommLink-1.1.3/LICENSE.txt` & `rpicommlink-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RPICommLink-1.1.3/PKG-INFO` & `rpicommlink-1.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RPICommLink
-Version: 1.1.3
+Version: 1.1.4
 Summary: A library for communication on Raspberry Pi
 Author: adixu
 Author-email: adixu7@gmail.com
 License-File: LICENSE.txt
 
 RPICommLink 是一个用于在不同设备之间建立通信连接的 Python 类。提供了一系列方法使设备能够通过 TCP/IP 协议进行数据交换。灵活的通信设置可以轻松地在设备之间建立通信连接，无论是在局域网内部还是通过互联网。具备完善的错误处理机制及时发现并处理连接中断、超时等异常情况，保证通信的稳定性和可靠性。使用简单易用的接口可以方便地发送和接收数据，无需过多关注底层网络细节，让设备之间的通信变得更加简单和高效。通过 RPICommLink 类，可以实现设备之间的数据交换，为项目提供强大的通信支持。
 
@@ -69,7 +69,13 @@
 1.1.2 -现在服务端与客户端都可以进行发送或接收了
 
 
 
 
 
 1.1.3 -添加了装饰器的用法，使代码更加简介
+
+
+
+
+
+1.1.4 -给图像接收添加了装饰器的用法；auto_frame现在可以选择不同的相机了
```

### Comparing `RPICommLink-1.1.3/RPICommLink/__init__.py` & `rpicommlink-1.1.4/RPICommLink/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -352,28 +352,28 @@
             except Exception:
                 print('\033[91mError:一个服务器发送失败！请确认是否有连接服务器 \033[0m')
                 self._send_server_socket.remove(sock)
                 if len(self._send_server_socket) == 0:
                     print('\033[91mError:无服务器连接 \033[0m')
                     sys.exit()
 
-    def auto_frame(self):
+    def auto_frame(self, cap: int = 0):
         if self._device_state == 'server':
-            threading.Thread(target=self._auto_frame, daemon=True).start()
+            threading.Thread(target=self._auto_frame, args=(cap, ), daemon=True).start()
         elif self._device_state is None:
             print(f'\033[91mError:未开启或连接服务器 \033[0m')
         else:
-            threading.Thread(target=self._auto_frame, daemon=True).start()
+            threading.Thread(target=self._auto_frame, args=(cap, ), daemon=True).start()
             print(f'\033[93mWarning:客户端发送系统冲突！这会导致无法发送正常数据以及其它报错！'
                   f'这不是一个正常用法，强烈建议使用send_frame自行进行发送！ \033[0m')
 
-    def _auto_frame(self):
+    def _auto_frame(self, capnumber):
         import cv2
 
-        cap = cv2.VideoCapture(0)
+        cap = cv2.VideoCapture(capnumber)
         while True:
             ret, _frame = cap.read()
             self.send_frame(_frame)
 
     def send_frame(self, frame):
         """读摄像头数据 发送给服务器"""
         import cv2
@@ -427,14 +427,49 @@
                 length -= len(temp_size)
                 img_data += temp_size
         data = numpy.frombuffer(img_data, dtype='uint8')
         image = cv2.imdecode(data, cv2.IMREAD_UNCHANGED)
         self.state = False
         return image
 
+    def recv_frame_test(self, func):
+        def wrapper():
+            threading.Thread(target=self._thread_recv_frame, args=(func, ), daemon=True).start()
+        return wrapper()
+
+    def _thread_recv_frame(self, func):
+        import struct
+        import numpy
+        import cv2
+        while True:
+            data = None
+            sock_list = []
+            if self._device_state == 'client':
+                sock_list.append(self._send_server_socket)
+            elif self._device_state is None:
+                print(f'\033[91mError:未开启或连接服务器 \033[0m')
+            else:
+                self.state = True
+                sock_list = self.socket_list
+                self.wait()
+            for sock in sock_list:
+                data = sock[0].recv(8)
+
+            length, width, height = struct.unpack('ihh', data)
+            img_data = b''  # 存放最终的图片数据
+            while length:
+                for sock in sock_list:
+                    temp_size = sock[0].recv(length)
+                    length -= len(temp_size)
+                    img_data += temp_size
+            data = numpy.frombuffer(img_data, dtype='uint8')
+            image = cv2.imdecode(data, cv2.IMREAD_UNCHANGED)
+            self.state = False
+            func(image)
+
 
 def get_host_ip():
     """
     查询本机IP地址
     :return:本机IP地址
     """
     try:
```

### Comparing `RPICommLink-1.1.3/RPICommLink.egg-info/PKG-INFO` & `rpicommlink-1.1.4/RPICommLink.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RPICommLink
-Version: 1.1.3
+Version: 1.1.4
 Summary: A library for communication on Raspberry Pi
 Author: adixu
 Author-email: adixu7@gmail.com
 License-File: LICENSE.txt
 
 RPICommLink 是一个用于在不同设备之间建立通信连接的 Python 类。提供了一系列方法使设备能够通过 TCP/IP 协议进行数据交换。灵活的通信设置可以轻松地在设备之间建立通信连接，无论是在局域网内部还是通过互联网。具备完善的错误处理机制及时发现并处理连接中断、超时等异常情况，保证通信的稳定性和可靠性。使用简单易用的接口可以方便地发送和接收数据，无需过多关注底层网络细节，让设备之间的通信变得更加简单和高效。通过 RPICommLink 类，可以实现设备之间的数据交换，为项目提供强大的通信支持。
 
@@ -69,7 +69,13 @@
 1.1.2 -现在服务端与客户端都可以进行发送或接收了
 
 
 
 
 
 1.1.3 -添加了装饰器的用法，使代码更加简介
+
+
+
+
+
+1.1.4 -给图像接收添加了装饰器的用法；auto_frame现在可以选择不同的相机了
```

### Comparing `RPICommLink-1.1.3/setup.py` & `rpicommlink-1.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='RPICommLink',
-    version='1.1.3',
+    version='1.1.4',
     author='adixu',
     author_email='adixu7@gmail.com',
     description='A library for communication on Raspberry Pi',
     long_description="RPICommLink 是一个用于在不同设备之间建立通信连接的 Python 类。提供了一系列方法使设备能够通过 TCP/IP 协议进行数据交换。"
                      "灵活的通信设置可以轻松地在设备之间建立通信连接，无论是在局域网内部还是通过互联网。"
                      "具备完善的错误处理机制及时发现并处理连接中断、超时等异常情况，保证通信的稳定性和可靠性。"
                      "使用简单易用的接口可以方便地发送和接收数据，无需过多关注底层网络细节，让设备之间的通信变得更加简单和高效。"
@@ -17,12 +17,13 @@
                      "\n\n\n\n\n\n1.0.4 -重新了上传中文介绍。"
                      "\n\n\n\n\n\n1.0.5 -修复了无法在无互联网下获取IP的报错，修复了无法同时连接两个服务器的bug。"
                      "\n\n\n\n\n\n1.0.6 -修复了潜在bug"
                      "\n\n\n\n\n\n1.0.7 -轻量化"
                      "\n\n\n\n\n\n1.1   -增加了传输摄像头帧的函数，需要自行下载opencv-python库。注意：该版本为测试版，将会有许多未发现的报错，建议在在服务器端发送摄像头帧而不是客户端。"
                      "\n\n\n\n\n\n1.1.1 -修复了几个bug。注意：该版本为测试版，将会有许多未发现的报错，建议在在服务器端发送摄像头帧而不是客户端。"
                      "\n\n\n\n\n\n1.1.2 -现在服务端与客户端都可以进行发送或接收了"
-                     "\n\n\n\n\n\n1.1.3 -添加了装饰器的用法，使代码更加简介",
+                     "\n\n\n\n\n\n1.1.3 -添加了装饰器的用法，使代码更加简介"
+                     "\n\n\n\n\n\n1.1.4 -给图像接收添加了装饰器的用法；auto_frame现在可以选择不同的相机了",
     packages=['RPICommLink'],
     include_package_data=True,
     install_requires=[],
 )
```

