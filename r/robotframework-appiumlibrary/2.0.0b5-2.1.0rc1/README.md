# Comparing `tmp/robotframework-appiumlibrary-2.0.0b5.tar.gz` & `tmp/robotframework-appiumlibrary-2.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-appiumlibrary-2.0.0b5.tar", last modified: Sat Oct 29 10:29:42 2022, max compression
+gzip compressed data, was "robotframework-appiumlibrary-2.1.0rc1.tar", last modified: Sat May 18 01:53:09 2024, max compression
```

## Comparing `robotframework-appiumlibrary-2.0.0b5.tar` & `robotframework-appiumlibrary-2.1.0rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 serhat.bolsu   (502) staff       (20)        0 2022-10-29 10:29:42.101629 robotframework-appiumlibrary-2.0.0b5/
-drwxr-xr-x   0 serhat.bolsu   (502) staff       (20)        0 2022-10-29 10:29:42.096963 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)     5544 2022-10-25 11:28:33.000000 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/__init__.py
-drwxr-xr-x   0 serhat.bolsu   (502) staff       (20)        0 2022-10-29 10:29:42.099876 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)      843 2022-10-25 11:28:33.000000 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/__init__.py
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)     6985 2022-10-25 13:06:24.000000 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/_android_utils.py
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)    18892 2022-10-29 09:27:28.000000 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/_applicationmanagement.py
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)    30086 2022-10-29 10:22:29.000000 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/_element.py
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)     1302 2022-10-25 11:28:33.000000 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/_keyevent.py
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)     1923 2022-10-25 11:28:33.000000 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/_logging.py
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)     2919 2022-10-25 11:28:33.000000 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/_runonfailure.py
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)     6787 2022-10-25 11:28:33.000000 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/_screenrecord.py
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)     1887 2022-10-25 11:28:33.000000 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/_screenshot.py
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)     8257 2022-10-26 08:57:42.000000 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/_touch.py
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)     5460 2022-10-25 11:28:33.000000 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/_waiting.py
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)     1037 2022-10-25 11:28:33.000000 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/keywordgroup.py
-drwxr-xr-x   0 serhat.bolsu   (502) staff       (20)        0 2022-10-29 10:29:42.100269 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/locators/
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)      109 2022-10-25 11:28:33.000000 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/locators/__init__.py
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)    11198 2022-10-29 10:28:56.000000 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/locators/elementfinder.py
-drwxr-xr-x   0 serhat.bolsu   (502) staff       (20)        0 2022-10-29 10:29:42.100661 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/utils/
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)      391 2022-10-25 11:28:33.000000 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/utils/__init__.py
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)     1024 2022-10-25 11:28:33.000000 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/utils/applicationcache.py
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)       45 2022-10-29 10:29:35.000000 robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/version.py
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)    10273 2022-10-25 11:28:33.000000 robotframework-appiumlibrary-2.0.0b5/LICENSE
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)     6339 2022-10-29 10:29:42.101730 robotframework-appiumlibrary-2.0.0b5/PKG-INFO
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)     5249 2022-10-25 11:28:33.000000 robotframework-appiumlibrary-2.0.0b5/README.rst
-drwxr-xr-x   0 serhat.bolsu   (502) staff       (20)        0 2022-10-29 10:29:42.101480 robotframework-appiumlibrary-2.0.0b5/robotframework_appiumlibrary.egg-info/
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)     6339 2022-10-29 10:29:42.000000 robotframework-appiumlibrary-2.0.0b5/robotframework_appiumlibrary.egg-info/PKG-INFO
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)      950 2022-10-29 10:29:42.000000 robotframework-appiumlibrary-2.0.0b5/robotframework_appiumlibrary.egg-info/SOURCES.txt
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)        1 2022-10-29 10:29:42.000000 robotframework-appiumlibrary-2.0.0b5/robotframework_appiumlibrary.egg-info/dependency_links.txt
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)      126 2022-10-29 10:29:42.000000 robotframework-appiumlibrary-2.0.0b5/robotframework_appiumlibrary.egg-info/requires.txt
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)       14 2022-10-29 10:29:42.000000 robotframework-appiumlibrary-2.0.0b5/robotframework_appiumlibrary.egg-info/top_level.txt
--rw-r--r--   0 serhat.bolsu   (502) staff       (20)      134 2022-10-29 10:29:42.102028 robotframework-appiumlibrary-2.0.0b5/setup.cfg
--rwxr-xr-x   0 serhat.bolsu   (502) staff       (20)     2190 2022-10-29 09:40:35.000000 robotframework-appiumlibrary-2.0.0b5/setup.py
+drwxr-xr-x   0 emanlove   (501) staff       (20)        0 2024-05-18 01:53:09.830629 robotframework-appiumlibrary-2.1.0rc1/
+drwxr-xr-x   0 emanlove   (501) staff       (20)        0 2024-05-18 01:53:09.825159 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/
+-rw-r--r--   0 emanlove   (501) staff       (20)     5918 2024-05-18 00:22:24.000000 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/__init__.py
+drwxr-xr-x   0 emanlove   (501) staff       (20)        0 2024-05-18 01:53:09.828282 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/
+-rw-r--r--   0 emanlove   (501) staff       (20)      843 2024-04-27 13:15:52.000000 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/__init__.py
+-rw-r--r--   0 emanlove   (501) staff       (20)     6902 2024-05-18 00:22:24.000000 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/_android_utils.py
+-rw-r--r--   0 emanlove   (501) staff       (20)    18833 2024-04-27 13:15:52.000000 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/_applicationmanagement.py
+-rw-r--r--   0 emanlove   (501) staff       (20)    30501 2024-05-18 00:22:24.000000 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/_element.py
+-rw-r--r--   0 emanlove   (501) staff       (20)     1302 2024-04-27 13:15:52.000000 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/_keyevent.py
+-rw-r--r--   0 emanlove   (501) staff       (20)     1923 2024-04-27 13:15:52.000000 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/_logging.py
+-rw-r--r--   0 emanlove   (501) staff       (20)     2919 2024-04-27 13:15:52.000000 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/_runonfailure.py
+-rw-r--r--   0 emanlove   (501) staff       (20)     6787 2024-04-27 13:15:52.000000 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/_screenrecord.py
+-rw-r--r--   0 emanlove   (501) staff       (20)     1887 2024-04-27 13:15:52.000000 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/_screenshot.py
+-rw-r--r--   0 emanlove   (501) staff       (20)     9817 2024-05-18 00:22:24.000000 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/_touch.py
+-rw-r--r--   0 emanlove   (501) staff       (20)     6264 2024-04-27 13:15:52.000000 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/_waiting.py
+-rw-r--r--   0 emanlove   (501) staff       (20)     1037 2024-04-27 13:15:52.000000 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/keywordgroup.py
+drwxr-xr-x   0 emanlove   (501) staff       (20)        0 2024-05-18 01:53:09.828737 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/locators/
+-rw-r--r--   0 emanlove   (501) staff       (20)      109 2024-04-27 13:15:52.000000 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/locators/__init__.py
+-rw-r--r--   0 emanlove   (501) staff       (20)    11198 2024-04-27 13:15:52.000000 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/locators/elementfinder.py
+drwxr-xr-x   0 emanlove   (501) staff       (20)        0 2024-05-18 01:53:09.829181 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/utils/
+-rw-r--r--   0 emanlove   (501) staff       (20)      391 2024-04-27 13:15:52.000000 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/utils/__init__.py
+-rw-r--r--   0 emanlove   (501) staff       (20)     1024 2024-04-27 13:15:52.000000 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/utils/applicationcache.py
+-rw-r--r--   0 emanlove   (501) staff       (20)       45 2024-05-18 00:22:40.000000 robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/version.py
+-rw-r--r--   0 emanlove   (501) staff       (20)    10273 2024-04-27 13:15:52.000000 robotframework-appiumlibrary-2.1.0rc1/LICENSE
+-rw-r--r--   0 emanlove   (501) staff       (20)     7638 2024-05-18 01:53:09.830546 robotframework-appiumlibrary-2.1.0rc1/PKG-INFO
+-rw-r--r--   0 emanlove   (501) staff       (20)     6307 2024-05-18 01:52:51.000000 robotframework-appiumlibrary-2.1.0rc1/README.rst
+drwxr-xr-x   0 emanlove   (501) staff       (20)        0 2024-05-18 01:53:09.830211 robotframework-appiumlibrary-2.1.0rc1/robotframework_appiumlibrary.egg-info/
+-rw-r--r--   0 emanlove   (501) staff       (20)     7638 2024-05-18 01:53:09.000000 robotframework-appiumlibrary-2.1.0rc1/robotframework_appiumlibrary.egg-info/PKG-INFO
+-rw-r--r--   0 emanlove   (501) staff       (20)      950 2024-05-18 01:53:09.000000 robotframework-appiumlibrary-2.1.0rc1/robotframework_appiumlibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 emanlove   (501) staff       (20)        1 2024-05-18 01:53:09.000000 robotframework-appiumlibrary-2.1.0rc1/robotframework_appiumlibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 emanlove   (501) staff       (20)      137 2024-05-18 01:53:09.000000 robotframework-appiumlibrary-2.1.0rc1/robotframework_appiumlibrary.egg-info/requires.txt
+-rw-r--r--   0 emanlove   (501) staff       (20)       14 2024-05-18 01:53:09.000000 robotframework-appiumlibrary-2.1.0rc1/robotframework_appiumlibrary.egg-info/top_level.txt
+-rw-r--r--   0 emanlove   (501) staff       (20)      134 2024-05-18 01:53:09.831002 robotframework-appiumlibrary-2.1.0rc1/setup.cfg
+-rwxr-xr-x   0 emanlove   (501) staff       (20)     2202 2024-05-18 00:22:24.000000 robotframework-appiumlibrary-2.1.0rc1/setup.py
```

### Comparing `robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/__init__.py` & `robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     | identifier        | Click Element `|` identifier=my_element                        | Matches by @id attribute          |                             |
     | id                | Click Element `|` id=my_element                                | Matches by @resource-id attribute |                             |
     | accessibility_id  | Click Element `|` accessibility_id=button3                     | Accessibility options utilize.    |                             |
     | xpath             | Click Element `|` xpath=//UIATableView/UIATableCell/UIAButton  | Matches with arbitrary XPath      |                             |
     | class             | Click Element `|` class=UIAPickerWheel                         | Matches by class                  |                             |
     | android           | Click Element `|` android=UiSelector().description('Apps')     | Matches by Android UI Automator   |                             |
     | ios               | Click Element `|` ios=.buttons().withName('Apps')              | Matches by iOS UI Automation      |                             |
-    | nsp               | Click Element `|` nsp=name=="login"                            | Matches by iOSNsPredicate         | Check PR: #196              |
+    | predicate         | Click Element `|` predicate=name=="login"                      | Matches by iOS Predicate          | Check PR: #196              |
     | chain             | Click Element `|` chain=XCUIElementTypeWindow[1]/*             | Matches by iOS Class Chain        |                             |
     | css               | Click Element `|` css=.green_button                            | Matches by css in webview         |                             |
     | name              | Click Element `|` name=my_element                              | Matches by @name attribute        | *Only valid* for Selendroid |
 
     == Using webelements ==
 
     Starting with version 1.4 of the AppiumLibrary, one can pass an argument
@@ -75,29 +75,33 @@
     | Click Element    @{elements}[2]
 
     """
 
     ROBOT_LIBRARY_SCOPE = 'GLOBAL'
     ROBOT_LIBRARY_VERSION = VERSION
 
-    def __init__(self, timeout=5, run_on_failure='Capture Page Screenshot'):
+    def __init__(self, timeout=5, run_on_failure='Capture Page Screenshot', sleep_between_wait_loop=0.2):
         """AppiumLibrary can be imported with optional arguments.
 
         ``timeout`` is the default timeout used to wait for all waiting actions.
         It can be later set with `Set Appium Timeout`.
 
         ``run_on_failure`` specifies the name of a keyword (from any available
         libraries) to execute when a AppiumLibrary keyword fails.
 
         By default `Capture Page Screenshot` will be used to take a screenshot of the current page.
         Using the value `No Operation` will disable this feature altogether. See
         `Register Keyword To Run On Failure` keyword for more information about this
         functionality.
+        
+        ``sleep_between_wait_loop`` is the default sleep used to wait between loop in all wait until keywords
 
         Examples:
         | Library | AppiumLibrary | 10 | # Sets default timeout to 10 seconds                                                                             |
         | Library | AppiumLibrary | timeout=10 | run_on_failure=No Operation | # Sets default timeout to 10 seconds and does nothing on failure           |
+        | Library | AppiumLibrary | timeout=10 | sleep_between_wait_loop=0.3 | # Sets default timeout to 10 seconds and sleep 300 ms between wait loop    |
         """
         for base in AppiumLibrary.__bases__:
             base.__init__(self)
         self.set_appium_timeout(timeout)
         self.register_keyword_to_run_on_failure(run_on_failure)
+        self.set_sleep_between_wait_loop(sleep_between_wait_loop)
```

### Comparing `robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/__init__.py` & `robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/_android_utils.py` & `robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/_android_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,18 +159,14 @@
 
         Android only.
 
          - _activity_ - target activity
          - _timeout_ - max wait time, in seconds
          - _interval_ - sleep interval between retries, in seconds
         """
-
-        if not activity.startswith('.'):
-            activity = ".%s" % activity
-
         driver = self._current_application()
         if not driver.wait_activity(activity=activity, timeout=float(timeout), interval=float(interval)):
             raise TimeoutException(msg="Activity %s never presented, current activity: %s" % (activity, self.get_activity()))
 
     def install_app(self, app_path, app_package):
         """ Install App via Appium
```

### Comparing `robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/_applicationmanagement.py` & `robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/_applicationmanagement.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
         self._debug('Closing all applications')
         self._cache.close_all()
 
     def open_application(self, remote_url, alias=None, **kwargs):
         """Opens a new application to given Appium server.
         Capabilities of appium server, Android and iOS,
-        Please check https://github.com/appium/appium/blob/master/docs/en/writing-running-appium/server-args.md
+        Please check https://appium.io/docs/en/2.1/cli/args/
         | *Option*            | *Man.* | *Description*     |
         | remote_url          | Yes    | Appium server url |
         | alias               | no     | alias             |
         | strict_ssl          | No     | allows you to send commands to an invalid certificate host like a self-signed one. |
 
         Examples:
         | Open Application | http://localhost:4723/wd/hub | alias=Myapp1         | platformName=iOS      | platformVersion=7.0            | deviceName='iPhone Simulator'           | app=your.app                         |
@@ -467,15 +467,15 @@
     def _current_application(self):
         if not self._cache.current:
             raise RuntimeError('No application is open')
         return self._cache.current
 
     def _get_platform(self):
         try:
-            platform_name = self._current_application().desired_capabilities['platformName']
+            platform_name = self._current_application().capabilities['platformName']
         except Exception as e:
             raise e
         return platform_name.lower()
 
     def _is_platform(self, platform):
         platform_name = self._get_platform()
         return platform.lower() == platform_name
```

### Comparing `robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/_element.py` & `robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/_element.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,24 @@
 
         If there are multiple use  of ``text`` and you do not want first one,
         use `locator` with `Get Web Elements` instead.
 
         """
         self._element_find_by_text(text,exact_match).click()
 
+    def input_text_into_current_element(self, text):
+        """Types the given `text` into currently selected text field.
+
+            Android only.
+        """
+        self._info("Typing text '%s' into current text field" % text)
+        driver = self._current_application()
+        driver.set_clipboard_text(text)
+        driver.press_keycode(50, 0x1000 | 0x2000)
+
     def input_text(self, locator, text):
         """Types the given `text` into text field identified by `locator`.
 
         See `introduction` for details about locating elements.
         """
         self._info("Typing text '%s' into text field '%s'" % (text, locator))
         self._element_input_text_by_locator(locator, text)
@@ -233,19 +243,16 @@
 
         | 1. is a string pattern match i.e. the 'text' attribute should end with the string 'foobar'
         | 2. is a regular expression match i.e. the regexp 'f.*ar' should be within the 'text' attribute
         | 3. is a boolead match i.e. the 'enabled' attribute should be True
 
 
         _*NOTE: *_
-        On Android the supported attribute names are hard-coded in the
-        [https://github.com/appium/appium/blob/master/lib/devices/android/bootstrap/src/io/appium/android/bootstrap/AndroidElement.java|AndroidElement]
-        Class's getBoolAttribute() and getStringAttribute() methods.
-        Currently supported (appium v1.4.11):
-        _contentDescription, text, className, resourceId, enabled, checkable, checked, clickable, focusable, focused, longClickable, scrollable, selected, displayed_
+        On Android the supported attribute names can be found in the uiautomator2 driver readme:
+        [https://github.com/appium/appium-uiautomator2-driver?tab=readme-ov-file#element-attributes]
 
 
         _*NOTE: *_
         Some attributes can be evaluated in two different ways e.g. these evaluate the same thing:
 
         | Element Attribute Should Match | xpath = //*[contains(@text,'example text')] | name | txt_field_name |
         | Element Name Should Be         | xpath = //*[contains(@text,'example text')] | txt_field_name |      |
@@ -456,24 +463,26 @@
         `introduction` for details about locating elements.
         """
         element = self._element_find(locator, True, True)
         element_rect = element.rect
         self._info("Element '%s' rect: %s " % (locator, element_rect))
         return element_rect
 
-    def get_text(self, locator):
+    def get_text(self, locator, first_only: bool = True):
         """Get element text (for hybrid and mobile browser use `xpath` locator, others might cause problem)
 
-        Example:
+        first_only parameter allow to get the text from the 1st match (Default) or a list of text from all match.
 
-        | ${text} | Get Text | //*[contains(@text,'foo')] |
+        Example:
+        | ${text} | Get Text | //*[contains(@text,'foo')] |          |
+        | @{text} | Get Text | //*[contains(@text,'foo')] | ${False} |
 
         New in AppiumLibrary 1.4.
         """
-        text = self._get_text(locator)
+        text = self._get_text(locator, first_only)
         self._info("Element '%s' text is '%s' " % (locator, text))
         return text
 
     def get_matching_xpath_count(self, xpath):
         """Returns number of elements matching ``xpath``
 
         One should not use the `xpath=` prefix for 'xpath'. XPath is assumed.
@@ -656,18 +665,20 @@
         elif self._get_platform() == 'android':
             if exact_match:
                 _xpath = u'//*[@{}="{}"]'.format('text', text)
             else:
                 _xpath = u'//*[contains(@{},"{}")]'.format('text', text)
             return self._element_find(_xpath, True, True)
 
-    def _get_text(self, locator):
-        element = self._element_find(locator, True, True)
+    def _get_text(self, locator, first_only: bool = True):
+        element = self._element_find(locator, first_only, True)
         if element is not None:
-            return element.text
+            if first_only:
+                return element.text
+            return [el.text for el in element]
         return None
 
     def _is_text_present(self, text):
         text_norm = normalize('NFD', text)
         source_norm = normalize('NFD', self.get_source())
         return text_norm in source_norm
```

### Comparing `robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/_keyevent.py` & `robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/_keyevent.py`

 * *Files identical despite different names*

### Comparing `robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/_logging.py` & `robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/_logging.py`

 * *Files identical despite different names*

### Comparing `robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/_runonfailure.py` & `robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/_runonfailure.py`

 * *Files identical despite different names*

### Comparing `robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/_screenrecord.py` & `robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/_screenrecord.py`

 * *Files identical despite different names*

### Comparing `robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/_screenshot.py` & `robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/_screenshot.py`

 * *Files identical despite different names*

### Comparing `robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/_touch.py` & `robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/_touch.py`

 * *Files 20% similar despite different names*

```diff
@@ -163,14 +163,29 @@
         - ``number_of_touches`` - The number of touch points.
         """
         driver = self._current_application()
         element = self._element_find(locator, True, True)
         params = {'element': element, 'numberOfTaps': number_of_taps, 'numberOfTouches': number_of_touches}
         driver.execute_script("mobile: tapWithNumberOfTaps", params)
 
+    def click_alert_button(self, button_name):
+        """ Clicks on Alert button identified by Name.iOS only.
+
+        Args:
+        - ``button_name`` - Text on the iOS alert button.
+
+        Example:
+        |  Click Alert Button  |  Allow  |
+
+        New in AppiumLibrary v2
+        """
+        driver = self._current_application()
+        params={'action': 'accept', 'buttonLabel': button_name}
+        driver.execute_script("mobile: alert", params)
+
     def click_a_point(self, x=0, y=0, duration=100):
         """*DEPRECATED!!* Since selenium v4, use other keywords.
 
         Click on a point"""
         self._info("Clicking on a point (%s,%s)." % (x,y))
         driver = self._current_application()
         action = TouchAction(driver)
@@ -184,14 +199,40 @@
 
         click element at a certain coordinate """
         self._info("Pressing at (%s, %s)." % (coordinate_X, coordinate_Y))
         driver = self._current_application()
         action = TouchAction(driver)
         action.press(x=coordinate_X, y=coordinate_Y).release().perform()
 
-    def drag_and_drop(self):
-        """TO BE IMPLEMENTED
-        Refer to : appium.webdriver.extensions.action_helpers"""
-
-    def flick(self):
-        """TO BE IMPLEMENTED
-        Refer to : appium.webdriver.extensions.action_helpers"""
+    def drag_and_drop(self, locator: str, target: str):
+        """Drags the element identified by ``locator`` into the ``target`` element.
+
+        The ``locator`` argument is the locator of the dragged element
+        and the ``target`` is the locator of the target. See the
+        `Locating elements` section for details about the locator syntax.
+
+        Args:
+        - ``origin`` - the element to drag
+        - ``destination`` - the element to drag to
+
+        Usage:
+        | `Drag And Drop` | id=div#element | id=div.target |
+        """
+        element = self._element_find(locator, True, True)
+        target = self._element_find(target, True, True)
+        driver = self._current_application()
+        driver.drag_and_drop(element, target)
+
+    def flick(self, start_x:int, start_y:int, end_x:int, end_y:int):
+        """Flick from one point to another point.
+
+        Args:
+        - ``start_x`` - x-coordinate at which to start
+        - ``start_y`` - y-coordinate at which to start
+        - ``end_x``   - x-coordinate at which to stop
+        - ``end_y``   - y-coordinate at which to stop
+
+        Usage:
+        | Flick | 100 | 100 | 100 | 400 | # Flicks the screen up. |
+        """
+        driver = self._current_application()
+        driver.flick(start_x, start_y, end_x, end_y)
```

### Comparing `robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/_waiting.py` & `robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/_waiting.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import time
 import robot
 from .keywordgroup import KeywordGroup
 
 
 class _WaitingKeywords(KeywordGroup):
+    
+    def __init__(self):
+        self._sleep_between_wait = 0.2
+        
     def wait_until_element_is_visible(self, locator, timeout=None, error=None):
         """Waits until element specified with `locator` is visible.
 
         Fails if `timeout` expires before the element is visible. See
         `introduction` for more information about `timeout` and its
         default value.
 
@@ -107,14 +111,30 @@
             if not present:
                 return
             else:
                 return error or "Element '%s' did not disappear in %s" % (locator, self._format_timeout(timeout))
 
         self._wait_until_no_error(timeout, check_present)
 
+    def set_sleep_between_wait_loop(self, seconds=0.2):
+        """Sets the sleep in seconds used by wait until loop.
+        
+        If you use the remote appium server, the default value is not recommended because 
+        it is another 200ms overhead to the network latency and will slow down your test
+        execution.
+        """
+        old_sleep = self._sleep_between_wait
+        self._sleep_between_wait = robot.utils.timestr_to_secs(seconds)
+        return old_sleep
+    
+    def get_sleep_between_wait_loop(self):
+        """Gets the sleep between wait loop in seconds that is used by wait until keywords.
+        """
+        return robot.utils.secs_to_timestr(self._sleep_between_wait)
+    
     # Private
 
     def _wait_until(self, timeout, error, function, *args):
         error = error.replace('<TIMEOUT>', self._format_timeout(timeout))
 
         def wait_func():
             return None if function(*args) else error
@@ -127,12 +147,12 @@
         while True:
             timeout_error = wait_func(*args)
             if not timeout_error:
                 return
             if time.time() > maxtime:
                 self.log_source()
                 raise AssertionError(timeout_error)
-            time.sleep(0.2)
+            time.sleep(self._sleep_between_wait)
 
     def _format_timeout(self, timeout):
         timeout = robot.utils.timestr_to_secs(timeout) if timeout is not None else self._timeout_in_secs
         return robot.utils.secs_to_timestr(timeout)
```

### Comparing `robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/keywords/keywordgroup.py` & `robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/keywords/keywordgroup.py`

 * *Files identical despite different names*

### Comparing `robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/locators/elementfinder.py` & `robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/locators/elementfinder.py`

 * *Files identical despite different names*

### Comparing `robotframework-appiumlibrary-2.0.0b5/AppiumLibrary/utils/applicationcache.py` & `robotframework-appiumlibrary-2.1.0rc1/AppiumLibrary/utils/applicationcache.py`

 * *Files identical despite different names*

### Comparing `robotframework-appiumlibrary-2.0.0b5/LICENSE` & `robotframework-appiumlibrary-2.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-appiumlibrary-2.0.0b5/PKG-INFO` & `robotframework-appiumlibrary-2.1.0rc1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: robotframework-appiumlibrary
-Version: 2.0.0b5
-Summary: Robot Framework Mobile app testing library for Appium Client Android & iOS & Web
-Home-page: https://github.com/serhatbolsu/robotframework-appiumlibrary
-Author: Serhat Bolsu, William Zhang, Xie Lieping, Jari Nurminen
-Author-email: serhatbolsu@gmail.com,jollychang@gmail.com,frankbp@gmail.com
-License: Apache License 2.0
-Keywords: robotframework testing testautomation mobile appium webdriver app android ios
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: Topic :: Software Development :: Testing
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Framework :: Robot Framework
-Classifier: Framework :: Robot Framework :: Library
-License-File: LICENSE
-
 Appium library for RobotFramework
 ==================================================
 
 Introduction
 ------------
 
 AppiumLibrary_ is an appium testing library for `Robot Framework`_. Library can be downloaded from PyPI_.
@@ -38,33 +15,52 @@
     :target: https://pypi.python.org/pypi/robotframework-appiumlibrary/
     :alt: Latest PyPI version
 
 .. image:: https://img.shields.io/pypi/dm/robotframework-appiumlibrary.svg
     :target: https://pypi.python.org/pypi/robotframework-appiumlibrary/
     :alt: Number of PyPI downloads
 
+.. image:: https://img.shields.io/badge/License-Apache%202.0-blue.svg
+    :target: https://opensource.org/licenses/Apache-2.0
+    :alt: License
+
 
 .. contents::
 
 
 Keyword Documentation
 ---------------------
 
 See `Keyword Documentation`_ for available keywords and more information about the library in general.
 
 
 Installation
 ------------
 
+**Option 1**  (recommended)
+
 The recommended installation method is using
 `pip <http://pip-installer.org>`__::
 
     pip install --upgrade robotframework-appiumlibrary
 
 
+**Option 2**  
+
+It is possible to install directly from GitHub repository. To Install latest source
+from the master branch, use this command:
+`pip <http://pip-installer.org>`__::
+
+  pip install git+https://github.com/serhatbolsu/robotframework-appiumlibrary.git
+
+Please note that installation will take some time, because ``pip`` will
+clone the `AppiumLibrary`_ project to a temporary directory and then
+perform the installation.
+
+
 See `Robot Framework installation instructions`_ for detailed information
 about installing Python and Robot Framework itself.
 
 Device Setup
 ------------
 After installing the library, you still need to setup an simulator/emulator or real device to use in tests.
 iOS and Android have separate paths to follow, and those steps better explained in `Appium Driver Setup Guide`_.
@@ -136,23 +132,32 @@
 
 Contributing
 -------------
 Fork the project, make a change, and send a pull request!
 
 Project Contributors
 --------------------
-* `Serhat Bolsu <https://github.com/serhatbolsu>`_
-* `William Zhang <https://github.com/jollychang>`_
-* `Xie Lieping <https://github.com/frankbp>`_
-* `Jari Nurminen <https://github.com/yahman72>`_
+
+==============  ====================  ============
+William Zhang   akupahkala            Arnaud Ruffin
+Serhat Bolsu    soukingang            Junuen Villa
+Xie Lieping     Erik Bartalos         Tanakiat Srisaranyakul
+Joshua Rivera   Minh Nguyen           Thiago Paiva Brito
+js361014        Sadik Kuzu            Jonathan Gayvallet
+matthew-dahm    KumarS                jennyw1
+JMcn            Xia Clark             ac-simoes
+Ulhas Deshmukh  Leon Guo              Pramod
+smaspe          eXtReMaL              Erol Selitektay
+Filipe Arruda   Felipe Luiz Tortella  Filipe Henrique Benjamim de Arruda
+==============  ====================  ============
+
 
 AppiumLibrary is modeled after (and forked from)  `appiumandroidlibrary <https://github.com/frankbp/robotframework-appiumandroidlibrary>`_,  but re-implemented to use appium 1.X technologies.
 
 
 .. _AppiumLibrary: https://github.com/serhatbolsu/robotframework-appiumlibrary
 .. _Robot Framework: https://robotframework.org
 .. _Keyword Documentation: http://serhatbolsu.github.io/robotframework-appiumlibrary/AppiumLibrary.html
 .. _PyPI: https://pypi.org/project/robotframework-appiumlibrary/
 .. _Robot Framework installation instructions: https://github.com/robotframework/robotframework/blob/master/INSTALL.rst
 .. _Appium Driver Setup Guide: http://appium.io/docs/en/about-appium/getting-started/?lang=en
 .. _sample project: https://github.com/serhatbolsu/robotframework-appium-sample
-
```

### Comparing `robotframework-appiumlibrary-2.0.0b5/robotframework_appiumlibrary.egg-info/SOURCES.txt` & `robotframework-appiumlibrary-2.1.0rc1/robotframework_appiumlibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-appiumlibrary-2.0.0b5/setup.py` & `robotframework-appiumlibrary-2.1.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
       setup_requires=[
           "pytest-runner"
       ],
       install_requires=[
           'decorator >= 3.3.2',
           'robotframework >= 2.6.0',
           'docutils >= 0.8.1',
-          'Appium-Python-Client >= 2.7.1',
-          'selenium >= 4.0.0',
+          'selenium >=4.0,<=4.9',
+          'Appium-Python-Client >= 2.7.1, < 4.0.0',
           'kitchen >= 1.2.4',
           'six >= 1.10.0'
       ],
       tests_require=[
           'mock >= 2.0.0',
           'pytest-cov >= 2.5.1',
           'pytest-xdist >= 1.16.0',
```

