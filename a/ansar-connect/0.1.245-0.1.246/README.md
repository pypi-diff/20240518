# Comparing `tmp/ansar_connect-0.1.245.tar.gz` & `tmp/ansar_connect-0.1.246.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.245.tar", last modified: Wed May 15 01:33:16 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.246.tar", last modified: Sat May 18 01:34:30 2024, max compression
```

## Comparing `ansar_connect-0.1.245.tar` & `ansar_connect-0.1.246.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-15 01:33:16.292724 ansar_connect-0.1.245/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.245/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-15 01:33:16.292724 ansar_connect-0.1.245/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.245/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-15 01:33:06.000000 ansar_connect-0.1.245/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-15 01:33:16.292724 ansar_connect-0.1.245/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-15 01:32:55.000000 ansar_connect-0.1.245/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-15 01:33:16.288724 ansar_connect-0.1.245/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-15 01:33:16.288724 ansar_connect-0.1.245/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-15 01:33:16.288724 ansar_connect-0.1.245/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.245/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3259 2024-05-08 21:30:23.000000 ansar_connect-0.1.245/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.245/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8855 2024-05-08 21:32:04.000000 ansar_connect-0.1.245/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-15 01:33:16.292724 ansar_connect-0.1.245/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-15 01:33:13.000000 ansar_connect-0.1.245/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.245/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    87458 2024-05-09 02:23:09.000000 ansar_connect-0.1.245/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8445 2024-05-07 03:55:37.000000 ansar_connect-0.1.245/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10461 2024-05-10 15:14:29.000000 ansar_connect-0.1.245/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.245/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14241 2024-05-09 13:41:02.000000 ansar_connect-0.1.245/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.245/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-07 01:18:28.000000 ansar_connect-0.1.245/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.245/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8453 2024-05-09 12:04:12.000000 ansar_connect-0.1.245/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.245/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33894 2024-05-13 17:10:04.000000 ansar_connect-0.1.245/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.245/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    39110 2024-05-15 01:30:21.000000 ansar_connect-0.1.245/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.245/src/ansar/connect/standard.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2063 2024-05-07 01:18:28.000000 ansar_connect-0.1.245/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.245/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.245/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-15 01:33:16.292724 ansar_connect-0.1.245/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-15 01:33:16.000000 ansar_connect-0.1.245/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-15 01:33:16.000000 ansar_connect-0.1.245/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-15 01:33:16.000000 ansar_connect-0.1.245/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-15 01:33:16.000000 ansar_connect-0.1.245/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-15 01:33:16.000000 ansar_connect-0.1.245/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-15 01:33:16.000000 ansar_connect-0.1.245/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-18 01:34:30.228791 ansar_connect-0.1.246/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.246/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-18 01:34:30.228791 ansar_connect-0.1.246/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.246/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-15 01:33:06.000000 ansar_connect-0.1.246/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-18 01:34:30.228791 ansar_connect-0.1.246/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-15 01:32:55.000000 ansar_connect-0.1.246/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-18 01:34:30.224791 ansar_connect-0.1.246/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-18 01:34:30.224791 ansar_connect-0.1.246/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-18 01:34:30.224791 ansar_connect-0.1.246/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.246/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-0.1.246/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.246/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-0.1.246/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-18 01:34:30.228791 ansar_connect-0.1.246/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-18 01:34:27.000000 ansar_connect-0.1.246/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.246/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    87458 2024-05-09 02:23:09.000000 ansar_connect-0.1.246/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8445 2024-05-07 03:55:37.000000 ansar_connect-0.1.246/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10461 2024-05-10 15:14:29.000000 ansar_connect-0.1.246/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.246/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14241 2024-05-09 13:41:02.000000 ansar_connect-0.1.246/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.246/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-07 01:18:28.000000 ansar_connect-0.1.246/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.246/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8453 2024-05-09 12:04:12.000000 ansar_connect-0.1.246/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.246/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33894 2024-05-13 17:10:04.000000 ansar_connect-0.1.246/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.246/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    39110 2024-05-15 01:30:21.000000 ansar_connect-0.1.246/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.246/src/ansar/connect/standard.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2063 2024-05-07 01:18:28.000000 ansar_connect-0.1.246/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.246/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.246/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-18 01:34:30.228791 ansar_connect-0.1.246/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-18 01:34:30.000000 ansar_connect-0.1.246/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-18 01:34:30.000000 ansar_connect-0.1.246/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-18 01:34:30.000000 ansar_connect-0.1.246/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-18 01:34:30.000000 ansar_connect-0.1.246/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-18 01:34:30.000000 ansar_connect-0.1.246/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-18 01:34:30.000000 ansar_connect-0.1.246/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.245/LICENSE` & `ansar_connect-0.1.246/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/PKG-INFO` & `ansar_connect-0.1.246/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.245
+Version: 0.1.246
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.245/README.md` & `ansar_connect-0.1.246/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/pyproject.toml` & `ansar_connect-0.1.246/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/setup.py` & `ansar_connect-0.1.246/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.246/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.246/src/ansar/command/ansar_directory.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,33 +32,39 @@
 	'main',
 ]
 
 #
 #
 class Settings(object):
 	def __init__(self, directory_scope=None, connect_above=None, accept_below=None,
-			encrypted=False):
+			encrypted=False,
+			custom_port=None):
 		self.directory_scope = directory_scope or ar.ScopeOfService.HOST
 		self.connect_above = connect_above or ar.HostPort()
 		self.accept_below = accept_below or ar.HostPort()
 		self.encrypted = encrypted
+		self.custom_port = custom_port
 
 SETTINGS_SCHEMA = {
 	'directory_scope': ar.ScopeOfService,
 	'connect_above': ar.Any(),
 	'accept_below': ar.UserDefined(ar.HostPort),
 	'encrypted': ar.Boolean(),
+	'custom_port': ar.Integer8(),
 }
 
 ar.bind(Settings, object_schema=SETTINGS_SCHEMA)
 
 # Just need an object to stay "on duty" while the 
 # global ServiceDirectory does its work.
 def directory(self, settings):
 	encrypted = settings.encrypted
+	if settings.custom_port:
+		d = settings.accept_below.port - ANSAR_DIRECTORY_PORT
+		settings.accept_below.port = settings.custom_port + d
 	a = self.create(ar.ServiceDirectory, settings.directory_scope,
 		settings.connect_above, settings.accept_below,
 		encrypted=encrypted)
 	m = self.select(ar.HostPort, ar.Completed, ar.Stop)
 	if isinstance(m, ar.Completed):
 		return m.value
 	elif isinstance(m, ar.Stop):
@@ -92,14 +98,15 @@
 
 #
 #
 factory_settings = Settings(
 	directory_scope=ar.ScopeOfService.HOST,
 	accept_below=ANSAR_LOCAL_DEDICATED,
 	connect_above=ar.HostPort(),
+	custom_port=0
 )
 
 #
 #
 def main():
     ar.create_object(directory, factory_settings=factory_settings)
```

### Comparing `ansar_connect-0.1.245/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.246/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.246/src/ansar/command/shared_directory.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,18 @@
 	self.recover = recover
 
 	# Initial load.
 	self.recover()
 
 	settings = self.settings
 	encrypted = settings.encrypted
-	ar.listen(self, self.settings.public_access, encrypted=encrypted)
+	if settings.custom_port:
+		d = settings.public_access.port - ANSAR_DIRECTORY_PORT
+		settings.public_access.port = settings.custom_port + d
+	ar.listen(self, settings.public_access, encrypted=encrypted)
 	return STARTING
 
 # Verify access
 def ProductDirectory_STARTING_Listening(self, message):
 	self.public_access = message
 	return READY
 
@@ -273,31 +276,34 @@
 
 ar.bind(ProductDirectory, PRODUCT_DIRECTORY_DISPATCH)
 
 
 # Allow configuration of network details.
 #
 class Settings(object):
-	def __init__(self, directory_scope=None, public_access=None, encrypted=False):
+	def __init__(self, directory_scope=None, public_access=None, encrypted=False, custom_port=None):
 		self.directory_scope = directory_scope
 		self.public_access = public_access or ar.HostPort()
 		self.encrypted = encrypted
+		self.custom_port = custom_port
 
 SETTINGS_SCHEMA = {
 	'directory_scope': ar.ScopeOfService,
 	'public_access': ar.UserDefined(ar.HostPort),
 	'encrypted': ar.Boolean(),
+	'custom_port': ar.Integer8(),
 }
 
 ar.bind(Settings, object_schema=SETTINGS_SCHEMA)
 
 #
 #
 factory_settings = Settings(directory_scope=ar.ScopeOfService.HOST,
-	public_access=ANSAR_LOCAL_SHARED)
+	public_access=ANSAR_LOCAL_SHARED,
+	custom_port=0)
 
 #
 #
 def main():
     ar.create_object(ProductDirectory, factory_settings=factory_settings)
 
 # The standard entry point. Needed for IDEs
```

### Comparing `ansar_connect-0.1.245/src/ansar/connect/__init__.py` & `ansar_connect-0.1.246/src/ansar/connect/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: f5031da98c580f6b3b5fe80a000122d7f454f6e5
-Version: 0.1.244 (2024-05-15@13:33:13+NZST)
+Commit: f998cfe99efc82b815305705e5b5d7644d129a40
+Version: 0.1.245 (2024-05-18@13:34:27+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.245/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.246/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar/connect/directory.py` & `ansar_connect-0.1.246/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.246/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.246/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar/connect/group_if.py` & `ansar_connect-0.1.246/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar/connect/grouping.py` & `ansar_connect-0.1.246/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar/connect/moving.py` & `ansar_connect-0.1.246/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar/connect/networking.py` & `ansar_connect-0.1.246/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.246/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar/connect/node.py` & `ansar_connect-0.1.246/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.246/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar/connect/procedure.py` & `ansar_connect-0.1.246/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar/connect/product.py` & `ansar_connect-0.1.246/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar/connect/socketry.py` & `ansar_connect-0.1.246/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar/connect/standard.py` & `ansar_connect-0.1.246/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar/connect/transporting.py` & `ansar_connect-0.1.246/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.246/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar/connect/wan.py` & `ansar_connect-0.1.246/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.245/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.246/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.245
+Version: 0.1.246
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.245/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.246/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

