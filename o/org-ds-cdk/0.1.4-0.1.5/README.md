# Comparing `tmp/org-ds-cdk-0.1.4.tar.gz` & `tmp/org-ds-cdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "org-ds-cdk-0.1.4.tar", last modified: Sat May 18 09:41:43 2024, max compression
+gzip compressed data, was "org-ds-cdk-0.1.5.tar", last modified: Sat May 18 09:50:24 2024, max compression
```

## Comparing `org-ds-cdk-0.1.4.tar` & `org-ds-cdk-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-18 09:41:43.320026 org-ds-cdk-0.1.4/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      207 2024-05-18 09:41:43.320026 org-ds-cdk-0.1.4/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      981 2024-05-18 05:53:16.000000 org-ds-cdk-0.1.4/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-18 09:41:43.316025 org-ds-cdk-0.1.4/lib/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-18 09:41:43.320026 org-ds-cdk-0.1.4/lib/org_dist_cdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-18 07:05:46.000000 org-ds-cdk-0.1.4/lib/org_dist_cdk/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1919 2024-05-18 04:59:50.000000 org-ds-cdk-0.1.4/lib/org_dist_cdk/apigateway.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1349 2024-05-18 09:32:10.000000 org-ds-cdk-0.1.4/lib/org_dist_cdk/multilambda.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-18 09:41:43.320026 org-ds-cdk-0.1.4/lib/org_ds_cdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      207 2024-05-18 09:41:43.000000 org-ds-cdk-0.1.4/lib/org_ds_cdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      299 2024-05-18 09:41:43.000000 org-ds-cdk-0.1.4/lib/org_ds_cdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-18 09:41:43.000000 org-ds-cdk-0.1.4/lib/org_ds_cdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2024-05-18 09:41:43.000000 org-ds-cdk-0.1.4/lib/org_ds_cdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2024-05-18 09:41:43.000000 org-ds-cdk-0.1.4/lib/org_ds_cdk.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-18 09:41:43.320026 org-ds-cdk-0.1.4/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      572 2024-05-18 09:33:24.000000 org-ds-cdk-0.1.4/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-18 09:50:24.159509 org-ds-cdk-0.1.5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1221 2024-05-18 09:50:24.155508 org-ds-cdk-0.1.5/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      981 2024-05-18 05:53:16.000000 org-ds-cdk-0.1.5/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-18 09:50:24.155508 org-ds-cdk-0.1.5/lib/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-18 09:50:24.155508 org-ds-cdk-0.1.5/lib/org_ds_cdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-18 07:05:46.000000 org-ds-cdk-0.1.5/lib/org_ds_cdk/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1919 2024-05-18 04:59:50.000000 org-ds-cdk-0.1.5/lib/org_ds_cdk/apigateway.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1349 2024-05-18 09:32:10.000000 org-ds-cdk-0.1.5/lib/org_ds_cdk/multilambda.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-18 09:50:24.155508 org-ds-cdk-0.1.5/lib/org_ds_cdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1221 2024-05-18 09:50:24.000000 org-ds-cdk-0.1.5/lib/org_ds_cdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      293 2024-05-18 09:50:24.000000 org-ds-cdk-0.1.5/lib/org_ds_cdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-18 09:50:24.000000 org-ds-cdk-0.1.5/lib/org_ds_cdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2024-05-18 09:50:24.000000 org-ds-cdk-0.1.5/lib/org_ds_cdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2024-05-18 09:50:24.000000 org-ds-cdk-0.1.5/lib/org_ds_cdk.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-18 09:50:24.159509 org-ds-cdk-0.1.5/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      662 2024-05-18 09:49:59.000000 org-ds-cdk-0.1.5/setup.py
```

### Comparing `org-ds-cdk-0.1.4/README.md` & `org-ds-cdk-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `org-ds-cdk-0.1.4/lib/org_dist_cdk/apigateway.py` & `org-ds-cdk-0.1.5/lib/org_ds_cdk/apigateway.py`

 * *Files identical despite different names*

### Comparing `org-ds-cdk-0.1.4/lib/org_dist_cdk/multilambda.py` & `org-ds-cdk-0.1.5/lib/org_ds_cdk/multilambda.py`

 * *Files identical despite different names*

### Comparing `org-ds-cdk-0.1.4/setup.py` & `org-ds-cdk-0.1.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 # Read the contents of your README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='org-ds-cdk',
-    version='0.1.04',
+    version='0.1.05',
     description='Constructs for creating an API Gateway and Routes from input JSON configuration',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     packages=find_packages('lib'),
     package_dir={'': 'lib'},
     install_requires=[
         'aws-cdk-lib==2.142.0',
         'constructs>=10.0.0'
     ],
 )
```

