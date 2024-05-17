# Comparing `tmp/tensorset-0.4.1.tar.gz` & `tmp/tensorset-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorset-0.4.1.tar", last modified: Tue May 14 16:52:55 2024, max compression
+gzip compressed data, was "tensorset-0.4.2.tar", last modified: Fri May 17 22:55:01 2024, max compression
```

## Comparing `tensorset-0.4.1.tar` & `tensorset-0.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:52:55.732997 tensorset-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-14 16:52:55.732997 tensorset-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-14 16:52:48.000000 tensorset-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:52:55.732997 tensorset-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-14 16:52:48.000000 tensorset-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:52:55.728997 tensorset-0.4.1/tensorset/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 16:52:48.000000 tensorset-0.4.1/tensorset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-14 16:52:48.000000 tensorset-0.4.1/tensorset/tensorset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:52:55.732997 tensorset-0.4.1/tensorset/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:52:48.000000 tensorset-0.4.1/tensorset/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-05-14 16:52:48.000000 tensorset-0.4.1/tensorset/tests/test_tensorset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:52:55.732997 tensorset-0.4.1/tensorset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-14 16:52:55.000000 tensorset-0.4.1/tensorset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-14 16:52:55.000000 tensorset-0.4.1/tensorset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:52:55.000000 tensorset-0.4.1/tensorset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 16:52:55.000000 tensorset-0.4.1/tensorset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 16:52:55.000000 tensorset-0.4.1/tensorset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:55:01.600428 tensorset-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-17 22:55:01.600428 tensorset-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-17 22:54:57.000000 tensorset-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 22:55:01.600428 tensorset-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-17 22:54:57.000000 tensorset-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:55:01.596428 tensorset-0.4.2/tensorset/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-17 22:54:57.000000 tensorset-0.4.2/tensorset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-05-17 22:54:57.000000 tensorset-0.4.2/tensorset/tensorset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:55:01.600428 tensorset-0.4.2/tensorset/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:54:57.000000 tensorset-0.4.2/tensorset/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7303 2024-05-17 22:54:57.000000 tensorset-0.4.2/tensorset/tests/test_tensorset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:55:01.600428 tensorset-0.4.2/tensorset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-17 22:55:01.000000 tensorset-0.4.2/tensorset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-17 22:55:01.000000 tensorset-0.4.2/tensorset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:55:01.000000 tensorset-0.4.2/tensorset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 22:55:01.000000 tensorset-0.4.2/tensorset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 22:55:01.000000 tensorset-0.4.2/tensorset.egg-info/top_level.txt
```

### Comparing `tensorset-0.4.1/PKG-INFO` & `tensorset-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorset
-Version: 0.4.1
+Version: 0.4.2
 Summary: manipulate sets of tensors
 Home-page: https://github.com/theAdamColton/tensorset
 Author: Adam Colton
 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.0.1
 
 # tensorset
```

### Comparing `tensorset-0.4.1/README.md` & `tensorset-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `tensorset-0.4.1/tensorset/tensorset.py` & `tensorset-0.4.2/tensorset/tensorset.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,16 +94,15 @@
                 size = "irregular"
             s += size
             if i < ndim - 1:
                 s += ", "
         s += "])"
         return s
 
-    else:
-        return str(col.shape)
+    return str(col.shape)
 
 
 class TensorSet:
     """
     A simple container of tensors in columns and named_columns
     """
 
@@ -181,14 +180,35 @@
         Assign to a new or existing column of this tensorset
         """
         if isinstance(key, int):
             self.columns[key] = item
         elif isinstance(key, str):
             self.named_columns[key] = item
 
+    def __delitem__(self, key: Union[str, int]):
+        """
+        deletes item based on column
+        """
+        if isinstance(key, int):
+            self.columns = self.columns.drop(key)
+        elif isinstance(key, str):
+            self.columns = self.columns.drop(key)
+
+    def __iter__(self):
+        """
+        returns an iterator
+        """
+        return iter(self.all_columns)
+
+    def __len__(self):
+        """
+        return number of columns
+        """
+        return len(self.all_columns)
+
     def to_device(self, device, **kwargs):
         """
         in-place
         """
         self.columns = [c.to(device, **kwargs) for c in self.columns]
         self.named_columns = {
             k: c.to(device, **kwargs) for k, c in self.named_columns.items()
```

### Comparing `tensorset-0.4.1/tensorset/tests/test_tensorset.py` & `tensorset-0.4.2/tensorset/tests/test_tensorset.py`

 * *Files 13% similar despite different names*

```diff
@@ -190,7 +190,57 @@
         )
         seq2 = ts.TensorSet(torch.empty(10, 13, 100), torch.empty(10, 13, 20))
         catted = ts.cat((seq1, seq2), -1)
         self.assertEqual(10, catted.size(0))
         self.assertEqual(13, catted.size(1))
         self.assertEqual(132, catted[0].size(-1))
         self.assertEqual(36, catted[1].size(-1))
+
+    def test_set_item(self):
+        seq = ts.TensorSet()
+        seq["asdf"] = torch.empty(1, 1, 1)
+        self.assertEqual(1, seq.num_columns)
+        seq2 = ts.TensorSet(torch.empty(10, 10))
+
+        seq2[0] = torch.zeros(1, 1, 1)
+        self.assertEqual(seq2[0].shape, torch.zeros(1, 1, 1).shape)
+
+    def test_iter(self):
+
+        seq = ts.TensorSet(
+            torch.empty(1, 1, 1),
+            torch.empty(
+                1,
+                1,
+            ),
+            torch.empty(
+                1,
+            ),
+        )
+        iterator = iter(seq)
+        self.assertEqual(torch.empty(1, 1, 1).shape, next(iterator).shape)
+        self.assertEqual(
+            torch.empty(
+                1,
+                1,
+            ).shape,
+            next(iterator).shape,
+        )
+        self.assertEqual(
+            torch.empty(
+                1,
+            ).shape,
+            next(iterator).shape,
+        )
+
+    def test_len(self):
+        seq = ts.TensorSet(
+            torch.empty(1, 1, 1),
+            torch.empty(
+                1,
+                1,
+            ),
+            torch.empty(
+                1,
+            ),
+        )
+        self.assertEqual(len(seq), 3)
```

### Comparing `tensorset-0.4.1/tensorset.egg-info/PKG-INFO` & `tensorset-0.4.2/tensorset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorset
-Version: 0.4.1
+Version: 0.4.2
 Summary: manipulate sets of tensors
 Home-page: https://github.com/theAdamColton/tensorset
 Author: Adam Colton
 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.0.1
 
 # tensorset
```

