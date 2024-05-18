# Comparing `tmp/sixtracktools-0.0.8.tar.gz` & `tmp/sixtracktools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sixtracktools-0.0.8.tar", last modified: Sun May  1 08:17:23 2022, max compression
+gzip compressed data, was "sixtracktools-0.0.9.tar", last modified: Wed Jun  8 20:05:05 2022, max compression
```

## Comparing `sixtracktools-0.0.8.tar` & `sixtracktools-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 giadarol  (1000) giadarol  (1000)        0 2022-05-01 08:17:23.548602 sixtracktools-0.0.8/
--rw-rw-r--   0 giadarol  (1000) giadarol  (1000)      256 2022-05-01 08:17:23.548602 sixtracktools-0.0.8/PKG-INFO
--rw-rw-r--   0 giadarol  (1000) giadarol  (1000)       38 2022-05-01 08:17:23.548602 sixtracktools-0.0.8/setup.cfg
--rw-rw-r--   0 giadarol  (1000) giadarol  (1000)      415 2022-05-01 08:16:56.000000 sixtracktools-0.0.8/setup.py
-drwxrwxr-x   0 giadarol  (1000) giadarol  (1000)        0 2022-05-01 08:17:23.548602 sixtracktools-0.0.8/sixtracktools/
--rw-rw-r--   0 giadarol  (1000) giadarol  (1000)      100 2022-03-31 10:46:40.000000 sixtracktools-0.0.8/sixtracktools/__init__.py
--rw-rw-r--   0 giadarol  (1000) giadarol  (1000)     4655 2022-03-31 10:46:40.000000 sixtracktools-0.0.8/sixtracktools/sixbin.py
--rw-rw-r--   0 giadarol  (1000) giadarol  (1000)     6710 2022-03-31 10:46:40.000000 sixtracktools-0.0.8/sixtracktools/sixdump.py
--rw-rw-r--   0 giadarol  (1000) giadarol  (1000)    55717 2022-05-01 08:16:41.000000 sixtracktools-0.0.8/sixtracktools/sixinput.py
--rw-rw-r--   0 giadarol  (1000) giadarol  (1000)   266592 2022-03-31 10:46:40.000000 sixtracktools-0.0.8/sixtracktools/sixtrack_slicing_table.py
--rw-rw-r--   0 giadarol  (1000) giadarol  (1000)     6118 2022-05-01 08:16:41.000000 sixtracktools-0.0.8/sixtracktools/xline_generation.py
-drwxrwxr-x   0 giadarol  (1000) giadarol  (1000)        0 2022-05-01 08:17:23.548602 sixtracktools-0.0.8/sixtracktools.egg-info/
--rw-rw-r--   0 giadarol  (1000) giadarol  (1000)      256 2022-05-01 08:17:23.000000 sixtracktools-0.0.8/sixtracktools.egg-info/PKG-INFO
--rw-rw-r--   0 giadarol  (1000) giadarol  (1000)      367 2022-05-01 08:17:23.000000 sixtracktools-0.0.8/sixtracktools.egg-info/SOURCES.txt
--rw-rw-r--   0 giadarol  (1000) giadarol  (1000)        1 2022-05-01 08:17:23.000000 sixtracktools-0.0.8/sixtracktools.egg-info/dependency_links.txt
--rw-rw-r--   0 giadarol  (1000) giadarol  (1000)        6 2022-05-01 08:17:23.000000 sixtracktools-0.0.8/sixtracktools.egg-info/requires.txt
--rw-rw-r--   0 giadarol  (1000) giadarol  (1000)       14 2022-05-01 08:17:23.000000 sixtracktools-0.0.8/sixtracktools.egg-info/top_level.txt
+drwxrwxr-x   0 giadarol  (1000) giadarol  (1000)        0 2022-06-08 20:05:05.516023 sixtracktools-0.0.9/
+-rw-rw-r--   0 giadarol  (1000) giadarol  (1000)      256 2022-06-08 20:05:05.516023 sixtracktools-0.0.9/PKG-INFO
+-rw-rw-r--   0 giadarol  (1000) giadarol  (1000)       38 2022-06-08 20:05:05.516023 sixtracktools-0.0.9/setup.cfg
+-rw-rw-r--   0 giadarol  (1000) giadarol  (1000)      415 2022-06-08 20:04:57.000000 sixtracktools-0.0.9/setup.py
+drwxrwxr-x   0 giadarol  (1000) giadarol  (1000)        0 2022-06-08 20:05:05.512023 sixtracktools-0.0.9/sixtracktools/
+-rw-rw-r--   0 giadarol  (1000) giadarol  (1000)      100 2022-03-31 10:46:40.000000 sixtracktools-0.0.9/sixtracktools/__init__.py
+-rw-rw-r--   0 giadarol  (1000) giadarol  (1000)     4655 2022-03-31 10:46:40.000000 sixtracktools-0.0.9/sixtracktools/sixbin.py
+-rw-rw-r--   0 giadarol  (1000) giadarol  (1000)     6758 2022-06-08 20:04:30.000000 sixtracktools-0.0.9/sixtracktools/sixdump.py
+-rw-rw-r--   0 giadarol  (1000) giadarol  (1000)    55764 2022-06-08 20:04:30.000000 sixtracktools-0.0.9/sixtracktools/sixinput.py
+-rw-rw-r--   0 giadarol  (1000) giadarol  (1000)   266592 2022-03-31 10:46:40.000000 sixtracktools-0.0.9/sixtracktools/sixtrack_slicing_table.py
+-rw-rw-r--   0 giadarol  (1000) giadarol  (1000)     6118 2022-05-01 08:16:41.000000 sixtracktools-0.0.9/sixtracktools/xline_generation.py
+drwxrwxr-x   0 giadarol  (1000) giadarol  (1000)        0 2022-06-08 20:05:05.512023 sixtracktools-0.0.9/sixtracktools.egg-info/
+-rw-rw-r--   0 giadarol  (1000) giadarol  (1000)      256 2022-06-08 20:05:05.000000 sixtracktools-0.0.9/sixtracktools.egg-info/PKG-INFO
+-rw-rw-r--   0 giadarol  (1000) giadarol  (1000)      367 2022-06-08 20:05:05.000000 sixtracktools-0.0.9/sixtracktools.egg-info/SOURCES.txt
+-rw-rw-r--   0 giadarol  (1000) giadarol  (1000)        1 2022-06-08 20:05:05.000000 sixtracktools-0.0.9/sixtracktools.egg-info/dependency_links.txt
+-rw-rw-r--   0 giadarol  (1000) giadarol  (1000)        6 2022-06-08 20:05:05.000000 sixtracktools-0.0.9/sixtracktools.egg-info/requires.txt
+-rw-rw-r--   0 giadarol  (1000) giadarol  (1000)       14 2022-06-08 20:05:05.000000 sixtracktools-0.0.9/sixtracktools.egg-info/top_level.txt
```

### Comparing `sixtracktools-0.0.8/sixtracktools/sixbin.py` & `sixtracktools-0.0.9/sixtracktools/sixbin.py`

 * *Files identical despite different names*

### Comparing `sixtracktools-0.0.8/sixtracktools/sixdump.py` & `sixtracktools-0.0.9/sixtracktools/sixdump.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         self.particles['deltaE'] *= 1e6
         self.mass0 = mass0
         self.energy0 = energy0
     px = property(lambda p: p.xp/p.rpp)
     py = property(lambda p: p.yp/p.rpp)
     ptau = property(lambda p: (p.energy-p.energy0)/p.p0c)
     psigma = property(lambda p: p.ptau/p.beta0)
-    tau = property(lambda p: p.sigma*p.beta0)
+    tau = property(lambda p: p.sigma/p.beta0)
     z = property(lambda p: p.beta/p.beta0*p.sigma)
     mass = property(lambda p: p.mass0)
     charge = property(lambda p: 1)
     charge0 = property(lambda p: 1)
     qratio = property(lambda p: p.charge/p.charge0)
     mratio = property(lambda p: p.mass/p.mass0)
     state = property(lambda p: 0)
@@ -132,29 +132,32 @@
     def __getitem__(self, idx):
         return SixDump101Abs(self.particles[idx].copy())
 
     px = property(lambda p: p.xp/p.rpp)
     py = property(lambda p: p.yp/p.rpp)
     ptau = property(lambda p: (p.energy-p.energy0)/p.p0c)
     psigma = property(lambda p: p.ptau/p.beta0)
-    tau = property(lambda p: p.sigma*p.beta0)
-    zeta = property(lambda p: p.sigma*p.rvv)
+    tau = property(lambda p: p.sigma/p.beta0)
     mass = property(lambda p: p.mass0)
     charge = property(lambda p: 1)
     charge0 = property(lambda p: 1)
     qratio = property(lambda p: p.charge/p.charge0)
     mratio = property(lambda p: p.mass/p.mass0)
     state = property(lambda p: 0)
     chi = property(lambda p: p.qratio/p.mratio)
     gamma0 = property(lambda p: p.energy0/p.mass0)
     beta0 = property(lambda p: p.p0c/p.energy0)
     gamma = property(lambda p: p.energy/p.mass)
     beta = property(lambda p: p.pc/p.energy)
     mass0 = property(lambda p: np.sqrt(p.energy0**2-p.p0c**2))
 
+    @property
+    def zeta(self):
+        raise ValueError('Not anymore supported, use tau')
+
     def __getattr__(self, k):
         return self.particles[k]
 
     def __dir__(self):
         return sorted(list(self.__dict__.keys()) +
                       list(self.particles.dtype.names))
 
@@ -168,15 +171,15 @@
         for name in names:
             out[name] = getattr(self, name)
         return out
 
     def get_minimal_beam(self):
         out = {}
         names = 'partid elemid turn state'.split()
-        names += 's x px y py zeta delta'.split()
+        names += 's x px y py tau delta'.split()
         names += 'mass0 p0c'.split()
         for name in names:
             out[name] = getattr(self, name)
         return out
 
 
 class SixDump101(SixDump101Abs):
```

### Comparing `sixtracktools-0.0.8/sixtracktools/sixinput.py` & `sixtracktools-0.0.9/sixtracktools/sixinput.py`

 * *Files 0% similar despite different names*

```diff
@@ -588,15 +588,16 @@
                 currline = next(f3)
                 if not currline.startswith("NEXT"):
                     linesplit = currline.split()
                     self.diff_nord = int(linesplit[0])
                     self.diff_nvar = int(linesplit[1])
                     self.diff_preda = myfloat(linesplit[2])
                     self.diff_nsix = int(linesplit[3])
-                    self.diff_ncor = int(linesplit[4])
+                    if len(linesplit) > 4:
+                        self.diff_ncor = int(linesplit[4])
                     currline = next(f3)
                 if not currline.startswith("NEXT"):
                     if self.diff_ncor != len(currline.split()):
                         # temporary error handling, does not abort execution
                         print("ERROR: Mismatch between #items in row 2 and ncor")
                     self.diff_name = currline.split()
```

### Comparing `sixtracktools-0.0.8/sixtracktools/sixtrack_slicing_table.py` & `sixtracktools-0.0.9/sixtracktools/sixtrack_slicing_table.py`

 * *Files identical despite different names*

### Comparing `sixtracktools-0.0.8/sixtracktools/xline_generation.py` & `sixtracktools-0.0.9/sixtracktools/xline_generation.py`

 * *Files identical despite different names*

