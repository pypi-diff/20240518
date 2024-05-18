# Comparing `tmp/physicslab-1.4.8.tar.gz` & `tmp/physicslab-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physicslab-1.4.8.tar", last modified: Sat May 11 15:59:14 2024, max compression
+gzip compressed data, was "physicslab-1.4.9.tar", last modified: Sat May 18 12:46:03 2024, max compression
```

## Comparing `physicslab-1.4.8.tar` & `physicslab-1.4.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:59:14.561728 physicslab-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-11 15:59:10.000000 physicslab-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-11 15:59:14.561728 physicslab-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-11 15:59:10.000000 physicslab-1.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:59:14.557728 physicslab-1.4.8/physicsLab/
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/_colorUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:59:14.557728 physicslab-1.4.8/physicsLab/celestial/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/celestial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/celestial/elementsClass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:59:14.557728 physicslab-1.4.8/physicsLab/circuit/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/circuit/elementXYZ.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:59:14.561728 physicslab-1.4.8/physicsLab/circuit/elements/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/circuit/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/circuit/elements/_elementBase.py
--rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/circuit/elements/artificialCircuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/circuit/elements/basicCircuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    18290 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/circuit/elements/logicCircuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/circuit/elements/otherCircuit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/circuit/wire.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:59:14.561728 physicslab-1.4.8/physicsLab/electromagnetism/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/electromagnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/electromagnetism/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/element.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/elementBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    28498 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/experimentType.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:59:14.561728 physicslab-1.4.8/physicsLab/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/lib/_unionClassHead.py
--rw-r--r--   0 runner    (1001) docker     (127)    19381 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/lib/logic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/lib/wires.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:59:14.561728 physicslab-1.4.8/physicsLab/music/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/music/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26688 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/music/music.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/savTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/typehint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:59:14.561728 physicslab-1.4.8/physicsLab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-11 15:59:14.000000 physicslab-1.4.8/physicsLab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-11 15:59:14.000000 physicslab-1.4.8/physicsLab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 15:59:14.000000 physicslab-1.4.8/physicsLab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-11 15:59:14.000000 physicslab-1.4.8/physicsLab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-11 15:59:14.000000 physicslab-1.4.8/physicsLab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 15:59:14.561728 physicslab-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-11 15:59:10.000000 physicslab-1.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:46:03.377227 physicslab-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-18 12:45:59.000000 physicslab-1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-18 12:46:03.373227 physicslab-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-18 12:45:59.000000 physicslab-1.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:46:03.369227 physicslab-1.4.9/physicsLab/
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/_colorUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:46:03.373227 physicslab-1.4.9/physicsLab/celestial/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/celestial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/celestial/elementsClass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:46:03.373227 physicslab-1.4.9/physicsLab/circuit/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/circuit/elementXYZ.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:46:03.373227 physicslab-1.4.9/physicsLab/circuit/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/circuit/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/circuit/elements/_elementBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/circuit/elements/artificialCircuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/circuit/elements/basicCircuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18290 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/circuit/elements/logicCircuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/circuit/elements/otherCircuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/circuit/wire.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:46:03.373227 physicslab-1.4.9/physicsLab/electromagnetism/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/electromagnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/electromagnetism/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/elementBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28498 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/experimentType.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:46:03.373227 physicslab-1.4.9/physicsLab/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/lib/_unionClassHead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19381 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/lib/logic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/lib/wires.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:46:03.373227 physicslab-1.4.9/physicsLab/music/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/music/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27351 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/music/music.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/savTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-18 12:45:59.000000 physicslab-1.4.9/physicsLab/typehint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:46:03.373227 physicslab-1.4.9/physicsLab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-18 12:46:03.000000 physicslab-1.4.9/physicsLab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-18 12:46:03.000000 physicslab-1.4.9/physicsLab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 12:46:03.000000 physicslab-1.4.9/physicsLab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-18 12:46:03.000000 physicslab-1.4.9/physicsLab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-18 12:46:03.000000 physicslab-1.4.9/physicsLab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 12:46:03.377227 physicslab-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-18 12:45:59.000000 physicslab-1.4.9/setup.py
```

### Comparing `physicslab-1.4.8/LICENSE` & `physicslab-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/PKG-INFO` & `physicslab-1.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsLab
-Version: 1.4.8
+Version: 1.4.9
 Summary: Python API for Physics-Lab-AR
 Home-page: https://gitee.com/script2000/physicsLab
 Author: Goodenough
 Author-email: 2381642961@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `physicslab-1.4.8/README.md` & `physicslab-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/physicsLab/__init__.py` & `physicslab-1.4.9/physicsLab/__init__.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/physicsLab/_colorUtils.py` & `physicslab-1.4.9/physicsLab/_colorUtils.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/physicsLab/_tools.py` & `physicslab-1.4.9/physicsLab/_tools.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/physicsLab/circuit/elementXYZ.py` & `physicslab-1.4.9/physicsLab/circuit/elementXYZ.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/physicsLab/circuit/elements/_elementBase.py` & `physicslab-1.4.9/physicsLab/circuit/elements/_elementBase.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/physicsLab/circuit/elements/artificialCircuit.py` & `physicslab-1.4.9/physicsLab/circuit/elements/artificialCircuit.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/physicsLab/circuit/elements/basicCircuit.py` & `physicslab-1.4.9/physicsLab/circuit/elements/basicCircuit.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/physicsLab/circuit/elements/logicCircuit.py` & `physicslab-1.4.9/physicsLab/circuit/elements/logicCircuit.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/physicsLab/circuit/elements/otherCircuit.py` & `physicslab-1.4.9/physicsLab/circuit/elements/otherCircuit.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/physicsLab/circuit/wire.py` & `physicslab-1.4.9/physicsLab/circuit/wire.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/physicsLab/electromagnetism/elements.py` & `physicslab-1.4.9/physicsLab/electromagnetism/elements.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/physicsLab/element.py` & `physicslab-1.4.9/physicsLab/element.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/physicsLab/errors.py` & `physicslab-1.4.9/physicsLab/errors.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/physicsLab/experiment.py` & `physicslab-1.4.9/physicsLab/experiment.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/physicsLab/lib/_unionClassHead.py` & `physicslab-1.4.9/physicsLab/lib/_unionClassHead.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/physicsLab/lib/logic.py` & `physicslab-1.4.9/physicsLab/lib/logic.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/physicsLab/lib/wires.py` & `physicslab-1.4.9/physicsLab/lib/wires.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/physicsLab/music/music.py` & `physicslab-1.4.9/physicsLab/music/music.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,35 +72,29 @@
             raise FileNotFoundError
 
         if midifile.endswith(".mido.py"):
             read_midopy(midifile)
         else:
             self.midifile: str = midifile
 
-        self.channels: List[int] = [0] * 16
-        self.tempo: int = 500_000
         self.messages: mido.MidiTrack = self.__get_midi_messages()
 
-    # 使用mido打开一个midi文件并获取其tracks
     def __get_midi_messages(self) -> mido.MidiTrack:
+        ''' 使用mido打开一个midi文件并获取其messages '''
         self._midifile = mido.MidiFile(self.midifile, clip=True)
         wait_time: numType = 0
         res = mido.MidiTrack()
         for msg in self._midifile.merged_track:
             if msg.type in ("note_on", "note_off", "program_change", "set_tempo"):
                 res.append(msg)
                 msg.time += wait_time
                 wait_time = 0
             elif msg.time != 0:
                 wait_time += msg.time
 
-            if msg.type == "program_change":
-                self.channels[msg.channel] = msg.program
-            if msg.type == "set_tempo":
-                self.tempo = msg.tempo
         return res
 
     # 播放midi类存储的信息
     def sound(self, player: Optional[PLAYER] = None, is_sourcefile: bool = False) -> Self:
         # 使用plmidi播放midi
         def sound_by_plmidi() -> bool:
             try:
@@ -172,46 +166,59 @@
         elif sound_by_os():
             pass
         else:
             errors.warning("can not use sound methods")
 
         return self
 
-    # 将time重设为原来的num倍
     def set_tempo(self, num: numType = 1) -> Self:
+        ''' 将time重设为原来的num倍 '''
         if not isinstance(num, (int, float)):
             raise TypeError
 
         for msg in self.messages:
             msg.time *= num
 
         return self
 
     # 返回 [Note(...), Chord(...), ...]
     def _get_notes_list(self,
-                        div_time: numType, max_notes: Optional[int],
-                        is_fix_strange_note: bool = False,
+                        div_time: Optional[numType],
+                        max_notes: Optional[int],
+                        fix_strange_note: bool = False,
                         ) -> List[Union["Note", "Chord"]]:
 
         res: List[Union[Note, Chord]] = []
         wait_time: int = 0
         len_res: int = 0
+        channels: List[int] = [0] * 16
+        tempo: int = 500_000
+        _div_time = div_time
 
         for msg in self.messages:
+            if msg.type == "program_change":
+                channels[msg.channel] = msg.program
+            if msg.type == "set_tempo":
+                tempo = msg.tempo
+                if div_time is None:
+                    _div_time = mido.second2tick(0.11, self._midifile.ticks_per_beat, tempo)
+
             if msg.type == "note_on":
                 velocity: float = _format_velocity(msg.velocity / 127) # 音符的响度
-                ins: int = self.channels[msg.channel]
+                ins: int = channels[msg.channel]
 
-                if velocity == 0 or (is_fix_strange_note and ins == 0 and velocity >= 0.85):
+                if velocity == 0 or (fix_strange_note and ins == 0 and velocity >= 0.85):
                     if msg.time != 0:
                         wait_time += msg.time
                     continue
 
                 len_res += 1
-                note_time = round((msg.time + wait_time) / div_time)
+                if _div_time is None:
+                    raise RuntimeError("find some error in midifile, please manually pass in the div_time parameter")
+                note_time = round((msg.time + wait_time) / _div_time)
 
                 if note_time != 0 or len(res) == 0:
                     if note_time == 0:
                         note_time = 1
                     res.append(Note(time=note_time, instrument=ins, pitch=msg.note, velocity=velocity))
                 else:
                     # res[-1]是`Note`或`Chord`且在赋值之后一定是Chord, 此时Note的time的值不重要(因为和弦的音符是同时播放的)
@@ -222,21 +229,22 @@
 
             if max_notes is not None and len_res >= max_notes:
                 break
 
         return res
 
     def to_piece(self,
-                 div_time: numType = 100,
+                 div_time: Optional[numType] = None,
                  max_notes: Optional[int] = 800,
                  is_optimize: bool = True, # 是否将多个音符优化为和弦
-                 is_fix_strange_note: bool = False, # 是否修正一些奇怪的音符
+                 fix_strange_note: bool = False, # 是否修正一些奇怪的音符
                  ) -> "Piece":
         ''' 转换为Piece类 '''
-        return Piece(self._get_notes_list(div_time, max_notes, is_fix_strange_note),
+
+        return Piece(self._get_notes_list(div_time, max_notes, fix_strange_note),
                      is_optimize=is_optimize)
 
     ''' *.pl.py文件:
         pl即为 physicsLab file
         为了更方便于手动调控物实音乐电路的生成而诞生的文件格式
         该文件运行之后即可生成对应的物实播放音乐电路
     '''
@@ -252,44 +260,48 @@
         if not path.endswith(".mido.py"):
             path += ".mido.py"
 
         with open(path, "w", encoding="utf-8") as f:
             f.write(f"import os\n"
                     f"os.environ['PYGAME_HIDE_SUPPORT_PROMPT'] = '1'\n"
                     f"from mido import MidiFile, MidiTrack, MetaMessage, Message\n"
-                    f"mid = MidiFile()\n"
-                    f"track = {str(self.messages)}\n"
+                    f"mid = MidiFile(type={self._midifile.type}, "
+                    f"ticks_per_beat={self._midifile.ticks_per_beat}, "
+                    f"charset='{self._midifile.charset}', "
+                    f"clip={self._midifile.clip})\n"
+                    f"track = {self.messages}\n"
                     f"mid.tracks.append(track)\n"
                     f"mid.save(\"temp.mid\")\n"
                     f"from physicsLab.music import Midi\n"
                     f"Midi(\"temp.mid\").sound()")
 
         return self
 
-    # 以 .mid 的形式导出, read_midi已经在Midi的__init__中实现
     def write_midi(self, midipath: str = "temp.mid") -> Self:
+        """ 导出一个 .mid 文件 """
         if not isinstance(midipath, str):
             raise TypeError
         if not midipath.endswith(".mid"):
             midipath += ".mid"
 
-        mid = mido.MidiFile()
+        mid = mido.MidiFile(ticks_per_beat=self._midifile.ticks_per_beat,
+                            type=self._midifile.type,
+                            charset=self._midifile.charset)
         mid.tracks.append(self.messages)
         mid.save(midipath)
 
         return self
 
-    # 以.pl.py的格式导出, div_time: midi的time的单位长度与Note的time的单位长度不同，支持用户手动调整
-    # max_notes: 最大的音符数，因为物实没法承受过多的元件
     def write_plpy(self,
                   filepath: str = "temp.pl.py",
-                  div_time: numType = 100,
-                  max_notes: Optional[int] = 800,
+                  div_time: numType = 100, # midi的time的单位长度与Note的time的单位长度不同，支持用户手动调整
+                  max_notes: Optional[int] = 800, # 最大的音符数，因为物实没法承受过多的元件
                   sav_name: str = "temp" # 产生的存档的名字, 也可直接在生成.pl.py中修改
     ) -> Self:
+        ''' 以.pl.py的格式导出 '''
         if not (isinstance(div_time, (int, float)) or
                 isinstance(max_notes, int)) and max_notes is not None:
            raise TypeError
 
         if not filepath.endswith(".pl.py"):
             filepath += ".pl.py"
```

### Comparing `physicslab-1.4.8/physicsLab/savTemplate.py` & `physicslab-1.4.9/physicsLab/savTemplate.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/physicsLab.egg-info/PKG-INFO` & `physicslab-1.4.9/physicsLab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsLab
-Version: 1.4.8
+Version: 1.4.9
 Summary: Python API for Physics-Lab-AR
 Home-page: https://gitee.com/script2000/physicsLab
 Author: Goodenough
 Author-email: 2381642961@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `physicslab-1.4.8/physicsLab.egg-info/SOURCES.txt` & `physicslab-1.4.9/physicsLab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.8/setup.py` & `physicslab-1.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 import setuptools
 
 setuptools.setup(
     name="physicsLab",
-    version="1.4.8",
+    version="1.4.9",
     license="MIT",
     author="Goodenough",
     author_email="2381642961@qq.com",
     description="Python API for Physics-Lab-AR",
     long_description="click \"[there](https://gitee.com/script2000/physicsLab)\" to show more information",
     long_description_content_type="text/markdown",
     url="https://gitee.com/script2000/physicsLab",
```

