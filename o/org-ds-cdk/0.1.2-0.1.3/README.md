# Comparing `tmp/org-ds-cdk-0.1.2.tar.gz` & `tmp/org-ds-cdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "org-ds-cdk-0.1.2.tar", last modified: Sat May 18 06:28:04 2024, max compression
+gzip compressed data, was "org-ds-cdk-0.1.3.tar", last modified: Sat May 18 09:22:01 2024, max compression
```

## Comparing `org-ds-cdk-0.1.2.tar` & `org-ds-cdk-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-18 06:28:04.329251 org-ds-cdk-0.1.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      207 2024-05-18 06:28:04.329251 org-ds-cdk-0.1.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      981 2024-05-18 05:53:16.000000 org-ds-cdk-0.1.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-18 06:28:04.321250 org-ds-cdk-0.1.2/lib/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-18 06:28:04.325250 org-ds-cdk-0.1.2/lib/org_ds_cdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      207 2024-05-18 06:28:04.000000 org-ds-cdk-0.1.2/lib/org_ds_cdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      207 2024-05-18 06:28:04.000000 org-ds-cdk-0.1.2/lib/org_ds_cdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-18 06:28:04.000000 org-ds-cdk-0.1.2/lib/org_ds_cdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2024-05-18 06:28:04.000000 org-ds-cdk-0.1.2/lib/org_ds_cdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-18 06:28:04.000000 org-ds-cdk-0.1.2/lib/org_ds_cdk.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-18 06:28:04.329251 org-ds-cdk-0.1.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      572 2024-05-18 06:25:19.000000 org-ds-cdk-0.1.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-18 09:22:01.813803 org-ds-cdk-0.1.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      207 2024-05-18 09:22:01.813803 org-ds-cdk-0.1.3/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      981 2024-05-18 05:53:16.000000 org-ds-cdk-0.1.3/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-18 09:22:01.809803 org-ds-cdk-0.1.3/lib/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-18 09:22:01.813803 org-ds-cdk-0.1.3/lib/org_ds_cdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      207 2024-05-18 09:22:01.000000 org-ds-cdk-0.1.3/lib/org_ds_cdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      207 2024-05-18 09:22:01.000000 org-ds-cdk-0.1.3/lib/org_ds_cdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-18 09:22:01.000000 org-ds-cdk-0.1.3/lib/org_ds_cdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2024-05-18 09:22:01.000000 org-ds-cdk-0.1.3/lib/org_ds_cdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-18 09:22:01.000000 org-ds-cdk-0.1.3/lib/org_ds_cdk.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-18 09:22:01.813803 org-ds-cdk-0.1.3/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      572 2024-05-18 09:22:00.000000 org-ds-cdk-0.1.3/setup.py
```

### Comparing `org-ds-cdk-0.1.2/README.md` & `org-ds-cdk-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `org-ds-cdk-0.1.2/setup.py` & `org-ds-cdk-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Read the contents of your README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='org-ds-cdk',
-    version='0.1.02',
+    version='0.1.03',
     description='Constructs for creating an API Gateway and Routes from input JSON configuration',
     packages=find_packages('lib'),
     package_dir={'': 'lib'},
     install_requires=[
         'aws-cdk-lib==2.142.0',
         'constructs>=10.0.0'
     ],
```

