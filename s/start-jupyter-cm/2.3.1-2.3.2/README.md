# Comparing `tmp/start_jupyter_cm-2.3.1.tar.gz` & `tmp/start_jupyter_cm-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "start_jupyter_cm-2.3.1.tar", last modified: Wed Sep  1 09:41:37 2021, max compression
+gzip compressed data, was "start_jupyter_cm-2.3.2.tar", last modified: Sat May 18 11:22:59 2024, max compression
```

## Comparing `start_jupyter_cm-2.3.1.tar` & `start_jupyter_cm-2.3.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-01 09:41:37.437326 start_jupyter_cm-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1846 2021-09-01 09:41:01.000000 start_jupyter_cm-2.3.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2021-09-01 09:41:01.000000 start_jupyter_cm-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-09-01 09:41:01.000000 start_jupyter_cm-2.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8965 2021-09-01 09:41:37.437326 start_jupyter_cm-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6466 2021-09-01 09:41:01.000000 start_jupyter_cm-2.3.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-01 09:41:37.437326 start_jupyter_cm-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2577 2021-09-01 09:41:01.000000 start_jupyter_cm-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-01 09:41:37.437326 start_jupyter_cm-2.3.1/start_jupyter_cm/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-09-01 09:41:36.000000 start_jupyter_cm-2.3.1/start_jupyter_cm/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1249 2021-09-01 09:41:01.000000 start_jupyter_cm-2.3.1/start_jupyter_cm/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     2343 2021-09-01 09:41:01.000000 start_jupyter_cm-2.3.1/start_jupyter_cm/gnome.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-01 09:41:37.437326 start_jupyter_cm-2.3.1/start_jupyter_cm/icons/
--rw-r--r--   0 runner    (1001) docker     (121)    14447 2021-09-01 09:41:01.000000 start_jupyter_cm-2.3.1/start_jupyter_cm/icons/jupyter-qtconsole.ico
--rw-r--r--   0 runner    (1001) docker     (121)    14508 2021-09-01 09:41:01.000000 start_jupyter_cm-2.3.1/start_jupyter_cm/icons/jupyter-qtconsole.png
--rw-r--r--   0 runner    (1001) docker     (121)     6587 2021-09-01 09:41:01.000000 start_jupyter_cm-2.3.1/start_jupyter_cm/icons/jupyter.ico
--rw-r--r--   0 runner    (1001) docker     (121)     6751 2021-09-01 09:41:01.000000 start_jupyter_cm-2.3.1/start_jupyter_cm/icons/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (121)     6877 2021-09-01 09:41:01.000000 start_jupyter_cm-2.3.1/start_jupyter_cm/linux.py
--rw-r--r--   0 runner    (1001) docker     (121)     3398 2021-09-01 09:41:01.000000 start_jupyter_cm-2.3.1/start_jupyter_cm/macos.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-01 09:41:37.437326 start_jupyter_cm-2.3.1/start_jupyter_cm/prototype.workflow/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-01 09:41:37.437326 start_jupyter_cm-2.3.1/start_jupyter_cm/prototype.workflow/Contents/
--rw-r--r--   0 runner    (1001) docker     (121)      983 2021-09-01 09:41:01.000000 start_jupyter_cm-2.3.1/start_jupyter_cm/prototype.workflow/Contents/Info.plist
--rw-r--r--   0 runner    (1001) docker     (121)     8958 2021-09-01 09:41:01.000000 start_jupyter_cm-2.3.1/start_jupyter_cm/prototype.workflow/Contents/document.wflow
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-01 09:41:37.437326 start_jupyter_cm-2.3.1/start_jupyter_cm/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-01 09:41:01.000000 start_jupyter_cm-2.3.1/start_jupyter_cm/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3819 2021-09-01 09:41:01.000000 start_jupyter_cm-2.3.1/start_jupyter_cm/tests/test_command.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      382 2021-09-01 09:41:01.000000 start_jupyter_cm-2.3.1/start_jupyter_cm/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6993 2021-09-01 09:41:01.000000 start_jupyter_cm-2.3.1/start_jupyter_cm/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-01 09:41:37.437326 start_jupyter_cm-2.3.1/start_jupyter_cm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8965 2021-09-01 09:41:37.000000 start_jupyter_cm-2.3.1/start_jupyter_cm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      793 2021-09-01 09:41:37.000000 start_jupyter_cm-2.3.1/start_jupyter_cm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-01 09:41:37.000000 start_jupyter_cm-2.3.1/start_jupyter_cm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2021-09-01 09:41:37.000000 start_jupyter_cm-2.3.1/start_jupyter_cm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-09-01 09:41:37.000000 start_jupyter_cm-2.3.1/start_jupyter_cm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:22:59.414585 start_jupyter_cm-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-18 11:22:52.000000 start_jupyter_cm-2.3.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-18 11:22:52.000000 start_jupyter_cm-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-18 11:22:52.000000 start_jupyter_cm-2.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-05-18 11:22:59.414585 start_jupyter_cm-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-18 11:22:52.000000 start_jupyter_cm-2.3.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 11:22:59.414585 start_jupyter_cm-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-18 11:22:52.000000 start_jupyter_cm-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:22:59.410585 start_jupyter_cm-2.3.2/start_jupyter_cm/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-18 11:22:52.000000 start_jupyter_cm-2.3.2/start_jupyter_cm/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1249 2024-05-18 11:22:52.000000 start_jupyter_cm-2.3.2/start_jupyter_cm/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-18 11:22:52.000000 start_jupyter_cm-2.3.2/start_jupyter_cm/gnome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:22:59.414585 start_jupyter_cm-2.3.2/start_jupyter_cm/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)    14447 2024-05-18 11:22:52.000000 start_jupyter_cm-2.3.2/start_jupyter_cm/icons/jupyter-qtconsole.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    14508 2024-05-18 11:22:52.000000 start_jupyter_cm-2.3.2/start_jupyter_cm/icons/jupyter-qtconsole.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-18 11:22:52.000000 start_jupyter_cm-2.3.2/start_jupyter_cm/icons/jupyter.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-05-18 11:22:52.000000 start_jupyter_cm-2.3.2/start_jupyter_cm/icons/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-18 11:22:52.000000 start_jupyter_cm-2.3.2/start_jupyter_cm/linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-18 11:22:52.000000 start_jupyter_cm-2.3.2/start_jupyter_cm/macos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:22:59.410585 start_jupyter_cm-2.3.2/start_jupyter_cm/prototype.workflow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:22:59.414585 start_jupyter_cm-2.3.2/start_jupyter_cm/prototype.workflow/Contents/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-18 11:22:52.000000 start_jupyter_cm-2.3.2/start_jupyter_cm/prototype.workflow/Contents/Info.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     8958 2024-05-18 11:22:52.000000 start_jupyter_cm-2.3.2/start_jupyter_cm/prototype.workflow/Contents/document.wflow
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:22:59.414585 start_jupyter_cm-2.3.2/start_jupyter_cm/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 11:22:52.000000 start_jupyter_cm-2.3.2/start_jupyter_cm/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3819 2024-05-18 11:22:52.000000 start_jupyter_cm-2.3.2/start_jupyter_cm/tests/test_command.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      382 2024-05-18 11:22:52.000000 start_jupyter_cm-2.3.2/start_jupyter_cm/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6993 2024-05-18 11:22:52.000000 start_jupyter_cm-2.3.2/start_jupyter_cm/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:22:59.414585 start_jupyter_cm-2.3.2/start_jupyter_cm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-05-18 11:22:59.000000 start_jupyter_cm-2.3.2/start_jupyter_cm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-18 11:22:59.000000 start_jupyter_cm-2.3.2/start_jupyter_cm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 11:22:59.000000 start_jupyter_cm-2.3.2/start_jupyter_cm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-18 11:22:59.000000 start_jupyter_cm-2.3.2/start_jupyter_cm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-18 11:22:59.000000 start_jupyter_cm-2.3.2/start_jupyter_cm.egg-info/top_level.txt
```

### Comparing `start_jupyter_cm-2.3.1/LICENSE` & `start_jupyter_cm-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `start_jupyter_cm-2.3.1/PKG-INFO` & `start_jupyter_cm-2.3.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,214 +1,223 @@
 Metadata-Version: 2.1
 Name: start_jupyter_cm
-Version: 2.3.1
+Version: 2.3.2
 Summary: Add entries to start Jupyter from context menu.
 Home-page: https://github.com/hyperspy/start_jupyter_cm
 Author: The HyperSpy Developers
 License: BSDv3
-Description: start\_jupyter\_cm
-        ==================
-        
-        |pypi_version|_  |python_version|_ |conda-forge|_ |tests|_
-        
-        .. |pypi_version| image:: https://img.shields.io/pypi/v/start-jupyter-cm.svg?style=flat
-        .. _pypi_version: https://pypi.python.org/pypi/start-jupyter-cm
-        
-        .. |python_version| image:: https://img.shields.io/pypi/pyversions/start-jupyter-cm.svg?style=flat
-        .. _python_version: https://pypi.python.org/pypi/start-jupyter-cm
-        
-        .. |conda-forge| image:: https://img.shields.io/conda/pn/conda-forge/start_jupyter_cm?label=conda-forge
-        .. _conda-forge: https://anaconda.org/conda-forge/start_jupyter_cm
-        
-        .. |Tests| image:: https://github.com/hyperspy/start_jupyter_cm/actions/workflows/tests.yml/badge.svg
-        .. _tests: https://github.com/hyperspy/start_jupyter_cm/actions/workflows/tests.yml
-        
-        
-        Description
-        -----------
-        
-        Add entries to start the `Jupyter Notebook <https://jupyter-notebook.readthedocs.io>`__,
-        `Jupyter QtConsole <https://qtconsole.readthedocs.io>`__ or
-        `JupyterLab <https://jupyterlab.readthedocs.io>`__ from the file
-        manager context menu. This offers a convenient way of starting Jupyter
-        in a folder. Currently it only supports Microsoft Windows, GNOME (and
-        its many derivatives), and macOS. Contributions to support other OSs/desktop
-        environments are highly welcome.
-        
-        `WinPython <http://winpython.github.io>`__ and
-        `Anaconda <https://www.anaconda.com/distribution>`__/
-        `Miniconda <https://docs.conda.io/en/latest/miniconda.html>`__/
-        `Miniforge <https://github.com/conda-forge/miniforge>`__/
-        `Mambaforge <https://github.com/conda-forge/miniforge#mambaforge>`__
-        distributions are supported. If run from a conda environment other than `root`,
-        the name of the environment will be specified in brackets in the context menu name.
-        
-        Microsoft Windows
-        ~~~~~~~~~~~~~~~~~
-        
-        .. figure:: https://github.com/hyperspy/start_jupyter_cm/raw/main/images/jupyter_cm_windows.png
-           :alt: Jupyter context menu entries in windows
-           :width: 250px
-        
-           Jupyter context menu entries in windows.
-        
-        
-        In addition to starting the QtConsole, the Jupyter Notebook or the Jupyter Lab,
-        and launching the default browser, in Microsoft Windows the process runs from
-        a terminal. Closing the terminal closes the QtConsole or the Jupyter server.
-        Single and all users installations are supported, see installation instructions below.
-        
-        Linux
-        ~~~~~
-        
-        On linux, the supported file managers are: Nautilus (GNOME), Caja (MATE), Dolphin (KDE) and Nemo (Cinnamon).
-        With Nautilus and Caja, the shortcut will appear in the *Scripts* menu and with
-        Dolphin, it will appear in the *Actions* menu.
-        
-        .. figure:: https://github.com/hyperspy/start_jupyter_cm/raw/main/images/jupyter_cm_gnome.png
-           :alt: Jupyter context menu entries in Nautilus
-           :width: 450px
-        
-           Jupyter context menu entries on Linux (Nautilus).
-        
-        
-        When selecting multiple folders, one instance of Jupyter
-        QtConsole/notebook/lab opens in each of the selected folders. Selecting a
-        file starts Jupyter in the file directory.
-        
-        Note that on Linux the processes run in the background: to stop the jupyter
-        notebook or lab, don't forget to exit using the *quit* button - only closing
-        the tab will not stop the jupyter server. Alternatively, `nbmanager <https://github.com/takluyver/nbmanager>`__
-        can discover all running servers and shut them down using via an UI.
-        
-        
-        macOS
-        ~~~~~
-        
-        .. figure:: https://github.com/hyperspy/start_jupyter_cm/raw/main/images/jupyter_cm_macos.png
-           :alt: Jupyter context menu entries in macOS
-           :width: 450px
-        
-           Jupyter context menu entries on macOS.
-        
-        
-        The context menu is only available when an object (folder or file) is
-        selected in Finder. The Jupyter options will be available from the
-        "Services" section of the menu. If a folder is selected then an instance of
-        Jupyter QTConsole/notebook/lab opens in the selected folder. If a file
-        is selected then Jupyter is started in the file directory. If the
-        file is a jupyter notebook (\*.ipynb), then selecting Jupyter notebook/lab
-        will open the file in that program; Jupyter QtConsole will still only
-        open in the file directory.
-        
-        As the processes are opened through a shell script in Automator, a spinning
-        cog will be visible in the menu bar when the processes are running. Once you
-        have finished with the server then manually kill the process via the
-        drop-down menu from this spinning cog.
-        
-        The launchers have been tested on macOS Mojave (10.14.6), Catalina (10.15) and Big Sur (11.1-11.5.1).
-        
-        Installation instructions
-        -------------------------
-        
-        Install from pypi using pip:
-        
-        .. code:: bash
-        
-            $ pip install start_jupyter_cm
-        
-        Or install from conda-forge channel using conda (in a Anaconda/Miniconda distribution):
-        
-        .. code:: bash
-        
-            $ conda install -c conda-forge start_jupyter_cm
-        
-        Usage
-        -----
-        
-        Create context menu shortcut(s)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        After installation, enable the context menu entries from a terminal as follows:
-        
-        .. code:: bash
-        
-            $ start_jupyter_cm
-        
-        On Microscoft Windows, the administrator rights are required to add the
-        entry for all users, otherwise the entries will be added only for the
-        current user. In GNOME and OSX only for the current user.
-        
-        Remove context menu shortcut(s)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        To remove the context menu entries execute the following in a terminal:
-        
-        .. code::
-        
-            $ start_jupyter_cm --remove
-        
-        Also, be aware that, uninstalling the package does not
-        remove the context menu entries. If you are left with the context menu
-        entries after uninstalling ``start_jupyter_cm``, reinstall it, remove
-        the entries as above and uninstall it again.
-        
-        Optional arguments
-        ~~~~~~~~~~~~~~~~~~
-        
-        On Linux, several file manager can be installed, to create or remove the context
-        menu shortcut(s) for a specific file manager, use the ``--file_manager`` (``-f``) option:
-        
-        .. code:: bash
-        
-            $ start_jupyter_cm -f nautilus
-        
-        Help
-        ~~~~
-        
-        Use the command line help for more information:
-        
-        .. code:: bash
-        
-            $ start_jupyter_cm -h
-        
-        
-        More information
-        ----------------
-        
-        Linux
-        ~~~~~
-        
-        On linux, the context menu shortcuts are created by adding scripts or
-        configuration files for each file manager. The location of these files are:
-        
-        - Nautilus: ``~/.local/share/nautilus/scripts``
-        - Caja: ``~/.config/caja/scripts``
-        - Dolphin: ``~/.local/share/kservices5/ServiceMenus``
-        - Nemo: ``~/.local/share/nemo/actions``
-        
-        
-        Related software
-        ----------------
-        
-        -  `nbmanager <https://github.com/takluyver/nbmanager>`__ Discover and
-           shutdown Jupyter servers.
-        -  `nbopen <https://github.com/takluyver/nbopen>`__ Open a notebook
-           using your filemanager.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Topic :: Desktop Environment :: Gnome
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+start\_jupyter\_cm
+==================
+
+|python_version| |pypi_version| |conda-forge| |tests| |license|
+
+.. |pypi_version| image:: https://img.shields.io/pypi/v/start-jupyter-cm.svg?style=flat
+   :target: https://pypi.python.org/pypi/start-jupyter-cm
+   :alt: PyPI version
+
+.. |python_version| image:: https://img.shields.io/pypi/pyversions/start-jupyter-cm.svg?style=flat
+   :target: https://pypi.python.org/pypi/start-jupyter-cm
+   :alt: Supported python versions
+
+.. |conda-forge| image:: https://img.shields.io/conda/vn/conda-forge/start_jupyter_cm
+   :target: https://anaconda.org/conda-forge/start_jupyter_cm
+   :alt: Conda forge version
+
+.. |Tests| image:: https://github.com/hyperspy/start_jupyter_cm/actions/workflows/tests.yml/badge.svg
+   :target: https://github.com/hyperspy/start_jupyter_cm/actions/workflows/tests.yml
+   :alt: Github tests status
+
+.. |license| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
+   :target: https://www.gnu.org/licenses/gpl-3.0
+   :alt: License: GPL v3
+
+Description
+-----------
+
+Add entries to start the `Jupyter Notebook <https://jupyter-notebook.readthedocs.io>`__,
+`Jupyter QtConsole <https://qtconsole.readthedocs.io>`__ or
+`JupyterLab <https://jupyterlab.readthedocs.io>`__ from the file
+manager context menu. This offers a convenient way of starting Jupyter
+in a folder. Currently it only supports Microsoft Windows, GNOME (and
+its many derivatives), and macOS. Contributions to support other OSs/desktop
+environments are highly welcome.
+
+`WinPython <http://winpython.github.io>`__ and
+`Anaconda <https://www.anaconda.com/distribution>`__/
+`Miniconda <https://docs.conda.io/en/latest/miniconda.html>`__/
+`Miniforge <https://github.com/conda-forge/miniforge>`__/
+`Mambaforge <https://github.com/conda-forge/miniforge#mambaforge>`__
+distributions are supported. If run from a conda environment other than `root`,
+the name of the environment will be specified in brackets in the context menu name.
+
+Microsoft Windows
+~~~~~~~~~~~~~~~~~
+
+.. figure:: https://github.com/hyperspy/start_jupyter_cm/raw/main/images/jupyter_cm_windows.png
+   :alt: Jupyter context menu entries in windows
+   :width: 250px
+
+   Jupyter context menu entries in windows.
+
+
+In addition to starting the QtConsole, the Jupyter Notebook or the Jupyter Lab,
+and launching the default browser, in Microsoft Windows the process runs from
+a terminal. Closing the terminal closes the QtConsole or the Jupyter server.
+Single and all users installations are supported, see installation instructions below.
+
+Linux
+~~~~~
+
+On linux, the supported file managers are: Nautilus (GNOME), Caja (MATE), Dolphin (KDE) and Nemo (Cinnamon).
+With Nautilus and Caja, the shortcut will appear in the *Scripts* menu and with
+Dolphin, it will appear in the *Actions* menu.
+
+.. figure:: https://github.com/hyperspy/start_jupyter_cm/raw/main/images/jupyter_cm_gnome.png
+   :alt: Jupyter context menu entries in Nautilus
+   :width: 450px
+
+   Jupyter context menu entries on Linux (Nautilus).
+
+
+When selecting multiple folders, one instance of Jupyter
+QtConsole/notebook/lab opens in each of the selected folders. Selecting a
+file starts Jupyter in the file directory.
+
+Note that on Linux the processes run in the background: to stop the jupyter
+notebook or lab, don't forget to exit using the *quit* button - only closing
+the tab will not stop the jupyter server. Alternatively, `nbmanager <https://github.com/takluyver/nbmanager>`__
+can discover all running servers and shut them down using via an UI.
+
+
+macOS
+~~~~~
+
+.. figure:: https://github.com/hyperspy/start_jupyter_cm/raw/main/images/jupyter_cm_macos.png
+   :alt: Jupyter context menu entries in macOS
+   :width: 450px
+
+   Jupyter context menu entries on macOS.
+
+
+The context menu is only available when an object (folder or file) is
+selected in Finder. The Jupyter options will be available from the
+"Services" section of the menu. If a folder is selected then an instance of
+Jupyter QTConsole/notebook/lab opens in the selected folder. If a file
+is selected then Jupyter is started in the file directory. If the
+file is a jupyter notebook (\*.ipynb), then selecting Jupyter notebook/lab
+will open the file in that program; Jupyter QtConsole will still only
+open in the file directory.
+
+As the processes are opened through a shell script in Automator, a spinning
+cog will be visible in the menu bar when the processes are running. Once you
+have finished with the server then manually kill the process via the
+drop-down menu from this spinning cog.
+
+The launchers have been tested on macOS Mojave (10.14) to Sonoma (14).
+
+Installation instructions
+-------------------------
+
+Install from pypi using pip:
+
+.. code:: bash
+
+    $ pip install start_jupyter_cm
+
+Or install from conda-forge channel using conda (in a Anaconda/Miniconda distribution):
+
+.. code:: bash
+
+    $ conda install -c conda-forge start_jupyter_cm
+
+Usage
+-----
+
+Create context menu shortcut(s)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+After installation, enable the context menu entries from a terminal as follows:
+
+.. code:: bash
+
+    $ start_jupyter_cm
+
+On Microscoft Windows, the administrator rights are required to add the
+entry for all users, otherwise the entries will be added only for the
+current user. In GNOME and OSX only for the current user.
+
+Remove context menu shortcut(s)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+To remove the context menu entries execute the following in a terminal:
+
+.. code::
+
+    $ start_jupyter_cm --remove
+
+Also, be aware that, uninstalling the package does not
+remove the context menu entries. If you are left with the context menu
+entries after uninstalling ``start_jupyter_cm``, reinstall it, remove
+the entries as above and uninstall it again.
+
+Optional arguments
+~~~~~~~~~~~~~~~~~~
+
+On Linux, several file manager can be installed, to create or remove the context
+menu shortcut(s) for a specific file manager, use the ``--file_manager`` (``-f``) option:
+
+.. code:: bash
+
+    $ start_jupyter_cm -f nautilus
+
+Help
+~~~~
+
+Use the command line help for more information:
+
+.. code:: bash
+
+    $ start_jupyter_cm -h
+
+
+More information
+----------------
+
+Linux
+~~~~~
+
+On linux, the context menu shortcuts are created by adding scripts or
+configuration files for each file manager. The location of these files are:
+
+- Nautilus: ``~/.local/share/nautilus/scripts``
+- Caja: ``~/.config/caja/scripts``
+- Dolphin: ``~/.local/share/kservices5/ServiceMenus``
+- Nemo: ``~/.local/share/nemo/actions``
+
+
+Related software
+----------------
+
+-  `nbmanager <https://github.com/takluyver/nbmanager>`__ Discover and
+   shutdown Jupyter servers.
+-  `nbopen <https://github.com/takluyver/nbopen>`__ Open a notebook
+   using your filemanager.
```

### Comparing `start_jupyter_cm-2.3.1/README.rst` & `start_jupyter_cm-2.3.2/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 start\_jupyter\_cm
 ==================
 
-|pypi_version|_  |python_version|_ |conda-forge|_ |tests|_
+|python_version| |pypi_version| |conda-forge| |tests| |license|
 
 .. |pypi_version| image:: https://img.shields.io/pypi/v/start-jupyter-cm.svg?style=flat
-.. _pypi_version: https://pypi.python.org/pypi/start-jupyter-cm
+   :target: https://pypi.python.org/pypi/start-jupyter-cm
+   :alt: PyPI version
 
 .. |python_version| image:: https://img.shields.io/pypi/pyversions/start-jupyter-cm.svg?style=flat
-.. _python_version: https://pypi.python.org/pypi/start-jupyter-cm
+   :target: https://pypi.python.org/pypi/start-jupyter-cm
+   :alt: Supported python versions
 
-.. |conda-forge| image:: https://img.shields.io/conda/pn/conda-forge/start_jupyter_cm?label=conda-forge
-.. _conda-forge: https://anaconda.org/conda-forge/start_jupyter_cm
+.. |conda-forge| image:: https://img.shields.io/conda/vn/conda-forge/start_jupyter_cm
+   :target: https://anaconda.org/conda-forge/start_jupyter_cm
+   :alt: Conda forge version
 
 .. |Tests| image:: https://github.com/hyperspy/start_jupyter_cm/actions/workflows/tests.yml/badge.svg
-.. _tests: https://github.com/hyperspy/start_jupyter_cm/actions/workflows/tests.yml
+   :target: https://github.com/hyperspy/start_jupyter_cm/actions/workflows/tests.yml
+   :alt: Github tests status
 
+.. |license| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
+   :target: https://www.gnu.org/licenses/gpl-3.0
+   :alt: License: GPL v3
 
 Description
 -----------
 
 Add entries to start the `Jupyter Notebook <https://jupyter-notebook.readthedocs.io>`__,
 `Jupyter QtConsole <https://qtconsole.readthedocs.io>`__ or
 `JupyterLab <https://jupyterlab.readthedocs.io>`__ from the file
@@ -94,15 +101,15 @@
 open in the file directory.
 
 As the processes are opened through a shell script in Automator, a spinning
 cog will be visible in the menu bar when the processes are running. Once you
 have finished with the server then manually kill the process via the
 drop-down menu from this spinning cog.
 
-The launchers have been tested on macOS Mojave (10.14.6), Catalina (10.15) and Big Sur (11.1-11.5.1).
+The launchers have been tested on macOS Mojave (10.14) to Sonoma (14).
 
 Installation instructions
 -------------------------
 
 Install from pypi using pip:
 
 .. code:: bash
```

### Comparing `start_jupyter_cm-2.3.1/setup.py` & `start_jupyter_cm-2.3.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,18 +44,20 @@
     description="Add entries to start Jupyter from context menu.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     license="BSDv3",
     url="https://github.com/hyperspy/start_jupyter_cm",
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Programming Language :: Python :: 3.13",
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
```

### Comparing `start_jupyter_cm-2.3.1/start_jupyter_cm/command.py` & `start_jupyter_cm-2.3.2/start_jupyter_cm/command.py`

 * *Files identical despite different names*

### Comparing `start_jupyter_cm-2.3.1/start_jupyter_cm/gnome.py` & `start_jupyter_cm-2.3.2/start_jupyter_cm/gnome.py`

 * *Files identical despite different names*

### Comparing `start_jupyter_cm-2.3.1/start_jupyter_cm/icons/jupyter-qtconsole.ico` & `start_jupyter_cm-2.3.2/start_jupyter_cm/icons/jupyter-qtconsole.ico`

 * *Files identical despite different names*

### Comparing `start_jupyter_cm-2.3.1/start_jupyter_cm/icons/jupyter-qtconsole.png` & `start_jupyter_cm-2.3.2/start_jupyter_cm/icons/jupyter-qtconsole.png`

 * *Files identical despite different names*

### Comparing `start_jupyter_cm-2.3.1/start_jupyter_cm/icons/jupyter.ico` & `start_jupyter_cm-2.3.2/start_jupyter_cm/icons/jupyter.ico`

 * *Files identical despite different names*

### Comparing `start_jupyter_cm-2.3.1/start_jupyter_cm/icons/jupyter.png` & `start_jupyter_cm-2.3.2/start_jupyter_cm/icons/jupyter.png`

 * *Files identical despite different names*

### Comparing `start_jupyter_cm-2.3.1/start_jupyter_cm/linux.py` & `start_jupyter_cm-2.3.2/start_jupyter_cm/linux.py`

 * *Files identical despite different names*

### Comparing `start_jupyter_cm-2.3.1/start_jupyter_cm/macos.py` & `start_jupyter_cm-2.3.2/start_jupyter_cm/macos.py`

 * *Files identical despite different names*

### Comparing `start_jupyter_cm-2.3.1/start_jupyter_cm/prototype.workflow/Contents/Info.plist` & `start_jupyter_cm-2.3.2/start_jupyter_cm/prototype.workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `start_jupyter_cm-2.3.1/start_jupyter_cm/prototype.workflow/Contents/document.wflow` & `start_jupyter_cm-2.3.2/start_jupyter_cm/prototype.workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `start_jupyter_cm-2.3.1/start_jupyter_cm/tests/test_command.py` & `start_jupyter_cm-2.3.2/start_jupyter_cm/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `start_jupyter_cm-2.3.1/start_jupyter_cm/windows.py` & `start_jupyter_cm-2.3.2/start_jupyter_cm/windows.py`

 * *Files identical despite different names*

### Comparing `start_jupyter_cm-2.3.1/start_jupyter_cm.egg-info/PKG-INFO` & `start_jupyter_cm-2.3.2/start_jupyter_cm.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,214 +1,223 @@
 Metadata-Version: 2.1
-Name: start-jupyter-cm
-Version: 2.3.1
+Name: start_jupyter_cm
+Version: 2.3.2
 Summary: Add entries to start Jupyter from context menu.
 Home-page: https://github.com/hyperspy/start_jupyter_cm
 Author: The HyperSpy Developers
 License: BSDv3
-Description: start\_jupyter\_cm
-        ==================
-        
-        |pypi_version|_  |python_version|_ |conda-forge|_ |tests|_
-        
-        .. |pypi_version| image:: https://img.shields.io/pypi/v/start-jupyter-cm.svg?style=flat
-        .. _pypi_version: https://pypi.python.org/pypi/start-jupyter-cm
-        
-        .. |python_version| image:: https://img.shields.io/pypi/pyversions/start-jupyter-cm.svg?style=flat
-        .. _python_version: https://pypi.python.org/pypi/start-jupyter-cm
-        
-        .. |conda-forge| image:: https://img.shields.io/conda/pn/conda-forge/start_jupyter_cm?label=conda-forge
-        .. _conda-forge: https://anaconda.org/conda-forge/start_jupyter_cm
-        
-        .. |Tests| image:: https://github.com/hyperspy/start_jupyter_cm/actions/workflows/tests.yml/badge.svg
-        .. _tests: https://github.com/hyperspy/start_jupyter_cm/actions/workflows/tests.yml
-        
-        
-        Description
-        -----------
-        
-        Add entries to start the `Jupyter Notebook <https://jupyter-notebook.readthedocs.io>`__,
-        `Jupyter QtConsole <https://qtconsole.readthedocs.io>`__ or
-        `JupyterLab <https://jupyterlab.readthedocs.io>`__ from the file
-        manager context menu. This offers a convenient way of starting Jupyter
-        in a folder. Currently it only supports Microsoft Windows, GNOME (and
-        its many derivatives), and macOS. Contributions to support other OSs/desktop
-        environments are highly welcome.
-        
-        `WinPython <http://winpython.github.io>`__ and
-        `Anaconda <https://www.anaconda.com/distribution>`__/
-        `Miniconda <https://docs.conda.io/en/latest/miniconda.html>`__/
-        `Miniforge <https://github.com/conda-forge/miniforge>`__/
-        `Mambaforge <https://github.com/conda-forge/miniforge#mambaforge>`__
-        distributions are supported. If run from a conda environment other than `root`,
-        the name of the environment will be specified in brackets in the context menu name.
-        
-        Microsoft Windows
-        ~~~~~~~~~~~~~~~~~
-        
-        .. figure:: https://github.com/hyperspy/start_jupyter_cm/raw/main/images/jupyter_cm_windows.png
-           :alt: Jupyter context menu entries in windows
-           :width: 250px
-        
-           Jupyter context menu entries in windows.
-        
-        
-        In addition to starting the QtConsole, the Jupyter Notebook or the Jupyter Lab,
-        and launching the default browser, in Microsoft Windows the process runs from
-        a terminal. Closing the terminal closes the QtConsole or the Jupyter server.
-        Single and all users installations are supported, see installation instructions below.
-        
-        Linux
-        ~~~~~
-        
-        On linux, the supported file managers are: Nautilus (GNOME), Caja (MATE), Dolphin (KDE) and Nemo (Cinnamon).
-        With Nautilus and Caja, the shortcut will appear in the *Scripts* menu and with
-        Dolphin, it will appear in the *Actions* menu.
-        
-        .. figure:: https://github.com/hyperspy/start_jupyter_cm/raw/main/images/jupyter_cm_gnome.png
-           :alt: Jupyter context menu entries in Nautilus
-           :width: 450px
-        
-           Jupyter context menu entries on Linux (Nautilus).
-        
-        
-        When selecting multiple folders, one instance of Jupyter
-        QtConsole/notebook/lab opens in each of the selected folders. Selecting a
-        file starts Jupyter in the file directory.
-        
-        Note that on Linux the processes run in the background: to stop the jupyter
-        notebook or lab, don't forget to exit using the *quit* button - only closing
-        the tab will not stop the jupyter server. Alternatively, `nbmanager <https://github.com/takluyver/nbmanager>`__
-        can discover all running servers and shut them down using via an UI.
-        
-        
-        macOS
-        ~~~~~
-        
-        .. figure:: https://github.com/hyperspy/start_jupyter_cm/raw/main/images/jupyter_cm_macos.png
-           :alt: Jupyter context menu entries in macOS
-           :width: 450px
-        
-           Jupyter context menu entries on macOS.
-        
-        
-        The context menu is only available when an object (folder or file) is
-        selected in Finder. The Jupyter options will be available from the
-        "Services" section of the menu. If a folder is selected then an instance of
-        Jupyter QTConsole/notebook/lab opens in the selected folder. If a file
-        is selected then Jupyter is started in the file directory. If the
-        file is a jupyter notebook (\*.ipynb), then selecting Jupyter notebook/lab
-        will open the file in that program; Jupyter QtConsole will still only
-        open in the file directory.
-        
-        As the processes are opened through a shell script in Automator, a spinning
-        cog will be visible in the menu bar when the processes are running. Once you
-        have finished with the server then manually kill the process via the
-        drop-down menu from this spinning cog.
-        
-        The launchers have been tested on macOS Mojave (10.14.6), Catalina (10.15) and Big Sur (11.1-11.5.1).
-        
-        Installation instructions
-        -------------------------
-        
-        Install from pypi using pip:
-        
-        .. code:: bash
-        
-            $ pip install start_jupyter_cm
-        
-        Or install from conda-forge channel using conda (in a Anaconda/Miniconda distribution):
-        
-        .. code:: bash
-        
-            $ conda install -c conda-forge start_jupyter_cm
-        
-        Usage
-        -----
-        
-        Create context menu shortcut(s)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        After installation, enable the context menu entries from a terminal as follows:
-        
-        .. code:: bash
-        
-            $ start_jupyter_cm
-        
-        On Microscoft Windows, the administrator rights are required to add the
-        entry for all users, otherwise the entries will be added only for the
-        current user. In GNOME and OSX only for the current user.
-        
-        Remove context menu shortcut(s)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        To remove the context menu entries execute the following in a terminal:
-        
-        .. code::
-        
-            $ start_jupyter_cm --remove
-        
-        Also, be aware that, uninstalling the package does not
-        remove the context menu entries. If you are left with the context menu
-        entries after uninstalling ``start_jupyter_cm``, reinstall it, remove
-        the entries as above and uninstall it again.
-        
-        Optional arguments
-        ~~~~~~~~~~~~~~~~~~
-        
-        On Linux, several file manager can be installed, to create or remove the context
-        menu shortcut(s) for a specific file manager, use the ``--file_manager`` (``-f``) option:
-        
-        .. code:: bash
-        
-            $ start_jupyter_cm -f nautilus
-        
-        Help
-        ~~~~
-        
-        Use the command line help for more information:
-        
-        .. code:: bash
-        
-            $ start_jupyter_cm -h
-        
-        
-        More information
-        ----------------
-        
-        Linux
-        ~~~~~
-        
-        On linux, the context menu shortcuts are created by adding scripts or
-        configuration files for each file manager. The location of these files are:
-        
-        - Nautilus: ``~/.local/share/nautilus/scripts``
-        - Caja: ``~/.config/caja/scripts``
-        - Dolphin: ``~/.local/share/kservices5/ServiceMenus``
-        - Nemo: ``~/.local/share/nemo/actions``
-        
-        
-        Related software
-        ----------------
-        
-        -  `nbmanager <https://github.com/takluyver/nbmanager>`__ Discover and
-           shutdown Jupyter servers.
-        -  `nbopen <https://github.com/takluyver/nbopen>`__ Open a notebook
-           using your filemanager.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Topic :: Desktop Environment :: Gnome
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+start\_jupyter\_cm
+==================
+
+|python_version| |pypi_version| |conda-forge| |tests| |license|
+
+.. |pypi_version| image:: https://img.shields.io/pypi/v/start-jupyter-cm.svg?style=flat
+   :target: https://pypi.python.org/pypi/start-jupyter-cm
+   :alt: PyPI version
+
+.. |python_version| image:: https://img.shields.io/pypi/pyversions/start-jupyter-cm.svg?style=flat
+   :target: https://pypi.python.org/pypi/start-jupyter-cm
+   :alt: Supported python versions
+
+.. |conda-forge| image:: https://img.shields.io/conda/vn/conda-forge/start_jupyter_cm
+   :target: https://anaconda.org/conda-forge/start_jupyter_cm
+   :alt: Conda forge version
+
+.. |Tests| image:: https://github.com/hyperspy/start_jupyter_cm/actions/workflows/tests.yml/badge.svg
+   :target: https://github.com/hyperspy/start_jupyter_cm/actions/workflows/tests.yml
+   :alt: Github tests status
+
+.. |license| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
+   :target: https://www.gnu.org/licenses/gpl-3.0
+   :alt: License: GPL v3
+
+Description
+-----------
+
+Add entries to start the `Jupyter Notebook <https://jupyter-notebook.readthedocs.io>`__,
+`Jupyter QtConsole <https://qtconsole.readthedocs.io>`__ or
+`JupyterLab <https://jupyterlab.readthedocs.io>`__ from the file
+manager context menu. This offers a convenient way of starting Jupyter
+in a folder. Currently it only supports Microsoft Windows, GNOME (and
+its many derivatives), and macOS. Contributions to support other OSs/desktop
+environments are highly welcome.
+
+`WinPython <http://winpython.github.io>`__ and
+`Anaconda <https://www.anaconda.com/distribution>`__/
+`Miniconda <https://docs.conda.io/en/latest/miniconda.html>`__/
+`Miniforge <https://github.com/conda-forge/miniforge>`__/
+`Mambaforge <https://github.com/conda-forge/miniforge#mambaforge>`__
+distributions are supported. If run from a conda environment other than `root`,
+the name of the environment will be specified in brackets in the context menu name.
+
+Microsoft Windows
+~~~~~~~~~~~~~~~~~
+
+.. figure:: https://github.com/hyperspy/start_jupyter_cm/raw/main/images/jupyter_cm_windows.png
+   :alt: Jupyter context menu entries in windows
+   :width: 250px
+
+   Jupyter context menu entries in windows.
+
+
+In addition to starting the QtConsole, the Jupyter Notebook or the Jupyter Lab,
+and launching the default browser, in Microsoft Windows the process runs from
+a terminal. Closing the terminal closes the QtConsole or the Jupyter server.
+Single and all users installations are supported, see installation instructions below.
+
+Linux
+~~~~~
+
+On linux, the supported file managers are: Nautilus (GNOME), Caja (MATE), Dolphin (KDE) and Nemo (Cinnamon).
+With Nautilus and Caja, the shortcut will appear in the *Scripts* menu and with
+Dolphin, it will appear in the *Actions* menu.
+
+.. figure:: https://github.com/hyperspy/start_jupyter_cm/raw/main/images/jupyter_cm_gnome.png
+   :alt: Jupyter context menu entries in Nautilus
+   :width: 450px
+
+   Jupyter context menu entries on Linux (Nautilus).
+
+
+When selecting multiple folders, one instance of Jupyter
+QtConsole/notebook/lab opens in each of the selected folders. Selecting a
+file starts Jupyter in the file directory.
+
+Note that on Linux the processes run in the background: to stop the jupyter
+notebook or lab, don't forget to exit using the *quit* button - only closing
+the tab will not stop the jupyter server. Alternatively, `nbmanager <https://github.com/takluyver/nbmanager>`__
+can discover all running servers and shut them down using via an UI.
+
+
+macOS
+~~~~~
+
+.. figure:: https://github.com/hyperspy/start_jupyter_cm/raw/main/images/jupyter_cm_macos.png
+   :alt: Jupyter context menu entries in macOS
+   :width: 450px
+
+   Jupyter context menu entries on macOS.
+
+
+The context menu is only available when an object (folder or file) is
+selected in Finder. The Jupyter options will be available from the
+"Services" section of the menu. If a folder is selected then an instance of
+Jupyter QTConsole/notebook/lab opens in the selected folder. If a file
+is selected then Jupyter is started in the file directory. If the
+file is a jupyter notebook (\*.ipynb), then selecting Jupyter notebook/lab
+will open the file in that program; Jupyter QtConsole will still only
+open in the file directory.
+
+As the processes are opened through a shell script in Automator, a spinning
+cog will be visible in the menu bar when the processes are running. Once you
+have finished with the server then manually kill the process via the
+drop-down menu from this spinning cog.
+
+The launchers have been tested on macOS Mojave (10.14) to Sonoma (14).
+
+Installation instructions
+-------------------------
+
+Install from pypi using pip:
+
+.. code:: bash
+
+    $ pip install start_jupyter_cm
+
+Or install from conda-forge channel using conda (in a Anaconda/Miniconda distribution):
+
+.. code:: bash
+
+    $ conda install -c conda-forge start_jupyter_cm
+
+Usage
+-----
+
+Create context menu shortcut(s)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+After installation, enable the context menu entries from a terminal as follows:
+
+.. code:: bash
+
+    $ start_jupyter_cm
+
+On Microscoft Windows, the administrator rights are required to add the
+entry for all users, otherwise the entries will be added only for the
+current user. In GNOME and OSX only for the current user.
+
+Remove context menu shortcut(s)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+To remove the context menu entries execute the following in a terminal:
+
+.. code::
+
+    $ start_jupyter_cm --remove
+
+Also, be aware that, uninstalling the package does not
+remove the context menu entries. If you are left with the context menu
+entries after uninstalling ``start_jupyter_cm``, reinstall it, remove
+the entries as above and uninstall it again.
+
+Optional arguments
+~~~~~~~~~~~~~~~~~~
+
+On Linux, several file manager can be installed, to create or remove the context
+menu shortcut(s) for a specific file manager, use the ``--file_manager`` (``-f``) option:
+
+.. code:: bash
+
+    $ start_jupyter_cm -f nautilus
+
+Help
+~~~~
+
+Use the command line help for more information:
+
+.. code:: bash
+
+    $ start_jupyter_cm -h
+
+
+More information
+----------------
+
+Linux
+~~~~~
+
+On linux, the context menu shortcuts are created by adding scripts or
+configuration files for each file manager. The location of these files are:
+
+- Nautilus: ``~/.local/share/nautilus/scripts``
+- Caja: ``~/.config/caja/scripts``
+- Dolphin: ``~/.local/share/kservices5/ServiceMenus``
+- Nemo: ``~/.local/share/nemo/actions``
+
+
+Related software
+----------------
+
+-  `nbmanager <https://github.com/takluyver/nbmanager>`__ Discover and
+   shutdown Jupyter servers.
+-  `nbopen <https://github.com/takluyver/nbopen>`__ Open a notebook
+   using your filemanager.
```

### Comparing `start_jupyter_cm-2.3.1/start_jupyter_cm.egg-info/SOURCES.txt` & `start_jupyter_cm-2.3.2/start_jupyter_cm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

