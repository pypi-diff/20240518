# Comparing `tmp/talk_to_lollms-0.1.7.tar.gz` & `tmp/talk_to_lollms-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_to_lollms-0.1.7.tar", last modified: Fri May 17 20:51:50 2024, max compression
+gzip compressed data, was "talk_to_lollms-0.1.8.tar", last modified: Fri May 17 20:53:39 2024, max compression
```

## Comparing `talk_to_lollms-0.1.7.tar` & `talk_to_lollms-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 20:51:50.425751 talk_to_lollms-0.1.7/
--rw-rw-rw-   0        0        0    11558 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       45 2024-05-17 20:01:07.000000 talk_to_lollms-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0      329 2024-05-17 20:51:50.424752 talk_to_lollms-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0       57 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.7/README.md
--rw-rw-rw-   0        0        0      602 2024-05-17 20:42:43.000000 talk_to_lollms-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 20:51:50.426750 talk_to_lollms-0.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-17 20:51:50.405713 talk_to_lollms-0.1.7/talk_to_lollms/
--rw-rw-rw-   0        0        0        0 2024-05-15 23:47:06.000000 talk_to_lollms-0.1.7/talk_to_lollms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 20:51:50.421751 talk_to_lollms-0.1.7/talk_to_lollms/assets/
--rw-rw-rw-   0        0        0     3205 2024-05-15 23:43:16.000000 talk_to_lollms-0.1.7/talk_to_lollms/assets/settings.svg
--rw-rw-rw-   0        0        0    24212 2024-05-17 20:51:41.000000 talk_to_lollms-0.1.7/talk_to_lollms/main.py
-drwxrwxrwx   0        0        0        0 2024-05-17 20:51:50.423752 talk_to_lollms-0.1.7/talk_to_lollms.egg-info/
--rw-rw-rw-   0        0        0      329 2024-05-17 20:51:50.000000 talk_to_lollms-0.1.7/talk_to_lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2024-05-17 20:51:50.000000 talk_to_lollms-0.1.7/talk_to_lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 20:51:50.000000 talk_to_lollms-0.1.7/talk_to_lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-17 20:51:50.000000 talk_to_lollms-0.1.7/talk_to_lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       48 2024-05-17 20:51:50.000000 talk_to_lollms-0.1.7/talk_to_lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-17 20:51:50.000000 talk_to_lollms-0.1.7/talk_to_lollms.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 20:53:39.591621 talk_to_lollms-0.1.8/
+-rw-rw-rw-   0        0        0    11558 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0       45 2024-05-17 20:01:07.000000 talk_to_lollms-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      329 2024-05-17 20:53:39.590617 talk_to_lollms-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0       57 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.8/README.md
+-rw-rw-rw-   0        0        0      602 2024-05-17 20:53:30.000000 talk_to_lollms-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 20:53:39.591621 talk_to_lollms-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 20:53:39.572375 talk_to_lollms-0.1.8/talk_to_lollms/
+-rw-rw-rw-   0        0        0        0 2024-05-15 23:47:06.000000 talk_to_lollms-0.1.8/talk_to_lollms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 20:53:39.588105 talk_to_lollms-0.1.8/talk_to_lollms/assets/
+-rw-rw-rw-   0        0        0     3205 2024-05-15 23:43:16.000000 talk_to_lollms-0.1.8/talk_to_lollms/assets/settings.svg
+-rw-rw-rw-   0        0        0    24220 2024-05-17 20:53:22.000000 talk_to_lollms-0.1.8/talk_to_lollms/main.py
+drwxrwxrwx   0        0        0        0 2024-05-17 20:53:39.589611 talk_to_lollms-0.1.8/talk_to_lollms.egg-info/
+-rw-rw-rw-   0        0        0      329 2024-05-17 20:53:39.000000 talk_to_lollms-0.1.8/talk_to_lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2024-05-17 20:53:39.000000 talk_to_lollms-0.1.8/talk_to_lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 20:53:39.000000 talk_to_lollms-0.1.8/talk_to_lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-17 20:53:39.000000 talk_to_lollms-0.1.8/talk_to_lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       48 2024-05-17 20:53:39.000000 talk_to_lollms-0.1.8/talk_to_lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-17 20:53:39.000000 talk_to_lollms-0.1.8/talk_to_lollms.egg-info/top_level.txt
```

### Comparing `talk_to_lollms-0.1.7/LICENSE` & `talk_to_lollms-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `talk_to_lollms-0.1.7/pyproject.toml` & `talk_to_lollms-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "talk_to_lollms"
-version = "0.1.7"
+version = "0.1.8"
 description = "A client for Lollms that allows audio to audio full interaction with Lollms"
 authors = [
     { name = "ParisNeo", email = "parisneoai@gmail.com" }
 ]
 dependencies = [
     "requests",
     "pydantic",
```

### Comparing `talk_to_lollms-0.1.7/talk_to_lollms/assets/settings.svg` & `talk_to_lollms-0.1.8/talk_to_lollms/assets/settings.svg`

 * *Files identical despite different names*

### Comparing `talk_to_lollms-0.1.7/talk_to_lollms/main.py` & `talk_to_lollms-0.1.8/talk_to_lollms/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,17 +240,17 @@
                     transcription_fn = str(Path(self.logs_folder)/filename) + ".txt"
                     with open(transcription_fn, "w", encoding="utf-8") as f:
                         f.write(result["text"])
 
                     with self.transcribed_lock:
                         self.transcribed_files.append((filename, result["text"]))
                         self.transcribed_lock.notify()
-                    self.transcription_signal.new_user_transcription.emit(filename, result["text"])
-                    self.discussion.add_message("user",result["text"])
                     if result["text"]!="":
+                        self.transcription_signal.new_user_transcription.emit(filename, result["text"])
+                        self.discussion.add_message("user",result["text"])
                         discussion = self.discussion.format_discussion(self.context_size)
                         full_context = '!@>system:' + self.cond +"\n" + discussion+"\n!@>lollms:"
                         ASCIIColors.red(" ---------------- Discussion ---------------------")
                         ASCIIColors.yellow(full_context)
                         ASCIIColors.red(" -------------------------------------------------")
                         self.transcription_signal.update_status.emit("Generating answer")
                         ASCIIColors.green("<<RESPONDING>>")
```

