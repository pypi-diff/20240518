# Comparing `tmp/appstrings-1.0.1.tar.gz` & `tmp/appstrings-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appstrings-1.0.1.tar", last modified: Thu Jan 25 08:45:59 2024, max compression
+gzip compressed data, was "appstrings-1.0.2.tar", last modified: Sat May 18 08:57:40 2024, max compression
```

## Comparing `appstrings-1.0.1.tar` & `appstrings-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-01-25 08:45:59.868596 appstrings-1.0.1/
--rw-rw-rw-   0        0        0    14114 2024-01-24 17:51:47.000000 appstrings-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    23818 2024-01-25 08:45:59.868596 appstrings-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6754 2024-01-25 08:31:22.000000 appstrings-1.0.1/README.md
--rw-rw-rw-   0        0        0     1270 2024-01-25 07:21:18.000000 appstrings-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-25 08:45:59.868596 appstrings-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-25 08:45:59.849935 appstrings-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-01-25 08:45:59.867669 appstrings-1.0.1/src/appstrings.egg-info/
--rw-rw-rw-   0        0        0    23818 2024-01-25 08:45:59.000000 appstrings-1.0.1/src/appstrings.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-01-25 08:45:59.000000 appstrings-1.0.1/src/appstrings.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-25 08:45:59.000000 appstrings-1.0.1/src/appstrings.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-01-25 08:45:59.000000 appstrings-1.0.1/src/appstrings.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13736 2024-01-25 08:01:42.000000 appstrings-1.0.1/src/appstrings.py
+drwxrwxrwx   0        0        0        0 2024-05-18 08:57:40.206525 appstrings-1.0.2/
+-rw-rw-rw-   0        0        0       66 2024-01-23 07:14:34.000000 appstrings-1.0.2/.gitattributes
+-rw-rw-rw-   0        0        0     2915 2024-01-23 07:14:34.000000 appstrings-1.0.2/.gitignore
+-rw-rw-rw-   0        0        0    14114 2024-05-16 11:27:57.000000 appstrings-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0    23824 2024-05-18 08:57:40.205525 appstrings-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6760 2024-05-18 08:55:57.000000 appstrings-1.0.2/README.md
+-rw-rw-rw-   0        0        0     1270 2024-05-18 08:52:40.000000 appstrings-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-18 08:57:40.206525 appstrings-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-18 08:57:40.189530 appstrings-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-18 08:57:40.204525 appstrings-1.0.2/src/appstrings.egg-info/
+-rw-rw-rw-   0        0        0    23824 2024-05-18 08:57:40.000000 appstrings-1.0.2/src/appstrings.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-05-18 08:57:40.000000 appstrings-1.0.2/src/appstrings.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 08:57:40.000000 appstrings-1.0.2/src/appstrings.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-18 08:57:40.000000 appstrings-1.0.2/src/appstrings.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8532 2024-05-18 08:55:57.000000 appstrings-1.0.2/src/appstrings.py
+drwxrwxrwx   0        0        0        0 2024-05-18 08:57:40.203524 appstrings-1.0.2/tests/
+-rw-rw-rw-   0        0        0     5628 2024-05-18 08:55:57.000000 appstrings-1.0.2/tests/test.py
```

### Comparing `appstrings-1.0.1/LICENSE` & `appstrings-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `appstrings-1.0.1/PKG-INFO` & `appstrings-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appstrings
-Version: 1.0.1
+Version: 1.0.2
 Summary: Minimal string translation library
 Author: Ángel Fernández Pineda
 License:                       EUROPEAN UNION PUBLIC LICENCE v. 1.2
                               EUPL © the European Union 2007, 2016
         
         This European Union Public Licence (the ‘EUPL’) applies to the Work (as defined
         below) which is provided under the terms of this Licence. Any use of the Work,
@@ -398,49 +398,49 @@
 # _ = gettext
 
 _ = lambda id: id._value_
 
 print(_(EN.TEST)) # Always print all strings in english, for now
 ```
 
-The library chooses the best-matching translator for the current translation locale, which is initialized from `locale.getlocale()`.
+The library chooses the best-matching translator for the current translation locale, which is initialized from `_locale._getdefaultlocale()`.
 You may force a specific locale for translation at any time:
 
 ```python
 from appstrings import set_translation_locale
 
 set_translation_locale("es_MX")
-print(_(EN.TEST)) # Prints text in spanish language of Mexico
+print(_(EN.TEST)) # Prints text in Spanish language of Mexico
 ```
 
 then force the system locale again:
 
 ```python
 set_translation_locale()
 ```
 
 Note that forcing a specific locale not available in your application will not *magically* translate your strings to that locale.
 
 ### Fallback to a default language
 
 In the previous examples, there is no translator for the locale *pt_BR*, to say one.
 In such a case, the translator used in `gettext()` will work as the **default language** for non-translated locales.
-In the early example, brazilian people would read the text in english.
-However, if `print(_(ES_MX.TEST))` were used instead, brazilian people would read the text in spanish.
+In the early example, Brazilian people would read the text in english.
+However, if `print(_(ES_MX.TEST))` were used instead, Brazilian people would read the text in Spanish.
 
 The ability to change the default language at any time comes from aliases:
 
 ```python
 STR = EN
 
 print(_(STR.TEST)) # Prints TEST string in english if there is no matching translator
 
 STR = ES_MX
 
-print(_(STR.TEST)) # Prints TEST string in spanish if there is no matching translator
+print(_(STR.TEST)) # Prints TEST string in Spanish if there is no matching translator
 ```
 
 This approach is developer-friendly, but not user-friendly.
 
 ### Be user-friendly
 
 Your application should allow the user to choose an available language
@@ -466,30 +466,30 @@
 
 For example:
 
 ```mermaid
 flowchart TB
     main["__main__.py (your application)"]
     default["translation.py (defines default language)"]
-    lang_es["translation_es.py (defines spanish translator)"]
-    lang_pt["translation_pt.py (defines portuguese translator)"]
+    lang_es["translation_es.py (defines Spanish translator)"]
+    lang_pt["translation_pt.py (defines Portuguese translator)"]
 
     main --imports--> default
     default --imports--> lang_es
     default --imports--> lang_pt
 ```
 
 But the following schema will work just the same:
 
 ```mermaid
 flowchart TB
     main["__main__.py (your application)"]
     default["translation.py (defines default language)"]
-    lang_es["translation_es.py (defines spanish translator)"]
-    lang_pt["translation_pt.py (defines portuguese translator)"]
+    lang_es["translation_es.py (defines Spanish translator)"]
+    lang_pt["translation_pt.py (defines Portuguese translator)"]
 
     main --imports--> default
     main --imports--> lang_es
     main --imports--> lang_pt
 ```
 
 The "translation*.py" files would look like this:
@@ -510,14 +510,14 @@
 
 That is all about this library. As simple as that.
 
 ### Troubleshooting
 
 - Why some strings are properly translated, but not others?
 
-  - Ensure all your translators have a *_domain* attribute set to the very same value (case-sensitive).
+  Ensure all your translators have a *_domain* attribute set to the very same value (case-sensitive).
 
 - I get a TranslatorException : *String ID XXX from YYYY is missing at ZZZZ*. Why ?
 
   There are two possible reasons:
   - One of your translators is missing a string that others have. Check.
-  - Your application is in conflict with some library. User another string int the "_domain" attribute.
+  - Your application is in conflict with some library. User another string in the "_domain" attribute.
```

### Comparing `appstrings-1.0.1/README.md` & `appstrings-1.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -94,49 +94,49 @@
 # _ = gettext
 
 _ = lambda id: id._value_
 
 print(_(EN.TEST)) # Always print all strings in english, for now
 ```
 
-The library chooses the best-matching translator for the current translation locale, which is initialized from `locale.getlocale()`.
+The library chooses the best-matching translator for the current translation locale, which is initialized from `_locale._getdefaultlocale()`.
 You may force a specific locale for translation at any time:
 
 ```python
 from appstrings import set_translation_locale
 
 set_translation_locale("es_MX")
-print(_(EN.TEST)) # Prints text in spanish language of Mexico
+print(_(EN.TEST)) # Prints text in Spanish language of Mexico
 ```
 
 then force the system locale again:
 
 ```python
 set_translation_locale()
 ```
 
 Note that forcing a specific locale not available in your application will not *magically* translate your strings to that locale.
 
 ### Fallback to a default language
 
 In the previous examples, there is no translator for the locale *pt_BR*, to say one.
 In such a case, the translator used in `gettext()` will work as the **default language** for non-translated locales.
-In the early example, brazilian people would read the text in english.
-However, if `print(_(ES_MX.TEST))` were used instead, brazilian people would read the text in spanish.
+In the early example, Brazilian people would read the text in english.
+However, if `print(_(ES_MX.TEST))` were used instead, Brazilian people would read the text in Spanish.
 
 The ability to change the default language at any time comes from aliases:
 
 ```python
 STR = EN
 
 print(_(STR.TEST)) # Prints TEST string in english if there is no matching translator
 
 STR = ES_MX
 
-print(_(STR.TEST)) # Prints TEST string in spanish if there is no matching translator
+print(_(STR.TEST)) # Prints TEST string in Spanish if there is no matching translator
 ```
 
 This approach is developer-friendly, but not user-friendly.
 
 ### Be user-friendly
 
 Your application should allow the user to choose an available language
@@ -162,30 +162,30 @@
 
 For example:
 
 ```mermaid
 flowchart TB
     main["__main__.py (your application)"]
     default["translation.py (defines default language)"]
-    lang_es["translation_es.py (defines spanish translator)"]
-    lang_pt["translation_pt.py (defines portuguese translator)"]
+    lang_es["translation_es.py (defines Spanish translator)"]
+    lang_pt["translation_pt.py (defines Portuguese translator)"]
 
     main --imports--> default
     default --imports--> lang_es
     default --imports--> lang_pt
 ```
 
 But the following schema will work just the same:
 
 ```mermaid
 flowchart TB
     main["__main__.py (your application)"]
     default["translation.py (defines default language)"]
-    lang_es["translation_es.py (defines spanish translator)"]
-    lang_pt["translation_pt.py (defines portuguese translator)"]
+    lang_es["translation_es.py (defines Spanish translator)"]
+    lang_pt["translation_pt.py (defines Portuguese translator)"]
 
     main --imports--> default
     main --imports--> lang_es
     main --imports--> lang_pt
 ```
 
 The "translation*.py" files would look like this:
@@ -206,14 +206,14 @@
 
 That is all about this library. As simple as that.
 
 ### Troubleshooting
 
 - Why some strings are properly translated, but not others?
 
-  - Ensure all your translators have a *_domain* attribute set to the very same value (case-sensitive).
+  Ensure all your translators have a *_domain* attribute set to the very same value (case-sensitive).
 
 - I get a TranslatorException : *String ID XXX from YYYY is missing at ZZZZ*. Why ?
 
   There are two possible reasons:
   - One of your translators is missing a string that others have. Check.
-  - Your application is in conflict with some library. User another string int the "_domain" attribute.
+  - Your application is in conflict with some library. User another string in the "_domain" attribute.
```

### Comparing `appstrings-1.0.1/pyproject.toml` & `appstrings-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "Programming Language :: Python :: 3.11",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Internationalization",
     "License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)"
 ]
 # dynamic = ["version"]
-version = "1.0.1"
+version = "1.0.2"
 
 ## Back-end specific configuration
 
 [tool.setuptools]
 py-modules = [
     "appstrings"
 ]
```

### Comparing `appstrings-1.0.1/src/appstrings.egg-info/PKG-INFO` & `appstrings-1.0.2/src/appstrings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appstrings
-Version: 1.0.1
+Version: 1.0.2
 Summary: Minimal string translation library
 Author: Ángel Fernández Pineda
 License:                       EUROPEAN UNION PUBLIC LICENCE v. 1.2
                               EUPL © the European Union 2007, 2016
         
         This European Union Public Licence (the ‘EUPL’) applies to the Work (as defined
         below) which is provided under the terms of this Licence. Any use of the Work,
@@ -398,49 +398,49 @@
 # _ = gettext
 
 _ = lambda id: id._value_
 
 print(_(EN.TEST)) # Always print all strings in english, for now
 ```
 
-The library chooses the best-matching translator for the current translation locale, which is initialized from `locale.getlocale()`.
+The library chooses the best-matching translator for the current translation locale, which is initialized from `_locale._getdefaultlocale()`.
 You may force a specific locale for translation at any time:
 
 ```python
 from appstrings import set_translation_locale
 
 set_translation_locale("es_MX")
-print(_(EN.TEST)) # Prints text in spanish language of Mexico
+print(_(EN.TEST)) # Prints text in Spanish language of Mexico
 ```
 
 then force the system locale again:
 
 ```python
 set_translation_locale()
 ```
 
 Note that forcing a specific locale not available in your application will not *magically* translate your strings to that locale.
 
 ### Fallback to a default language
 
 In the previous examples, there is no translator for the locale *pt_BR*, to say one.
 In such a case, the translator used in `gettext()` will work as the **default language** for non-translated locales.
-In the early example, brazilian people would read the text in english.
-However, if `print(_(ES_MX.TEST))` were used instead, brazilian people would read the text in spanish.
+In the early example, Brazilian people would read the text in english.
+However, if `print(_(ES_MX.TEST))` were used instead, Brazilian people would read the text in Spanish.
 
 The ability to change the default language at any time comes from aliases:
 
 ```python
 STR = EN
 
 print(_(STR.TEST)) # Prints TEST string in english if there is no matching translator
 
 STR = ES_MX
 
-print(_(STR.TEST)) # Prints TEST string in spanish if there is no matching translator
+print(_(STR.TEST)) # Prints TEST string in Spanish if there is no matching translator
 ```
 
 This approach is developer-friendly, but not user-friendly.
 
 ### Be user-friendly
 
 Your application should allow the user to choose an available language
@@ -466,30 +466,30 @@
 
 For example:
 
 ```mermaid
 flowchart TB
     main["__main__.py (your application)"]
     default["translation.py (defines default language)"]
-    lang_es["translation_es.py (defines spanish translator)"]
-    lang_pt["translation_pt.py (defines portuguese translator)"]
+    lang_es["translation_es.py (defines Spanish translator)"]
+    lang_pt["translation_pt.py (defines Portuguese translator)"]
 
     main --imports--> default
     default --imports--> lang_es
     default --imports--> lang_pt
 ```
 
 But the following schema will work just the same:
 
 ```mermaid
 flowchart TB
     main["__main__.py (your application)"]
     default["translation.py (defines default language)"]
-    lang_es["translation_es.py (defines spanish translator)"]
-    lang_pt["translation_pt.py (defines portuguese translator)"]
+    lang_es["translation_es.py (defines Spanish translator)"]
+    lang_pt["translation_pt.py (defines Portuguese translator)"]
 
     main --imports--> default
     main --imports--> lang_es
     main --imports--> lang_pt
 ```
 
 The "translation*.py" files would look like this:
@@ -510,14 +510,14 @@
 
 That is all about this library. As simple as that.
 
 ### Troubleshooting
 
 - Why some strings are properly translated, but not others?
 
-  - Ensure all your translators have a *_domain* attribute set to the very same value (case-sensitive).
+  Ensure all your translators have a *_domain* attribute set to the very same value (case-sensitive).
 
 - I get a TranslatorException : *String ID XXX from YYYY is missing at ZZZZ*. Why ?
 
   There are two possible reasons:
   - One of your translators is missing a string that others have. Check.
-  - Your application is in conflict with some library. User another string int the "_domain" attribute.
+  - Your application is in conflict with some library. User another string in the "_domain" attribute.
```

