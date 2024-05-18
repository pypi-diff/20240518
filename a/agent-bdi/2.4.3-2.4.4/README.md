# Comparing `tmp/agent-bdi-2.4.3.tar.gz` & `tmp/agent-bdi-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent-bdi-2.4.3.tar", last modified: Sun May  5 19:53:48 2024, max compression
+gzip compressed data, was "agent-bdi-2.4.4.tar", last modified: Sat May 18 16:05:47 2024, max compression
```

## Comparing `agent-bdi-2.4.3.tar` & `agent-bdi-2.4.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 19:53:48.684872 agent-bdi-2.4.3/
--rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.3/LICENSE.md
--rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3202 2024-05-05 19:53:48.682873 agent-bdi-2.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     2650 2023-04-25 11:32:48.000000 agent-bdi-2.4.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 19:53:48.684872 agent-bdi-2.4.3/setup.cfg
--rw-rw-rw-   0        0        0      885 2024-05-05 19:53:15.000000 agent-bdi-2.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:53:48.629913 agent-bdi-2.4.3/src/
--rw-rw-rw-   0        0        0        0 2024-01-04 04:28:19.000000 agent-bdi-2.4.3/src/__init__.py
--rw-rw-rw-   0        0        0      657 2024-01-04 04:28:19.000000 agent-bdi-2.4.3/src/abdi_config.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:53:48.647598 agent-bdi-2.4.3/src/agent_bdi.egg-info/
--rw-rw-rw-   0        0        0     3202 2024-05-05 19:53:48.000000 agent-bdi-2.4.3/src/agent_bdi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1084 2024-05-05 19:53:48.000000 agent-bdi-2.4.3/src/agent_bdi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 19:53:48.000000 agent-bdi-2.4.3/src/agent_bdi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-05 19:53:48.000000 agent-bdi-2.4.3/src/agent_bdi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-05 19:53:48.657714 agent-bdi-2.4.3/src/broker/
--rw-rw-rw-   0        0        0      134 2023-12-25 14:17:27.000000 agent-bdi-2.4.3/src/broker/__init__.py
--rw-rw-rw-   0        0        0      964 2023-12-25 14:17:27.000000 agent-bdi-2.4.3/src/broker/broker_maker.py
--rw-rw-rw-   0        0        0      943 2024-01-04 04:28:19.000000 agent-bdi-2.4.3/src/broker/empty_broker.py
--rw-rw-rw-   0        0        0      645 2023-12-25 14:17:27.000000 agent-bdi-2.4.3/src/broker/message_broker.py
--rw-rw-rw-   0        0        0     2186 2024-03-13 16:08:10.000000 agent-bdi-2.4.3/src/broker/mqtt_broker.py
--rw-rw-rw-   0        0        0      383 2023-12-25 14:17:27.000000 agent-bdi-2.4.3/src/broker/notifier.py
--rw-rw-rw-   0        0        0      903 2024-01-04 04:28:19.000000 agent-bdi-2.4.3/src/broker/redis_broker.py
--rw-rw-rw-   0        0        0      897 2024-01-04 04:28:19.000000 agent-bdi-2.4.3/src/broker/ros_broker.py
--rw-rw-rw-   0        0        0     2651 2024-01-04 04:28:19.000000 agent-bdi-2.4.3/src/broker/ros_noetic_broker.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:53:48.662769 agent-bdi-2.4.3/src/core/
--rw-rw-rw-   0        0        0      316 2023-05-22 15:55:38.000000 agent-bdi-2.4.3/src/core/Agent.py
--rw-rw-rw-   0        0        0       58 2023-04-25 11:32:48.000000 agent-bdi-2.4.3/src/core/Belief.py
--rw-rw-rw-   0        0        0       52 2023-04-25 11:32:48.000000 agent-bdi-2.4.3/src/core/Desire.py
--rw-rw-rw-   0        0        0       55 2023-04-25 11:32:48.000000 agent-bdi-2.4.3/src/core/Intention.py
--rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.3/src/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:53:48.670283 agent-bdi-2.4.3/src/holon/
--rw-rw-rw-   0        0        0      116 2023-04-25 11:32:48.000000 agent-bdi-2.4.3/src/holon/Blackboard.py
--rw-rw-rw-   0        0        0      452 2023-05-28 19:59:05.000000 agent-bdi-2.4.3/src/holon/Heart.py
--rw-rw-rw-   0        0        0     9856 2024-05-04 16:12:54.000000 agent-bdi-2.4.3/src/holon/HolonicAgent.py
--rw-rw-rw-   0        0        0       72 2023-04-25 11:32:48.000000 agent-bdi-2.4.3/src/holon/HolonicDesire.py
--rw-rw-rw-   0        0        0       84 2023-04-25 11:32:48.000000 agent-bdi-2.4.3/src/holon/HolonicIntention.py
--rw-rw-rw-   0        0        0        0 2023-12-25 14:17:27.000000 agent-bdi-2.4.3/src/holon/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:53:48.676791 agent-bdi-2.4.3/src/holon/logistics/
--rw-rw-rw-   0        0        0        0 2024-02-13 16:04:18.000000 agent-bdi-2.4.3/src/holon/logistics/__init__.py
--rw-rw-rw-   0        0        0      722 2024-04-27 17:02:10.000000 agent-bdi-2.4.3/src/holon/logistics/base_logistic.py
--rw-rw-rw-   0        0        0      356 2024-02-07 10:01:09.000000 agent-bdi-2.4.3/src/holon/logistics/broker_logistic.py
--rw-rw-rw-   0        0        0     5299 2024-02-26 10:20:43.000000 agent-bdi-2.4.3/src/holon/logistics/loading_coordinator.py
--rw-rw-rw-   0        0        0     6781 2024-05-04 16:12:54.000000 agent-bdi-2.4.3/src/holon/logistics/payload_wrapper.py
--rw-rw-rw-   0        0        0     2399 2024-05-05 19:26:36.000000 agent-bdi-2.4.3/src/holon/logistics/request_logistic.py
--rw-rw-rw-   0        0        0     3552 2024-05-05 19:27:29.000000 agent-bdi-2.4.3/src/holon/logistics/response_logistic.py
--rw-rw-rw-   0        0        0       80 2024-01-05 16:48:07.000000 agent-bdi-2.4.3/src/holon/payload.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:53:48.681789 agent-bdi-2.4.3/tests/
--rw-rw-rw-   0        0        0      404 2024-04-27 15:27:38.000000 agent-bdi-2.4.3/tests/test01.py
--rw-rw-rw-   0        0        0     1837 2024-02-15 11:41:34.000000 agent-bdi-2.4.3/tests/test_loadingbal.py
--rw-rw-rw-   0        0        0     2318 2024-01-06 16:12:29.000000 agent-bdi-2.4.3/tests/test_request.py
--rw-rw-rw-   0        0        0     2754 2024-01-06 16:34:09.000000 agent-bdi-2.4.3/tests/test_send.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:05:47.234370 agent-bdi-2.4.4/
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.4/LICENSE.md
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3202 2024-05-18 16:05:47.233369 agent-bdi-2.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2650 2023-04-25 11:32:48.000000 agent-bdi-2.4.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-18 16:05:47.234370 agent-bdi-2.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      885 2024-05-18 16:04:56.000000 agent-bdi-2.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:05:47.050170 agent-bdi-2.4.4/src/
+-rw-rw-rw-   0        0        0        0 2024-01-04 04:28:19.000000 agent-bdi-2.4.4/src/__init__.py
+-rw-rw-rw-   0        0        0      657 2024-01-04 04:28:19.000000 agent-bdi-2.4.4/src/abdi_config.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:05:47.067186 agent-bdi-2.4.4/src/agent_bdi.egg-info/
+-rw-rw-rw-   0        0        0     3202 2024-05-18 16:05:46.000000 agent-bdi-2.4.4/src/agent_bdi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1084 2024-05-18 16:05:46.000000 agent-bdi-2.4.4/src/agent_bdi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 16:05:46.000000 agent-bdi-2.4.4/src/agent_bdi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-18 16:05:46.000000 agent-bdi-2.4.4/src/agent_bdi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 16:05:47.089997 agent-bdi-2.4.4/src/broker/
+-rw-rw-rw-   0        0        0      134 2023-12-25 14:17:27.000000 agent-bdi-2.4.4/src/broker/__init__.py
+-rw-rw-rw-   0        0        0      964 2023-12-25 14:17:27.000000 agent-bdi-2.4.4/src/broker/broker_maker.py
+-rw-rw-rw-   0        0        0      943 2024-01-04 04:28:19.000000 agent-bdi-2.4.4/src/broker/empty_broker.py
+-rw-rw-rw-   0        0        0      645 2023-12-25 14:17:27.000000 agent-bdi-2.4.4/src/broker/message_broker.py
+-rw-rw-rw-   0        0        0     2186 2024-03-13 16:08:10.000000 agent-bdi-2.4.4/src/broker/mqtt_broker.py
+-rw-rw-rw-   0        0        0      383 2023-12-25 14:17:27.000000 agent-bdi-2.4.4/src/broker/notifier.py
+-rw-rw-rw-   0        0        0      903 2024-01-04 04:28:19.000000 agent-bdi-2.4.4/src/broker/redis_broker.py
+-rw-rw-rw-   0        0        0      897 2024-01-04 04:28:19.000000 agent-bdi-2.4.4/src/broker/ros_broker.py
+-rw-rw-rw-   0        0        0     2651 2024-01-04 04:28:19.000000 agent-bdi-2.4.4/src/broker/ros_noetic_broker.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:05:47.107428 agent-bdi-2.4.4/src/core/
+-rw-rw-rw-   0        0        0      316 2023-05-22 15:55:38.000000 agent-bdi-2.4.4/src/core/Agent.py
+-rw-rw-rw-   0        0        0       58 2023-04-25 11:32:48.000000 agent-bdi-2.4.4/src/core/Belief.py
+-rw-rw-rw-   0        0        0       52 2023-04-25 11:32:48.000000 agent-bdi-2.4.4/src/core/Desire.py
+-rw-rw-rw-   0        0        0       55 2023-04-25 11:32:48.000000 agent-bdi-2.4.4/src/core/Intention.py
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.4/src/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:05:47.127034 agent-bdi-2.4.4/src/holon/
+-rw-rw-rw-   0        0        0      116 2023-04-25 11:32:48.000000 agent-bdi-2.4.4/src/holon/Blackboard.py
+-rw-rw-rw-   0        0        0      452 2023-05-28 19:59:05.000000 agent-bdi-2.4.4/src/holon/Heart.py
+-rw-rw-rw-   0        0        0     9856 2024-05-04 16:12:54.000000 agent-bdi-2.4.4/src/holon/HolonicAgent.py
+-rw-rw-rw-   0        0        0       72 2023-04-25 11:32:48.000000 agent-bdi-2.4.4/src/holon/HolonicDesire.py
+-rw-rw-rw-   0        0        0       84 2023-04-25 11:32:48.000000 agent-bdi-2.4.4/src/holon/HolonicIntention.py
+-rw-rw-rw-   0        0        0        0 2023-12-25 14:17:27.000000 agent-bdi-2.4.4/src/holon/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:05:47.179896 agent-bdi-2.4.4/src/holon/logistics/
+-rw-rw-rw-   0        0        0        0 2024-02-13 16:04:18.000000 agent-bdi-2.4.4/src/holon/logistics/__init__.py
+-rw-rw-rw-   0        0        0      722 2024-04-27 17:02:10.000000 agent-bdi-2.4.4/src/holon/logistics/base_logistic.py
+-rw-rw-rw-   0        0        0      356 2024-02-07 10:01:09.000000 agent-bdi-2.4.4/src/holon/logistics/broker_logistic.py
+-rw-rw-rw-   0        0        0     5283 2024-05-11 08:16:35.000000 agent-bdi-2.4.4/src/holon/logistics/loading_coordinator.py
+-rw-rw-rw-   0        0        0     6780 2024-05-07 17:25:25.000000 agent-bdi-2.4.4/src/holon/logistics/payload_wrapper.py
+-rw-rw-rw-   0        0        0     3335 2024-05-18 14:28:14.000000 agent-bdi-2.4.4/src/holon/logistics/request_logistic.py
+-rw-rw-rw-   0        0        0     5112 2024-05-18 14:31:46.000000 agent-bdi-2.4.4/src/holon/logistics/response_logistic.py
+-rw-rw-rw-   0        0        0       80 2024-01-05 16:48:07.000000 agent-bdi-2.4.4/src/holon/payload.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:05:47.231361 agent-bdi-2.4.4/tests/
+-rw-rw-rw-   0        0        0      404 2024-04-27 15:27:38.000000 agent-bdi-2.4.4/tests/test01.py
+-rw-rw-rw-   0        0        0     1837 2024-02-15 11:41:34.000000 agent-bdi-2.4.4/tests/test_loadingbal.py
+-rw-rw-rw-   0        0        0     2318 2024-01-06 16:12:29.000000 agent-bdi-2.4.4/tests/test_request.py
+-rw-rw-rw-   0        0        0     2754 2024-01-06 16:34:09.000000 agent-bdi-2.4.4/tests/test_send.py
```

### Comparing `agent-bdi-2.4.3/PKG-INFO` & `agent-bdi-2.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-bdi
-Version: 2.4.3
+Version: 2.4.4
 Summary: Agent BDI framework
 Home-page: https://github.com/mfshiu/abdi.git
 Author: Ming Fang Shiu
 Author-email: avatar.xu@gmail.com
 Project-URL: Bug Tracker, https://bugtracker.zoho.com/portal/avatardotxugmaildotcom#allprojects/1982079000000043717/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agent-bdi-2.4.3/README.md` & `agent-bdi-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.3/setup.py` & `agent-bdi-2.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "agent-bdi",
-    version = "2.4.3",
+    version = "2.4.4",
     author = "Ming Fang Shiu",
     author_email='avatar.xu@gmail.com',
     description='Agent BDI framework',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/mfshiu/abdi.git",
     project_urls = {
```

### Comparing `agent-bdi-2.4.3/src/abdi_config.py` & `agent-bdi-2.4.4/src/abdi_config.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.3/src/agent_bdi.egg-info/PKG-INFO` & `agent-bdi-2.4.4/src/agent_bdi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-bdi
-Version: 2.4.3
+Version: 2.4.4
 Summary: Agent BDI framework
 Home-page: https://github.com/mfshiu/abdi.git
 Author: Ming Fang Shiu
 Author-email: avatar.xu@gmail.com
 Project-URL: Bug Tracker, https://bugtracker.zoho.com/portal/avatardotxugmaildotcom#allprojects/1982079000000043717/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agent-bdi-2.4.3/src/agent_bdi.egg-info/SOURCES.txt` & `agent-bdi-2.4.4/src/agent_bdi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.3/src/broker/broker_maker.py` & `agent-bdi-2.4.4/src/broker/broker_maker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.3/src/broker/empty_broker.py` & `agent-bdi-2.4.4/src/broker/empty_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.3/src/broker/message_broker.py` & `agent-bdi-2.4.4/src/broker/message_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.3/src/broker/mqtt_broker.py` & `agent-bdi-2.4.4/src/broker/mqtt_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.3/src/broker/redis_broker.py` & `agent-bdi-2.4.4/src/broker/redis_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.3/src/broker/ros_broker.py` & `agent-bdi-2.4.4/src/broker/ros_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.3/src/broker/ros_noetic_broker.py` & `agent-bdi-2.4.4/src/broker/ros_noetic_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.3/src/holon/HolonicAgent.py` & `agent-bdi-2.4.4/src/holon/HolonicAgent.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.3/src/holon/logistics/base_logistic.py` & `agent-bdi-2.4.4/src/holon/logistics/base_logistic.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.3/src/holon/logistics/loading_coordinator.py` & `agent-bdi-2.4.4/src/holon/logistics/loading_coordinator.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         logger.debug(f"{self.agent.short_id}> Candidates: {self.candidates}")
         # logger.debug(f"{self.agent.short_id}> candidates size: {len(self.candidates)}")
         if len(self.candidates):
             min_agent = min(self.candidates, key=lambda x: (x['rank_number'], x['agent_id']))
             if self.agent.agent_id == min_agent['agent_id']:
                 logger.info(f"{self.agent.short_id}> Elected for topic: {topic}, payload: {payload}")
                 self.agent.publish(f"{HEADER_ELECTED}.{topic}", self.agent.agent_id)
-                
+
                 if self.topic_handler:
                     self.topic_handler(topic, payload)
                 else:
                     self.agent.on_message(topic, payload)
         
         
     def elected(self, topic:str, payload):
```

### Comparing `agent-bdi-2.4.3/src/holon/logistics/payload_wrapper.py` & `agent-bdi-2.4.4/src/holon/logistics/payload_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
             
         return acceptable
 
         
     def unpack(self, payload:str):
         payload_text = payload.decode('utf-8')
         payload_json = json.loads(payload_text[len(WRAPPER_REQUEST_HEAD):])
-        logger.debug(f"payload_json: {str(payload_json)[:300]}...")
+        logger.debug(f"payload_json: {str(payload_json)[:300]}..")
         if VERSION != payload_json["version"]:
             raise Exception("Invalid payload version.")
         return payload_json
 
 
     def wrap_for_request(self, payload, request_id, source_payload) -> str:
         request_json = self.payload_wrapper.create_request_json(payload, request_id, source_payload)
```

### Comparing `agent-bdi-2.4.3/src/holon/logistics/request_logistic.py` & `agent-bdi-2.4.4/src/holon/logistics/request_logistic.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,43 +11,67 @@
 SUBSCRIBE_HEADER = "@response"
 
 
 class RequestLogistic(BaseLogistic):
     __handlers = {}
     
     
-    def __init__(self, agent:HolonicAgent, request_id=""):
+    def __init__(self, agent:HolonicAgent, request_id="", job_topic=None):
         self.agent = agent
+        self.job_topic = job_topic
         self.request_id = request_id
         self.response_topic_header = f"{SUBSCRIBE_HEADER}.{self.agent.agent_id}.{self.request_id}"
         logger.debug(f"self, agent_id: {self.agent.agent_id}, short_id: {self.agent.short_id}, request_id: {self.request_id}")
         self._payload_wrapper = PayloadWrapper(self.agent.agent_id)
         
         
+    # def publish(self, payload, source_payload=None):
+    #     if not self.job_topic:
+    #         raise Exception("The job topic has not been set yet.")
+    #     self.publish(self.job_topic, payload, source_payload)
+        
+        
     def publish(self, topic, payload, source_payload=None):
-        logger.debug(f"topic: {topic}, source_payload: {str(source_payload)[:300]}")
+        if not topic:
+            if self.job_topic:
+                topic = self.job_topic
+            else:
+                raise Exception("The job topic has not been set yet.")
+
+        logger.debug(f"topic: {topic}, source_payload: {str(source_payload)[:300]}..")
         logistic_topic = f"{PUBLISH_HEADER}.{topic}"
         logger.debug(f"agent_id: {self.agent.agent_id}, request_id: {self.request_id}")
         packed_payload, request_token = self._payload_wrapper.wrap_for_request(payload, self.request_id, source_payload)
         logger.debug(f"logistic_topic: {logistic_topic}, packed_payload: {str(packed_payload)[:300]}..")
         self.agent.publish(logistic_topic, packed_payload)
 
         return request_token
 
 
-    def subscribe(self, topic, topic_handler=None, datatype="str"):
+    # def subscribeA(self, topic_handler=None, datatype="str"):
+    #     if not self.job_topic:
+    #         raise Exception("The job topic has not been set yet.")
+    #     self.subscribe(self.job_topic, topic_handler, datatype)
+        
+        
+    def subscribe(self, topic=None, topic_handler=None, datatype="str"):
+        if not topic:
+            if self.job_topic:
+                topic = self.job_topic
+            else:
+                raise Exception("The job topic has not been set yet.")
         response_topic = f"{self.response_topic_header}.{topic}"
         logger.debug(f"response_topic: {response_topic}")
         self.agent.subscribe(response_topic, datatype, self.handle_response)
         RequestLogistic.__handlers[self.response_topic_header] = topic_handler
 
 
     def handle_response(self, topic:str, payload):
         responsed_topic = topic[len(self.response_topic_header)+1:]
         unpacked = self._payload_wrapper.unpack(payload)
-        logger.debug(f"topic: {topic}, unpacked: {str(unpacked)[:300]}")
+        logger.debug(f"topic: {topic}, unpacked: {str(unpacked)[:300]}..")
 
         if topic_handler := RequestLogistic.__handlers[self.response_topic_header]:
             self.agent.set_topic_handler(responsed_topic, topic_handler)
         self.agent._on_message(topic=responsed_topic, 
                                payload=unpacked["content"], 
                                source_payload=unpacked)
```

### Comparing `agent-bdi-2.4.3/tests/test_loadingbal.py` & `agent-bdi-2.4.4/tests/test_loadingbal.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.3/tests/test_request.py` & `agent-bdi-2.4.4/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.3/tests/test_send.py` & `agent-bdi-2.4.4/tests/test_send.py`

 * *Files identical despite different names*

