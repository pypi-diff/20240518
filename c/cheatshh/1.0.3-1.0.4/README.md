# Comparing `tmp/cheatshh-1.0.3.tar.gz` & `tmp/cheatshh-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheatshh-1.0.3.tar", last modified: Sat May 11 12:19:37 2024, max compression
+gzip compressed data, was "cheatshh-1.0.4.tar", last modified: Sat May 18 11:30:33 2024, max compression
```

## Comparing `cheatshh-1.0.3.tar` & `cheatshh-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-11 12:19:37.889249 cheatshh-1.0.3/
--rw-r--r--   0 root         (0) staff       (20)    11357 2024-05-09 07:38:12.000000 cheatshh-1.0.3/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     1340 2024-05-11 12:19:37.889013 cheatshh-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     4724 2024-05-11 12:12:30.000000 cheatshh-1.0.3/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-11 12:19:37.888333 cheatshh-1.0.3/cheatshh.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     1340 2024-05-11 12:19:37.000000 cheatshh-1.0.3/cheatshh.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      256 2024-05-11 12:19:37.000000 cheatshh-1.0.3/cheatshh.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-05-11 12:19:37.000000 cheatshh-1.0.3/cheatshh.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       51 2024-05-11 12:19:37.000000 cheatshh-1.0.3/cheatshh.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)       21 2024-05-11 12:19:37.000000 cheatshh-1.0.3/cheatshh.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        4 2024-05-11 12:19:37.000000 cheatshh-1.0.3/cheatshh.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2024-05-11 12:19:37.889294 cheatshh-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     3115 2024-05-11 12:18:45.000000 cheatshh-1.0.3/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-11 12:19:37.888558 cheatshh-1.0.3/src/
--rw-r--r--   0 root         (0) staff       (20)        0 2024-05-09 09:59:20.000000 cheatshh-1.0.3/src/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      222 2024-05-10 19:10:43.000000 cheatshh-1.0.3/src/run_cheatshh.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-18 11:30:33.981696 cheatshh-1.0.4/
+-rw-r--r--   0 root         (0) staff       (20)    11357 2024-05-09 07:38:12.000000 cheatshh-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     1411 2024-05-18 11:30:33.981427 cheatshh-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     4844 2024-05-18 11:22:35.000000 cheatshh-1.0.4/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-18 11:30:33.980885 cheatshh-1.0.4/cheatshh.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     1411 2024-05-18 11:30:33.000000 cheatshh-1.0.4/cheatshh.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      256 2024-05-18 11:30:33.000000 cheatshh-1.0.4/cheatshh.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-05-18 11:30:33.000000 cheatshh-1.0.4/cheatshh.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       51 2024-05-18 11:30:33.000000 cheatshh-1.0.4/cheatshh.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)       21 2024-05-18 11:30:33.000000 cheatshh-1.0.4/cheatshh.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        4 2024-05-18 11:30:33.000000 cheatshh-1.0.4/cheatshh.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-05-18 11:30:33.981742 cheatshh-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     3250 2024-05-18 11:27:52.000000 cheatshh-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-18 11:30:33.981102 cheatshh-1.0.4/src/
+-rw-r--r--   0 root         (0) staff       (20)        0 2024-05-09 09:59:20.000000 cheatshh-1.0.4/src/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      222 2024-05-18 10:34:26.000000 cheatshh-1.0.4/src/run_cheatshh.py
```

### Comparing `cheatshh-1.0.3/LICENSE` & `cheatshh-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cheatshh-1.0.3/PKG-INFO` & `cheatshh-1.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheatshh
-Version: 1.0.3
+Version: 1.0.4
 Author: Anirudh Gupta
 Keywords: cheatsheet, cheat, command-line, cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fuzzyfinder
 Requires-Dist: whiptail
 
@@ -21,17 +21,17 @@
 - TLDR and MAN pages visible in the preview.
 - Easy to add, edit, delete commands and groups and playing around.
 - Press Enter on a command to copy it to clipboard and exit.
 
 Visit the Github Repository for more details: https://github.com/AnirudhG07/cheatshh
 
 # Version
-1.0.3
+1.0.4
 
 ## Note:
 - This package is best used in Unix based systems, like linux and MacOS. For Windows, see the github repository for more details.
 - The package is installed in ~/.config/cheatshh directory.
 
-## Bugs fixed in 1.0.3
+## Bugs fixed in 1.0.4
 - Path configuration for Linux has been fixed.
-- docs has been updated.
+- group names will be displayed whenever asked to enter a group name in option functionalities.
```

### Comparing `cheatshh-1.0.3/README.md` & `cheatshh-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-# cheatshh ![Static Badge](https://img.shields.io/badge/version-1.0.3-blue)
+# cheatshh ![Static Badge](https://img.shields.io/badge/version-1.0.4-blue)
 
 Cheatshh is an interactive CLI meant for managing command line cheatshheets, written in shell script. Now you don't have to remember CLI commands and just refer your cheatshhet. You can group commands and view their TLDR and MAN pages along with a custom description for the command.
 
+# Preview/Screenshots 
+
+https://github.com/AnirudhG07/cheatshh/assets/146579014/831405bb-aba4-461f-9ca9-e0f75d74155d
+
+
 # Features
 
 - Comprehensive cheatsheets for various command-line utilities and tools.
 - Easy-to-use interface for quickly accessing and executing commands, powered by fuzzy finder(fzf) and whiptail.
 - Customizable cheatshheets and groups to suit your needs.
 - TLDR and MAN pages visible in the preview.
 - Easy to add, edit, delete commands and groups and playing around.
@@ -99,11 +104,11 @@
 source ~/.bashrc  # For Bash
 source ~/.zshrc   # For Zsh
 ```
 This should add the path in your shell-rc file and you should be able to run.<br>
 Note: If you are using some other shell like fish or any other, configure the settings accordingly. Using Fish is not recommended for this tool.
 
 # Documentation
-Cheatshh is an interactive, easy CLI tool to maintain your custom cheatshheets. You can check our the <a href="https://github.com/AnirudhG07/cheatshh/tree/1.0.3/docs"> docs </a> to see how to use cheatshh.
+Cheatshh is an interactive, easy CLI tool to maintain your custom cheatshheets. You can check our the <a href="https://github.com/AnirudhG07/cheatshh/tree/1.0.4/docs"> docs </a> to see how to use cheatshh.
 
 # Contributing
 I would love to take contributions from the community! If you have suggestions for new cheatsheets, improvements to existing ones, or bug fixes, please feel free to submit a pull request.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-# cheatshh ![Static Badge](https://img.shields.io/badge/version-1.0.3-blue)
+# cheatshh ![Static Badge](https://img.shields.io/badge/version-1.0.4-blue)
 Cheatshh is an interactive CLI meant for managing command line cheatshheets,
 written in shell script. Now you don't have to remember CLI commands and just
 refer your cheatshhet. You can group commands and view their TLDR and MAN pages
-along with a custom description for the command. # Features - Comprehensive
-cheatsheets for various command-line utilities and tools. - Easy-to-use
-interface for quickly accessing and executing commands, powered by fuzzy finder
-(fzf) and whiptail. - Customizable cheatshheets and groups to suit your needs.
-- TLDR and MAN pages visible in the preview. - Easy to add, edit, delete
-commands and groups and playing around. # Installation The following
-installation guidelines hold for Linux and MacOS.
+along with a custom description for the command. # Preview/ScreenshotsÂ  https:
+//github.com/AnirudhG07/cheatshh/assets/146579014/831405bb-aba4-461f-9ca9-
+e0f75d74155d # Features - Comprehensive cheatsheets for various command-line
+utilities and tools. - Easy-to-use interface for quickly accessing and
+executing commands, powered by fuzzy finder(fzf) and whiptail. - Customizable
+cheatshheets and groups to suit your needs. - TLDR and MAN pages visible in the
+preview. - Easy to add, edit, delete commands and groups and playing around. #
+Installation The following installation guidelines hold for Linux and MacOS.
 You can download cheatshh through following ways- (more will be added soon) ##
 Pip Installation Before running the below commands, make sure your dependencies
 are satisfied. See the DEPENDENCIES section for more info. From your command
 line, run- ```bash pip install cheatshh ``` This will create ~/.config/cheatshh
 in your home directory. Now simply run- ```bash cheatshh ``` and you are done.
 Use various options to add, edit and delete commands and groups. ## Manual
 Installation through git clone You can setup manual installation with the
```

### Comparing `cheatshh-1.0.3/cheatshh.egg-info/PKG-INFO` & `cheatshh-1.0.4/cheatshh.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheatshh
-Version: 1.0.3
+Version: 1.0.4
 Author: Anirudh Gupta
 Keywords: cheatsheet, cheat, command-line, cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fuzzyfinder
 Requires-Dist: whiptail
 
@@ -21,17 +21,17 @@
 - TLDR and MAN pages visible in the preview.
 - Easy to add, edit, delete commands and groups and playing around.
 - Press Enter on a command to copy it to clipboard and exit.
 
 Visit the Github Repository for more details: https://github.com/AnirudhG07/cheatshh
 
 # Version
-1.0.3
+1.0.4
 
 ## Note:
 - This package is best used in Unix based systems, like linux and MacOS. For Windows, see the github repository for more details.
 - The package is installed in ~/.config/cheatshh directory.
 
-## Bugs fixed in 1.0.3
+## Bugs fixed in 1.0.4
 - Path configuration for Linux has been fixed.
-- docs has been updated.
+- group names will be displayed whenever asked to enter a group name in option functionalities.
```

### Comparing `cheatshh-1.0.3/setup.py` & `cheatshh-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,21 +40,20 @@
         ("requirements.txt", "requirements.txt")
     ]
     # Copy files to ~/.config/cheatshh
     for file_name, src_file in files_to_copy:
         src_path = os.path.join(setup_dir, src_file)
         dest_path = os.path.join(config_dir, file_name)
         shutil.copy(src_path, dest_path)
-
+    print("Cheatshh installed successfully!")
 
 def run_cheatshh():
-    subprocess.run(["bash", "~/.config/cheatshh/cheats.sh"])
-
+    subprocess.run(["bash", os.path.expanduser("~/.config/cheatshh/cheats.sh")])
 
-setup(name="cheatshh", version="1.0.3", cmdclass={"install": CustomInstallCommand},
+setup(name="cheatshh", version="1.0.4", cmdclass={"install": CustomInstallCommand},
       long_description="""
 # cheatshh
 
 Cheatshh is an interactive CLI meant for managing command line cheatshheets. Now you don't have to remember CLI commands and just refer your cheatshhet. You can group commands and view their TLDR and MAN pages along with a custom description for the command.
 
 # Features
 
@@ -64,23 +63,23 @@
 - TLDR and MAN pages visible in the preview.
 - Easy to add, edit, delete commands and groups and playing around.
 - Press Enter on a command to copy it to clipboard and exit.
 
 Visit the Github Repository for more details: https://github.com/AnirudhG07/cheatshh
 
 # Version
-1.0.3
+1.0.4
 
 ## Note:
 - This package is best used in Unix based systems, like linux and MacOS. For Windows, see the github repository for more details.
 - The package is installed in ~/.config/cheatshh directory.
 
-## Bugs fixed in 1.0.3
+## Bugs fixed in 1.0.4
 - Path configuration for Linux has been fixed.
-- docs has been updated.
+- group names will be displayed whenever asked to enter a group name in option functionalities.
 
 """,
     long_description_content_type="text/markdown",
     keywords=["cheatsheet, cheat, command-line, cli"],
     install_requires=["fuzzyfinder", "whiptail"],
     author="Anirudh Gupta",
     packages=find_packages(),
```

