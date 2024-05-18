# Comparing `tmp/debloat-1.5.5.tar.gz` & `tmp/debloat-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debloat-1.5.5.tar", last modified: Tue Apr  9 14:19:31 2024, max compression
+gzip compressed data, was "debloat-1.5.6.tar", last modified: Sat May 18 14:00:12 2024, max compression
```

## Comparing `debloat-1.5.5.tar` & `debloat-1.5.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 14:19:31.733606 debloat-1.5.5/
--rw-rw-rw-   0        0        0     1525 2023-03-27 10:23:04.000000 debloat-1.5.5/LICENSE
--rw-rw-rw-   0        0        0     8476 2024-04-09 14:19:31.733106 debloat-1.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     7856 2024-02-14 16:37:20.000000 debloat-1.5.5/README.md
--rw-rw-rw-   0        0        0      790 2024-04-09 14:16:17.000000 debloat-1.5.5/pyproject.toml
--rw-rw-rw-   0        0        0      166 2024-04-09 14:19:31.739607 debloat-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-03-27 10:34:30.000000 debloat-1.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:19:31.639180 debloat-1.5.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 14:19:31.684098 debloat-1.5.5/src/debloat/
--rw-rw-rw-   0        0        0        0 2023-07-11 19:08:33.000000 debloat-1.5.5/src/debloat/__init__.py
--rw-rw-rw-   0        0        0      495 2023-07-11 19:08:33.000000 debloat-1.5.5/src/debloat/auxiliary.py
--rw-rw-rw-   0        0        0     4355 2024-04-09 14:16:17.000000 debloat-1.5.5/src/debloat/gui.py
--rw-rw-rw-   0        0        0     2169 2024-04-09 14:16:17.000000 debloat-1.5.5/src/debloat/main.py
--rw-rw-rw-   0        0        0     2912 2024-03-18 00:27:19.000000 debloat-1.5.5/src/debloat/performanceTest.py
--rw-rw-rw-   0        0        0    26816 2024-04-09 14:16:17.000000 debloat-1.5.5/src/debloat/processor.py
--rw-rw-rw-   0        0        0     1486 2023-08-18 12:49:16.000000 debloat-1.5.5/src/debloat/processor.pyi
-drwxrwxrwx   0        0        0        0 2024-04-09 14:19:31.722104 debloat-1.5.5/src/debloat/tests/
--rw-rw-rw-   0        0        0        0 2023-07-11 19:08:33.000000 debloat-1.5.5/src/debloat/tests/__init__.py
--rw-rw-rw-   0        0        0      561 2023-07-11 19:08:33.000000 debloat-1.5.5/src/debloat/tests/debloat_test.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:19:31.730105 debloat-1.5.5/src/debloat/utilities/
--rw-rw-rw-   0        0        0        0 2023-07-11 19:08:33.000000 debloat-1.5.5/src/debloat/utilities/__init__.py
--rw-rw-rw-   0        0        0    51764 2024-02-21 18:11:20.000000 debloat-1.5.5/src/debloat/utilities/nsisParser.py
--rw-rw-rw-   0        0        0    23201 2024-02-21 18:11:20.000000 debloat-1.5.5/src/debloat/utilities/pyflate.py
--rw-rw-rw-   0        0        0    21202 2023-08-28 21:25:25.000000 debloat-1.5.5/src/debloat/utilities/readers.py
--rw-rw-rw-   0        0        0      746 2023-07-11 19:08:33.000000 debloat-1.5.5/src/debloat/utilities/rsrc.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:19:31.732106 debloat-1.5.5/src/debloat.egg-info/
--rw-rw-rw-   0        0        0     8476 2024-04-09 14:19:31.000000 debloat-1.5.5/src/debloat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      663 2024-04-09 14:19:31.000000 debloat-1.5.5/src/debloat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 14:19:31.000000 debloat-1.5.5/src/debloat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2024-04-09 14:19:31.000000 debloat-1.5.5/src/debloat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-04-09 14:19:31.000000 debloat-1.5.5/src/debloat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-09 14:19:31.000000 debloat-1.5.5/src/debloat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 14:00:12.555950 debloat-1.5.6/
+-rw-rw-rw-   0        0        0     1525 2023-03-27 10:23:04.000000 debloat-1.5.6/LICENSE
+-rw-rw-rw-   0        0        0     8708 2024-05-18 14:00:12.555451 debloat-1.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     8088 2024-05-18 13:59:44.000000 debloat-1.5.6/README.md
+-rw-rw-rw-   0        0        0      790 2024-05-18 13:59:45.000000 debloat-1.5.6/pyproject.toml
+-rw-rw-rw-   0        0        0      166 2024-05-18 14:00:12.557985 debloat-1.5.6/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-03-27 10:34:30.000000 debloat-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:00:12.408424 debloat-1.5.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-18 14:00:12.477436 debloat-1.5.6/src/debloat/
+-rw-rw-rw-   0        0        0        0 2023-07-11 19:08:33.000000 debloat-1.5.6/src/debloat/__init__.py
+-rw-rw-rw-   0        0        0      495 2023-07-11 19:08:33.000000 debloat-1.5.6/src/debloat/auxiliary.py
+-rw-rw-rw-   0        0        0     4745 2024-05-18 13:57:59.000000 debloat-1.5.6/src/debloat/gui.py
+-rw-rw-rw-   0        0        0     2595 2024-05-18 13:57:59.000000 debloat-1.5.6/src/debloat/main.py
+-rw-rw-rw-   0        0        0     2936 2024-05-18 13:59:45.000000 debloat-1.5.6/src/debloat/performanceTest.py
+-rw-rw-rw-   0        0        0    27497 2024-05-18 13:59:45.000000 debloat-1.5.6/src/debloat/processor.py
+-rw-rw-rw-   0        0        0     1486 2023-08-18 12:49:16.000000 debloat-1.5.6/src/debloat/processor.pyi
+drwxrwxrwx   0        0        0        0 2024-05-18 14:00:12.515443 debloat-1.5.6/src/debloat/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-11 19:08:33.000000 debloat-1.5.6/src/debloat/tests/__init__.py
+-rw-rw-rw-   0        0        0      561 2023-07-11 19:08:33.000000 debloat-1.5.6/src/debloat/tests/debloat_test.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:00:12.551949 debloat-1.5.6/src/debloat/utilities/
+-rw-rw-rw-   0        0        0        0 2023-07-11 19:08:33.000000 debloat-1.5.6/src/debloat/utilities/__init__.py
+-rw-rw-rw-   0        0        0    51764 2024-02-21 18:11:20.000000 debloat-1.5.6/src/debloat/utilities/nsisParser.py
+-rw-rw-rw-   0        0        0    23201 2024-02-21 18:11:20.000000 debloat-1.5.6/src/debloat/utilities/pyflate.py
+-rw-rw-rw-   0        0        0    21202 2023-08-28 21:25:25.000000 debloat-1.5.6/src/debloat/utilities/readers.py
+-rw-rw-rw-   0        0        0      746 2023-07-11 19:08:33.000000 debloat-1.5.6/src/debloat/utilities/rsrc.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:00:12.553951 debloat-1.5.6/src/debloat.egg-info/
+-rw-rw-rw-   0        0        0     8708 2024-05-18 14:00:12.000000 debloat-1.5.6/src/debloat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      663 2024-05-18 14:00:12.000000 debloat-1.5.6/src/debloat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 14:00:12.000000 debloat-1.5.6/src/debloat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2024-05-18 14:00:12.000000 debloat-1.5.6/src/debloat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2024-05-18 14:00:12.000000 debloat-1.5.6/src/debloat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-18 14:00:12.000000 debloat-1.5.6/src/debloat.egg-info/top_level.txt
```

### Comparing `debloat-1.5.5/LICENSE` & `debloat-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `debloat-1.5.5/PKG-INFO` & `debloat-1.5.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,17 @@
-Metadata-Version: 2.1
-Name: debloat
-Version: 1.5.5
-Summary: Debloat is an tool to remove excess garbage from bloated executables.
-Author-email: Squiblydoo <Squiblydoo@pm.me>
-Project-URL: Homepage, https://github.com/Squiblydoo/debloat
-Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: tkinterdnd2>=0.3.0
-Requires-Dist: pefile>=2023.2.0
-
 ![debloat](https://user-images.githubusercontent.com/77356206/215351855-9f89c298-36b4-4234-89b5-dc3f26d1f8b0.png)
 
 # Debloat
 Debloat is a GUI and CLI tool to remove excess garbage from bloated executables.
 
-By excess garbage, I mean 100 - 800 MB of junk bytes added to a binary to keep it from going into a sandbox.
+By excess garbage, I mean 100 - 800 MB of junk bytes added to a binary to keep it from going into a sandbox. This method of adding junk is called "inflating" or "pumping" a binary. Debloat currently handles the 10 most common inflation tactics.
+
+Being built with Python, the application can easily be leveraged in other workflows. Currently, debloat is used by [CCCS's AssemblyLine](https://www.cyber.gc.ca/en/tools-services/assemblyline) and [CERT Polska's MWDB](https://github.com/CERT-Polska/karton-archive-extractor).
 
-Being built with Python, the code and logic is easily accessible for others to take the concepts and apply them to their own tools. The program can be compiled for Windows, MacOS, Linux. The GUI removes any need for remembering commandline options and reading through CLI manuals: it is intended to be as simple as possible. The logic within the program handles the different use cases automatically.
+ The program can be compiled for Windows, MacOS, Linux. The GUI and CLI have minimal options: it is intended to be as simple as possible and the logic within the program handles the different use cases automatically.
 
 Compiled binaries have already been included in the [Releases](https://github.com/Squiblydoo/debloat/releases/).
 
 The debloat can installed using `pip install debloat`. Use `debloat` to launch the CLI and `debloat-gui` to launch the GUI.
 
 For advanced users, Debloat can also be imported into other scripts and the processing functions can be called individually.
 
@@ -43,15 +29,15 @@
 After installing using `pip install debloat` use the command `debloat`.<br>
 `debloat` can take two arguments. The first argument is required: the file to debloat. The second argument is optional: the output location. When no output is provided, it will be written to the same directory as the original file.
 
 The gui can also be launched from the CLI using the command `debloat-gui`.
 
 ## Does it always work?
 Not yet.
-My unscientific guess is that it should work for every 7 of 8 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
+My unscientific guess is that it should work for every 9 of 10 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
 
 In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "--last-ditch" switch. If you ever need this switch, consider sharing the sample for additional analysis. This option has now been added to the GUI. Functionally, what the function does is it will remove the whole overlay, if there is one. In some cases this is necessary as no pattern for the junk was found---this is most commonly the case in samples that do not compress well.
 
 ## Use Cases (Images from [Malcat](https://malcat.fr/))
 ### Full support
 - [x] Bloat appended to the end of a Signed PE.<br>
 In the image below, the bloat has been appended to the end of the executable. <br>
```

### Comparing `debloat-1.5.5/README.md` & `debloat-1.5.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,33 @@
+Metadata-Version: 2.1
+Name: debloat
+Version: 1.5.6
+Summary: Debloat is an tool to remove excess garbage from bloated executables.
+Author-email: Squiblydoo <Squiblydoo@pm.me>
+Project-URL: Homepage, https://github.com/Squiblydoo/debloat
+Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: tkinterdnd2>=0.3.0
+Requires-Dist: pefile>=2023.2.0
+
 ![debloat](https://user-images.githubusercontent.com/77356206/215351855-9f89c298-36b4-4234-89b5-dc3f26d1f8b0.png)
 
 # Debloat
 Debloat is a GUI and CLI tool to remove excess garbage from bloated executables.
 
-By excess garbage, I mean 100 - 800 MB of junk bytes added to a binary to keep it from going into a sandbox.
+By excess garbage, I mean 100 - 800 MB of junk bytes added to a binary to keep it from going into a sandbox. This method of adding junk is called "inflating" or "pumping" a binary. Debloat currently handles the 10 most common inflation tactics.
+
+Being built with Python, the application can easily be leveraged in other workflows. Currently, debloat is used by [CCCS's AssemblyLine](https://www.cyber.gc.ca/en/tools-services/assemblyline) and [CERT Polska's MWDB](https://github.com/CERT-Polska/karton-archive-extractor).
 
-Being built with Python, the code and logic is easily accessible for others to take the concepts and apply them to their own tools. The program can be compiled for Windows, MacOS, Linux. The GUI removes any need for remembering commandline options and reading through CLI manuals: it is intended to be as simple as possible. The logic within the program handles the different use cases automatically.
+ The program can be compiled for Windows, MacOS, Linux. The GUI and CLI have minimal options: it is intended to be as simple as possible and the logic within the program handles the different use cases automatically.
 
 Compiled binaries have already been included in the [Releases](https://github.com/Squiblydoo/debloat/releases/).
 
 The debloat can installed using `pip install debloat`. Use `debloat` to launch the CLI and `debloat-gui` to launch the GUI.
 
 For advanced users, Debloat can also be imported into other scripts and the processing functions can be called individually.
 
@@ -27,15 +45,15 @@
 After installing using `pip install debloat` use the command `debloat`.<br>
 `debloat` can take two arguments. The first argument is required: the file to debloat. The second argument is optional: the output location. When no output is provided, it will be written to the same directory as the original file.
 
 The gui can also be launched from the CLI using the command `debloat-gui`.
 
 ## Does it always work?
 Not yet.
-My unscientific guess is that it should work for every 7 of 8 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
+My unscientific guess is that it should work for every 9 of 10 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
 
 In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "--last-ditch" switch. If you ever need this switch, consider sharing the sample for additional analysis. This option has now been added to the GUI. Functionally, what the function does is it will remove the whole overlay, if there is one. In some cases this is necessary as no pattern for the junk was found---this is most commonly the case in samples that do not compress well.
 
 ## Use Cases (Images from [Malcat](https://malcat.fr/))
 ### Full support
 - [x] Bloat appended to the end of a Signed PE.<br>
 In the image below, the bloat has been appended to the end of the executable. <br>
```

### Comparing `debloat-1.5.5/pyproject.toml` & `debloat-1.5.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "debloat"
-version = "1.5.5"
+version = "1.5.6"
 authors = [
   { name="Squiblydoo", email="Squiblydoo@pm.me" },
 ]
 description = "Debloat is an tool to remove excess garbage from bloated executables."
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = [
```

### Comparing `debloat-1.5.5/src/debloat/gui.py` & `debloat-1.5.6/src/debloat/gui.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,20 @@
         # Safe processing value and checkbox: Maybe not even needed?
         self.unsafe_processing = BooleanVar(value=False)
         self.unsafe_checkbox = Checkbutton(self,
                                         text="Check to run last ditch effort processing",
                                          variable=self.unsafe_processing)
         self.unsafe_checkbox.pack()
 
+        self.cert_preservation = BooleanVar(value=False)
+        self.cert_checkbox = Checkbutton(self, 
+                                        text="Preserve Cert. Cert will be invalid but informational.",
+                                        variable=self.cert_preservation)
+        self.cert_checkbox.pack()
+
         
 
         # Define Scrollbox for output of program.
         self.output_scrollbox = st.ScrolledText(self, 
                                                 width=100, 
                                                 height=100,
                                                 wrap=WORD)
@@ -86,14 +92,15 @@
             return
         file_size = os.path.getsize(file_path)
         out_path = file_path.parent \
             / f"{file_path.stem}_patched{file_path.suffix}"
 
         result_code = debloat.processor.process_pe(pe,  out_path, 
                                      self.unsafe_processing.get(), 
+                                     self.cert_preservation.get(),
                    log_message=self.output_scrollbox_handler,
                    beginning_file_size=file_size)
         self.output_scrollbox_handler("Tactic identified: " , RESULT_CODES.get(result_code) +"\n")
         self.output_scrollbox_handler("-----Processing took %s seconds ---\n" \
                                     % round((time.time() - start_time), 2))
         self.clear_pathbox()
```

### Comparing `debloat-1.5.5/src/debloat/main.py` & `debloat-1.5.6/src/debloat/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,21 @@
                         required=False)
     parser.add_argument("-yolo", "--last-ditch", dest="last_ditch_processing",
                         help="""
     Run last-ditch processing. In this mode Debloat may remove the
     whole PE Overlay as a last resort if no smarter method works.
                             """,
                         action='store_true', default=False)
+    parser.add_argument("-c", "--cert", dest="cert_preservation", 
+                        help="""
+    Preserve the certificate on the end of the file if there is a certificate.
+    The certificate will no longer be valid.""",
+                        action='store_true',
+                        required=False,
+                        default=False)
     parser.add_argument("-v", "--version", action='version', version='debloat version ' + DEBLOAT_VERSION, help="Prints program version")
     args = parser.parse_args()
 
     file_path = args.executable
     out_path = args.output
     file_size = os.path.getsize(file_path)
 
@@ -45,14 +52,15 @@
 Maybe it needs unzipped?'''
               )
         return 1
 
     result_code = debloat.processor.process_pe(pe, 
                         out_path=str(out_path), 
                         last_ditch_processing=args.last_ditch_processing,
+                        cert_preservation=args.cert_preservation,
                         log_message=print,
                         beginning_file_size=file_size
                         )
     print("Tactic identifed:", RESULT_CODES.get(result_code))
     return 0
 
 if __name__ == "__main__":
```

### Comparing `debloat-1.5.5/src/debloat/performanceTest.py` & `debloat-1.5.6/src/debloat/performanceTest.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 argparser.add_argument("--directory", help="Specify sample directory", default="samples")
 argparser.add_argument("--keep", help="Keeps patched copies.", action="store_true")
 args = argparser.parse_args()
 
 def process_samples(sample, directory):
     file_size=os.path.getsize(args.directory +"/"+ sample)
     setup = f"import pefile; import debloat; filename = '{args.directory}/{sample}'; "
-    code = f"binary = pefile.PE(filename, fast_load=True); result= debloat.processor.process_pe(binary, filename + '.patched', last_ditch_processing=False, log_message=lambda *args, **kwargs: None, beginning_file_size={file_size}); print(result, end=' ')"
+    code = f"binary = pefile.PE(filename, fast_load=True); result= debloat.processor.process_pe(binary, filename + '.patched', last_ditch_processing=False, cert_preservation=True, log_message=lambda *args, **kwargs: None, beginning_file_size={file_size}); print(result, end=' ')"
 
     if args.mem:
         mem_profiler(setup, code, file_size, sample, directory)
     if args.cpu:
         cpu_profiler()
     if not args.keep:
         try:
```

### Comparing `debloat-1.5.5/src/debloat/processor.py` & `debloat-1.5.6/src/debloat/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,20 +119,22 @@
     last_section = None
     for section in pe.sections:
         if last_section is None \
                         or section.PointerToRawData > last_section.PointerToRawData:
             last_section = section
     return last_section
 
-def get_signature_info(pe: pefile.PE) -> Tuple[int, int]:
+def get_signature_info(pe: pefile.PE, cert_preservation) -> Tuple[int, int]:
     '''Remove PE signature and update header.'''
     signature_address = pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].VirtualAddress
     signature_size = pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].Size
     pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].VirtualAddress = 0
-    pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].Size = 0
+    # If the cert is to be preservered, we do not need to modify the size in the header. 
+    if cert_preservation == False:
+        pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].Size = 0
 
     return signature_address, signature_size
 
 
 def adjust_offsets(pe: pefile.PE, gap_offset: int, gap_size: int):
     base = pe.OPTIONAL_HEADER.ImageBase
     alignment = pe.OPTIONAL_HEADER.FileAlignment
@@ -391,14 +393,15 @@
             biggest_section_end = biggest_section.PointerToRawData + biggest_section.SizeOfRawData
             original_section_size = biggest_section.SizeOfRawData
             biggest_section_data = memoryview(pe.__data__)[biggest_section.PointerToRawData:biggest_section_end]
             delta_last_non_junk, result_code = trim_junk(pe, biggest_section_data, original_section_size)
             # Remove the junk from the section.
             if delta_last_non_junk > original_section_size:
                 log_message("Section was not able to be reduced.")
+                result_code = 0
                 return result
             data_to_delete.append((biggest_section.PointerToRawData + delta_last_non_junk, biggest_section_end))
             
             section_bytes_to_remove = original_section_size - delta_last_non_junk
             # Adjust all offsets for the file.
             adjust_offsets(pe, biggest_section.PointerToRawData, section_bytes_to_remove)
             log_message("Bloated section reduced.")
@@ -480,29 +483,36 @@
     not_aligned = alignment - (delta_last_non_junk % alignment)
     delta_last_non_junk = delta_last_non_junk + not_aligned
     if not result_code:
         result_code = 0
     return delta_last_non_junk, result_code
 
 def process_pe(pe: pefile.PE, out_path: str, last_ditch_processing: bool,
-               log_message: Callable[[str], None], beginning_file_size: int = 0) -> None:
+                cert_preservation: bool,log_message: Callable[[str], None], 
+                beginning_file_size: int = 0) -> None:
     '''Prepare PE, perform checks, remote junk, write patched binary.'''
     result_code = 0
     if not beginning_file_size:
         beginning_file_size = len(pe.write())
+
     # Remove Signature and modify size of Optional Header Security entry.
-    signature_address, signature_size = get_signature_info(pe)
-    data_to_delete = [(signature_address, signature_address + signature_size)]
+    signature_address, signature_size = get_signature_info(pe, cert_preservation)
+    if cert_preservation == True:
+        cert = [(signature_address, signature_address + signature_size)]
+        data_to_delete = []
+    else:
+        if signature_size > 0:
+            log_message("""A certificate is being removed from this file.\n-To preserve the certificate use the Cert Preservation option.""")
+        data_to_delete = [(signature_address, signature_address + signature_size)]
+
     signature_abnormality = handle_signature_abnormality(signature_address,
                                                         signature_size,
                                                         beginning_file_size)
     if signature_abnormality:
-        log_message('''
-    We detected data after the signature. This is abnormal. Removing signature and extra data...''')
-        data_to_delete.append((signature_address, beginning_file_size))
+        data_to_delete.append((signature_address + signature_size, beginning_file_size))
         result_code = 1  # Junk after signture
 
     # Handle Overlays: this includes packers and overlays which are completely junk
     elif pe.get_overlay_data_start_offset() and signature_size < len(pe.__data__) - pe.get_overlay_data_start_offset():
         possible_header = pe.__data__[pe.get_overlay_data_start_offset():pe.get_overlay_data_start_offset() + 30]
         # Check first to see if the file is NSIS
         nsis_extracted = check_and_extract_NSIS(possible_header, pe)
@@ -554,29 +564,31 @@
     else:
         # In order to solve some use cases, we will find the biggest section
         # within the binary.
         result, result_code = check_section_compression(pe, data_to_delete, log_message=log_message)
         log_message(result)
     # All processing is done. Report results.
     # There is always the signature in the list
-    if len(data_to_delete) == 1 or sum(slice_end-slice_start for slice_start, slice_end in data_to_delete) <= (beginning_file_size * 0.1):
+    if len(data_to_delete) == 0 or sum(slice_end-slice_start for slice_start, slice_end in data_to_delete) <= (beginning_file_size * 0.1):
         log_message("""No automated method for reducing the size worked. Please consider sharing the
 sample for additional analysis.
 Email: Squiblydoo@pm.me
 Twitter: @SquiblydooBlog.
                     """)
         result_code = 0
         return result_code
     else:
         pe_data = bytearray()
         start = 0
         for slice_start, slice_end in sorted(data_to_delete):
             pe_data += bytearray(pe.__data__[start:slice_start])
             start = slice_end
         pe_data += bytearray(pe.__data__[start:beginning_file_size])
+        if cert_preservation == True and signature_size > 0:
+            pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].VirtualAddress = len(pe_data) - signature_size
 
         pe.__data__ = pe_data
         final_filesize, new_pe_name = write_patched_file(out_path,
                                                          pe)
         reduction_calculation = round(((beginning_file_size \
                                         - final_filesize) \
                                         / beginning_file_size) * 100, 2)
```

### Comparing `debloat-1.5.5/src/debloat/processor.pyi` & `debloat-1.5.6/src/debloat/processor.pyi`

 * *Files identical despite different names*

### Comparing `debloat-1.5.5/src/debloat/tests/debloat_test.py` & `debloat-1.5.6/src/debloat/tests/debloat_test.py`

 * *Files identical despite different names*

### Comparing `debloat-1.5.5/src/debloat/utilities/nsisParser.py` & `debloat-1.5.6/src/debloat/utilities/nsisParser.py`

 * *Files identical despite different names*

### Comparing `debloat-1.5.5/src/debloat/utilities/pyflate.py` & `debloat-1.5.6/src/debloat/utilities/pyflate.py`

 * *Files identical despite different names*

### Comparing `debloat-1.5.5/src/debloat/utilities/readers.py` & `debloat-1.5.6/src/debloat/utilities/readers.py`

 * *Files identical despite different names*

### Comparing `debloat-1.5.5/src/debloat/utilities/rsrc.py` & `debloat-1.5.6/src/debloat/utilities/rsrc.py`

 * *Files identical despite different names*

### Comparing `debloat-1.5.5/src/debloat.egg-info/PKG-INFO` & `debloat-1.5.6/src/debloat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debloat
-Version: 1.5.5
+Version: 1.5.6
 Summary: Debloat is an tool to remove excess garbage from bloated executables.
 Author-email: Squiblydoo <Squiblydoo@pm.me>
 Project-URL: Homepage, https://github.com/Squiblydoo/debloat
 Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -15,17 +15,19 @@
 Requires-Dist: pefile>=2023.2.0
 
 ![debloat](https://user-images.githubusercontent.com/77356206/215351855-9f89c298-36b4-4234-89b5-dc3f26d1f8b0.png)
 
 # Debloat
 Debloat is a GUI and CLI tool to remove excess garbage from bloated executables.
 
-By excess garbage, I mean 100 - 800 MB of junk bytes added to a binary to keep it from going into a sandbox.
+By excess garbage, I mean 100 - 800 MB of junk bytes added to a binary to keep it from going into a sandbox. This method of adding junk is called "inflating" or "pumping" a binary. Debloat currently handles the 10 most common inflation tactics.
 
-Being built with Python, the code and logic is easily accessible for others to take the concepts and apply them to their own tools. The program can be compiled for Windows, MacOS, Linux. The GUI removes any need for remembering commandline options and reading through CLI manuals: it is intended to be as simple as possible. The logic within the program handles the different use cases automatically.
+Being built with Python, the application can easily be leveraged in other workflows. Currently, debloat is used by [CCCS's AssemblyLine](https://www.cyber.gc.ca/en/tools-services/assemblyline) and [CERT Polska's MWDB](https://github.com/CERT-Polska/karton-archive-extractor).
+
+ The program can be compiled for Windows, MacOS, Linux. The GUI and CLI have minimal options: it is intended to be as simple as possible and the logic within the program handles the different use cases automatically.
 
 Compiled binaries have already been included in the [Releases](https://github.com/Squiblydoo/debloat/releases/).
 
 The debloat can installed using `pip install debloat`. Use `debloat` to launch the CLI and `debloat-gui` to launch the GUI.
 
 For advanced users, Debloat can also be imported into other scripts and the processing functions can be called individually.
 
@@ -43,15 +45,15 @@
 After installing using `pip install debloat` use the command `debloat`.<br>
 `debloat` can take two arguments. The first argument is required: the file to debloat. The second argument is optional: the output location. When no output is provided, it will be written to the same directory as the original file.
 
 The gui can also be launched from the CLI using the command `debloat-gui`.
 
 ## Does it always work?
 Not yet.
-My unscientific guess is that it should work for every 7 of 8 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
+My unscientific guess is that it should work for every 9 of 10 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
 
 In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "--last-ditch" switch. If you ever need this switch, consider sharing the sample for additional analysis. This option has now been added to the GUI. Functionally, what the function does is it will remove the whole overlay, if there is one. In some cases this is necessary as no pattern for the junk was found---this is most commonly the case in samples that do not compress well.
 
 ## Use Cases (Images from [Malcat](https://malcat.fr/))
 ### Full support
 - [x] Bloat appended to the end of a Signed PE.<br>
 In the image below, the bloat has been appended to the end of the executable. <br>
```

### Comparing `debloat-1.5.5/src/debloat.egg-info/SOURCES.txt` & `debloat-1.5.6/src/debloat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

