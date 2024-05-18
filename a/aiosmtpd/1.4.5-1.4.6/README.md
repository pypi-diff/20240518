# Comparing `tmp/aiosmtpd-1.4.5.tar.gz` & `tmp/aiosmtpd-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosmtpd-1.4.5.tar", last modified: Mon Mar  4 16:40:28 2024, max compression
+gzip compressed data, was "aiosmtpd-1.4.6.tar", last modified: Sat May 18 11:37:40 2024, max compression
```

## Comparing `aiosmtpd-1.4.5.tar` & `aiosmtpd-1.4.6.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:40:28.617266 aiosmtpd-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/.mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/DESCRIPTION.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10121 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-03-04 16:40:28.617266 aiosmtpd-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13248 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:40:28.609266 aiosmtpd-1.4.5/aiosmtpd/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18134 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:40:28.613266 aiosmtpd-1.4.5/aiosmtpd/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    13103 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:40:28.613266 aiosmtpd-1.4.5/aiosmtpd/docs/_exts/
--rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/_exts/autoprogramm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:40:28.613266 aiosmtpd-1.4.5/aiosmtpd/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/_static/aiosmtpd.css
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/auth.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/concepts.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    24993 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/controller.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14378 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/handlers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/lmtp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/manpage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/migrating.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16707 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/proxyprotocol.rst
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19249 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/smtp.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/lmtp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9538 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    17127 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/proxy_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:40:28.617266 aiosmtpd-1.4.5/aiosmtpd/qa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/qa/test_0packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/qa/test_1testsuite.py
--rw-r--r--   0 runner    (1001) docker     (127)    62501 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/smtp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:40:28.617266 aiosmtpd-1.4.5/aiosmtpd/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/testing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/testing/statuscodes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:40:28.617266 aiosmtpd-1.4.5/aiosmtpd/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:40:28.617266 aiosmtpd-1.4.5/aiosmtpd/tests/certs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/tests/certs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/tests/certs/server.crt
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/tests/certs/server.key
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/tests/certs/server_alt.crt
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/tests/certs/server_alt.key
--rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    34049 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/tests/test_lmtp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    41029 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/tests/test_proxyprotocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    23296 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    75092 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/tests/test_smtp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/tests/test_smtps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/tests/test_smtpsmuggling.py
--rw-r--r--   0 runner    (1001) docker     (127)    12805 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/aiosmtpd/tests/test_starttls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:40:28.617266 aiosmtpd-1.4.5/aiosmtpd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-03-04 16:40:28.000000 aiosmtpd-1.4.5/aiosmtpd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-03-04 16:40:28.000000 aiosmtpd-1.4.5/aiosmtpd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 16:40:28.000000 aiosmtpd-1.4.5/aiosmtpd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-04 16:40:28.000000 aiosmtpd-1.4.5/aiosmtpd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 16:40:28.000000 aiosmtpd-1.4.5/aiosmtpd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-04 16:40:28.000000 aiosmtpd-1.4.5/aiosmtpd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-04 16:40:28.000000 aiosmtpd-1.4.5/aiosmtpd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/bandit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/housekeep.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/lgtm.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/pytest.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)     5799 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/release.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-03-04 16:40:28.621266 aiosmtpd-1.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-03-04 16:40:19.000000 aiosmtpd-1.4.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:37:40.000693 aiosmtpd-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/.mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/DESCRIPTION.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10121 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-05-18 11:37:40.000693 aiosmtpd-1.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13408 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:37:39.992693 aiosmtpd-1.4.6/aiosmtpd/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18142 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:37:39.996693 aiosmtpd-1.4.6/aiosmtpd/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    13184 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:37:39.996693 aiosmtpd-1.4.6/aiosmtpd/docs/_exts/
+-rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/_exts/autoprogramm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:37:39.996693 aiosmtpd-1.4.6/aiosmtpd/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/_static/aiosmtpd.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/auth.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24993 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/controller.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14378 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/handlers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/lmtp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/manpage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/migrating.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16707 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/proxyprotocol.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19249 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/smtp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/lmtp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9538 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17127 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/proxy_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:37:39.996693 aiosmtpd-1.4.6/aiosmtpd/qa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/qa/test_0packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/qa/test_1testsuite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62685 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/smtp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:37:39.996693 aiosmtpd-1.4.6/aiosmtpd/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/testing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/testing/statuscodes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:37:40.000693 aiosmtpd-1.4.6/aiosmtpd/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:37:40.000693 aiosmtpd-1.4.6/aiosmtpd/tests/certs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/tests/certs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/tests/certs/server.crt
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/tests/certs/server.key
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/tests/certs/server_alt.crt
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/tests/certs/server_alt.key
+-rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34049 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/tests/test_lmtp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41029 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/tests/test_proxyprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23296 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75092 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/tests/test_smtp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/tests/test_smtps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/tests/test_smtpsmuggling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12805 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/aiosmtpd/tests/test_starttls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:37:40.000693 aiosmtpd-1.4.6/aiosmtpd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-05-18 11:37:39.000000 aiosmtpd-1.4.6/aiosmtpd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-18 11:37:39.000000 aiosmtpd-1.4.6/aiosmtpd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 11:37:39.000000 aiosmtpd-1.4.6/aiosmtpd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-18 11:37:39.000000 aiosmtpd-1.4.6/aiosmtpd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 11:37:39.000000 aiosmtpd-1.4.6/aiosmtpd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 11:37:39.000000 aiosmtpd-1.4.6/aiosmtpd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-18 11:37:39.000000 aiosmtpd-1.4.6/aiosmtpd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/bandit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/housekeep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/lgtm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/pytest.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5799 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/release.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-18 11:37:40.000693 aiosmtpd-1.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-18 11:37:31.000000 aiosmtpd-1.4.6/tox.ini
```

### Comparing `aiosmtpd-1.4.5/.mypy.ini` & `aiosmtpd-1.4.6/.mypy.ini`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/DESCRIPTION.rst` & `aiosmtpd-1.4.6/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/LICENSE` & `aiosmtpd-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/PKG-INFO` & `aiosmtpd-1.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosmtpd
-Version: 1.4.5
+Version: 1.4.6
 Summary: aiosmtpd - asyncio based SMTP server
 Home-page: https://aiosmtpd.readthedocs.io/
 Maintainer: The aiosmtpd Developers
 Maintainer-email: aiosmtpd@googlegroups.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/aio-libs/aiosmtpd/issues
 Project-URL: Documentation, https://aiosmtpd.readthedocs.io/
```

### Comparing `aiosmtpd-1.4.5/README.rst` & `aiosmtpd-1.4.6/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -313,14 +313,16 @@
 +=========================+================+==================================+
 | ``5D60 CE28 9CD7 C258`` | Pandu E POLUAN | pepoluan at gmail period com     |
 +-------------------------+----------------+----------------------------------+
 | ``5555 A6A6 7AE1 DC91`` | Pandu E POLUAN | pepoluan at gmail period com     |
 +-------------------------+----------------+----------------------------------+
 | ``E309 FD82 73BD 8465`` | Wayne Werner   | waynejwerner at gmail period com |
 +-------------------------+----------------+----------------------------------+
+| ``5FE9 28CD 9626 CE2B`` | Sam Bull       | sam at sambull period org        |
++-------------------------+----------------+----------------------------------+
 
 
 
 .. _PyPI: https://pypi.org/project/aiosmtpd/
 .. _`GitHub Releases`: https://github.com/aio-libs/aiosmtpd/releases
```

### Comparing `aiosmtpd-1.4.5/aiosmtpd/__init__.py` & `aiosmtpd-1.4.6/aiosmtpd/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2014-2021 The aiosmtpd Developers
 # SPDX-License-Identifier: Apache-2.0
 import asyncio
 import warnings
 
 
-__version__ = "1.4.5"
+__version__ = "1.4.6"
 
 
 def _get_or_new_eventloop() -> asyncio.AbstractEventLoop:
     loop = None
     with warnings.catch_warnings():
         warnings.simplefilter("error")
         try:
```

### Comparing `aiosmtpd-1.4.5/aiosmtpd/controller.py` & `aiosmtpd-1.4.6/aiosmtpd/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,15 @@
         # Perform some stoppages to ensure endpoint no longer bound.
         assert self.server is not None
         self.server.close()
         self.loop.run_until_complete(self.server.wait_closed())
         self.loop.close()
         self.server = None
 
-    def start(self):
+    def start(self) -> None:
         """
         Start a thread and run the asyncio event loop in that thread
         """
         assert self._thread is None, "SMTP daemon already running"
         self._factory_invoked.clear()
 
         ready_event = threading.Event()
```

### Comparing `aiosmtpd-1.4.5/aiosmtpd/docs/Makefile` & `aiosmtpd-1.4.6/aiosmtpd/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/docs/NEWS.rst` & `aiosmtpd-1.4.6/aiosmtpd/docs/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 ###################
  NEWS for aiosmtpd
 ###################
 
 .. towncrier release notes start
 
+1.4.6 (2024-05-18)
+==================
+
+* STARTTLS is now fully enforced if used.
 
 1.4.5 (2024-03-02)
 ==================
 
 * Fixed incorrect handling of newlines.
```

### Comparing `aiosmtpd-1.4.5/aiosmtpd/docs/_exts/autoprogramm.py` & `aiosmtpd-1.4.6/aiosmtpd/docs/_exts/autoprogramm.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,15 +300,15 @@
     is_program: bool,
     is_subgroup: bool,
     description: Optional[str],
     usage: Optional[str],
     usage_strip: bool,
     usage_codeblock: bool,
     epilog: Optional[str],
-    options_title: str,
+    options_title: Optional[str],
     options_adornment: str,
 ):
     if usage_strip:
         assert usage is not None
         to_strip = (title or "").rsplit(" ", 1)[0]
 
         len_to_strip = len(to_strip) - 4
```

### Comparing `aiosmtpd-1.4.5/aiosmtpd/docs/_static/aiosmtpd.css` & `aiosmtpd-1.4.6/aiosmtpd/docs/_static/aiosmtpd.css`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/docs/auth.rst` & `aiosmtpd-1.4.6/aiosmtpd/docs/auth.rst`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/docs/cli.rst` & `aiosmtpd-1.4.6/aiosmtpd/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/docs/concepts.rst` & `aiosmtpd-1.4.6/aiosmtpd/docs/concepts.rst`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/docs/conf.py` & `aiosmtpd-1.4.6/aiosmtpd/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/docs/controller.rst` & `aiosmtpd-1.4.6/aiosmtpd/docs/controller.rst`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/docs/handlers.rst` & `aiosmtpd-1.4.6/aiosmtpd/docs/handlers.rst`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/docs/intro.rst` & `aiosmtpd-1.4.6/aiosmtpd/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/docs/lmtp.rst` & `aiosmtpd-1.4.6/aiosmtpd/docs/lmtp.rst`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/docs/manpage.rst` & `aiosmtpd-1.4.6/aiosmtpd/docs/manpage.rst`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/docs/migrating.rst` & `aiosmtpd-1.4.6/aiosmtpd/docs/migrating.rst`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/docs/proxyprotocol.rst` & `aiosmtpd-1.4.6/aiosmtpd/docs/proxyprotocol.rst`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/docs/smtp.rst` & `aiosmtpd-1.4.6/aiosmtpd/docs/smtp.rst`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/docs/testing.rst` & `aiosmtpd-1.4.6/aiosmtpd/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/handlers.py` & `aiosmtpd-1.4.6/aiosmtpd/handlers.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/lmtp.py` & `aiosmtpd-1.4.6/aiosmtpd/lmtp.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/main.py` & `aiosmtpd-1.4.6/aiosmtpd/main.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/proxy_protocol.py` & `aiosmtpd-1.4.6/aiosmtpd/proxy_protocol.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/qa/test_0packaging.py` & `aiosmtpd-1.4.6/aiosmtpd/qa/test_0packaging.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/qa/test_1testsuite.py` & `aiosmtpd-1.4.6/aiosmtpd/qa/test_1testsuite.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/smtp.py` & `aiosmtpd-1.4.6/aiosmtpd/smtp.py`

 * *Files 0% similar despite different names*

```diff
@@ -500,14 +500,17 @@
         self._reset_timeout()
         seen_starttls = (self._original_transport is not None)
         if self.transport is not None and seen_starttls:
             # It is STARTTLS connection over normal connection.
             self._reader._transport = transport  # type: ignore[attr-defined]
             self._writer._transport = transport  # type: ignore[attr-defined]
             self.transport = transport
+            # Discard any leftover unencrypted data
+            # See https://tools.ietf.org/html/rfc3207#page-7
+            self._reader._buffer.clear()  # type: ignore[attr-defined]
             # Do SSL certificate checking as rfc3207 part 4.1 says.  Why is
             # _extra a protected attribute?
             assert self._tls_protocol is not None
             self.session.ssl = self._tls_protocol._extra
             hook = self._handle_hooks.get("STARTTLS")
             if hook is None:
                 self._tls_handshake_okay = True
```

### Comparing `aiosmtpd-1.4.5/aiosmtpd/testing/helpers.py` & `aiosmtpd-1.4.6/aiosmtpd/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/testing/statuscodes.py` & `aiosmtpd-1.4.6/aiosmtpd/testing/statuscodes.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/tests/certs/server.crt` & `aiosmtpd-1.4.6/aiosmtpd/tests/certs/server.crt`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/tests/certs/server.key` & `aiosmtpd-1.4.6/aiosmtpd/tests/certs/server.key`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/tests/certs/server_alt.crt` & `aiosmtpd-1.4.6/aiosmtpd/tests/certs/server_alt.crt`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/tests/certs/server_alt.key` & `aiosmtpd-1.4.6/aiosmtpd/tests/certs/server_alt.key`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/tests/conftest.py` & `aiosmtpd-1.4.6/aiosmtpd/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/tests/test_handlers.py` & `aiosmtpd-1.4.6/aiosmtpd/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/tests/test_lmtp.py` & `aiosmtpd-1.4.6/aiosmtpd/tests/test_lmtp.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/tests/test_main.py` & `aiosmtpd-1.4.6/aiosmtpd/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/tests/test_misc.py` & `aiosmtpd-1.4.6/aiosmtpd/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/tests/test_proxyprotocol.py` & `aiosmtpd-1.4.6/aiosmtpd/tests/test_proxyprotocol.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/tests/test_server.py` & `aiosmtpd-1.4.6/aiosmtpd/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/tests/test_smtp.py` & `aiosmtpd-1.4.6/aiosmtpd/tests/test_smtp.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/tests/test_smtps.py` & `aiosmtpd-1.4.6/aiosmtpd/tests/test_smtps.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/tests/test_smtpsmuggling.py` & `aiosmtpd-1.4.6/aiosmtpd/tests/test_smtpsmuggling.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd/tests/test_starttls.py` & `aiosmtpd-1.4.6/aiosmtpd/tests/test_starttls.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/aiosmtpd.egg-info/PKG-INFO` & `aiosmtpd-1.4.6/aiosmtpd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosmtpd
-Version: 1.4.5
+Version: 1.4.6
 Summary: aiosmtpd - asyncio based SMTP server
 Home-page: https://aiosmtpd.readthedocs.io/
 Maintainer: The aiosmtpd Developers
 Maintainer-email: aiosmtpd@googlegroups.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/aio-libs/aiosmtpd/issues
 Project-URL: Documentation, https://aiosmtpd.readthedocs.io/
```

### Comparing `aiosmtpd-1.4.5/aiosmtpd.egg-info/SOURCES.txt` & `aiosmtpd-1.4.6/aiosmtpd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/bandit.yml` & `aiosmtpd-1.4.6/bandit.yml`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/housekeep.py` & `aiosmtpd-1.4.6/housekeep.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/pyproject.toml` & `aiosmtpd-1.4.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/pytest.ini` & `aiosmtpd-1.4.6/pytest.ini`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/release.py` & `aiosmtpd-1.4.6/release.py`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/setup.cfg` & `aiosmtpd-1.4.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `aiosmtpd-1.4.5/tox.ini` & `aiosmtpd-1.4.6/tox.ini`

 * *Files identical despite different names*

