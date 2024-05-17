# Comparing `tmp/mixpanel-utils-2.2.5.tar.gz` & `tmp/mixpanel_utils-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jaredmcfarland/PyPi Package/dist/tmp7ln_p61n/mixpanel-utils-2.2.5.tar", last modified: Wed Feb 23 23:49:02 2022, max compression
+gzip compressed data, was "mixpanel_utils-2.2.6.tar", last modified: Fri May 17 21:43:21 2024, max compression
```

## Comparing `mixpanel-utils-2.2.5.tar` & `mixpanel_utils-2.2.6.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 jaredmcfarland   (501) staff       (20)        0 2022-02-23 23:49:02.369383 mixpanel-utils-2.2.5/
--rw-r--r--   0 jaredmcfarland   (501) staff       (20)      469 2022-02-23 23:49:02.369012 mixpanel-utils-2.2.5/PKG-INFO
-drwxr-xr-x   0 jaredmcfarland   (501) staff       (20)        0 2022-02-23 23:49:02.364963 mixpanel-utils-2.2.5/mixpanel_utils/
--rwxr-xr-x   0 jaredmcfarland   (501) staff       (20)   100703 2022-02-23 23:26:59.000000 mixpanel-utils-2.2.5/mixpanel_utils/__init__.py
--rw-r--r--   0 jaredmcfarland   (501) staff       (20)     5712 2021-03-25 20:26:51.000000 mixpanel-utils-2.2.5/mixpanel_utils/mixpanel_utils_example.py
--rw-r--r--   0 jaredmcfarland   (501) staff       (20)     3259 2021-03-25 19:12:40.000000 mixpanel-utils-2.2.5/mixpanel_utils/paginator.py
-drwxr-xr-x   0 jaredmcfarland   (501) staff       (20)        0 2022-02-23 23:49:02.368455 mixpanel-utils-2.2.5/mixpanel_utils.egg-info/
--rw-r--r--   0 jaredmcfarland   (501) staff       (20)      469 2022-02-23 23:49:02.000000 mixpanel-utils-2.2.5/mixpanel_utils.egg-info/PKG-INFO
--rw-r--r--   0 jaredmcfarland   (501) staff       (20)      256 2022-02-23 23:49:02.000000 mixpanel-utils-2.2.5/mixpanel_utils.egg-info/SOURCES.txt
--rw-r--r--   0 jaredmcfarland   (501) staff       (20)        1 2022-02-23 23:49:02.000000 mixpanel-utils-2.2.5/mixpanel_utils.egg-info/dependency_links.txt
--rw-r--r--   0 jaredmcfarland   (501) staff       (20)       15 2022-02-23 23:49:02.000000 mixpanel-utils-2.2.5/mixpanel_utils.egg-info/top_level.txt
--rw-r--r--   0 jaredmcfarland   (501) staff       (20)       38 2022-02-23 23:49:02.369555 mixpanel-utils-2.2.5/setup.cfg
--rw-r--r--   0 jaredmcfarland   (501) staff       (20)      580 2022-02-23 23:45:56.000000 mixpanel-utils-2.2.5/setup.py
+drwxr-xr-x   0 dpark      (505) staff       (20)        0 2024-05-17 21:43:21.961684 mixpanel_utils-2.2.6/
+-rw-r--r--   0 dpark      (505) staff       (20)    11923 2024-05-13 16:02:43.000000 mixpanel_utils-2.2.6/LICENSE
+-rw-r--r--   0 dpark      (505) staff       (20)      455 2024-05-17 21:43:21.961405 mixpanel_utils-2.2.6/PKG-INFO
+-rw-r--r--   0 dpark      (505) staff       (20)    19610 2024-05-13 16:02:43.000000 mixpanel_utils-2.2.6/README.md
+-rw-r--r--   0 dpark      (505) staff       (20)       38 2024-05-17 21:43:21.961749 mixpanel_utils-2.2.6/setup.cfg
+-rw-r--r--   0 dpark      (505) staff       (20)      573 2024-05-17 21:42:18.000000 mixpanel_utils-2.2.6/setup.py
+drwxr-xr-x   0 dpark      (505) staff       (20)        0 2024-05-17 21:43:21.956318 mixpanel_utils-2.2.6/src/
+drwxr-xr-x   0 dpark      (505) staff       (20)        0 2024-05-17 21:43:21.959442 mixpanel_utils-2.2.6/src/mixpanel_utils/
+-rwxr-xr-x   0 dpark      (505) staff       (20)   104799 2024-05-17 21:42:18.000000 mixpanel_utils-2.2.6/src/mixpanel_utils/__init__.py
+-rw-r--r--   0 dpark      (505) staff       (20)     3259 2024-05-17 16:21:43.000000 mixpanel_utils-2.2.6/src/mixpanel_utils/paginator.py
+drwxr-xr-x   0 dpark      (505) staff       (20)        0 2024-05-17 21:43:21.961115 mixpanel_utils-2.2.6/src/mixpanel_utils.egg-info/
+-rw-r--r--   0 dpark      (505) staff       (20)      455 2024-05-17 21:43:21.000000 mixpanel_utils-2.2.6/src/mixpanel_utils.egg-info/PKG-INFO
+-rw-r--r--   0 dpark      (505) staff       (20)      257 2024-05-17 21:43:21.000000 mixpanel_utils-2.2.6/src/mixpanel_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 dpark      (505) staff       (20)        1 2024-05-17 21:43:21.000000 mixpanel_utils-2.2.6/src/mixpanel_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 dpark      (505) staff       (20)       15 2024-05-17 21:43:21.000000 mixpanel_utils-2.2.6/src/mixpanel_utils.egg-info/top_level.txt
```

### Comparing `mixpanel-utils-2.2.5/mixpanel_utils/__init__.py` & `mixpanel_utils-2.2.6/src/mixpanel_utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1482,14 +1482,35 @@
         credentials = f"{amplitude_api_key}:{amplitude_api_secret}"
 
         extract_data_path = self._extract_amplitude_data(amplitude_export_url, credentials)
         self._transform_and_load_amplitude_data(extract_data_path)
 
         return
 
+    def import_from_amplitude_id_mgmt_v3(self, amplitude_api_key, amplitude_api_secret, start, end):
+        """Exports all data from an Amplitude project and imports it into Mixpanel
+
+            :param amplitude_api_key: Your Amplitude API key
+            :param amplitude_api_secret: Your Amplitude API secret
+            :param start: Date and time in the format of YYYYMMDDTHH (e.g. '20150201T05')
+            :param end: Date and time in the format of YYYYMMDDTHH (e.g. '20150203T20')
+
+            :type amplitude_api_key: string
+            :type amplitude_api_secret: string
+            :type start: string
+            :type end: string
+        """
+        amplitude_export_url = f"https://amplitude.com/api/2/export?start={start}&end={end}"
+        credentials = f"{amplitude_api_key}:{amplitude_api_secret}"
+
+        extract_data_path = self._extract_amplitude_data(amplitude_export_url, credentials)
+        self._transform_and_load_amplitude_data_id_mgmt_v3(extract_data_path)
+
+        return
+
     """
     Private, internal methods
     """
 
     @staticmethod
     def _unicode_urlencode(params):
         """URL encodes a dict of Mixpanel parameters
@@ -1737,21 +1758,21 @@
         :type filename: str
         :return: A list of Mixpanel events or profiles
         :rtype: list
 
         """
         item_list = []
         try:
-            with open(filename, "rbU") as item_file:
+            with open(filename, "rb") as item_file:
                 # First try loading it as a JSON list
                 item_list = json.load(item_file)
         except JSONDecodeError as e:
             if "Expecting value" in str(e):
                 # Based on the error message, try to treat it as CSV
-                with open(filename, "rU", encoding="utf-8") as item_file:
+                with open(filename, "r", encoding="utf-8") as item_file:
                     reader = csv.reader(item_file)
                     header = next(reader)
                     # Determine if the data is events or profiles based on keys in the header.
                     # NOTE: this will fail if it were profile data with a people property named 'event'
                     if "event" in header:
                         event_index = header.index("event")
                         distinct_id_index = header.index("distinct_id")
@@ -1772,15 +1793,15 @@
                         MixpanelUtils.LOGGER.error(
                             "Unable to determine Mixpanel data type: CSV header does not contain 'event' or '$distinct_id'"
                         )
                         return None
             else:
                 # Try treating the file as newline delimited JSON objects
                 item_list = []
-                with open(filename, "rbU") as item_file:
+                with open(filename, "rb") as item_file:
                     for item in item_file:
                         item_list.append(json.loads(item))
         except IOError:
             MixpanelUtils.LOGGER.error(
                 f"Error loading data from file: {filename}", exc_info=True
             )
 
@@ -2255,14 +2276,16 @@
         }
         return amplitude_to_mixpanel_map.get(property_name)
 
     def _transform_amplitude_profiles(self, amplitude_profile):
         properties = amplitude_profile["user_properties"]
         default_properties = {self._map_amplitude_property_to_mixpanel(key): value for key, value in
                               amplitude_profile.items() if self._map_amplitude_property_to_mixpanel(key)}
+        if amplitude_profile["user_properties"]["Name"]:
+            default_properties["$name"] = amplitude_profile["user_properties"]["Name"]
         profile = {
             "$token": self.token,
             "$distinct_id": amplitude_profile["user_id"],
             "$ip": amplitude_profile["ip_address"],
             "$properties": {**properties, **default_properties}
         }
 
@@ -2301,14 +2324,45 @@
         event = {
             "event": amplitude_event["event_type"],
             "properties": combined_properties
         }
 
         return event
 
+    def _transform_amplitude_events_id_mgmt_v3(self, amplitude_event):
+        event_dt = self._format_amplitude_time(amplitude_event["event_time"])
+
+        no_user_id_fallback = amplitude_event.get("device_id") or amplitude_event["amplitude_id"]
+
+        mixpanel_properties = {
+            "distinct_id": amplitude_event.get("user_id") or amplitude_event.get("device_id") or amplitude_event["amplitude_id"],
+            "$device_id": amplitude_event["device_id"],
+            "time": int(event_dt.timestamp() * 1000),
+            "ip": amplitude_event["ip_address"],
+            "mp_country_code": amplitude_event["country"],
+            "source": "amplitude",
+            "$user_id": amplitude_event.get("user_id") or amplitude_event.get("user_properties").get("user_id") or no_user_id_fallback,
+        }
+
+        default_properties = {
+            self._map_amplitude_property_to_mixpanel(key): value for key, value in amplitude_event.items()
+            if self._map_amplitude_property_to_mixpanel(key)
+        }
+        if "$insert_id" in default_properties:
+            default_properties["$insert_id"] = re.sub(r"[^a-zA-Z0-9-]", "", default_properties["$insert_id"])
+
+        combined_properties = {**mixpanel_properties, **amplitude_event["event_properties"], **default_properties}
+
+        event = {
+            "event": amplitude_event["event_type"],
+            "properties": combined_properties
+        }
+
+        return event
+
     def _dedupe_merge_events(self, merge_events):
         unique_merge_events = {}
         for event in merge_events:
             merge_pair = (event["properties"]["$distinct_ids"][0], event["properties"]["$distinct_ids"][1])
             if not unique_merge_events.get(merge_pair):
                 unique_merge_events[merge_pair] = event
 
@@ -2375,13 +2429,52 @@
 
                 self.import_people(transformed_profiles)
                 self.import_events(transformed_events, 0)
                 self.import_events(unique_merge_events, 0)
                 total_events += len(all_events)
 
             print(f"Imported {total_events} events")
+
+        except:
+            MixpanelUtils.LOGGER.error(
+                "Error transforming Amplitude data", exc_info=True
+            )
+            return
+
+    def _transform_and_load_amplitude_data_id_mgmt_v3(self, extract_data_path):
+        transform_data_path = "./amp_data/amplitude_transform"
+        try:
+            total_events = 0
+            for filename in os.listdir(extract_data_path):
+                all_events = []
+                with open(
+                    os.path.join(extract_data_path, filename), "r"
+                ) as extract_file:
+                    all_events = json.loads(extract_file.read())
+
+                transformed_profiles = [
+                    self._transform_amplitude_profiles(profile)
+                    for profile in all_events
+                    if profile["user_properties"]
+                ]
+                transformed_events = [
+                    self._transform_amplitude_events_id_mgmt_v3(event) for event in all_events
+                ]
+
+                unique_merge_events = [
+                    self._create_merge_event(event)
+                    for event in all_events
+                    if event.get("user_id") and event.get("amplitude_id")
+                ]
+
+                self.import_people(transformed_profiles)
+                self.import_events(transformed_events, 0)
+                self.import_events(unique_merge_events, 0)
+                total_events += len(all_events)
+
+            print(f"Imported {total_events} events")
 
         except:
             MixpanelUtils.LOGGER.error(
                 "Error transforming Amplitude data", exc_info=True
             )
             return
```

### Comparing `mixpanel-utils-2.2.5/mixpanel_utils/paginator.py` & `mixpanel_utils-2.2.6/src/mixpanel_utils/paginator.py`

 * *Files identical despite different names*

