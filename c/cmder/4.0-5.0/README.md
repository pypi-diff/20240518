# Comparing `tmp/cmder-4.0.tar.gz` & `tmp/cmder-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmder-4.0.tar", last modified: Tue Apr 30 04:41:42 2024, max compression
+gzip compressed data, was "cmder-5.0.tar", last modified: Sat May 18 06:00:09 2024, max compression
```

## Comparing `cmder-4.0.tar` & `cmder-5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:41:42.428839 cmder-4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-30 04:41:36.000000 cmder-4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-30 04:41:42.428839 cmder-4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-30 04:41:36.000000 cmder-4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-30 04:41:36.000000 cmder-4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-30 04:41:42.428839 cmder-4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:41:42.428839 cmder-4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:41:42.428839 cmder-4.0/src/cmder/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 04:41:36.000000 cmder-4.0/src/cmder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-30 04:41:36.000000 cmder-4.0/src/cmder/cmder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:41:42.428839 cmder-4.0/src/cmder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-30 04:41:42.000000 cmder-4.0/src/cmder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-30 04:41:42.000000 cmder-4.0/src/cmder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 04:41:42.000000 cmder-4.0/src/cmder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 04:41:42.000000 cmder-4.0/src/cmder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:00:09.492863 cmder-5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-18 06:00:03.000000 cmder-5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-18 06:00:09.492863 cmder-5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-18 06:00:03.000000 cmder-5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-18 06:00:03.000000 cmder-5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-18 06:00:09.492863 cmder-5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:00:09.492863 cmder-5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:00:09.492863 cmder-5.0/src/cmder/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 06:00:03.000000 cmder-5.0/src/cmder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11403 2024-05-18 06:00:03.000000 cmder-5.0/src/cmder/cmder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:00:09.492863 cmder-5.0/src/cmder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-18 06:00:09.000000 cmder-5.0/src/cmder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-18 06:00:09.000000 cmder-5.0/src/cmder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 06:00:09.000000 cmder-5.0/src/cmder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-18 06:00:09.000000 cmder-5.0/src/cmder.egg-info/top_level.txt
```

### Comparing `cmder-4.0/LICENSE` & `cmder-5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmder-4.0/PKG-INFO` & `cmder-5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmder
-Version: 4.0
+Version: 5.0
 Summary: A shortcut for running shell command.
 Home-page: https://github.com/iBiology/cmder.git
 Author: FEI YUAN
 Author-email: yuanfeifuzzy@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cmder-4.0/README.md` & `cmder-5.0/README.md`

 * *Files identical despite different names*

### Comparing `cmder-4.0/setup.cfg` & `cmder-5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cmder
-version = 4.0
+version = 5.0
 author = FEI YUAN
 author_email = yuanfeifuzzy@gmail.com
 description = A shortcut for running shell command.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/iBiology/cmder.git
 project_urls =
```

### Comparing `cmder-4.0/src/cmder/cmder.py` & `cmder-5.0/src/cmder/cmder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,67 +1,71 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """
 A shortcut for running shell command.
 """
-import argparse
+
 import subprocess
 import os
 import sys
 import shlex
 import tempfile
 from pathlib import Path
 
-CMD_LINE_LENGTH = 100
+CMD_LINE_LENGTH = 80
 PMT = False
 
 try:
     from loguru import logger
+    
     logger.remove()
     logger.add(sys.stderr, format="<level>{message}</level>", filter=lambda record: record["level"].name == "DEBUG")
     logger.add(sys.stderr, format="<light-green>[{time:HH:mm:ss}]</light-green> <level>{message}</level>", level="INFO")
 except ImportError:
     import logging
+    
     logging.basicConfig(format='[%(asctime)s] %(message)s', datefmt='%H:%M:%S', level=logging.DEBUG)
     logger = logging.getLogger()
 
 
-def run(cmd, **kwargs):
-    """ Run cmd or raise exception if run fails. """
-    def format_cmd(command):
-        if isinstance(command, str):
-            command = shlex.shlex(command, posix=True, punctuation_chars=True)
-            command.whitespace_split = True
-            command = list(command)
-        elif isinstance(command, (list, tuple)):
-            command = [str(c) for c in command]
+def format_cmd(command, max_length=0):
+    if isinstance(command, str):
+        command = shlex.shlex(command, posix=True, punctuation_chars=True)
+        command.whitespace_split = True
+        command = list(command)
+    elif isinstance(command, (list, tuple)):
+        command = [str(c) for c in command]
+    else:
+        raise TypeError('Command only accepts a string or a list (or tuple) of strings.')
+    exe = command[0]
+    if len(' '.join(command)) <= (max_length or CMD_LINE_LENGTH):
+        return exe, ' '.join(command)
+    command = ' '.join([f'\\\n  {c}' if c.startswith('-') or '<' in c or '>' in c else c for c in command])
+    command = command.splitlines()
+    commands = []
+    for i, c in enumerate(command):
+        if i == 0:
+            commands.append(c)
         else:
-            raise TypeError('Command only accepts a string or a list (or tuple) of strings.')
-        exe = command[0]
-        if len(' '.join(command)) <= CMD_LINE_LENGTH:
-            return exe, ' '.join(command)
-        command = ' '.join([f'\\\n  {c}' if c.startswith('-') or '<' in c or '>' in c else c for c in command])
-        command = command.splitlines()
-        commands = []
-        for i, c in enumerate(command):
-            if i == 0:
+            if len(c) <= 80:
                 commands.append(c)
             else:
-                if len(c) <= 80:
-                    commands.append(c)
-                else:
-                    items = c.strip().replace(' \\', '').split()
-                    commands.append(f'  {items[0]} {items[1]} \\')
-                    for item in items[2:]:
-                        commands.append(' ' * (len(items[0]) + 3) + item + ' \\')
-        command = '\n'.join(commands)
-        if command.endswith(' \\'):
-            command = command[:-2]
-        return exe, command
+                items = c.strip().replace(' \\', '').split()
+                commands.append(f'  {items[0]} {items[1]} \\')
+                for item in items[2:]:
+                    commands.append(' ' * (len(items[0]) + 3) + item + ' \\')
+    command = '\n'.join(commands)
+    if command.endswith(' \\'):
+        command = command[:-2]
+    return exe, command
+
+
+def run(cmd, **kwargs):
+    """ Run cmd or raise exception if run fails. """
     
     def parse_profile():
         try:
             with open(profile_output) as f:
                 t, m = f.read().strip().split()
                 t = t.split(".")[0]
                 try:
@@ -98,17 +102,18 @@
     cwd = kwargs.pop('cwd', None)
     profile_output = tempfile.mktemp(suffix='.txt', prefix='.profile.', dir=cwd)
     try:
         if msg and (pmt or PMT):
             cmd = f'/usr/bin/time -f "%E %M" -o {profile_output} {cmd}'
         kwargs['stdout'] = kwargs.pop('stdout', sys.stdout if debug else subprocess.PIPE)
         kwargs['stderr'] = kwargs.pop('stderr', sys.stderr if debug else subprocess.PIPE)
+        timeout = kwargs.pop('timeout', None)
         process = subprocess.Popen(cmd, universal_newlines=True, shell=True, cwd=cwd, **kwargs)
-        process.wait()
-        if process.returncode: 
+        process.wait(timeout)
+        if process.returncode:
             stdout, stderr = process.communicate()
             logger.error(f'Failed to run {program} (exit code {process.returncode}):\n{stderr or stdout}')
             if exit_on_error:
                 sys.exit(process.returncode)
         if not process.returncode and msg:
             msg = msg.replace(' ...', f' complete.')
             if pmt or PMT:
@@ -141,36 +146,42 @@
 
 
 def submit(command, **kwargs):
     try:
         script = Path(kwargs.get('script', 'submit.sh')).resolve()
         logger.info(f'Generating submission script {script}')
         nodes = kwargs.get('nodes', 1)
-        ntasks_per_node = kwargs.get('ntasks_per_node', 1)
-        ntasks = kwargs.get('ntasks', 1)
+        ntasks_per_node = kwargs.get('ntasks_per_node', 0)
+        ntasks = kwargs.get('ntasks', 0)
         queue = kwargs.get('queue', '')
-        day = kwargs.get('day', 1)
         hour = kwargs.get('hour', 1)
-
+        
         with script.open('w') as o:
             o.write('#!/usr/bin/env bash\n')
             o.write('\n')
             o.write(f'#SBATCH --nodes={nodes}\n')
             o.write(f'#SBATCH --ntasks={ntasks}\n')
-            o.write(f'#SBATCH --ntasks-per-node={ntasks_per_node}\n')
-            o.write(f'#SBATCH --time={day}-{hour}:59\n')
-            o.write(f'#SBATCH --partition={queue}\n')
+            o.write(f'#SBATCH --time={hour}:00:00\n')
+            
+            if ntasks_per_node:
+                o.write(f'#SBATCH --ntasks-per-node={ntasks_per_node}\n')
+            if queue:
+                o.write(f'#SBATCH --partition={queue}\n')
             
-            cpus_per_node = kwargs.get('cpus_per_node', '')
+            cpus_per_node = kwargs.get('cpus_per_task', '')
             if cpus_per_node:
-                o.write(f'#SBATCH --cpus-per-node={cpus_per_node}\n')
+                o.write(f'#SBATCH --cpus-per-task={cpus_per_node}\n')
             
-            gpus_per_node = kwargs.get('gpus_per_node', '')
+            gpus_per_node = kwargs.get('gpus_per_task', '')
             if gpus_per_node:
-                o.write(f'#SBATCH --gpus-per-node={gpus_per_node}\n')
+                o.write(f'#SBATCH --gpus-per-task={gpus_per_node}\n')
+            
+            gres = kwargs.get('gres', '')
+            if gres:
+                o.write(f'#SBATCH --gres={gres}\n')
             
             array = kwargs.get('array', '')
             if array:
                 o.write(f'#SBATCH --array={array}\n')
             
             name = kwargs.get('name', '')
             if name:
@@ -201,18 +212,21 @@
             directives = kwargs.get('directives', [])
             if directives:
                 for directive in directives:
                     o.write(f'{directive}\n')
             
             environments = kwargs.get('environments', [])
             if environments:
+                o.write('\n')
                 for environment in environments:
                     o.write(f'{environment}\n')
             
-            o.write(f'{cmd}\n\n')
+            if kwargs.get('fmt_cmds', False):
+                command = '\n\n'.join([format_cmd(c)[1] for c in command.split('\n\n\n')])
+            o.write(f'\n{command}\n')
         
         logger.info(f'Successfully generated submit script {script}')
         
         if kwargs.get('hold', False):
             logger.info(f'Script {script.name} has not been submitted due to hold is True\n')
             return 0, 0
         else:
@@ -234,9 +248,70 @@
                     logger.error(f'Failed to get job id from submit result due to {e}:\n\n{s}')
                     return 0, 0
     except Exception as e:
         logger.error(f'Failed to generate submit script and submit the job due to\n{e}\n\n')
         return 1, 0
 
 
+def error_and_exit(message):
+    logger.error(message)
+    sys.exit(1)
+
+
+class File:
+    def __init__(self, path):
+        try:
+            if not Path(path).is_file():
+                error_and_exit(f'File {path} is not a file or does not exist')
+        except Exception as e:
+            error_and_exit(f'Check file {path} failed due to {e}')
+        self.path = Path(path).resolve()
+    
+    def __call__(self, *args, **kwargs):
+        return self.path
+    
+    def __getattr__(self, item):
+        return getattr(self.path, item)
+
+
+class Files:
+    def __init__(self, paths):
+        self.paths = [File(path) for path in paths]
+    
+    def __call__(self, *args, **kwargs):
+        return self.paths
+
+
+class Dir:
+    def __init__(self, path):
+        try:
+            if not Path(path).is_dir():
+                error_and_exit(f'Directory {path} is not a directory or does not exist')
+        except Exception as e:
+            error_and_exit(f'Check directory {path} failed due to {e}')
+        self.path = Path(path).resolve()
+    
+    def __call__(self, *args, **kwargs):
+        return self.path
+    
+    def __getattr__(self, item):
+        return getattr(self.path, item)
+
+
+class Exe:
+    def __init__(self, exe, exe_name='program'):
+        if exe:
+            p = run(f'which {exe}', log_cmd=False)
+            if p.returncode:
+                error_and_exit(f'Executable {exe} does not exist')
+            else:
+                exe = p.stdout.read().strip()
+        else:
+            error_and_exit(f'Path to {exe_name} executable is None, cannot continue')
+        self.exe = exe
+    
+    def __call__(self, *args, **kwargs):
+        return self.exe
+
+
 if __name__ == '__main__':
     pass
```

### Comparing `cmder-4.0/src/cmder.egg-info/PKG-INFO` & `cmder-5.0/src/cmder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmder
-Version: 4.0
+Version: 5.0
 Summary: A shortcut for running shell command.
 Home-page: https://github.com/iBiology/cmder.git
 Author: FEI YUAN
 Author-email: yuanfeifuzzy@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

