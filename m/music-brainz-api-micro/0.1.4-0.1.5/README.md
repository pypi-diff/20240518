# Comparing `tmp/music_brainz_api_micro-0.1.4.tar.gz` & `tmp/music_brainz_api_micro-0.1.5.tar.gz`

## Comparing `music_brainz_api_micro-0.1.4.tar` & `music_brainz_api_micro-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0      122 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.4/MusicBrainzAPI.code-workspace
--rwxr-xr-x   0        0        0      469 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.4/profile/benchmark.py
--rwxr-xr-x   0        0        0      513 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.4/src/music_brainz_api_micro/__init__.py
--rwxr-xr-x   0        0        0      368 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.4/src/music_brainz_api_micro/cover_reponse.py
--rwxr-xr-x   0        0        0     6355 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.4/src/music_brainz_api_micro/music_brainz_api.py
--rwxr-xr-x   0        0        0     1363 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.4/tests/flask_server.py
--rwxr-xr-x   0        0        0     1528 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.4/tests/test_musicbrainzapi.py
--rwxr-xr-x   0        0        0     1831 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.4/.gitignore
--rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.4/LICENSE
--rwxr-xr-x   0        0        0     1190 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.4/README.md
--rwxr-xr-x   0        0        0      733 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.4/PKG-INFO
+-rwxr-xr-x   0        0        0      122 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/MusicBrainzAPI.code-workspace
+-rwxr-xr-x   0        0        0      469 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/profile/benchmark.py
+-rwxr-xr-x   0        0        0      513 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/src/music_brainz_api_micro/__init__.py
+-rwxr-xr-x   0        0        0      368 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/src/music_brainz_api_micro/cover_reponse.py
+-rwxr-xr-x   0        0        0     7157 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/src/music_brainz_api_micro/music_brainz_api.py
+-rwxr-xr-x   0        0        0     1363 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/tests/flask_server.py
+-rwxr-xr-x   0        0        0     1528 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/tests/test_musicbrainzapi.py
+-rwxr-xr-x   0        0        0     1831 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/.gitignore
+-rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/LICENSE
+-rwxr-xr-x   0        0        0     1190 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/README.md
+-rwxr-xr-x   0        0        0      733 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 music_brainz_api_micro-0.1.5/PKG-INFO
```

### Comparing `music_brainz_api_micro-0.1.4/src/music_brainz_api_micro/__init__.py` & `music_brainz_api_micro-0.1.5/src/music_brainz_api_micro/__init__.py`

 * *Files identical despite different names*

### Comparing `music_brainz_api_micro-0.1.4/src/music_brainz_api_micro/music_brainz_api.py` & `music_brainz_api_micro-0.1.5/src/music_brainz_api_micro/music_brainz_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -125,37 +125,53 @@
         :returns: Response, check for error property True or False, if 
             False 'response' property can be used
         """
         self._debug("getArtistByMBID")
         return self._run_get(f'artist/{mbid}', {'inc': 'aliases'}, mbid, 'artist')
 
     def get_releases_by_artist(self, mbid: str) -> R:
-        """contains property 'release-groups'"""
+        """Using the MusicBrainz ID of an artist returns the full
+        MusicBrainz response with `release-groups`
+
+        :param mbid: MusicBrainz ID including dashes
+        :returns: Response, check for error property True or False, if 
+            False 'response' property can be used
+        """
         return self._run_rest(f'artist/{mbid}', {'inc': 'aliases+release-groups'}, mbid, 'releases')
 
+    def get_release(self, mbid: str) -> R:
+        """Using the MusicBrainz ID of a release, returns the release response 
+        https://musicbrainz.org/doc/Release
+
+        :param mbid: MusicBrainz Id for the release, dashes included
+        :returns: Response, check for error property True or False, if 
+            False 'response' property can be used
+        """
+        return self._run_get(f"release/{mbid}", {'inc': 'aliases+artist-credits+labels+discids+recordings'}, mbid, 'releases')
+
     def get_release_titles_by_artist(self, mbid: str) -> list[str] | list[R]:
         """Runs a getReleasesByArtist but returns the release titles of the responses
 
         :param mbid: MusicBrainz ID including dashes
-        :returns: List of release titles for the associated artist        
+        :returns: List of release titles for the associated artist or the Response
+            with the error message     
         """
         ret_val = []
         artist_releases = self.get_releases_by_artist(mbid)
         if artist_releases.error is True:
             ret_val.append(artist_releases)
             return ret_val
         thawed = jsonpickle.decode(artist_releases.response)
         for release in thawed['release-groups']:
             ret_val.append(release['title'])
         return ret_val
 
     def get_recording_cover(self, recording_mbid: str) -> CR | None:
         """From a recording mbid determines if it is a recording
 
-
         :param mbid: MusicBrainz recording ID including dashes
         :returns: CoverResponse object or None
         """
         recording_rels = self._run_get(
             f"recording/{recording_mbid}",
             {"inc": "aliases+work-rels+artist-credits"},
             recording_mbid,
```

### Comparing `music_brainz_api_micro-0.1.4/tests/flask_server.py` & `music_brainz_api_micro-0.1.5/tests/flask_server.py`

 * *Files identical despite different names*

### Comparing `music_brainz_api_micro-0.1.4/tests/test_musicbrainzapi.py` & `music_brainz_api_micro-0.1.5/tests/test_musicbrainzapi.py`

 * *Files identical despite different names*

### Comparing `music_brainz_api_micro-0.1.4/.gitignore` & `music_brainz_api_micro-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `music_brainz_api_micro-0.1.4/LICENSE` & `music_brainz_api_micro-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `music_brainz_api_micro-0.1.4/README.md` & `music_brainz_api_micro-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `music_brainz_api_micro-0.1.4/pyproject.toml` & `music_brainz_api_micro-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
   "hatchling",
 ]
 build-backend = "hatchling.build"
 [project]
 name = "music_brainz_api_micro"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name = "Samuel Shiels" },
 ]
 description = "A micro client for MusicBrainz, implements simple functions to retrieve information"
 readme = "README.md"
 requires-python = ">=3.11.5"
 classifiers = [
```

### Comparing `music_brainz_api_micro-0.1.4/PKG-INFO` & `music_brainz_api_micro-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: music_brainz_api_micro
-Version: 0.1.4
+Version: 0.1.5
 Summary: A micro client for MusicBrainz, implements simple functions to retrieve information
 Author: Samuel Shiels
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

