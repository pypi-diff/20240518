# Comparing `tmp/music_brainz_api_micro-0.1.5.tar.gz` & `tmp/music_brainz_api_micro-0.1.6.tar.gz`

## Comparing `music_brainz_api_micro-0.1.5.tar` & `music_brainz_api_micro-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0      122 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/MusicBrainzAPI.code-workspace
--rwxr-xr-x   0        0        0      469 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/profile/benchmark.py
--rwxr-xr-x   0        0        0      513 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/src/music_brainz_api_micro/__init__.py
--rwxr-xr-x   0        0        0      368 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/src/music_brainz_api_micro/cover_reponse.py
--rwxr-xr-x   0        0        0     7157 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/src/music_brainz_api_micro/music_brainz_api.py
--rwxr-xr-x   0        0        0     1363 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/tests/flask_server.py
--rwxr-xr-x   0        0        0     1528 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/tests/test_musicbrainzapi.py
--rwxr-xr-x   0        0        0     1831 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/.gitignore
--rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/LICENSE
--rwxr-xr-x   0        0        0     1190 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/README.md
--rwxr-xr-x   0        0        0      733 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/PKG-INFO
+-rwxr-xr-x   0        0        0      122 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.6/MusicBrainzAPI.code-workspace
+-rwxr-xr-x   0        0        0      469 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.6/profile/benchmark.py
+-rwxr-xr-x   0        0        0      513 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.6/src/music_brainz_api_micro/__init__.py
+-rwxr-xr-x   0        0        0      368 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.6/src/music_brainz_api_micro/cover_reponse.py
+-rwxr-xr-x   0        0        0     7642 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.6/src/music_brainz_api_micro/music_brainz_api.py
+-rwxr-xr-x   0        0        0     1363 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.6/tests/flask_server.py
+-rwxr-xr-x   0        0        0     1528 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.6/tests/test_musicbrainzapi.py
+-rwxr-xr-x   0        0        0     1831 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.6/.gitignore
+-rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.6/LICENSE
+-rwxr-xr-x   0        0        0     1190 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.6/README.md
+-rwxr-xr-x   0        0        0      733 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.6/PKG-INFO
```

### Comparing `music_brainz_api_micro-0.1.5/src/music_brainz_api_micro/__init__.py` & `music_brainz_api_micro-0.1.6/src/music_brainz_api_micro/__init__.py`

 * *Files identical despite different names*

### Comparing `music_brainz_api_micro-0.1.5/src/music_brainz_api_micro/music_brainz_api.py` & `music_brainz_api_micro-0.1.6/src/music_brainz_api_micro/music_brainz_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,14 +144,24 @@
 
         :param mbid: MusicBrainz Id for the release, dashes included
         :returns: Response, check for error property True or False, if 
             False 'response' property can be used
         """
         return self._run_get(f"release/{mbid}", {'inc': 'aliases+artist-credits+labels+discids+recordings'}, mbid, 'releases')
 
+    def get_release_group(self, mbid: str) -> R:
+        """Using the MusicBrainz ID of a release, returns the release response 
+        https://musicbrainz.org/doc/Release
+
+        :param mbid: MusicBrainz Id for the release, dashes included
+        :returns: Response, check for error property True or False, if 
+            False 'response' property can be used
+        """
+        return self._run_get(f"release-group/{mbid}", {'inc': 'aliases+artist-credits'}, mbid, 'releases')
+
     def get_release_titles_by_artist(self, mbid: str) -> list[str] | list[R]:
         """Runs a getReleasesByArtist but returns the release titles of the responses
 
         :param mbid: MusicBrainz ID including dashes
         :returns: List of release titles for the associated artist or the Response
             with the error message     
         """
```

### Comparing `music_brainz_api_micro-0.1.5/tests/flask_server.py` & `music_brainz_api_micro-0.1.6/tests/flask_server.py`

 * *Files identical despite different names*

### Comparing `music_brainz_api_micro-0.1.5/tests/test_musicbrainzapi.py` & `music_brainz_api_micro-0.1.6/tests/test_musicbrainzapi.py`

 * *Files identical despite different names*

### Comparing `music_brainz_api_micro-0.1.5/.gitignore` & `music_brainz_api_micro-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `music_brainz_api_micro-0.1.5/LICENSE` & `music_brainz_api_micro-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `music_brainz_api_micro-0.1.5/README.md` & `music_brainz_api_micro-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `music_brainz_api_micro-0.1.5/pyproject.toml` & `music_brainz_api_micro-0.1.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
   "hatchling",
 ]
 build-backend = "hatchling.build"
 [project]
 name = "music_brainz_api_micro"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name = "Samuel Shiels" },
 ]
 description = "A micro client for MusicBrainz, implements simple functions to retrieve information"
 readme = "README.md"
 requires-python = ">=3.11.5"
 classifiers = [
```

### Comparing `music_brainz_api_micro-0.1.5/PKG-INFO` & `music_brainz_api_micro-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: music_brainz_api_micro
-Version: 0.1.5
+Version: 0.1.6
 Summary: A micro client for MusicBrainz, implements simple functions to retrieve information
 Author: Samuel Shiels
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

