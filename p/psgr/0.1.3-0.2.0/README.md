# Comparing `tmp/psgr-0.1.3.tar.gz` & `tmp/psgr-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psgr-0.1.3.tar", last modified: Fri May 17 15:53:49 2024, max compression
+gzip compressed data, was "psgr-0.2.0.tar", last modified: Sat May 18 10:09:51 2024, max compression
```

## Comparing `psgr-0.1.3.tar` & `psgr-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-17 15:53:49.103437 psgr-0.1.3/
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      161 2024-05-17 15:53:49.103437 psgr-0.1.3/PKG-INFO
-drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-17 15:53:49.099437 psgr-0.1.3/psgr/
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       19 2024-04-28 12:52:49.000000 psgr-0.1.3/psgr/__init__.py
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)     8511 2024-05-17 15:49:16.000000 psgr-0.1.3/psgr/main.py
-drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-17 15:53:49.103437 psgr-0.1.3/psgr.egg-info/
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      161 2024-05-17 15:53:49.000000 psgr-0.1.3/psgr.egg-info/PKG-INFO
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      208 2024-05-17 15:53:49.000000 psgr-0.1.3/psgr.egg-info/SOURCES.txt
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        1 2024-05-17 15:53:49.000000 psgr-0.1.3/psgr.egg-info/dependency_links.txt
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       65 2024-05-17 15:53:49.000000 psgr-0.1.3/psgr.egg-info/entry_points.txt
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       24 2024-05-17 15:53:49.000000 psgr-0.1.3/psgr.egg-info/requires.txt
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        5 2024-05-17 15:53:49.000000 psgr-0.1.3/psgr.egg-info/top_level.txt
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       38 2024-05-17 15:53:49.103437 psgr-0.1.3/setup.cfg
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      485 2024-05-17 15:52:50.000000 psgr-0.1.3/setup.py
+drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-18 10:09:51.690371 psgr-0.2.0/
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      161 2024-05-18 10:09:51.690371 psgr-0.2.0/PKG-INFO
+drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-18 10:09:51.690371 psgr-0.2.0/psgr/
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       19 2024-05-18 09:54:37.000000 psgr-0.2.0/psgr/__init__.py
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)    11045 2024-05-18 10:09:48.000000 psgr-0.2.0/psgr/main.py
+drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-18 10:09:51.690371 psgr-0.2.0/psgr.egg-info/
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      161 2024-05-18 10:09:51.000000 psgr-0.2.0/psgr.egg-info/PKG-INFO
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      208 2024-05-18 10:09:51.000000 psgr-0.2.0/psgr.egg-info/SOURCES.txt
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        1 2024-05-18 10:09:51.000000 psgr-0.2.0/psgr.egg-info/dependency_links.txt
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       65 2024-05-18 10:09:51.000000 psgr-0.2.0/psgr.egg-info/entry_points.txt
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       24 2024-05-18 10:09:51.000000 psgr-0.2.0/psgr.egg-info/requires.txt
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        5 2024-05-18 10:09:51.000000 psgr-0.2.0/psgr.egg-info/top_level.txt
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       38 2024-05-18 10:09:51.690371 psgr-0.2.0/setup.cfg
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      485 2024-05-18 09:51:59.000000 psgr-0.2.0/setup.py
```

### Comparing `psgr-0.1.3/psgr/main.py` & `psgr-0.2.0/psgr/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import json
+import random
 import sys
 import time
 import base64
 import os.path
 import getpass
 from tabulate import tabulate
 import json
 import rsa
 from InquirerPy import inquirer
 import signal
 
 
-
 def main():
 
     def generateKeys():
         (pubkey, privkey) = rsa.newkeys(512)
         keyData = {
             "public_key": pubkey.save_pkcs1().decode(),
             "private_key": privkey.save_pkcs1().decode()
@@ -83,40 +83,45 @@
         elif command == "remove":
             remove(additional)
         elif command == "refresh":
             refreshkeys()
         elif command == "keys":
             (pub, priv) = fetchKeys()
             print(pub, priv)
+        elif command == "genkeys":
+            generateKeys()
+        elif command == "genpass":
+            passwordGen()
 
         return
 
     def add(accountName="", password=""):
         (pubkey, privkey) = fetchKeys()
         if not accountName:
             accountName = input("Enter The Account Name: ")
 
         if accounts.get(accountName) is not None:
             message = input("Password for this account is already entered. Overrite? This cannot be undone. [Y]/[N]? ")
             if message.upper() == "N":
                 return
             
         if not password:        
-            password = getpass.getpass(f"Enter Password for {accountName}: ").encode("utf-8")
+            password = getpass.getpass(f"Enter Password for {accountName}: ", stream=sys.stderr).encode("utf-8")
         else:
             password = password.encode("utf-8")
 
         encyrptedPW = encrypt(password, pubkey)
         accounts[accountName] = base64.b64encode(encyrptedPW).decode("utf-8")
         try:
             with open("accountinfo.json", "w") as f:
                 json.dump(accounts, f)
         except Exception as e:
             print("An error occurred while writing to the file:", e)
         # print(accounts)
+        print("Password saved successfully.")
         return
 
     def show(name=""):
         (pubkey, privkey) = fetchKeys()
         showAccounts = {}
         for k,v in accounts.items():
             try:
@@ -157,54 +162,69 @@
                 return
             else:
                 table_data = [(accountName, showAccounts[accountName])]
                 table = tabulate(table_data, headers=["Account", "Password"], tablefmt="github")
                 print(table)
                 print(" ")
 
+            tableLines = table.count("\n") + 2
+
         def ignore_ctrl_c(signum, frame):
-            print("Ctrl+C is disabled.", end="\r")
+            print("                             ", end="\r")
+            for i in range(tableLines):
+                print("\033[F", end="")  # Move cursor up one line
+                print("\033[K", end="")
+            sys.exit(0)
+        
         original_handler = signal.getsignal(signal.SIGINT)
         signal.signal(signal.SIGINT, ignore_ctrl_c)
-        for i in range(5, 0, -1):
+        for i in range(7, 0, -1):
             print(f"clearing screen in {i} seconds.", end="\r")
             time.sleep(1)
+        print("                             ", end="\r")
         signal.signal(signal.SIGINT, original_handler)
-        if os.name == 'nt':
-            _ = os.system('cls')
-        # For UNIX-like systems (Linux, macOS)
-        else:
-            _ = os.system('clear')
-        return
+        
+        for i in range(tableLines):
+            print("\033[F", end="")  # Move cursor up one line
+            print("\033[K", end="")
+        
+        sys.exit(0)
 
     def help():
         help_message = """
     Passman - Password Manager
 
     Usage:
         passman command
 
     Commands:
         add          Add a new account
         show         Show account information
         refresh      Refresh account information
+        genpass      Create and generate a strong password of the length of your choice
+        keys         View your current RSA encryption keys protecting your passwords
+        genkeys      Generate new keys. This will also be done automatically everytime you run "passman show".
         help         Show this help message
 
     Examples:
+        passman add                        
         passman add Google                # Add a new account named "Google"
         passman add Facebook password     # Add a new account named "Facebook" with password "password"
+        passman show                        # Promted to a list to choose your account from
         passman show all                       # Show all accounts
-        passman show Google               # Show account information for "Google"
-        passman refresh                     # Refresh account information
+        passman show Google               # Show account password for "Google"
+        passman refresh                     # Refresh keys
 
-    For more information, visit: https://github.com/nareshkarthigeyan/passwordManager
+    For more information and source code, visit: https://github.com/nareshkarthigeyan/passwordManager
 
     Note:
-        - Passwords are encrypted at all times.
-        - Passwords will disappear from the screen after 5 seconds.
+        - Passwords are encrypted using RSA encryption.
+        - Passwords will disappear from the screen after 7 seconds.
+
+    Made with Love by K V Naresh Karthigeyan
     """
         print(help_message)
         return
 
     def remove(alll=""):
         message = inquirer.select(
                     message = "Choose Account:",
@@ -225,19 +245,56 @@
                 ).execute()
 
             if alll in accounts:
                 accounts.pop(alll)
                 with open("accountinfo.json", "w") as f:
                     json.dump(accounts, f)            
         return
+    
+    def genpass(length):
+        digits = [x for x in "0123456789"]
+        lowercase = [x for x in "abcdefghijklmnopqrstuvwxyz"]
+        uppercase = [x for x in "abcdefghijklmnopqrstuvwxyz".upper()]
+        special = [x for x in "!@#$%^&*()_+~|}{:'?><" +'"']
+        combinedList = digits + lowercase + uppercase + special
+
+        password = "" + random.choice(uppercase) + random.choice(lowercase) + random.choice(special)
+        for i in range (length - 3):
+            password += random.choice(combinedList)
+
+        return password
+    
+    def passwordGen():
+        length = inquirer.select(
+                    message = "Choose Length of Password to be generated:",
+                    choices = [12, 16, 24]
+                ).execute()
+        password = genpass(length=length)
+        print("\t", password)
+        savePassword = inquirer.select(
+                    message = "Do you want to save this password for an account?",
+                    choices = ["yes", "no"]
+                ).execute()
+        if savePassword == "yes":
+            chooseIt = ["Create a New Account"]
+            for k, v in accounts.items():
+                chooseIt.append(k)
+            accountName = inquirer.select(
+                message = "Choose the account:",
+                choices = chooseIt
+            ).execute()
 
+            if accountName == "Create a New Account":
+                add(password=password)
+            else:
+                add(accountName=accountName, password=password)
 
     n = len(sys.argv)
 
-    arguments = ("help", "add", "show", "remove", "keys", "refresh")
+    arguments = ("help", "-h", "add", "-a", "show", '-s', "remove", "-rm", "keys", "refresh", "-r" "genkeys", "genpass", "-p")
 
     if os.path.isfile("accountinfo.json"):
         with open("accountinfo.json", "r") as f:
             accounts = json.load(f)
     else:
         accounts = {}
 
@@ -252,8 +309,8 @@
         assign_task(sys.argv[1])
     elif n == 3:
         assign_task(sys.argv[1], sys.argv[2])
     elif n == 4:
         assign_task(sys.argv[1], sys.argv[2], sys.argv[3]) 
 
 
-main()
+#main()
```

