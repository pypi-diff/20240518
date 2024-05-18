# Comparing `tmp/pycord-multicog-2.1.0.tar.gz` & `tmp/pycord-multicog-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycord-multicog-2.1.0.tar", last modified: Tue Apr  2 14:46:34 2024, max compression
+gzip compressed data, was "pycord-multicog-2.1.1.tar", last modified: Sat May 18 04:35:13 2024, max compression
```

## Comparing `pycord-multicog-2.1.0.tar` & `pycord-multicog-2.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:46:34.060705 pycord-multicog-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-02 14:46:20.000000 pycord-multicog-2.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-02 14:46:34.060705 pycord-multicog-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-02 14:46:20.000000 pycord-multicog-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:46:34.056705 pycord-multicog-2.1.0/pycord/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:46:34.060705 pycord-multicog-2.1.0/pycord/multicog/
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-02 14:46:20.000000 pycord-multicog-2.1.0/pycord/multicog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:46:34.060705 pycord-multicog-2.1.0/pycord_multicog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-02 14:46:34.000000 pycord-multicog-2.1.0/pycord_multicog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-02 14:46:34.000000 pycord-multicog-2.1.0/pycord_multicog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:46:34.000000 pycord-multicog-2.1.0/pycord_multicog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 14:46:34.000000 pycord-multicog-2.1.0/pycord_multicog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 14:46:34.000000 pycord-multicog-2.1.0/pycord_multicog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:46:34.060705 pycord-multicog-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-02 14:46:20.000000 pycord-multicog-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:35:13.912902 pycord-multicog-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-18 04:35:06.000000 pycord-multicog-2.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-18 04:35:13.908903 pycord-multicog-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-18 04:35:06.000000 pycord-multicog-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:35:13.908903 pycord-multicog-2.1.1/pycord/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:35:13.908903 pycord-multicog-2.1.1/pycord/multicog/
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-18 04:35:06.000000 pycord-multicog-2.1.1/pycord/multicog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:35:13.908903 pycord-multicog-2.1.1/pycord_multicog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-18 04:35:13.000000 pycord-multicog-2.1.1/pycord_multicog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-18 04:35:13.000000 pycord-multicog-2.1.1/pycord_multicog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 04:35:13.000000 pycord-multicog-2.1.1/pycord_multicog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 04:35:13.000000 pycord-multicog-2.1.1/pycord_multicog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-18 04:35:13.000000 pycord-multicog-2.1.1/pycord_multicog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 04:35:13.912902 pycord-multicog-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-18 04:35:06.000000 pycord-multicog-2.1.1/setup.py
```

### Comparing `pycord-multicog-2.1.0/LICENSE.txt` & `pycord-multicog-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycord-multicog-2.1.0/PKG-INFO` & `pycord-multicog-2.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycord-multicog
-Version: 2.1.0
+Version: 2.1.1
 Summary: A pycord extension that allows splitting command groups into multiple cogs
 Home-page: https://github.com/Dorukyum/pycord-multicog
 Author: Dorukyum
 License: MIT
 Project-URL: Source, https://github.com/Dorukyum/pycord-multicog
 Keywords: Pycord
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pycord-multicog-2.1.0/README.md` & `pycord-multicog-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pycord-multicog-2.1.0/pycord/multicog/__init__.py` & `pycord-multicog-2.1.1/pycord/multicog/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,19 +56,16 @@
 
     def _add_to_group(
         self, command: discord.SlashCommand, group: discord.SlashCommandGroup
     ) -> None:
         """A helper funcion to change attributes of a command to match those of the target group's."""
 
         index = multicog_commands.index(command)
-        command.cog, command.parent, command.guild_ids = (
-            group.cog,
-            group,
-            group.guild_ids,
-        )
+        command.parent = group
+        command.guild_ids = group.guild_ids
         group.add_command(command)
         multicog_commands[index] = command
 
     def _find_group(self, name: str) -> Optional[discord.SlashCommandGroup]:
         """A helper function to find and return a slash command group with the
         provided name.
         """
@@ -87,15 +84,14 @@
 
     def add_application_command(self, command: discord.ApplicationCommand) -> None:
         if isinstance(command, discord.SlashCommandGroup) and (
             group := self._find_group(command.name)
         ):
             for subcommand in group.subcommands:
                 command.subcommands.append(subcommand)
-                subcommand.cog = group.cog
 
             super().remove_application_command(group)
 
         if not (
             isinstance(command, discord.SlashCommand)
             and (meta := self._get_meta(command))
         ):
@@ -104,20 +100,18 @@
         if group := self._find_group(meta.group):
             return self._add_to_group(command, group)
 
         if meta.independent:
             options = meta.group_options or {}
             if " " not in meta.group:
                 group = discord.SlashCommandGroup(meta.group, **options)
-                group.cog = command.cog
                 self._add_to_group(command, group)
             else:
                 group_name, subgroup_name = meta.group.split(" ")
                 group = discord.SlashCommandGroup(group_name, **options)
-                group.cog = command.cog
                 subgroup = group.create_subgroup(subgroup_name)
                 self._add_to_group(command, subgroup)
 
             return super().add_application_command(group)
 
         raise ValueError(
             f"Command {command.name} is dependent yet group {meta.group} could "
@@ -135,18 +129,15 @@
             if (
                 not (isinstance(subcommand, discord.SlashCommand))
                 or not (meta := self._get_meta(subcommand))
                 or not meta.independent
             ):
                 command.subcommands.remove(subcommand)
 
-        if command.subcommands:
-            command.cog = command.subcommands[0].cog
-            return
-
-        return super().remove_application_command(command)
+        if not command.subcommands:
+            return super().remove_application_command(command)
 
 
 class AutoShardedBot(discord.AutoShardedBot, Bot):
     """A subclass of `discord.AutoShardedBot` that supports splitting
     command groups into multiple cogs.
     """
```

### Comparing `pycord-multicog-2.1.0/pycord_multicog.egg-info/PKG-INFO` & `pycord-multicog-2.1.1/pycord_multicog.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycord-multicog
-Version: 2.1.0
+Version: 2.1.1
 Summary: A pycord extension that allows splitting command groups into multiple cogs
 Home-page: https://github.com/Dorukyum/pycord-multicog
 Author: Dorukyum
 License: MIT
 Project-URL: Source, https://github.com/Dorukyum/pycord-multicog
 Keywords: Pycord
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pycord-multicog-2.1.0/setup.py` & `pycord-multicog-2.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="pycord-multicog",
     packages=["pycord.multicog"],
-    version="2.1.0",
+    version="2.1.1",
     license="MIT",
     description="A pycord extension that allows splitting command groups into multiple cogs",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Dorukyum",
     url="https://github.com/Dorukyum/pycord-multicog",
     keywords="Pycord",
```

