# Comparing `tmp/lavague_drivers_selenium-0.1.1.post1.tar.gz` & `tmp/lavague_drivers_selenium-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_drivers_selenium-0.1.1.post1.tar", max compression
+gzip compressed data, was "lavague_drivers_selenium-0.1.2.tar", max compression
```

## Comparing `lavague_drivers_selenium-0.1.1.post1.tar` & `lavague_drivers_selenium-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       34 2024-05-15 22:13:36.166566 lavague_drivers_selenium-0.1.1.post1/README.md
--rw-r--r--   0        0        0       57 2024-05-15 22:13:36.166566 lavague_drivers_selenium-0.1.1.post1/lavague/drivers/selenium/__init__.py
--rw-r--r--   0        0        0    11746 2024-05-15 22:13:36.166566 lavague_drivers_selenium-0.1.1.post1/lavague/drivers/selenium/base.py
--rw-r--r--   0        0        0      982 2024-05-15 22:13:36.170566 lavague_drivers_selenium-0.1.1.post1/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 lavague_drivers_selenium-0.1.1.post1/PKG-INFO
+-rw-r--r--   0        0        0       34 2024-05-18 13:00:01.403135 lavague_drivers_selenium-0.1.2/README.md
+-rw-r--r--   0        0        0       57 2024-05-18 13:00:01.403135 lavague_drivers_selenium-0.1.2/lavague/drivers/selenium/__init__.py
+-rw-r--r--   0        0        0    11834 2024-05-18 13:00:20.363119 lavague_drivers_selenium-0.1.2/lavague/drivers/selenium/base.py
+-rw-r--r--   0        0        0      976 2024-05-18 13:05:44.627475 lavague_drivers_selenium-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 lavague_drivers_selenium-0.1.2/PKG-INFO
```

### Comparing `lavague_drivers_selenium-0.1.1.post1/lavague/drivers/selenium/base.py` & `lavague_drivers_selenium-0.1.2/lavague/drivers/selenium/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,27 +13,34 @@
 class SeleniumDriver(BaseDriver):
     driver: WebDriver
 
     def __init__(
         self,
         url: Optional[str] = None,
         get_selenium_driver: Optional[Callable[[], WebDriver]] = None,
+        headless: bool = True,
+        chrome_user_dir: Optional[str] = None,
     ):
+        self.headless = headless
+        self.chrome_user_dir = chrome_user_dir
         super().__init__(url, get_selenium_driver)
 
     def default_init_code(self) -> Any:
         # these imports are necessary as they will be pasted to the output
         from selenium import webdriver
         from selenium.webdriver.common.by import By
         from selenium.webdriver.chrome.options import Options
         from selenium.webdriver.common.keys import Keys
         from selenium.webdriver.common.action_chains import ActionChains
 
         chrome_options = Options()
-        chrome_options.add_argument("--headless")
+        if self.headless:
+            chrome_options.add_argument("--headless")
+        if self.chrome_user_dir:
+            chrome_options.add_argument(f"--user-data-dir={self.chrome_user_dir}")
         chrome_options.add_argument("--no-sandbox")
 
         self.driver = webdriver.Chrome(options=chrome_options)
         self.resize_driver(1024, 1024)
         return self.driver
 
     def get_driver(self) -> WebDriver:
@@ -158,44 +165,43 @@
                 "viewport_size": viewport_size,
             }
             outputs.append(output)
         return outputs
 
     def get_capability(self) -> str:
         return '''
+
 Your goal is to write Selenium code to answer queries.
 
 Your answer must be a Python markdown only.
 You can have access to external websites and libraries.
-
-Don't assume attribute values are unique, use the combination of most available attributes to target precisely the element.
-Even if there is mutliple elements doing the same action, choose the most relevant and target it precisely.
-Always use //*[contains(@attributes_names ,'value')] to target elements by XPATH.
+Always target elements by XPATH.
 
 You can assume the following code has been executed:
 ```python
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 
 driver = webdriver.Firefox()
 ```
 
 ---
 
 HTML:
 <!DOCTYPE html>
-<html>
-<head>
-    <title>Mock Search Page</title>
+<html xpath="/html">
+<head xpath="/html/head">
+    <title xpath="/html/head/title">Mock Search Page</title>
+    <meta charset="utf-8" xpath="/html/head/meta[1]"/>
 </head>
-<body>
-    <h1>Search Page Example</h1>
-    <input id="searchBar" type="text" placeholder="Type here to search...">
-    <button id="searchButton">Search</button>
-    <script>
+<body xpath="/html/body">
+    <h1 xpath="/html/body/h1">Search Page Example</h1>
+    <input id="searchBar" type="text" placeholder="Type here to search..." xpath="/html/body/input[1]"/>
+    <button id="searchButton" xpath="/html/body/button">Search</button>
+    <script xpath="/html/body/script">
         document.getElementById('searchButton').onclick = function() {{
             var searchText = document.getElementById('searchBar').value;
             alert("Searching for: " + searchText);
         }};
     </script>
 </body>
 </html>
@@ -203,64 +209,61 @@
 Query: Click on the search bar 'Type here to search...', type 'selenium', and press the 'Enter' key
 
 Completion:
 ```python
 # Let's proceed step by step.
 # First we need to identify the component first, then we can click on it.
 
-# Based on the HTML, the link can be uniquely identified using the ID "searchBar"
-# Let's use this ID with Selenium to identify the link
-search_bar = driver.find_element(By.XPATH, """//*[contains(@id,"searchBar")][contains(@placeholder,"Type here to search...")]""")
+# We use the XPATH to identify the element
+search_bar = driver.find_element(By.XPATH, "/html/body/input[1]")
 
 search_bar.click()
 
 # Now we can type the asked input
 search_bar.send_keys("selenium")
 
 # Finally we can press the 'Enter' key
 search_bar.send_keys(Keys.ENTER)
 ```
 
 ---
 
 HTML:
 <!DOCTYPE html>
-<html lang="en">
-<head>
-    <meta charset="UTF-8">
-    <title>Mock Page for Selenium</title>
+<html lang="en" xpath="/html">
+<head xpath="/html/head">
+    <meta charset="UTF-8" xpath="/html/head/meta[1]">
+    <title xpath="/html/head/title">Mock Page for Selenium</title>
 </head>
-<body>
-    <h1>Welcome to the Mock Page</h1>
-    <div id="links">
-        <a href="#link1" id="link1">Link 1</a>
-        <br>
-        <a href="#link2" class="link perf">Link 2</a>
-        <br>
+<body xpath="/html/body">
+    <h1 xpath="/html/body/h1">Welcome to the Mock Page</h1>
+    <div id="links" xpath="/html/body/div">
+        <a href="#link1" id="link1" xpath="/html/body/div/a[1]">Link 1</a>
+        <br xpath="/html/body/div/br[1]">
+        <a href="#link2" class="link perf" xpath="/html/body/div/a[2]">Link 2</a>
+        <br xpath="/html/body/div/br[2]">
     </div>
 </body>
 </html>
 
 Query: Click on the title Link 1 and then click on the title Link 2
 
 Completion:
 ```python
 # Let's proceed step by step.
 # First we need to identify the first component, then we can click on it. Then we can identify the second component and click on it.
 
-# Based on the HTML, the first link the link can be uniquely identified using the ID "link1"
-# Let's use this ID with Selenium to identify the link
-link_to_click = driver.find_element(By.XPATH, """//*[contains(@id,"link1")][contains(@href,"#link1")]""")
+# We use the XPATH to identify the element
+link_to_click = driver.find_element(By.XPATH, "/html/body/div/a[1]")
 
 # Then we click on the link
 link_to_click.click()
 
-# The other link can be uniquely identified using the class "link" but as it's not unique, we can use the class "perf" to make it more precise
-# Let's use this class to identify the link
-link_to_click = driver.find_element(By.XPATH, """//*[contains(@class, "link")][contains(@class, "perf")][contains(@href,"#link2")]""")
+# We use the XPATH to identify the element
+link_to_click = driver.find_element(By.XPATH, "/html/body/div/a[2]")
 
 # Click on the element found
 link_to_click.click()
 ```
 
 ---
 
@@ -325,44 +328,43 @@
 
 ---
 
 ---
 
 HTML:
 <!DOCTYPE html>
-<html lang="en">
-<head>
-    <meta charset="UTF-8">
-    <title>Enhanced Mock Page for Selenium Testing</title>
+<html lang="en" xpath="/html">
+<head xpath="/html/head">
+    <meta charset="UTF-8" xpath="/html/head/meta[1]">
+    <title xpath="/html/head/title">Enhanced Mock Page for Selenium Testing</title>
 </head>
-<body>
-    <h1>Enhanced Test Page for Selenium</h1>
-    <div class="container">
-        <button id="firstButton" onclick="alert('First button clicked!');">First Button</button>
+<body xpath="/html/body">
+    <h1 xpath="/html/body/h1">Enhanced Test Page for Selenium</h1>
+    <div class="container" xpath="/html/body/div[1]">
+        <button id="firstButton" onclick="alert('First button clicked!');" xpath="/html/body/div[1]/button[1]">First Button</button>
         <!-- This is the button we're targeting with the class name "action-btn" -->
-        <button class="action-btn" onclick="alert('Action button clicked!');">Action Button</button>
-        <div class="nested-container">
-            <button id="testButton" onclick="alert('Test Button clicked!');">Test Button</button>
+        <button class="action-btn" onclick="alert('Action button clicked!');" xpath="/html/body/div[1]/button[2]">Action Button</button>
+        <div class="nested-container" xpath="/html/body/div[1]/div">
+            <button id="testButton" onclick="alert('Test Button clicked!');" xpath="/html/body/div[1]/div/button">Test Button</button>
         </div>
-        <button class="hidden" onclick="alert('Hidden button clicked!');">Hidden Button</button>
+        <button class="hidden" onclick="alert('Hidden button clicked!');" xpath="/html/body/div[1]/button[3]">Hidden Button</button>
     </div>
 </body>
 </html>
 
 
 Query: Click on the Button 'First Button'
 
 Completion:
 ```python
 # Let's proceed step by step.
 # First we need to identify the button first, then we can click on it.
 
-# Based on the HTML provided, we need to devise the best strategy to select the button.
-# The action button can be identified using the class name "action-btn" as it is unique we don't use contains
-action_button = driver.find_element(By.XPATH, """//*[contains(@class,"action-btn")][contains(@onclick,"alert('Action button clicked!");')][contains(.,"Action Button")]""")
+# We use the XPATH to identify the element
+action_button = driver.find_element(By.XPATH, "/html/body/div[1]/button[2]")
 
 # Then we can click on it
 action_button.click()
 ```
 
 ---
 '''
```

### Comparing `lavague_drivers_selenium-0.1.1.post1/pyproject.toml` & `lavague_drivers_selenium-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lavague-drivers-selenium"
-version = "0.1.1-post1"
+version = "0.1.2"
 description = "Selenium integration for lavague"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `lavague_drivers_selenium-0.1.1.post1/PKG-INFO` & `lavague_drivers_selenium-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-drivers-selenium
-Version: 0.1.1.post1
+Version: 0.1.2
 Summary: Selenium integration for lavague
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,selenium
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

