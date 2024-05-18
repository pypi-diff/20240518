# Comparing `tmp/st_login_form-0.2.3.tar.gz` & `tmp/st-login-form-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_login_form-0.2.3.tar", last modified: Sat May 18 09:37:16 2024, max compression
+gzip compressed data, was "st-login-form-0.3.0.tar", last modified: Fri Jul 21 15:56:51 2023, max compression
```

## Comparing `st_login_form-0.2.3.tar` & `st-login-form-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:37:16.299693 st_login_form-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-18 09:37:05.000000 st_login_form-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-18 09:37:05.000000 st_login_form-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-18 09:37:16.299693 st_login_form-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-18 09:37:05.000000 st_login_form-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 09:37:16.299693 st_login_form-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-18 09:37:05.000000 st_login_form-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:37:16.299693 st_login_form-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:37:16.299693 st_login_form-0.2.3/src/st_login_form/
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-18 09:37:05.000000 st_login_form-0.2.3/src/st_login_form/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:37:16.299693 st_login_form-0.2.3/src/st_login_form.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-18 09:37:16.000000 st_login_form-0.2.3/src/st_login_form.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-18 09:37:16.000000 st_login_form-0.2.3/src/st_login_form.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 09:37:16.000000 st_login_form-0.2.3/src/st_login_form.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 09:37:16.000000 st_login_form-0.2.3/src/st_login_form.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-18 09:37:16.000000 st_login_form-0.2.3/src/st_login_form.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:56:51.754086 st-login-form-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-21 15:56:42.000000 st-login-form-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 15:56:42.000000 st-login-form-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-21 15:56:51.754086 st-login-form-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-21 15:56:42.000000 st-login-form-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:56:51.754086 st-login-form-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-21 15:56:42.000000 st-login-form-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:56:51.750085 st-login-form-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:56:51.750085 st-login-form-0.3.0/src/st_login_form/
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-21 15:56:42.000000 st-login-form-0.3.0/src/st_login_form/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:56:51.754086 st-login-form-0.3.0/src/st_login_form.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-21 15:56:51.000000 st-login-form-0.3.0/src/st_login_form.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-21 15:56:51.000000 st-login-form-0.3.0/src/st_login_form.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:56:51.000000 st-login-form-0.3.0/src/st_login_form.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-21 15:56:51.000000 st-login-form-0.3.0/src/st_login_form.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-21 15:56:51.000000 st-login-form-0.3.0/src/st_login_form.egg-info/top_level.txt
```

### Comparing `st_login_form-0.2.3/PKG-INFO` & `st-login-form-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,43 @@
 Metadata-Version: 2.1
 Name: st-login-form
-Version: 0.2.3
+Version: 0.3.0
 Summary: A streamlit component that creates a user login form connected to a Supabase DB. It lets users create a new username and password, login to an existing account, or login as an anonymous guest.
 Home-page: https://github.com/SiddhantSadangi/st_login_form
 Author: Siddhant Sadangi
 Author-email: siddhant.sadangi@gmail.com
 Project-URL: Documentation, https://github.com/SiddhantSadangi/st_login_form/blob/main/README.md
-Project-URL: Funding, https://www.buymeacoffee.com/siddhantsadangi
+Project-URL: Support, https://www.buymeacoffee.com/siddhantsadangi
 Keywords: streamlit,login
 Classifier: Environment :: Plugins
-Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: streamlit>=1.2
-Requires-Dist: jinja2
-Requires-Dist: supabase>=2.4.5
 
 # :lock: st-login-form
 [![Downloads](https://static.pepy.tech/personalized-badge/st-login-form?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/st-login-form)
 
 A streamlit component that creates a user login form connected to a Supabase DB. It lets users create a new username and password, login to an existing account, or login as an anonymous guest.
 
 ![Form screenshot](assets/screenshot.png)
 
 The login form collapses after login to free screen-space.
 
-> [!WARNING]  
-> Passwords are saved as plain text. Use with caution.
-
 ## :computer: Demo app
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://st-lgn-form.streamlit.app/)
 
-## :construction: Installation
+## :construction: Installation 
 
-1. Install `st-login-form`
+1. Install `st-login-form` 
 ```sh
 pip install st-login-form
 ```
 2. Create a Supabase project as mentioned [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/supabase#sign-in-to-supabase-and-create-a-project)
 3. Create a table to store the usernames and passwords. The table name and column names can be as per your choice.
 ```sql
 CREATE TABLE users (
@@ -77,21 +70,22 @@
   ) tablespace pg_default;
 ```
 4. Follow the rest of the steps from [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/supabase#copy-your-app-secrets-to-the-cloud) to connect your Streamlit app to Supabase
 
 
 ## :pen: Usage
 
-On authentication, `login_form()` sets the `st.session_state['authenticated']` to `True`. This also collapses and disables the login form.  
-`st.session_state['username']` is set to the provided username for a new or existing user, and to `None` for guest login.
+`login_form()` sets `session_state["authenticated"]` to `True` if the login is successful, `session_state["username"]` to the `username` or new or existing user, and to `None` for guest login.
+
+Returns the initialized `supabase.Client` instance to let you interact with the databse downstream in the script.
 
 ```python
 import streamlit as st
 
-from st_login_form import login_form
+from streamlit_login import login_form
 
 client = login_form()
 
 if st.session_state["authenticated"]:
     if st.session_state["username"]:
         st.success(f"Welcome {st.session_state['username']}")
     else:
```

#### html2text {}

```diff
@@ -1,49 +1,47 @@
-Metadata-Version: 2.1 Name: st-login-form Version: 0.2.3 Summary: A streamlit
+Metadata-Version: 2.1 Name: st-login-form Version: 0.3.0 Summary: A streamlit
 component that creates a user login form connected to a Supabase DB. It lets
 users create a new username and password, login to an existing account, or
 login as an anonymous guest. Home-page: https://github.com/SiddhantSadangi/
 st_login_form Author: Siddhant Sadangi Author-email: siddhant.sadangi@gmail.com
 Project-URL: Documentation, https://github.com/SiddhantSadangi/st_login_form/
-blob/main/README.md Project-URL: Funding, https://www.buymeacoffee.com/
+blob/main/README.md Project-URL: Support, https://www.buymeacoffee.com/
 siddhantsadangi Keywords: streamlit,login Classifier: Environment :: Plugins
-Classifier: Environment :: Web Environment Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: User Interfaces Requires-Python:
->=3.8 Description-Content-Type: text/markdown License-File: LICENSE Requires-
-Dist: streamlit>=1.2 Requires-Dist: jinja2 Requires-Dist: supabase>=2.4.5 # :
-lock: st-login-form [![Downloads](https://static.pepy.tech/personalized-badge/
-st-login-
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: GNU General Public License v3 (GPLv3) Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Topic ::
+Software Development :: User Interfaces Requires-Python: >=3.8 Description-
+Content-Type: text/markdown License-File: LICENSE # :lock: st-login-form [!
+[Downloads](https://static.pepy.tech/personalized-badge/st-login-
 form?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=Downloads)]
 (https://pepy.tech/project/st-login-form) A streamlit component that creates a
 user login form connected to a Supabase DB. It lets users create a new username
 and password, login to an existing account, or login as an anonymous guest. !
 [Form screenshot](assets/screenshot.png) The login form collapses after login
-to free screen-space. > [!WARNING] > Passwords are saved as plain text. Use
-with caution. ## :computer: Demo app [![Open in Streamlit](https://
+to free screen-space. ## :computer: Demo app [![Open in Streamlit](https://
 static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://st-lgn-
 form.streamlit.app/) ## :construction: Installation 1. Install `st-login-form`
 ```sh pip install st-login-form ``` 2. Create a Supabase project as mentioned
 [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/
 supabase#sign-in-to-supabase-and-create-a-project) 3. Create a table to store
 the usernames and passwords. The table name and column names can be as per your
 choice. ```sql CREATE TABLE users ( username text not null default ''::text,
 password text not null, constraint users_pkey primary key (username),
 constraint users_username_key unique (username), constraint
 users_password_check check ( ( length( trim( both from password ) ) > 1 ) ),
 constraint users_username_check check ( ( length( trim( both from username ) )
 > 1 ) ) ) tablespace pg_default; ``` 4. Follow the rest of the steps from
 [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/
 supabase#copy-your-app-secrets-to-the-cloud) to connect your Streamlit app to
-Supabase ## :pen: Usage On authentication, `login_form()` sets the
-`st.session_state['authenticated']` to `True`. This also collapses and disables
-the login form. `st.session_state['username']` is set to the provided username
-for a new or existing user, and to `None` for guest login. ```python import
-streamlit as st from st_login_form import login_form client = login_form() if
-st.session_state["authenticated"]: if st.session_state["username"]: st.success
-(f"Welcome {st.session_state['username']}") else: st.success("Welcome guest")
-else: st.error("Not authenticated") ``` [![See demo in Streamlit](https://
-static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://st-lgn-
-form.streamlit.app/) ## ð¤ Want to support my work?
+Supabase ## :pen: Usage `login_form()` sets `session_state["authenticated"]` to
+`True` if the login is successful, `session_state["username"]` to the
+`username` or new or existing user, and to `None` for guest login. Returns the
+initialized `supabase.Client` instance to let you interact with the databse
+downstream in the script. ```python import streamlit as st from streamlit_login
+import login_form client = login_form() if st.session_state["authenticated"]:
+if st.session_state["username"]: st.success(f"Welcome {st.session_state
+['username']}") else: st.success("Welcome guest") else: st.error("Not
+authenticated") ``` [![See demo in Streamlit](https://static.streamlit.io/
+badges/streamlit_badge_black_white.svg)](https://st-lgn-form.streamlit.app/) ##
+ð¤ Want to support my work?
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
```

### Comparing `st_login_form-0.2.3/README.md` & `st-login-form-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,20 @@
 
 A streamlit component that creates a user login form connected to a Supabase DB. It lets users create a new username and password, login to an existing account, or login as an anonymous guest.
 
 ![Form screenshot](assets/screenshot.png)
 
 The login form collapses after login to free screen-space.
 
-> [!WARNING]  
-> Passwords are saved as plain text. Use with caution.
-
 ## :computer: Demo app
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://st-lgn-form.streamlit.app/)
 
-## :construction: Installation
+## :construction: Installation 
 
-1. Install `st-login-form`
+1. Install `st-login-form` 
 ```sh
 pip install st-login-form
 ```
 2. Create a Supabase project as mentioned [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/supabase#sign-in-to-supabase-and-create-a-project)
 3. Create a table to store the usernames and passwords. The table name and column names can be as per your choice.
 ```sql
 CREATE TABLE users (
@@ -52,21 +49,22 @@
   ) tablespace pg_default;
 ```
 4. Follow the rest of the steps from [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/supabase#copy-your-app-secrets-to-the-cloud) to connect your Streamlit app to Supabase
 
 
 ## :pen: Usage
 
-On authentication, `login_form()` sets the `st.session_state['authenticated']` to `True`. This also collapses and disables the login form.  
-`st.session_state['username']` is set to the provided username for a new or existing user, and to `None` for guest login.
+`login_form()` sets `session_state["authenticated"]` to `True` if the login is successful, `session_state["username"]` to the `username` or new or existing user, and to `None` for guest login.
+
+Returns the initialized `supabase.Client` instance to let you interact with the databse downstream in the script.
 
 ```python
 import streamlit as st
 
-from st_login_form import login_form
+from streamlit_login import login_form
 
 client = login_form()
 
 if st.session_state["authenticated"]:
     if st.session_state["username"]:
         st.success(f"Welcome {st.session_state['username']}")
     else:
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
 # :lock: st-login-form [![Downloads](https://static.pepy.tech/personalized-
 badge/st-login-
 form?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=Downloads)]
 (https://pepy.tech/project/st-login-form) A streamlit component that creates a
 user login form connected to a Supabase DB. It lets users create a new username
 and password, login to an existing account, or login as an anonymous guest. !
 [Form screenshot](assets/screenshot.png) The login form collapses after login
-to free screen-space. > [!WARNING] > Passwords are saved as plain text. Use
-with caution. ## :computer: Demo app [![Open in Streamlit](https://
+to free screen-space. ## :computer: Demo app [![Open in Streamlit](https://
 static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://st-lgn-
 form.streamlit.app/) ## :construction: Installation 1. Install `st-login-form`
 ```sh pip install st-login-form ``` 2. Create a Supabase project as mentioned
 [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/
 supabase#sign-in-to-supabase-and-create-a-project) 3. Create a table to store
 the usernames and passwords. The table name and column names can be as per your
 choice. ```sql CREATE TABLE users ( username text not null default ''::text,
 password text not null, constraint users_pkey primary key (username),
 constraint users_username_key unique (username), constraint
 users_password_check check ( ( length( trim( both from password ) ) > 1 ) ),
 constraint users_username_check check ( ( length( trim( both from username ) )
 > 1 ) ) ) tablespace pg_default; ``` 4. Follow the rest of the steps from
 [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/
 supabase#copy-your-app-secrets-to-the-cloud) to connect your Streamlit app to
-Supabase ## :pen: Usage On authentication, `login_form()` sets the
-`st.session_state['authenticated']` to `True`. This also collapses and disables
-the login form. `st.session_state['username']` is set to the provided username
-for a new or existing user, and to `None` for guest login. ```python import
-streamlit as st from st_login_form import login_form client = login_form() if
-st.session_state["authenticated"]: if st.session_state["username"]: st.success
-(f"Welcome {st.session_state['username']}") else: st.success("Welcome guest")
-else: st.error("Not authenticated") ``` [![See demo in Streamlit](https://
-static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://st-lgn-
-form.streamlit.app/) ## ð¤ Want to support my work?
+Supabase ## :pen: Usage `login_form()` sets `session_state["authenticated"]` to
+`True` if the login is successful, `session_state["username"]` to the
+`username` or new or existing user, and to `None` for guest login. Returns the
+initialized `supabase.Client` instance to let you interact with the databse
+downstream in the script. ```python import streamlit as st from streamlit_login
+import login_form client = login_form() if st.session_state["authenticated"]:
+if st.session_state["username"]: st.success(f"Welcome {st.session_state
+['username']}") else: st.success("Welcome guest") else: st.error("Not
+authenticated") ``` [![See demo in Streamlit](https://static.streamlit.io/
+badges/streamlit_badge_black_white.svg)](https://st-lgn-form.streamlit.app/) ##
+ð¤ Want to support my work?
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
```

### Comparing `st_login_form-0.2.3/setup.py` & `st-login-form-0.3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,36 @@
 from pathlib import Path
 
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-
-def get_version(rel_path):
-    with open(rel_path, "r", encoding="UTF-8") as f:
-        for line in f:
-            if line.startswith("__version__"):
-                delim = '"' if '"' in line else "'"
-                return line.split(delim)[1]
-    raise RuntimeError("Unable to find version string.")
-
-
 setuptools.setup(
     name="st-login-form",
-    version=get_version("src/st_login_form/__init__.py"),
+    version="0.3.0",
     url="https://github.com/SiddhantSadangi/st_login_form",
     author="Siddhant Sadangi",
     author_email="siddhant.sadangi@gmail.com",
     description="A streamlit component that creates a user login form connected to a Supabase DB. It lets users create a new username and password, login to an existing account, or login as an anonymous guest.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "Documentation": "https://github.com/SiddhantSadangi/st_login_form/blob/main/README.md",
-        "Funding": "https://www.buymeacoffee.com/siddhantsadangi",
+        "Support": "https://www.buymeacoffee.com/siddhantsadangi",
     },
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     classifiers=[
         "Environment :: Plugins",
-        "Environment :: Web Environment",
         "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: User Interfaces",
     ],
     keywords=["streamlit", "login"],
     python_requires=">=3.8",
-    install_requires=["streamlit>=1.2", "jinja2", "supabase>=2.4.5"],
+    install_requires=["streamlit>=1.2", "jinja2", "supabase"],
 )
```

### Comparing `st_login_form-0.2.3/src/st_login_form/__init__.py` & `st-login-form-0.3.0/src/st_login_form/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 import streamlit as st
-from supabase import Client, create_client
-
-__version__ = "0.2.3"
+from supabase import create_client, Client
 
 
 @st.cache_resource
 def init_connection() -> Client:
-    try:
-        return create_client(
-            st.secrets["connections"]["supabase"]["SUPABASE_URL"],
-            st.secrets["connections"]["supabase"]["SUPABASE_KEY"],
-        )
-    except KeyError:
-        return create_client(st.secrets["SUPABASE_URL"], st.secrets["SUPABASE_KEY"])
+    return create_client(st.secrets["SUPABASE_URL"], st.secrets["SUPABASE_KEY"])
 
 
 def login_success(message: str, username: str) -> None:
     st.success(message)
     st.session_state["authenticated"] = True
     st.session_state["username"] = username
 
@@ -32,15 +24,15 @@
     allow_guest: bool = True,
     guest_title: str = "Guest login :ninja: ",
     create_username_label: str = "Create a unique username",
     create_username_placeholder: str = None,
     create_username_help: str = None,
     create_password_label: str = "Create a password",
     create_password_placeholder: str = None,
-    create_password_help: str = "⚠️ Password will be stored as plain text. Do not reuse from other websites. Password cannot be recovered.",
+    create_password_help: str = "⚠️ Remember your password. You won't be able to recover it if forgotten.",
     create_submit_label: str = "Create account",
     create_success_message: str = "Account created :tada:",
     login_username_label: str = "Enter your unique username",
     login_username_placeholder: str = None,
     login_username_help: str = None,
     login_password_label: str = "Enter your password",
     login_password_placeholder: str = None,
@@ -107,20 +99,23 @@
 
                 if st.form_submit_button(
                     label=create_submit_label,
                     type="primary",
                     disabled=st.session_state["authenticated"],
                 ):
                     try:
-                        client.table(user_tablename).insert(
-                            {username_col: username, password_col: password}
-                        ).execute()
+                        data, _ = (
+                            client.table(user_tablename)
+                            .insert(
+                                {username_col: username, password_col: hash(password)}
+                            )
+                            .execute()
+                        )
                     except Exception as e:
                         st.error(e.message)
-                        st.session_state["authenticated"] = False
                     else:
                         login_success(create_success_message, username)
 
         # Login to existing account
         with login_tab:
             with st.form(key="login"):
                 username = st.text_input(
@@ -139,27 +134,26 @@
                 )
 
                 if st.form_submit_button(
                     label=login_submit_label,
                     disabled=st.session_state["authenticated"],
                     type="primary",
                 ):
-                    response = (
+                    data, _ = (
                         client.table(user_tablename)
                         .select(f"{username_col}, {password_col}")
                         .eq(username_col, username)
-                        .eq(password_col, password)
+                        .eq(password_col, hash(password))
                         .execute()
                     )
 
-                    if len(response.data) > 0:
+                    if len(data[-1]) > 0:
                         login_success(login_success_message, username)
                     else:
                         st.error(login_error_message)
-                        st.session_state["authenticated"] = False
 
         # Guest login
         if allow_guest:
             with guest_tab:
                 if st.button(
                     label=guest_submit_label,
                     type="primary",
@@ -169,14 +163,14 @@
 
         return client
 
 
 def main() -> None:
     login_form(
         create_username_placeholder="Username will be visible in the global leaderboard.",
-        create_password_placeholder="⚠️ Password will be stored as plain text. You won't be able to recover it if you forget.",
+        create_password_placeholder="⚠️ Remember your password. You won't be able to recover it if you forget.",
         guest_submit_label="Play as a guest ⚠️ Scores won't be saved",
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `st_login_form-0.2.3/src/st_login_form.egg-info/PKG-INFO` & `st-login-form-0.3.0/src/st_login_form.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,43 @@
 Metadata-Version: 2.1
 Name: st-login-form
-Version: 0.2.3
+Version: 0.3.0
 Summary: A streamlit component that creates a user login form connected to a Supabase DB. It lets users create a new username and password, login to an existing account, or login as an anonymous guest.
 Home-page: https://github.com/SiddhantSadangi/st_login_form
 Author: Siddhant Sadangi
 Author-email: siddhant.sadangi@gmail.com
 Project-URL: Documentation, https://github.com/SiddhantSadangi/st_login_form/blob/main/README.md
-Project-URL: Funding, https://www.buymeacoffee.com/siddhantsadangi
+Project-URL: Support, https://www.buymeacoffee.com/siddhantsadangi
 Keywords: streamlit,login
 Classifier: Environment :: Plugins
-Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: streamlit>=1.2
-Requires-Dist: jinja2
-Requires-Dist: supabase>=2.4.5
 
 # :lock: st-login-form
 [![Downloads](https://static.pepy.tech/personalized-badge/st-login-form?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/st-login-form)
 
 A streamlit component that creates a user login form connected to a Supabase DB. It lets users create a new username and password, login to an existing account, or login as an anonymous guest.
 
 ![Form screenshot](assets/screenshot.png)
 
 The login form collapses after login to free screen-space.
 
-> [!WARNING]  
-> Passwords are saved as plain text. Use with caution.
-
 ## :computer: Demo app
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://st-lgn-form.streamlit.app/)
 
-## :construction: Installation
+## :construction: Installation 
 
-1. Install `st-login-form`
+1. Install `st-login-form` 
 ```sh
 pip install st-login-form
 ```
 2. Create a Supabase project as mentioned [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/supabase#sign-in-to-supabase-and-create-a-project)
 3. Create a table to store the usernames and passwords. The table name and column names can be as per your choice.
 ```sql
 CREATE TABLE users (
@@ -77,21 +70,22 @@
   ) tablespace pg_default;
 ```
 4. Follow the rest of the steps from [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/supabase#copy-your-app-secrets-to-the-cloud) to connect your Streamlit app to Supabase
 
 
 ## :pen: Usage
 
-On authentication, `login_form()` sets the `st.session_state['authenticated']` to `True`. This also collapses and disables the login form.  
-`st.session_state['username']` is set to the provided username for a new or existing user, and to `None` for guest login.
+`login_form()` sets `session_state["authenticated"]` to `True` if the login is successful, `session_state["username"]` to the `username` or new or existing user, and to `None` for guest login.
+
+Returns the initialized `supabase.Client` instance to let you interact with the databse downstream in the script.
 
 ```python
 import streamlit as st
 
-from st_login_form import login_form
+from streamlit_login import login_form
 
 client = login_form()
 
 if st.session_state["authenticated"]:
     if st.session_state["username"]:
         st.success(f"Welcome {st.session_state['username']}")
     else:
```

#### html2text {}

```diff
@@ -1,49 +1,47 @@
-Metadata-Version: 2.1 Name: st-login-form Version: 0.2.3 Summary: A streamlit
+Metadata-Version: 2.1 Name: st-login-form Version: 0.3.0 Summary: A streamlit
 component that creates a user login form connected to a Supabase DB. It lets
 users create a new username and password, login to an existing account, or
 login as an anonymous guest. Home-page: https://github.com/SiddhantSadangi/
 st_login_form Author: Siddhant Sadangi Author-email: siddhant.sadangi@gmail.com
 Project-URL: Documentation, https://github.com/SiddhantSadangi/st_login_form/
-blob/main/README.md Project-URL: Funding, https://www.buymeacoffee.com/
+blob/main/README.md Project-URL: Support, https://www.buymeacoffee.com/
 siddhantsadangi Keywords: streamlit,login Classifier: Environment :: Plugins
-Classifier: Environment :: Web Environment Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: User Interfaces Requires-Python:
->=3.8 Description-Content-Type: text/markdown License-File: LICENSE Requires-
-Dist: streamlit>=1.2 Requires-Dist: jinja2 Requires-Dist: supabase>=2.4.5 # :
-lock: st-login-form [![Downloads](https://static.pepy.tech/personalized-badge/
-st-login-
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: GNU General Public License v3 (GPLv3) Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Topic ::
+Software Development :: User Interfaces Requires-Python: >=3.8 Description-
+Content-Type: text/markdown License-File: LICENSE # :lock: st-login-form [!
+[Downloads](https://static.pepy.tech/personalized-badge/st-login-
 form?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=Downloads)]
 (https://pepy.tech/project/st-login-form) A streamlit component that creates a
 user login form connected to a Supabase DB. It lets users create a new username
 and password, login to an existing account, or login as an anonymous guest. !
 [Form screenshot](assets/screenshot.png) The login form collapses after login
-to free screen-space. > [!WARNING] > Passwords are saved as plain text. Use
-with caution. ## :computer: Demo app [![Open in Streamlit](https://
+to free screen-space. ## :computer: Demo app [![Open in Streamlit](https://
 static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://st-lgn-
 form.streamlit.app/) ## :construction: Installation 1. Install `st-login-form`
 ```sh pip install st-login-form ``` 2. Create a Supabase project as mentioned
 [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/
 supabase#sign-in-to-supabase-and-create-a-project) 3. Create a table to store
 the usernames and passwords. The table name and column names can be as per your
 choice. ```sql CREATE TABLE users ( username text not null default ''::text,
 password text not null, constraint users_pkey primary key (username),
 constraint users_username_key unique (username), constraint
 users_password_check check ( ( length( trim( both from password ) ) > 1 ) ),
 constraint users_username_check check ( ( length( trim( both from username ) )
 > 1 ) ) ) tablespace pg_default; ``` 4. Follow the rest of the steps from
 [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/
 supabase#copy-your-app-secrets-to-the-cloud) to connect your Streamlit app to
-Supabase ## :pen: Usage On authentication, `login_form()` sets the
-`st.session_state['authenticated']` to `True`. This also collapses and disables
-the login form. `st.session_state['username']` is set to the provided username
-for a new or existing user, and to `None` for guest login. ```python import
-streamlit as st from st_login_form import login_form client = login_form() if
-st.session_state["authenticated"]: if st.session_state["username"]: st.success
-(f"Welcome {st.session_state['username']}") else: st.success("Welcome guest")
-else: st.error("Not authenticated") ``` [![See demo in Streamlit](https://
-static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://st-lgn-
-form.streamlit.app/) ## ð¤ Want to support my work?
+Supabase ## :pen: Usage `login_form()` sets `session_state["authenticated"]` to
+`True` if the login is successful, `session_state["username"]` to the
+`username` or new or existing user, and to `None` for guest login. Returns the
+initialized `supabase.Client` instance to let you interact with the databse
+downstream in the script. ```python import streamlit as st from streamlit_login
+import login_form client = login_form() if st.session_state["authenticated"]:
+if st.session_state["username"]: st.success(f"Welcome {st.session_state
+['username']}") else: st.success("Welcome guest") else: st.error("Not
+authenticated") ``` [![See demo in Streamlit](https://static.streamlit.io/
+badges/streamlit_badge_black_white.svg)](https://st-lgn-form.streamlit.app/) ##
+ð¤ Want to support my work?
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
```

