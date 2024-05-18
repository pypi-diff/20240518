# Comparing `tmp/adafruit_circuitpython_requests-3.2.9.tar.gz` & `tmp/adafruit_circuitpython_requests-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit_circuitpython_requests-3.2.9.tar", last modified: Sun May 12 19:50:14 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_requests-4.0.0.tar", last modified: Sat May 18 15:37:09 2024, max compression
```

## Comparing `adafruit_circuitpython_requests-3.2.9.tar` & `adafruit_circuitpython_requests-4.0.0.tar`

### file list

```diff
@@ -1,90 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.128449 adafruit_circuitpython_requests-3.2.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.116448 adafruit_circuitpython_requests-3.2.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.116448 adafruit_circuitpython_requests-3.2.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.120449 adafruit_circuitpython_requests-3.2.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/.github/workflows/release_pypi.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1724 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     6147 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1098 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.120449 adafruit_circuitpython_requests-3.2.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-12 19:50:14.128449 adafruit_circuitpython_requests-3.2.9/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2642 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.128449 adafruit_circuitpython_requests-3.2.9/adafruit_circuitpython_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-12 19:50:14.000000 adafruit_circuitpython_requests-3.2.9/adafruit_circuitpython_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-12 19:50:14.000000 adafruit_circuitpython_requests-3.2.9/adafruit_circuitpython_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 19:50:14.000000 adafruit_circuitpython_requests-3.2.9/adafruit_circuitpython_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-12 19:50:14.000000 adafruit_circuitpython_requests-3.2.9/adafruit_circuitpython_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-12 19:50:14.000000 adafruit_circuitpython_requests-3.2.9/adafruit_circuitpython_requests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21326 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/adafruit_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.120449 adafruit_circuitpython_requests-3.2.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.120449 adafruit_circuitpython_requests-3.2.9/docs/_static/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4414 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/docs/_static/favicon.ico.license
--rwxr-xr-x   0 runner    (1001) docker     (127)      267 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/docs/api.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (127)     5400 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      803 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/docs/examples.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (127)      973 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.116448 adafruit_circuitpython_requests-3.2.9/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.120449 adafruit_circuitpython_requests-3.2.9/examples/cpython/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/cpython/requests_cpython_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/cpython/requests_cpython_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.124449 adafruit_circuitpython_requests-3.2.9/examples/esp32spi/
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/esp32spi/requests_esp32spi_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/esp32spi/requests_esp32spi_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.124449 adafruit_circuitpython_requests-3.2.9/examples/fona/
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/fona/requests_fona_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/fona/requests_fona_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.124449 adafruit_circuitpython_requests-3.2.9/examples/wifi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.124449 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_discord.py
--rw-r--r--   0 runner    (1001) docker     (127)    15772 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_fitbit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_mastodon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py
--rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_premiereleague.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_queuetimes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_steam.py
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_twitch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_youtube.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_multiple_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_status_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/requests_wifi_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/requests_wifi_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.124449 adafruit_circuitpython_requests-3.2.9/examples/wiznet5k/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wiznet5k/requests_wiznet5k_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wiznet5k/requests_wiznet5k_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 19:50:14.128449 adafruit_circuitpython_requests-3.2.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.128449 adafruit_circuitpython_requests-3.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/tests/chunk_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/tests/chunked_redirect_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/tests/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/tests/header_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/tests/method_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/tests/mocket.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/tests/parse_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/tests/protocol_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/tests/reuse_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:37:09.660899 adafruit_circuitpython_requests-4.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:37:09.644899 adafruit_circuitpython_requests-4.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:37:09.648899 adafruit_circuitpython_requests-4.0.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:37:09.648899 adafruit_circuitpython_requests-4.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/.github/workflows/release_pypi.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1724 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6147 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1098 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:37:09.648899 adafruit_circuitpython_requests-4.0.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-18 15:37:09.660899 adafruit_circuitpython_requests-4.0.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2642 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:37:09.660899 adafruit_circuitpython_requests-4.0.0/adafruit_circuitpython_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-18 15:37:09.000000 adafruit_circuitpython_requests-4.0.0/adafruit_circuitpython_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-18 15:37:09.000000 adafruit_circuitpython_requests-4.0.0/adafruit_circuitpython_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:37:09.000000 adafruit_circuitpython_requests-4.0.0/adafruit_circuitpython_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-18 15:37:09.000000 adafruit_circuitpython_requests-4.0.0/adafruit_circuitpython_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-18 15:37:09.000000 adafruit_circuitpython_requests-4.0.0/adafruit_circuitpython_requests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24905 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/adafruit_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:37:09.652899 adafruit_circuitpython_requests-4.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:37:09.652899 adafruit_circuitpython_requests-4.0.0/docs/_static/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4414 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/docs/_static/favicon.ico.license
+-rwxr-xr-x   0 runner    (1001) docker     (127)      267 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/docs/api.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5400 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      803 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/docs/examples.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (127)      973 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:37:09.644899 adafruit_circuitpython_requests-4.0.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:37:09.652899 adafruit_circuitpython_requests-4.0.0/examples/cpython/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/cpython/requests_cpython_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/cpython/requests_cpython_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:37:09.652899 adafruit_circuitpython_requests-4.0.0/examples/esp32spi/
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/esp32spi/requests_esp32spi_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/esp32spi/requests_esp32spi_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:37:09.652899 adafruit_circuitpython_requests-4.0.0/examples/fona/
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/fona/requests_fona_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/fona/requests_fona_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:37:09.652899 adafruit_circuitpython_requests-4.0.0/examples/wifi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:37:09.656899 adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_discord.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15772 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_fitbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_mastodon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_premiereleague.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_queuetimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_steam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_twitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_youtube.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_file_upload_image.png
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_file_upload_image.png.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_multiple_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_status_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/requests_wifi_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wifi/requests_wifi_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:37:09.656899 adafruit_circuitpython_requests-4.0.0/examples/wiznet5k/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wiznet5k/requests_wiznet5k_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/examples/wiznet5k/requests_wiznet5k_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 15:37:09.660899 adafruit_circuitpython_requests-4.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:37:09.656899 adafruit_circuitpython_requests-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/tests/chunk_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/tests/chunked_redirect_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/tests/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:37:09.656899 adafruit_circuitpython_requests-4.0.0/tests/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/tests/files/green_red.png
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/tests/files/green_red.png.license
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/tests/files/red_green.png
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/tests/files/red_green.png.license
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/tests/files_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/tests/header_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/tests/method_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/tests/mocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/tests/parse_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/tests/protocol_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-05-18 15:37:07.000000 adafruit_circuitpython_requests-4.0.0/tests/reuse_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-18 15:37:00.000000 adafruit_circuitpython_requests-4.0.0/tox.ini
```

### Comparing `adafruit_circuitpython_requests-3.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_requests-4.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/.gitignore` & `adafruit_circuitpython_requests-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/.pre-commit-config.yaml` & `adafruit_circuitpython_requests-4.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/.pylintrc` & `adafruit_circuitpython_requests-4.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_requests-4.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/LICENSE` & `adafruit_circuitpython_requests-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_requests-4.0.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/LICENSES/MIT.txt` & `adafruit_circuitpython_requests-4.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/LICENSES/Unlicense.txt` & `adafruit_circuitpython_requests-4.0.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/PKG-INFO` & `adafruit_circuitpython_requests-4.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-requests
-Version: 3.2.9
+Version: 4.0.0
 Summary: A requests-like library for web interfacing
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Requests
 Keywords: adafruit,blinka,circuitpython,micropython,requests,requests,,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Adafruit-Blinka
 Requires-Dist: Adafruit-Circuitpython-ConnectionManager
 Provides-Extra: optional
+Requires-Dist: requests; extra == "optional"
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-requests/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/requests/en/latest/
     :alt: Documentation Status
```

### Comparing `adafruit_circuitpython_requests-3.2.9/README.rst` & `adafruit_circuitpython_requests-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/adafruit_circuitpython_requests.egg-info/PKG-INFO` & `adafruit_circuitpython_requests-4.0.0/adafruit_circuitpython_requests.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-requests
-Version: 3.2.9
+Version: 4.0.0
 Summary: A requests-like library for web interfacing
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Requests
 Keywords: adafruit,blinka,circuitpython,micropython,requests,requests,,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Adafruit-Blinka
 Requires-Dist: Adafruit-Circuitpython-ConnectionManager
 Provides-Extra: optional
+Requires-Dist: requests; extra == "optional"
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-requests/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/requests/en/latest/
     :alt: Documentation Status
```

### Comparing `adafruit_circuitpython_requests-3.2.9/adafruit_circuitpython_requests.egg-info/SOURCES.txt` & `adafruit_circuitpython_requests-4.0.0/adafruit_circuitpython_requests.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -52,21 +52,29 @@
 examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py
 examples/wifi/expanded/requests_wifi_api_premiereleague.py
 examples/wifi/expanded/requests_wifi_api_queuetimes.py
 examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py
 examples/wifi/expanded/requests_wifi_api_steam.py
 examples/wifi/expanded/requests_wifi_api_twitch.py
 examples/wifi/expanded/requests_wifi_api_youtube.py
+examples/wifi/expanded/requests_wifi_file_upload.py
+examples/wifi/expanded/requests_wifi_file_upload_image.png
+examples/wifi/expanded/requests_wifi_file_upload_image.png.license
 examples/wifi/expanded/requests_wifi_multiple_cookies.py
 examples/wifi/expanded/requests_wifi_status_codes.py
 examples/wiznet5k/requests_wiznet5k_advanced.py
 examples/wiznet5k/requests_wiznet5k_simpletest.py
 tests/chunk_test.py
 tests/chunked_redirect_test.py
 tests/concurrent_test.py
 tests/conftest.py
+tests/files_test.py
 tests/header_test.py
 tests/method_test.py
 tests/mocket.py
 tests/parse_test.py
 tests/protocol_test.py
-tests/reuse_test.py
+tests/reuse_test.py
+tests/files/green_red.png
+tests/files/green_red.png.license
+tests/files/red_green.png
+tests/files/red_green.png.license
```

### Comparing `adafruit_circuitpython_requests-3.2.9/adafruit_requests.py` & `adafruit_circuitpython_requests-4.0.0/adafruit_requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,23 +32,26 @@
   https://github.com/adafruit/circuitpython/releases
 
 * Adafruit's Connection Manager library:
   https://github.com/adafruit/Adafruit_CircuitPython_ConnectionManager
 
 """
 
-__version__ = "3.2.9"
+__version__ = "4.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Requests.git"
 
 import errno
 import json as json_module
+import os
 import sys
 
 from adafruit_connection_manager import get_connection_manager
 
+SEEK_END = 2
+
 if not sys.implementation.name == "circuitpython":
     from types import TracebackType
     from typing import Any, Dict, Optional, Type
 
     from circuitpython_typing.socket import (
         SocketpoolModuleType,
         SocketType,
@@ -353,23 +356,79 @@
         session_id: Optional[str] = None,
     ) -> None:
         self._connection_manager = get_connection_manager(socket_pool)
         self._ssl_context = ssl_context
         self._session_id = session_id
         self._last_response = None
 
+    def _build_boundary_data(self, files: dict):  # pylint: disable=too-many-locals
+        boundary_string = self._build_boundary_string()
+        content_length = 0
+        boundary_objects = []
+
+        for field_name, field_values in files.items():
+            file_name = field_values[0]
+            file_handle = field_values[1]
+
+            boundary_objects.append(
+                f'--{boundary_string}\r\nContent-Disposition: form-data; name="{field_name}"'
+            )
+            if file_name is not None:
+                boundary_objects.append(f'; filename="{file_name}"')
+            boundary_objects.append("\r\n")
+            if len(field_values) >= 3:
+                file_content_type = field_values[2]
+                boundary_objects.append(f"Content-Type: {file_content_type}\r\n")
+            if len(field_values) >= 4:
+                file_headers = field_values[3]
+                for file_header_key, file_header_value in file_headers.items():
+                    boundary_objects.append(
+                        f"{file_header_key}: {file_header_value}\r\n"
+                    )
+            boundary_objects.append("\r\n")
+
+            if hasattr(file_handle, "read"):
+                is_binary = False
+                try:
+                    content = file_handle.read(1)
+                    is_binary = isinstance(content, bytes)
+                except UnicodeError:
+                    is_binary = False
+
+                if not is_binary:
+                    raise ValueError("Files must be opened in binary mode")
+
+                file_handle.seek(0, SEEK_END)
+                content_length += file_handle.tell()
+                file_handle.seek(0)
+
+            boundary_objects.append(file_handle)
+            boundary_objects.append("\r\n")
+
+        boundary_objects.append(f"--{boundary_string}--\r\n")
+
+        for boundary_object in boundary_objects:
+            if isinstance(boundary_object, str):
+                content_length += len(boundary_object)
+
+        return boundary_string, content_length, boundary_objects
+
+    @staticmethod
+    def _build_boundary_string():
+        return os.urandom(16).hex()
+
     @staticmethod
     def _check_headers(headers: Dict[str, str]):
         if not isinstance(headers, dict):
-            raise AttributeError("headers must be in dict format")
+            raise TypeError("Headers must be in dict format")
 
         for key, value in headers.items():
             if isinstance(value, (str, bytes)) or value is None:
                 continue
-            raise AttributeError(
+            raise TypeError(
                 f"Header part ({value}) from {key} must be of type str or bytes, not {type(value)}"
             )
 
     @staticmethod
     def _send(socket: SocketType, data: bytes):
         total_sent = 0
         while total_sent < len(data):
@@ -390,61 +449,89 @@
                 # Not EAGAIN; that was already handled.
                 raise OSError(errno.EIO)
             total_sent += sent
 
     def _send_as_bytes(self, socket: SocketType, data: str):
         return self._send(socket, bytes(data, "utf-8"))
 
+    def _send_boundary_objects(self, socket: SocketType, boundary_objects: Any):
+        for boundary_object in boundary_objects:
+            if isinstance(boundary_object, str):
+                self._send_as_bytes(socket, boundary_object)
+            else:
+                chunk_size = 32
+                b = bytearray(chunk_size)
+                while True:
+                    size = boundary_object.readinto(b)
+                    if size == 0:
+                        break
+                    self._send(socket, b[:size])
+
     def _send_header(self, socket, header, value):
         if value is None:
             return
         self._send_as_bytes(socket, header)
         self._send(socket, b": ")
         if isinstance(value, bytes):
             self._send(socket, value)
         else:
             self._send_as_bytes(socket, value)
         self._send(socket, b"\r\n")
 
-    # pylint: disable=too-many-arguments
-    def _send_request(
+    def _send_request(  # pylint: disable=too-many-arguments
         self,
         socket: SocketType,
         host: str,
         method: str,
         path: str,
         headers: Dict[str, str],
         data: Any,
         json: Any,
-    ):
+        files: Optional[Dict[str, tuple]],
+    ):  # pylint: disable=too-many-branches,too-many-locals,too-many-statements
         # Check headers
         self._check_headers(headers)
 
         # Convert data
         content_type_header = None
 
         # If json is sent, set content type header and convert to string
         if json is not None:
             assert data is None
+            assert files is None
             content_type_header = "application/json"
             data = json_module.dumps(json)
 
         # If data is sent and it's a dict, set content type header and convert to string
         if data and isinstance(data, dict):
+            assert files is None
             content_type_header = "application/x-www-form-urlencoded"
             _post_data = ""
             for k in data:
                 _post_data = "{}&{}={}".format(_post_data, k, data[k])
             # remove first "&" from concatenation
             data = _post_data[1:]
 
         # Convert str data to bytes
         if data and isinstance(data, str):
             data = bytes(data, "utf-8")
 
+        # If files are send, build data to send and calculate length
+        content_length = 0
+        boundary_objects = None
+        if files and isinstance(files, dict):
+            boundary_string, content_length, boundary_objects = (
+                self._build_boundary_data(files)
+            )
+            content_type_header = f"multipart/form-data; boundary={boundary_string}"
+        else:
+            if data is None:
+                data = b""
+            content_length = len(data)
+
         self._send_as_bytes(socket, method)
         self._send(socket, b" /")
         self._send_as_bytes(socket, path)
         self._send(socket, b" HTTP/1.1\r\n")
 
         # create lower-case supplied header list
         supplied_headers = {header.lower() for header in headers}
@@ -452,36 +539,39 @@
         # Send headers
         if not "host" in supplied_headers:
             self._send_header(socket, "Host", host)
         if not "user-agent" in supplied_headers:
             self._send_header(socket, "User-Agent", "Adafruit CircuitPython")
         if content_type_header and not "content-type" in supplied_headers:
             self._send_header(socket, "Content-Type", content_type_header)
-        if data and not "content-length" in supplied_headers:
-            self._send_header(socket, "Content-Length", str(len(data)))
+        if (data or files) and not "content-length" in supplied_headers:
+            self._send_header(socket, "Content-Length", str(content_length))
         # Iterate over keys to avoid tuple alloc
         for header in headers:
             self._send_header(socket, header, headers[header])
         self._send(socket, b"\r\n")
 
         # Send data
         if data:
             self._send(socket, bytes(data))
+        elif boundary_objects:
+            self._send_boundary_objects(socket, boundary_objects)
 
     # pylint: disable=too-many-branches, too-many-statements, unused-argument, too-many-arguments, too-many-locals
     def request(
         self,
         method: str,
         url: str,
         data: Optional[Any] = None,
         json: Optional[Any] = None,
         headers: Optional[Dict[str, str]] = None,
         stream: bool = False,
         timeout: float = 60,
         allow_redirects: bool = True,
+        files: Optional[Dict[str, tuple]] = None,
     ) -> Response:
         """Perform an HTTP request to the given url which we will parse to determine
         whether to use SSL ('https://') or not. We can also send some provided 'data'
         or a json dictionary which we will stringify. 'headers' is optional HTTP headers
         sent along. 'stream' will determine if we buffer everything, or whether to only
         read only when requested
         """
@@ -522,15 +612,17 @@
                 proto,
                 session_id=self._session_id,
                 timeout=timeout,
                 ssl_context=self._ssl_context,
             )
             ok = True
             try:
-                self._send_request(socket, host, method, path, headers, data, json)
+                self._send_request(
+                    socket, host, method, path, headers, data, json, files
+                )
             except OSError as exc:
                 last_exc = exc
                 ok = False
             if ok:
                 # Read the H of "HTTP/1.1" to make sure the socket is alive. send can appear to work
                 # even when the socket is closed.
                 if hasattr(socket, "recv"):
```

### Comparing `adafruit_circuitpython_requests-3.2.9/docs/_static/favicon.ico` & `adafruit_circuitpython_requests-4.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/docs/conf.py` & `adafruit_circuitpython_requests-4.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/docs/examples.rst` & `adafruit_circuitpython_requests-4.0.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/docs/index.rst` & `adafruit_circuitpython_requests-4.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/cpython/requests_cpython_advanced.py` & `adafruit_circuitpython_requests-4.0.0/examples/cpython/requests_cpython_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/cpython/requests_cpython_simpletest.py` & `adafruit_circuitpython_requests-4.0.0/examples/cpython/requests_cpython_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/esp32spi/requests_esp32spi_advanced.py` & `adafruit_circuitpython_requests-4.0.0/examples/esp32spi/requests_esp32spi_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/esp32spi/requests_esp32spi_simpletest.py` & `adafruit_circuitpython_requests-4.0.0/examples/esp32spi/requests_esp32spi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/fona/requests_fona_advanced.py` & `adafruit_circuitpython_requests-4.0.0/examples/fona/requests_fona_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/fona/requests_fona_simpletest.py` & `adafruit_circuitpython_requests-4.0.0/examples/fona/requests_fona_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py` & `adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_discord.py` & `adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_discord.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_fitbit.py` & `adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_fitbit.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_github.py` & `adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_github.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_mastodon.py` & `adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_mastodon.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py` & `adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py` & `adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py` & `adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_premiereleague.py` & `adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_premiereleague.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_queuetimes.py` & `adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_queuetimes.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py` & `adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_steam.py` & `adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_steam.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_twitch.py` & `adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_twitch.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_youtube.py` & `adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_api_youtube.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_multiple_cookies.py` & `adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_multiple_cookies.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_status_codes.py` & `adafruit_circuitpython_requests-4.0.0/examples/wifi/expanded/requests_wifi_status_codes.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/wifi/requests_wifi_advanced.py` & `adafruit_circuitpython_requests-4.0.0/examples/wifi/requests_wifi_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/wifi/requests_wifi_simpletest.py` & `adafruit_circuitpython_requests-4.0.0/examples/wifi/requests_wifi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/wiznet5k/requests_wiznet5k_advanced.py` & `adafruit_circuitpython_requests-4.0.0/examples/wiznet5k/requests_wiznet5k_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/examples/wiznet5k/requests_wiznet5k_simpletest.py` & `adafruit_circuitpython_requests-4.0.0/examples/wiznet5k/requests_wiznet5k_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/pyproject.toml` & `adafruit_circuitpython_requests-4.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-requests"
 description = "A requests-like library for web interfacing"
-version = "3.2.9"
+version = "4.0.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Requests"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit_circuitpython_requests-3.2.9/tests/chunk_test.py` & `adafruit_circuitpython_requests-4.0.0/tests/chunk_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/tests/chunked_redirect_test.py` & `adafruit_circuitpython_requests-4.0.0/tests/chunked_redirect_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/tests/concurrent_test.py` & `adafruit_circuitpython_requests-4.0.0/tests/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/tests/conftest.py` & `adafruit_circuitpython_requests-4.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/tests/header_test.py` & `adafruit_circuitpython_requests-4.0.0/tests/header_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 """ Header Tests """
 
 import mocket
 import pytest
 
 
 def test_check_headers_not_dict(requests):
-    with pytest.raises(AttributeError) as context:
+    with pytest.raises(TypeError) as context:
         requests._check_headers("")
-    assert "headers must be in dict format" in str(context)
+    assert "Headers must be in dict format" in str(context)
 
 
 def test_check_headers_not_valid(requests):
-    with pytest.raises(AttributeError) as context:
+    with pytest.raises(TypeError) as context:
         requests._check_headers(
             {"Good1": "a", "Good2": b"b", "Good3": None, "Bad1": True}
         )
     assert "Header part (True) from Bad1 must be of type str or bytes" in str(context)
 
 
 def test_check_headers_valid(requests):
```

### Comparing `adafruit_circuitpython_requests-3.2.9/tests/method_test.py` & `adafruit_circuitpython_requests-4.0.0/tests/method_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,30 +48,36 @@
     data = "31F"
     requests.post("http://" + mocket.MOCK_HOST_1 + "/post", data=data)
     sock.connect.assert_called_once_with((mocket.MOCK_POOL_IP, 80))
     sock.send.assert_called_with(b"31F")
 
 
 def test_post_form(sock, requests):
-    data = {"Date": "July 25, 2019", "Time": "12:00"}
+    data = {
+        "Date": "July 25, 2019",
+        "Time": "12:00",
+    }
     requests.post("http://" + mocket.MOCK_HOST_1 + "/post", data=data)
     sock.connect.assert_called_once_with((mocket.MOCK_POOL_IP, 80))
     sock.send.assert_has_calls(
         [
             mock.call(b"Content-Type"),
             mock.call(b": "),
             mock.call(b"application/x-www-form-urlencoded"),
             mock.call(b"\r\n"),
         ]
     )
     sock.send.assert_called_with(b"Date=July 25, 2019&Time=12:00")
 
 
 def test_post_json(sock, requests):
-    json_data = {"Date": "July 25, 2019", "Time": "12:00"}
+    json_data = {
+        "Date": "July 25, 2019",
+        "Time": "12:00",
+    }
     requests.post("http://" + mocket.MOCK_HOST_1 + "/post", json=json_data)
     sock.connect.assert_called_once_with((mocket.MOCK_POOL_IP, 80))
     sock.send.assert_has_calls(
         [
             mock.call(b"Content-Type"),
             mock.call(b": "),
             mock.call(b"application/json"),
```

### Comparing `adafruit_circuitpython_requests-3.2.9/tests/mocket.py` & `adafruit_circuitpython_requests-4.0.0/tests/mocket.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/tests/parse_test.py` & `adafruit_circuitpython_requests-4.0.0/tests/parse_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/tests/protocol_test.py` & `adafruit_circuitpython_requests-4.0.0/tests/protocol_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/tests/reuse_test.py` & `adafruit_circuitpython_requests-4.0.0/tests/reuse_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.9/tox.ini` & `adafruit_circuitpython_requests-4.0.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 [tox]
 envlist = py311
 
 [testenv]
 description = run tests
 deps =
     pytest==7.4.3
+    requests
 commands = pytest
 
 [testenv:coverage]
 description = run coverage
 deps =
     pytest==7.4.3
     pytest-cov==4.1.0
+    requests
 package = editable
 commands =
     coverage run --source=. --omit=tests/* --branch {posargs} -m pytest
     coverage report
     coverage html
 
 [testenv:lint]
```

