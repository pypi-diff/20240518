# Comparing `tmp/ai_project_setup-0.2.6.tar.gz` & `tmp/ai_project_setup-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_project_setup-0.2.6.tar", last modified: Fri May 17 02:10:50 2024, max compression
+gzip compressed data, was "ai_project_setup-0.2.7.tar", last modified: Sat May 18 06:15:56 2024, max compression
```

## Comparing `ai_project_setup-0.2.6.tar` & `ai_project_setup-0.2.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:10:50.494490 ai_project_setup-0.2.6/
--rw-r--r--   0 root         (0) root         (0)     1544 2024-05-17 02:10:50.494490 ai_project_setup-0.2.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3159 2024-05-17 01:19:44.000000 ai_project_setup-0.2.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:10:50.493490 ai_project_setup-0.2.6/ai_project_setup.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1544 2024-05-17 02:10:50.000000 ai_project_setup-0.2.6/ai_project_setup.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      280 2024-05-17 02:10:50.000000 ai_project_setup-0.2.6/ai_project_setup.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 02:10:50.000000 ai_project_setup-0.2.6/ai_project_setup.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-05-17 02:10:50.000000 ai_project_setup-0.2.6/ai_project_setup.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:10:50.493490 ai_project_setup-0.2.6/git_clone/
--rw-r--r--   0 root         (0) root         (0)       33 2024-05-17 00:52:56.000000 ai_project_setup-0.2.6/git_clone/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10003 2024-05-17 02:09:15.000000 ai_project_setup-0.2.6/git_clone/git_clone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:10:50.494490 ai_project_setup-0.2.6/project_setup/
--rw-r--r--   0 root         (0) root         (0)       41 2024-05-17 00:50:04.000000 ai_project_setup-0.2.6/project_setup/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5173 2024-05-17 00:50:04.000000 ai_project_setup-0.2.6/project_setup/project_setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 02:10:50.494490 ai_project_setup-0.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1880 2024-05-17 02:10:47.000000 ai_project_setup-0.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 06:15:56.639082 ai_project_setup-0.2.7/
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-05-18 06:15:56.638081 ai_project_setup-0.2.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3159 2024-05-18 06:01:49.000000 ai_project_setup-0.2.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 06:15:56.637081 ai_project_setup-0.2.7/ai_project_setup.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-05-18 06:15:56.000000 ai_project_setup-0.2.7/ai_project_setup.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      280 2024-05-18 06:15:56.000000 ai_project_setup-0.2.7/ai_project_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-18 06:15:56.000000 ai_project_setup-0.2.7/ai_project_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-18 06:15:56.000000 ai_project_setup-0.2.7/ai_project_setup.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 06:15:56.638081 ai_project_setup-0.2.7/git_clone/
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-18 06:01:49.000000 ai_project_setup-0.2.7/git_clone/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12237 2024-05-18 06:05:51.000000 ai_project_setup-0.2.7/git_clone/git_clone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 06:15:56.638081 ai_project_setup-0.2.7/project_setup/
+-rw-r--r--   0 root         (0) root         (0)       41 2024-05-18 06:01:49.000000 ai_project_setup-0.2.7/project_setup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5173 2024-05-18 06:01:49.000000 ai_project_setup-0.2.7/project_setup/project_setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-18 06:15:56.639082 ai_project_setup-0.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-05-18 06:15:38.000000 ai_project_setup-0.2.7/setup.py
```

### Comparing `ai_project_setup-0.2.6/PKG-INFO` & `ai_project_setup-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai_project_setup
-Version: 0.2.6
+Version: 0.2.7
 Summary: A versatile utility package designed to streamline the setup of AI project structures while seamlessly integrating with Git repositories and Google Colab, simplifying the process of building collaborative AI projects.
 Author: Patrick Ogbuitepu
 Author-email: pat2echo@gmail.com
 Keywords: AI,utility package,project structure,Git integration,Google Colab integration,collaborative projects,ease of use,streamlined workflow,automation,project management,project,setup,structure,ai,artificial intelligence,research,data science,machine learning
 Description-Content-Type: text/markdown
 
 # AI Project Starter Pack
```

### Comparing `ai_project_setup-0.2.6/README.md` & `ai_project_setup-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `ai_project_setup-0.2.6/ai_project_setup.egg-info/PKG-INFO` & `ai_project_setup-0.2.7/ai_project_setup.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-project-setup
-Version: 0.2.6
+Version: 0.2.7
 Summary: A versatile utility package designed to streamline the setup of AI project structures while seamlessly integrating with Git repositories and Google Colab, simplifying the process of building collaborative AI projects.
 Author: Patrick Ogbuitepu
 Author-email: pat2echo@gmail.com
 Keywords: AI,utility package,project structure,Git integration,Google Colab integration,collaborative projects,ease of use,streamlined workflow,automation,project management,project,setup,structure,ai,artificial intelligence,research,data science,machine learning
 Description-Content-Type: text/markdown
 
 # AI Project Starter Pack
```

### Comparing `ai_project_setup-0.2.6/git_clone/git_clone.py` & `ai_project_setup-0.2.7/git_clone/git_clone.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,22 +18,23 @@
     def __init__(self, mount_google_drive=True, vc_repo='', vc_user='', vc_token=''):
         self.vc_repo = vc_repo
         self.vc_user = vc_user
         self.vc_token = vc_token
         self.content_dir = 'content'
         self.base_dir = f'/{self.content_dir}/'
         self.no_error = True
+        self.git_dir = ''
 
         self.url, self.dirname, self.user_email, self.user_name = self.get_repo_data(vc_repo, vc_user, vc_token)
         
         if self.no_error and mount_google_drive:
           self.base_dir = self.mount_gdrive(self.base_dir)
 
         if self.no_error:
-          self.clone_repo(self.url, self.dirname, self.base_dir)
+          self.git_dir = self.clone_repo(self.url, self.dirname, self.base_dir)
           
         if self.no_error:
           self.branch_name = self.get_git_branch_name()
 
     def mount_gdrive(self, base_dir):
       """Mount google drive, git repo will be cloned into google drive
 
@@ -103,25 +104,24 @@
           print(error, "You can also define this value as a secret")
           user_email = input("Tell us your git email address: ")
           if self.is_valid_email(user_email):
             error = ''
           else:
             error += f"\nEmail address provided is invalid: {user_email}"
 
-      # if error == '': 
-      #   try:
-      #       user_email = userdata.get('username')
-      #   except Exception as e:
-      #       error = f"An error occurred: {e}"
-      #       print(error, "You can also define this value as a secret")
-      #       user_name = input("Tell us your git username: ")
-      #       if user_name != '':
-      #         error = ''
-      #       else:
-      #         error += f"\nUsername provided is invalid: {user_name}"
+      if error == '': 
+        try:
+            user_name = userdata.get('username')
+        except Exception as e:
+            print(f"An error occurred: {e}", "You can also define this value as a secret")
+
+        if user_name == '':
+          print("Using email as username")
+          user_name = user_email
+
 
       if error == '':
         if vc_repo == '':
           try:
             vc_repo = userdata.get('url')
           except Exception as e:
             error = f"An error occurred: {e}"
@@ -164,59 +164,81 @@
 
       Parameters:
         url (str): Git URL with Auth. Credentials
         dir (str): Directory Name after cloning the repository
         base_dir (str): Base/Root Directory Path. E.g In google colab its usually /content/
 
       Returns:
-        none: Returns Nothing
+        str: Directory Path of the Repo
       """
       error = ''
+      git_dir = ''
       user_dir = base_dir
       if url.startswith("http") and url.endswith(".git"):
         if os.path.exists(user_dir):
             os.chdir(user_dir)
             git_dir = os.path.join(user_dir,dir)
             if os.path.exists(git_dir):
               print(f"\033[91mIMPORTANT! Directory {git_dir} already exists\033[0m")
               confirm = input(f"The directory {git_dir} already exists.\nAre you sure you want to delete the directory '{git_dir}' and all its contents and re-clone it? (yes/no): ")
               if confirm.lower() == 'yes':
                   shutil.rmtree(git_dir)
               else:
-                  error = f"User aborted the Clone Operation because the directory exists"
-              
+                  error = "User aborted the Clone Operation because the directory exists"
+            
+            attempt_pull = True  
             if error == '':
               #!git clone {url}
-              subprocess.run(["git", "clone", url])
+              self.subprocess_run(["git", "clone", url])
+              attempt_pull = False
             
             if os.path.exists(git_dir):
               os.chdir(dir)
               print('List files: ', os.listdir())
+
+              if attempt_pull:
+                print(error)
+                branch_name = self.get_git_branch_name()
+                if branch_name == '':
+                  error = "Unable to read branch name of git repo"
+                else:
+                  print(f"\033[94mIMPORTANT! About to Pull Updates from the repo\033[0m")
+                  confirm = input(f"Recent updates on *{branch_name} branch of the repo will be pulled and overwrite your local changes.\nDo you wish to proceed (yes/no): ")
+                  
+                  if confirm.lower() == 'yes':
+                    self.subprocess_run(["git", "pull", "origin", branch_name])
+                  else:
+                    error = "User pull process"
             else:
               error = f"Failed to Clone Repo: Directory {git_dir} does not exists"
               self.no_error = False
         else:
             error = f"Directory {user_dir} does not exists"
             self.no_error = False
       else:
         error = f"Invalid repo url, url must start with [http://...] or [https://...] and end with [.git]"
         self.no_error = False
 
       if error: print(error)
+
+      return git_dir
     
     def get_git_branch_name(self):
       """Run the git branch command and capture the output
       
       Returns:
         str: Name of current git branch
       """
       error = ''
-      branch_name = subprocess.check_output(['git', 'rev-parse', '--abbrev-ref', 'HEAD']).decode().strip()
-      ansi_escape = re.compile(r'\x1B\[[0-?]*[ -/]*[@-~]')
-      branch_name = ansi_escape.sub('', branch_name)
+      try:
+        branch_name = subprocess.check_output(['git', 'rev-parse', '--abbrev-ref', 'HEAD']).decode().strip()
+        ansi_escape = re.compile(r'\x1B\[[0-?]*[ -/]*[@-~]')
+        branch_name = ansi_escape.sub('', branch_name)
+      except subprocess.CalledProcessError as e:
+          error = str(e)
 
       # branch_name = ''
       # try:
       #     branch_output = !git branch
       #     # Find the line with an asterisk (*) indicating the current branch
       #     for line in branch_output:
       #         if line.startswith('*'):
@@ -230,38 +252,95 @@
       #     error = f"Error: Unable to get Git branch: {e}"
 
       if error: 
         print(error)
         self.no_error = False
 
       return branch_name
-
-    def commit_and_push(self, commit_message=''):
+    
+    def commit_and_push(self):
       """Save (commit) and push changes to git repository
 
+      Returns:
+        none: Returns Nothing
+      """
+      commit_msg = input("Enter your commit message that describes the changes that you have made to the files: ")
+      if commit_msg == '':
+        commit_msg = f'Commit at {datetime.now()}'
+
+      self.commit(commit_msg)
+      self.push()
+    
+    def set_dir(self):
+      """Check status of git repo
+
+      Returns:
+        none: Returns Nothing
+      """
+      os.chdir(self.git_dir)
+      self.subprocess_run(["git", "status"])
+
+    def status(self):
+      """Check status of git repo
+
+      Returns:
+        none: Returns Nothing
+      """
+      self.subprocess_run(["git", "status"])
+
+    def commit(self, commit_message=''):
+      """Commit or Save changes to local git repository
+
       Parameters:
-        commit_message (str): Describe the changes that you have made
+        commit_message (str): Commit message that describe the changes that you have made to the code
 
       Returns:
         none: Returns Nothing
       """
       #!git config --global user.email {self.user_email}
-      subprocess.run(["git", "config", "--global", "user.email", self.user_email])
+      self.subprocess_run(["git", "config", "user.email", self.user_email])
 
       #!git config --global user.name {self.user_email}
-      subprocess.run(["git", "config", "--global", "user.name", self.user_name])
+      self.subprocess_run(["git", "config", "user.name", self.user_name])
 
       #!git config --global user.name {self.user_name}
       #!git add . 
-      subprocess.run(["git", "add", "."])
+      self.subprocess_run(["git", "add", "."])
 
-      commit_msg = input("Enter your commit message that describes the changes that you have made to the files: ")
-      if commit_msg == '':
-        commit_msg = f'Commit at {datetime.now()}'
       #!git commit -m "{commit_msg}"
-      subprocess.run(["git", "commit", "-m", commit_msg])
+      self.subprocess_run(["git", "commit", "-m", commit_message])
+
+    def push(self):
+      """Save changes to remote git repository
+
+      Returns:
+        none: Returns Nothing
+      """
       #!git remote set-url origin {self.url}
-      subprocess.run(["git", "remote", "set-url", "origin", self.url])
+      self.subprocess_run(["git", "remote", "set-url", "origin", self.url])
       #!git push origin {self.branch_name}
-      subprocess.run(["git", "push", "origin", self.branch_name])
+      self.subprocess_run(["git", "push", "origin", self.branch_name])
+
+    def subprocess_run(self, args):
+      """Run commands in terminal and display the output
+
+      Parameters:
+        args (list): Command to run
+
+      Returns:
+        str: Return Error Message
+      """
+      error = ''
+      try:
+        result = subprocess.run(args, capture_output=True)
+        if result.returncode == 0:
+            # Print the output
+            print("Output:", result.stdout.decode())
+        else:
+            error = result.stderr.decode()
+            print("Error:", error)
+      except subprocess.CalledProcessError as e:
+        error = str(e)
+        print(error)
 
+      return error
```

### Comparing `ai_project_setup-0.2.6/project_setup/project_setup.py` & `ai_project_setup-0.2.7/project_setup/project_setup.py`

 * *Files identical despite different names*

### Comparing `ai_project_setup-0.2.6/setup.py` & `ai_project_setup-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ai_project_setup',
-    version='0.2.6',
+    version='0.2.7',
     packages=find_packages(),
     description='A versatile utility package designed to streamline the setup of AI project structures while seamlessly integrating with Git repositories and Google Colab, simplifying the process of building collaborative AI projects.',
     long_description="""# AI Project Starter Pack
 The AI Project Starter Pack is a meticulously structured directory and module framework designed for creating machine learning and data science projects. This starter pack aims to streamline the project setup process, helping data scientists and developers organize their code, data, and documentation efficiently. 
 
 ## GITHUB: https://github.com/pat2echo/AI-Project-Starter-Pack/
```

