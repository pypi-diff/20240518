# Comparing `tmp/spectrum_image-0.3.1.tar.gz` & `tmp/spectrum_image-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_image-0.3.1.tar", last modified: Mon Apr 22 22:30:48 2024, max compression
+gzip compressed data, was "spectrum_image-0.3.2.tar", last modified: Sat May 18 00:49:05 2024, max compression
```

## Comparing `spectrum_image-0.3.1.tar` & `spectrum_image-0.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-22 22:30:48.818126 spectrum_image-0.3.1/
--rw-r--r--   0 sung       (501) staff       (20)    35149 2024-03-12 18:53:01.000000 spectrum_image-0.3.1/LICENSE
--rw-r--r--   0 sung       (501) staff       (20)     1800 2024-04-22 22:30:48.817921 spectrum_image-0.3.1/PKG-INFO
--rw-r--r--   0 sung       (501) staff       (20)      922 2024-04-10 01:05:24.000000 spectrum_image-0.3.1/README.md
--rw-r--r--   0 sung       (501) staff       (20)      981 2024-04-22 22:30:33.000000 spectrum_image-0.3.1/pyproject.toml
--rw-r--r--   0 sung       (501) staff       (20)       38 2024-04-22 22:30:48.818173 spectrum_image-0.3.1/setup.cfg
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-22 22:30:48.814235 spectrum_image-0.3.1/src/
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-22 22:30:48.815486 spectrum_image-0.3.1/src/spectrum_image/
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-22 22:30:48.817267 spectrum_image-0.3.1/src/spectrum_image/EELS/
--rw-r--r--   0 sung       (501) staff       (20)    24186 2024-04-22 03:59:53.000000 spectrum_image-0.3.1/src/spectrum_image/EELS/EELS_LP.py
--rw-r--r--   0 sung       (501) staff       (20)    23464 2024-04-22 04:04:52.000000 spectrum_image-0.3.1/src/spectrum_image/EELS/EELS_SI.py
--rw-r--r--   0 sung       (501) staff       (20)    13359 2024-04-22 03:35:02.000000 spectrum_image-0.3.1/src/spectrum_image/EELS/EELS_bgsub.py
--rw-r--r--   0 sung       (501) staff       (20)      764 2024-04-22 02:26:56.000000 spectrum_image-0.3.1/src/spectrum_image/EELS/EELS_edge.py
--rw-r--r--   0 sung       (501) staff       (20)     1466 2024-03-26 23:43:32.000000 spectrum_image-0.3.1/src/spectrum_image/EELS/EELS_lineshapes.py
--rw-r--r--   0 sung       (501) staff       (20)    12303 2024-04-22 02:15:06.000000 spectrum_image-0.3.1/src/spectrum_image/EELS/EELS_util.py
--rw-r--r--   0 sung       (501) staff       (20)      582 2024-04-22 04:00:49.000000 spectrum_image-0.3.1/src/spectrum_image/EELS/__init__.py
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-22 22:30:48.817514 spectrum_image-0.3.1/src/spectrum_image/RIXS/
--rw-r--r--   0 sung       (501) staff       (20)    11970 2024-04-22 22:14:47.000000 spectrum_image-0.3.1/src/spectrum_image/RIXS/RIXS_EM.py
--rw-r--r--   0 sung       (501) staff       (20)      643 2024-04-22 04:42:02.000000 spectrum_image-0.3.1/src/spectrum_image/RIXS/__init__.py
--rw-r--r--   0 sung       (501) staff       (20)      280 2024-03-12 18:53:01.000000 spectrum_image-0.3.1/src/spectrum_image/__init__.py
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-22 22:30:48.817671 spectrum_image-0.3.1/src/spectrum_image.egg-info/
--rw-r--r--   0 sung       (501) staff       (20)     1800 2024-04-22 22:30:48.000000 spectrum_image-0.3.1/src/spectrum_image.egg-info/PKG-INFO
--rw-r--r--   0 sung       (501) staff       (20)      604 2024-04-22 22:30:48.000000 spectrum_image-0.3.1/src/spectrum_image.egg-info/SOURCES.txt
--rw-r--r--   0 sung       (501) staff       (20)        1 2024-04-22 22:30:48.000000 spectrum_image-0.3.1/src/spectrum_image.egg-info/dependency_links.txt
--rw-r--r--   0 sung       (501) staff       (20)       52 2024-04-22 22:30:48.000000 spectrum_image-0.3.1/src/spectrum_image.egg-info/requires.txt
--rw-r--r--   0 sung       (501) staff       (20)       15 2024-04-22 22:30:48.000000 spectrum_image-0.3.1/src/spectrum_image.egg-info/top_level.txt
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-05-18 00:49:05.474372 spectrum_image-0.3.2/
+-rw-r--r--   0 sung       (501) staff       (20)    35149 2024-03-12 18:53:01.000000 spectrum_image-0.3.2/LICENSE
+-rw-r--r--   0 sung       (501) staff       (20)     1800 2024-05-18 00:49:05.474198 spectrum_image-0.3.2/PKG-INFO
+-rw-r--r--   0 sung       (501) staff       (20)      922 2024-04-10 01:05:24.000000 spectrum_image-0.3.2/README.md
+-rw-r--r--   0 sung       (501) staff       (20)      981 2024-05-18 00:49:02.000000 spectrum_image-0.3.2/pyproject.toml
+-rw-r--r--   0 sung       (501) staff       (20)       38 2024-05-18 00:49:05.474410 spectrum_image-0.3.2/setup.cfg
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-05-18 00:49:05.471704 spectrum_image-0.3.2/src/
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-05-18 00:49:05.472265 spectrum_image-0.3.2/src/spectrum_image/
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-05-18 00:49:05.473650 spectrum_image-0.3.2/src/spectrum_image/EELS/
+-rw-r--r--   0 sung       (501) staff       (20)    24186 2024-04-22 03:59:53.000000 spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_LP.py
+-rw-r--r--   0 sung       (501) staff       (20)    23464 2024-04-22 04:04:52.000000 spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_SI.py
+-rw-r--r--   0 sung       (501) staff       (20)    13359 2024-04-22 03:35:02.000000 spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_bgsub.py
+-rw-r--r--   0 sung       (501) staff       (20)      764 2024-04-22 02:26:56.000000 spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_edge.py
+-rw-r--r--   0 sung       (501) staff       (20)     1466 2024-03-26 23:43:32.000000 spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_lineshapes.py
+-rw-r--r--   0 sung       (501) staff       (20)    12303 2024-04-22 02:15:06.000000 spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_util.py
+-rw-r--r--   0 sung       (501) staff       (20)      582 2024-04-22 04:00:49.000000 spectrum_image-0.3.2/src/spectrum_image/EELS/__init__.py
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-05-18 00:49:05.473876 spectrum_image-0.3.2/src/spectrum_image/RIXS/
+-rw-r--r--   0 sung       (501) staff       (20)    12352 2024-05-17 20:50:10.000000 spectrum_image-0.3.2/src/spectrum_image/RIXS/RIXS_EM.py
+-rw-r--r--   0 sung       (501) staff       (20)      643 2024-04-22 04:42:02.000000 spectrum_image-0.3.2/src/spectrum_image/RIXS/__init__.py
+-rw-r--r--   0 sung       (501) staff       (20)      280 2024-03-12 18:53:01.000000 spectrum_image-0.3.2/src/spectrum_image/__init__.py
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-05-18 00:49:05.474017 spectrum_image-0.3.2/src/spectrum_image.egg-info/
+-rw-r--r--   0 sung       (501) staff       (20)     1800 2024-05-18 00:49:05.000000 spectrum_image-0.3.2/src/spectrum_image.egg-info/PKG-INFO
+-rw-r--r--   0 sung       (501) staff       (20)      604 2024-05-18 00:49:05.000000 spectrum_image-0.3.2/src/spectrum_image.egg-info/SOURCES.txt
+-rw-r--r--   0 sung       (501) staff       (20)        1 2024-05-18 00:49:05.000000 spectrum_image-0.3.2/src/spectrum_image.egg-info/dependency_links.txt
+-rw-r--r--   0 sung       (501) staff       (20)       52 2024-05-18 00:49:05.000000 spectrum_image-0.3.2/src/spectrum_image.egg-info/requires.txt
+-rw-r--r--   0 sung       (501) staff       (20)       15 2024-05-18 00:49:05.000000 spectrum_image-0.3.2/src/spectrum_image.egg-info/top_level.txt
```

### Comparing `spectrum_image-0.3.1/LICENSE` & `spectrum_image-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.3.1/PKG-INFO` & `spectrum_image-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum_image
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python Package for EELS (Electron Energy Loss Spectroscopy) Analysis
 Author-email: Suk Hyun Sung <sukhsung@umich.edu>, Michale Colletta <mrc297@cornell.edu>, Alex Stangle <astangel@umich.edu>
 Project-URL: Homepage, https://github.com/sukhsung/spectrum-image
 Project-URL: Repository, https://github.com/sukhsung/spectrum-image
 Project-URL: Bug Tracker, https://github.com/sukhsung/spectrum-image/issues
 Keywords: Electron Microscopy,EELS,TEM,STEM,Electron Energy Loss Spectroscopy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spectrum_image-0.3.1/README.md` & `spectrum_image-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.3.1/pyproject.toml` & `spectrum_image-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spectrum_image"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
   "numpy",
   "matplotlib",
   "jupyterlab",
   "ipympl",
   "scipy",
   "tqdm",
```

### Comparing `spectrum_image-0.3.1/src/spectrum_image/EELS/EELS_LP.py` & `spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_LP.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.3.1/src/spectrum_image/EELS/EELS_SI.py` & `spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_SI.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.3.1/src/spectrum_image/EELS/EELS_bgsub.py` & `spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_bgsub.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.3.1/src/spectrum_image/EELS/EELS_edge.py` & `spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_edge.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.3.1/src/spectrum_image/EELS/EELS_lineshapes.py` & `spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_lineshapes.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.3.1/src/spectrum_image/EELS/EELS_util.py` & `spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_util.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.3.1/src/spectrum_image/EELS/__init__.py` & `spectrum_image-0.3.2/src/spectrum_image/EELS/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.3.1/src/spectrum_image/RIXS/RIXS_EM.py` & `spectrum_image-0.3.2/src/spectrum_image/RIXS/RIXS_EM.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,15 +16,24 @@
             eloss = np.arange( self.neloss )
         if einc is None:
             einc = np.arange( self.neinc )
 
         self.eloss = eloss
         self.einc = einc
 
-    def browser( self, cmap='gray', figsize=(6,8)):
+        ind_eloss = np.argsort( self.eloss )
+        ind_einc  = np.argsort( self.einc )
+
+        self.eloss = self.eloss[ind_eloss]
+        self.einc = self.einc[ind_einc]
+
+        self.si = self.si[ind_eloss,:]
+        self.si = self.si[:,ind_einc]
+
+    def browser( self, cmap='gray', figsize=(6,8), vmin=None, vmax=None):
         
         self.int_dir = 0
         self.eaxis  = [self.einc, self.eloss]
         self.elabel = ["Incident Energy (eV)", "Energy Loss (eV)"]
         ## Initialize browser object
         self.spec1 = np.mean(self.si,axis=self.int_dir)
         self.spec2 = np.mean(self.si,axis=self.int_dir)
@@ -40,25 +49,28 @@
         self.ax['spec']=self.fig.add_axes([0.1,0.05,0.8,0.4]) # Spectrum
         self.ax['ck_ysetting'] = self.fig.add_axes([0.7,0.45,0.3,0.07]) # Y-lock chkbox
         self.ax['ck_roisetting'] = self.fig.add_axes([0.7,0.94,0.3,0.07]) # ROI2 chkbox
 
         ## Initialize plot handles
         self.h = {}
         ################## ax['inel'] ######################
-        self.h['inel'] = self.ax['inel'].pcolormesh( self.einc, self.eloss, self.im_inel,cmap = cmap)
+        self.h['inel'] = self.ax['inel'].pcolormesh( self.einc, self.eloss, self.im_inel,cmap = cmap, vmin=vmin, vmax=vmax)
         self.ax['inel'].set_axis_on()
         self.ax['inel'].set_title('RIXS Energy Map')
         self.ax['inel'].set_ylabel('Energy Loss (eV)')
         self.ax['inel'].set_xlabel('Incident Energy (eV)')
+        self.ax['inel'].set_xlim( (np.min(self.einc),np.max(self.einc)))
+        self.ax['inel'].set_ylim( (np.min(self.eloss),np.max(self.eloss)))
+        # self.ax['inel'].autoscale(enable=True, axis='xy', tight=True)
 
         ################## ax['spec'] ######################
         self.h['spec1'], = self.ax['spec'].plot(self.eaxis[self.int_dir], self.spec1,color='crimson')
         self.h['spec2'], = self.ax['spec'].plot(self.eaxis[self.int_dir], self.spec2,color='royalblue')
         self.h['spec2'].set_alpha(0)
-        self.ax['spec'].set_yticks([])
+        # self.ax['spec'].set_yticks([])
         self.ax['spec'].set_xlabel(self.elabel[self.int_dir])
         self.ax['spec'].set_ylabel('Intensity')
 
 
         ## Initialize ui handles
         self.ui={}
         ### Check box 
@@ -66,15 +78,15 @@
         self.ui['ck_ysetting'] = CheckButtons(ax=self.ax['ck_ysetting'], labels= ["Lock Y-axis","Log(y)"],
                                             actives=[False, False], check_props={'facecolor': 'k'} )
         self.ui['ck_ysetting'].on_clicked( lambda v: self.onclick_ck_ysetting() )
         self.y_locked = False
         self.y_log = False
 
 
-        self.ui['ck_roisetting'] = CheckButtons(ax=self.ax['ck_roisetting'], labels= ["Enable ROI 2", "Flip Integration"],
+        self.ui['ck_roisetting'] = CheckButtons(ax=self.ax['ck_roisetting'], labels= ["Enable ROI 2", "Integrate E-loss"],
                                         actives=[False, False], check_props={'facecolor': 'k'} )
         self.ui['ck_roisetting'].on_clicked( lambda v: self.onclick_ck_roisetting() )
         self.roi2_enabled = False
 
 
         ################### Selectors ###################
         self.ui['roi1'] = RectangleSelector(self.ax['inel'], self.dummy, button=[1],
@@ -113,92 +125,99 @@
             self.ui['roi2'].set_visible( True )
             self.ui['roi2'].set_active( True )
         else:
             self.h['spec2'].set_alpha(0)
             self.ui['roi2'].set_visible( False )
             self.ui['roi2'].set_active( False )
 
+
         # Check for integration flip
         if self.ui['ck_roisetting'].get_status()[1]:
             self.int_dir = 1
+            self.ui['ck_roisetting'].labels[1].set_text('Integrate E-inc')
         else:
             self.int_dir = 0
+            self.ui['ck_roisetting'].labels[1].set_text('Integrate E-loss')
 
         self.int_dir = int(self.ui['ck_roisetting'].get_status()[1])
         self.on_change_roi1()
         # self.on_change_roi2()
 
 
     def on_change_roi1(self):
         roi1 = self.ui['roi1'].extents
+        roi2 = self.ui['roi2'].extents
+        if self.int_dir == 0:
+            self.ui['roi2'].extents = (roi1[0],roi1[1],roi2[2],roi2[3])
+        else:
+            self.ui['roi2'].extents = (roi2[0],roi2[1],roi1[2],roi1[3])
+
+        eimin = np.searchsorted( self.einc,  float(roi1[0]))
+        eimax = np.searchsorted( self.einc,  float(roi1[1]))
+        elmin = np.searchsorted( self.eloss, float(roi1[2]))
+        elmax = np.searchsorted( self.eloss, float(roi1[3]))
 
-        eimin = np.searchsorted( self.einc,  int(roi1[0]))
-        eimax = np.searchsorted( self.einc,  int(roi1[1]))
-        elmin = np.searchsorted( self.eloss, int(roi1[2]))
-        elmax = np.searchsorted( self.eloss, int(roi1[3]))
         if eimin == eimax:
             eimax += 1
         if elmin == elmax:
             elmax += 1
 
+
         if self.int_dir == 0:
             self.spec1  = np.mean(self.si[elmin:elmax,:],axis=(0))
             eminmax = (self.einc[eimin], self.einc[eimax])
         else:
             self.spec1 = np.mean(self.si[:,eimin:eimax],axis=(1))
             eminmax = (self.eloss[elmin], self.eloss[elmax])
         
         self.ax['spec'].set_xlim( eminmax )
         self.h['spec1'].set_data( self.eaxis[self.int_dir], self.spec1)
 
-        # roi2 =self.ui['roi2'].extents
-        # if self.int_dir == 0:
-        #     self.ui['roi2'].extents = (eimin,eimax,roi2[2],roi2[3])
-        # else:
-        #     print((roi2[0],roi2[1], elmin,elmax))
-        #     self.ui['roi2'].extents = (roi2[0],roi2[1], elmin,elmax)
+
 
         self.rescale_yrange()
 
     def on_change_roi2(self):
+        roi1 = self.ui['roi1'].extents
         roi2 = self.ui['roi2'].extents
 
-        eimin = np.searchsorted( self.einc,  int(roi2[0]))
-        eimax = np.searchsorted( self.einc,  int(roi2[1]))
-        elmin = np.searchsorted( self.eloss, int(roi2[2]))
-        elmax = np.searchsorted( self.eloss, int(roi2[3]))
+        if self.int_dir == 0:
+            self.ui['roi2'].extents = (roi1[0],roi1[1],roi2[2],roi2[3])
+        else:
+            self.ui['roi2'].extents = (roi2[0],roi2[1],roi1[2],roi1[3])
+
+        eimin = np.searchsorted( self.einc,  float(roi2[0]))
+        eimax = np.searchsorted( self.einc,  float(roi2[1]))
+        elmin = np.searchsorted( self.eloss, float(roi2[2]))
+        elmax = np.searchsorted( self.eloss, float(roi2[3]))
         if eimin == eimax:
             eimax += 1
         if elmin == elmax:
             elmax += 1
 
         if self.int_dir == 0:
             self.spec2  = np.mean(self.si[elmin:elmax,:],axis=(0))
-            eminmax = (self.einc[eimin], self.einc[eimax])
         else:
             self.spec2 = np.mean(self.si[:,eimin:eimax],axis=(1))
-            eminmax = (self.eloss[elmin], self.eloss[elmax])
         
-        self.ax['spec'].set_xlim( eminmax )
+
         self.h['spec2'].set_data( self.eaxis[self.int_dir], self.spec2)
 
         self.rescale_yrange()
     
 
 
     def rescale_yrange(self):
 
         if self.y_log:
             self.ax['spec'].set_yscale('log')
             self.ax['spec'].set_ylabel('Log Intensity')
-            self.ax['spec'].set_yticks([])
         else:
             self.ax['spec'].set_yscale('linear')
             self.ax['spec'].set_ylabel('Intensity')
-            self.ax['spec'].set_yticks([])
 
         if self.y_locked == False:
 
             roi1 = self.ui['roi1'].extents
             eimin = np.searchsorted( self.einc,  int(roi1[0]))
             eimax = np.searchsorted( self.einc,  int(roi1[1]))
             elmin = np.searchsorted( self.eloss, int(roi1[2]))
@@ -207,51 +226,51 @@
                 eimax += 1
             if elmin == elmax:
                 elmax += 1
 
 
             if not self.y_log:
                 if self.int_dir == 1:
-                    print(self.spec1)
-                    maxval =  1.1*self.spec1[eimin:eimax].max()
-                    minval =  min( 0.9*self.spec1[eimin:eimax].min(),0)
+                    maxval =  1.02*self.spec1.max()
+                    minval =  0.98*self.spec1.min()
                 else:
-                    maxval =  1.1*self.spec1[elmin:elmax].max()
-                    minval =  min( 0.9*self.spec1[elmin:elmax].min(),0)
+                    maxval =  1.02*self.spec1.max()
+                    minval =  0.98*self.spec1.min()
 
             else:
                 if self.int_dir == 1:
-                    maxval =  1.2*self.spec1[eimin:eimax].max()
-                    minval =  0.8*self.spec1[eimin:eimax].min()
+                    maxval =  1.1*self.spec1.max()
+                    minval =  0.9*self.spec1.min()
                 else:
-                    maxval =  1.2*self.spec1[elmin:elmax].max()
-                    minval =  0.8*self.spec1[elmin:elmax].min()
+                    maxval =  1.1*self.spec1.max()
+                    minval =  0.9*self.spec1.min()
 
 
 
             if self.roi2_enabled:
                 if not self.y_log:
                     if self.int_dir == 1:
-                        maxval2 =  1.1*self.spec2[eimin:eimax].max()
-                        minval2 =  min( 0.9*self.spec2[eimin:eimax].min(),0)
+                        maxval2 =  1.02*self.spec2.max()
+                        minval2 =  0.98*self.spec2.min()
                     else:
-                        maxval2 =  1.1*self.spec2[elmin:elmax].max()
-                        minval2 =  min( 0.9*self.spec2[elmin:elmax].min(),0)
+                        maxval2 =  1.02*self.spec2.max()
+                        minval2 =  0.98*self.spec2.min()
 
                 else:
                     if self.int_dir == 1:
-                        maxval2 =  1.2*self.spec2[eimin:eimax].max()
-                        minval2 =  0.8*self.spec2[eimin:eimax].min()
+                        maxval2 =  1.1*self.spec2.max()
+                        minval2 =  0.9*self.spec2.min()
                     else:
-                        maxval2 =  1.2*self.spec2[elmin:elmax].max()
-                        minval2 =  0.8*self.spec2[elmin:elmax].min()
+                        maxval2 =  1.1*self.spec2.max()
+                        minval2 =  0.9*self.spec2.min()
 
                 minval = min( minval, minval2)
                 maxval = max( maxval, maxval2)
 
+            # print( minval, maxval )
 
             self.ax['spec'].set_ylim([minval,maxval])
 
 
     ############### Event Handlers ###################
     def onclick_figure( self, event ):
         if event.inaxes in [self.ax['inel']]:
```

### Comparing `spectrum_image-0.3.1/src/spectrum_image/RIXS/__init__.py` & `spectrum_image-0.3.2/src/spectrum_image/RIXS/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.3.1/src/spectrum_image.egg-info/PKG-INFO` & `spectrum_image-0.3.2/src/spectrum_image.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum_image
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python Package for EELS (Electron Energy Loss Spectroscopy) Analysis
 Author-email: Suk Hyun Sung <sukhsung@umich.edu>, Michale Colletta <mrc297@cornell.edu>, Alex Stangle <astangel@umich.edu>
 Project-URL: Homepage, https://github.com/sukhsung/spectrum-image
 Project-URL: Repository, https://github.com/sukhsung/spectrum-image
 Project-URL: Bug Tracker, https://github.com/sukhsung/spectrum-image/issues
 Keywords: Electron Microscopy,EELS,TEM,STEM,Electron Energy Loss Spectroscopy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spectrum_image-0.3.1/src/spectrum_image.egg-info/SOURCES.txt` & `spectrum_image-0.3.2/src/spectrum_image.egg-info/SOURCES.txt`

 * *Files identical despite different names*

