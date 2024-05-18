# Comparing `tmp/nokey-0.5.0.tar.gz` & `tmp/nokey-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nokey-0.5.0.tar", max compression
+gzip compressed data, was "nokey-0.6.0.tar", max compression
```

## Comparing `nokey-0.5.0.tar` & `nokey-0.6.0.tar`

### file list

```diff
@@ -1,61 +1,64 @@
--rw-r--r--   0        0        0     1068 2024-04-10 23:28:41.225586 nokey-0.5.0/LICENSE
--rw-r--r--   0        0        0     3236 2024-05-11 23:20:17.607494 nokey-0.5.0/README.md
--rw-r--r--   0        0        0        0 2024-05-11 23:18:00.967494 nokey-0.5.0/nokey/__init__.py
--rw-r--r--   0        0        0     5116 2024-05-11 23:18:00.979494 nokey-0.5.0/nokey/activities/bored_api.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:00.939494 nokey-0.5.0/nokey/animals/__init__.py
--rw-r--r--   0        0        0     2754 2024-05-11 23:18:00.935494 nokey-0.5.0/nokey/animals/dog_api.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:01.035494 nokey-0.5.0/nokey/art_and_images/__init__.py
--rw-r--r--   0        0        0    92946 2024-05-11 23:18:01.031494 nokey-0.5.0/nokey/art_and_images/artic.py
--rw-r--r--   0        0        0     7770 2024-05-11 23:18:01.035494 nokey-0.5.0/nokey/art_and_images/lorem_picsum.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:00.923494 nokey-0.5.0/nokey/books_and_literature/__init__.py
--rw-r--r--   0        0        0     6079 2024-05-11 23:18:00.919494 nokey-0.5.0/nokey/books_and_literature/gutendex.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:01.103494 nokey-0.5.0/nokey/calendar/__init__.py
--rw-r--r--   0        0        0     4848 2024-05-11 23:18:01.099494 nokey-0.5.0/nokey/calendar/nager_date.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:01.043494 nokey-0.5.0/nokey/country_info/__init__.py
--rw-r--r--   0        0        0     4740 2024-05-11 23:18:01.043494 nokey-0.5.0/nokey/country_info/rest_country.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:00.895494 nokey-0.5.0/nokey/developer_tools/__init__.py
--rw-r--r--   0        0        0     3945 2024-05-11 23:18:00.887494 nokey-0.5.0/nokey/developer_tools/apis_guru.py
--rw-r--r--   0        0        0     3564 2024-05-11 23:18:00.883494 nokey-0.5.0/nokey/developer_tools/filter_lists.py
--rw-r--r--   0        0        0     2578 2024-05-11 23:18:00.883494 nokey-0.5.0/nokey/developer_tools/microlink.py
--rw-r--r--   0        0        0     7314 2024-05-11 23:18:00.895494 nokey-0.5.0/nokey/developer_tools/url_haus.py
--rw-r--r--   0        0        0     1621 2024-05-11 23:18:00.891494 nokey-0.5.0/nokey/developer_tools/url_shortener.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:00.927494 nokey-0.5.0/nokey/education/__init__.py
--rw-r--r--   0        0        0     2348 2024-05-11 23:18:00.931494 nokey-0.5.0/nokey/education/university_domains_and_names.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:01.083494 nokey-0.5.0/nokey/finance_and_crypto/__init__.py
--rw-r--r--   0        0        0     5877 2024-05-11 23:18:01.075494 nokey-0.5.0/nokey/finance_and_crypto/coinmap.py
--rw-r--r--   0        0        0     2513 2024-05-11 23:18:01.079494 nokey-0.5.0/nokey/finance_and_crypto/exchange_api.py
--rw-r--r--   0        0        0     1127 2024-05-11 23:18:01.087494 nokey-0.5.0/nokey/finance_and_crypto/wall_street_bets.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:01.059494 nokey-0.5.0/nokey/food/__init__.py
--rw-r--r--   0        0        0     3198 2024-05-11 23:18:01.059494 nokey-0.5.0/nokey/food/fruityvice.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:01.011494 nokey-0.5.0/nokey/games/__init__.py
--rw-r--r--   0        0        0     6542 2024-05-11 23:18:01.011494 nokey-0.5.0/nokey/games/free_to_game.py
--rw-r--r--   0        0        0     5382 2024-05-11 23:18:01.007494 nokey-0.5.0/nokey/games/open_trivia_db.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:01.019494 nokey-0.5.0/nokey/geolocation/__init__.py
--rw-r--r--   0        0        0     1045 2024-05-11 23:18:01.023494 nokey-0.5.0/nokey/geolocation/ip_api.py
--rw-r--r--   0        0        0     1874 2024-05-11 23:18:01.019494 nokey-0.5.0/nokey/geolocation/zippopotamus.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:00.875494 nokey-0.5.0/nokey/government/__init__.py
--rw-r--r--   0        0        0    10654 2024-05-11 23:18:00.867494 nokey-0.5.0/nokey/government/federal_register.py
--rw-r--r--   0        0        0   157333 2024-05-11 23:18:00.875494 nokey-0.5.0/nokey/government/usa_spending.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:00.955494 nokey-0.5.0/nokey/helperFuncs/__init__.py
--rw-r--r--   0        0        0      822 2024-05-11 23:18:00.947494 nokey-0.5.0/nokey/helperFuncs/get_api_list.py
--rw-r--r--   0        0        0     5137 2024-05-11 23:18:00.951494 nokey-0.5.0/nokey/helperFuncs/make_request.py
--rw-r--r--   0        0        0      998 2024-05-11 23:18:00.947494 nokey-0.5.0/nokey/helperFuncs/nokey_apis.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:00.911494 nokey-0.5.0/nokey/inspiration/__init__.py
--rw-r--r--   0        0        0     5925 2024-05-11 23:18:00.915494 nokey-0.5.0/nokey/inspiration/dictum.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:01.051494 nokey-0.5.0/nokey/jokes/__init__.py
--rw-r--r--   0        0        0     3004 2024-05-11 23:18:01.051494 nokey-0.5.0/nokey/jokes/joke_api.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:01.095494 nokey-0.5.0/nokey/language/__init__.py
--rw-r--r--   0        0        0     1185 2024-05-11 23:18:01.091494 nokey-0.5.0/nokey/language/free_dictionary.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:00.999494 nokey-0.5.0/nokey/random/__init__.py
--rw-r--r--   0        0        0     1119 2024-05-11 23:18:00.999494 nokey-0.5.0/nokey/random/random_user.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:00.991494 nokey-0.5.0/nokey/science_and_nature/__init__.py
--rw-r--r--   0        0        0    50596 2024-05-11 23:18:00.987494 nokey-0.5.0/nokey/science_and_nature/integrated_taxonomic_information_system.py
--rw-r--r--   0        0        0     2948 2024-05-11 23:18:00.991494 nokey-0.5.0/nokey/science_and_nature/nobel_prize.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:00.963494 nokey-0.5.0/nokey/spaceflight/__init__.py
--rw-r--r--   0        0        0     8784 2024-05-11 23:18:00.959494 nokey-0.5.0/nokey/spaceflight/spaceflight_news.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:01.071494 nokey-0.5.0/nokey/tv_and_film/__init__.py
--rw-r--r--   0        0        0    43523 2024-05-11 23:18:01.067494 nokey-0.5.0/nokey/tv_and_film/star_trek_api.py
--rw-r--r--   0        0        0        0 2024-05-11 23:18:00.903494 nokey-0.5.0/nokey/weather/__init__.py
--rw-r--r--   0        0        0    26115 2024-05-11 23:18:00.907494 nokey-0.5.0/nokey/weather/national_weather_service.py
--rw-r--r--   0        0        0      684 2024-05-11 23:33:58.711494 nokey-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 nokey-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-10 23:28:41.225586 nokey-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3269 2024-05-18 19:50:31.691711 nokey-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:41.771711 nokey-0.6.0/nokey/__init__.py
+-rw-r--r--   0        0        0     5116 2024-05-18 19:53:41.879711 nokey-0.6.0/nokey/activities/bored_api.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:41.775711 nokey-0.6.0/nokey/animals/__init__.py
+-rw-r--r--   0        0        0     2754 2024-05-18 19:53:41.779711 nokey-0.6.0/nokey/animals/dog_api.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:42.019711 nokey-0.6.0/nokey/art_and_images/__init__.py
+-rw-r--r--   0        0        0    92946 2024-05-18 19:53:42.027711 nokey-0.6.0/nokey/art_and_images/artic.py
+-rw-r--r--   0        0        0     7770 2024-05-18 19:53:42.023711 nokey-0.6.0/nokey/art_and_images/lorem_picsum.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:41.931711 nokey-0.6.0/nokey/books_and_literature/__init__.py
+-rw-r--r--   0        0        0     6079 2024-05-18 19:53:41.931711 nokey-0.6.0/nokey/books_and_literature/gutendex.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:41.891711 nokey-0.6.0/nokey/calendar/__init__.py
+-rw-r--r--   0        0        0     4848 2024-05-18 19:53:41.895711 nokey-0.6.0/nokey/calendar/nager_date.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:41.783711 nokey-0.6.0/nokey/country_info/__init__.py
+-rw-r--r--   0        0        0     4740 2024-05-18 19:53:41.787711 nokey-0.6.0/nokey/country_info/rest_country.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:41.939711 nokey-0.6.0/nokey/developer_tools/__init__.py
+-rw-r--r--   0        0        0     3945 2024-05-18 19:53:41.951711 nokey-0.6.0/nokey/developer_tools/apis_guru.py
+-rw-r--r--   0        0        0     3564 2024-05-18 19:53:41.955711 nokey-0.6.0/nokey/developer_tools/filter_lists.py
+-rw-r--r--   0        0        0     2578 2024-05-18 19:53:41.955711 nokey-0.6.0/nokey/developer_tools/microlink.py
+-rw-r--r--   0        0        0     7314 2024-05-18 19:53:41.943711 nokey-0.6.0/nokey/developer_tools/url_haus.py
+-rw-r--r--   0        0        0     1621 2024-05-18 19:53:41.947711 nokey-0.6.0/nokey/developer_tools/url_shortener.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:41.871711 nokey-0.6.0/nokey/education/__init__.py
+-rw-r--r--   0        0        0     2348 2024-05-18 19:53:41.875711 nokey-0.6.0/nokey/education/university_domains_and_names.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:41.963711 nokey-0.6.0/nokey/finance_and_crypto/__init__.py
+-rw-r--r--   0        0        0     5877 2024-05-18 19:53:41.975711 nokey-0.6.0/nokey/finance_and_crypto/coinmap.py
+-rw-r--r--   0        0        0     2513 2024-05-18 19:53:41.971711 nokey-0.6.0/nokey/finance_and_crypto/exchange_api.py
+-rw-r--r--   0        0        0     1127 2024-05-18 19:53:41.967711 nokey-0.6.0/nokey/finance_and_crypto/wall_street_bets.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:41.795711 nokey-0.6.0/nokey/food/__init__.py
+-rw-r--r--   0        0        0     3198 2024-05-18 19:53:41.799711 nokey-0.6.0/nokey/food/fruityvice.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:41.903711 nokey-0.6.0/nokey/games/__init__.py
+-rw-r--r--   0        0        0     6542 2024-05-18 19:53:41.907711 nokey-0.6.0/nokey/games/free_to_game.py
+-rw-r--r--   0        0        0     5382 2024-05-18 19:53:41.911711 nokey-0.6.0/nokey/games/open_trivia_db.py
+-rw-r--r--   0        0        0    30240 2024-05-18 19:53:41.915711 nokey-0.6.0/nokey/games/shadify.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:41.859711 nokey-0.6.0/nokey/geolocation/__init__.py
+-rw-r--r--   0        0        0     1045 2024-05-18 19:53:41.859711 nokey-0.6.0/nokey/geolocation/ip_api.py
+-rw-r--r--   0        0        0     1874 2024-05-18 19:53:41.863711 nokey-0.6.0/nokey/geolocation/zippopotamus.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:41.991711 nokey-0.6.0/nokey/government/__init__.py
+-rw-r--r--   0        0        0    10654 2024-05-18 19:53:41.995711 nokey-0.6.0/nokey/government/federal_register.py
+-rw-r--r--   0        0        0   157333 2024-05-18 19:53:41.999711 nokey-0.6.0/nokey/government/usa_spending.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:42.035711 nokey-0.6.0/nokey/health/__init__.py
+-rw-r--r--   0        0        0    32028 2024-05-18 19:53:42.031711 nokey-0.6.0/nokey/health/open_disease.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:42.007711 nokey-0.6.0/nokey/helperFuncs/__init__.py
+-rw-r--r--   0        0        0      822 2024-05-18 19:53:42.011711 nokey-0.6.0/nokey/helperFuncs/get_api_list.py
+-rw-r--r--   0        0        0     5461 2024-05-18 19:53:42.011711 nokey-0.6.0/nokey/helperFuncs/make_request.py
+-rw-r--r--   0        0        0     1041 2024-05-18 19:53:42.015711 nokey-0.6.0/nokey/helperFuncs/nokey_apis.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:41.839711 nokey-0.6.0/nokey/inspiration/__init__.py
+-rw-r--r--   0        0        0     5925 2024-05-18 19:53:41.843711 nokey-0.6.0/nokey/inspiration/dictum.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:41.803711 nokey-0.6.0/nokey/jokes/__init__.py
+-rw-r--r--   0        0        0     3004 2024-05-18 19:53:41.807711 nokey-0.6.0/nokey/jokes/joke_api.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:41.847711 nokey-0.6.0/nokey/language/__init__.py
+-rw-r--r--   0        0        0     1185 2024-05-18 19:53:41.851711 nokey-0.6.0/nokey/language/free_dictionary.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:41.811711 nokey-0.6.0/nokey/random/__init__.py
+-rw-r--r--   0        0        0     1119 2024-05-18 19:53:41.815711 nokey-0.6.0/nokey/random/random_user.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:41.979711 nokey-0.6.0/nokey/science_and_nature/__init__.py
+-rw-r--r--   0        0        0    50596 2024-05-18 19:53:41.987711 nokey-0.6.0/nokey/science_and_nature/integrated_taxonomic_information_system.py
+-rw-r--r--   0        0        0     2948 2024-05-18 19:53:41.983711 nokey-0.6.0/nokey/science_and_nature/nobel_prize.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:41.823711 nokey-0.6.0/nokey/spaceflight/__init__.py
+-rw-r--r--   0        0        0     8784 2024-05-18 19:53:41.823711 nokey-0.6.0/nokey/spaceflight/spaceflight_news.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:41.919711 nokey-0.6.0/nokey/tv_and_film/__init__.py
+-rw-r--r--   0        0        0    43523 2024-05-18 19:53:41.923711 nokey-0.6.0/nokey/tv_and_film/star_trek_api.py
+-rw-r--r--   0        0        0        0 2024-05-18 19:53:41.831711 nokey-0.6.0/nokey/weather/__init__.py
+-rw-r--r--   0        0        0    26115 2024-05-18 19:53:41.835711 nokey-0.6.0/nokey/weather/national_weather_service.py
+-rw-r--r--   0        0        0      684 2024-05-18 19:52:25.415711 nokey-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4145 1970-01-01 00:00:00.000000 nokey-0.6.0/PKG-INFO
```

### Comparing `nokey-0.5.0/LICENSE` & `nokey-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/README.md` & `nokey-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,16 @@
 Free Dictionary
 
 ## games
 Free To Game
 
 Open Trivia Database
 
+Shadify
+
 ## activities
 Bored API
 
 ## calendar
 Nager.Date
 
 ## government
@@ -130,14 +132,17 @@
 Gutendex
 
 ## art_and_images
 Lorum Picsum
 
 Art Institute of Chicago
 
+## health
+Open Disease
+
 # Future Roadmap
 As the project grows, we envision expanding the collection of keyless APIs to cover a wide range of categories. Your feedback and contributions will play a crucial role in shaping the future of nokey.
 
 # License
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 # Documentation
```

### Comparing `nokey-0.5.0/nokey/activities/bored_api.py` & `nokey-0.6.0/nokey/activities/bored_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/animals/dog_api.py` & `nokey-0.6.0/nokey/animals/dog_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/art_and_images/artic.py` & `nokey-0.6.0/nokey/art_and_images/artic.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/art_and_images/lorem_picsum.py` & `nokey-0.6.0/nokey/art_and_images/lorem_picsum.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/books_and_literature/gutendex.py` & `nokey-0.6.0/nokey/books_and_literature/gutendex.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/calendar/nager_date.py` & `nokey-0.6.0/nokey/calendar/nager_date.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/country_info/rest_country.py` & `nokey-0.6.0/nokey/country_info/rest_country.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/developer_tools/apis_guru.py` & `nokey-0.6.0/nokey/developer_tools/apis_guru.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/developer_tools/filter_lists.py` & `nokey-0.6.0/nokey/developer_tools/filter_lists.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/developer_tools/microlink.py` & `nokey-0.6.0/nokey/developer_tools/microlink.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/developer_tools/url_haus.py` & `nokey-0.6.0/nokey/developer_tools/url_haus.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/developer_tools/url_shortener.py` & `nokey-0.6.0/nokey/developer_tools/url_shortener.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/education/university_domains_and_names.py` & `nokey-0.6.0/nokey/education/university_domains_and_names.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/finance_and_crypto/coinmap.py` & `nokey-0.6.0/nokey/finance_and_crypto/coinmap.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/finance_and_crypto/exchange_api.py` & `nokey-0.6.0/nokey/finance_and_crypto/exchange_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/finance_and_crypto/wall_street_bets.py` & `nokey-0.6.0/nokey/finance_and_crypto/wall_street_bets.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/food/fruityvice.py` & `nokey-0.6.0/nokey/food/fruityvice.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/games/free_to_game.py` & `nokey-0.6.0/nokey/games/free_to_game.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/games/open_trivia_db.py` & `nokey-0.6.0/nokey/games/open_trivia_db.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/geolocation/ip_api.py` & `nokey-0.6.0/nokey/geolocation/ip_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/geolocation/zippopotamus.py` & `nokey-0.6.0/nokey/geolocation/zippopotamus.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/government/federal_register.py` & `nokey-0.6.0/nokey/government/federal_register.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/government/usa_spending.py` & `nokey-0.6.0/nokey/government/usa_spending.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/helperFuncs/get_api_list.py` & `nokey-0.6.0/nokey/helperFuncs/get_api_list.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/helperFuncs/make_request.py` & `nokey-0.6.0/nokey/helperFuncs/make_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         else:
             response = requests.get(url, headers=headers)
         
         response.raise_for_status()  # Raise an exception for 4xx or 5xx status codes
         return response.json()  # Return JSON response
     except HTTPError as http_err:
         # Handle HTTP error
-        return {"error": f"HTTP error occurred: {http_err}"}
+        return {"error": f"HTTP error occurred: {http_err}", "message": response.json()["message"] if "message" in response.json() else None}
     except Timeout:
         # Handle timeout error
         return {"error": "Request timed out."}
     except RequestException as req_err:
         # Handle other request exceptions
         return {"error": f"Request exception occurred: {req_err}"}
     except Exception as err:
@@ -46,15 +46,15 @@
     - dict: A dictionary containing either the response data or an error message.
     """
     try:
         response = requests.get(url, params)
         return response.json()
     except HTTPError as http_err:
         # Handle HTTP error
-        return {"error": f"HTTP error occurred: {http_err}"}
+        return {"error": f"HTTP error occurred: {http_err}", "message": response.json()["message"] if "message" in response.json() else None}
     except Timeout:
         # Handle timeout error
         return {"error": "Request timed out."}
     except RequestException as req_err:
         # Handle other request exceptions
         return {"error": f"Request exception occurred: {req_err}"}
     except Exception as err:
@@ -99,15 +99,15 @@
     - dict: A dictionary containing either the response data or an error message.
     """
     try:
         response = requests.post(url, data=data)
         return response.json()
     except HTTPError as http_err:
         # Handle HTTP error
-        return {"error": f"HTTP error occurred: {http_err}"}
+        return {"error": f"HTTP error occurred: {http_err}", "message": response.json()["message"] if "message" in response.json() else None}
     except Timeout:
         # Handle timeout error
         return {"error": "Request timed out."}
     except RequestException as req_err:
         # Handle other request exceptions
         return {"error": f"Request exception occurred: {req_err}"}
     except Exception as err:
@@ -126,15 +126,15 @@
     - dict: A dictionary containing either the response data or an error message.
     """
     try:
         response = requests.post(url, json=json)
         return response.json()
     except HTTPError as http_err:
         # Handle HTTP error
-        return {"error": f"HTTP error occurred: {http_err}"}
+        return {"error": f"HTTP error occurred: {http_err}", "message": response.json()["message"] if "message" in response.json() else None}
     except Timeout:
         # Handle timeout error
         return {"error": "Request timed out."}
     except RequestException as req_err:
         # Handle other request exceptions
         return {"error": f"Request exception occurred: {req_err}"}
     except Exception as err:
```

### Comparing `nokey-0.5.0/nokey/helperFuncs/nokey_apis.py` & `nokey-0.6.0/nokey/helperFuncs/nokey_apis.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,16 @@
     "jokes": ["JokeAPI"],
     "animals": ["DogAPI"],
     "science_and_nature": ["Nobel Prize API", "Integrative Taxonomic Information System"],
     "weather": ["National Weather Service API"],
     "developer_tools": ["URL Shortener", "URLHaus", "APIsGuru", "Microlink", "FilterLists"],
     "inspiration": ["Dictum"],
     "language": ["Free Dictionary"],
-    "games": ["Free To Game", "Open Trivia Database"],
+    "games": ["Free To Game", "Open Trivia Database", "Shadify"],
     "activities": ["Bored API"],
     "calendar": ["Nager.Date"],
     "government": ["Federal Register", "USA Spending"],
     "art_and_images": ["Lorem Picsum", "Art Institute of Chicago"],
     "tv_and_film": ["Star Trek API"],
-    "books": ["Gutendex"]
+    "books": ["Gutendex"],
+    "health": ["Open Disease"]
 }
```

### Comparing `nokey-0.5.0/nokey/inspiration/dictum.py` & `nokey-0.6.0/nokey/inspiration/dictum.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/jokes/joke_api.py` & `nokey-0.6.0/nokey/jokes/joke_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/language/free_dictionary.py` & `nokey-0.6.0/nokey/language/free_dictionary.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/random/random_user.py` & `nokey-0.6.0/nokey/random/random_user.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/science_and_nature/integrated_taxonomic_information_system.py` & `nokey-0.6.0/nokey/science_and_nature/integrated_taxonomic_information_system.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/science_and_nature/nobel_prize.py` & `nokey-0.6.0/nokey/science_and_nature/nobel_prize.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/spaceflight/spaceflight_news.py` & `nokey-0.6.0/nokey/spaceflight/spaceflight_news.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/tv_and_film/star_trek_api.py` & `nokey-0.6.0/nokey/tv_and_film/star_trek_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/nokey/weather/national_weather_service.py` & `nokey-0.6.0/nokey/weather/national_weather_service.py`

 * *Files identical despite different names*

### Comparing `nokey-0.5.0/pyproject.toml` & `nokey-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nokey"
-version = "0.5.0"
+version = "0.6.0"
 description = "A python package for accessing APIs that require no key."
 authors = ["Spyder Rex <billyjohnsonauthor@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/SpyderRex/nokey"
 repository = "https://github.com/SpyderRex/nokey"
 license = "MIT"
 keywords = ["API", "requests", "xmltodict"]
```

### Comparing `nokey-0.5.0/PKG-INFO` & `nokey-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nokey
-Version: 0.5.0
+Version: 0.6.0
 Summary: A python package for accessing APIs that require no key.
 Home-page: https://github.com/SpyderRex/nokey
 License: MIT
 Keywords: API,requests,xmltodict
 Author: Spyder Rex
 Author-email: billyjohnsonauthor@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -131,14 +131,16 @@
 Free Dictionary
 
 ## games
 Free To Game
 
 Open Trivia Database
 
+Shadify
+
 ## activities
 Bored API
 
 ## calendar
 Nager.Date
 
 ## government
@@ -153,14 +155,17 @@
 Gutendex
 
 ## art_and_images
 Lorum Picsum
 
 Art Institute of Chicago
 
+## health
+Open Disease
+
 # Future Roadmap
 As the project grows, we envision expanding the collection of keyless APIs to cover a wide range of categories. Your feedback and contributions will play a crucial role in shaping the future of nokey.
 
 # License
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 # Documentation
```

