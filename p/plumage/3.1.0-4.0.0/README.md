# Comparing `tmp/plumage-3.1.0.tar.gz` & `tmp/plumage-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plumage-3.1.0.tar", max compression
+gzip compressed data, was "plumage-4.0.0.tar", max compression
```

## Comparing `plumage-3.1.0.tar` & `plumage-4.0.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     1613 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/__init__.py
--rw-r--r--   0        0        0     2175 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/config.py
--rw-r--r--   0        0        0     3703 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/dom_transforms.py
--rw-r--r--   0        0        0     2440 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/favicon.py
--rw-r--r--   0        0        0    33129 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/package-lock.json
--rw-r--r--   0        0        0      260 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/package.json
--rw-r--r--   0        0        0       73 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/postcss.config.js
--rw-r--r--   0        0        0        0 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/py.typed
--rw-r--r--   0        0        0     2765 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/code.scss
--rw-r--r--   0        0        0     5479 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/main.scss
--rw-r--r--   0        0        0      724 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/mglass.scss
--rw-r--r--   0        0        0     4514 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/abap.css
--rw-r--r--   0        0        0     4690 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/algol.css
--rw-r--r--   0        0        0     4600 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/algol_nu.css
--rw-r--r--   0        0        0     4761 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/arduino.css
--rw-r--r--   0        0        0     5240 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/autumn.css
--rw-r--r--   0        0        0     4470 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/borland.css
--rw-r--r--   0        0        0     3195 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/bw.css
--rw-r--r--   0        0        0     6160 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/colorful.css
--rw-r--r--   0        0        0     5823 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/default.css
--rw-r--r--   0        0        0     5612 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/emacs.css
--rw-r--r--   0        0        0     5974 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/friendly.css
--rw-r--r--   0        0        0     6587 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/fruity.css
--rw-r--r--   0        0        0     2905 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/igor.css
--rw-r--r--   0        0        0     6144 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/inkpot.css
--rw-r--r--   0        0        0     5727 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/lovelace.css
--rw-r--r--   0        0        0     5678 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/manni.css
--rw-r--r--   0        0        0     5596 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/monokai.css
--rw-r--r--   0        0        0     6113 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/murphy.css
--rw-r--r--   0        0        0     6390 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/native.css
--rw-r--r--   0        0        0     5972 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/paraiso-dark.css
--rw-r--r--   0        0        0     6044 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/paraiso-light.css
--rw-r--r--   0        0        0     6130 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/pastie.css
--rw-r--r--   0        0        0     5516 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/perldoc.css
--rw-r--r--   0        0        0     6078 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/rainbow_dash.css
--rw-r--r--   0        0        0     2988 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/rrt.css
--rw-r--r--   0        0        0     5044 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/sas.css
--rw-r--r--   0        0        0     6733 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/solarized-dark.css
--rw-r--r--   0        0        0     6811 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/solarized-light.css
--rw-r--r--   0        0        0     4513 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/stata-dark.css
--rw-r--r--   0        0        0     4485 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/stata-light.css
--rw-r--r--   0        0        0     4203 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/stata.css
--rw-r--r--   0        0        0     6480 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/tango.css
--rw-r--r--   0        0        0     5292 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/trac.css
--rw-r--r--   0        0        0     5715 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/vim.css
--rw-r--r--   0        0        0     2956 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/vs.css
--rw-r--r--   0        0        0     4703 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/xcode.css
--rw-r--r--   0        0        0     1369 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/android-chrome-192x192.png
--rw-r--r--   0        0        0     3279 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/android-chrome-512x512.png
--rw-r--r--   0        0        0     1035 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/apple-touch-icon.png
--rw-r--r--   0        0        0      246 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/browserconfig.xml
--rw-r--r--   0        0        0      260 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/favicon-16x16.png
--rw-r--r--   0        0        0      388 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/favicon-32x32.png
--rw-r--r--   0        0        0    15086 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/favicon.ico
--rw-r--r--   0        0        0     1115 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/mstile-144x144.png
--rw-r--r--   0        0        0     1007 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/mstile-150x150.png
--rw-r--r--   0        0        0     1022 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/mstile-310x150.png
--rw-r--r--   0        0        0     1848 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/mstile-310x310.png
--rw-r--r--   0        0        0      843 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/mstile-70x70.png
--rw-r--r--   0        0        0     2152 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/safari-pinned-tab.svg
--rw-r--r--   0        0        0      426 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/site.webmanifest
--rw-r--r--   0        0        0     1655 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/img/creampaper.jpeg
--rw-r--r--   0        0        0     1074 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/img/fabric_plaid.jpeg
--rw-r--r--   0        0        0      641 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/img/feather-alt-solid.svg
--rw-r--r--   0        0        0     1211 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/img/magnifier.png
--rw-r--r--   0        0        0     3588 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/img/play-button.png
--rw-r--r--   0        0        0     2543 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/js/application.js
--rw-r--r--   0        0        0     2366 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/js/jquery.mglass.js
--rw-r--r--   0        0        0      387 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/analytics.html
--rw-r--r--   0        0        0     3493 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/archives.html
--rw-r--r--   0        0        0     7667 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/article.html
--rw-r--r--   0        0        0      317 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/author.html
--rw-r--r--   0        0        0     1076 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/authors.html
--rw-r--r--   0        0        0    17390 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/base.html
--rw-r--r--   0        0        0     1117 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/categories.html
--rw-r--r--   0        0        0      715 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/category.html
--rw-r--r--   0        0        0      780 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/index.html
--rw-r--r--   0        0        0     2048 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/macros.html
--rw-r--r--   0        0        0      477 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/page.html
--rw-r--r--   0        0        0     2920 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/pagination.html
--rw-r--r--   0        0        0     1159 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/period_archives.html
--rw-r--r--   0        0        0     6982 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/projects.html
--rw-r--r--   0        0        0      695 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/tag.html
--rw-r--r--   0        0        0     1581 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/tags.html
--rw-r--r--   0        0        0      285 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/translations.html
--rw-r--r--   0        0        0     3864 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/webassets.py
--rw-r--r--   0        0        0     2250 2023-06-03 09:26:24.077968 plumage-3.1.0/pyproject.toml
--rw-r--r--   0        0        0    24824 2023-06-03 09:26:24.077968 plumage-3.1.0/readme.md
--rw-r--r--   0        0        0    26875 1970-01-01 00:00:00.000000 plumage-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1618 2024-05-18 05:59:32.170854 plumage-4.0.0/plumage/__init__.py
+-rw-r--r--   0        0        0     2194 2024-05-18 05:59:32.170854 plumage-4.0.0/plumage/config.py
+-rw-r--r--   0        0        0     3451 2024-05-18 05:59:32.170854 plumage-4.0.0/plumage/dom_transforms.py
+-rw-r--r--   0        0        0     2429 2024-05-18 05:59:32.170854 plumage-4.0.0/plumage/favicon.py
+-rw-r--r--   0        0        0    33966 2024-05-18 05:59:32.170854 plumage-4.0.0/plumage/package-lock.json
+-rw-r--r--   0        0        0      262 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/package.json
+-rw-r--r--   0        0        0       73 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/postcss.config.js
+-rw-r--r--   0        0        0        0 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/py.typed
+-rw-r--r--   0        0        0     2765 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/code.scss
+-rw-r--r--   0        0        0     6218 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/main.scss
+-rw-r--r--   0        0        0      724 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/mglass.scss
+-rw-r--r--   0        0        0     4431 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/abap.css
+-rw-r--r--   0        0        0     4513 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/algol.css
+-rw-r--r--   0        0        0     4442 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/algol_nu.css
+-rw-r--r--   0        0        0     4698 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/arduino.css
+-rw-r--r--   0        0        0     5229 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/autumn.css
+-rw-r--r--   0        0        0     4462 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/borland.css
+-rw-r--r--   0        0        0     3240 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/bw.css
+-rw-r--r--   0        0        0     6087 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/colorful.css
+-rw-r--r--   0        0        0     5798 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/default.css
+-rw-r--r--   0        0        0     5567 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/emacs.css
+-rw-r--r--   0        0        0     5923 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/friendly.css
+-rw-r--r--   0        0        0     6552 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/fruity.css
+-rw-r--r--   0        0        0     2848 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/igor.css
+-rw-r--r--   0        0        0     6175 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/inkpot.css
+-rw-r--r--   0        0        0     5787 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/lovelace.css
+-rw-r--r--   0        0        0     5623 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/manni.css
+-rw-r--r--   0        0        0     6119 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/monokai.css
+-rw-r--r--   0        0        0     6028 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/murphy.css
+-rw-r--r--   0        0        0     6433 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/native.css
+-rw-r--r--   0        0        0     6065 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/paraiso-dark.css
+-rw-r--r--   0        0        0     6139 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/paraiso-light.css
+-rw-r--r--   0        0        0     6032 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/pastie.css
+-rw-r--r--   0        0        0     5497 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/perldoc.css
+-rw-r--r--   0        0        0     5998 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/rainbow_dash.css
+-rw-r--r--   0        0        0     5492 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/rrt.css
+-rw-r--r--   0        0        0     4979 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/sas.css
+-rw-r--r--   0        0        0     6826 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/solarized-dark.css
+-rw-r--r--   0        0        0     6906 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/solarized-light.css
+-rw-r--r--   0        0        0     6519 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/stata-dark.css
+-rw-r--r--   0        0        0     4373 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/stata-light.css
+-rw-r--r--   0        0        0     4203 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/stata.css
+-rw-r--r--   0        0        0     6460 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/tango.css
+-rw-r--r--   0        0        0     5271 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/trac.css
+-rw-r--r--   0        0        0     5780 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/vim.css
+-rw-r--r--   0        0        0     3008 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/vs.css
+-rw-r--r--   0        0        0     4638 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/css/pygments/xcode.css
+-rw-r--r--   0        0        0     1369 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/favicon/android-chrome-192x192.png
+-rw-r--r--   0        0        0     3279 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/favicon/android-chrome-512x512.png
+-rw-r--r--   0        0        0     1035 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/favicon/apple-touch-icon.png
+-rw-r--r--   0        0        0      246 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/favicon/browserconfig.xml
+-rw-r--r--   0        0        0      260 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/favicon/favicon-16x16.png
+-rw-r--r--   0        0        0      388 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/favicon/favicon-32x32.png
+-rw-r--r--   0        0        0    15086 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/favicon/favicon.ico
+-rw-r--r--   0        0        0     1115 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/favicon/mstile-144x144.png
+-rw-r--r--   0        0        0     1007 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/favicon/mstile-150x150.png
+-rw-r--r--   0        0        0     1022 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/favicon/mstile-310x150.png
+-rw-r--r--   0        0        0     1848 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/favicon/mstile-310x310.png
+-rw-r--r--   0        0        0      843 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/favicon/mstile-70x70.png
+-rw-r--r--   0        0        0     2152 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/favicon/safari-pinned-tab.svg
+-rw-r--r--   0        0        0      426 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/favicon/site.webmanifest
+-rw-r--r--   0        0        0     1655 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/img/creampaper.jpeg
+-rw-r--r--   0        0        0     1074 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/img/fabric_plaid.jpeg
+-rw-r--r--   0        0        0      641 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/img/feather-alt-solid.svg
+-rw-r--r--   0        0        0     1211 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/img/magnifier.png
+-rw-r--r--   0        0        0     3588 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/img/play-button.png
+-rw-r--r--   0        0        0     2523 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/js/application.js
+-rw-r--r--   0        0        0     2366 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/static/js/jquery.mglass.js
+-rw-r--r--   0        0        0      387 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/templates/analytics.html
+-rw-r--r--   0        0        0     3458 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/templates/archives.html
+-rw-r--r--   0        0        0     6642 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/templates/article.html
+-rw-r--r--   0        0        0      334 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/templates/author.html
+-rw-r--r--   0        0        0     1101 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/templates/authors.html
+-rw-r--r--   0        0        0    17926 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/templates/base.html
+-rw-r--r--   0        0        0     1129 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/templates/categories.html
+-rw-r--r--   0        0        0      740 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/templates/category.html
+-rw-r--r--   0        0        0      794 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/templates/index.html
+-rw-r--r--   0        0        0     2360 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/templates/macros.html
+-rw-r--r--   0        0        0      502 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/templates/page.html
+-rw-r--r--   0        0        0     2908 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/templates/pagination.html
+-rw-r--r--   0        0        0     1184 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/templates/period_archives.html
+-rw-r--r--   0        0        0     6562 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/templates/projects.html
+-rw-r--r--   0        0        0      720 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/templates/tag.html
+-rw-r--r--   0        0        0     1551 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/templates/tags.html
+-rw-r--r--   0        0        0      285 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/templates/translations.html
+-rw-r--r--   0        0        0     4970 2024-05-18 05:59:32.174854 plumage-4.0.0/plumage/webassets.py
+-rw-r--r--   0        0        0     3026 2024-05-18 05:59:32.178854 plumage-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0    24429 2024-05-18 05:59:32.178854 plumage-4.0.0/readme.md
+-rw-r--r--   0        0        0    26511 1970-01-01 00:00:00.000000 plumage-4.0.0/PKG-INFO
```

### Comparing `plumage-3.1.0/plumage/__init__.py` & `plumage-4.0.0/plumage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,31 +13,30 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 
 import logging
 from pathlib import Path
 
-__version__ = "3.1.0"
-
+__version__ = "4.0.0"
 """ Examples of valid version strings according :pep:`440#version-scheme`:
 
 .. code-block:: python
     __version__ = "1.2.3.dev1"  # Development release 1
     __version__ = "1.2.3a1"  # Alpha Release 1
     __version__ = "1.2.3b1"  # Beta Release 1
     __version__ = "1.2.3rc1"  # RC Release 1
     __version__ = "1.2.3"  # Final Release
     __version__ = "1.2.3.post1"  # Post Release 1
 """
 
 
 logger = logging.getLogger(__name__)
 
-PLUMAGE_ROOT = Path(__file__).resolve().parent
+PLUMAGE_ROOT: Path = Path(__file__).resolve().parent
 
 
 def get_path() -> str:
     """Returns installation path of the theme.
 
     Used in ``pelicanconf.py`` to dynamiccaly fetch theme location on the system.
     """
```

### Comparing `plumage-3.1.0/plumage/config.py` & `plumage-4.0.0/plumage/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,12 +58,13 @@
     """
     # Defaults code style to Monokai.
     if not conf.get("CODE_STYLE"):
         conf["CODE_STYLE"] = "monokai"
 
     code_style = conf["CODE_STYLE"]
     if code_style not in ALL_CODE_STYLES:
+        msg = f"{code_style} not recognized among {sorted(ALL_CODE_STYLES)}."
         raise ValueError(
-            f"{code_style} not recognized among {sorted(ALL_CODE_STYLES)}."
+            msg,
         )
 
     return conf
```

### Comparing `plumage-3.1.0/plumage/dom_transforms.py` & `plumage-4.0.0/plumage/dom_transforms.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,50 +26,44 @@
     # https://github.com/gawel/pyquery/issues/199
     doc = pq(filename=path)
 
     # Add bootstrap table style to table elements.
     doc("#content table").add_class("table table-hover")
     doc("#content table thead th").attr("scope", "col")
 
-    # Style TOC permalinks produced by Python's markdown.extensions.toc:
-    # https://python-markdown.github.io/extensions/toc/
-    doc(".headerlink").add_class("text-decoration-none small ps-2")
-
     # Make images responsive and styled in article content, but ignore
-    # images in cards (like those from project template), images attached to
-    # links, and emojis rendered as images.
-    main_images_selector = (
-        "#content img:not(.card-img-top):not(.link-icon):not(.emojione)"
-    )
+    # images in cards (like those from project template), and images attached to
+    # links.
+    main_images_selector = "#content img:not(.card-img-top):not(.link-icon)"
     doc(main_images_selector).add_class("img-fluid border rounded shadow")
 
     # Process all images from the main content to create a reduced set with
     # lower dimensions.
-    # XXX Hack to bypass the bug on extenal images from image-process
+    # XXX Hack to bypass the bug on external images from image-process
     # plugin: https://github.com/pelican-plugins/image-process/issues/33
 
     def exclude_external_images(_, this):
         source = urlparse(this.get("src", ""))
         if (source.scheme and BASE_URL.scheme) and (source.netloc != BASE_URL.netloc):
             return False
         return True
 
     doc(main_images_selector).filter(exclude_external_images).add_class(
-        "image-process-article-photo"
+        "image-process-article-photo",
     )
 
     # Style blockquotes in the way Bootstrap does.
     doc("blockquote").add_class(
-        "blockquote border-start border-primary-subtle bg-dark-subtle fs-6 border-4 ps-2"
+        "blockquote border-start border-primary-subtle bg-dark-subtle fs-6 border-4 ps-2",
     )
     doc("blockquote p").add_class("p-2")
 
     # Style code boxes.
     doc(".codehilite, .highlight").add_class(
-        f"pygments-style-{context.get('CODE_STYLE')} rounded shadow-sm mb-3"
+        f"pygments-style-{context.get('CODE_STYLE')} rounded shadow-sm mb-3",
     )
 
     # Style admonitions produced by Python Markdown into alerts.
     doc(".admonition").add_class("alert shadow").attr("role", "alert")
     doc(".admonition-title").add_class("alert-heading h4")
     # Map rST's admonition types to Bootstrap's:
     # https://python-markdown.github.io/extensions/admonition/#syntax
```

### Comparing `plumage-3.1.0/plumage/favicon.py` & `plumage-4.0.0/plumage/favicon.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,11 +49,11 @@
             context_sender=sender,
         )
 
         # Forces the asset to be saved at the root of the output folder.
         # See:
         # https://github.com/getpelican/pelican/blob/8033162ba4393db60791b201fb100d1be0f04431/pelican/contents.py#L55-L59
         static.metadata["save_as"] = asset.name
-        setattr(static, "override_save_as", asset.name)
+        static.override_save_as = asset.name
 
         # Register the new asset along other static files.
         sender.context["staticfiles"].append(static)
```

### Comparing `plumage-3.1.0/plumage/package-lock.json` & `plumage-4.0.0/plumage/package-lock.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875875806051587%*

 * *Differences: {"'packages'": "{'': {'dependencies': {'autoprefixer': '^10.4.19', 'bootstrap': '^5.3.3', "*

 * *               "'postcss': '^8.4.38', 'postcss-cli': '^11.0.0'}}, 'node_modules/autoprefixer': "*

 * *               "{'version': '10.4.19', 'resolved': "*

 * *               "'https://registry.npmjs.org/autoprefixer/-/autoprefixer-10.4.19.tgz', 'integrity': "*

 * *               "'sha512-BaENR2+zBZ8xXhM4pUaKUxlVdxZ0EZhjvbopwnXmxRUfqDmwSpC2lAi/QXvx7NRdPCo1WKEcEF6mV64si1z4Ew==', "*

 * *               "'funding': {insert: [(2, OrderedDict […]*

```diff
@@ -1,17 +1,17 @@
 {
     "lockfileVersion": 3,
     "name": "plumage-webassets-pipeline",
     "packages": {
         "": {
             "dependencies": {
-                "autoprefixer": "^10.4.14",
-                "bootstrap": "^5.3.0",
-                "postcss": "^8.4.24",
-                "postcss-cli": "^10.1.0"
+                "autoprefixer": "^10.4.19",
+                "bootstrap": "^5.3.3",
+                "postcss": "^8.4.38",
+                "postcss-cli": "^11.0.0"
             },
             "name": "plumage-webassets-pipeline"
         },
         "node_modules/@nodelib/fs.scandir": {
             "dependencies": {
                 "@nodelib/fs.stat": "2.0.5",
                 "run-parallel": "^1.1.9"
@@ -49,14 +49,25 @@
                 "url": "https://opencollective.com/popperjs"
             },
             "integrity": "sha512-P1st0aksCrn9sGZhp8GMYwBnQsbvAWsZAX44oXNNvLHGqAOcoVxmjZiohstwQ7SqKnbR47akdNi+uleWD8+g6A==",
             "peer": true,
             "resolved": "https://registry.npmjs.org/@popperjs/core/-/core-2.11.8.tgz",
             "version": "2.11.8"
         },
+        "node_modules/@sindresorhus/merge-streams": {
+            "engines": {
+                "node": ">=18"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-LtoMMhxAlorcGhmFYI+LhPgbPZCkgP6ra1YL604EeF6U98pLlQ3iWIGMdWSC+vWmPBWBNgmDBAhnAobLROJmwg==",
+            "resolved": "https://registry.npmjs.org/@sindresorhus/merge-streams/-/merge-streams-2.3.0.tgz",
+            "version": "2.3.0"
+        },
         "node_modules/ansi-regex": {
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-quJQXlTSUGL2LH9SUXo8VwsY4soanhgo6LNSm84E1LBcE8s3O0wpdiRzyR9z/ZZJMlMWv37qOOb9pdJlMUEKFQ==",
             "resolved": "https://registry.npmjs.org/ansi-regex/-/ansi-regex-5.0.1.tgz",
             "version": "5.0.1"
@@ -88,17 +99,17 @@
             "version": "3.1.3"
         },
         "node_modules/autoprefixer": {
             "bin": {
                 "autoprefixer": "bin/autoprefixer"
             },
             "dependencies": {
-                "browserslist": "^4.21.5",
-                "caniuse-lite": "^1.0.30001464",
-                "fraction.js": "^4.2.0",
+                "browserslist": "^4.23.0",
+                "caniuse-lite": "^1.0.30001599",
+                "fraction.js": "^4.3.7",
                 "normalize-range": "^0.1.2",
                 "picocolors": "^1.0.0",
                 "postcss-value-parser": "^4.2.0"
             },
             "engines": {
                 "node": "^10 || ^12 || >=14"
             },
@@ -106,22 +117,26 @@
                 {
                     "type": "opencollective",
                     "url": "https://opencollective.com/postcss/"
                 },
                 {
                     "type": "tidelift",
                     "url": "https://tidelift.com/funding/github/npm/autoprefixer"
+                },
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-FQzyfOsTlwVzjHxKEqRIAdJx9niO6VCBCoEwax/VLSoQF29ggECcPuBqUMZ+u8jCZOPSy8b8/8KnuFbp0SaFZQ==",
+            "integrity": "sha512-BaENR2+zBZ8xXhM4pUaKUxlVdxZ0EZhjvbopwnXmxRUfqDmwSpC2lAi/QXvx7NRdPCo1WKEcEF6mV64si1z4Ew==",
             "peerDependencies": {
                 "postcss": "^8.1.0"
             },
-            "resolved": "https://registry.npmjs.org/autoprefixer/-/autoprefixer-10.4.14.tgz",
-            "version": "10.4.14"
+            "resolved": "https://registry.npmjs.org/autoprefixer/-/autoprefixer-10.4.19.tgz",
+            "version": "10.4.19"
         },
         "node_modules/binary-extensions": {
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-jDctJ/IVQbZoJykoeHbhXpOlNBqGNcwXJKJog42E5HDPUwQTSdjCHdihjj0DlnheQ7blbT6dHOafNAiS8ooQKA==",
             "resolved": "https://registry.npmjs.org/binary-extensions/-/binary-extensions-2.2.0.tgz",
@@ -134,20 +149,20 @@
                     "url": "https://github.com/sponsors/twbs"
                 },
                 {
                     "type": "opencollective",
                     "url": "https://opencollective.com/bootstrap"
                 }
             ],
-            "integrity": "sha512-UnBV3E3v4STVNQdms6jSGO2CvOkjUMdDAVR2V5N4uCMdaIkaQjbcEAMqRimDHIs4uqBYzDAKCQwCB+97tJgHQw==",
+            "integrity": "sha512-8HLCdWgyoMguSO9o+aH+iuZ+aht+mzW0u3HIMzVu7Srrpv7EBBxTnrFlSCskwdY1+EOFQSm7uMJhNQHkdPcmjg==",
             "peerDependencies": {
-                "@popperjs/core": "^2.11.7"
+                "@popperjs/core": "^2.11.8"
             },
-            "resolved": "https://registry.npmjs.org/bootstrap/-/bootstrap-5.3.0.tgz",
-            "version": "5.3.0"
+            "resolved": "https://registry.npmjs.org/bootstrap/-/bootstrap-5.3.3.tgz",
+            "version": "5.3.3"
         },
         "node_modules/braces": {
             "dependencies": {
                 "fill-range": "^7.0.1"
             },
             "engines": {
                 "node": ">=8"
@@ -157,50 +172,58 @@
             "version": "3.0.2"
         },
         "node_modules/browserslist": {
             "bin": {
                 "browserslist": "cli.js"
             },
             "dependencies": {
-                "caniuse-lite": "^1.0.30001449",
-                "electron-to-chromium": "^1.4.284",
-                "node-releases": "^2.0.8",
-                "update-browserslist-db": "^1.0.10"
+                "caniuse-lite": "^1.0.30001587",
+                "electron-to-chromium": "^1.4.668",
+                "node-releases": "^2.0.14",
+                "update-browserslist-db": "^1.0.13"
             },
             "engines": {
                 "node": "^6 || ^7 || ^8 || ^9 || ^10 || ^11 || ^12 || >=13.7"
             },
             "funding": [
                 {
                     "type": "opencollective",
                     "url": "https://opencollective.com/browserslist"
                 },
                 {
                     "type": "tidelift",
                     "url": "https://tidelift.com/funding/github/npm/browserslist"
+                },
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-tUkiguQGW7S3IhB7N+c2MV/HZPSCPAAiYBZXLsBhFB/PCy6ZKKsZrmBayHV9fdGV/ARIfJ14NkxKzRDjvp7L6w==",
-            "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.21.5.tgz",
-            "version": "4.21.5"
+            "integrity": "sha512-QW8HiM1shhT2GuzkvklfjcKDiWFXHOeFCIA/huJPwHsslwcydgk7X+z2zXpEijP98UCY7HbubZt5J2Zgvf0CaQ==",
+            "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.23.0.tgz",
+            "version": "4.23.0"
         },
         "node_modules/caniuse-lite": {
             "funding": [
                 {
                     "type": "opencollective",
                     "url": "https://opencollective.com/browserslist"
                 },
                 {
                     "type": "tidelift",
                     "url": "https://tidelift.com/funding/github/npm/caniuse-lite"
+                },
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-oww27MtUmusatpRpCGSOneQk2/l5czXANDSFvsc7VuOQ86s3ANhZetpwXNf1zY/zdfP63Xvjz325DAdAoES13g==",
-            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001464.tgz",
-            "version": "1.0.30001464"
+            "integrity": "sha512-cjUJTQkk9fQlJR2s4HMuPMvTiRggl0rAVMtthQuyOlDWuqHXqN8azLq+pi8B2TjwKJ32diHjUqRIKeFX4z1FoA==",
+            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001608.tgz",
+            "version": "1.0.30001608"
         },
         "node_modules/chokidar": {
             "dependencies": {
                 "anymatch": "~3.1.2",
                 "braces": "~3.0.2",
                 "glob-parent": "~5.1.2",
                 "is-binary-path": "~2.1.0",
@@ -257,29 +280,18 @@
             "engines": {
                 "node": ">= 0.6.0"
             },
             "integrity": "sha512-JeMq7fEshyepOWDfcfHK06N3MhyPhz++vtqWhMT5O9A3K42rdsEDpfdVqjaqaAhsw6a+ZqeDvQVtD0hFHQWrzg==",
             "resolved": "https://registry.npmjs.org/dependency-graph/-/dependency-graph-0.11.0.tgz",
             "version": "0.11.0"
         },
-        "node_modules/dir-glob": {
-            "dependencies": {
-                "path-type": "^4.0.0"
-            },
-            "engines": {
-                "node": ">=8"
-            },
-            "integrity": "sha512-WkrWp9GR4KXfKGYzOLmTuGVi1UWFfws377n9cc55/tb6DuqyF6pcQ5AbiHEshaDpY9v6oaSr2XCDidGmMwdzIA==",
-            "resolved": "https://registry.npmjs.org/dir-glob/-/dir-glob-3.0.1.tgz",
-            "version": "3.0.1"
-        },
         "node_modules/electron-to-chromium": {
-            "integrity": "sha512-Uk7C+7aPBryUR1Fwvk9VmipBcN9fVsqBO57jV2ZjTm+IZ6BMNqu7EDVEg2HxCNufk6QcWlFsBkhQyQroB2VWKw==",
-            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.302.tgz",
-            "version": "1.4.302"
+            "integrity": "sha512-gUI9nhI2iBGF0OaYYLKOaOtliFMl+Bt1rY7VmEjwxOxqoYLub/D9xmduPEhbw2imE6gYkJKhIE5it+KE2ulVxQ==",
+            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.733.tgz",
+            "version": "1.4.733"
         },
         "node_modules/emoji-regex": {
             "integrity": "sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==",
             "resolved": "https://registry.npmjs.org/emoji-regex/-/emoji-regex-8.0.0.tgz",
             "version": "8.0.0"
         },
         "node_modules/escalade": {
@@ -297,25 +309,25 @@
                 "glob-parent": "^5.1.2",
                 "merge2": "^1.3.0",
                 "micromatch": "^4.0.4"
             },
             "engines": {
                 "node": ">=8.6.0"
             },
-            "integrity": "sha512-DVj4CQIYYow0BlaelwK1pHl5n5cRSJfM60UA0zK891sVInoPri2Ekj7+e1CT3/3qxXenpI+nBBmQAcJPJgaj4w==",
-            "resolved": "https://registry.npmjs.org/fast-glob/-/fast-glob-3.2.12.tgz",
-            "version": "3.2.12"
+            "integrity": "sha512-oX2ruAFQwf/Orj8m737Y5adxDQO0LAB7/S5MnxCdTNDd4p6BsyIVsv9JQsATbTSq8KHRpLwIHbVlUNatxd+1Ow==",
+            "resolved": "https://registry.npmjs.org/fast-glob/-/fast-glob-3.3.2.tgz",
+            "version": "3.3.2"
         },
         "node_modules/fastq": {
             "dependencies": {
                 "reusify": "^1.0.4"
             },
-            "integrity": "sha512-wBrocU2LCXXa+lWBt8RoIRD89Fi8OdABODa/kEnyeyjS5aZO5/GNvI5sEINADqP/h8M29UHTHUb53sUu5Ihqdw==",
-            "resolved": "https://registry.npmjs.org/fastq/-/fastq-1.15.0.tgz",
-            "version": "1.15.0"
+            "integrity": "sha512-sRVD3lWVIXWg6By68ZN7vho9a1pQcN/WBFaAAsDDFzlJjvoGx0P8z7V1t72grFJfJhu3YPZBuu25f7Kaw2jN1w==",
+            "resolved": "https://registry.npmjs.org/fastq/-/fastq-1.17.1.tgz",
+            "version": "1.17.1"
         },
         "node_modules/fill-range": {
             "dependencies": {
                 "to-regex-range": "^5.0.1"
             },
             "engines": {
                 "node": ">=8"
@@ -326,19 +338,19 @@
         },
         "node_modules/fraction.js": {
             "engines": {
                 "node": "*"
             },
             "funding": {
                 "type": "patreon",
-                "url": "https://www.patreon.com/infusion"
+                "url": "https://github.com/sponsors/rawify"
             },
-            "integrity": "sha512-MhLuK+2gUcnZe8ZHlaaINnQLl0xRIGRfcGk2yl8xoQAfHrSsL3rYu6FCmBdkdbhc9EPlwyGHewaRsvwRMJtAlA==",
-            "resolved": "https://registry.npmjs.org/fraction.js/-/fraction.js-4.2.0.tgz",
-            "version": "4.2.0"
+            "integrity": "sha512-ZsDfxO51wGAXREY55a7la9LScWpwv9RxIrYABrlvOFBlH/ShPnrtsXeuUIfXKKOVicNxQ+o8JTbJvjS4M89yew==",
+            "resolved": "https://registry.npmjs.org/fraction.js/-/fraction.js-4.3.7.tgz",
+            "version": "4.3.7"
         },
         "node_modules/fs-extra": {
             "dependencies": {
                 "graceful-fs": "^4.2.0",
                 "jsonfile": "^6.0.1",
                 "universalify": "^2.0.0"
             },
@@ -390,53 +402,43 @@
             },
             "integrity": "sha512-AOIgSQCepiJYwP3ARnGx+5VnTu2HBYdzbGP45eLw1vr3zB3vZLeyed1sC9hnbcOc9/SrMyM5RPQrkGz4aS9Zow==",
             "resolved": "https://registry.npmjs.org/glob-parent/-/glob-parent-5.1.2.tgz",
             "version": "5.1.2"
         },
         "node_modules/globby": {
             "dependencies": {
-                "dir-glob": "^3.0.1",
-                "fast-glob": "^3.2.11",
-                "ignore": "^5.2.0",
-                "merge2": "^1.4.1",
-                "slash": "^4.0.0"
+                "@sindresorhus/merge-streams": "^2.1.0",
+                "fast-glob": "^3.3.2",
+                "ignore": "^5.2.4",
+                "path-type": "^5.0.0",
+                "slash": "^5.1.0",
+                "unicorn-magic": "^0.1.0"
             },
             "engines": {
-                "node": "^12.20.0 || ^14.13.1 || >=16.0.0"
+                "node": ">=18"
             },
             "funding": {
                 "url": "https://github.com/sponsors/sindresorhus"
             },
-            "integrity": "sha512-8krCNHXvlCgHDpegPzleMq07yMYTO2sXKASmZmquEYWEmCx6J5UTRbp5RwMJkTJGtcQ44YpiUYUiN0b9mzy8Bw==",
-            "resolved": "https://registry.npmjs.org/globby/-/globby-13.1.3.tgz",
-            "version": "13.1.3"
-        },
-        "node_modules/globby/node_modules/slash": {
-            "engines": {
-                "node": ">=12"
-            },
-            "funding": {
-                "url": "https://github.com/sponsors/sindresorhus"
-            },
-            "integrity": "sha512-3dOsAHXXUkQTpOYcoAxLIorMTp4gIQr5IW3iVb7A7lFIp0VHhnynm9izx6TssdrIcVIESAlVjtnO2K8bg+Coew==",
-            "resolved": "https://registry.npmjs.org/slash/-/slash-4.0.0.tgz",
-            "version": "4.0.0"
+            "integrity": "sha512-jOMLD2Z7MAhyG8aJpNOpmziMOP4rPLcc95oQPKXBazW82z+CEgPFBQvEpRUa1KeIMUJo4Wsm+q6uzO/Q/4BksQ==",
+            "resolved": "https://registry.npmjs.org/globby/-/globby-14.0.1.tgz",
+            "version": "14.0.1"
         },
         "node_modules/graceful-fs": {
             "integrity": "sha512-9ByhssR2fPVsNZj478qUUbKfmL0+t5BDVyjShtyZZLiK7ZDAArFFfopyOTj0M05wE2tJPisA4iTnnXl2YoPvOA==",
             "resolved": "https://registry.npmjs.org/graceful-fs/-/graceful-fs-4.2.10.tgz",
             "version": "4.2.10"
         },
         "node_modules/ignore": {
             "engines": {
                 "node": ">= 4"
             },
-            "integrity": "sha512-MAb38BcSbH0eHNBxn7ql2NH/kX33OkB3lZ1BNdh7ENeRChHTYsTvWrMubiIAMNS2llXEEgZ1MUOBtXChP3kaFQ==",
-            "resolved": "https://registry.npmjs.org/ignore/-/ignore-5.2.4.tgz",
-            "version": "5.2.4"
+            "integrity": "sha512-5Fytz/IraMjqpwfd34ke28PTVMjZjJG2MPn5t7OE4eUCUNf8BAa7b5WUS9/Qvr6mwOQS7Mk6vdsMno5he+T8Xw==",
+            "resolved": "https://registry.npmjs.org/ignore/-/ignore-5.3.1.tgz",
+            "version": "5.3.1"
         },
         "node_modules/is-binary-path": {
             "dependencies": {
                 "binary-extensions": "^2.0.0"
             },
             "engines": {
                 "node": ">=8"
@@ -489,19 +491,22 @@
                 "graceful-fs": "^4.1.6"
             },
             "resolved": "https://registry.npmjs.org/jsonfile/-/jsonfile-6.1.0.tgz",
             "version": "6.1.0"
         },
         "node_modules/lilconfig": {
             "engines": {
-                "node": ">=10"
+                "node": ">=14"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/antonk52"
             },
-            "integrity": "sha512-9JROoBW7pobfsx+Sq2JsASvCo6Pfo6WWoUW79HuB1BCoBXD4PLWJPqDF6fNj67pqBYTbAHkE57M1kS/+L1neOg==",
-            "resolved": "https://registry.npmjs.org/lilconfig/-/lilconfig-2.0.6.tgz",
-            "version": "2.0.6"
+            "integrity": "sha512-O18pf7nyvHTckunPWCV1XUNXU1piu01y2b7ATJ0ppkUkk8ocqVWBrYjJBCwHDjD/ZWcfyrA0P4gKhzWGi5EINQ==",
+            "resolved": "https://registry.npmjs.org/lilconfig/-/lilconfig-3.1.1.tgz",
+            "version": "3.1.1"
         },
         "node_modules/merge2": {
             "engines": {
                 "node": ">= 8"
             },
             "integrity": "sha512-8q7VEgMJW4J8tcfVPy8g09NcQwZdbwFEqhe/WZkoIzjn/3TGDwtOCYtXGxA3O8tPzpczCCDgv+P2P5y00ZJOOg==",
             "resolved": "https://registry.npmjs.org/merge2/-/merge2-1.4.1.tgz",
@@ -528,22 +533,22 @@
             },
             "funding": [
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-BGcqMMJuToF7i1rt+2PWSNVnWIkGCU78jBG3RxO/bZlnZPK2Cmi2QaffxGO/2RvWi9sL+FAiRiXMgsyxQ1DIDA==",
-            "resolved": "https://registry.npmjs.org/nanoid/-/nanoid-3.3.6.tgz",
-            "version": "3.3.6"
+            "integrity": "sha512-eSRppjcPIatRIMC1U6UngP8XFcz8MQWGQdt1MTBQ7NaAmvXDfvNxbvWV3x2y6CdEUciCSsDHDQZbhYaB8QEo2g==",
+            "resolved": "https://registry.npmjs.org/nanoid/-/nanoid-3.3.7.tgz",
+            "version": "3.3.7"
         },
         "node_modules/node-releases": {
-            "integrity": "sha512-5GFldHPXVG/YZmFzJvKK2zDSzPKhEp0+ZR5SVaoSag9fsL5YgHbUHDfnG5494ISANDcK4KwPXAx2xqVEydmd7w==",
-            "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-2.0.10.tgz",
-            "version": "2.0.10"
+            "integrity": "sha512-y10wOWt8yZpqXmOgRo77WaHEmhYQYGNA6y421PKsKYWEK8aW+cqAphborZDhqfyKrbZEN92CN1X2KbafY2s7Yw==",
+            "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-2.0.14.tgz",
+            "version": "2.0.14"
         },
         "node_modules/normalize-path": {
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-6eZs5Ls3WtCisHWp9S2GUy8dqkpGi4BVSz3GaqiE6ezub0512ESztXUwUB6C6IKbQkY2Pnb/mD4WYojCRwcwLA==",
             "resolved": "https://registry.npmjs.org/normalize-path/-/normalize-path-3.0.0.tgz",
@@ -555,19 +560,22 @@
             },
             "integrity": "sha512-bdok/XvKII3nUpklnV6P2hxtMNrCboOjAcyBuQnWEhO665FwrSNRxU+AqpsyvO6LgGYPspN+lu5CLtw4jPRKNA==",
             "resolved": "https://registry.npmjs.org/normalize-range/-/normalize-range-0.1.2.tgz",
             "version": "0.1.2"
         },
         "node_modules/path-type": {
             "engines": {
-                "node": ">=8"
+                "node": ">=12"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
             },
-            "integrity": "sha512-gDKb8aZMDeD/tZWs9P6+q0J9Mwkdl6xMV8TjnGP3qJVJ06bdMgkbBlLU8IdfOsIsFz2BW1rNVT3XuNEl8zPAvw==",
-            "resolved": "https://registry.npmjs.org/path-type/-/path-type-4.0.0.tgz",
-            "version": "4.0.0"
+            "integrity": "sha512-5HviZNaZcfqP95rwpv+1HDgUamezbqdSYTyzjTvwtJSnIH+3vnbmWsItli8OFEndS984VT55M3jduxZbX351gg==",
+            "resolved": "https://registry.npmjs.org/path-type/-/path-type-5.0.0.tgz",
+            "version": "5.0.0"
         },
         "node_modules/picocolors": {
             "integrity": "sha512-1fygroTLlHu66zi26VoTDv8yRgm0Fccecssto+MhsZ0D/DGW2sm8E8AjW7NU5VVTRt5GxbeZ5qBuJr+HyLYkjQ==",
             "resolved": "https://registry.npmjs.org/picocolors/-/picocolors-1.0.0.tgz",
             "version": "1.0.0"
         },
         "node_modules/picomatch": {
@@ -587,17 +595,17 @@
             },
             "integrity": "sha512-udgsAY+fTnvv7kI7aaxbqwWNb0AHiB0qBO89PZKPkoTmGOgdbrHDKD+0B2X4uTfJ/FT1R09r9gTsjUjNJotuog==",
             "resolved": "https://registry.npmjs.org/pify/-/pify-2.3.0.tgz",
             "version": "2.3.0"
         },
         "node_modules/postcss": {
             "dependencies": {
-                "nanoid": "^3.3.6",
+                "nanoid": "^3.3.7",
                 "picocolors": "^1.0.0",
-                "source-map-js": "^1.0.2"
+                "source-map-js": "^1.2.0"
             },
             "engines": {
                 "node": "^10 || ^12 || >=14"
             },
             "funding": [
                 {
                     "type": "opencollective",
@@ -608,73 +616,79 @@
                     "url": "https://tidelift.com/funding/github/npm/postcss"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-M0RzbcI0sO/XJNucsGjvWU9ERWxb/ytp1w6dKtxTKgixdtQDq4rmx/g8W1hnaheq9jgwL/oyEdH5Bc4WwJKMqg==",
-            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.24.tgz",
-            "version": "8.4.24"
+            "integrity": "sha512-Wglpdk03BSfXkHoQa3b/oulrotAkwrlLDRSOb9D0bN86FdRyE9lppSp33aHNPgBa0JKCoB+drFLZkQoRRYae5A==",
+            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.38.tgz",
+            "version": "8.4.38"
         },
         "node_modules/postcss-cli": {
             "bin": {
                 "postcss": "index.js"
             },
             "dependencies": {
                 "chokidar": "^3.3.0",
                 "dependency-graph": "^0.11.0",
                 "fs-extra": "^11.0.0",
                 "get-stdin": "^9.0.0",
-                "globby": "^13.0.0",
+                "globby": "^14.0.0",
                 "picocolors": "^1.0.0",
-                "postcss-load-config": "^4.0.0",
+                "postcss-load-config": "^5.0.0",
                 "postcss-reporter": "^7.0.0",
                 "pretty-hrtime": "^1.0.3",
                 "read-cache": "^1.0.0",
                 "slash": "^5.0.0",
                 "yargs": "^17.0.0"
             },
             "engines": {
-                "node": ">=14"
+                "node": ">=18"
             },
-            "integrity": "sha512-Zu7PLORkE9YwNdvOeOVKPmWghprOtjFQU3srMUGbdz3pHJiFh7yZ4geiZFMkjMfB0mtTFR3h8RemR62rPkbOPA==",
+            "integrity": "sha512-xMITAI7M0u1yolVcXJ9XTZiO9aO49mcoKQy6pCDFdMh9kGqhzLVpWxeD/32M/QBmkhcGypZFFOLNLmIW4Pg4RA==",
             "peerDependencies": {
                 "postcss": "^8.0.0"
             },
-            "resolved": "https://registry.npmjs.org/postcss-cli/-/postcss-cli-10.1.0.tgz",
-            "version": "10.1.0"
+            "resolved": "https://registry.npmjs.org/postcss-cli/-/postcss-cli-11.0.0.tgz",
+            "version": "11.0.0"
         },
         "node_modules/postcss-load-config": {
             "dependencies": {
-                "lilconfig": "^2.0.5",
-                "yaml": "^2.1.1"
+                "lilconfig": "^3.0.0",
+                "yaml": "^2.3.4"
             },
             "engines": {
-                "node": ">= 14"
+                "node": ">= 18"
             },
-            "funding": {
-                "type": "opencollective",
-                "url": "https://opencollective.com/postcss/"
-            },
-            "integrity": "sha512-vEJIc8RdiBRu3oRAI0ymerOn+7rPuMvRXslTvZUKZonDHFIczxztIyJ1urxM1x9JXEikvpWWTUUqal5j/8QgvA==",
+            "funding": [
+                {
+                    "type": "opencollective",
+                    "url": "https://opencollective.com/postcss/"
+                },
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/ai"
+                }
+            ],
+            "integrity": "sha512-90pBBI5apUVruIEdCxZic93Wm+i9fTrp7TXbgdUCH+/L+2WnfpITSpq5dFU/IPvbv7aNiMlQISpUkAm3fEcvgQ==",
             "peerDependencies": {
-                "postcss": ">=8.0.9",
-                "ts-node": ">=9.0.0"
+                "jiti": ">=1.21.0",
+                "postcss": ">=8.0.9"
             },
             "peerDependenciesMeta": {
-                "postcss": {
+                "jiti": {
                     "optional": true
                 },
-                "ts-node": {
+                "postcss": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/postcss-load-config/-/postcss-load-config-4.0.1.tgz",
-            "version": "4.0.1"
+            "resolved": "https://registry.npmjs.org/postcss-load-config/-/postcss-load-config-5.0.3.tgz",
+            "version": "5.0.3"
         },
         "node_modules/postcss-reporter": {
             "dependencies": {
                 "picocolors": "^1.0.0",
                 "thenby": "^1.3.4"
             },
             "engines": {
@@ -784,25 +798,25 @@
         "node_modules/slash": {
             "engines": {
                 "node": ">=14.16"
             },
             "funding": {
                 "url": "https://github.com/sponsors/sindresorhus"
             },
-            "integrity": "sha512-n6KkmvKS0623igEVj3FF0OZs1gYYJ0o0Hj939yc1fyxl2xt+xYpLnzJB6xBSqOfV9ZFLEWodBBN/heZJahuIJQ==",
-            "resolved": "https://registry.npmjs.org/slash/-/slash-5.0.0.tgz",
-            "version": "5.0.0"
+            "integrity": "sha512-ZA6oR3T/pEyuqwMgAKT0/hAv8oAXckzbkmR0UkUosQ+Mc4RxGoJkRmwHgHufaenlyAgE1Mxgpdcrf75y6XcnDg==",
+            "resolved": "https://registry.npmjs.org/slash/-/slash-5.1.0.tgz",
+            "version": "5.1.0"
         },
         "node_modules/source-map-js": {
             "engines": {
                 "node": ">=0.10.0"
             },
-            "integrity": "sha512-R0XvVJ9WusLiqTCEiGCmICCMplcCkIwwR11mOSD9CR5u+IXYdiseeEuXCVAjS54zqwkLcPNnmU4OeJ6tUrWhDw==",
-            "resolved": "https://registry.npmjs.org/source-map-js/-/source-map-js-1.0.2.tgz",
-            "version": "1.0.2"
+            "integrity": "sha512-itJW8lvSA0TXEphiRoawsCksnlf8SyvmFzIhltqAHluXd88pkCd+cXJVHTDwdCr0IzwptSm035IHQktUu1QUMg==",
+            "resolved": "https://registry.npmjs.org/source-map-js/-/source-map-js-1.2.0.tgz",
+            "version": "1.2.0"
         },
         "node_modules/string-width": {
             "dependencies": {
                 "emoji-regex": "^8.0.0",
                 "is-fullwidth-code-point": "^3.0.0",
                 "strip-ansi": "^6.0.1"
             },
@@ -836,46 +850,61 @@
             "engines": {
                 "node": ">=8.0"
             },
             "integrity": "sha512-65P7iz6X5yEr1cwcgvQxbbIw7Uk3gOy5dIdtZ4rDveLqhrdJP+Li/Hx6tyK0NEb+2GCyneCMJiGqrADCSNk8sQ==",
             "resolved": "https://registry.npmjs.org/to-regex-range/-/to-regex-range-5.0.1.tgz",
             "version": "5.0.1"
         },
+        "node_modules/unicorn-magic": {
+            "engines": {
+                "node": ">=18"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-lRfVq8fE8gz6QMBuDM6a+LO3IAzTi05H6gCVaUpir2E1Rwpo4ZUog45KpNXKC/Mn3Yb9UDuHumeFTo9iV/D9FQ==",
+            "resolved": "https://registry.npmjs.org/unicorn-magic/-/unicorn-magic-0.1.0.tgz",
+            "version": "0.1.0"
+        },
         "node_modules/universalify": {
             "engines": {
                 "node": ">= 10.0.0"
             },
             "integrity": "sha512-hAZsKq7Yy11Zu1DE0OzWjw7nnLZmJZYTDZZyEFHZdUhV8FkH5MCfoU1XMaxXovpyW5nq5scPqq0ZDP9Zyl04oQ==",
             "resolved": "https://registry.npmjs.org/universalify/-/universalify-2.0.0.tgz",
             "version": "2.0.0"
         },
         "node_modules/update-browserslist-db": {
             "bin": {
-                "browserslist-lint": "cli.js"
+                "update-browserslist-db": "cli.js"
             },
             "dependencies": {
                 "escalade": "^3.1.1",
                 "picocolors": "^1.0.0"
             },
             "funding": [
                 {
                     "type": "opencollective",
                     "url": "https://opencollective.com/browserslist"
                 },
                 {
                     "type": "tidelift",
                     "url": "https://tidelift.com/funding/github/npm/browserslist"
+                },
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-OztqDenkfFkbSG+tRxBeAnCVPckDBcvibKd35yDONx6OU8N7sqgwc7rCbkJ/WcYtVRZ4ba68d6byhC21GFh7sQ==",
+            "integrity": "sha512-xebP81SNcPuNpPP3uzeW1NYXxI3rxyJzF3pD6sH4jE7o/IX+WtSpwnVU+qIsDPyk0d3hmFQ7mjqc6AtV604hbg==",
             "peerDependencies": {
                 "browserslist": ">= 4.21.0"
             },
-            "resolved": "https://registry.npmjs.org/update-browserslist-db/-/update-browserslist-db-1.0.10.tgz",
-            "version": "1.0.10"
+            "resolved": "https://registry.npmjs.org/update-browserslist-db/-/update-browserslist-db-1.0.13.tgz",
+            "version": "1.0.13"
         },
         "node_modules/wrap-ansi": {
             "dependencies": {
                 "ansi-styles": "^4.0.0",
                 "string-width": "^4.1.0",
                 "strip-ansi": "^6.0.0"
             },
@@ -894,20 +923,23 @@
                 "node": ">=10"
             },
             "integrity": "sha512-0pfFzegeDWJHJIAmTLRP2DwHjdF5s7jo9tuztdQxAhINCdvS+3nGINqPd00AphqJR/0LhANUS6/+7SCb98YOfA==",
             "resolved": "https://registry.npmjs.org/y18n/-/y18n-5.0.8.tgz",
             "version": "5.0.8"
         },
         "node_modules/yaml": {
+            "bin": {
+                "yaml": "bin.mjs"
+            },
             "engines": {
                 "node": ">= 14"
             },
-            "integrity": "sha512-CBKFWExMn46Foo4cldiChEzn7S7SRV+wqiluAb6xmueD/fGyRHIhX8m14vVGgeFWjN540nKCNVj6P21eQjgTuA==",
-            "resolved": "https://registry.npmjs.org/yaml/-/yaml-2.2.2.tgz",
-            "version": "2.2.2"
+            "integrity": "sha512-pIXzoImaqmfOrL7teGUBt/T7ZDnyeGBWyXQBvOVhLkWLN37GXv8NMLK406UY6dS51JfcQHsmcW5cJ441bHg6Lg==",
+            "resolved": "https://registry.npmjs.org/yaml/-/yaml-2.4.1.tgz",
+            "version": "2.4.1"
         },
         "node_modules/yargs": {
             "dependencies": {
                 "cliui": "^8.0.1",
                 "escalade": "^3.1.1",
                 "get-caller-file": "^2.0.5",
                 "require-directory": "^2.1.1",
```

### Comparing `plumage-3.1.0/plumage/static/css/code.scss` & `plumage-4.0.0/plumage/static/css/code.scss`

 * *Files identical despite different names*

### Comparing `plumage-3.1.0/plumage/static/css/main.scss` & `plumage-4.0.0/plumage/static/css/main.scss`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,32 @@
-// Import thw whole Bootstrap framework.
+// Import the whole Bootstrap framework.
 // See: https://getbootstrap.com/docs/5.3/customize/sass/#importing
 @import "../../node_modules/bootstrap/scss/bootstrap";
-// Custom Plumage CSS is below.
 
+// Custom Plumage CSS is below.
 // TODO: replace hard-coded styling with bootstrap's own class names for consistency.
 
-
 html {
   background: rgb(236, 236, 236) url("/theme/img/fabric_plaid.jpeg");
   box-shadow: inset 0 1rem 6rem -2rem rgba(0, 0, 0, 0.5);
 }
 
 
 a {
   // Do not underline links but on hover.
   @extend .text-decoration-none;
 
   &:hover {
     @extend .text-decoration-underline;
   }
 
-  /* Style title headers anchors produced by Python's Markdown module. See:
-   * https://python-markdown.github.io/extensions/toc/#usage
-   */
+  // Style title headers anchors
   &.headerlink {
     visibility: hidden;
+    @extend .fs-4;
 
     @each $tag in 'h1',
     'h2',
     'h3',
     'h4',
     'h5',
     'h6',
@@ -37,38 +35,28 @@
         visibility: visible !important;
       }
     }
   }
 }
 
 
-/* Style to support pymdown-extensions' emoji:
- * https://facelessuser.github.io/pymdown-extensions/extensions/emoji/#default-emoji-generators
- */
-img.emojione {
-  $size: 1.3rem;
-  height: $size;
-  width: $size;
-}
-
-
 .avatar-container {
   $size: 6rem;
   height: $size;
   perspective: 600;
   position: relative;
   width: $size;
   z-index: 10;
 
   .avatar {
     $size: 100%;
     height: $size;
     position: absolute;
     transform-style: preserve-3d;
-    transition: all 0.3s ease-in-out;
+    transition: all 0.2s ease-in-out;
     width: $size;
 
     .side {
       $size: 100%;
       backface-visibility: hidden;
 
       border: solid 0.2rem white {
@@ -85,31 +73,29 @@
     .back {
       background-image: linear-gradient(#eee, #ddd);
       box-shadow: inset 0 0 1.5rem rgba(0, 0, 0, 0.1);
     }
 
     .side:hover,
     .back {
-      border-color: #005580;
+      @extend .border-primary;
     }
 
     &.animate:hover,
     &.animate .back {
       transform: rotateY(180deg);
     }
   }
 }
 
 
-/* Custom styling of the DOM produced by Stork's default Javascript.
- * See: https://github.com/jameslittle230/stork/blob/master/js/entityDom.ts
- *
- * All customization is performed by aliasing the default Stork classes to Bootstrap's own default classes.
- */
-
+// Custom styling of the DOM produced by Stork's default Javascript.
+// See: https://github.com/jameslittle230/stork/blob/master/js/entityDom.ts
+//
+// All customization is performed by aliasing the default Stork classes to Bootstrap's own default classes.
 .stork-close-button {
   // Place the reset button on the right side of the search box.
   @extend .position-absolute, .top-50, .end-0, .translate-middle-y;
   // Use Bootstrap's default SVG-based close button.
   @extend .btn-close;
   // Shape the button into a circle.
   @extend .rounded-circle;
@@ -212,25 +198,68 @@
   .stork-attribution {
     // Silence the search engine self-ads.
     @extend .d-none;
   }
 }
 
 
+// Custom style for the article's right sidebar
+.list-group.list-group-flush {
+  // Reduce text size and weight
+  @extend .small, .fw-light;
+  // Add a thick border on the left side of the sidebar
+  @extend .border-start, .border-5;
+
+  .list-group-item {
+    // Reduce text color
+    @extend .text-body-secondary;
+    // Remove the default white background
+    @extend .bg-transparent;
+    // Remove the default border
+    @extend .border-0;
+    // Aligns vertical padding to horizontal padding to double the top and bottom padding
+    --bs-list-group-item-padding-y: var(--bs-list-group-item-padding-x);
+
+    // Align the bottom of the sidebar with the bottom of the last item.
+    &:last-child {
+      @extend .pb-0;
+    }
+  }
+
+  // Do not underline the older and newer article links
+  .nav a:hover {
+    @extend .text-decoration-none;
+  }
+
+}
+
+
 h1,
 h2 {
   text-shadow: 0.1rem 0.1rem 0.1rem #ddd;
 }
 
 
-/* Typogrify's ampersands */
+// Typogrify's ampersands
 span.amp {
   font-family: cursive;
 }
 
+.badge {
+  @extend .btn, .btn-light, .rounded-pill;
+
+  &.category {
+    @extend .bg-primary-subtle, .text-primary-emphasis;
+  }
+
+  &.tag {
+    @extend .bg-secondary-subtle, .text-secondary-emphasis;
+  }
+}
+
 
 .card .corner-banner {
   font-size: 1rem;
   position: absolute;
   right: -4rem;
   text-align: center;
   top: 1rem;
```

### Comparing `plumage-3.1.0/plumage/static/css/mglass.scss` & `plumage-4.0.0/plumage/static/css/mglass.scss`

 * *Files identical despite different names*

### Comparing `plumage-3.1.0/plumage/static/css/pygments/abap.css` & `plumage-4.0.0/plumage/static/css/pygments/abap.css`

 * *Files 14% similar despite different names*

```diff
@@ -1,116 +1,96 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-.pygments-style-abap .hll { background-color: #ffc; }
-
-.pygments-style-abap {
-  background: #fff;
-}
-
-.pygments-style-abap .c {
-  color: #888;
-  font-style: italic;
-} /* Comment */
-.pygments-style-abap .err { color: #f00; } /* Error */
-.pygments-style-abap .k { color: #00f; } /* Keyword */
-.pygments-style-abap .n { color: #000; } /* Name */
-.pygments-style-abap .ch {
-  color: #888;
-  font-style: italic;
-} /* Comment.Hashbang */
-.pygments-style-abap .cm {
-  color: #888;
-  font-style: italic;
-} /* Comment.Multiline */
-.pygments-style-abap .cp {
-  color: #888;
-  font-style: italic;
-} /* Comment.Preproc */
-.pygments-style-abap .cpf {
-  color: #888;
-  font-style: italic;
-} /* Comment.PreprocFile */
-.pygments-style-abap .c1 {
-  color: #888;
-  font-style: italic;
-} /* Comment.Single */
-.pygments-style-abap .cs {
-  color: #888;
-  font-style: italic;
-} /* Comment.Special */
-.pygments-style-abap .kc { color: #00f; } /* Keyword.Constant */
-.pygments-style-abap .kd { color: #00f; } /* Keyword.Declaration */
-.pygments-style-abap .kn { color: #00f; } /* Keyword.Namespace */
-.pygments-style-abap .kp { color: #00f; } /* Keyword.Pseudo */
-.pygments-style-abap .kr { color: #00f; } /* Keyword.Reserved */
-.pygments-style-abap .kt { color: #00f; } /* Keyword.Type */
-.pygments-style-abap .m { color: #3af; } /* Literal.Number */
-.pygments-style-abap .s { color: #5a2; } /* Literal.String */
-.pygments-style-abap .na { color: #000; } /* Name.Attribute */
-.pygments-style-abap .nb { color: #000; } /* Name.Builtin */
-.pygments-style-abap .nc { color: #000; } /* Name.Class */
-.pygments-style-abap .no { color: #000; } /* Name.Constant */
-.pygments-style-abap .nd { color: #000; } /* Name.Decorator */
-.pygments-style-abap .ni { color: #000; } /* Name.Entity */
-.pygments-style-abap .ne { color: #000; } /* Name.Exception */
-.pygments-style-abap .nf { color: #000; } /* Name.Function */
-.pygments-style-abap .nl { color: #000; } /* Name.Label */
-.pygments-style-abap .nn { color: #000; } /* Name.Namespace */
-.pygments-style-abap .nx { color: #000; } /* Name.Other */
-.pygments-style-abap .py { color: #000; } /* Name.Property */
-.pygments-style-abap .nt { color: #000; } /* Name.Tag */
-.pygments-style-abap .nv { color: #000; } /* Name.Variable */
-.pygments-style-abap .ow { color: #00f; } /* Operator.Word */
-.pygments-style-abap .mb { color: #3af; } /* Literal.Number.Bin */
-.pygments-style-abap .mf { color: #3af; } /* Literal.Number.Float */
-.pygments-style-abap .mh { color: #3af; } /* Literal.Number.Hex */
-.pygments-style-abap .mi { color: #3af; } /* Literal.Number.Integer */
-.pygments-style-abap .mo { color: #3af; } /* Literal.Number.Oct */
-.pygments-style-abap .sa { color: #5a2; } /* Literal.String.Affix */
-.pygments-style-abap .sb { color: #5a2; } /* Literal.String.Backtick */
-.pygments-style-abap .sc { color: #5a2; } /* Literal.String.Char */
-.pygments-style-abap .dl { color: #5a2; } /* Literal.String.Delimiter */
-.pygments-style-abap .sd { color: #5a2; } /* Literal.String.Doc */
-.pygments-style-abap .s2 { color: #5a2; } /* Literal.String.Double */
-.pygments-style-abap .se { color: #5a2; } /* Literal.String.Escape */
-.pygments-style-abap .sh { color: #5a2; } /* Literal.String.Heredoc */
-.pygments-style-abap .si { color: #5a2; } /* Literal.String.Interpol */
-.pygments-style-abap .sx { color: #5a2; } /* Literal.String.Other */
-.pygments-style-abap .sr { color: #5a2; } /* Literal.String.Regex */
-.pygments-style-abap .s1 { color: #5a2; } /* Literal.String.Single */
-.pygments-style-abap .ss { color: #5a2; } /* Literal.String.Symbol */
-.pygments-style-abap .bp { color: #000; } /* Name.Builtin.Pseudo */
-.pygments-style-abap .fm { color: #000; } /* Name.Function.Magic */
-.pygments-style-abap .vc { color: #000; } /* Name.Variable.Class */
-.pygments-style-abap .vg { color: #000; } /* Name.Variable.Global */
-.pygments-style-abap .vi { color: #000; } /* Name.Variable.Instance */
-.pygments-style-abap .vm { color: #000; } /* Name.Variable.Magic */
-.pygments-style-abap .il { color: #3af; } /* Literal.Number.Integer.Long */
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+.pygments-style-abap .hll { background-color: #ffc }
+
+.pygments-style-abap { background: #fff; 
+}
+
+.pygments-style-abap .c { color: #888; 
+font-style: italic } /* Comment */
+.pygments-style-abap .err { color: #F00 } /* Error */
+.pygments-style-abap .k { color: #00f } /* Keyword */
+.pygments-style-abap .n { color: #000 } /* Name */
+.pygments-style-abap .ch { color: #888; 
+font-style: italic } /* Comment.Hashbang */
+.pygments-style-abap .cm { color: #888; 
+font-style: italic } /* Comment.Multiline */
+.pygments-style-abap .cp { color: #888; 
+font-style: italic } /* Comment.Preproc */
+.pygments-style-abap .cpf { color: #888; 
+font-style: italic } /* Comment.PreprocFile */
+.pygments-style-abap .c1 { color: #888; 
+font-style: italic } /* Comment.Single */
+.pygments-style-abap .cs { color: #888; 
+font-style: italic } /* Comment.Special */
+.pygments-style-abap .kc { color: #00f } /* Keyword.Constant */
+.pygments-style-abap .kd { color: #00f } /* Keyword.Declaration */
+.pygments-style-abap .kn { color: #00f } /* Keyword.Namespace */
+.pygments-style-abap .kp { color: #00f } /* Keyword.Pseudo */
+.pygments-style-abap .kr { color: #00f } /* Keyword.Reserved */
+.pygments-style-abap .kt { color: #00f } /* Keyword.Type */
+.pygments-style-abap .m { color: #3af } /* Literal.Number */
+.pygments-style-abap .s { color: #5a2 } /* Literal.String */
+.pygments-style-abap .na { color: #000 } /* Name.Attribute */
+.pygments-style-abap .nb { color: #000 } /* Name.Builtin */
+.pygments-style-abap .nc { color: #000 } /* Name.Class */
+.pygments-style-abap .no { color: #000 } /* Name.Constant */
+.pygments-style-abap .nd { color: #000 } /* Name.Decorator */
+.pygments-style-abap .ni { color: #000 } /* Name.Entity */
+.pygments-style-abap .ne { color: #000 } /* Name.Exception */
+.pygments-style-abap .nf { color: #000 } /* Name.Function */
+.pygments-style-abap .nl { color: #000 } /* Name.Label */
+.pygments-style-abap .nn { color: #000 } /* Name.Namespace */
+.pygments-style-abap .nx { color: #000 } /* Name.Other */
+.pygments-style-abap .py { color: #000 } /* Name.Property */
+.pygments-style-abap .nt { color: #000 } /* Name.Tag */
+.pygments-style-abap .nv { color: #000 } /* Name.Variable */
+.pygments-style-abap .ow { color: #00f } /* Operator.Word */
+.pygments-style-abap .mb { color: #3af } /* Literal.Number.Bin */
+.pygments-style-abap .mf { color: #3af } /* Literal.Number.Float */
+.pygments-style-abap .mh { color: #3af } /* Literal.Number.Hex */
+.pygments-style-abap .mi { color: #3af } /* Literal.Number.Integer */
+.pygments-style-abap .mo { color: #3af } /* Literal.Number.Oct */
+.pygments-style-abap .sa { color: #5a2 } /* Literal.String.Affix */
+.pygments-style-abap .sb { color: #5a2 } /* Literal.String.Backtick */
+.pygments-style-abap .sc { color: #5a2 } /* Literal.String.Char */
+.pygments-style-abap .dl { color: #5a2 } /* Literal.String.Delimiter */
+.pygments-style-abap .sd { color: #5a2 } /* Literal.String.Doc */
+.pygments-style-abap .s2 { color: #5a2 } /* Literal.String.Double */
+.pygments-style-abap .se { color: #5a2 } /* Literal.String.Escape */
+.pygments-style-abap .sh { color: #5a2 } /* Literal.String.Heredoc */
+.pygments-style-abap .si { color: #5a2 } /* Literal.String.Interpol */
+.pygments-style-abap .sx { color: #5a2 } /* Literal.String.Other */
+.pygments-style-abap .sr { color: #5a2 } /* Literal.String.Regex */
+.pygments-style-abap .s1 { color: #5a2 } /* Literal.String.Single */
+.pygments-style-abap .ss { color: #5a2 } /* Literal.String.Symbol */
+.pygments-style-abap .bp { color: #000 } /* Name.Builtin.Pseudo */
+.pygments-style-abap .fm { color: #000 } /* Name.Function.Magic */
+.pygments-style-abap .vc { color: #000 } /* Name.Variable.Class */
+.pygments-style-abap .vg { color: #000 } /* Name.Variable.Global */
+.pygments-style-abap .vi { color: #000 } /* Name.Variable.Instance */
+.pygments-style-abap .vm { color: #000 } /* Name.Variable.Magic */
+.pygments-style-abap .il { color: #3af } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/algol.css` & `plumage-4.0.0/plumage/static/css/pygments/algol.css`

 * *Files 21% similar despite different names*

```diff
@@ -1,210 +1,124 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-.pygments-style-algol .hll { background-color: #ffc; }
-
-.pygments-style-algol {
-  background: #fff;
-}
-
-.pygments-style-algol .c {
-  color: #888;
-  font-style: italic;
-} /* Comment */
-.pygments-style-algol .err { border: 1px solid #f00; } /* Error */
-.pygments-style-algol .k {
-  font-weight: bold;
-  text-decoration: underline;
-} /* Keyword */
-.pygments-style-algol .ch {
-  color: #888;
-  font-style: italic;
-} /* Comment.Hashbang */
-.pygments-style-algol .cm {
-  color: #888;
-  font-style: italic;
-} /* Comment.Multiline */
-.pygments-style-algol .cp {
-  color: #888;
-  font-weight: bold;
-} /* Comment.Preproc */
-.pygments-style-algol .cpf {
-  color: #888;
-  font-style: italic;
-} /* Comment.PreprocFile */
-.pygments-style-algol .c1 {
-  color: #888;
-  font-style: italic;
-} /* Comment.Single */
-.pygments-style-algol .cs {
-  color: #888;
-  font-weight: bold;
-} /* Comment.Special */
-.pygments-style-algol .kc {
-  font-weight: bold;
-  text-decoration: underline;
-} /* Keyword.Constant */
-.pygments-style-algol .kd {
-  font-weight: bold;
-  font-style: italic;
-  text-decoration: underline;
-} /* Keyword.Declaration */
-.pygments-style-algol .kn {
-  font-weight: bold;
-  text-decoration: underline;
-} /* Keyword.Namespace */
-.pygments-style-algol .kp {
-  font-weight: bold;
-  text-decoration: underline;
-} /* Keyword.Pseudo */
-.pygments-style-algol .kr {
-  font-weight: bold;
-  text-decoration: underline;
-} /* Keyword.Reserved */
-.pygments-style-algol .kt {
-  font-weight: bold;
-  text-decoration: underline;
-} /* Keyword.Type */
-.pygments-style-algol .s {
-  color: #666;
-  font-style: italic;
-} /* Literal.String */
-.pygments-style-algol .nb {
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Builtin */
-.pygments-style-algol .nc {
-  color: #666;
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Class */
-.pygments-style-algol .no {
-  color: #666;
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Constant */
-.pygments-style-algol .nf {
-  color: #666;
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Function */
-.pygments-style-algol .nn {
-  color: #666;
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Namespace */
-.pygments-style-algol .nv {
-  color: #666;
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Variable */
-.pygments-style-algol .ow { font-weight: bold; } /* Operator.Word */
-.pygments-style-algol .sa {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Affix */
-.pygments-style-algol .sb {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Backtick */
-.pygments-style-algol .sc {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Char */
-.pygments-style-algol .dl {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Delimiter */
-.pygments-style-algol .sd {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Doc */
-.pygments-style-algol .s2 {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Double */
-.pygments-style-algol .se {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Escape */
-.pygments-style-algol .sh {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Heredoc */
-.pygments-style-algol .si {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Interpol */
-.pygments-style-algol .sx {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Other */
-.pygments-style-algol .sr {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Regex */
-.pygments-style-algol .s1 {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Single */
-.pygments-style-algol .ss {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Symbol */
-.pygments-style-algol .bp {
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Builtin.Pseudo */
-.pygments-style-algol .fm {
-  color: #666;
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Function.Magic */
-.pygments-style-algol .vc {
-  color: #666;
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Variable.Class */
-.pygments-style-algol .vg {
-  color: #666;
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Variable.Global */
-.pygments-style-algol .vi {
-  color: #666;
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Variable.Instance */
-.pygments-style-algol .vm {
-  color: #666;
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Variable.Magic */
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+.pygments-style-algol .hll { background-color: #ffc }
+
+.pygments-style-algol { background: #fff; 
+}
+
+.pygments-style-algol .c { color: #888; 
+font-style: italic } /* Comment */
+.pygments-style-algol .err { border: 1px solid #F00 } /* Error */
+.pygments-style-algol .k { font-weight: bold; 
+text-decoration: underline } /* Keyword */
+.pygments-style-algol .ch { color: #888; 
+font-style: italic } /* Comment.Hashbang */
+.pygments-style-algol .cm { color: #888; 
+font-style: italic } /* Comment.Multiline */
+.pygments-style-algol .cp { color: #888; 
+font-weight: bold } /* Comment.Preproc */
+.pygments-style-algol .cpf { color: #888; 
+font-style: italic } /* Comment.PreprocFile */
+.pygments-style-algol .c1 { color: #888; 
+font-style: italic } /* Comment.Single */
+.pygments-style-algol .cs { color: #888; 
+font-weight: bold } /* Comment.Special */
+.pygments-style-algol .kc { font-weight: bold; 
+text-decoration: underline } /* Keyword.Constant */
+.pygments-style-algol .kd { font-weight: bold; 
+font-style: italic; 
+text-decoration: underline } /* Keyword.Declaration */
+.pygments-style-algol .kn { font-weight: bold; 
+text-decoration: underline } /* Keyword.Namespace */
+.pygments-style-algol .kp { font-weight: bold; 
+text-decoration: underline } /* Keyword.Pseudo */
+.pygments-style-algol .kr { font-weight: bold; 
+text-decoration: underline } /* Keyword.Reserved */
+.pygments-style-algol .kt { font-weight: bold; 
+text-decoration: underline } /* Keyword.Type */
+.pygments-style-algol .s { color: #666; 
+font-style: italic } /* Literal.String */
+.pygments-style-algol .nb { font-weight: bold; 
+font-style: italic } /* Name.Builtin */
+.pygments-style-algol .nc { color: #666; 
+font-weight: bold; 
+font-style: italic } /* Name.Class */
+.pygments-style-algol .no { color: #666; 
+font-weight: bold; 
+font-style: italic } /* Name.Constant */
+.pygments-style-algol .nf { color: #666; 
+font-weight: bold; 
+font-style: italic } /* Name.Function */
+.pygments-style-algol .nn { color: #666; 
+font-weight: bold; 
+font-style: italic } /* Name.Namespace */
+.pygments-style-algol .nv { color: #666; 
+font-weight: bold; 
+font-style: italic } /* Name.Variable */
+.pygments-style-algol .ow { font-weight: bold } /* Operator.Word */
+.pygments-style-algol .sa { color: #666; 
+font-style: italic } /* Literal.String.Affix */
+.pygments-style-algol .sb { color: #666; 
+font-style: italic } /* Literal.String.Backtick */
+.pygments-style-algol .sc { color: #666; 
+font-style: italic } /* Literal.String.Char */
+.pygments-style-algol .dl { color: #666; 
+font-style: italic } /* Literal.String.Delimiter */
+.pygments-style-algol .sd { color: #666; 
+font-style: italic } /* Literal.String.Doc */
+.pygments-style-algol .s2 { color: #666; 
+font-style: italic } /* Literal.String.Double */
+.pygments-style-algol .se { color: #666; 
+font-style: italic } /* Literal.String.Escape */
+.pygments-style-algol .sh { color: #666; 
+font-style: italic } /* Literal.String.Heredoc */
+.pygments-style-algol .si { color: #666; 
+font-style: italic } /* Literal.String.Interpol */
+.pygments-style-algol .sx { color: #666; 
+font-style: italic } /* Literal.String.Other */
+.pygments-style-algol .sr { color: #666; 
+font-style: italic } /* Literal.String.Regex */
+.pygments-style-algol .s1 { color: #666; 
+font-style: italic } /* Literal.String.Single */
+.pygments-style-algol .ss { color: #666; 
+font-style: italic } /* Literal.String.Symbol */
+.pygments-style-algol .bp { font-weight: bold; 
+font-style: italic } /* Name.Builtin.Pseudo */
+.pygments-style-algol .fm { color: #666; 
+font-weight: bold; 
+font-style: italic } /* Name.Function.Magic */
+.pygments-style-algol .vc { color: #666; 
+font-weight: bold; 
+font-style: italic } /* Name.Variable.Class */
+.pygments-style-algol .vg { color: #666; 
+font-weight: bold; 
+font-style: italic } /* Name.Variable.Global */
+.pygments-style-algol .vi { color: #666; 
+font-weight: bold; 
+font-style: italic } /* Name.Variable.Instance */
+.pygments-style-algol .vm { color: #666; 
+font-weight: bold; 
+font-style: italic } /* Name.Variable.Magic */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/algol_nu.css` & `plumage-4.0.0/plumage/static/css/pygments/algol_nu.css`

 * *Files 22% similar despite different names*

```diff
@@ -1,191 +1,117 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-.pygments-style-algol_nu .hll { background-color: #ffc; }
-
-.pygments-style-algol_nu {
-  background: #fff;
-}
-
-.pygments-style-algol_nu .c {
-  color: #888;
-  font-style: italic;
-} /* Comment */
-.pygments-style-algol_nu .err { border: 1px solid #f00; } /* Error */
-.pygments-style-algol_nu .k { font-weight: bold; } /* Keyword */
-.pygments-style-algol_nu .ch {
-  color: #888;
-  font-style: italic;
-} /* Comment.Hashbang */
-.pygments-style-algol_nu .cm {
-  color: #888;
-  font-style: italic;
-} /* Comment.Multiline */
-.pygments-style-algol_nu .cp {
-  color: #888;
-  font-weight: bold;
-} /* Comment.Preproc */
-.pygments-style-algol_nu .cpf {
-  color: #888;
-  font-style: italic;
-} /* Comment.PreprocFile */
-.pygments-style-algol_nu .c1 {
-  color: #888;
-  font-style: italic;
-} /* Comment.Single */
-.pygments-style-algol_nu .cs {
-  color: #888;
-  font-weight: bold;
-} /* Comment.Special */
-.pygments-style-algol_nu .kc { font-weight: bold; } /* Keyword.Constant */
-.pygments-style-algol_nu .kd {
-  font-weight: bold;
-  font-style: italic;
-} /* Keyword.Declaration */
-.pygments-style-algol_nu .kn { font-weight: bold; } /* Keyword.Namespace */
-.pygments-style-algol_nu .kp { font-weight: bold; } /* Keyword.Pseudo */
-.pygments-style-algol_nu .kr { font-weight: bold; } /* Keyword.Reserved */
-.pygments-style-algol_nu .kt { font-weight: bold; } /* Keyword.Type */
-.pygments-style-algol_nu .s {
-  color: #666;
-  font-style: italic;
-} /* Literal.String */
-.pygments-style-algol_nu .nb {
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Builtin */
-.pygments-style-algol_nu .nc {
-  color: #666;
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Class */
-.pygments-style-algol_nu .no {
-  color: #666;
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Constant */
-.pygments-style-algol_nu .nf {
-  color: #666;
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Function */
-.pygments-style-algol_nu .nn {
-  color: #666;
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Namespace */
-.pygments-style-algol_nu .nv {
-  color: #666;
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Variable */
-.pygments-style-algol_nu .ow { font-weight: bold; } /* Operator.Word */
-.pygments-style-algol_nu .sa {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Affix */
-.pygments-style-algol_nu .sb {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Backtick */
-.pygments-style-algol_nu .sc {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Char */
-.pygments-style-algol_nu .dl {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Delimiter */
-.pygments-style-algol_nu .sd {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Doc */
-.pygments-style-algol_nu .s2 {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Double */
-.pygments-style-algol_nu .se {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Escape */
-.pygments-style-algol_nu .sh {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Heredoc */
-.pygments-style-algol_nu .si {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Interpol */
-.pygments-style-algol_nu .sx {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Other */
-.pygments-style-algol_nu .sr {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Regex */
-.pygments-style-algol_nu .s1 {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Single */
-.pygments-style-algol_nu .ss {
-  color: #666;
-  font-style: italic;
-} /* Literal.String.Symbol */
-.pygments-style-algol_nu .bp {
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Builtin.Pseudo */
-.pygments-style-algol_nu .fm {
-  color: #666;
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Function.Magic */
-.pygments-style-algol_nu .vc {
-  color: #666;
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Variable.Class */
-.pygments-style-algol_nu .vg {
-  color: #666;
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Variable.Global */
-.pygments-style-algol_nu .vi {
-  color: #666;
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Variable.Instance */
-.pygments-style-algol_nu .vm {
-  color: #666;
-  font-weight: bold;
-  font-style: italic;
-} /* Name.Variable.Magic */
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+.pygments-style-algol_nu .hll { background-color: #ffc }
+
+.pygments-style-algol_nu { background: #fff; 
+}
+
+.pygments-style-algol_nu .c { color: #888; 
+font-style: italic } /* Comment */
+.pygments-style-algol_nu .err { border: 1px solid #F00 } /* Error */
+.pygments-style-algol_nu .k { font-weight: bold } /* Keyword */
+.pygments-style-algol_nu .ch { color: #888; 
+font-style: italic } /* Comment.Hashbang */
+.pygments-style-algol_nu .cm { color: #888; 
+font-style: italic } /* Comment.Multiline */
+.pygments-style-algol_nu .cp { color: #888; 
+font-weight: bold } /* Comment.Preproc */
+.pygments-style-algol_nu .cpf { color: #888; 
+font-style: italic } /* Comment.PreprocFile */
+.pygments-style-algol_nu .c1 { color: #888; 
+font-style: italic } /* Comment.Single */
+.pygments-style-algol_nu .cs { color: #888; 
+font-weight: bold } /* Comment.Special */
+.pygments-style-algol_nu .kc { font-weight: bold } /* Keyword.Constant */
+.pygments-style-algol_nu .kd { font-weight: bold; 
+font-style: italic } /* Keyword.Declaration */
+.pygments-style-algol_nu .kn { font-weight: bold } /* Keyword.Namespace */
+.pygments-style-algol_nu .kp { font-weight: bold } /* Keyword.Pseudo */
+.pygments-style-algol_nu .kr { font-weight: bold } /* Keyword.Reserved */
+.pygments-style-algol_nu .kt { font-weight: bold } /* Keyword.Type */
+.pygments-style-algol_nu .s { color: #666; 
+font-style: italic } /* Literal.String */
+.pygments-style-algol_nu .nb { font-weight: bold; 
+font-style: italic } /* Name.Builtin */
+.pygments-style-algol_nu .nc { color: #666; 
+font-weight: bold; 
+font-style: italic } /* Name.Class */
+.pygments-style-algol_nu .no { color: #666; 
+font-weight: bold; 
+font-style: italic } /* Name.Constant */
+.pygments-style-algol_nu .nf { color: #666; 
+font-weight: bold; 
+font-style: italic } /* Name.Function */
+.pygments-style-algol_nu .nn { color: #666; 
+font-weight: bold; 
+font-style: italic } /* Name.Namespace */
+.pygments-style-algol_nu .nv { color: #666; 
+font-weight: bold; 
+font-style: italic } /* Name.Variable */
+.pygments-style-algol_nu .ow { font-weight: bold } /* Operator.Word */
+.pygments-style-algol_nu .sa { color: #666; 
+font-style: italic } /* Literal.String.Affix */
+.pygments-style-algol_nu .sb { color: #666; 
+font-style: italic } /* Literal.String.Backtick */
+.pygments-style-algol_nu .sc { color: #666; 
+font-style: italic } /* Literal.String.Char */
+.pygments-style-algol_nu .dl { color: #666; 
+font-style: italic } /* Literal.String.Delimiter */
+.pygments-style-algol_nu .sd { color: #666; 
+font-style: italic } /* Literal.String.Doc */
+.pygments-style-algol_nu .s2 { color: #666; 
+font-style: italic } /* Literal.String.Double */
+.pygments-style-algol_nu .se { color: #666; 
+font-style: italic } /* Literal.String.Escape */
+.pygments-style-algol_nu .sh { color: #666; 
+font-style: italic } /* Literal.String.Heredoc */
+.pygments-style-algol_nu .si { color: #666; 
+font-style: italic } /* Literal.String.Interpol */
+.pygments-style-algol_nu .sx { color: #666; 
+font-style: italic } /* Literal.String.Other */
+.pygments-style-algol_nu .sr { color: #666; 
+font-style: italic } /* Literal.String.Regex */
+.pygments-style-algol_nu .s1 { color: #666; 
+font-style: italic } /* Literal.String.Single */
+.pygments-style-algol_nu .ss { color: #666; 
+font-style: italic } /* Literal.String.Symbol */
+.pygments-style-algol_nu .bp { font-weight: bold; 
+font-style: italic } /* Name.Builtin.Pseudo */
+.pygments-style-algol_nu .fm { color: #666; 
+font-weight: bold; 
+font-style: italic } /* Name.Function.Magic */
+.pygments-style-algol_nu .vc { color: #666; 
+font-weight: bold; 
+font-style: italic } /* Name.Variable.Class */
+.pygments-style-algol_nu .vg { color: #666; 
+font-weight: bold; 
+font-style: italic } /* Name.Variable.Global */
+.pygments-style-algol_nu .vi { color: #666; 
+font-weight: bold; 
+font-style: italic } /* Name.Variable.Instance */
+.pygments-style-algol_nu .vm { color: #666; 
+font-weight: bold; 
+font-style: italic } /* Name.Variable.Magic */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/arduino.css` & `plumage-4.0.0/plumage/static/css/pygments/arduino.css`

 * *Files 9% similar despite different names*

```diff
@@ -1,95 +1,89 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
-.pygments-style-arduino .hll { background-color: #ffc; }
+.pygments-style-arduino .hll { background-color: #ffc }
 
-.pygments-style-arduino {
-  background: #fff;
+.pygments-style-arduino { background: #fff; 
 }
-.pygments-style-arduino .c { color: #95a5a6; } /* Comment */
-.pygments-style-arduino .err { color: #a61717; } /* Error */
-.pygments-style-arduino .k { color: #728e00; } /* Keyword */
-.pygments-style-arduino .n { color: #434f54; } /* Name */
-.pygments-style-arduino .o { color: #728e00; } /* Operator */
-.pygments-style-arduino .ch { color: #95a5a6; } /* Comment.Hashbang */
-.pygments-style-arduino .cm { color: #95a5a6; } /* Comment.Multiline */
-.pygments-style-arduino .cp { color: #728e00; } /* Comment.Preproc */
-.pygments-style-arduino .cpf { color: #95a5a6; } /* Comment.PreprocFile */
-.pygments-style-arduino .c1 { color: #95a5a6; } /* Comment.Single */
-.pygments-style-arduino .cs { color: #95a5a6; } /* Comment.Special */
-.pygments-style-arduino .kc { color: #00979d; } /* Keyword.Constant */
-.pygments-style-arduino .kd { color: #728e00; } /* Keyword.Declaration */
-.pygments-style-arduino .kn { color: #728e00; } /* Keyword.Namespace */
-.pygments-style-arduino .kp { color: #00979d; } /* Keyword.Pseudo */
-.pygments-style-arduino .kr { color: #00979d; } /* Keyword.Reserved */
-.pygments-style-arduino .kt { color: #00979d; } /* Keyword.Type */
-.pygments-style-arduino .m { color: #8a7b52; } /* Literal.Number */
-.pygments-style-arduino .s { color: #7f8c8d; } /* Literal.String */
-.pygments-style-arduino .na { color: #434f54; } /* Name.Attribute */
-.pygments-style-arduino .nb { color: #728e00; } /* Name.Builtin */
-.pygments-style-arduino .nc { color: #434f54; } /* Name.Class */
-.pygments-style-arduino .no { color: #434f54; } /* Name.Constant */
-.pygments-style-arduino .nd { color: #434f54; } /* Name.Decorator */
-.pygments-style-arduino .ni { color: #434f54; } /* Name.Entity */
-.pygments-style-arduino .ne { color: #434f54; } /* Name.Exception */
-.pygments-style-arduino .nf { color: #d35400; } /* Name.Function */
-.pygments-style-arduino .nl { color: #434f54; } /* Name.Label */
-.pygments-style-arduino .nn { color: #434f54; } /* Name.Namespace */
-.pygments-style-arduino .nx { color: #728e00; } /* Name.Other */
-.pygments-style-arduino .py { color: #434f54; } /* Name.Property */
-.pygments-style-arduino .nt { color: #434f54; } /* Name.Tag */
-.pygments-style-arduino .nv { color: #434f54; } /* Name.Variable */
-.pygments-style-arduino .ow { color: #728e00; } /* Operator.Word */
-.pygments-style-arduino .mb { color: #8a7b52; } /* Literal.Number.Bin */
-.pygments-style-arduino .mf { color: #8a7b52; } /* Literal.Number.Float */
-.pygments-style-arduino .mh { color: #8a7b52; } /* Literal.Number.Hex */
-.pygments-style-arduino .mi { color: #8a7b52; } /* Literal.Number.Integer */
-.pygments-style-arduino .mo { color: #8a7b52; } /* Literal.Number.Oct */
-.pygments-style-arduino .sa { color: #7f8c8d; } /* Literal.String.Affix */
-.pygments-style-arduino .sb { color: #7f8c8d; } /* Literal.String.Backtick */
-.pygments-style-arduino .sc { color: #7f8c8d; } /* Literal.String.Char */
-.pygments-style-arduino .dl { color: #7f8c8d; } /* Literal.String.Delimiter */
-.pygments-style-arduino .sd { color: #7f8c8d; } /* Literal.String.Doc */
-.pygments-style-arduino .s2 { color: #7f8c8d; } /* Literal.String.Double */
-.pygments-style-arduino .se { color: #7f8c8d; } /* Literal.String.Escape */
-.pygments-style-arduino .sh { color: #7f8c8d; } /* Literal.String.Heredoc */
-.pygments-style-arduino .si { color: #7f8c8d; } /* Literal.String.Interpol */
-.pygments-style-arduino .sx { color: #7f8c8d; } /* Literal.String.Other */
-.pygments-style-arduino .sr { color: #7f8c8d; } /* Literal.String.Regex */
-.pygments-style-arduino .s1 { color: #7f8c8d; } /* Literal.String.Single */
-.pygments-style-arduino .ss { color: #7f8c8d; } /* Literal.String.Symbol */
-.pygments-style-arduino .bp { color: #728e00; } /* Name.Builtin.Pseudo */
-.pygments-style-arduino .fm { color: #d35400; } /* Name.Function.Magic */
-.pygments-style-arduino .vc { color: #434f54; } /* Name.Variable.Class */
-.pygments-style-arduino .vg { color: #434f54; } /* Name.Variable.Global */
-.pygments-style-arduino .vi { color: #434f54; } /* Name.Variable.Instance */
-.pygments-style-arduino .vm { color: #434f54; } /* Name.Variable.Magic */
-.pygments-style-arduino .il { color: #8a7b52; } /* Literal.Number.Integer.Long */
+.pygments-style-arduino .c { color: #95a5a6 } /* Comment */
+.pygments-style-arduino .err { color: #a61717 } /* Error */
+.pygments-style-arduino .k { color: #728E00 } /* Keyword */
+.pygments-style-arduino .n { color: #434f54 } /* Name */
+.pygments-style-arduino .o { color: #728E00 } /* Operator */
+.pygments-style-arduino .ch { color: #95a5a6 } /* Comment.Hashbang */
+.pygments-style-arduino .cm { color: #95a5a6 } /* Comment.Multiline */
+.pygments-style-arduino .cp { color: #728E00 } /* Comment.Preproc */
+.pygments-style-arduino .cpf { color: #95a5a6 } /* Comment.PreprocFile */
+.pygments-style-arduino .c1 { color: #95a5a6 } /* Comment.Single */
+.pygments-style-arduino .cs { color: #95a5a6 } /* Comment.Special */
+.pygments-style-arduino .kc { color: #00979D } /* Keyword.Constant */
+.pygments-style-arduino .kd { color: #728E00 } /* Keyword.Declaration */
+.pygments-style-arduino .kn { color: #728E00 } /* Keyword.Namespace */
+.pygments-style-arduino .kp { color: #00979D } /* Keyword.Pseudo */
+.pygments-style-arduino .kr { color: #00979D } /* Keyword.Reserved */
+.pygments-style-arduino .kt { color: #00979D } /* Keyword.Type */
+.pygments-style-arduino .m { color: #8A7B52 } /* Literal.Number */
+.pygments-style-arduino .s { color: #7F8C8D } /* Literal.String */
+.pygments-style-arduino .na { color: #434f54 } /* Name.Attribute */
+.pygments-style-arduino .nb { color: #728E00 } /* Name.Builtin */
+.pygments-style-arduino .nc { color: #434f54 } /* Name.Class */
+.pygments-style-arduino .no { color: #434f54 } /* Name.Constant */
+.pygments-style-arduino .nd { color: #434f54 } /* Name.Decorator */
+.pygments-style-arduino .ni { color: #434f54 } /* Name.Entity */
+.pygments-style-arduino .ne { color: #434f54 } /* Name.Exception */
+.pygments-style-arduino .nf { color: #D35400 } /* Name.Function */
+.pygments-style-arduino .nl { color: #434f54 } /* Name.Label */
+.pygments-style-arduino .nn { color: #434f54 } /* Name.Namespace */
+.pygments-style-arduino .nx { color: #728E00 } /* Name.Other */
+.pygments-style-arduino .py { color: #434f54 } /* Name.Property */
+.pygments-style-arduino .nt { color: #434f54 } /* Name.Tag */
+.pygments-style-arduino .nv { color: #434f54 } /* Name.Variable */
+.pygments-style-arduino .ow { color: #728E00 } /* Operator.Word */
+.pygments-style-arduino .mb { color: #8A7B52 } /* Literal.Number.Bin */
+.pygments-style-arduino .mf { color: #8A7B52 } /* Literal.Number.Float */
+.pygments-style-arduino .mh { color: #8A7B52 } /* Literal.Number.Hex */
+.pygments-style-arduino .mi { color: #8A7B52 } /* Literal.Number.Integer */
+.pygments-style-arduino .mo { color: #8A7B52 } /* Literal.Number.Oct */
+.pygments-style-arduino .sa { color: #7F8C8D } /* Literal.String.Affix */
+.pygments-style-arduino .sb { color: #7F8C8D } /* Literal.String.Backtick */
+.pygments-style-arduino .sc { color: #7F8C8D } /* Literal.String.Char */
+.pygments-style-arduino .dl { color: #7F8C8D } /* Literal.String.Delimiter */
+.pygments-style-arduino .sd { color: #7F8C8D } /* Literal.String.Doc */
+.pygments-style-arduino .s2 { color: #7F8C8D } /* Literal.String.Double */
+.pygments-style-arduino .se { color: #7F8C8D } /* Literal.String.Escape */
+.pygments-style-arduino .sh { color: #7F8C8D } /* Literal.String.Heredoc */
+.pygments-style-arduino .si { color: #7F8C8D } /* Literal.String.Interpol */
+.pygments-style-arduino .sx { color: #7F8C8D } /* Literal.String.Other */
+.pygments-style-arduino .sr { color: #7F8C8D } /* Literal.String.Regex */
+.pygments-style-arduino .s1 { color: #7F8C8D } /* Literal.String.Single */
+.pygments-style-arduino .ss { color: #7F8C8D } /* Literal.String.Symbol */
+.pygments-style-arduino .bp { color: #728E00 } /* Name.Builtin.Pseudo */
+.pygments-style-arduino .fm { color: #D35400 } /* Name.Function.Magic */
+.pygments-style-arduino .vc { color: #434f54 } /* Name.Variable.Class */
+.pygments-style-arduino .vg { color: #434f54 } /* Name.Variable.Global */
+.pygments-style-arduino .vi { color: #434f54 } /* Name.Variable.Instance */
+.pygments-style-arduino .vm { color: #434f54 } /* Name.Variable.Magic */
+.pygments-style-arduino .il { color: #8A7B52 } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/autumn.css` & `plumage-4.0.0/plumage/static/css/pygments/autumn.css`

 * *Files 18% similar despite different names*

```diff
@@ -1,140 +1,110 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-.pygments-style-autumn .hll { background-color: #ffc; }
-
-.pygments-style-autumn {
-  background: #fff;
-}
-
-.pygments-style-autumn .c {
-  color: #aaa;
-  font-style: italic;
-} /* Comment */
-.pygments-style-autumn .err {
-  color: #f00;
-  background-color: #faa;
-} /* Error */
-.pygments-style-autumn .k { color: #00a; } /* Keyword */
-.pygments-style-autumn .ch {
-  color: #aaa;
-  font-style: italic;
-} /* Comment.Hashbang */
-.pygments-style-autumn .cm {
-  color: #aaa;
-  font-style: italic;
-} /* Comment.Multiline */
-.pygments-style-autumn .cp { color: #4c8317; } /* Comment.Preproc */
-.pygments-style-autumn .cpf {
-  color: #aaa;
-  font-style: italic;
-} /* Comment.PreprocFile */
-.pygments-style-autumn .c1 {
-  color: #aaa;
-  font-style: italic;
-} /* Comment.Single */
-.pygments-style-autumn .cs {
-  color: #00a;
-  font-style: italic;
-} /* Comment.Special */
-.pygments-style-autumn .gd { color: #a00; } /* Generic.Deleted */
-.pygments-style-autumn .ge { font-style: italic; } /* Generic.Emph */
-.pygments-style-autumn .gr { color: #a00; } /* Generic.Error */
-.pygments-style-autumn .gh {
-  color: #000080;
-  font-weight: bold;
-} /* Generic.Heading */
-.pygments-style-autumn .gi { color: #0a0; } /* Generic.Inserted */
-.pygments-style-autumn .go { color: #888; } /* Generic.Output */
-.pygments-style-autumn .gp { color: #555; } /* Generic.Prompt */
-.pygments-style-autumn .gs { font-weight: bold; } /* Generic.Strong */
-.pygments-style-autumn .gu {
-  color: #800080;
-  font-weight: bold;
-} /* Generic.Subheading */
-.pygments-style-autumn .gt { color: #a00; } /* Generic.Traceback */
-.pygments-style-autumn .kc { color: #00a; } /* Keyword.Constant */
-.pygments-style-autumn .kd { color: #00a; } /* Keyword.Declaration */
-.pygments-style-autumn .kn { color: #00a; } /* Keyword.Namespace */
-.pygments-style-autumn .kp { color: #00a; } /* Keyword.Pseudo */
-.pygments-style-autumn .kr { color: #00a; } /* Keyword.Reserved */
-.pygments-style-autumn .kt { color: #0aa; } /* Keyword.Type */
-.pygments-style-autumn .m { color: #099; } /* Literal.Number */
-.pygments-style-autumn .s { color: #a50; } /* Literal.String */
-.pygments-style-autumn .na { color: #1e90ff; } /* Name.Attribute */
-.pygments-style-autumn .nb { color: #0aa; } /* Name.Builtin */
-.pygments-style-autumn .nc {
-  color: #0a0;
-  text-decoration: underline;
-} /* Name.Class */
-.pygments-style-autumn .no { color: #a00; } /* Name.Constant */
-.pygments-style-autumn .nd { color: #888; } /* Name.Decorator */
-.pygments-style-autumn .ni {
-  color: #800;
-  font-weight: bold;
-} /* Name.Entity */
-.pygments-style-autumn .nf { color: #0a0; } /* Name.Function */
-.pygments-style-autumn .nn {
-  color: #0aa;
-  text-decoration: underline;
-} /* Name.Namespace */
-.pygments-style-autumn .nt {
-  color: #1e90ff;
-  font-weight: bold;
-} /* Name.Tag */
-.pygments-style-autumn .nv { color: #a00; } /* Name.Variable */
-.pygments-style-autumn .ow { color: #00a; } /* Operator.Word */
-.pygments-style-autumn .w { color: #bbb; } /* Text.Whitespace */
-.pygments-style-autumn .mb { color: #099; } /* Literal.Number.Bin */
-.pygments-style-autumn .mf { color: #099; } /* Literal.Number.Float */
-.pygments-style-autumn .mh { color: #099; } /* Literal.Number.Hex */
-.pygments-style-autumn .mi { color: #099; } /* Literal.Number.Integer */
-.pygments-style-autumn .mo { color: #099; } /* Literal.Number.Oct */
-.pygments-style-autumn .sa { color: #a50; } /* Literal.String.Affix */
-.pygments-style-autumn .sb { color: #a50; } /* Literal.String.Backtick */
-.pygments-style-autumn .sc { color: #a50; } /* Literal.String.Char */
-.pygments-style-autumn .dl { color: #a50; } /* Literal.String.Delimiter */
-.pygments-style-autumn .sd { color: #a50; } /* Literal.String.Doc */
-.pygments-style-autumn .s2 { color: #a50; } /* Literal.String.Double */
-.pygments-style-autumn .se { color: #a50; } /* Literal.String.Escape */
-.pygments-style-autumn .sh { color: #a50; } /* Literal.String.Heredoc */
-.pygments-style-autumn .si { color: #a50; } /* Literal.String.Interpol */
-.pygments-style-autumn .sx { color: #a50; } /* Literal.String.Other */
-.pygments-style-autumn .sr { color: #099; } /* Literal.String.Regex */
-.pygments-style-autumn .s1 { color: #a50; } /* Literal.String.Single */
-.pygments-style-autumn .ss { color: #00a; } /* Literal.String.Symbol */
-.pygments-style-autumn .bp { color: #0aa; } /* Name.Builtin.Pseudo */
-.pygments-style-autumn .fm { color: #0a0; } /* Name.Function.Magic */
-.pygments-style-autumn .vc { color: #a00; } /* Name.Variable.Class */
-.pygments-style-autumn .vg { color: #a00; } /* Name.Variable.Global */
-.pygments-style-autumn .vi { color: #a00; } /* Name.Variable.Instance */
-.pygments-style-autumn .vm { color: #a00; } /* Name.Variable.Magic */
-.pygments-style-autumn .il { color: #099; } /* Literal.Number.Integer.Long */
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+.pygments-style-autumn .hll { background-color: #ffc }
+
+.pygments-style-autumn { background: #fff; 
+}
+
+.pygments-style-autumn .c { color: #aaa; 
+font-style: italic } /* Comment */
+.pygments-style-autumn .err { color: #F00; 
+background-color: #FAA } /* Error */
+.pygments-style-autumn .k { color: #00a } /* Keyword */
+.pygments-style-autumn .ch { color: #aaa; 
+font-style: italic } /* Comment.Hashbang */
+.pygments-style-autumn .cm { color: #aaa; 
+font-style: italic } /* Comment.Multiline */
+.pygments-style-autumn .cp { color: #4c8317 } /* Comment.Preproc */
+.pygments-style-autumn .cpf { color: #aaa; 
+font-style: italic } /* Comment.PreprocFile */
+.pygments-style-autumn .c1 { color: #aaa; 
+font-style: italic } /* Comment.Single */
+.pygments-style-autumn .cs { color: #00a; 
+font-style: italic } /* Comment.Special */
+.pygments-style-autumn .gd { color: #a00 } /* Generic.Deleted */
+.pygments-style-autumn .ge { font-style: italic } /* Generic.Emph */
+.pygments-style-autumn .ges { font-weight: bold; 
+font-style: italic } /* Generic.EmphStrong */
+.pygments-style-autumn .gr { color: #a00 } /* Generic.Error */
+.pygments-style-autumn .gh { color: #000080; 
+font-weight: bold } /* Generic.Heading */
+.pygments-style-autumn .gi { color: #0a0 } /* Generic.Inserted */
+.pygments-style-autumn .go { color: #888 } /* Generic.Output */
+.pygments-style-autumn .gp { color: #555 } /* Generic.Prompt */
+.pygments-style-autumn .gs { font-weight: bold } /* Generic.Strong */
+.pygments-style-autumn .gu { color: #800080; 
+font-weight: bold } /* Generic.Subheading */
+.pygments-style-autumn .gt { color: #a00 } /* Generic.Traceback */
+.pygments-style-autumn .kc { color: #00a } /* Keyword.Constant */
+.pygments-style-autumn .kd { color: #00a } /* Keyword.Declaration */
+.pygments-style-autumn .kn { color: #00a } /* Keyword.Namespace */
+.pygments-style-autumn .kp { color: #00a } /* Keyword.Pseudo */
+.pygments-style-autumn .kr { color: #00a } /* Keyword.Reserved */
+.pygments-style-autumn .kt { color: #0aa } /* Keyword.Type */
+.pygments-style-autumn .m { color: #099 } /* Literal.Number */
+.pygments-style-autumn .s { color: #a50 } /* Literal.String */
+.pygments-style-autumn .na { color: #1e90ff } /* Name.Attribute */
+.pygments-style-autumn .nb { color: #0aa } /* Name.Builtin */
+.pygments-style-autumn .nc { color: #0a0; 
+text-decoration: underline } /* Name.Class */
+.pygments-style-autumn .no { color: #a00 } /* Name.Constant */
+.pygments-style-autumn .nd { color: #888 } /* Name.Decorator */
+.pygments-style-autumn .ni { color: #800; 
+font-weight: bold } /* Name.Entity */
+.pygments-style-autumn .nf { color: #0a0 } /* Name.Function */
+.pygments-style-autumn .nn { color: #0aa; 
+text-decoration: underline } /* Name.Namespace */
+.pygments-style-autumn .nt { color: #1e90ff; 
+font-weight: bold } /* Name.Tag */
+.pygments-style-autumn .nv { color: #a00 } /* Name.Variable */
+.pygments-style-autumn .ow { color: #00a } /* Operator.Word */
+.pygments-style-autumn .w { color: #bbb } /* Text.Whitespace */
+.pygments-style-autumn .mb { color: #099 } /* Literal.Number.Bin */
+.pygments-style-autumn .mf { color: #099 } /* Literal.Number.Float */
+.pygments-style-autumn .mh { color: #099 } /* Literal.Number.Hex */
+.pygments-style-autumn .mi { color: #099 } /* Literal.Number.Integer */
+.pygments-style-autumn .mo { color: #099 } /* Literal.Number.Oct */
+.pygments-style-autumn .sa { color: #a50 } /* Literal.String.Affix */
+.pygments-style-autumn .sb { color: #a50 } /* Literal.String.Backtick */
+.pygments-style-autumn .sc { color: #a50 } /* Literal.String.Char */
+.pygments-style-autumn .dl { color: #a50 } /* Literal.String.Delimiter */
+.pygments-style-autumn .sd { color: #a50 } /* Literal.String.Doc */
+.pygments-style-autumn .s2 { color: #a50 } /* Literal.String.Double */
+.pygments-style-autumn .se { color: #a50 } /* Literal.String.Escape */
+.pygments-style-autumn .sh { color: #a50 } /* Literal.String.Heredoc */
+.pygments-style-autumn .si { color: #a50 } /* Literal.String.Interpol */
+.pygments-style-autumn .sx { color: #a50 } /* Literal.String.Other */
+.pygments-style-autumn .sr { color: #099 } /* Literal.String.Regex */
+.pygments-style-autumn .s1 { color: #a50 } /* Literal.String.Single */
+.pygments-style-autumn .ss { color: #00a } /* Literal.String.Symbol */
+.pygments-style-autumn .bp { color: #0aa } /* Name.Builtin.Pseudo */
+.pygments-style-autumn .fm { color: #0a0 } /* Name.Function.Magic */
+.pygments-style-autumn .vc { color: #a00 } /* Name.Variable.Class */
+.pygments-style-autumn .vg { color: #a00 } /* Name.Variable.Global */
+.pygments-style-autumn .vi { color: #a00 } /* Name.Variable.Instance */
+.pygments-style-autumn .vm { color: #a00 } /* Name.Variable.Magic */
+.pygments-style-autumn .il { color: #099 } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/borland.css` & `plumage-4.0.0/plumage/static/css/pygments/borland.css`

 * *Files 10% similar despite different names*

```diff
@@ -1,138 +1,100 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-.pygments-style-borland .hll { background-color: #ffc; }
-
-.pygments-style-borland {
-  background: #fff;
-}
-
-.pygments-style-borland .c {
-  color: #080;
-  font-style: italic;
-} /* Comment */
-.pygments-style-borland .err {
-  color: #a61717;
-  background-color: #e3d2d2;
-} /* Error */
-.pygments-style-borland .k {
-  color: #000080;
-  font-weight: bold;
-} /* Keyword */
-.pygments-style-borland .ch {
-  color: #080;
-  font-style: italic;
-} /* Comment.Hashbang */
-.pygments-style-borland .cm {
-  color: #080;
-  font-style: italic;
-} /* Comment.Multiline */
-.pygments-style-borland .cp { color: #008080; } /* Comment.Preproc */
-.pygments-style-borland .cpf {
-  color: #080;
-  font-style: italic;
-} /* Comment.PreprocFile */
-.pygments-style-borland .c1 {
-  color: #080;
-  font-style: italic;
-} /* Comment.Single */
-.pygments-style-borland .cs {
-  color: #080;
-  font-weight: bold;
-} /* Comment.Special */
-.pygments-style-borland .gd {
-  color: #000;
-  background-color: #fdd;
-} /* Generic.Deleted */
-.pygments-style-borland .ge { font-style: italic; } /* Generic.Emph */
-.pygments-style-borland .gr { color: #a00; } /* Generic.Error */
-.pygments-style-borland .gh { color: #999; } /* Generic.Heading */
-.pygments-style-borland .gi {
-  color: #000;
-  background-color: #dfd;
-} /* Generic.Inserted */
-.pygments-style-borland .go { color: #888; } /* Generic.Output */
-.pygments-style-borland .gp { color: #555; } /* Generic.Prompt */
-.pygments-style-borland .gs { font-weight: bold; } /* Generic.Strong */
-.pygments-style-borland .gu { color: #aaa; } /* Generic.Subheading */
-.pygments-style-borland .gt { color: #a00; } /* Generic.Traceback */
-.pygments-style-borland .kc {
-  color: #000080;
-  font-weight: bold;
-} /* Keyword.Constant */
-.pygments-style-borland .kd {
-  color: #000080;
-  font-weight: bold;
-} /* Keyword.Declaration */
-.pygments-style-borland .kn {
-  color: #000080;
-  font-weight: bold;
-} /* Keyword.Namespace */
-.pygments-style-borland .kp {
-  color: #000080;
-  font-weight: bold;
-} /* Keyword.Pseudo */
-.pygments-style-borland .kr {
-  color: #000080;
-  font-weight: bold;
-} /* Keyword.Reserved */
-.pygments-style-borland .kt {
-  color: #000080;
-  font-weight: bold;
-} /* Keyword.Type */
-.pygments-style-borland .m { color: #00f; } /* Literal.Number */
-.pygments-style-borland .s { color: #00f; } /* Literal.String */
-.pygments-style-borland .na { color: #f00; } /* Name.Attribute */
-.pygments-style-borland .nt {
-  color: #000080;
-  font-weight: bold;
-} /* Name.Tag */
-.pygments-style-borland .ow { font-weight: bold; } /* Operator.Word */
-.pygments-style-borland .w { color: #bbb; } /* Text.Whitespace */
-.pygments-style-borland .mb { color: #00f; } /* Literal.Number.Bin */
-.pygments-style-borland .mf { color: #00f; } /* Literal.Number.Float */
-.pygments-style-borland .mh { color: #00f; } /* Literal.Number.Hex */
-.pygments-style-borland .mi { color: #00f; } /* Literal.Number.Integer */
-.pygments-style-borland .mo { color: #00f; } /* Literal.Number.Oct */
-.pygments-style-borland .sa { color: #00f; } /* Literal.String.Affix */
-.pygments-style-borland .sb { color: #00f; } /* Literal.String.Backtick */
-.pygments-style-borland .sc { color: #800080; } /* Literal.String.Char */
-.pygments-style-borland .dl { color: #00f; } /* Literal.String.Delimiter */
-.pygments-style-borland .sd { color: #00f; } /* Literal.String.Doc */
-.pygments-style-borland .s2 { color: #00f; } /* Literal.String.Double */
-.pygments-style-borland .se { color: #00f; } /* Literal.String.Escape */
-.pygments-style-borland .sh { color: #00f; } /* Literal.String.Heredoc */
-.pygments-style-borland .si { color: #00f; } /* Literal.String.Interpol */
-.pygments-style-borland .sx { color: #00f; } /* Literal.String.Other */
-.pygments-style-borland .sr { color: #00f; } /* Literal.String.Regex */
-.pygments-style-borland .s1 { color: #00f; } /* Literal.String.Single */
-.pygments-style-borland .ss { color: #00f; } /* Literal.String.Symbol */
-.pygments-style-borland .il { color: #00f; } /* Literal.Number.Integer.Long */
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+.pygments-style-borland .hll { background-color: #ffc }
+
+.pygments-style-borland { background: #fff; 
+}
+
+.pygments-style-borland .c { color: #080; 
+font-style: italic } /* Comment */
+.pygments-style-borland .err { color: #a61717; 
+background-color: #e3d2d2 } /* Error */
+.pygments-style-borland .k { color: #000080; 
+font-weight: bold } /* Keyword */
+.pygments-style-borland .ch { color: #080; 
+font-style: italic } /* Comment.Hashbang */
+.pygments-style-borland .cm { color: #080; 
+font-style: italic } /* Comment.Multiline */
+.pygments-style-borland .cp { color: #008080 } /* Comment.Preproc */
+.pygments-style-borland .cpf { color: #080; 
+font-style: italic } /* Comment.PreprocFile */
+.pygments-style-borland .c1 { color: #080; 
+font-style: italic } /* Comment.Single */
+.pygments-style-borland .cs { color: #080; 
+font-weight: bold } /* Comment.Special */
+.pygments-style-borland .gd { color: #000; 
+background-color: #fdd } /* Generic.Deleted */
+.pygments-style-borland .ge { font-style: italic } /* Generic.Emph */
+.pygments-style-borland .ges { font-weight: bold; 
+font-style: italic } /* Generic.EmphStrong */
+.pygments-style-borland .gr { color: #a00 } /* Generic.Error */
+.pygments-style-borland .gh { color: #999 } /* Generic.Heading */
+.pygments-style-borland .gi { color: #000; 
+background-color: #dfd } /* Generic.Inserted */
+.pygments-style-borland .go { color: #888 } /* Generic.Output */
+.pygments-style-borland .gp { color: #555 } /* Generic.Prompt */
+.pygments-style-borland .gs { font-weight: bold } /* Generic.Strong */
+.pygments-style-borland .gu { color: #aaa } /* Generic.Subheading */
+.pygments-style-borland .gt { color: #a00 } /* Generic.Traceback */
+.pygments-style-borland .kc { color: #000080; 
+font-weight: bold } /* Keyword.Constant */
+.pygments-style-borland .kd { color: #000080; 
+font-weight: bold } /* Keyword.Declaration */
+.pygments-style-borland .kn { color: #000080; 
+font-weight: bold } /* Keyword.Namespace */
+.pygments-style-borland .kp { color: #000080; 
+font-weight: bold } /* Keyword.Pseudo */
+.pygments-style-borland .kr { color: #000080; 
+font-weight: bold } /* Keyword.Reserved */
+.pygments-style-borland .kt { color: #000080; 
+font-weight: bold } /* Keyword.Type */
+.pygments-style-borland .m { color: #00F } /* Literal.Number */
+.pygments-style-borland .s { color: #00F } /* Literal.String */
+.pygments-style-borland .na { color: #F00 } /* Name.Attribute */
+.pygments-style-borland .nt { color: #000080; 
+font-weight: bold } /* Name.Tag */
+.pygments-style-borland .ow { font-weight: bold } /* Operator.Word */
+.pygments-style-borland .w { color: #bbb } /* Text.Whitespace */
+.pygments-style-borland .mb { color: #00F } /* Literal.Number.Bin */
+.pygments-style-borland .mf { color: #00F } /* Literal.Number.Float */
+.pygments-style-borland .mh { color: #00F } /* Literal.Number.Hex */
+.pygments-style-borland .mi { color: #00F } /* Literal.Number.Integer */
+.pygments-style-borland .mo { color: #00F } /* Literal.Number.Oct */
+.pygments-style-borland .sa { color: #00F } /* Literal.String.Affix */
+.pygments-style-borland .sb { color: #00F } /* Literal.String.Backtick */
+.pygments-style-borland .sc { color: #800080 } /* Literal.String.Char */
+.pygments-style-borland .dl { color: #00F } /* Literal.String.Delimiter */
+.pygments-style-borland .sd { color: #00F } /* Literal.String.Doc */
+.pygments-style-borland .s2 { color: #00F } /* Literal.String.Double */
+.pygments-style-borland .se { color: #00F } /* Literal.String.Escape */
+.pygments-style-borland .sh { color: #00F } /* Literal.String.Heredoc */
+.pygments-style-borland .si { color: #00F } /* Literal.String.Interpol */
+.pygments-style-borland .sx { color: #00F } /* Literal.String.Other */
+.pygments-style-borland .sr { color: #00F } /* Literal.String.Regex */
+.pygments-style-borland .s1 { color: #00F } /* Literal.String.Single */
+.pygments-style-borland .ss { color: #00F } /* Literal.String.Symbol */
+.pygments-style-borland .il { color: #00F } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/bw.css` & `plumage-4.0.0/plumage/static/css/pygments/bw.css`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,71 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
-.pygments-style-bw .hll { background-color: #ffc; }
+.pygments-style-bw .hll { background-color: #ffc }
 
-.pygments-style-bw {
-  background: #fff;
+.pygments-style-bw { background: #fff; 
 }
-.pygments-style-bw .c { font-style: italic; } /* Comment */
-.pygments-style-bw .err { border: 1px solid #f00; } /* Error */
-.pygments-style-bw .k { font-weight: bold; } /* Keyword */
-.pygments-style-bw .ch { font-style: italic; } /* Comment.Hashbang */
-.pygments-style-bw .cm { font-style: italic; } /* Comment.Multiline */
-.pygments-style-bw .cpf { font-style: italic; } /* Comment.PreprocFile */
-.pygments-style-bw .c1 { font-style: italic; } /* Comment.Single */
-.pygments-style-bw .cs { font-style: italic; } /* Comment.Special */
-.pygments-style-bw .ge { font-style: italic; } /* Generic.Emph */
-.pygments-style-bw .gh { font-weight: bold; } /* Generic.Heading */
-.pygments-style-bw .gp { font-weight: bold; } /* Generic.Prompt */
-.pygments-style-bw .gs { font-weight: bold; } /* Generic.Strong */
-.pygments-style-bw .gu { font-weight: bold; } /* Generic.Subheading */
-.pygments-style-bw .kc { font-weight: bold; } /* Keyword.Constant */
-.pygments-style-bw .kd { font-weight: bold; } /* Keyword.Declaration */
-.pygments-style-bw .kn { font-weight: bold; } /* Keyword.Namespace */
-.pygments-style-bw .kr { font-weight: bold; } /* Keyword.Reserved */
-.pygments-style-bw .s { font-style: italic; } /* Literal.String */
-.pygments-style-bw .nc { font-weight: bold; } /* Name.Class */
-.pygments-style-bw .ni { font-weight: bold; } /* Name.Entity */
-.pygments-style-bw .ne { font-weight: bold; } /* Name.Exception */
-.pygments-style-bw .nn { font-weight: bold; } /* Name.Namespace */
-.pygments-style-bw .nt { font-weight: bold; } /* Name.Tag */
-.pygments-style-bw .ow { font-weight: bold; } /* Operator.Word */
-.pygments-style-bw .sa { font-style: italic; } /* Literal.String.Affix */
-.pygments-style-bw .sb { font-style: italic; } /* Literal.String.Backtick */
-.pygments-style-bw .sc { font-style: italic; } /* Literal.String.Char */
-.pygments-style-bw .dl { font-style: italic; } /* Literal.String.Delimiter */
-.pygments-style-bw .sd { font-style: italic; } /* Literal.String.Doc */
-.pygments-style-bw .s2 { font-style: italic; } /* Literal.String.Double */
-.pygments-style-bw .se {
-  font-weight: bold;
-  font-style: italic;
-} /* Literal.String.Escape */
-.pygments-style-bw .sh { font-style: italic; } /* Literal.String.Heredoc */
-.pygments-style-bw .si {
-  font-weight: bold;
-  font-style: italic;
-} /* Literal.String.Interpol */
-.pygments-style-bw .sx { font-style: italic; } /* Literal.String.Other */
-.pygments-style-bw .sr { font-style: italic; } /* Literal.String.Regex */
-.pygments-style-bw .s1 { font-style: italic; } /* Literal.String.Single */
-.pygments-style-bw .ss { font-style: italic; } /* Literal.String.Symbol */
+.pygments-style-bw .c { font-style: italic } /* Comment */
+.pygments-style-bw .err { border: 1px solid #F00 } /* Error */
+.pygments-style-bw .k { font-weight: bold } /* Keyword */
+.pygments-style-bw .ch { font-style: italic } /* Comment.Hashbang */
+.pygments-style-bw .cm { font-style: italic } /* Comment.Multiline */
+.pygments-style-bw .cpf { font-style: italic } /* Comment.PreprocFile */
+.pygments-style-bw .c1 { font-style: italic } /* Comment.Single */
+.pygments-style-bw .cs { font-style: italic } /* Comment.Special */
+.pygments-style-bw .ge { font-style: italic } /* Generic.Emph */
+.pygments-style-bw .ges { font-weight: bold; 
+font-style: italic } /* Generic.EmphStrong */
+.pygments-style-bw .gh { font-weight: bold } /* Generic.Heading */
+.pygments-style-bw .gp { font-weight: bold } /* Generic.Prompt */
+.pygments-style-bw .gs { font-weight: bold } /* Generic.Strong */
+.pygments-style-bw .gu { font-weight: bold } /* Generic.Subheading */
+.pygments-style-bw .kc { font-weight: bold } /* Keyword.Constant */
+.pygments-style-bw .kd { font-weight: bold } /* Keyword.Declaration */
+.pygments-style-bw .kn { font-weight: bold } /* Keyword.Namespace */
+.pygments-style-bw .kr { font-weight: bold } /* Keyword.Reserved */
+.pygments-style-bw .s { font-style: italic } /* Literal.String */
+.pygments-style-bw .nc { font-weight: bold } /* Name.Class */
+.pygments-style-bw .ni { font-weight: bold } /* Name.Entity */
+.pygments-style-bw .ne { font-weight: bold } /* Name.Exception */
+.pygments-style-bw .nn { font-weight: bold } /* Name.Namespace */
+.pygments-style-bw .nt { font-weight: bold } /* Name.Tag */
+.pygments-style-bw .ow { font-weight: bold } /* Operator.Word */
+.pygments-style-bw .sa { font-style: italic } /* Literal.String.Affix */
+.pygments-style-bw .sb { font-style: italic } /* Literal.String.Backtick */
+.pygments-style-bw .sc { font-style: italic } /* Literal.String.Char */
+.pygments-style-bw .dl { font-style: italic } /* Literal.String.Delimiter */
+.pygments-style-bw .sd { font-style: italic } /* Literal.String.Doc */
+.pygments-style-bw .s2 { font-style: italic } /* Literal.String.Double */
+.pygments-style-bw .se { font-weight: bold; 
+font-style: italic } /* Literal.String.Escape */
+.pygments-style-bw .sh { font-style: italic } /* Literal.String.Heredoc */
+.pygments-style-bw .si { font-weight: bold; 
+font-style: italic } /* Literal.String.Interpol */
+.pygments-style-bw .sx { font-style: italic } /* Literal.String.Other */
+.pygments-style-bw .sr { font-style: italic } /* Literal.String.Regex */
+.pygments-style-bw .s1 { font-style: italic } /* Literal.String.Single */
+.pygments-style-bw .ss { font-style: italic } /* Literal.String.Symbol */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/colorful.css` & `plumage-4.0.0/plumage/static/css/pygments/colorful.css`

 * *Files 14% similar despite different names*

```diff
@@ -1,203 +1,133 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
-.pygments-style-colorful .hll { background-color: #ffc; }
+.pygments-style-colorful .hll { background-color: #ffc }
 
-.pygments-style-colorful {
-  background: #fff;
+.pygments-style-colorful { background: #fff; 
 }
-.pygments-style-colorful .c { color: #888; } /* Comment */
-.pygments-style-colorful .err {
-  color: #f00;
-  background-color: #faa;
-} /* Error */
-.pygments-style-colorful .k {
-  color: #080;
-  font-weight: bold;
-} /* Keyword */
-.pygments-style-colorful .o { color: #333; } /* Operator */
-.pygments-style-colorful .ch { color: #888; } /* Comment.Hashbang */
-.pygments-style-colorful .cm { color: #888; } /* Comment.Multiline */
-.pygments-style-colorful .cp { color: #579; } /* Comment.Preproc */
-.pygments-style-colorful .cpf { color: #888; } /* Comment.PreprocFile */
-.pygments-style-colorful .c1 { color: #888; } /* Comment.Single */
-.pygments-style-colorful .cs {
-  color: #c00;
-  font-weight: bold;
-} /* Comment.Special */
-.pygments-style-colorful .gd { color: #a00000; } /* Generic.Deleted */
-.pygments-style-colorful .ge { font-style: italic; } /* Generic.Emph */
-.pygments-style-colorful .gr { color: #f00; } /* Generic.Error */
-.pygments-style-colorful .gh {
-  color: #000080;
-  font-weight: bold;
-} /* Generic.Heading */
-.pygments-style-colorful .gi { color: #00a000; } /* Generic.Inserted */
-.pygments-style-colorful .go { color: #888; } /* Generic.Output */
-.pygments-style-colorful .gp {
-  color: #c65d09;
-  font-weight: bold;
-} /* Generic.Prompt */
-.pygments-style-colorful .gs { font-weight: bold; } /* Generic.Strong */
-.pygments-style-colorful .gu {
-  color: #800080;
-  font-weight: bold;
-} /* Generic.Subheading */
-.pygments-style-colorful .gt { color: #04d; } /* Generic.Traceback */
-.pygments-style-colorful .kc {
-  color: #080;
-  font-weight: bold;
-} /* Keyword.Constant */
-.pygments-style-colorful .kd {
-  color: #080;
-  font-weight: bold;
-} /* Keyword.Declaration */
-.pygments-style-colorful .kn {
-  color: #080;
-  font-weight: bold;
-} /* Keyword.Namespace */
-.pygments-style-colorful .kp {
-  color: #038;
-  font-weight: bold;
-} /* Keyword.Pseudo */
-.pygments-style-colorful .kr {
-  color: #080;
-  font-weight: bold;
-} /* Keyword.Reserved */
-.pygments-style-colorful .kt {
-  color: #339;
-  font-weight: bold;
-} /* Keyword.Type */
-.pygments-style-colorful .m {
-  color: #60e;
-  font-weight: bold;
-} /* Literal.Number */
-.pygments-style-colorful .s { background-color: #fff0f0; } /* Literal.String */
-.pygments-style-colorful .na { color: #00c; } /* Name.Attribute */
-.pygments-style-colorful .nb { color: #007020; } /* Name.Builtin */
-.pygments-style-colorful .nc {
-  color: #b06;
-  font-weight: bold;
-} /* Name.Class */
-.pygments-style-colorful .no {
-  color: #036;
-  font-weight: bold;
-} /* Name.Constant */
-.pygments-style-colorful .nd {
-  color: #555;
-  font-weight: bold;
-} /* Name.Decorator */
-.pygments-style-colorful .ni {
-  color: #800;
-  font-weight: bold;
-} /* Name.Entity */
-.pygments-style-colorful .ne {
-  color: #f00;
-  font-weight: bold;
-} /* Name.Exception */
-.pygments-style-colorful .nf {
-  color: #06b;
-  font-weight: bold;
-} /* Name.Function */
-.pygments-style-colorful .nl {
-  color: #970;
-  font-weight: bold;
-} /* Name.Label */
-.pygments-style-colorful .nn {
-  color: #0e84b5;
-  font-weight: bold;
-} /* Name.Namespace */
-.pygments-style-colorful .nt { color: #070; } /* Name.Tag */
-.pygments-style-colorful .nv { color: #963; } /* Name.Variable */
-.pygments-style-colorful .ow {
-  color: #000;
-  font-weight: bold;
-} /* Operator.Word */
-.pygments-style-colorful .w { color: #bbb; } /* Text.Whitespace */
-.pygments-style-colorful .mb {
-  color: #60e;
-  font-weight: bold;
-} /* Literal.Number.Bin */
-.pygments-style-colorful .mf {
-  color: #60e;
-  font-weight: bold;
-} /* Literal.Number.Float */
-.pygments-style-colorful .mh {
-  color: #058;
-  font-weight: bold;
-} /* Literal.Number.Hex */
-.pygments-style-colorful .mi {
-  color: #00d;
-  font-weight: bold;
-} /* Literal.Number.Integer */
-.pygments-style-colorful .mo {
-  color: #40e;
-  font-weight: bold;
-} /* Literal.Number.Oct */
-.pygments-style-colorful .sa { background-color: #fff0f0; } /* Literal.String.Affix */
-.pygments-style-colorful .sb { background-color: #fff0f0; } /* Literal.String.Backtick */
-.pygments-style-colorful .sc { color: #04d; } /* Literal.String.Char */
-.pygments-style-colorful .dl { background-color: #fff0f0; } /* Literal.String.Delimiter */
-.pygments-style-colorful .sd { color: #d42; } /* Literal.String.Doc */
-.pygments-style-colorful .s2 { background-color: #fff0f0; } /* Literal.String.Double */
-.pygments-style-colorful .se {
-  color: #666;
-  font-weight: bold;
-  background-color: #fff0f0;
-} /* Literal.String.Escape */
-.pygments-style-colorful .sh { background-color: #fff0f0; } /* Literal.String.Heredoc */
-.pygments-style-colorful .si { background-color: #eee; } /* Literal.String.Interpol */
-.pygments-style-colorful .sx {
-  color: #d20;
-  background-color: #fff0f0;
-} /* Literal.String.Other */
-.pygments-style-colorful .sr {
-  color: #000;
-  background-color: #fff0ff;
-} /* Literal.String.Regex */
-.pygments-style-colorful .s1 { background-color: #fff0f0; } /* Literal.String.Single */
-.pygments-style-colorful .ss { color: #a60; } /* Literal.String.Symbol */
-.pygments-style-colorful .bp { color: #007020; } /* Name.Builtin.Pseudo */
-.pygments-style-colorful .fm {
-  color: #06b;
-  font-weight: bold;
-} /* Name.Function.Magic */
-.pygments-style-colorful .vc { color: #369; } /* Name.Variable.Class */
-.pygments-style-colorful .vg {
-  color: #d70;
-  font-weight: bold;
-} /* Name.Variable.Global */
-.pygments-style-colorful .vi { color: #33b; } /* Name.Variable.Instance */
-.pygments-style-colorful .vm { color: #963; } /* Name.Variable.Magic */
-.pygments-style-colorful .il {
-  color: #00d;
-  font-weight: bold;
-} /* Literal.Number.Integer.Long */
+.pygments-style-colorful .c { color: #888 } /* Comment */
+.pygments-style-colorful .err { color: #F00; 
+background-color: #FAA } /* Error */
+.pygments-style-colorful .k { color: #080; 
+font-weight: bold } /* Keyword */
+.pygments-style-colorful .o { color: #333 } /* Operator */
+.pygments-style-colorful .ch { color: #888 } /* Comment.Hashbang */
+.pygments-style-colorful .cm { color: #888 } /* Comment.Multiline */
+.pygments-style-colorful .cp { color: #579 } /* Comment.Preproc */
+.pygments-style-colorful .cpf { color: #888 } /* Comment.PreprocFile */
+.pygments-style-colorful .c1 { color: #888 } /* Comment.Single */
+.pygments-style-colorful .cs { color: #c00; 
+font-weight: bold } /* Comment.Special */
+.pygments-style-colorful .gd { color: #A00000 } /* Generic.Deleted */
+.pygments-style-colorful .ge { font-style: italic } /* Generic.Emph */
+.pygments-style-colorful .ges { font-weight: bold; 
+font-style: italic } /* Generic.EmphStrong */
+.pygments-style-colorful .gr { color: #F00 } /* Generic.Error */
+.pygments-style-colorful .gh { color: #000080; 
+font-weight: bold } /* Generic.Heading */
+.pygments-style-colorful .gi { color: #00A000 } /* Generic.Inserted */
+.pygments-style-colorful .go { color: #888 } /* Generic.Output */
+.pygments-style-colorful .gp { color: #c65d09; 
+font-weight: bold } /* Generic.Prompt */
+.pygments-style-colorful .gs { font-weight: bold } /* Generic.Strong */
+.pygments-style-colorful .gu { color: #800080; 
+font-weight: bold } /* Generic.Subheading */
+.pygments-style-colorful .gt { color: #04D } /* Generic.Traceback */
+.pygments-style-colorful .kc { color: #080; 
+font-weight: bold } /* Keyword.Constant */
+.pygments-style-colorful .kd { color: #080; 
+font-weight: bold } /* Keyword.Declaration */
+.pygments-style-colorful .kn { color: #080; 
+font-weight: bold } /* Keyword.Namespace */
+.pygments-style-colorful .kp { color: #038; 
+font-weight: bold } /* Keyword.Pseudo */
+.pygments-style-colorful .kr { color: #080; 
+font-weight: bold } /* Keyword.Reserved */
+.pygments-style-colorful .kt { color: #339; 
+font-weight: bold } /* Keyword.Type */
+.pygments-style-colorful .m { color: #60E; 
+font-weight: bold } /* Literal.Number */
+.pygments-style-colorful .s { background-color: #fff0f0 } /* Literal.String */
+.pygments-style-colorful .na { color: #00C } /* Name.Attribute */
+.pygments-style-colorful .nb { color: #007020 } /* Name.Builtin */
+.pygments-style-colorful .nc { color: #B06; 
+font-weight: bold } /* Name.Class */
+.pygments-style-colorful .no { color: #036; 
+font-weight: bold } /* Name.Constant */
+.pygments-style-colorful .nd { color: #555; 
+font-weight: bold } /* Name.Decorator */
+.pygments-style-colorful .ni { color: #800; 
+font-weight: bold } /* Name.Entity */
+.pygments-style-colorful .ne { color: #F00; 
+font-weight: bold } /* Name.Exception */
+.pygments-style-colorful .nf { color: #06B; 
+font-weight: bold } /* Name.Function */
+.pygments-style-colorful .nl { color: #970; 
+font-weight: bold } /* Name.Label */
+.pygments-style-colorful .nn { color: #0e84b5; 
+font-weight: bold } /* Name.Namespace */
+.pygments-style-colorful .nt { color: #070 } /* Name.Tag */
+.pygments-style-colorful .nv { color: #963 } /* Name.Variable */
+.pygments-style-colorful .ow { color: #000; 
+font-weight: bold } /* Operator.Word */
+.pygments-style-colorful .w { color: #bbb } /* Text.Whitespace */
+.pygments-style-colorful .mb { color: #60E; 
+font-weight: bold } /* Literal.Number.Bin */
+.pygments-style-colorful .mf { color: #60E; 
+font-weight: bold } /* Literal.Number.Float */
+.pygments-style-colorful .mh { color: #058; 
+font-weight: bold } /* Literal.Number.Hex */
+.pygments-style-colorful .mi { color: #00D; 
+font-weight: bold } /* Literal.Number.Integer */
+.pygments-style-colorful .mo { color: #40E; 
+font-weight: bold } /* Literal.Number.Oct */
+.pygments-style-colorful .sa { background-color: #fff0f0 } /* Literal.String.Affix */
+.pygments-style-colorful .sb { background-color: #fff0f0 } /* Literal.String.Backtick */
+.pygments-style-colorful .sc { color: #04D } /* Literal.String.Char */
+.pygments-style-colorful .dl { background-color: #fff0f0 } /* Literal.String.Delimiter */
+.pygments-style-colorful .sd { color: #D42 } /* Literal.String.Doc */
+.pygments-style-colorful .s2 { background-color: #fff0f0 } /* Literal.String.Double */
+.pygments-style-colorful .se { color: #666; 
+font-weight: bold; 
+background-color: #fff0f0 } /* Literal.String.Escape */
+.pygments-style-colorful .sh { background-color: #fff0f0 } /* Literal.String.Heredoc */
+.pygments-style-colorful .si { background-color: #eee } /* Literal.String.Interpol */
+.pygments-style-colorful .sx { color: #D20; 
+background-color: #fff0f0 } /* Literal.String.Other */
+.pygments-style-colorful .sr { color: #000; 
+background-color: #fff0ff } /* Literal.String.Regex */
+.pygments-style-colorful .s1 { background-color: #fff0f0 } /* Literal.String.Single */
+.pygments-style-colorful .ss { color: #A60 } /* Literal.String.Symbol */
+.pygments-style-colorful .bp { color: #007020 } /* Name.Builtin.Pseudo */
+.pygments-style-colorful .fm { color: #06B; 
+font-weight: bold } /* Name.Function.Magic */
+.pygments-style-colorful .vc { color: #369 } /* Name.Variable.Class */
+.pygments-style-colorful .vg { color: #d70; 
+font-weight: bold } /* Name.Variable.Global */
+.pygments-style-colorful .vi { color: #33B } /* Name.Variable.Instance */
+.pygments-style-colorful .vm { color: #963 } /* Name.Variable.Magic */
+.pygments-style-colorful .il { color: #00D; 
+font-weight: bold } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/default.css` & `plumage-4.0.0/plumage/static/css/pygments/default.css`

 * *Files 17% similar despite different names*

```diff
@@ -1,173 +1,123 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-.pygments-style-default .hll { background-color: #ffc; }
-
-.pygments-style-default {
-  background: #f8f8f8;
-}
-
-.pygments-style-default .c {
-  color: #408080;
-  font-style: italic;
-} /* Comment */
-.pygments-style-default .err { border: 1px solid #f00; } /* Error */
-.pygments-style-default .k {
-  color: #008000;
-  font-weight: bold;
-} /* Keyword */
-.pygments-style-default .o { color: #666; } /* Operator */
-.pygments-style-default .ch {
-  color: #408080;
-  font-style: italic;
-} /* Comment.Hashbang */
-.pygments-style-default .cm {
-  color: #408080;
-  font-style: italic;
-} /* Comment.Multiline */
-.pygments-style-default .cp { color: #bc7a00; } /* Comment.Preproc */
-.pygments-style-default .cpf {
-  color: #408080;
-  font-style: italic;
-} /* Comment.PreprocFile */
-.pygments-style-default .c1 {
-  color: #408080;
-  font-style: italic;
-} /* Comment.Single */
-.pygments-style-default .cs {
-  color: #408080;
-  font-style: italic;
-} /* Comment.Special */
-.pygments-style-default .gd { color: #a00000; } /* Generic.Deleted */
-.pygments-style-default .ge { font-style: italic; } /* Generic.Emph */
-.pygments-style-default .gr { color: #f00; } /* Generic.Error */
-.pygments-style-default .gh {
-  color: #000080;
-  font-weight: bold;
-} /* Generic.Heading */
-.pygments-style-default .gi { color: #00a000; } /* Generic.Inserted */
-.pygments-style-default .go { color: #888; } /* Generic.Output */
-.pygments-style-default .gp {
-  color: #000080;
-  font-weight: bold;
-} /* Generic.Prompt */
-.pygments-style-default .gs { font-weight: bold; } /* Generic.Strong */
-.pygments-style-default .gu {
-  color: #800080;
-  font-weight: bold;
-} /* Generic.Subheading */
-.pygments-style-default .gt { color: #04d; } /* Generic.Traceback */
-.pygments-style-default .kc {
-  color: #008000;
-  font-weight: bold;
-} /* Keyword.Constant */
-.pygments-style-default .kd {
-  color: #008000;
-  font-weight: bold;
-} /* Keyword.Declaration */
-.pygments-style-default .kn {
-  color: #008000;
-  font-weight: bold;
-} /* Keyword.Namespace */
-.pygments-style-default .kp { color: #008000; } /* Keyword.Pseudo */
-.pygments-style-default .kr {
-  color: #008000;
-  font-weight: bold;
-} /* Keyword.Reserved */
-.pygments-style-default .kt { color: #b00040; } /* Keyword.Type */
-.pygments-style-default .m { color: #666; } /* Literal.Number */
-.pygments-style-default .s { color: #ba2121; } /* Literal.String */
-.pygments-style-default .na { color: #7d9029; } /* Name.Attribute */
-.pygments-style-default .nb { color: #008000; } /* Name.Builtin */
-.pygments-style-default .nc {
-  color: #00f;
-  font-weight: bold;
-} /* Name.Class */
-.pygments-style-default .no { color: #800; } /* Name.Constant */
-.pygments-style-default .nd { color: #a2f; } /* Name.Decorator */
-.pygments-style-default .ni {
-  color: #999;
-  font-weight: bold;
-} /* Name.Entity */
-.pygments-style-default .ne {
-  color: #d2413a;
-  font-weight: bold;
-} /* Name.Exception */
-.pygments-style-default .nf { color: #00f; } /* Name.Function */
-.pygments-style-default .nl { color: #a0a000; } /* Name.Label */
-.pygments-style-default .nn {
-  color: #00f;
-  font-weight: bold;
-} /* Name.Namespace */
-.pygments-style-default .nt {
-  color: #008000;
-  font-weight: bold;
-} /* Name.Tag */
-.pygments-style-default .nv { color: #19177c; } /* Name.Variable */
-.pygments-style-default .ow {
-  color: #a2f;
-  font-weight: bold;
-} /* Operator.Word */
-.pygments-style-default .w { color: #bbb; } /* Text.Whitespace */
-.pygments-style-default .mb { color: #666; } /* Literal.Number.Bin */
-.pygments-style-default .mf { color: #666; } /* Literal.Number.Float */
-.pygments-style-default .mh { color: #666; } /* Literal.Number.Hex */
-.pygments-style-default .mi { color: #666; } /* Literal.Number.Integer */
-.pygments-style-default .mo { color: #666; } /* Literal.Number.Oct */
-.pygments-style-default .sa { color: #ba2121; } /* Literal.String.Affix */
-.pygments-style-default .sb { color: #ba2121; } /* Literal.String.Backtick */
-.pygments-style-default .sc { color: #ba2121; } /* Literal.String.Char */
-.pygments-style-default .dl { color: #ba2121; } /* Literal.String.Delimiter */
-.pygments-style-default .sd {
-  color: #ba2121;
-  font-style: italic;
-} /* Literal.String.Doc */
-.pygments-style-default .s2 { color: #ba2121; } /* Literal.String.Double */
-.pygments-style-default .se {
-  color: #b62;
-  font-weight: bold;
-} /* Literal.String.Escape */
-.pygments-style-default .sh { color: #ba2121; } /* Literal.String.Heredoc */
-.pygments-style-default .si {
-  color: #b68;
-  font-weight: bold;
-} /* Literal.String.Interpol */
-.pygments-style-default .sx { color: #008000; } /* Literal.String.Other */
-.pygments-style-default .sr { color: #b68; } /* Literal.String.Regex */
-.pygments-style-default .s1 { color: #ba2121; } /* Literal.String.Single */
-.pygments-style-default .ss { color: #19177c; } /* Literal.String.Symbol */
-.pygments-style-default .bp { color: #008000; } /* Name.Builtin.Pseudo */
-.pygments-style-default .fm { color: #00f; } /* Name.Function.Magic */
-.pygments-style-default .vc { color: #19177c; } /* Name.Variable.Class */
-.pygments-style-default .vg { color: #19177c; } /* Name.Variable.Global */
-.pygments-style-default .vi { color: #19177c; } /* Name.Variable.Instance */
-.pygments-style-default .vm { color: #19177c; } /* Name.Variable.Magic */
-.pygments-style-default .il { color: #666; } /* Literal.Number.Integer.Long */
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+.pygments-style-default .hll { background-color: #ffc }
+
+.pygments-style-default { background: #f8f8f8; 
+}
+
+.pygments-style-default .c { color: #3D7B7B; 
+font-style: italic } /* Comment */
+.pygments-style-default .err { border: 1px solid #F00 } /* Error */
+.pygments-style-default .k { color: #008000; 
+font-weight: bold } /* Keyword */
+.pygments-style-default .o { color: #666 } /* Operator */
+.pygments-style-default .ch { color: #3D7B7B; 
+font-style: italic } /* Comment.Hashbang */
+.pygments-style-default .cm { color: #3D7B7B; 
+font-style: italic } /* Comment.Multiline */
+.pygments-style-default .cp { color: #9C6500 } /* Comment.Preproc */
+.pygments-style-default .cpf { color: #3D7B7B; 
+font-style: italic } /* Comment.PreprocFile */
+.pygments-style-default .c1 { color: #3D7B7B; 
+font-style: italic } /* Comment.Single */
+.pygments-style-default .cs { color: #3D7B7B; 
+font-style: italic } /* Comment.Special */
+.pygments-style-default .gd { color: #A00000 } /* Generic.Deleted */
+.pygments-style-default .ge { font-style: italic } /* Generic.Emph */
+.pygments-style-default .ges { font-weight: bold; 
+font-style: italic } /* Generic.EmphStrong */
+.pygments-style-default .gr { color: #E40000 } /* Generic.Error */
+.pygments-style-default .gh { color: #000080; 
+font-weight: bold } /* Generic.Heading */
+.pygments-style-default .gi { color: #008400 } /* Generic.Inserted */
+.pygments-style-default .go { color: #717171 } /* Generic.Output */
+.pygments-style-default .gp { color: #000080; 
+font-weight: bold } /* Generic.Prompt */
+.pygments-style-default .gs { font-weight: bold } /* Generic.Strong */
+.pygments-style-default .gu { color: #800080; 
+font-weight: bold } /* Generic.Subheading */
+.pygments-style-default .gt { color: #04D } /* Generic.Traceback */
+.pygments-style-default .kc { color: #008000; 
+font-weight: bold } /* Keyword.Constant */
+.pygments-style-default .kd { color: #008000; 
+font-weight: bold } /* Keyword.Declaration */
+.pygments-style-default .kn { color: #008000; 
+font-weight: bold } /* Keyword.Namespace */
+.pygments-style-default .kp { color: #008000 } /* Keyword.Pseudo */
+.pygments-style-default .kr { color: #008000; 
+font-weight: bold } /* Keyword.Reserved */
+.pygments-style-default .kt { color: #B00040 } /* Keyword.Type */
+.pygments-style-default .m { color: #666 } /* Literal.Number */
+.pygments-style-default .s { color: #BA2121 } /* Literal.String */
+.pygments-style-default .na { color: #687822 } /* Name.Attribute */
+.pygments-style-default .nb { color: #008000 } /* Name.Builtin */
+.pygments-style-default .nc { color: #00F; 
+font-weight: bold } /* Name.Class */
+.pygments-style-default .no { color: #800 } /* Name.Constant */
+.pygments-style-default .nd { color: #A2F } /* Name.Decorator */
+.pygments-style-default .ni { color: #717171; 
+font-weight: bold } /* Name.Entity */
+.pygments-style-default .ne { color: #CB3F38; 
+font-weight: bold } /* Name.Exception */
+.pygments-style-default .nf { color: #00F } /* Name.Function */
+.pygments-style-default .nl { color: #767600 } /* Name.Label */
+.pygments-style-default .nn { color: #00F; 
+font-weight: bold } /* Name.Namespace */
+.pygments-style-default .nt { color: #008000; 
+font-weight: bold } /* Name.Tag */
+.pygments-style-default .nv { color: #19177C } /* Name.Variable */
+.pygments-style-default .ow { color: #A2F; 
+font-weight: bold } /* Operator.Word */
+.pygments-style-default .w { color: #bbb } /* Text.Whitespace */
+.pygments-style-default .mb { color: #666 } /* Literal.Number.Bin */
+.pygments-style-default .mf { color: #666 } /* Literal.Number.Float */
+.pygments-style-default .mh { color: #666 } /* Literal.Number.Hex */
+.pygments-style-default .mi { color: #666 } /* Literal.Number.Integer */
+.pygments-style-default .mo { color: #666 } /* Literal.Number.Oct */
+.pygments-style-default .sa { color: #BA2121 } /* Literal.String.Affix */
+.pygments-style-default .sb { color: #BA2121 } /* Literal.String.Backtick */
+.pygments-style-default .sc { color: #BA2121 } /* Literal.String.Char */
+.pygments-style-default .dl { color: #BA2121 } /* Literal.String.Delimiter */
+.pygments-style-default .sd { color: #BA2121; 
+font-style: italic } /* Literal.String.Doc */
+.pygments-style-default .s2 { color: #BA2121 } /* Literal.String.Double */
+.pygments-style-default .se { color: #AA5D1F; 
+font-weight: bold } /* Literal.String.Escape */
+.pygments-style-default .sh { color: #BA2121 } /* Literal.String.Heredoc */
+.pygments-style-default .si { color: #A45A77; 
+font-weight: bold } /* Literal.String.Interpol */
+.pygments-style-default .sx { color: #008000 } /* Literal.String.Other */
+.pygments-style-default .sr { color: #A45A77 } /* Literal.String.Regex */
+.pygments-style-default .s1 { color: #BA2121 } /* Literal.String.Single */
+.pygments-style-default .ss { color: #19177C } /* Literal.String.Symbol */
+.pygments-style-default .bp { color: #008000 } /* Name.Builtin.Pseudo */
+.pygments-style-default .fm { color: #00F } /* Name.Function.Magic */
+.pygments-style-default .vc { color: #19177C } /* Name.Variable.Class */
+.pygments-style-default .vg { color: #19177C } /* Name.Variable.Global */
+.pygments-style-default .vi { color: #19177C } /* Name.Variable.Instance */
+.pygments-style-default .vm { color: #19177C } /* Name.Variable.Magic */
+.pygments-style-default .il { color: #666 } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/emacs.css` & `plumage-4.0.0/plumage/static/css/pygments/tango.css`

 * *Files 26% similar despite different names*

```diff
@@ -1,173 +1,146 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-.pygments-style-emacs .hll { background-color: #ffc; }
-
-.pygments-style-emacs {
-  background: #f8f8f8;
-}
-
-.pygments-style-emacs .c {
-  color: #080;
-  font-style: italic;
-} /* Comment */
-.pygments-style-emacs .err { border: 1px solid #f00; } /* Error */
-.pygments-style-emacs .k {
-  color: #a2f;
-  font-weight: bold;
-} /* Keyword */
-.pygments-style-emacs .o { color: #666; } /* Operator */
-.pygments-style-emacs .ch {
-  color: #080;
-  font-style: italic;
-} /* Comment.Hashbang */
-.pygments-style-emacs .cm {
-  color: #080;
-  font-style: italic;
-} /* Comment.Multiline */
-.pygments-style-emacs .cp { color: #080; } /* Comment.Preproc */
-.pygments-style-emacs .cpf {
-  color: #080;
-  font-style: italic;
-} /* Comment.PreprocFile */
-.pygments-style-emacs .c1 {
-  color: #080;
-  font-style: italic;
-} /* Comment.Single */
-.pygments-style-emacs .cs {
-  color: #080;
-  font-weight: bold;
-} /* Comment.Special */
-.pygments-style-emacs .gd { color: #a00000; } /* Generic.Deleted */
-.pygments-style-emacs .ge { font-style: italic; } /* Generic.Emph */
-.pygments-style-emacs .gr { color: #f00; } /* Generic.Error */
-.pygments-style-emacs .gh {
-  color: #000080;
-  font-weight: bold;
-} /* Generic.Heading */
-.pygments-style-emacs .gi { color: #00a000; } /* Generic.Inserted */
-.pygments-style-emacs .go { color: #888; } /* Generic.Output */
-.pygments-style-emacs .gp {
-  color: #000080;
-  font-weight: bold;
-} /* Generic.Prompt */
-.pygments-style-emacs .gs { font-weight: bold; } /* Generic.Strong */
-.pygments-style-emacs .gu {
-  color: #800080;
-  font-weight: bold;
-} /* Generic.Subheading */
-.pygments-style-emacs .gt { color: #04d; } /* Generic.Traceback */
-.pygments-style-emacs .kc {
-  color: #a2f;
-  font-weight: bold;
-} /* Keyword.Constant */
-.pygments-style-emacs .kd {
-  color: #a2f;
-  font-weight: bold;
-} /* Keyword.Declaration */
-.pygments-style-emacs .kn {
-  color: #a2f;
-  font-weight: bold;
-} /* Keyword.Namespace */
-.pygments-style-emacs .kp { color: #a2f; } /* Keyword.Pseudo */
-.pygments-style-emacs .kr {
-  color: #a2f;
-  font-weight: bold;
-} /* Keyword.Reserved */
-.pygments-style-emacs .kt {
-  color: #0b0;
-  font-weight: bold;
-} /* Keyword.Type */
-.pygments-style-emacs .m { color: #666; } /* Literal.Number */
-.pygments-style-emacs .s { color: #b44; } /* Literal.String */
-.pygments-style-emacs .na { color: #b44; } /* Name.Attribute */
-.pygments-style-emacs .nb { color: #a2f; } /* Name.Builtin */
-.pygments-style-emacs .nc { color: #00f; } /* Name.Class */
-.pygments-style-emacs .no { color: #800; } /* Name.Constant */
-.pygments-style-emacs .nd { color: #a2f; } /* Name.Decorator */
-.pygments-style-emacs .ni {
-  color: #999;
-  font-weight: bold;
-} /* Name.Entity */
-.pygments-style-emacs .ne {
-  color: #d2413a;
-  font-weight: bold;
-} /* Name.Exception */
-.pygments-style-emacs .nf { color: #00a000; } /* Name.Function */
-.pygments-style-emacs .nl { color: #a0a000; } /* Name.Label */
-.pygments-style-emacs .nn {
-  color: #00f;
-  font-weight: bold;
-} /* Name.Namespace */
-.pygments-style-emacs .nt {
-  color: #008000;
-  font-weight: bold;
-} /* Name.Tag */
-.pygments-style-emacs .nv { color: #b8860b; } /* Name.Variable */
-.pygments-style-emacs .ow {
-  color: #a2f;
-  font-weight: bold;
-} /* Operator.Word */
-.pygments-style-emacs .w { color: #bbb; } /* Text.Whitespace */
-.pygments-style-emacs .mb { color: #666; } /* Literal.Number.Bin */
-.pygments-style-emacs .mf { color: #666; } /* Literal.Number.Float */
-.pygments-style-emacs .mh { color: #666; } /* Literal.Number.Hex */
-.pygments-style-emacs .mi { color: #666; } /* Literal.Number.Integer */
-.pygments-style-emacs .mo { color: #666; } /* Literal.Number.Oct */
-.pygments-style-emacs .sa { color: #b44; } /* Literal.String.Affix */
-.pygments-style-emacs .sb { color: #b44; } /* Literal.String.Backtick */
-.pygments-style-emacs .sc { color: #b44; } /* Literal.String.Char */
-.pygments-style-emacs .dl { color: #b44; } /* Literal.String.Delimiter */
-.pygments-style-emacs .sd {
-  color: #b44;
-  font-style: italic;
-} /* Literal.String.Doc */
-.pygments-style-emacs .s2 { color: #b44; } /* Literal.String.Double */
-.pygments-style-emacs .se {
-  color: #b62;
-  font-weight: bold;
-} /* Literal.String.Escape */
-.pygments-style-emacs .sh { color: #b44; } /* Literal.String.Heredoc */
-.pygments-style-emacs .si {
-  color: #b68;
-  font-weight: bold;
-} /* Literal.String.Interpol */
-.pygments-style-emacs .sx { color: #008000; } /* Literal.String.Other */
-.pygments-style-emacs .sr { color: #b68; } /* Literal.String.Regex */
-.pygments-style-emacs .s1 { color: #b44; } /* Literal.String.Single */
-.pygments-style-emacs .ss { color: #b8860b; } /* Literal.String.Symbol */
-.pygments-style-emacs .bp { color: #a2f; } /* Name.Builtin.Pseudo */
-.pygments-style-emacs .fm { color: #00a000; } /* Name.Function.Magic */
-.pygments-style-emacs .vc { color: #b8860b; } /* Name.Variable.Class */
-.pygments-style-emacs .vg { color: #b8860b; } /* Name.Variable.Global */
-.pygments-style-emacs .vi { color: #b8860b; } /* Name.Variable.Instance */
-.pygments-style-emacs .vm { color: #b8860b; } /* Name.Variable.Magic */
-.pygments-style-emacs .il { color: #666; } /* Literal.Number.Integer.Long */
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+.pygments-style-tango .hll { background-color: #ffc }
+
+.pygments-style-tango { background: #f8f8f8; 
+}
+
+.pygments-style-tango .c { color: #8f5902; 
+font-style: italic } /* Comment */
+.pygments-style-tango .err { color: #a40000; 
+border: 1px solid #ef2929 } /* Error */
+.pygments-style-tango .g { color: #000 } /* Generic */
+.pygments-style-tango .k { color: #204a87; 
+font-weight: bold } /* Keyword */
+.pygments-style-tango .l { color: #000 } /* Literal */
+.pygments-style-tango .n { color: #000 } /* Name */
+.pygments-style-tango .o { color: #ce5c00; 
+font-weight: bold } /* Operator */
+.pygments-style-tango .x { color: #000 } /* Other */
+.pygments-style-tango .p { color: #000; 
+font-weight: bold } /* Punctuation */
+.pygments-style-tango .ch { color: #8f5902; 
+font-style: italic } /* Comment.Hashbang */
+.pygments-style-tango .cm { color: #8f5902; 
+font-style: italic } /* Comment.Multiline */
+.pygments-style-tango .cp { color: #8f5902; 
+font-style: italic } /* Comment.Preproc */
+.pygments-style-tango .cpf { color: #8f5902; 
+font-style: italic } /* Comment.PreprocFile */
+.pygments-style-tango .c1 { color: #8f5902; 
+font-style: italic } /* Comment.Single */
+.pygments-style-tango .cs { color: #8f5902; 
+font-style: italic } /* Comment.Special */
+.pygments-style-tango .gd { color: #a40000 } /* Generic.Deleted */
+.pygments-style-tango .ge { color: #000; 
+font-style: italic } /* Generic.Emph */
+.pygments-style-tango .ges { color: #000; 
+font-weight: bold; 
+font-style: italic } /* Generic.EmphStrong */
+.pygments-style-tango .gr { color: #ef2929 } /* Generic.Error */
+.pygments-style-tango .gh { color: #000080; 
+font-weight: bold } /* Generic.Heading */
+.pygments-style-tango .gi { color: #00A000 } /* Generic.Inserted */
+.pygments-style-tango .go { color: #000; 
+font-style: italic } /* Generic.Output */
+.pygments-style-tango .gp { color: #8f5902 } /* Generic.Prompt */
+.pygments-style-tango .gs { color: #000; 
+font-weight: bold } /* Generic.Strong */
+.pygments-style-tango .gu { color: #800080; 
+font-weight: bold } /* Generic.Subheading */
+.pygments-style-tango .gt { color: #a40000; 
+font-weight: bold } /* Generic.Traceback */
+.pygments-style-tango .kc { color: #204a87; 
+font-weight: bold } /* Keyword.Constant */
+.pygments-style-tango .kd { color: #204a87; 
+font-weight: bold } /* Keyword.Declaration */
+.pygments-style-tango .kn { color: #204a87; 
+font-weight: bold } /* Keyword.Namespace */
+.pygments-style-tango .kp { color: #204a87; 
+font-weight: bold } /* Keyword.Pseudo */
+.pygments-style-tango .kr { color: #204a87; 
+font-weight: bold } /* Keyword.Reserved */
+.pygments-style-tango .kt { color: #204a87; 
+font-weight: bold } /* Keyword.Type */
+.pygments-style-tango .ld { color: #000 } /* Literal.Date */
+.pygments-style-tango .m { color: #0000cf; 
+font-weight: bold } /* Literal.Number */
+.pygments-style-tango .s { color: #4e9a06 } /* Literal.String */
+.pygments-style-tango .na { color: #c4a000 } /* Name.Attribute */
+.pygments-style-tango .nb { color: #204a87 } /* Name.Builtin */
+.pygments-style-tango .nc { color: #000 } /* Name.Class */
+.pygments-style-tango .no { color: #000 } /* Name.Constant */
+.pygments-style-tango .nd { color: #5c35cc; 
+font-weight: bold } /* Name.Decorator */
+.pygments-style-tango .ni { color: #ce5c00 } /* Name.Entity */
+.pygments-style-tango .ne { color: #c00; 
+font-weight: bold } /* Name.Exception */
+.pygments-style-tango .nf { color: #000 } /* Name.Function */
+.pygments-style-tango .nl { color: #f57900 } /* Name.Label */
+.pygments-style-tango .nn { color: #000 } /* Name.Namespace */
+.pygments-style-tango .nx { color: #000 } /* Name.Other */
+.pygments-style-tango .py { color: #000 } /* Name.Property */
+.pygments-style-tango .nt { color: #204a87; 
+font-weight: bold } /* Name.Tag */
+.pygments-style-tango .nv { color: #000 } /* Name.Variable */
+.pygments-style-tango .ow { color: #204a87; 
+font-weight: bold } /* Operator.Word */
+.pygments-style-tango .pm { color: #000; 
+font-weight: bold } /* Punctuation.Marker */
+.pygments-style-tango .w { color: #f8f8f8 } /* Text.Whitespace */
+.pygments-style-tango .mb { color: #0000cf; 
+font-weight: bold } /* Literal.Number.Bin */
+.pygments-style-tango .mf { color: #0000cf; 
+font-weight: bold } /* Literal.Number.Float */
+.pygments-style-tango .mh { color: #0000cf; 
+font-weight: bold } /* Literal.Number.Hex */
+.pygments-style-tango .mi { color: #0000cf; 
+font-weight: bold } /* Literal.Number.Integer */
+.pygments-style-tango .mo { color: #0000cf; 
+font-weight: bold } /* Literal.Number.Oct */
+.pygments-style-tango .sa { color: #4e9a06 } /* Literal.String.Affix */
+.pygments-style-tango .sb { color: #4e9a06 } /* Literal.String.Backtick */
+.pygments-style-tango .sc { color: #4e9a06 } /* Literal.String.Char */
+.pygments-style-tango .dl { color: #4e9a06 } /* Literal.String.Delimiter */
+.pygments-style-tango .sd { color: #8f5902; 
+font-style: italic } /* Literal.String.Doc */
+.pygments-style-tango .s2 { color: #4e9a06 } /* Literal.String.Double */
+.pygments-style-tango .se { color: #4e9a06 } /* Literal.String.Escape */
+.pygments-style-tango .sh { color: #4e9a06 } /* Literal.String.Heredoc */
+.pygments-style-tango .si { color: #4e9a06 } /* Literal.String.Interpol */
+.pygments-style-tango .sx { color: #4e9a06 } /* Literal.String.Other */
+.pygments-style-tango .sr { color: #4e9a06 } /* Literal.String.Regex */
+.pygments-style-tango .s1 { color: #4e9a06 } /* Literal.String.Single */
+.pygments-style-tango .ss { color: #4e9a06 } /* Literal.String.Symbol */
+.pygments-style-tango .bp { color: #3465a4 } /* Name.Builtin.Pseudo */
+.pygments-style-tango .fm { color: #000 } /* Name.Function.Magic */
+.pygments-style-tango .vc { color: #000 } /* Name.Variable.Class */
+.pygments-style-tango .vg { color: #000 } /* Name.Variable.Global */
+.pygments-style-tango .vi { color: #000 } /* Name.Variable.Instance */
+.pygments-style-tango .vm { color: #000 } /* Name.Variable.Magic */
+.pygments-style-tango .il { color: #0000cf; 
+font-weight: bold } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/friendly.css` & `plumage-4.0.0/plumage/static/css/pygments/friendly.css`

 * *Files 18% similar despite different names*

```diff
@@ -1,176 +1,124 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-.pygments-style-friendly .hll { background-color: #ffc; }
-
-.pygments-style-friendly {
-  background: #f0f0f0;
-}
-
-.pygments-style-friendly .c {
-  color: #60a0b0;
-  font-style: italic;
-} /* Comment */
-.pygments-style-friendly .err { border: 1px solid #f00; } /* Error */
-.pygments-style-friendly .k {
-  color: #007020;
-  font-weight: bold;
-} /* Keyword */
-.pygments-style-friendly .o { color: #666; } /* Operator */
-.pygments-style-friendly .ch {
-  color: #60a0b0;
-  font-style: italic;
-} /* Comment.Hashbang */
-.pygments-style-friendly .cm {
-  color: #60a0b0;
-  font-style: italic;
-} /* Comment.Multiline */
-.pygments-style-friendly .cp { color: #007020; } /* Comment.Preproc */
-.pygments-style-friendly .cpf {
-  color: #60a0b0;
-  font-style: italic;
-} /* Comment.PreprocFile */
-.pygments-style-friendly .c1 {
-  color: #60a0b0;
-  font-style: italic;
-} /* Comment.Single */
-.pygments-style-friendly .cs {
-  color: #60a0b0;
-  background-color: #fff0f0;
-} /* Comment.Special */
-.pygments-style-friendly .gd { color: #a00000; } /* Generic.Deleted */
-.pygments-style-friendly .ge { font-style: italic; } /* Generic.Emph */
-.pygments-style-friendly .gr { color: #f00; } /* Generic.Error */
-.pygments-style-friendly .gh {
-  color: #000080;
-  font-weight: bold;
-} /* Generic.Heading */
-.pygments-style-friendly .gi { color: #00a000; } /* Generic.Inserted */
-.pygments-style-friendly .go { color: #888; } /* Generic.Output */
-.pygments-style-friendly .gp {
-  color: #c65d09;
-  font-weight: bold;
-} /* Generic.Prompt */
-.pygments-style-friendly .gs { font-weight: bold; } /* Generic.Strong */
-.pygments-style-friendly .gu {
-  color: #800080;
-  font-weight: bold;
-} /* Generic.Subheading */
-.pygments-style-friendly .gt { color: #04d; } /* Generic.Traceback */
-.pygments-style-friendly .kc {
-  color: #007020;
-  font-weight: bold;
-} /* Keyword.Constant */
-.pygments-style-friendly .kd {
-  color: #007020;
-  font-weight: bold;
-} /* Keyword.Declaration */
-.pygments-style-friendly .kn {
-  color: #007020;
-  font-weight: bold;
-} /* Keyword.Namespace */
-.pygments-style-friendly .kp { color: #007020; } /* Keyword.Pseudo */
-.pygments-style-friendly .kr {
-  color: #007020;
-  font-weight: bold;
-} /* Keyword.Reserved */
-.pygments-style-friendly .kt { color: #902000; } /* Keyword.Type */
-.pygments-style-friendly .m { color: #40a070; } /* Literal.Number */
-.pygments-style-friendly .s { color: #4070a0; } /* Literal.String */
-.pygments-style-friendly .na { color: #4070a0; } /* Name.Attribute */
-.pygments-style-friendly .nb { color: #007020; } /* Name.Builtin */
-.pygments-style-friendly .nc {
-  color: #0e84b5;
-  font-weight: bold;
-} /* Name.Class */
-.pygments-style-friendly .no { color: #60add5; } /* Name.Constant */
-.pygments-style-friendly .nd {
-  color: #555;
-  font-weight: bold;
-} /* Name.Decorator */
-.pygments-style-friendly .ni {
-  color: #d55537;
-  font-weight: bold;
-} /* Name.Entity */
-.pygments-style-friendly .ne { color: #007020; } /* Name.Exception */
-.pygments-style-friendly .nf { color: #06287e; } /* Name.Function */
-.pygments-style-friendly .nl {
-  color: #002070;
-  font-weight: bold;
-} /* Name.Label */
-.pygments-style-friendly .nn {
-  color: #0e84b5;
-  font-weight: bold;
-} /* Name.Namespace */
-.pygments-style-friendly .nt {
-  color: #062873;
-  font-weight: bold;
-} /* Name.Tag */
-.pygments-style-friendly .nv { color: #bb60d5; } /* Name.Variable */
-.pygments-style-friendly .ow {
-  color: #007020;
-  font-weight: bold;
-} /* Operator.Word */
-.pygments-style-friendly .w { color: #bbb; } /* Text.Whitespace */
-.pygments-style-friendly .mb { color: #40a070; } /* Literal.Number.Bin */
-.pygments-style-friendly .mf { color: #40a070; } /* Literal.Number.Float */
-.pygments-style-friendly .mh { color: #40a070; } /* Literal.Number.Hex */
-.pygments-style-friendly .mi { color: #40a070; } /* Literal.Number.Integer */
-.pygments-style-friendly .mo { color: #40a070; } /* Literal.Number.Oct */
-.pygments-style-friendly .sa { color: #4070a0; } /* Literal.String.Affix */
-.pygments-style-friendly .sb { color: #4070a0; } /* Literal.String.Backtick */
-.pygments-style-friendly .sc { color: #4070a0; } /* Literal.String.Char */
-.pygments-style-friendly .dl { color: #4070a0; } /* Literal.String.Delimiter */
-.pygments-style-friendly .sd {
-  color: #4070a0;
-  font-style: italic;
-} /* Literal.String.Doc */
-.pygments-style-friendly .s2 { color: #4070a0; } /* Literal.String.Double */
-.pygments-style-friendly .se {
-  color: #4070a0;
-  font-weight: bold;
-} /* Literal.String.Escape */
-.pygments-style-friendly .sh { color: #4070a0; } /* Literal.String.Heredoc */
-.pygments-style-friendly .si {
-  color: #70a0d0;
-  font-style: italic;
-} /* Literal.String.Interpol */
-.pygments-style-friendly .sx { color: #c65d09; } /* Literal.String.Other */
-.pygments-style-friendly .sr { color: #235388; } /* Literal.String.Regex */
-.pygments-style-friendly .s1 { color: #4070a0; } /* Literal.String.Single */
-.pygments-style-friendly .ss { color: #517918; } /* Literal.String.Symbol */
-.pygments-style-friendly .bp { color: #007020; } /* Name.Builtin.Pseudo */
-.pygments-style-friendly .fm { color: #06287e; } /* Name.Function.Magic */
-.pygments-style-friendly .vc { color: #bb60d5; } /* Name.Variable.Class */
-.pygments-style-friendly .vg { color: #bb60d5; } /* Name.Variable.Global */
-.pygments-style-friendly .vi { color: #bb60d5; } /* Name.Variable.Instance */
-.pygments-style-friendly .vm { color: #bb60d5; } /* Name.Variable.Magic */
-.pygments-style-friendly .il { color: #40a070; } /* Literal.Number.Integer.Long */
+td.linenos .normal { color: #666; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos { color: #666; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+.pygments-style-friendly .hll { background-color: #ffc }
+
+.pygments-style-friendly { background: #f0f0f0; 
+}
+
+.pygments-style-friendly .c { color: #60a0b0; 
+font-style: italic } /* Comment */
+.pygments-style-friendly .err { border: 1px solid #F00 } /* Error */
+.pygments-style-friendly .k { color: #007020; 
+font-weight: bold } /* Keyword */
+.pygments-style-friendly .o { color: #666 } /* Operator */
+.pygments-style-friendly .ch { color: #60a0b0; 
+font-style: italic } /* Comment.Hashbang */
+.pygments-style-friendly .cm { color: #60a0b0; 
+font-style: italic } /* Comment.Multiline */
+.pygments-style-friendly .cp { color: #007020 } /* Comment.Preproc */
+.pygments-style-friendly .cpf { color: #60a0b0; 
+font-style: italic } /* Comment.PreprocFile */
+.pygments-style-friendly .c1 { color: #60a0b0; 
+font-style: italic } /* Comment.Single */
+.pygments-style-friendly .cs { color: #60a0b0; 
+background-color: #fff0f0 } /* Comment.Special */
+.pygments-style-friendly .gd { color: #A00000 } /* Generic.Deleted */
+.pygments-style-friendly .ge { font-style: italic } /* Generic.Emph */
+.pygments-style-friendly .ges { font-weight: bold; 
+font-style: italic } /* Generic.EmphStrong */
+.pygments-style-friendly .gr { color: #F00 } /* Generic.Error */
+.pygments-style-friendly .gh { color: #000080; 
+font-weight: bold } /* Generic.Heading */
+.pygments-style-friendly .gi { color: #00A000 } /* Generic.Inserted */
+.pygments-style-friendly .go { color: #888 } /* Generic.Output */
+.pygments-style-friendly .gp { color: #c65d09; 
+font-weight: bold } /* Generic.Prompt */
+.pygments-style-friendly .gs { font-weight: bold } /* Generic.Strong */
+.pygments-style-friendly .gu { color: #800080; 
+font-weight: bold } /* Generic.Subheading */
+.pygments-style-friendly .gt { color: #04D } /* Generic.Traceback */
+.pygments-style-friendly .kc { color: #007020; 
+font-weight: bold } /* Keyword.Constant */
+.pygments-style-friendly .kd { color: #007020; 
+font-weight: bold } /* Keyword.Declaration */
+.pygments-style-friendly .kn { color: #007020; 
+font-weight: bold } /* Keyword.Namespace */
+.pygments-style-friendly .kp { color: #007020 } /* Keyword.Pseudo */
+.pygments-style-friendly .kr { color: #007020; 
+font-weight: bold } /* Keyword.Reserved */
+.pygments-style-friendly .kt { color: #902000 } /* Keyword.Type */
+.pygments-style-friendly .m { color: #40a070 } /* Literal.Number */
+.pygments-style-friendly .s { color: #4070a0 } /* Literal.String */
+.pygments-style-friendly .na { color: #4070a0 } /* Name.Attribute */
+.pygments-style-friendly .nb { color: #007020 } /* Name.Builtin */
+.pygments-style-friendly .nc { color: #0e84b5; 
+font-weight: bold } /* Name.Class */
+.pygments-style-friendly .no { color: #60add5 } /* Name.Constant */
+.pygments-style-friendly .nd { color: #555; 
+font-weight: bold } /* Name.Decorator */
+.pygments-style-friendly .ni { color: #d55537; 
+font-weight: bold } /* Name.Entity */
+.pygments-style-friendly .ne { color: #007020 } /* Name.Exception */
+.pygments-style-friendly .nf { color: #06287e } /* Name.Function */
+.pygments-style-friendly .nl { color: #002070; 
+font-weight: bold } /* Name.Label */
+.pygments-style-friendly .nn { color: #0e84b5; 
+font-weight: bold } /* Name.Namespace */
+.pygments-style-friendly .nt { color: #062873; 
+font-weight: bold } /* Name.Tag */
+.pygments-style-friendly .nv { color: #bb60d5 } /* Name.Variable */
+.pygments-style-friendly .ow { color: #007020; 
+font-weight: bold } /* Operator.Word */
+.pygments-style-friendly .w { color: #bbb } /* Text.Whitespace */
+.pygments-style-friendly .mb { color: #40a070 } /* Literal.Number.Bin */
+.pygments-style-friendly .mf { color: #40a070 } /* Literal.Number.Float */
+.pygments-style-friendly .mh { color: #40a070 } /* Literal.Number.Hex */
+.pygments-style-friendly .mi { color: #40a070 } /* Literal.Number.Integer */
+.pygments-style-friendly .mo { color: #40a070 } /* Literal.Number.Oct */
+.pygments-style-friendly .sa { color: #4070a0 } /* Literal.String.Affix */
+.pygments-style-friendly .sb { color: #4070a0 } /* Literal.String.Backtick */
+.pygments-style-friendly .sc { color: #4070a0 } /* Literal.String.Char */
+.pygments-style-friendly .dl { color: #4070a0 } /* Literal.String.Delimiter */
+.pygments-style-friendly .sd { color: #4070a0; 
+font-style: italic } /* Literal.String.Doc */
+.pygments-style-friendly .s2 { color: #4070a0 } /* Literal.String.Double */
+.pygments-style-friendly .se { color: #4070a0; 
+font-weight: bold } /* Literal.String.Escape */
+.pygments-style-friendly .sh { color: #4070a0 } /* Literal.String.Heredoc */
+.pygments-style-friendly .si { color: #70a0d0; 
+font-style: italic } /* Literal.String.Interpol */
+.pygments-style-friendly .sx { color: #c65d09 } /* Literal.String.Other */
+.pygments-style-friendly .sr { color: #235388 } /* Literal.String.Regex */
+.pygments-style-friendly .s1 { color: #4070a0 } /* Literal.String.Single */
+.pygments-style-friendly .ss { color: #517918 } /* Literal.String.Symbol */
+.pygments-style-friendly .bp { color: #007020 } /* Name.Builtin.Pseudo */
+.pygments-style-friendly .fm { color: #06287e } /* Name.Function.Magic */
+.pygments-style-friendly .vc { color: #bb60d5 } /* Name.Variable.Class */
+.pygments-style-friendly .vg { color: #bb60d5 } /* Name.Variable.Global */
+.pygments-style-friendly .vi { color: #bb60d5 } /* Name.Variable.Instance */
+.pygments-style-friendly .vm { color: #bb60d5 } /* Name.Variable.Magic */
+.pygments-style-friendly .il { color: #40a070 } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/fruity.css` & `plumage-4.0.0/plumage/static/css/pygments/fruity.css`

 * *Files 10% similar despite different names*

```diff
@@ -1,203 +1,144 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-.pygments-style-fruity .hll { background-color: #333; }
-
-.pygments-style-fruity {
-  background: #111;
-  color: #fff;
-}
-
-.pygments-style-fruity .c {
-  color: #080;
-  font-style: italic;
-  background-color: #0f140f;
-} /* Comment */
-.pygments-style-fruity .err { color: #fff; } /* Error */
-.pygments-style-fruity .esc { color: #fff; } /* Escape */
-.pygments-style-fruity .g { color: #fff; } /* Generic */
-.pygments-style-fruity .k {
-  color: #fb660a;
-  font-weight: bold;
-} /* Keyword */
-.pygments-style-fruity .l { color: #fff; } /* Literal */
-.pygments-style-fruity .n { color: #fff; } /* Name */
-.pygments-style-fruity .o { color: #fff; } /* Operator */
-.pygments-style-fruity .x { color: #fff; } /* Other */
-.pygments-style-fruity .p { color: #fff; } /* Punctuation */
-.pygments-style-fruity .ch {
-  color: #080;
-  font-style: italic;
-  background-color: #0f140f;
-} /* Comment.Hashbang */
-.pygments-style-fruity .cm {
-  color: #080;
-  font-style: italic;
-  background-color: #0f140f;
-} /* Comment.Multiline */
-.pygments-style-fruity .cp {
-  color: #ff0007;
-  font-weight: bold;
-  font-style: italic;
-  background-color: #0f140f;
-} /* Comment.Preproc */
-.pygments-style-fruity .cpf {
-  color: #080;
-  font-style: italic;
-  background-color: #0f140f;
-} /* Comment.PreprocFile */
-.pygments-style-fruity .c1 {
-  color: #080;
-  font-style: italic;
-  background-color: #0f140f;
-} /* Comment.Single */
-.pygments-style-fruity .cs {
-  color: #080;
-  font-style: italic;
-  background-color: #0f140f;
-} /* Comment.Special */
-.pygments-style-fruity .gd { color: #fff; } /* Generic.Deleted */
-.pygments-style-fruity .ge { color: #fff; } /* Generic.Emph */
-.pygments-style-fruity .gr { color: #fff; } /* Generic.Error */
-.pygments-style-fruity .gh {
-  color: #fff;
-  font-weight: bold;
-} /* Generic.Heading */
-.pygments-style-fruity .gi { color: #fff; } /* Generic.Inserted */
-.pygments-style-fruity .go {
-  color: #444;
-  background-color: #222;
-} /* Generic.Output */
-.pygments-style-fruity .gp { color: #fff; } /* Generic.Prompt */
-.pygments-style-fruity .gs { color: #fff; } /* Generic.Strong */
-.pygments-style-fruity .gu {
-  color: #fff;
-  font-weight: bold;
-} /* Generic.Subheading */
-.pygments-style-fruity .gt { color: #fff; } /* Generic.Traceback */
-.pygments-style-fruity .kc {
-  color: #fb660a;
-  font-weight: bold;
-} /* Keyword.Constant */
-.pygments-style-fruity .kd {
-  color: #fb660a;
-  font-weight: bold;
-} /* Keyword.Declaration */
-.pygments-style-fruity .kn {
-  color: #fb660a;
-  font-weight: bold;
-} /* Keyword.Namespace */
-.pygments-style-fruity .kp { color: #fb660a; } /* Keyword.Pseudo */
-.pygments-style-fruity .kr {
-  color: #fb660a;
-  font-weight: bold;
-} /* Keyword.Reserved */
-.pygments-style-fruity .kt {
-  color: #cdcaa9;
-  font-weight: bold;
-} /* Keyword.Type */
-.pygments-style-fruity .ld { color: #fff; } /* Literal.Date */
-.pygments-style-fruity .m {
-  color: #0086f7;
-  font-weight: bold;
-} /* Literal.Number */
-.pygments-style-fruity .s { color: #0086d2; } /* Literal.String */
-.pygments-style-fruity .na {
-  color: #ff0086;
-  font-weight: bold;
-} /* Name.Attribute */
-.pygments-style-fruity .nb { color: #fff; } /* Name.Builtin */
-.pygments-style-fruity .nc { color: #fff; } /* Name.Class */
-.pygments-style-fruity .no { color: #0086d2; } /* Name.Constant */
-.pygments-style-fruity .nd { color: #fff; } /* Name.Decorator */
-.pygments-style-fruity .ni { color: #fff; } /* Name.Entity */
-.pygments-style-fruity .ne { color: #fff; } /* Name.Exception */
-.pygments-style-fruity .nf {
-  color: #ff0086;
-  font-weight: bold;
-} /* Name.Function */
-.pygments-style-fruity .nl { color: #fff; } /* Name.Label */
-.pygments-style-fruity .nn { color: #fff; } /* Name.Namespace */
-.pygments-style-fruity .nx { color: #fff; } /* Name.Other */
-.pygments-style-fruity .py { color: #fff; } /* Name.Property */
-.pygments-style-fruity .nt {
-  color: #fb660a;
-  font-weight: bold;
-} /* Name.Tag */
-.pygments-style-fruity .nv { color: #fb660a; } /* Name.Variable */
-.pygments-style-fruity .ow { color: #fff; } /* Operator.Word */
-.pygments-style-fruity .w { color: #888; } /* Text.Whitespace */
-.pygments-style-fruity .mb {
-  color: #0086f7;
-  font-weight: bold;
-} /* Literal.Number.Bin */
-.pygments-style-fruity .mf {
-  color: #0086f7;
-  font-weight: bold;
-} /* Literal.Number.Float */
-.pygments-style-fruity .mh {
-  color: #0086f7;
-  font-weight: bold;
-} /* Literal.Number.Hex */
-.pygments-style-fruity .mi {
-  color: #0086f7;
-  font-weight: bold;
-} /* Literal.Number.Integer */
-.pygments-style-fruity .mo {
-  color: #0086f7;
-  font-weight: bold;
-} /* Literal.Number.Oct */
-.pygments-style-fruity .sa { color: #0086d2; } /* Literal.String.Affix */
-.pygments-style-fruity .sb { color: #0086d2; } /* Literal.String.Backtick */
-.pygments-style-fruity .sc { color: #0086d2; } /* Literal.String.Char */
-.pygments-style-fruity .dl { color: #0086d2; } /* Literal.String.Delimiter */
-.pygments-style-fruity .sd { color: #0086d2; } /* Literal.String.Doc */
-.pygments-style-fruity .s2 { color: #0086d2; } /* Literal.String.Double */
-.pygments-style-fruity .se { color: #0086d2; } /* Literal.String.Escape */
-.pygments-style-fruity .sh { color: #0086d2; } /* Literal.String.Heredoc */
-.pygments-style-fruity .si { color: #0086d2; } /* Literal.String.Interpol */
-.pygments-style-fruity .sx { color: #0086d2; } /* Literal.String.Other */
-.pygments-style-fruity .sr { color: #0086d2; } /* Literal.String.Regex */
-.pygments-style-fruity .s1 { color: #0086d2; } /* Literal.String.Single */
-.pygments-style-fruity .ss { color: #0086d2; } /* Literal.String.Symbol */
-.pygments-style-fruity .bp { color: #fff; } /* Name.Builtin.Pseudo */
-.pygments-style-fruity .fm {
-  color: #ff0086;
-  font-weight: bold;
-} /* Name.Function.Magic */
-.pygments-style-fruity .vc { color: #fb660a; } /* Name.Variable.Class */
-.pygments-style-fruity .vg { color: #fb660a; } /* Name.Variable.Global */
-.pygments-style-fruity .vi { color: #fb660a; } /* Name.Variable.Instance */
-.pygments-style-fruity .vm { color: #fb660a; } /* Name.Variable.Magic */
-.pygments-style-fruity .il {
-  color: #0086f7;
-  font-weight: bold;
-} /* Literal.Number.Integer.Long */
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+.pygments-style-fruity .hll { background-color: #333 }
+
+.pygments-style-fruity { background: #111; 
+color: #fff }
+
+.pygments-style-fruity .c { color: #080; 
+font-style: italic; 
+background-color: #0f140f } /* Comment */
+.pygments-style-fruity .err { color: #fff } /* Error */
+.pygments-style-fruity .esc { color: #fff } /* Escape */
+.pygments-style-fruity .g { color: #fff } /* Generic */
+.pygments-style-fruity .k { color: #fb660a; 
+font-weight: bold } /* Keyword */
+.pygments-style-fruity .l { color: #fff } /* Literal */
+.pygments-style-fruity .n { color: #fff } /* Name */
+.pygments-style-fruity .o { color: #fff } /* Operator */
+.pygments-style-fruity .x { color: #fff } /* Other */
+.pygments-style-fruity .p { color: #fff } /* Punctuation */
+.pygments-style-fruity .ch { color: #080; 
+font-style: italic; 
+background-color: #0f140f } /* Comment.Hashbang */
+.pygments-style-fruity .cm { color: #080; 
+font-style: italic; 
+background-color: #0f140f } /* Comment.Multiline */
+.pygments-style-fruity .cp { color: #ff0007; 
+font-weight: bold; 
+font-style: italic; 
+background-color: #0f140f } /* Comment.Preproc */
+.pygments-style-fruity .cpf { color: #080; 
+font-style: italic; 
+background-color: #0f140f } /* Comment.PreprocFile */
+.pygments-style-fruity .c1 { color: #080; 
+font-style: italic; 
+background-color: #0f140f } /* Comment.Single */
+.pygments-style-fruity .cs { color: #080; 
+font-style: italic; 
+background-color: #0f140f } /* Comment.Special */
+.pygments-style-fruity .gd { color: #fff } /* Generic.Deleted */
+.pygments-style-fruity .ge { color: #fff } /* Generic.Emph */
+.pygments-style-fruity .ges { color: #fff } /* Generic.EmphStrong */
+.pygments-style-fruity .gr { color: #fff } /* Generic.Error */
+.pygments-style-fruity .gh { color: #fff; 
+font-weight: bold } /* Generic.Heading */
+.pygments-style-fruity .gi { color: #fff } /* Generic.Inserted */
+.pygments-style-fruity .go { color: #444; 
+background-color: #222 } /* Generic.Output */
+.pygments-style-fruity .gp { color: #fff } /* Generic.Prompt */
+.pygments-style-fruity .gs { color: #fff } /* Generic.Strong */
+.pygments-style-fruity .gu { color: #fff; 
+font-weight: bold } /* Generic.Subheading */
+.pygments-style-fruity .gt { color: #fff } /* Generic.Traceback */
+.pygments-style-fruity .kc { color: #fb660a; 
+font-weight: bold } /* Keyword.Constant */
+.pygments-style-fruity .kd { color: #fb660a; 
+font-weight: bold } /* Keyword.Declaration */
+.pygments-style-fruity .kn { color: #fb660a; 
+font-weight: bold } /* Keyword.Namespace */
+.pygments-style-fruity .kp { color: #fb660a } /* Keyword.Pseudo */
+.pygments-style-fruity .kr { color: #fb660a; 
+font-weight: bold } /* Keyword.Reserved */
+.pygments-style-fruity .kt { color: #cdcaa9; 
+font-weight: bold } /* Keyword.Type */
+.pygments-style-fruity .ld { color: #fff } /* Literal.Date */
+.pygments-style-fruity .m { color: #0086f7; 
+font-weight: bold } /* Literal.Number */
+.pygments-style-fruity .s { color: #0086d2 } /* Literal.String */
+.pygments-style-fruity .na { color: #ff0086; 
+font-weight: bold } /* Name.Attribute */
+.pygments-style-fruity .nb { color: #fff } /* Name.Builtin */
+.pygments-style-fruity .nc { color: #fff } /* Name.Class */
+.pygments-style-fruity .no { color: #0086d2 } /* Name.Constant */
+.pygments-style-fruity .nd { color: #fff } /* Name.Decorator */
+.pygments-style-fruity .ni { color: #fff } /* Name.Entity */
+.pygments-style-fruity .ne { color: #fff } /* Name.Exception */
+.pygments-style-fruity .nf { color: #ff0086; 
+font-weight: bold } /* Name.Function */
+.pygments-style-fruity .nl { color: #fff } /* Name.Label */
+.pygments-style-fruity .nn { color: #fff } /* Name.Namespace */
+.pygments-style-fruity .nx { color: #fff } /* Name.Other */
+.pygments-style-fruity .py { color: #fff } /* Name.Property */
+.pygments-style-fruity .nt { color: #fb660a; 
+font-weight: bold } /* Name.Tag */
+.pygments-style-fruity .nv { color: #fb660a } /* Name.Variable */
+.pygments-style-fruity .ow { color: #fff } /* Operator.Word */
+.pygments-style-fruity .pm { color: #fff } /* Punctuation.Marker */
+.pygments-style-fruity .w { color: #888 } /* Text.Whitespace */
+.pygments-style-fruity .mb { color: #0086f7; 
+font-weight: bold } /* Literal.Number.Bin */
+.pygments-style-fruity .mf { color: #0086f7; 
+font-weight: bold } /* Literal.Number.Float */
+.pygments-style-fruity .mh { color: #0086f7; 
+font-weight: bold } /* Literal.Number.Hex */
+.pygments-style-fruity .mi { color: #0086f7; 
+font-weight: bold } /* Literal.Number.Integer */
+.pygments-style-fruity .mo { color: #0086f7; 
+font-weight: bold } /* Literal.Number.Oct */
+.pygments-style-fruity .sa { color: #0086d2 } /* Literal.String.Affix */
+.pygments-style-fruity .sb { color: #0086d2 } /* Literal.String.Backtick */
+.pygments-style-fruity .sc { color: #0086d2 } /* Literal.String.Char */
+.pygments-style-fruity .dl { color: #0086d2 } /* Literal.String.Delimiter */
+.pygments-style-fruity .sd { color: #0086d2 } /* Literal.String.Doc */
+.pygments-style-fruity .s2 { color: #0086d2 } /* Literal.String.Double */
+.pygments-style-fruity .se { color: #0086d2 } /* Literal.String.Escape */
+.pygments-style-fruity .sh { color: #0086d2 } /* Literal.String.Heredoc */
+.pygments-style-fruity .si { color: #0086d2 } /* Literal.String.Interpol */
+.pygments-style-fruity .sx { color: #0086d2 } /* Literal.String.Other */
+.pygments-style-fruity .sr { color: #0086d2 } /* Literal.String.Regex */
+.pygments-style-fruity .s1 { color: #0086d2 } /* Literal.String.Single */
+.pygments-style-fruity .ss { color: #0086d2 } /* Literal.String.Symbol */
+.pygments-style-fruity .bp { color: #fff } /* Name.Builtin.Pseudo */
+.pygments-style-fruity .fm { color: #ff0086; 
+font-weight: bold } /* Name.Function.Magic */
+.pygments-style-fruity .vc { color: #fb660a } /* Name.Variable.Class */
+.pygments-style-fruity .vg { color: #fb660a } /* Name.Variable.Global */
+.pygments-style-fruity .vi { color: #fb660a } /* Name.Variable.Instance */
+.pygments-style-fruity .vm { color: #fb660a } /* Name.Variable.Magic */
+.pygments-style-fruity .il { color: #0086f7; 
+font-weight: bold } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/igor.css` & `plumage-4.0.0/plumage/static/css/pygments/igor.css`

 * *Files 20% similar despite different names*

```diff
@@ -1,90 +1,70 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-.pygments-style-igor .hll { background-color: #ffc; }
-
-.pygments-style-igor {
-  background: #fff;
-}
-
-.pygments-style-igor .c {
-  color: #f00;
-  font-style: italic;
-} /* Comment */
-.pygments-style-igor .k { color: #00f; } /* Keyword */
-.pygments-style-igor .ch {
-  color: #f00;
-  font-style: italic;
-} /* Comment.Hashbang */
-.pygments-style-igor .cm {
-  color: #f00;
-  font-style: italic;
-} /* Comment.Multiline */
-.pygments-style-igor .cp {
-  color: #f00;
-  font-style: italic;
-} /* Comment.Preproc */
-.pygments-style-igor .cpf {
-  color: #f00;
-  font-style: italic;
-} /* Comment.PreprocFile */
-.pygments-style-igor .c1 {
-  color: #f00;
-  font-style: italic;
-} /* Comment.Single */
-.pygments-style-igor .cs {
-  color: #f00;
-  font-style: italic;
-} /* Comment.Special */
-.pygments-style-igor .kc { color: #00f; } /* Keyword.Constant */
-.pygments-style-igor .kd { color: #00f; } /* Keyword.Declaration */
-.pygments-style-igor .kn { color: #00f; } /* Keyword.Namespace */
-.pygments-style-igor .kp { color: #00f; } /* Keyword.Pseudo */
-.pygments-style-igor .kr { color: #00f; } /* Keyword.Reserved */
-.pygments-style-igor .kt { color: #00f; } /* Keyword.Type */
-.pygments-style-igor .s { color: #009c00; } /* Literal.String */
-.pygments-style-igor .nc { color: #007575; } /* Name.Class */
-.pygments-style-igor .nd { color: #cc00a3; } /* Name.Decorator */
-.pygments-style-igor .nf { color: #c34e00; } /* Name.Function */
-.pygments-style-igor .sa { color: #009c00; } /* Literal.String.Affix */
-.pygments-style-igor .sb { color: #009c00; } /* Literal.String.Backtick */
-.pygments-style-igor .sc { color: #009c00; } /* Literal.String.Char */
-.pygments-style-igor .dl { color: #009c00; } /* Literal.String.Delimiter */
-.pygments-style-igor .sd { color: #009c00; } /* Literal.String.Doc */
-.pygments-style-igor .s2 { color: #009c00; } /* Literal.String.Double */
-.pygments-style-igor .se { color: #009c00; } /* Literal.String.Escape */
-.pygments-style-igor .sh { color: #009c00; } /* Literal.String.Heredoc */
-.pygments-style-igor .si { color: #009c00; } /* Literal.String.Interpol */
-.pygments-style-igor .sx { color: #009c00; } /* Literal.String.Other */
-.pygments-style-igor .sr { color: #009c00; } /* Literal.String.Regex */
-.pygments-style-igor .s1 { color: #009c00; } /* Literal.String.Single */
-.pygments-style-igor .ss { color: #009c00; } /* Literal.String.Symbol */
-.pygments-style-igor .fm { color: #c34e00; } /* Name.Function.Magic */
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+.pygments-style-igor .hll { background-color: #ffc }
+
+.pygments-style-igor { background: #fff; 
+}
+
+.pygments-style-igor .c { color: #F00; 
+font-style: italic } /* Comment */
+.pygments-style-igor .k { color: #00F } /* Keyword */
+.pygments-style-igor .ch { color: #F00; 
+font-style: italic } /* Comment.Hashbang */
+.pygments-style-igor .cm { color: #F00; 
+font-style: italic } /* Comment.Multiline */
+.pygments-style-igor .cp { color: #F00; 
+font-style: italic } /* Comment.Preproc */
+.pygments-style-igor .cpf { color: #F00; 
+font-style: italic } /* Comment.PreprocFile */
+.pygments-style-igor .c1 { color: #F00; 
+font-style: italic } /* Comment.Single */
+.pygments-style-igor .cs { color: #F00; 
+font-style: italic } /* Comment.Special */
+.pygments-style-igor .kc { color: #00F } /* Keyword.Constant */
+.pygments-style-igor .kd { color: #00F } /* Keyword.Declaration */
+.pygments-style-igor .kn { color: #00F } /* Keyword.Namespace */
+.pygments-style-igor .kp { color: #00F } /* Keyword.Pseudo */
+.pygments-style-igor .kr { color: #00F } /* Keyword.Reserved */
+.pygments-style-igor .kt { color: #00F } /* Keyword.Type */
+.pygments-style-igor .s { color: #009C00 } /* Literal.String */
+.pygments-style-igor .nc { color: #007575 } /* Name.Class */
+.pygments-style-igor .nd { color: #CC00A3 } /* Name.Decorator */
+.pygments-style-igor .nf { color: #C34E00 } /* Name.Function */
+.pygments-style-igor .sa { color: #009C00 } /* Literal.String.Affix */
+.pygments-style-igor .sb { color: #009C00 } /* Literal.String.Backtick */
+.pygments-style-igor .sc { color: #009C00 } /* Literal.String.Char */
+.pygments-style-igor .dl { color: #009C00 } /* Literal.String.Delimiter */
+.pygments-style-igor .sd { color: #009C00 } /* Literal.String.Doc */
+.pygments-style-igor .s2 { color: #009C00 } /* Literal.String.Double */
+.pygments-style-igor .se { color: #009C00 } /* Literal.String.Escape */
+.pygments-style-igor .sh { color: #009C00 } /* Literal.String.Heredoc */
+.pygments-style-igor .si { color: #009C00 } /* Literal.String.Interpol */
+.pygments-style-igor .sx { color: #009C00 } /* Literal.String.Other */
+.pygments-style-igor .sr { color: #009C00 } /* Literal.String.Regex */
+.pygments-style-igor .s1 { color: #009C00 } /* Literal.String.Single */
+.pygments-style-igor .ss { color: #009C00 } /* Literal.String.Symbol */
+.pygments-style-igor .fm { color: #C34E00 } /* Name.Function.Magic */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/inkpot.css` & `plumage-4.0.0/plumage/static/css/pygments/inkpot.css`

 * *Files 19% similar despite different names*

```diff
@@ -1,166 +1,124 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
-.pygments-style-inkpot .hll { background-color: #ffc; }
+.pygments-style-inkpot .hll { background-color: #ffc }
 
-.pygments-style-inkpot {
-  background: #1e1e27;
-  color: #cfbfad;
-}
-.pygments-style-inkpot .c { color: #cd8b00; } /* Comment */
-.pygments-style-inkpot .err {
-  color: #fff;
-  background-color: #6e2e2e;
-} /* Error */
-.pygments-style-inkpot .k { color: #808bed; } /* Keyword */
-.pygments-style-inkpot .n { color: #cfbfad; } /* Name */
-.pygments-style-inkpot .o { color: #666; } /* Operator */
-.pygments-style-inkpot .x { color: #cfbfad; } /* Other */
-.pygments-style-inkpot .p { color: #cfbfad; } /* Punctuation */
-.pygments-style-inkpot .ch { color: #cd8b00; } /* Comment.Hashbang */
-.pygments-style-inkpot .cm { color: #cd8b00; } /* Comment.Multiline */
-.pygments-style-inkpot .cp { color: #409090; } /* Comment.Preproc */
-.pygments-style-inkpot .cpf {
-  color: #ffcd8b;
-  background-color: #404040;
-} /* Comment.PreprocFile */
-.pygments-style-inkpot .c1 { color: #cd8b00; } /* Comment.Single */
-.pygments-style-inkpot .cs { color: #808bed; } /* Comment.Special */
-.pygments-style-inkpot .gd { color: #a00000; } /* Generic.Deleted */
-.pygments-style-inkpot .ge { font-style: italic; } /* Generic.Emph */
-.pygments-style-inkpot .gr { color: #f00; } /* Generic.Error */
-.pygments-style-inkpot .gh {
-  color: #000080;
-  font-weight: bold;
-} /* Generic.Heading */
-.pygments-style-inkpot .gi { color: #00a000; } /* Generic.Inserted */
-.pygments-style-inkpot .go { color: #888; } /* Generic.Output */
-.pygments-style-inkpot .gp {
-  color: #000080;
-  font-weight: bold;
-} /* Generic.Prompt */
-.pygments-style-inkpot .gs { font-weight: bold; } /* Generic.Strong */
-.pygments-style-inkpot .gu {
-  color: #800080;
-  font-weight: bold;
-} /* Generic.Subheading */
-.pygments-style-inkpot .gt { color: #04d; } /* Generic.Traceback */
-.pygments-style-inkpot .kc { color: #808bed; } /* Keyword.Constant */
-.pygments-style-inkpot .kd { color: #808bed; } /* Keyword.Declaration */
-.pygments-style-inkpot .kn { color: #808bed; } /* Keyword.Namespace */
-.pygments-style-inkpot .kp { color: #808bed; } /* Keyword.Pseudo */
-.pygments-style-inkpot .kr { color: #808bed; } /* Keyword.Reserved */
-.pygments-style-inkpot .kt { color: #ff8bff; } /* Keyword.Type */
-.pygments-style-inkpot .m { color: #f0ad6d; } /* Literal.Number */
-.pygments-style-inkpot .s {
-  color: #ffcd8b;
-  background-color: #404040;
-} /* Literal.String */
-.pygments-style-inkpot .na { color: #cfbfad; } /* Name.Attribute */
-.pygments-style-inkpot .nb { color: #808bed; } /* Name.Builtin */
-.pygments-style-inkpot .nc { color: #ff8bff; } /* Name.Class */
-.pygments-style-inkpot .no { color: #409090; } /* Name.Constant */
-.pygments-style-inkpot .nd { color: #409090; } /* Name.Decorator */
-.pygments-style-inkpot .ni { color: #cfbfad; } /* Name.Entity */
-.pygments-style-inkpot .ne { color: #f00; } /* Name.Exception */
-.pygments-style-inkpot .nf { color: #c080d0; } /* Name.Function */
-.pygments-style-inkpot .nl { color: #808bed; } /* Name.Label */
-.pygments-style-inkpot .nn { color: #f00; } /* Name.Namespace */
-.pygments-style-inkpot .nx { color: #cfbfad; } /* Name.Other */
-.pygments-style-inkpot .py { color: #cfbfad; } /* Name.Property */
-.pygments-style-inkpot .nt { color: #cfbfad; } /* Name.Tag */
-.pygments-style-inkpot .nv { color: #cfbfad; } /* Name.Variable */
-.pygments-style-inkpot .ow { color: #666; } /* Operator.Word */
-.pygments-style-inkpot .w { color: #434357; } /* Text.Whitespace */
-.pygments-style-inkpot .mb { color: #f0ad6d; } /* Literal.Number.Bin */
-.pygments-style-inkpot .mf { color: #f0ad6d; } /* Literal.Number.Float */
-.pygments-style-inkpot .mh { color: #f0ad6d; } /* Literal.Number.Hex */
-.pygments-style-inkpot .mi { color: #f0ad6d; } /* Literal.Number.Integer */
-.pygments-style-inkpot .mo { color: #f0ad6d; } /* Literal.Number.Oct */
-.pygments-style-inkpot .sa {
-  color: #ffcd8b;
-  background-color: #404040;
-} /* Literal.String.Affix */
-.pygments-style-inkpot .sb {
-  color: #ffcd8b;
-  background-color: #404040;
-} /* Literal.String.Backtick */
-.pygments-style-inkpot .sc {
-  color: #ffcd8b;
-  background-color: #404040;
-} /* Literal.String.Char */
-.pygments-style-inkpot .dl {
-  color: #ffcd8b;
-  background-color: #404040;
-} /* Literal.String.Delimiter */
-.pygments-style-inkpot .sd {
-  color: #808bed;
-  background-color: #404040;
-} /* Literal.String.Doc */
-.pygments-style-inkpot .s2 {
-  color: #ffcd8b;
-  background-color: #404040;
-} /* Literal.String.Double */
-.pygments-style-inkpot .se {
-  color: #ffcd8b;
-  background-color: #404040;
-} /* Literal.String.Escape */
-.pygments-style-inkpot .sh {
-  color: #ffcd8b;
-  background-color: #404040;
-} /* Literal.String.Heredoc */
-.pygments-style-inkpot .si {
-  color: #ffcd8b;
-  background-color: #404040;
-} /* Literal.String.Interpol */
-.pygments-style-inkpot .sx {
-  color: #ffcd8b;
-  background-color: #404040;
-} /* Literal.String.Other */
-.pygments-style-inkpot .sr {
-  color: #ffcd8b;
-  background-color: #404040;
-} /* Literal.String.Regex */
-.pygments-style-inkpot .s1 {
-  color: #ffcd8b;
-  background-color: #404040;
-} /* Literal.String.Single */
-.pygments-style-inkpot .ss {
-  color: #ffcd8b;
-  background-color: #404040;
-} /* Literal.String.Symbol */
-.pygments-style-inkpot .bp { color: #ff0; } /* Name.Builtin.Pseudo */
-.pygments-style-inkpot .fm { color: #c080d0; } /* Name.Function.Magic */
-.pygments-style-inkpot .vc { color: #cfbfad; } /* Name.Variable.Class */
-.pygments-style-inkpot .vg { color: #cfbfad; } /* Name.Variable.Global */
-.pygments-style-inkpot .vi { color: #cfbfad; } /* Name.Variable.Instance */
-.pygments-style-inkpot .vm { color: #cfbfad; } /* Name.Variable.Magic */
-.pygments-style-inkpot .il { color: #f0ad6d; } /* Literal.Number.Integer.Long */
+.pygments-style-inkpot { background: #1e1e27; 
+color: #cfbfad }
+.pygments-style-inkpot .c { color: #cd8b00 } /* Comment */
+.pygments-style-inkpot .err { color: #fff; 
+background-color: #6e2e2e } /* Error */
+.pygments-style-inkpot .k { color: #808bed } /* Keyword */
+.pygments-style-inkpot .n { color: #cfbfad } /* Name */
+.pygments-style-inkpot .o { color: #666 } /* Operator */
+.pygments-style-inkpot .x { color: #cfbfad } /* Other */
+.pygments-style-inkpot .p { color: #cfbfad } /* Punctuation */
+.pygments-style-inkpot .ch { color: #cd8b00 } /* Comment.Hashbang */
+.pygments-style-inkpot .cm { color: #cd8b00 } /* Comment.Multiline */
+.pygments-style-inkpot .cp { color: #409090 } /* Comment.Preproc */
+.pygments-style-inkpot .cpf { color: #ffcd8b; 
+background-color: #404040 } /* Comment.PreprocFile */
+.pygments-style-inkpot .c1 { color: #cd8b00 } /* Comment.Single */
+.pygments-style-inkpot .cs { color: #808bed } /* Comment.Special */
+.pygments-style-inkpot .gd { color: #A00000 } /* Generic.Deleted */
+.pygments-style-inkpot .ge { font-style: italic } /* Generic.Emph */
+.pygments-style-inkpot .ges { font-weight: bold; 
+font-style: italic } /* Generic.EmphStrong */
+.pygments-style-inkpot .gr { color: #F00 } /* Generic.Error */
+.pygments-style-inkpot .gh { color: #000080; 
+font-weight: bold } /* Generic.Heading */
+.pygments-style-inkpot .gi { color: #00A000 } /* Generic.Inserted */
+.pygments-style-inkpot .go { color: #888 } /* Generic.Output */
+.pygments-style-inkpot .gp { color: #000080; 
+font-weight: bold } /* Generic.Prompt */
+.pygments-style-inkpot .gs { font-weight: bold } /* Generic.Strong */
+.pygments-style-inkpot .gu { color: #800080; 
+font-weight: bold } /* Generic.Subheading */
+.pygments-style-inkpot .gt { color: #04D } /* Generic.Traceback */
+.pygments-style-inkpot .kc { color: #808bed } /* Keyword.Constant */
+.pygments-style-inkpot .kd { color: #808bed } /* Keyword.Declaration */
+.pygments-style-inkpot .kn { color: #808bed } /* Keyword.Namespace */
+.pygments-style-inkpot .kp { color: #808bed } /* Keyword.Pseudo */
+.pygments-style-inkpot .kr { color: #808bed } /* Keyword.Reserved */
+.pygments-style-inkpot .kt { color: #ff8bff } /* Keyword.Type */
+.pygments-style-inkpot .m { color: #f0ad6d } /* Literal.Number */
+.pygments-style-inkpot .s { color: #ffcd8b; 
+background-color: #404040 } /* Literal.String */
+.pygments-style-inkpot .na { color: #cfbfad } /* Name.Attribute */
+.pygments-style-inkpot .nb { color: #808bed } /* Name.Builtin */
+.pygments-style-inkpot .nc { color: #ff8bff } /* Name.Class */
+.pygments-style-inkpot .no { color: #409090 } /* Name.Constant */
+.pygments-style-inkpot .nd { color: #409090 } /* Name.Decorator */
+.pygments-style-inkpot .ni { color: #cfbfad } /* Name.Entity */
+.pygments-style-inkpot .ne { color: #f00 } /* Name.Exception */
+.pygments-style-inkpot .nf { color: #c080d0 } /* Name.Function */
+.pygments-style-inkpot .nl { color: #808bed } /* Name.Label */
+.pygments-style-inkpot .nn { color: #f00 } /* Name.Namespace */
+.pygments-style-inkpot .nx { color: #cfbfad } /* Name.Other */
+.pygments-style-inkpot .py { color: #cfbfad } /* Name.Property */
+.pygments-style-inkpot .nt { color: #cfbfad } /* Name.Tag */
+.pygments-style-inkpot .nv { color: #cfbfad } /* Name.Variable */
+.pygments-style-inkpot .ow { color: #666 } /* Operator.Word */
+.pygments-style-inkpot .pm { color: #cfbfad } /* Punctuation.Marker */
+.pygments-style-inkpot .w { color: #434357 } /* Text.Whitespace */
+.pygments-style-inkpot .mb { color: #f0ad6d } /* Literal.Number.Bin */
+.pygments-style-inkpot .mf { color: #f0ad6d } /* Literal.Number.Float */
+.pygments-style-inkpot .mh { color: #f0ad6d } /* Literal.Number.Hex */
+.pygments-style-inkpot .mi { color: #f0ad6d } /* Literal.Number.Integer */
+.pygments-style-inkpot .mo { color: #f0ad6d } /* Literal.Number.Oct */
+.pygments-style-inkpot .sa { color: #ffcd8b; 
+background-color: #404040 } /* Literal.String.Affix */
+.pygments-style-inkpot .sb { color: #ffcd8b; 
+background-color: #404040 } /* Literal.String.Backtick */
+.pygments-style-inkpot .sc { color: #ffcd8b; 
+background-color: #404040 } /* Literal.String.Char */
+.pygments-style-inkpot .dl { color: #ffcd8b; 
+background-color: #404040 } /* Literal.String.Delimiter */
+.pygments-style-inkpot .sd { color: #808bed; 
+background-color: #404040 } /* Literal.String.Doc */
+.pygments-style-inkpot .s2 { color: #ffcd8b; 
+background-color: #404040 } /* Literal.String.Double */
+.pygments-style-inkpot .se { color: #ffcd8b; 
+background-color: #404040 } /* Literal.String.Escape */
+.pygments-style-inkpot .sh { color: #ffcd8b; 
+background-color: #404040 } /* Literal.String.Heredoc */
+.pygments-style-inkpot .si { color: #ffcd8b; 
+background-color: #404040 } /* Literal.String.Interpol */
+.pygments-style-inkpot .sx { color: #ffcd8b; 
+background-color: #404040 } /* Literal.String.Other */
+.pygments-style-inkpot .sr { color: #ffcd8b; 
+background-color: #404040 } /* Literal.String.Regex */
+.pygments-style-inkpot .s1 { color: #ffcd8b; 
+background-color: #404040 } /* Literal.String.Single */
+.pygments-style-inkpot .ss { color: #ffcd8b; 
+background-color: #404040 } /* Literal.String.Symbol */
+.pygments-style-inkpot .bp { color: #ff0 } /* Name.Builtin.Pseudo */
+.pygments-style-inkpot .fm { color: #c080d0 } /* Name.Function.Magic */
+.pygments-style-inkpot .vc { color: #cfbfad } /* Name.Variable.Class */
+.pygments-style-inkpot .vg { color: #cfbfad } /* Name.Variable.Global */
+.pygments-style-inkpot .vi { color: #cfbfad } /* Name.Variable.Instance */
+.pygments-style-inkpot .vm { color: #cfbfad } /* Name.Variable.Magic */
+.pygments-style-inkpot .il { color: #f0ad6d } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/lovelace.css` & `plumage-4.0.0/plumage/static/css/pygments/lovelace.css`

 * *Files 12% similar despite different names*

```diff
@@ -1,141 +1,114 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-.pygments-style-lovelace .hll { background-color: #ffc; }
-
-.pygments-style-lovelace {
-  background: #fff;
-}
-
-.pygments-style-lovelace .c {
-  color: #888;
-  font-style: italic;
-} /* Comment */
-.pygments-style-lovelace .err { background-color: #a848a8; } /* Error */
-.pygments-style-lovelace .k { color: #2838b0; } /* Keyword */
-.pygments-style-lovelace .o { color: #666; } /* Operator */
-.pygments-style-lovelace .p { color: #888; } /* Punctuation */
-.pygments-style-lovelace .ch {
-  color: #287088;
-  font-style: italic;
-} /* Comment.Hashbang */
-.pygments-style-lovelace .cm {
-  color: #888;
-  font-style: italic;
-} /* Comment.Multiline */
-.pygments-style-lovelace .cp { color: #289870; } /* Comment.Preproc */
-.pygments-style-lovelace .cpf {
-  color: #888;
-  font-style: italic;
-} /* Comment.PreprocFile */
-.pygments-style-lovelace .c1 {
-  color: #888;
-  font-style: italic;
-} /* Comment.Single */
-.pygments-style-lovelace .cs {
-  color: #888;
-  font-style: italic;
-} /* Comment.Special */
-.pygments-style-lovelace .gd { color: #c02828; } /* Generic.Deleted */
-.pygments-style-lovelace .ge { font-style: italic; } /* Generic.Emph */
-.pygments-style-lovelace .gr { color: #c02828; } /* Generic.Error */
-.pygments-style-lovelace .gh { color: #666; } /* Generic.Heading */
-.pygments-style-lovelace .gi { color: #388038; } /* Generic.Inserted */
-.pygments-style-lovelace .go { color: #666; } /* Generic.Output */
-.pygments-style-lovelace .gp { color: #444; } /* Generic.Prompt */
-.pygments-style-lovelace .gs { font-weight: bold; } /* Generic.Strong */
-.pygments-style-lovelace .gu { color: #444; } /* Generic.Subheading */
-.pygments-style-lovelace .gt { color: #2838b0; } /* Generic.Traceback */
-.pygments-style-lovelace .kc {
-  color: #444;
-  font-style: italic;
-} /* Keyword.Constant */
-.pygments-style-lovelace .kd {
-  color: #2838b0;
-  font-style: italic;
-} /* Keyword.Declaration */
-.pygments-style-lovelace .kn { color: #2838b0; } /* Keyword.Namespace */
-.pygments-style-lovelace .kp { color: #2838b0; } /* Keyword.Pseudo */
-.pygments-style-lovelace .kr { color: #2838b0; } /* Keyword.Reserved */
-.pygments-style-lovelace .kt {
-  color: #2838b0;
-  font-style: italic;
-} /* Keyword.Type */
-.pygments-style-lovelace .m { color: #444; } /* Literal.Number */
-.pygments-style-lovelace .s { color: #b83838; } /* Literal.String */
-.pygments-style-lovelace .na { color: #388038; } /* Name.Attribute */
-.pygments-style-lovelace .nb { color: #388038; } /* Name.Builtin */
-.pygments-style-lovelace .nc { color: #287088; } /* Name.Class */
-.pygments-style-lovelace .no { color: #b85820; } /* Name.Constant */
-.pygments-style-lovelace .nd { color: #287088; } /* Name.Decorator */
-.pygments-style-lovelace .ni { color: #709030; } /* Name.Entity */
-.pygments-style-lovelace .ne { color: #908828; } /* Name.Exception */
-.pygments-style-lovelace .nf { color: #785840; } /* Name.Function */
-.pygments-style-lovelace .nl { color: #289870; } /* Name.Label */
-.pygments-style-lovelace .nn { color: #289870; } /* Name.Namespace */
-.pygments-style-lovelace .nt { color: #2838b0; } /* Name.Tag */
-.pygments-style-lovelace .nv { color: #b04040; } /* Name.Variable */
-.pygments-style-lovelace .ow { color: #a848a8; } /* Operator.Word */
-.pygments-style-lovelace .w { color: #a89028; } /* Text.Whitespace */
-.pygments-style-lovelace .mb { color: #444; } /* Literal.Number.Bin */
-.pygments-style-lovelace .mf { color: #444; } /* Literal.Number.Float */
-.pygments-style-lovelace .mh { color: #444; } /* Literal.Number.Hex */
-.pygments-style-lovelace .mi { color: #444; } /* Literal.Number.Integer */
-.pygments-style-lovelace .mo { color: #444; } /* Literal.Number.Oct */
-.pygments-style-lovelace .sa { color: #444; } /* Literal.String.Affix */
-.pygments-style-lovelace .sb { color: #b83838; } /* Literal.String.Backtick */
-.pygments-style-lovelace .sc { color: #a848a8; } /* Literal.String.Char */
-.pygments-style-lovelace .dl { color: #b85820; } /* Literal.String.Delimiter */
-.pygments-style-lovelace .sd {
-  color: #b85820;
-  font-style: italic;
-} /* Literal.String.Doc */
-.pygments-style-lovelace .s2 { color: #b83838; } /* Literal.String.Double */
-.pygments-style-lovelace .se { color: #709030; } /* Literal.String.Escape */
-.pygments-style-lovelace .sh { color: #b83838; } /* Literal.String.Heredoc */
-.pygments-style-lovelace .si {
-  color: #b83838;
-  text-decoration: underline;
-} /* Literal.String.Interpol */
-.pygments-style-lovelace .sx { color: #a848a8; } /* Literal.String.Other */
-.pygments-style-lovelace .sr { color: #a848a8; } /* Literal.String.Regex */
-.pygments-style-lovelace .s1 { color: #b83838; } /* Literal.String.Single */
-.pygments-style-lovelace .ss { color: #b83838; } /* Literal.String.Symbol */
-.pygments-style-lovelace .bp {
-  color: #388038;
-  font-style: italic;
-} /* Name.Builtin.Pseudo */
-.pygments-style-lovelace .fm { color: #b85820; } /* Name.Function.Magic */
-.pygments-style-lovelace .vc { color: #b04040; } /* Name.Variable.Class */
-.pygments-style-lovelace .vg { color: #908828; } /* Name.Variable.Global */
-.pygments-style-lovelace .vi { color: #b04040; } /* Name.Variable.Instance */
-.pygments-style-lovelace .vm { color: #b85820; } /* Name.Variable.Magic */
-.pygments-style-lovelace .il { color: #444; } /* Literal.Number.Integer.Long */
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+.pygments-style-lovelace .hll { background-color: #ffc }
+
+.pygments-style-lovelace { background: #fff; 
+}
+
+.pygments-style-lovelace .c { color: #888; 
+font-style: italic } /* Comment */
+.pygments-style-lovelace .err { background-color: #a848a8 } /* Error */
+.pygments-style-lovelace .k { color: #2838b0 } /* Keyword */
+.pygments-style-lovelace .o { color: #666 } /* Operator */
+.pygments-style-lovelace .p { color: #888 } /* Punctuation */
+.pygments-style-lovelace .ch { color: #287088; 
+font-style: italic } /* Comment.Hashbang */
+.pygments-style-lovelace .cm { color: #888; 
+font-style: italic } /* Comment.Multiline */
+.pygments-style-lovelace .cp { color: #289870 } /* Comment.Preproc */
+.pygments-style-lovelace .cpf { color: #888; 
+font-style: italic } /* Comment.PreprocFile */
+.pygments-style-lovelace .c1 { color: #888; 
+font-style: italic } /* Comment.Single */
+.pygments-style-lovelace .cs { color: #888; 
+font-style: italic } /* Comment.Special */
+.pygments-style-lovelace .gd { color: #c02828 } /* Generic.Deleted */
+.pygments-style-lovelace .ge { font-style: italic } /* Generic.Emph */
+.pygments-style-lovelace .ges { font-weight: bold; 
+font-style: italic } /* Generic.EmphStrong */
+.pygments-style-lovelace .gr { color: #c02828 } /* Generic.Error */
+.pygments-style-lovelace .gh { color: #666 } /* Generic.Heading */
+.pygments-style-lovelace .gi { color: #388038 } /* Generic.Inserted */
+.pygments-style-lovelace .go { color: #666 } /* Generic.Output */
+.pygments-style-lovelace .gp { color: #444 } /* Generic.Prompt */
+.pygments-style-lovelace .gs { font-weight: bold } /* Generic.Strong */
+.pygments-style-lovelace .gu { color: #444 } /* Generic.Subheading */
+.pygments-style-lovelace .gt { color: #2838b0 } /* Generic.Traceback */
+.pygments-style-lovelace .kc { color: #444; 
+font-style: italic } /* Keyword.Constant */
+.pygments-style-lovelace .kd { color: #2838b0; 
+font-style: italic } /* Keyword.Declaration */
+.pygments-style-lovelace .kn { color: #2838b0 } /* Keyword.Namespace */
+.pygments-style-lovelace .kp { color: #2838b0 } /* Keyword.Pseudo */
+.pygments-style-lovelace .kr { color: #2838b0 } /* Keyword.Reserved */
+.pygments-style-lovelace .kt { color: #2838b0; 
+font-style: italic } /* Keyword.Type */
+.pygments-style-lovelace .m { color: #444 } /* Literal.Number */
+.pygments-style-lovelace .s { color: #b83838 } /* Literal.String */
+.pygments-style-lovelace .na { color: #388038 } /* Name.Attribute */
+.pygments-style-lovelace .nb { color: #388038 } /* Name.Builtin */
+.pygments-style-lovelace .nc { color: #287088 } /* Name.Class */
+.pygments-style-lovelace .no { color: #b85820 } /* Name.Constant */
+.pygments-style-lovelace .nd { color: #287088 } /* Name.Decorator */
+.pygments-style-lovelace .ni { color: #709030 } /* Name.Entity */
+.pygments-style-lovelace .ne { color: #908828 } /* Name.Exception */
+.pygments-style-lovelace .nf { color: #785840 } /* Name.Function */
+.pygments-style-lovelace .nl { color: #289870 } /* Name.Label */
+.pygments-style-lovelace .nn { color: #289870 } /* Name.Namespace */
+.pygments-style-lovelace .nt { color: #2838b0 } /* Name.Tag */
+.pygments-style-lovelace .nv { color: #b04040 } /* Name.Variable */
+.pygments-style-lovelace .ow { color: #a848a8 } /* Operator.Word */
+.pygments-style-lovelace .pm { color: #888 } /* Punctuation.Marker */
+.pygments-style-lovelace .w { color: #a89028 } /* Text.Whitespace */
+.pygments-style-lovelace .mb { color: #444 } /* Literal.Number.Bin */
+.pygments-style-lovelace .mf { color: #444 } /* Literal.Number.Float */
+.pygments-style-lovelace .mh { color: #444 } /* Literal.Number.Hex */
+.pygments-style-lovelace .mi { color: #444 } /* Literal.Number.Integer */
+.pygments-style-lovelace .mo { color: #444 } /* Literal.Number.Oct */
+.pygments-style-lovelace .sa { color: #444 } /* Literal.String.Affix */
+.pygments-style-lovelace .sb { color: #b83838 } /* Literal.String.Backtick */
+.pygments-style-lovelace .sc { color: #a848a8 } /* Literal.String.Char */
+.pygments-style-lovelace .dl { color: #b85820 } /* Literal.String.Delimiter */
+.pygments-style-lovelace .sd { color: #b85820; 
+font-style: italic } /* Literal.String.Doc */
+.pygments-style-lovelace .s2 { color: #b83838 } /* Literal.String.Double */
+.pygments-style-lovelace .se { color: #709030 } /* Literal.String.Escape */
+.pygments-style-lovelace .sh { color: #b83838 } /* Literal.String.Heredoc */
+.pygments-style-lovelace .si { color: #b83838; 
+text-decoration: underline } /* Literal.String.Interpol */
+.pygments-style-lovelace .sx { color: #a848a8 } /* Literal.String.Other */
+.pygments-style-lovelace .sr { color: #a848a8 } /* Literal.String.Regex */
+.pygments-style-lovelace .s1 { color: #b83838 } /* Literal.String.Single */
+.pygments-style-lovelace .ss { color: #b83838 } /* Literal.String.Symbol */
+.pygments-style-lovelace .bp { color: #388038; 
+font-style: italic } /* Name.Builtin.Pseudo */
+.pygments-style-lovelace .fm { color: #b85820 } /* Name.Function.Magic */
+.pygments-style-lovelace .vc { color: #b04040 } /* Name.Variable.Class */
+.pygments-style-lovelace .vg { color: #908828 } /* Name.Variable.Global */
+.pygments-style-lovelace .vi { color: #b04040 } /* Name.Variable.Instance */
+.pygments-style-lovelace .vm { color: #b85820 } /* Name.Variable.Magic */
+.pygments-style-lovelace .il { color: #444 } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/manni.css` & `plumage-4.0.0/plumage/static/css/pygments/manni.css`

 * *Files 16% similar despite different names*

```diff
@@ -1,183 +1,127 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-.pygments-style-manni .hll { background-color: #ffc; }
-
-.pygments-style-manni {
-  background: #f0f3f3;
-}
-
-.pygments-style-manni .c {
-  color: #09f;
-  font-style: italic;
-} /* Comment */
-.pygments-style-manni .err {
-  color: #a00;
-  background-color: #faa;
-} /* Error */
-.pygments-style-manni .k {
-  color: #069;
-  font-weight: bold;
-} /* Keyword */
-.pygments-style-manni .o { color: #555; } /* Operator */
-.pygments-style-manni .ch {
-  color: #09f;
-  font-style: italic;
-} /* Comment.Hashbang */
-.pygments-style-manni .cm {
-  color: #09f;
-  font-style: italic;
-} /* Comment.Multiline */
-.pygments-style-manni .cp { color: #099; } /* Comment.Preproc */
-.pygments-style-manni .cpf {
-  color: #09f;
-  font-style: italic;
-} /* Comment.PreprocFile */
-.pygments-style-manni .c1 {
-  color: #09f;
-  font-style: italic;
-} /* Comment.Single */
-.pygments-style-manni .cs {
-  color: #09f;
-  font-weight: bold;
-  font-style: italic;
-} /* Comment.Special */
-.pygments-style-manni .gd {
-  background-color: #fcc;
-  border: 1px solid #c00;
-} /* Generic.Deleted */
-.pygments-style-manni .ge { font-style: italic; } /* Generic.Emph */
-.pygments-style-manni .gr { color: #f00; } /* Generic.Error */
-.pygments-style-manni .gh {
-  color: #030;
-  font-weight: bold;
-} /* Generic.Heading */
-.pygments-style-manni .gi {
-  background-color: #cfc;
-  border: 1px solid #0c0;
-} /* Generic.Inserted */
-.pygments-style-manni .go { color: #aaa; } /* Generic.Output */
-.pygments-style-manni .gp {
-  color: #009;
-  font-weight: bold;
-} /* Generic.Prompt */
-.pygments-style-manni .gs { font-weight: bold; } /* Generic.Strong */
-.pygments-style-manni .gu {
-  color: #030;
-  font-weight: bold;
-} /* Generic.Subheading */
-.pygments-style-manni .gt { color: #9c6; } /* Generic.Traceback */
-.pygments-style-manni .kc {
-  color: #069;
-  font-weight: bold;
-} /* Keyword.Constant */
-.pygments-style-manni .kd {
-  color: #069;
-  font-weight: bold;
-} /* Keyword.Declaration */
-.pygments-style-manni .kn {
-  color: #069;
-  font-weight: bold;
-} /* Keyword.Namespace */
-.pygments-style-manni .kp { color: #069; } /* Keyword.Pseudo */
-.pygments-style-manni .kr {
-  color: #069;
-  font-weight: bold;
-} /* Keyword.Reserved */
-.pygments-style-manni .kt {
-  color: #078;
-  font-weight: bold;
-} /* Keyword.Type */
-.pygments-style-manni .m { color: #f60; } /* Literal.Number */
-.pygments-style-manni .s { color: #c30; } /* Literal.String */
-.pygments-style-manni .na { color: #309; } /* Name.Attribute */
-.pygments-style-manni .nb { color: #366; } /* Name.Builtin */
-.pygments-style-manni .nc {
-  color: #0a8;
-  font-weight: bold;
-} /* Name.Class */
-.pygments-style-manni .no { color: #360; } /* Name.Constant */
-.pygments-style-manni .nd { color: #99f; } /* Name.Decorator */
-.pygments-style-manni .ni {
-  color: #999;
-  font-weight: bold;
-} /* Name.Entity */
-.pygments-style-manni .ne {
-  color: #c00;
-  font-weight: bold;
-} /* Name.Exception */
-.pygments-style-manni .nf { color: #c0f; } /* Name.Function */
-.pygments-style-manni .nl { color: #99f; } /* Name.Label */
-.pygments-style-manni .nn {
-  color: #0cf;
-  font-weight: bold;
-} /* Name.Namespace */
-.pygments-style-manni .nt {
-  color: #309;
-  font-weight: bold;
-} /* Name.Tag */
-.pygments-style-manni .nv { color: #033; } /* Name.Variable */
-.pygments-style-manni .ow {
-  color: #000;
-  font-weight: bold;
-} /* Operator.Word */
-.pygments-style-manni .w { color: #bbb; } /* Text.Whitespace */
-.pygments-style-manni .mb { color: #f60; } /* Literal.Number.Bin */
-.pygments-style-manni .mf { color: #f60; } /* Literal.Number.Float */
-.pygments-style-manni .mh { color: #f60; } /* Literal.Number.Hex */
-.pygments-style-manni .mi { color: #f60; } /* Literal.Number.Integer */
-.pygments-style-manni .mo { color: #f60; } /* Literal.Number.Oct */
-.pygments-style-manni .sa { color: #c30; } /* Literal.String.Affix */
-.pygments-style-manni .sb { color: #c30; } /* Literal.String.Backtick */
-.pygments-style-manni .sc { color: #c30; } /* Literal.String.Char */
-.pygments-style-manni .dl { color: #c30; } /* Literal.String.Delimiter */
-.pygments-style-manni .sd {
-  color: #c30;
-  font-style: italic;
-} /* Literal.String.Doc */
-.pygments-style-manni .s2 { color: #c30; } /* Literal.String.Double */
-.pygments-style-manni .se {
-  color: #c30;
-  font-weight: bold;
-} /* Literal.String.Escape */
-.pygments-style-manni .sh { color: #c30; } /* Literal.String.Heredoc */
-.pygments-style-manni .si { color: #a00; } /* Literal.String.Interpol */
-.pygments-style-manni .sx { color: #c30; } /* Literal.String.Other */
-.pygments-style-manni .sr { color: #3aa; } /* Literal.String.Regex */
-.pygments-style-manni .s1 { color: #c30; } /* Literal.String.Single */
-.pygments-style-manni .ss { color: #fc3; } /* Literal.String.Symbol */
-.pygments-style-manni .bp { color: #366; } /* Name.Builtin.Pseudo */
-.pygments-style-manni .fm { color: #c0f; } /* Name.Function.Magic */
-.pygments-style-manni .vc { color: #033; } /* Name.Variable.Class */
-.pygments-style-manni .vg { color: #033; } /* Name.Variable.Global */
-.pygments-style-manni .vi { color: #033; } /* Name.Variable.Instance */
-.pygments-style-manni .vm { color: #033; } /* Name.Variable.Magic */
-.pygments-style-manni .il { color: #f60; } /* Literal.Number.Integer.Long */
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+.pygments-style-manni .hll { background-color: #ffc }
+
+.pygments-style-manni { background: #f0f3f3; 
+}
+
+.pygments-style-manni .c { color: #09F; 
+font-style: italic } /* Comment */
+.pygments-style-manni .err { color: #A00; 
+background-color: #FAA } /* Error */
+.pygments-style-manni .k { color: #069; 
+font-weight: bold } /* Keyword */
+.pygments-style-manni .o { color: #555 } /* Operator */
+.pygments-style-manni .ch { color: #09F; 
+font-style: italic } /* Comment.Hashbang */
+.pygments-style-manni .cm { color: #09F; 
+font-style: italic } /* Comment.Multiline */
+.pygments-style-manni .cp { color: #099 } /* Comment.Preproc */
+.pygments-style-manni .cpf { color: #09F; 
+font-style: italic } /* Comment.PreprocFile */
+.pygments-style-manni .c1 { color: #09F; 
+font-style: italic } /* Comment.Single */
+.pygments-style-manni .cs { color: #09F; 
+font-weight: bold; 
+font-style: italic } /* Comment.Special */
+.pygments-style-manni .gd { background-color: #FCC; 
+border: 1px solid #C00 } /* Generic.Deleted */
+.pygments-style-manni .ge { font-style: italic } /* Generic.Emph */
+.pygments-style-manni .ges { font-weight: bold; 
+font-style: italic } /* Generic.EmphStrong */
+.pygments-style-manni .gr { color: #F00 } /* Generic.Error */
+.pygments-style-manni .gh { color: #030; 
+font-weight: bold } /* Generic.Heading */
+.pygments-style-manni .gi { background-color: #CFC; 
+border: 1px solid #0C0 } /* Generic.Inserted */
+.pygments-style-manni .go { color: #AAA } /* Generic.Output */
+.pygments-style-manni .gp { color: #009; 
+font-weight: bold } /* Generic.Prompt */
+.pygments-style-manni .gs { font-weight: bold } /* Generic.Strong */
+.pygments-style-manni .gu { color: #030; 
+font-weight: bold } /* Generic.Subheading */
+.pygments-style-manni .gt { color: #9C6 } /* Generic.Traceback */
+.pygments-style-manni .kc { color: #069; 
+font-weight: bold } /* Keyword.Constant */
+.pygments-style-manni .kd { color: #069; 
+font-weight: bold } /* Keyword.Declaration */
+.pygments-style-manni .kn { color: #069; 
+font-weight: bold } /* Keyword.Namespace */
+.pygments-style-manni .kp { color: #069 } /* Keyword.Pseudo */
+.pygments-style-manni .kr { color: #069; 
+font-weight: bold } /* Keyword.Reserved */
+.pygments-style-manni .kt { color: #078; 
+font-weight: bold } /* Keyword.Type */
+.pygments-style-manni .m { color: #F60 } /* Literal.Number */
+.pygments-style-manni .s { color: #C30 } /* Literal.String */
+.pygments-style-manni .na { color: #309 } /* Name.Attribute */
+.pygments-style-manni .nb { color: #366 } /* Name.Builtin */
+.pygments-style-manni .nc { color: #0A8; 
+font-weight: bold } /* Name.Class */
+.pygments-style-manni .no { color: #360 } /* Name.Constant */
+.pygments-style-manni .nd { color: #99F } /* Name.Decorator */
+.pygments-style-manni .ni { color: #999; 
+font-weight: bold } /* Name.Entity */
+.pygments-style-manni .ne { color: #C00; 
+font-weight: bold } /* Name.Exception */
+.pygments-style-manni .nf { color: #C0F } /* Name.Function */
+.pygments-style-manni .nl { color: #99F } /* Name.Label */
+.pygments-style-manni .nn { color: #0CF; 
+font-weight: bold } /* Name.Namespace */
+.pygments-style-manni .nt { color: #309; 
+font-weight: bold } /* Name.Tag */
+.pygments-style-manni .nv { color: #033 } /* Name.Variable */
+.pygments-style-manni .ow { color: #000; 
+font-weight: bold } /* Operator.Word */
+.pygments-style-manni .w { color: #bbb } /* Text.Whitespace */
+.pygments-style-manni .mb { color: #F60 } /* Literal.Number.Bin */
+.pygments-style-manni .mf { color: #F60 } /* Literal.Number.Float */
+.pygments-style-manni .mh { color: #F60 } /* Literal.Number.Hex */
+.pygments-style-manni .mi { color: #F60 } /* Literal.Number.Integer */
+.pygments-style-manni .mo { color: #F60 } /* Literal.Number.Oct */
+.pygments-style-manni .sa { color: #C30 } /* Literal.String.Affix */
+.pygments-style-manni .sb { color: #C30 } /* Literal.String.Backtick */
+.pygments-style-manni .sc { color: #C30 } /* Literal.String.Char */
+.pygments-style-manni .dl { color: #C30 } /* Literal.String.Delimiter */
+.pygments-style-manni .sd { color: #C30; 
+font-style: italic } /* Literal.String.Doc */
+.pygments-style-manni .s2 { color: #C30 } /* Literal.String.Double */
+.pygments-style-manni .se { color: #C30; 
+font-weight: bold } /* Literal.String.Escape */
+.pygments-style-manni .sh { color: #C30 } /* Literal.String.Heredoc */
+.pygments-style-manni .si { color: #A00 } /* Literal.String.Interpol */
+.pygments-style-manni .sx { color: #C30 } /* Literal.String.Other */
+.pygments-style-manni .sr { color: #3AA } /* Literal.String.Regex */
+.pygments-style-manni .s1 { color: #C30 } /* Literal.String.Single */
+.pygments-style-manni .ss { color: #FC3 } /* Literal.String.Symbol */
+.pygments-style-manni .bp { color: #366 } /* Name.Builtin.Pseudo */
+.pygments-style-manni .fm { color: #C0F } /* Name.Function.Magic */
+.pygments-style-manni .vc { color: #033 } /* Name.Variable.Class */
+.pygments-style-manni .vg { color: #033 } /* Name.Variable.Global */
+.pygments-style-manni .vi { color: #033 } /* Name.Variable.Instance */
+.pygments-style-manni .vm { color: #033 } /* Name.Variable.Magic */
+.pygments-style-manni .il { color: #F60 } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/monokai.css` & `plumage-4.0.0/plumage/static/css/pygments/monokai.css`

 * *Files 9% similar despite different names*

```diff
@@ -1,113 +1,114 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
-.pygments-style-monokai .hll { background-color: #49483e; }
+.pygments-style-monokai .hll { background-color: #49483e }
 
-.pygments-style-monokai {
-  background: #272822;
-  color: #f8f8f2;
-}
-.pygments-style-monokai .c { color: #75715e; } /* Comment */
-.pygments-style-monokai .err {
-  color: #960050;
-  background-color: #1e0010;
-} /* Error */
-.pygments-style-monokai .k { color: #66d9ef; } /* Keyword */
-.pygments-style-monokai .l { color: #ae81ff; } /* Literal */
-.pygments-style-monokai .n { color: #f8f8f2; } /* Name */
-.pygments-style-monokai .o { color: #f92672; } /* Operator */
-.pygments-style-monokai .p { color: #f8f8f2; } /* Punctuation */
-.pygments-style-monokai .ch { color: #75715e; } /* Comment.Hashbang */
-.pygments-style-monokai .cm { color: #75715e; } /* Comment.Multiline */
-.pygments-style-monokai .cp { color: #75715e; } /* Comment.Preproc */
-.pygments-style-monokai .cpf { color: #75715e; } /* Comment.PreprocFile */
-.pygments-style-monokai .c1 { color: #75715e; } /* Comment.Single */
-.pygments-style-monokai .cs { color: #75715e; } /* Comment.Special */
-.pygments-style-monokai .gd { color: #f92672; } /* Generic.Deleted */
-.pygments-style-monokai .ge { font-style: italic; } /* Generic.Emph */
-.pygments-style-monokai .gi { color: #a6e22e; } /* Generic.Inserted */
-.pygments-style-monokai .go { color: #66d9ef; } /* Generic.Output */
-.pygments-style-monokai .gp {
-  color: #f92672;
-  font-weight: bold;
-} /* Generic.Prompt */
-.pygments-style-monokai .gs { font-weight: bold; } /* Generic.Strong */
-.pygments-style-monokai .gu { color: #75715e; } /* Generic.Subheading */
-.pygments-style-monokai .kc { color: #66d9ef; } /* Keyword.Constant */
-.pygments-style-monokai .kd { color: #66d9ef; } /* Keyword.Declaration */
-.pygments-style-monokai .kn { color: #f92672; } /* Keyword.Namespace */
-.pygments-style-monokai .kp { color: #66d9ef; } /* Keyword.Pseudo */
-.pygments-style-monokai .kr { color: #66d9ef; } /* Keyword.Reserved */
-.pygments-style-monokai .kt { color: #66d9ef; } /* Keyword.Type */
-.pygments-style-monokai .ld { color: #e6db74; } /* Literal.Date */
-.pygments-style-monokai .m { color: #ae81ff; } /* Literal.Number */
-.pygments-style-monokai .s { color: #e6db74; } /* Literal.String */
-.pygments-style-monokai .na { color: #a6e22e; } /* Name.Attribute */
-.pygments-style-monokai .nb { color: #f8f8f2; } /* Name.Builtin */
-.pygments-style-monokai .nc { color: #a6e22e; } /* Name.Class */
-.pygments-style-monokai .no { color: #66d9ef; } /* Name.Constant */
-.pygments-style-monokai .nd { color: #a6e22e; } /* Name.Decorator */
-.pygments-style-monokai .ni { color: #f8f8f2; } /* Name.Entity */
-.pygments-style-monokai .ne { color: #a6e22e; } /* Name.Exception */
-.pygments-style-monokai .nf { color: #a6e22e; } /* Name.Function */
-.pygments-style-monokai .nl { color: #f8f8f2; } /* Name.Label */
-.pygments-style-monokai .nn { color: #f8f8f2; } /* Name.Namespace */
-.pygments-style-monokai .nx { color: #a6e22e; } /* Name.Other */
-.pygments-style-monokai .py { color: #f8f8f2; } /* Name.Property */
-.pygments-style-monokai .nt { color: #f92672; } /* Name.Tag */
-.pygments-style-monokai .nv { color: #f8f8f2; } /* Name.Variable */
-.pygments-style-monokai .ow { color: #f92672; } /* Operator.Word */
-.pygments-style-monokai .w { color: #f8f8f2; } /* Text.Whitespace */
-.pygments-style-monokai .mb { color: #ae81ff; } /* Literal.Number.Bin */
-.pygments-style-monokai .mf { color: #ae81ff; } /* Literal.Number.Float */
-.pygments-style-monokai .mh { color: #ae81ff; } /* Literal.Number.Hex */
-.pygments-style-monokai .mi { color: #ae81ff; } /* Literal.Number.Integer */
-.pygments-style-monokai .mo { color: #ae81ff; } /* Literal.Number.Oct */
-.pygments-style-monokai .sa { color: #e6db74; } /* Literal.String.Affix */
-.pygments-style-monokai .sb { color: #e6db74; } /* Literal.String.Backtick */
-.pygments-style-monokai .sc { color: #e6db74; } /* Literal.String.Char */
-.pygments-style-monokai .dl { color: #e6db74; } /* Literal.String.Delimiter */
-.pygments-style-monokai .sd { color: #e6db74; } /* Literal.String.Doc */
-.pygments-style-monokai .s2 { color: #e6db74; } /* Literal.String.Double */
-.pygments-style-monokai .se { color: #ae81ff; } /* Literal.String.Escape */
-.pygments-style-monokai .sh { color: #e6db74; } /* Literal.String.Heredoc */
-.pygments-style-monokai .si { color: #e6db74; } /* Literal.String.Interpol */
-.pygments-style-monokai .sx { color: #e6db74; } /* Literal.String.Other */
-.pygments-style-monokai .sr { color: #e6db74; } /* Literal.String.Regex */
-.pygments-style-monokai .s1 { color: #e6db74; } /* Literal.String.Single */
-.pygments-style-monokai .ss { color: #e6db74; } /* Literal.String.Symbol */
-.pygments-style-monokai .bp { color: #f8f8f2; } /* Name.Builtin.Pseudo */
-.pygments-style-monokai .fm { color: #a6e22e; } /* Name.Function.Magic */
-.pygments-style-monokai .vc { color: #f8f8f2; } /* Name.Variable.Class */
-.pygments-style-monokai .vg { color: #f8f8f2; } /* Name.Variable.Global */
-.pygments-style-monokai .vi { color: #f8f8f2; } /* Name.Variable.Instance */
-.pygments-style-monokai .vm { color: #f8f8f2; } /* Name.Variable.Magic */
-.pygments-style-monokai .il { color: #ae81ff; } /* Literal.Number.Integer.Long */
+.pygments-style-monokai { background: #272822; 
+color: #f8f8f2 }
+.pygments-style-monokai .c { color: #959077 } /* Comment */
+.pygments-style-monokai .err { color: #ed007e; 
+background-color: #1e0010 } /* Error */
+.pygments-style-monokai .esc { color: #f8f8f2 } /* Escape */
+.pygments-style-monokai .g { color: #f8f8f2 } /* Generic */
+.pygments-style-monokai .k { color: #66d9ef } /* Keyword */
+.pygments-style-monokai .l { color: #ae81ff } /* Literal */
+.pygments-style-monokai .n { color: #f8f8f2 } /* Name */
+.pygments-style-monokai .o { color: #ff4689 } /* Operator */
+.pygments-style-monokai .x { color: #f8f8f2 } /* Other */
+.pygments-style-monokai .p { color: #f8f8f2 } /* Punctuation */
+.pygments-style-monokai .ch { color: #959077 } /* Comment.Hashbang */
+.pygments-style-monokai .cm { color: #959077 } /* Comment.Multiline */
+.pygments-style-monokai .cp { color: #959077 } /* Comment.Preproc */
+.pygments-style-monokai .cpf { color: #959077 } /* Comment.PreprocFile */
+.pygments-style-monokai .c1 { color: #959077 } /* Comment.Single */
+.pygments-style-monokai .cs { color: #959077 } /* Comment.Special */
+.pygments-style-monokai .gd { color: #ff4689 } /* Generic.Deleted */
+.pygments-style-monokai .ge { color: #f8f8f2; 
+font-style: italic } /* Generic.Emph */
+.pygments-style-monokai .ges { color: #f8f8f2; 
+font-weight: bold; 
+font-style: italic } /* Generic.EmphStrong */
+.pygments-style-monokai .gr { color: #f8f8f2 } /* Generic.Error */
+.pygments-style-monokai .gh { color: #f8f8f2 } /* Generic.Heading */
+.pygments-style-monokai .gi { color: #a6e22e } /* Generic.Inserted */
+.pygments-style-monokai .go { color: #66d9ef } /* Generic.Output */
+.pygments-style-monokai .gp { color: #ff4689; 
+font-weight: bold } /* Generic.Prompt */
+.pygments-style-monokai .gs { color: #f8f8f2; 
+font-weight: bold } /* Generic.Strong */
+.pygments-style-monokai .gu { color: #959077 } /* Generic.Subheading */
+.pygments-style-monokai .gt { color: #f8f8f2 } /* Generic.Traceback */
+.pygments-style-monokai .kc { color: #66d9ef } /* Keyword.Constant */
+.pygments-style-monokai .kd { color: #66d9ef } /* Keyword.Declaration */
+.pygments-style-monokai .kn { color: #ff4689 } /* Keyword.Namespace */
+.pygments-style-monokai .kp { color: #66d9ef } /* Keyword.Pseudo */
+.pygments-style-monokai .kr { color: #66d9ef } /* Keyword.Reserved */
+.pygments-style-monokai .kt { color: #66d9ef } /* Keyword.Type */
+.pygments-style-monokai .ld { color: #e6db74 } /* Literal.Date */
+.pygments-style-monokai .m { color: #ae81ff } /* Literal.Number */
+.pygments-style-monokai .s { color: #e6db74 } /* Literal.String */
+.pygments-style-monokai .na { color: #a6e22e } /* Name.Attribute */
+.pygments-style-monokai .nb { color: #f8f8f2 } /* Name.Builtin */
+.pygments-style-monokai .nc { color: #a6e22e } /* Name.Class */
+.pygments-style-monokai .no { color: #66d9ef } /* Name.Constant */
+.pygments-style-monokai .nd { color: #a6e22e } /* Name.Decorator */
+.pygments-style-monokai .ni { color: #f8f8f2 } /* Name.Entity */
+.pygments-style-monokai .ne { color: #a6e22e } /* Name.Exception */
+.pygments-style-monokai .nf { color: #a6e22e } /* Name.Function */
+.pygments-style-monokai .nl { color: #f8f8f2 } /* Name.Label */
+.pygments-style-monokai .nn { color: #f8f8f2 } /* Name.Namespace */
+.pygments-style-monokai .nx { color: #a6e22e } /* Name.Other */
+.pygments-style-monokai .py { color: #f8f8f2 } /* Name.Property */
+.pygments-style-monokai .nt { color: #ff4689 } /* Name.Tag */
+.pygments-style-monokai .nv { color: #f8f8f2 } /* Name.Variable */
+.pygments-style-monokai .ow { color: #ff4689 } /* Operator.Word */
+.pygments-style-monokai .pm { color: #f8f8f2 } /* Punctuation.Marker */
+.pygments-style-monokai .w { color: #f8f8f2 } /* Text.Whitespace */
+.pygments-style-monokai .mb { color: #ae81ff } /* Literal.Number.Bin */
+.pygments-style-monokai .mf { color: #ae81ff } /* Literal.Number.Float */
+.pygments-style-monokai .mh { color: #ae81ff } /* Literal.Number.Hex */
+.pygments-style-monokai .mi { color: #ae81ff } /* Literal.Number.Integer */
+.pygments-style-monokai .mo { color: #ae81ff } /* Literal.Number.Oct */
+.pygments-style-monokai .sa { color: #e6db74 } /* Literal.String.Affix */
+.pygments-style-monokai .sb { color: #e6db74 } /* Literal.String.Backtick */
+.pygments-style-monokai .sc { color: #e6db74 } /* Literal.String.Char */
+.pygments-style-monokai .dl { color: #e6db74 } /* Literal.String.Delimiter */
+.pygments-style-monokai .sd { color: #e6db74 } /* Literal.String.Doc */
+.pygments-style-monokai .s2 { color: #e6db74 } /* Literal.String.Double */
+.pygments-style-monokai .se { color: #ae81ff } /* Literal.String.Escape */
+.pygments-style-monokai .sh { color: #e6db74 } /* Literal.String.Heredoc */
+.pygments-style-monokai .si { color: #e6db74 } /* Literal.String.Interpol */
+.pygments-style-monokai .sx { color: #e6db74 } /* Literal.String.Other */
+.pygments-style-monokai .sr { color: #e6db74 } /* Literal.String.Regex */
+.pygments-style-monokai .s1 { color: #e6db74 } /* Literal.String.Single */
+.pygments-style-monokai .ss { color: #e6db74 } /* Literal.String.Symbol */
+.pygments-style-monokai .bp { color: #f8f8f2 } /* Name.Builtin.Pseudo */
+.pygments-style-monokai .fm { color: #a6e22e } /* Name.Function.Magic */
+.pygments-style-monokai .vc { color: #f8f8f2 } /* Name.Variable.Class */
+.pygments-style-monokai .vg { color: #f8f8f2 } /* Name.Variable.Global */
+.pygments-style-monokai .vi { color: #f8f8f2 } /* Name.Variable.Instance */
+.pygments-style-monokai .vm { color: #f8f8f2 } /* Name.Variable.Magic */
+.pygments-style-monokai .il { color: #ae81ff } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/murphy.css` & `plumage-4.0.0/plumage/static/css/pygments/murphy.css`

 * *Files 25% similar despite different names*

```diff
@@ -1,214 +1,138 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-.pygments-style-murphy .hll { background-color: #ffc; }
-
-.pygments-style-murphy {
-  background: #fff;
-}
-
-.pygments-style-murphy .c {
-  color: #666;
-  font-style: italic;
-} /* Comment */
-.pygments-style-murphy .err {
-  color: #f00;
-  background-color: #faa;
-} /* Error */
-.pygments-style-murphy .k {
-  color: #289;
-  font-weight: bold;
-} /* Keyword */
-.pygments-style-murphy .o { color: #333; } /* Operator */
-.pygments-style-murphy .ch {
-  color: #666;
-  font-style: italic;
-} /* Comment.Hashbang */
-.pygments-style-murphy .cm {
-  color: #666;
-  font-style: italic;
-} /* Comment.Multiline */
-.pygments-style-murphy .cp { color: #579; } /* Comment.Preproc */
-.pygments-style-murphy .cpf {
-  color: #666;
-  font-style: italic;
-} /* Comment.PreprocFile */
-.pygments-style-murphy .c1 {
-  color: #666;
-  font-style: italic;
-} /* Comment.Single */
-.pygments-style-murphy .cs {
-  color: #c00;
-  font-weight: bold;
-  font-style: italic;
-} /* Comment.Special */
-.pygments-style-murphy .gd { color: #a00000; } /* Generic.Deleted */
-.pygments-style-murphy .ge { font-style: italic; } /* Generic.Emph */
-.pygments-style-murphy .gr { color: #f00; } /* Generic.Error */
-.pygments-style-murphy .gh {
-  color: #000080;
-  font-weight: bold;
-} /* Generic.Heading */
-.pygments-style-murphy .gi { color: #00a000; } /* Generic.Inserted */
-.pygments-style-murphy .go { color: #888; } /* Generic.Output */
-.pygments-style-murphy .gp {
-  color: #c65d09;
-  font-weight: bold;
-} /* Generic.Prompt */
-.pygments-style-murphy .gs { font-weight: bold; } /* Generic.Strong */
-.pygments-style-murphy .gu {
-  color: #800080;
-  font-weight: bold;
-} /* Generic.Subheading */
-.pygments-style-murphy .gt { color: #04d; } /* Generic.Traceback */
-.pygments-style-murphy .kc {
-  color: #289;
-  font-weight: bold;
-} /* Keyword.Constant */
-.pygments-style-murphy .kd {
-  color: #289;
-  font-weight: bold;
-} /* Keyword.Declaration */
-.pygments-style-murphy .kn {
-  color: #289;
-  font-weight: bold;
-} /* Keyword.Namespace */
-.pygments-style-murphy .kp {
-  color: #08f;
-  font-weight: bold;
-} /* Keyword.Pseudo */
-.pygments-style-murphy .kr {
-  color: #289;
-  font-weight: bold;
-} /* Keyword.Reserved */
-.pygments-style-murphy .kt {
-  color: #66f;
-  font-weight: bold;
-} /* Keyword.Type */
-.pygments-style-murphy .m {
-  color: #60e;
-  font-weight: bold;
-} /* Literal.Number */
-.pygments-style-murphy .s { background-color: #e0e0ff; } /* Literal.String */
-.pygments-style-murphy .na { color: #007; } /* Name.Attribute */
-.pygments-style-murphy .nb { color: #072; } /* Name.Builtin */
-.pygments-style-murphy .nc {
-  color: #e9e;
-  font-weight: bold;
-} /* Name.Class */
-.pygments-style-murphy .no {
-  color: #5ed;
-  font-weight: bold;
-} /* Name.Constant */
-.pygments-style-murphy .nd {
-  color: #555;
-  font-weight: bold;
-} /* Name.Decorator */
-.pygments-style-murphy .ni { color: #800; } /* Name.Entity */
-.pygments-style-murphy .ne {
-  color: #f00;
-  font-weight: bold;
-} /* Name.Exception */
-.pygments-style-murphy .nf {
-  color: #5ed;
-  font-weight: bold;
-} /* Name.Function */
-.pygments-style-murphy .nl {
-  color: #970;
-  font-weight: bold;
-} /* Name.Label */
-.pygments-style-murphy .nn {
-  color: #0e84b5;
-  font-weight: bold;
-} /* Name.Namespace */
-.pygments-style-murphy .nt { color: #070; } /* Name.Tag */
-.pygments-style-murphy .nv { color: #036; } /* Name.Variable */
-.pygments-style-murphy .ow {
-  color: #000;
-  font-weight: bold;
-} /* Operator.Word */
-.pygments-style-murphy .w { color: #bbb; } /* Text.Whitespace */
-.pygments-style-murphy .mb {
-  color: #60e;
-  font-weight: bold;
-} /* Literal.Number.Bin */
-.pygments-style-murphy .mf {
-  color: #60e;
-  font-weight: bold;
-} /* Literal.Number.Float */
-.pygments-style-murphy .mh {
-  color: #058;
-  font-weight: bold;
-} /* Literal.Number.Hex */
-.pygments-style-murphy .mi {
-  color: #66f;
-  font-weight: bold;
-} /* Literal.Number.Integer */
-.pygments-style-murphy .mo {
-  color: #40e;
-  font-weight: bold;
-} /* Literal.Number.Oct */
-.pygments-style-murphy .sa { background-color: #e0e0ff; } /* Literal.String.Affix */
-.pygments-style-murphy .sb { background-color: #e0e0ff; } /* Literal.String.Backtick */
-.pygments-style-murphy .sc { color: #88f; } /* Literal.String.Char */
-.pygments-style-murphy .dl { background-color: #e0e0ff; } /* Literal.String.Delimiter */
-.pygments-style-murphy .sd { color: #d42; } /* Literal.String.Doc */
-.pygments-style-murphy .s2 { background-color: #e0e0ff; } /* Literal.String.Double */
-.pygments-style-murphy .se {
-  color: #666;
-  font-weight: bold;
-  background-color: #e0e0ff;
-} /* Literal.String.Escape */
-.pygments-style-murphy .sh { background-color: #e0e0ff; } /* Literal.String.Heredoc */
-.pygments-style-murphy .si { background-color: #eee; } /* Literal.String.Interpol */
-.pygments-style-murphy .sx {
-  color: #f88;
-  background-color: #e0e0ff;
-} /* Literal.String.Other */
-.pygments-style-murphy .sr {
-  color: #000;
-  background-color: #e0e0ff;
-} /* Literal.String.Regex */
-.pygments-style-murphy .s1 { background-color: #e0e0ff; } /* Literal.String.Single */
-.pygments-style-murphy .ss { color: #fc8; } /* Literal.String.Symbol */
-.pygments-style-murphy .bp { color: #072; } /* Name.Builtin.Pseudo */
-.pygments-style-murphy .fm {
-  color: #5ed;
-  font-weight: bold;
-} /* Name.Function.Magic */
-.pygments-style-murphy .vc { color: #ccf; } /* Name.Variable.Class */
-.pygments-style-murphy .vg { color: #f84; } /* Name.Variable.Global */
-.pygments-style-murphy .vi { color: #aaf; } /* Name.Variable.Instance */
-.pygments-style-murphy .vm { color: #036; } /* Name.Variable.Magic */
-.pygments-style-murphy .il {
-  color: #66f;
-  font-weight: bold;
-} /* Literal.Number.Integer.Long */
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+.pygments-style-murphy .hll { background-color: #ffc }
+
+.pygments-style-murphy { background: #fff; 
+}
+
+.pygments-style-murphy .c { color: #666; 
+font-style: italic } /* Comment */
+.pygments-style-murphy .err { color: #F00; 
+background-color: #FAA } /* Error */
+.pygments-style-murphy .k { color: #289; 
+font-weight: bold } /* Keyword */
+.pygments-style-murphy .o { color: #333 } /* Operator */
+.pygments-style-murphy .ch { color: #666; 
+font-style: italic } /* Comment.Hashbang */
+.pygments-style-murphy .cm { color: #666; 
+font-style: italic } /* Comment.Multiline */
+.pygments-style-murphy .cp { color: #579 } /* Comment.Preproc */
+.pygments-style-murphy .cpf { color: #666; 
+font-style: italic } /* Comment.PreprocFile */
+.pygments-style-murphy .c1 { color: #666; 
+font-style: italic } /* Comment.Single */
+.pygments-style-murphy .cs { color: #c00; 
+font-weight: bold; 
+font-style: italic } /* Comment.Special */
+.pygments-style-murphy .gd { color: #A00000 } /* Generic.Deleted */
+.pygments-style-murphy .ge { font-style: italic } /* Generic.Emph */
+.pygments-style-murphy .ges { font-weight: bold; 
+font-style: italic } /* Generic.EmphStrong */
+.pygments-style-murphy .gr { color: #F00 } /* Generic.Error */
+.pygments-style-murphy .gh { color: #000080; 
+font-weight: bold } /* Generic.Heading */
+.pygments-style-murphy .gi { color: #00A000 } /* Generic.Inserted */
+.pygments-style-murphy .go { color: #888 } /* Generic.Output */
+.pygments-style-murphy .gp { color: #c65d09; 
+font-weight: bold } /* Generic.Prompt */
+.pygments-style-murphy .gs { font-weight: bold } /* Generic.Strong */
+.pygments-style-murphy .gu { color: #800080; 
+font-weight: bold } /* Generic.Subheading */
+.pygments-style-murphy .gt { color: #04D } /* Generic.Traceback */
+.pygments-style-murphy .kc { color: #289; 
+font-weight: bold } /* Keyword.Constant */
+.pygments-style-murphy .kd { color: #289; 
+font-weight: bold } /* Keyword.Declaration */
+.pygments-style-murphy .kn { color: #289; 
+font-weight: bold } /* Keyword.Namespace */
+.pygments-style-murphy .kp { color: #08f; 
+font-weight: bold } /* Keyword.Pseudo */
+.pygments-style-murphy .kr { color: #289; 
+font-weight: bold } /* Keyword.Reserved */
+.pygments-style-murphy .kt { color: #66f; 
+font-weight: bold } /* Keyword.Type */
+.pygments-style-murphy .m { color: #60E; 
+font-weight: bold } /* Literal.Number */
+.pygments-style-murphy .s { background-color: #e0e0ff } /* Literal.String */
+.pygments-style-murphy .na { color: #007 } /* Name.Attribute */
+.pygments-style-murphy .nb { color: #072 } /* Name.Builtin */
+.pygments-style-murphy .nc { color: #e9e; 
+font-weight: bold } /* Name.Class */
+.pygments-style-murphy .no { color: #5ed; 
+font-weight: bold } /* Name.Constant */
+.pygments-style-murphy .nd { color: #555; 
+font-weight: bold } /* Name.Decorator */
+.pygments-style-murphy .ni { color: #800 } /* Name.Entity */
+.pygments-style-murphy .ne { color: #F00; 
+font-weight: bold } /* Name.Exception */
+.pygments-style-murphy .nf { color: #5ed; 
+font-weight: bold } /* Name.Function */
+.pygments-style-murphy .nl { color: #970; 
+font-weight: bold } /* Name.Label */
+.pygments-style-murphy .nn { color: #0e84b5; 
+font-weight: bold } /* Name.Namespace */
+.pygments-style-murphy .nt { color: #070 } /* Name.Tag */
+.pygments-style-murphy .nv { color: #036 } /* Name.Variable */
+.pygments-style-murphy .ow { color: #000; 
+font-weight: bold } /* Operator.Word */
+.pygments-style-murphy .w { color: #bbb } /* Text.Whitespace */
+.pygments-style-murphy .mb { color: #60E; 
+font-weight: bold } /* Literal.Number.Bin */
+.pygments-style-murphy .mf { color: #60E; 
+font-weight: bold } /* Literal.Number.Float */
+.pygments-style-murphy .mh { color: #058; 
+font-weight: bold } /* Literal.Number.Hex */
+.pygments-style-murphy .mi { color: #66f; 
+font-weight: bold } /* Literal.Number.Integer */
+.pygments-style-murphy .mo { color: #40E; 
+font-weight: bold } /* Literal.Number.Oct */
+.pygments-style-murphy .sa { background-color: #e0e0ff } /* Literal.String.Affix */
+.pygments-style-murphy .sb { background-color: #e0e0ff } /* Literal.String.Backtick */
+.pygments-style-murphy .sc { color: #88F } /* Literal.String.Char */
+.pygments-style-murphy .dl { background-color: #e0e0ff } /* Literal.String.Delimiter */
+.pygments-style-murphy .sd { color: #D42 } /* Literal.String.Doc */
+.pygments-style-murphy .s2 { background-color: #e0e0ff } /* Literal.String.Double */
+.pygments-style-murphy .se { color: #666; 
+font-weight: bold; 
+background-color: #e0e0ff } /* Literal.String.Escape */
+.pygments-style-murphy .sh { background-color: #e0e0ff } /* Literal.String.Heredoc */
+.pygments-style-murphy .si { background-color: #eee } /* Literal.String.Interpol */
+.pygments-style-murphy .sx { color: #f88; 
+background-color: #e0e0ff } /* Literal.String.Other */
+.pygments-style-murphy .sr { color: #000; 
+background-color: #e0e0ff } /* Literal.String.Regex */
+.pygments-style-murphy .s1 { background-color: #e0e0ff } /* Literal.String.Single */
+.pygments-style-murphy .ss { color: #fc8 } /* Literal.String.Symbol */
+.pygments-style-murphy .bp { color: #072 } /* Name.Builtin.Pseudo */
+.pygments-style-murphy .fm { color: #5ed; 
+font-weight: bold } /* Name.Function.Magic */
+.pygments-style-murphy .vc { color: #ccf } /* Name.Variable.Class */
+.pygments-style-murphy .vg { color: #f84 } /* Name.Variable.Global */
+.pygments-style-murphy .vi { color: #aaf } /* Name.Variable.Instance */
+.pygments-style-murphy .vm { color: #036 } /* Name.Variable.Magic */
+.pygments-style-murphy .il { color: #66f; 
+font-weight: bold } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/native.css` & `plumage-4.0.0/plumage/static/css/pygments/paraiso-dark.css`

 * *Files 21% similar despite different names*

```diff
@@ -1,181 +1,106 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-.pygments-style-native .hll { background-color: #404040; }
-
-.pygments-style-native {
-  background: #202020;
-  color: #d0d0d0;
-}
-
-.pygments-style-native .c {
-  color: #999;
-  font-style: italic;
-} /* Comment */
-.pygments-style-native .err {
-  color: #a61717;
-  background-color: #e3d2d2;
-} /* Error */
-.pygments-style-native .esc { color: #d0d0d0; } /* Escape */
-.pygments-style-native .g { color: #d0d0d0; } /* Generic */
-.pygments-style-native .k {
-  color: #6ab825;
-  font-weight: bold;
-} /* Keyword */
-.pygments-style-native .l { color: #d0d0d0; } /* Literal */
-.pygments-style-native .n { color: #d0d0d0; } /* Name */
-.pygments-style-native .o { color: #d0d0d0; } /* Operator */
-.pygments-style-native .x { color: #d0d0d0; } /* Other */
-.pygments-style-native .p { color: #d0d0d0; } /* Punctuation */
-.pygments-style-native .ch {
-  color: #999;
-  font-style: italic;
-} /* Comment.Hashbang */
-.pygments-style-native .cm {
-  color: #999;
-  font-style: italic;
-} /* Comment.Multiline */
-.pygments-style-native .cp {
-  color: #cd2828;
-  font-weight: bold;
-} /* Comment.Preproc */
-.pygments-style-native .cpf {
-  color: #999;
-  font-style: italic;
-} /* Comment.PreprocFile */
-.pygments-style-native .c1 {
-  color: #999;
-  font-style: italic;
-} /* Comment.Single */
-.pygments-style-native .cs {
-  color: #e50808;
-  font-weight: bold;
-  background-color: #520000;
-} /* Comment.Special */
-.pygments-style-native .gd { color: #d22323; } /* Generic.Deleted */
-.pygments-style-native .ge {
-  color: #d0d0d0;
-  font-style: italic;
-} /* Generic.Emph */
-.pygments-style-native .gr { color: #d22323; } /* Generic.Error */
-.pygments-style-native .gh {
-  color: #fff;
-  font-weight: bold;
-} /* Generic.Heading */
-.pygments-style-native .gi { color: #589819; } /* Generic.Inserted */
-.pygments-style-native .go { color: #ccc; } /* Generic.Output */
-.pygments-style-native .gp { color: #aaa; } /* Generic.Prompt */
-.pygments-style-native .gs {
-  color: #d0d0d0;
-  font-weight: bold;
-} /* Generic.Strong */
-.pygments-style-native .gu {
-  color: #fff;
-  text-decoration: underline;
-} /* Generic.Subheading */
-.pygments-style-native .gt { color: #d22323; } /* Generic.Traceback */
-.pygments-style-native .kc {
-  color: #6ab825;
-  font-weight: bold;
-} /* Keyword.Constant */
-.pygments-style-native .kd {
-  color: #6ab825;
-  font-weight: bold;
-} /* Keyword.Declaration */
-.pygments-style-native .kn {
-  color: #6ab825;
-  font-weight: bold;
-} /* Keyword.Namespace */
-.pygments-style-native .kp { color: #6ab825; } /* Keyword.Pseudo */
-.pygments-style-native .kr {
-  color: #6ab825;
-  font-weight: bold;
-} /* Keyword.Reserved */
-.pygments-style-native .kt {
-  color: #6ab825;
-  font-weight: bold;
-} /* Keyword.Type */
-.pygments-style-native .ld { color: #d0d0d0; } /* Literal.Date */
-.pygments-style-native .m { color: #3677a9; } /* Literal.Number */
-.pygments-style-native .s { color: #ed9d13; } /* Literal.String */
-.pygments-style-native .na { color: #bbb; } /* Name.Attribute */
-.pygments-style-native .nb { color: #24909d; } /* Name.Builtin */
-.pygments-style-native .nc {
-  color: #447fcf;
-  text-decoration: underline;
-} /* Name.Class */
-.pygments-style-native .no { color: #40ffff; } /* Name.Constant */
-.pygments-style-native .nd { color: #ffa500; } /* Name.Decorator */
-.pygments-style-native .ni { color: #d0d0d0; } /* Name.Entity */
-.pygments-style-native .ne { color: #bbb; } /* Name.Exception */
-.pygments-style-native .nf { color: #447fcf; } /* Name.Function */
-.pygments-style-native .nl { color: #d0d0d0; } /* Name.Label */
-.pygments-style-native .nn {
-  color: #447fcf;
-  text-decoration: underline;
-} /* Name.Namespace */
-.pygments-style-native .nx { color: #d0d0d0; } /* Name.Other */
-.pygments-style-native .py { color: #d0d0d0; } /* Name.Property */
-.pygments-style-native .nt {
-  color: #6ab825;
-  font-weight: bold;
-} /* Name.Tag */
-.pygments-style-native .nv { color: #40ffff; } /* Name.Variable */
-.pygments-style-native .ow {
-  color: #6ab825;
-  font-weight: bold;
-} /* Operator.Word */
-.pygments-style-native .w { color: #666; } /* Text.Whitespace */
-.pygments-style-native .mb { color: #3677a9; } /* Literal.Number.Bin */
-.pygments-style-native .mf { color: #3677a9; } /* Literal.Number.Float */
-.pygments-style-native .mh { color: #3677a9; } /* Literal.Number.Hex */
-.pygments-style-native .mi { color: #3677a9; } /* Literal.Number.Integer */
-.pygments-style-native .mo { color: #3677a9; } /* Literal.Number.Oct */
-.pygments-style-native .sa { color: #ed9d13; } /* Literal.String.Affix */
-.pygments-style-native .sb { color: #ed9d13; } /* Literal.String.Backtick */
-.pygments-style-native .sc { color: #ed9d13; } /* Literal.String.Char */
-.pygments-style-native .dl { color: #ed9d13; } /* Literal.String.Delimiter */
-.pygments-style-native .sd { color: #ed9d13; } /* Literal.String.Doc */
-.pygments-style-native .s2 { color: #ed9d13; } /* Literal.String.Double */
-.pygments-style-native .se { color: #ed9d13; } /* Literal.String.Escape */
-.pygments-style-native .sh { color: #ed9d13; } /* Literal.String.Heredoc */
-.pygments-style-native .si { color: #ed9d13; } /* Literal.String.Interpol */
-.pygments-style-native .sx { color: #ffa500; } /* Literal.String.Other */
-.pygments-style-native .sr { color: #ed9d13; } /* Literal.String.Regex */
-.pygments-style-native .s1 { color: #ed9d13; } /* Literal.String.Single */
-.pygments-style-native .ss { color: #ed9d13; } /* Literal.String.Symbol */
-.pygments-style-native .bp { color: #24909d; } /* Name.Builtin.Pseudo */
-.pygments-style-native .fm { color: #447fcf; } /* Name.Function.Magic */
-.pygments-style-native .vc { color: #40ffff; } /* Name.Variable.Class */
-.pygments-style-native .vg { color: #40ffff; } /* Name.Variable.Global */
-.pygments-style-native .vi { color: #40ffff; } /* Name.Variable.Instance */
-.pygments-style-native .vm { color: #40ffff; } /* Name.Variable.Magic */
-.pygments-style-native .il { color: #3677a9; } /* Literal.Number.Integer.Long */
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+.pygments-style-paraiso-dark .hll { background-color: #4f424c }
+
+.pygments-style-paraiso-dark { background: #2f1e2e; 
+color: #e7e9db }
+.pygments-style-paraiso-dark .c { color: #776e71 } /* Comment */
+.pygments-style-paraiso-dark .err { color: #ef6155 } /* Error */
+.pygments-style-paraiso-dark .k { color: #815ba4 } /* Keyword */
+.pygments-style-paraiso-dark .l { color: #f99b15 } /* Literal */
+.pygments-style-paraiso-dark .n { color: #e7e9db } /* Name */
+.pygments-style-paraiso-dark .o { color: #5bc4bf } /* Operator */
+.pygments-style-paraiso-dark .p { color: #e7e9db } /* Punctuation */
+.pygments-style-paraiso-dark .ch { color: #776e71 } /* Comment.Hashbang */
+.pygments-style-paraiso-dark .cm { color: #776e71 } /* Comment.Multiline */
+.pygments-style-paraiso-dark .cp { color: #776e71 } /* Comment.Preproc */
+.pygments-style-paraiso-dark .cpf { color: #776e71 } /* Comment.PreprocFile */
+.pygments-style-paraiso-dark .c1 { color: #776e71 } /* Comment.Single */
+.pygments-style-paraiso-dark .cs { color: #776e71 } /* Comment.Special */
+.pygments-style-paraiso-dark .gd { color: #ef6155 } /* Generic.Deleted */
+.pygments-style-paraiso-dark .ge { font-style: italic } /* Generic.Emph */
+.pygments-style-paraiso-dark .ges { font-weight: bold; 
+font-style: italic } /* Generic.EmphStrong */
+.pygments-style-paraiso-dark .gh { color: #e7e9db; 
+font-weight: bold } /* Generic.Heading */
+.pygments-style-paraiso-dark .gi { color: #48b685 } /* Generic.Inserted */
+.pygments-style-paraiso-dark .gp { color: #776e71; 
+font-weight: bold } /* Generic.Prompt */
+.pygments-style-paraiso-dark .gs { font-weight: bold } /* Generic.Strong */
+.pygments-style-paraiso-dark .gu { color: #5bc4bf; 
+font-weight: bold } /* Generic.Subheading */
+.pygments-style-paraiso-dark .kc { color: #815ba4 } /* Keyword.Constant */
+.pygments-style-paraiso-dark .kd { color: #815ba4 } /* Keyword.Declaration */
+.pygments-style-paraiso-dark .kn { color: #5bc4bf } /* Keyword.Namespace */
+.pygments-style-paraiso-dark .kp { color: #815ba4 } /* Keyword.Pseudo */
+.pygments-style-paraiso-dark .kr { color: #815ba4 } /* Keyword.Reserved */
+.pygments-style-paraiso-dark .kt { color: #fec418 } /* Keyword.Type */
+.pygments-style-paraiso-dark .ld { color: #48b685 } /* Literal.Date */
+.pygments-style-paraiso-dark .m { color: #f99b15 } /* Literal.Number */
+.pygments-style-paraiso-dark .s { color: #48b685 } /* Literal.String */
+.pygments-style-paraiso-dark .na { color: #06b6ef } /* Name.Attribute */
+.pygments-style-paraiso-dark .nb { color: #e7e9db } /* Name.Builtin */
+.pygments-style-paraiso-dark .nc { color: #fec418 } /* Name.Class */
+.pygments-style-paraiso-dark .no { color: #ef6155 } /* Name.Constant */
+.pygments-style-paraiso-dark .nd { color: #5bc4bf } /* Name.Decorator */
+.pygments-style-paraiso-dark .ni { color: #e7e9db } /* Name.Entity */
+.pygments-style-paraiso-dark .ne { color: #ef6155 } /* Name.Exception */
+.pygments-style-paraiso-dark .nf { color: #06b6ef } /* Name.Function */
+.pygments-style-paraiso-dark .nl { color: #e7e9db } /* Name.Label */
+.pygments-style-paraiso-dark .nn { color: #fec418 } /* Name.Namespace */
+.pygments-style-paraiso-dark .nx { color: #06b6ef } /* Name.Other */
+.pygments-style-paraiso-dark .py { color: #e7e9db } /* Name.Property */
+.pygments-style-paraiso-dark .nt { color: #5bc4bf } /* Name.Tag */
+.pygments-style-paraiso-dark .nv { color: #ef6155 } /* Name.Variable */
+.pygments-style-paraiso-dark .ow { color: #5bc4bf } /* Operator.Word */
+.pygments-style-paraiso-dark .pm { color: #e7e9db } /* Punctuation.Marker */
+.pygments-style-paraiso-dark .w { color: #e7e9db } /* Text.Whitespace */
+.pygments-style-paraiso-dark .mb { color: #f99b15 } /* Literal.Number.Bin */
+.pygments-style-paraiso-dark .mf { color: #f99b15 } /* Literal.Number.Float */
+.pygments-style-paraiso-dark .mh { color: #f99b15 } /* Literal.Number.Hex */
+.pygments-style-paraiso-dark .mi { color: #f99b15 } /* Literal.Number.Integer */
+.pygments-style-paraiso-dark .mo { color: #f99b15 } /* Literal.Number.Oct */
+.pygments-style-paraiso-dark .sa { color: #48b685 } /* Literal.String.Affix */
+.pygments-style-paraiso-dark .sb { color: #48b685 } /* Literal.String.Backtick */
+.pygments-style-paraiso-dark .sc { color: #e7e9db } /* Literal.String.Char */
+.pygments-style-paraiso-dark .dl { color: #48b685 } /* Literal.String.Delimiter */
+.pygments-style-paraiso-dark .sd { color: #776e71 } /* Literal.String.Doc */
+.pygments-style-paraiso-dark .s2 { color: #48b685 } /* Literal.String.Double */
+.pygments-style-paraiso-dark .se { color: #f99b15 } /* Literal.String.Escape */
+.pygments-style-paraiso-dark .sh { color: #48b685 } /* Literal.String.Heredoc */
+.pygments-style-paraiso-dark .si { color: #f99b15 } /* Literal.String.Interpol */
+.pygments-style-paraiso-dark .sx { color: #48b685 } /* Literal.String.Other */
+.pygments-style-paraiso-dark .sr { color: #48b685 } /* Literal.String.Regex */
+.pygments-style-paraiso-dark .s1 { color: #48b685 } /* Literal.String.Single */
+.pygments-style-paraiso-dark .ss { color: #48b685 } /* Literal.String.Symbol */
+.pygments-style-paraiso-dark .bp { color: #e7e9db } /* Name.Builtin.Pseudo */
+.pygments-style-paraiso-dark .fm { color: #06b6ef } /* Name.Function.Magic */
+.pygments-style-paraiso-dark .vc { color: #ef6155 } /* Name.Variable.Class */
+.pygments-style-paraiso-dark .vg { color: #ef6155 } /* Name.Variable.Global */
+.pygments-style-paraiso-dark .vi { color: #ef6155 } /* Name.Variable.Instance */
+.pygments-style-paraiso-dark .vm { color: #ef6155 } /* Name.Variable.Magic */
+.pygments-style-paraiso-dark .il { color: #f99b15 } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/paraiso-dark.css` & `plumage-4.0.0/plumage/static/css/pygments/perldoc.css`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,112 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
-.pygments-style-paraiso-dark .hll { background-color: #4f424c; }
+.pygments-style-perldoc .hll { background-color: #ffc }
 
-.pygments-style-paraiso-dark {
-  background: #2f1e2e;
-  color: #e7e9db;
-}
-.pygments-style-paraiso-dark .c { color: #776e71; } /* Comment */
-.pygments-style-paraiso-dark .err { color: #ef6155; } /* Error */
-.pygments-style-paraiso-dark .k { color: #815ba4; } /* Keyword */
-.pygments-style-paraiso-dark .l { color: #f99b15; } /* Literal */
-.pygments-style-paraiso-dark .n { color: #e7e9db; } /* Name */
-.pygments-style-paraiso-dark .o { color: #5bc4bf; } /* Operator */
-.pygments-style-paraiso-dark .p { color: #e7e9db; } /* Punctuation */
-.pygments-style-paraiso-dark .ch { color: #776e71; } /* Comment.Hashbang */
-.pygments-style-paraiso-dark .cm { color: #776e71; } /* Comment.Multiline */
-.pygments-style-paraiso-dark .cp { color: #776e71; } /* Comment.Preproc */
-.pygments-style-paraiso-dark .cpf { color: #776e71; } /* Comment.PreprocFile */
-.pygments-style-paraiso-dark .c1 { color: #776e71; } /* Comment.Single */
-.pygments-style-paraiso-dark .cs { color: #776e71; } /* Comment.Special */
-.pygments-style-paraiso-dark .gd { color: #ef6155; } /* Generic.Deleted */
-.pygments-style-paraiso-dark .ge { font-style: italic; } /* Generic.Emph */
-.pygments-style-paraiso-dark .gh {
-  color: #e7e9db;
-  font-weight: bold;
-} /* Generic.Heading */
-.pygments-style-paraiso-dark .gi { color: #48b685; } /* Generic.Inserted */
-.pygments-style-paraiso-dark .gp {
-  color: #776e71;
-  font-weight: bold;
-} /* Generic.Prompt */
-.pygments-style-paraiso-dark .gs { font-weight: bold; } /* Generic.Strong */
-.pygments-style-paraiso-dark .gu {
-  color: #5bc4bf;
-  font-weight: bold;
-} /* Generic.Subheading */
-.pygments-style-paraiso-dark .kc { color: #815ba4; } /* Keyword.Constant */
-.pygments-style-paraiso-dark .kd { color: #815ba4; } /* Keyword.Declaration */
-.pygments-style-paraiso-dark .kn { color: #5bc4bf; } /* Keyword.Namespace */
-.pygments-style-paraiso-dark .kp { color: #815ba4; } /* Keyword.Pseudo */
-.pygments-style-paraiso-dark .kr { color: #815ba4; } /* Keyword.Reserved */
-.pygments-style-paraiso-dark .kt { color: #fec418; } /* Keyword.Type */
-.pygments-style-paraiso-dark .ld { color: #48b685; } /* Literal.Date */
-.pygments-style-paraiso-dark .m { color: #f99b15; } /* Literal.Number */
-.pygments-style-paraiso-dark .s { color: #48b685; } /* Literal.String */
-.pygments-style-paraiso-dark .na { color: #06b6ef; } /* Name.Attribute */
-.pygments-style-paraiso-dark .nb { color: #e7e9db; } /* Name.Builtin */
-.pygments-style-paraiso-dark .nc { color: #fec418; } /* Name.Class */
-.pygments-style-paraiso-dark .no { color: #ef6155; } /* Name.Constant */
-.pygments-style-paraiso-dark .nd { color: #5bc4bf; } /* Name.Decorator */
-.pygments-style-paraiso-dark .ni { color: #e7e9db; } /* Name.Entity */
-.pygments-style-paraiso-dark .ne { color: #ef6155; } /* Name.Exception */
-.pygments-style-paraiso-dark .nf { color: #06b6ef; } /* Name.Function */
-.pygments-style-paraiso-dark .nl { color: #e7e9db; } /* Name.Label */
-.pygments-style-paraiso-dark .nn { color: #fec418; } /* Name.Namespace */
-.pygments-style-paraiso-dark .nx { color: #06b6ef; } /* Name.Other */
-.pygments-style-paraiso-dark .py { color: #e7e9db; } /* Name.Property */
-.pygments-style-paraiso-dark .nt { color: #5bc4bf; } /* Name.Tag */
-.pygments-style-paraiso-dark .nv { color: #ef6155; } /* Name.Variable */
-.pygments-style-paraiso-dark .ow { color: #5bc4bf; } /* Operator.Word */
-.pygments-style-paraiso-dark .w { color: #e7e9db; } /* Text.Whitespace */
-.pygments-style-paraiso-dark .mb { color: #f99b15; } /* Literal.Number.Bin */
-.pygments-style-paraiso-dark .mf { color: #f99b15; } /* Literal.Number.Float */
-.pygments-style-paraiso-dark .mh { color: #f99b15; } /* Literal.Number.Hex */
-.pygments-style-paraiso-dark .mi { color: #f99b15; } /* Literal.Number.Integer */
-.pygments-style-paraiso-dark .mo { color: #f99b15; } /* Literal.Number.Oct */
-.pygments-style-paraiso-dark .sa { color: #48b685; } /* Literal.String.Affix */
-.pygments-style-paraiso-dark .sb { color: #48b685; } /* Literal.String.Backtick */
-.pygments-style-paraiso-dark .sc { color: #e7e9db; } /* Literal.String.Char */
-.pygments-style-paraiso-dark .dl { color: #48b685; } /* Literal.String.Delimiter */
-.pygments-style-paraiso-dark .sd { color: #776e71; } /* Literal.String.Doc */
-.pygments-style-paraiso-dark .s2 { color: #48b685; } /* Literal.String.Double */
-.pygments-style-paraiso-dark .se { color: #f99b15; } /* Literal.String.Escape */
-.pygments-style-paraiso-dark .sh { color: #48b685; } /* Literal.String.Heredoc */
-.pygments-style-paraiso-dark .si { color: #f99b15; } /* Literal.String.Interpol */
-.pygments-style-paraiso-dark .sx { color: #48b685; } /* Literal.String.Other */
-.pygments-style-paraiso-dark .sr { color: #48b685; } /* Literal.String.Regex */
-.pygments-style-paraiso-dark .s1 { color: #48b685; } /* Literal.String.Single */
-.pygments-style-paraiso-dark .ss { color: #48b685; } /* Literal.String.Symbol */
-.pygments-style-paraiso-dark .bp { color: #e7e9db; } /* Name.Builtin.Pseudo */
-.pygments-style-paraiso-dark .fm { color: #06b6ef; } /* Name.Function.Magic */
-.pygments-style-paraiso-dark .vc { color: #ef6155; } /* Name.Variable.Class */
-.pygments-style-paraiso-dark .vg { color: #ef6155; } /* Name.Variable.Global */
-.pygments-style-paraiso-dark .vi { color: #ef6155; } /* Name.Variable.Instance */
-.pygments-style-paraiso-dark .vm { color: #ef6155; } /* Name.Variable.Magic */
-.pygments-style-paraiso-dark .il { color: #f99b15; } /* Literal.Number.Integer.Long */
+.pygments-style-perldoc { background: #eed; 
+}
+.pygments-style-perldoc .c { color: #228B22 } /* Comment */
+.pygments-style-perldoc .err { color: #a61717; 
+background-color: #e3d2d2 } /* Error */
+.pygments-style-perldoc .k { color: #8B008B; 
+font-weight: bold } /* Keyword */
+.pygments-style-perldoc .ch { color: #228B22 } /* Comment.Hashbang */
+.pygments-style-perldoc .cm { color: #228B22 } /* Comment.Multiline */
+.pygments-style-perldoc .cp { color: #1e889b } /* Comment.Preproc */
+.pygments-style-perldoc .cpf { color: #228B22 } /* Comment.PreprocFile */
+.pygments-style-perldoc .c1 { color: #228B22 } /* Comment.Single */
+.pygments-style-perldoc .cs { color: #8B008B; 
+font-weight: bold } /* Comment.Special */
+.pygments-style-perldoc .gd { color: #a00 } /* Generic.Deleted */
+.pygments-style-perldoc .ge { font-style: italic } /* Generic.Emph */
+.pygments-style-perldoc .ges { font-weight: bold; 
+font-style: italic } /* Generic.EmphStrong */
+.pygments-style-perldoc .gr { color: #a00 } /* Generic.Error */
+.pygments-style-perldoc .gh { color: #000080; 
+font-weight: bold } /* Generic.Heading */
+.pygments-style-perldoc .gi { color: #0a0 } /* Generic.Inserted */
+.pygments-style-perldoc .go { color: #888 } /* Generic.Output */
+.pygments-style-perldoc .gp { color: #555 } /* Generic.Prompt */
+.pygments-style-perldoc .gs { font-weight: bold } /* Generic.Strong */
+.pygments-style-perldoc .gu { color: #800080; 
+font-weight: bold } /* Generic.Subheading */
+.pygments-style-perldoc .gt { color: #a00 } /* Generic.Traceback */
+.pygments-style-perldoc .kc { color: #8B008B; 
+font-weight: bold } /* Keyword.Constant */
+.pygments-style-perldoc .kd { color: #8B008B; 
+font-weight: bold } /* Keyword.Declaration */
+.pygments-style-perldoc .kn { color: #8B008B; 
+font-weight: bold } /* Keyword.Namespace */
+.pygments-style-perldoc .kp { color: #8B008B; 
+font-weight: bold } /* Keyword.Pseudo */
+.pygments-style-perldoc .kr { color: #8B008B; 
+font-weight: bold } /* Keyword.Reserved */
+.pygments-style-perldoc .kt { color: #00688B; 
+font-weight: bold } /* Keyword.Type */
+.pygments-style-perldoc .m { color: #B452CD } /* Literal.Number */
+.pygments-style-perldoc .s { color: #CD5555 } /* Literal.String */
+.pygments-style-perldoc .na { color: #658b00 } /* Name.Attribute */
+.pygments-style-perldoc .nb { color: #658b00 } /* Name.Builtin */
+.pygments-style-perldoc .nc { color: #008b45; 
+font-weight: bold } /* Name.Class */
+.pygments-style-perldoc .no { color: #00688B } /* Name.Constant */
+.pygments-style-perldoc .nd { color: #707a7c } /* Name.Decorator */
+.pygments-style-perldoc .ne { color: #008b45; 
+font-weight: bold } /* Name.Exception */
+.pygments-style-perldoc .nf { color: #008b45 } /* Name.Function */
+.pygments-style-perldoc .nn { color: #008b45; 
+text-decoration: underline } /* Name.Namespace */
+.pygments-style-perldoc .nt { color: #8B008B; 
+font-weight: bold } /* Name.Tag */
+.pygments-style-perldoc .nv { color: #00688B } /* Name.Variable */
+.pygments-style-perldoc .ow { color: #8B008B } /* Operator.Word */
+.pygments-style-perldoc .w { color: #bbb } /* Text.Whitespace */
+.pygments-style-perldoc .mb { color: #B452CD } /* Literal.Number.Bin */
+.pygments-style-perldoc .mf { color: #B452CD } /* Literal.Number.Float */
+.pygments-style-perldoc .mh { color: #B452CD } /* Literal.Number.Hex */
+.pygments-style-perldoc .mi { color: #B452CD } /* Literal.Number.Integer */
+.pygments-style-perldoc .mo { color: #B452CD } /* Literal.Number.Oct */
+.pygments-style-perldoc .sa { color: #CD5555 } /* Literal.String.Affix */
+.pygments-style-perldoc .sb { color: #CD5555 } /* Literal.String.Backtick */
+.pygments-style-perldoc .sc { color: #CD5555 } /* Literal.String.Char */
+.pygments-style-perldoc .dl { color: #CD5555 } /* Literal.String.Delimiter */
+.pygments-style-perldoc .sd { color: #CD5555 } /* Literal.String.Doc */
+.pygments-style-perldoc .s2 { color: #CD5555 } /* Literal.String.Double */
+.pygments-style-perldoc .se { color: #CD5555 } /* Literal.String.Escape */
+.pygments-style-perldoc .sh { color: #1c7e71; 
+font-style: italic } /* Literal.String.Heredoc */
+.pygments-style-perldoc .si { color: #CD5555 } /* Literal.String.Interpol */
+.pygments-style-perldoc .sx { color: #cb6c20 } /* Literal.String.Other */
+.pygments-style-perldoc .sr { color: #1c7e71 } /* Literal.String.Regex */
+.pygments-style-perldoc .s1 { color: #CD5555 } /* Literal.String.Single */
+.pygments-style-perldoc .ss { color: #CD5555 } /* Literal.String.Symbol */
+.pygments-style-perldoc .bp { color: #658b00 } /* Name.Builtin.Pseudo */
+.pygments-style-perldoc .fm { color: #008b45 } /* Name.Function.Magic */
+.pygments-style-perldoc .vc { color: #00688B } /* Name.Variable.Class */
+.pygments-style-perldoc .vg { color: #00688B } /* Name.Variable.Global */
+.pygments-style-perldoc .vi { color: #00688B } /* Name.Variable.Instance */
+.pygments-style-perldoc .vm { color: #00688B } /* Name.Variable.Magic */
+.pygments-style-perldoc .il { color: #B452CD } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/pastie.css` & `plumage-4.0.0/plumage/static/css/pygments/rainbow_dash.css`

 * *Files 27% similar despite different names*

```diff
@@ -1,226 +1,132 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
-.pygments-style-pastie .hll { background-color: #ffc; }
+.pygments-style-rainbow_dash .hll { background-color: #ffc }
 
-.pygments-style-pastie {
-  background: #fff;
-}
-.pygments-style-pastie .c { color: #888; } /* Comment */
-.pygments-style-pastie .err {
-  color: #a61717;
-  background-color: #e3d2d2;
-} /* Error */
-.pygments-style-pastie .k {
-  color: #080;
-  font-weight: bold;
-} /* Keyword */
-.pygments-style-pastie .ch { color: #888; } /* Comment.Hashbang */
-.pygments-style-pastie .cm { color: #888; } /* Comment.Multiline */
-.pygments-style-pastie .cp {
-  color: #c00;
-  font-weight: bold;
-} /* Comment.Preproc */
-.pygments-style-pastie .cpf { color: #888; } /* Comment.PreprocFile */
-.pygments-style-pastie .c1 { color: #888; } /* Comment.Single */
-.pygments-style-pastie .cs {
-  color: #c00;
-  font-weight: bold;
-  background-color: #fff0f0;
-} /* Comment.Special */
-.pygments-style-pastie .gd {
-  color: #000;
-  background-color: #fdd;
-} /* Generic.Deleted */
-.pygments-style-pastie .ge { font-style: italic; } /* Generic.Emph */
-.pygments-style-pastie .gr { color: #a00; } /* Generic.Error */
-.pygments-style-pastie .gh { color: #333; } /* Generic.Heading */
-.pygments-style-pastie .gi {
-  color: #000;
-  background-color: #dfd;
-} /* Generic.Inserted */
-.pygments-style-pastie .go { color: #888; } /* Generic.Output */
-.pygments-style-pastie .gp { color: #555; } /* Generic.Prompt */
-.pygments-style-pastie .gs { font-weight: bold; } /* Generic.Strong */
-.pygments-style-pastie .gu { color: #666; } /* Generic.Subheading */
-.pygments-style-pastie .gt { color: #a00; } /* Generic.Traceback */
-.pygments-style-pastie .kc {
-  color: #080;
-  font-weight: bold;
-} /* Keyword.Constant */
-.pygments-style-pastie .kd {
-  color: #080;
-  font-weight: bold;
-} /* Keyword.Declaration */
-.pygments-style-pastie .kn {
-  color: #080;
-  font-weight: bold;
-} /* Keyword.Namespace */
-.pygments-style-pastie .kp { color: #080; } /* Keyword.Pseudo */
-.pygments-style-pastie .kr {
-  color: #080;
-  font-weight: bold;
-} /* Keyword.Reserved */
-.pygments-style-pastie .kt {
-  color: #888;
-  font-weight: bold;
-} /* Keyword.Type */
-.pygments-style-pastie .m {
-  color: #00d;
-  font-weight: bold;
-} /* Literal.Number */
-.pygments-style-pastie .s {
-  color: #d20;
-  background-color: #fff0f0;
-} /* Literal.String */
-.pygments-style-pastie .na { color: #369; } /* Name.Attribute */
-.pygments-style-pastie .nb { color: #038; } /* Name.Builtin */
-.pygments-style-pastie .nc {
-  color: #b06;
-  font-weight: bold;
-} /* Name.Class */
-.pygments-style-pastie .no {
-  color: #036;
-  font-weight: bold;
-} /* Name.Constant */
-.pygments-style-pastie .nd { color: #555; } /* Name.Decorator */
-.pygments-style-pastie .ne {
-  color: #b06;
-  font-weight: bold;
-} /* Name.Exception */
-.pygments-style-pastie .nf {
-  color: #06b;
-  font-weight: bold;
-} /* Name.Function */
-.pygments-style-pastie .nl {
-  color: #369;
-  font-style: italic;
-} /* Name.Label */
-.pygments-style-pastie .nn {
-  color: #b06;
-  font-weight: bold;
-} /* Name.Namespace */
-.pygments-style-pastie .py {
-  color: #369;
-  font-weight: bold;
-} /* Name.Property */
-.pygments-style-pastie .nt {
-  color: #b06;
-  font-weight: bold;
-} /* Name.Tag */
-.pygments-style-pastie .nv { color: #369; } /* Name.Variable */
-.pygments-style-pastie .ow { color: #080; } /* Operator.Word */
-.pygments-style-pastie .w { color: #bbb; } /* Text.Whitespace */
-.pygments-style-pastie .mb {
-  color: #00d;
-  font-weight: bold;
-} /* Literal.Number.Bin */
-.pygments-style-pastie .mf {
-  color: #00d;
-  font-weight: bold;
-} /* Literal.Number.Float */
-.pygments-style-pastie .mh {
-  color: #00d;
-  font-weight: bold;
-} /* Literal.Number.Hex */
-.pygments-style-pastie .mi {
-  color: #00d;
-  font-weight: bold;
-} /* Literal.Number.Integer */
-.pygments-style-pastie .mo {
-  color: #00d;
-  font-weight: bold;
-} /* Literal.Number.Oct */
-.pygments-style-pastie .sa {
-  color: #d20;
-  background-color: #fff0f0;
-} /* Literal.String.Affix */
-.pygments-style-pastie .sb {
-  color: #d20;
-  background-color: #fff0f0;
-} /* Literal.String.Backtick */
-.pygments-style-pastie .sc {
-  color: #d20;
-  background-color: #fff0f0;
-} /* Literal.String.Char */
-.pygments-style-pastie .dl {
-  color: #d20;
-  background-color: #fff0f0;
-} /* Literal.String.Delimiter */
-.pygments-style-pastie .sd {
-  color: #d20;
-  background-color: #fff0f0;
-} /* Literal.String.Doc */
-.pygments-style-pastie .s2 {
-  color: #d20;
-  background-color: #fff0f0;
-} /* Literal.String.Double */
-.pygments-style-pastie .se {
-  color: #04d;
-  background-color: #fff0f0;
-} /* Literal.String.Escape */
-.pygments-style-pastie .sh {
-  color: #d20;
-  background-color: #fff0f0;
-} /* Literal.String.Heredoc */
-.pygments-style-pastie .si {
-  color: #33b;
-  background-color: #fff0f0;
-} /* Literal.String.Interpol */
-.pygments-style-pastie .sx {
-  color: #2b2;
-  background-color: #f0fff0;
-} /* Literal.String.Other */
-.pygments-style-pastie .sr {
-  color: #080;
-  background-color: #fff0ff;
-} /* Literal.String.Regex */
-.pygments-style-pastie .s1 {
-  color: #d20;
-  background-color: #fff0f0;
-} /* Literal.String.Single */
-.pygments-style-pastie .ss {
-  color: #a60;
-  background-color: #fff0f0;
-} /* Literal.String.Symbol */
-.pygments-style-pastie .bp { color: #038; } /* Name.Builtin.Pseudo */
-.pygments-style-pastie .fm {
-  color: #06b;
-  font-weight: bold;
-} /* Name.Function.Magic */
-.pygments-style-pastie .vc { color: #369; } /* Name.Variable.Class */
-.pygments-style-pastie .vg { color: #d70; } /* Name.Variable.Global */
-.pygments-style-pastie .vi { color: #33b; } /* Name.Variable.Instance */
-.pygments-style-pastie .vm { color: #369; } /* Name.Variable.Magic */
-.pygments-style-pastie .il {
-  color: #00d;
-  font-weight: bold;
-} /* Literal.Number.Integer.Long */
+.pygments-style-rainbow_dash { background: #fff; 
+color: #4d4d4d }
+
+.pygments-style-rainbow_dash .c { color: #0080ff; 
+font-style: italic } /* Comment */
+.pygments-style-rainbow_dash .err { color: #fff; 
+background-color: #c00 } /* Error */
+.pygments-style-rainbow_dash .k { color: #2c5dcd; 
+font-weight: bold } /* Keyword */
+.pygments-style-rainbow_dash .o { color: #2c5dcd } /* Operator */
+.pygments-style-rainbow_dash .ch { color: #0080ff; 
+font-style: italic } /* Comment.Hashbang */
+.pygments-style-rainbow_dash .cm { color: #0080ff; 
+font-style: italic } /* Comment.Multiline */
+.pygments-style-rainbow_dash .cp { color: #0080ff } /* Comment.Preproc */
+.pygments-style-rainbow_dash .cpf { color: #0080ff; 
+font-style: italic } /* Comment.PreprocFile */
+.pygments-style-rainbow_dash .c1 { color: #0080ff; 
+font-style: italic } /* Comment.Single */
+.pygments-style-rainbow_dash .cs { color: #0080ff; 
+font-weight: bold; 
+font-style: italic } /* Comment.Special */
+.pygments-style-rainbow_dash .gd { background-color: #fcc; 
+border: 1px solid #c5060b } /* Generic.Deleted */
+.pygments-style-rainbow_dash .ge { font-style: italic } /* Generic.Emph */
+.pygments-style-rainbow_dash .ges { font-weight: bold; 
+font-style: italic } /* Generic.EmphStrong */
+.pygments-style-rainbow_dash .gr { color: #f00 } /* Generic.Error */
+.pygments-style-rainbow_dash .gh { color: #2c5dcd; 
+font-weight: bold } /* Generic.Heading */
+.pygments-style-rainbow_dash .gi { background-color: #cfc; 
+border: 1px solid #0c0 } /* Generic.Inserted */
+.pygments-style-rainbow_dash .go { color: #aaa } /* Generic.Output */
+.pygments-style-rainbow_dash .gp { color: #2c5dcd; 
+font-weight: bold } /* Generic.Prompt */
+.pygments-style-rainbow_dash .gs { font-weight: bold } /* Generic.Strong */
+.pygments-style-rainbow_dash .gu { color: #2c5dcd; 
+font-weight: bold } /* Generic.Subheading */
+.pygments-style-rainbow_dash .gt { color: #c5060b } /* Generic.Traceback */
+.pygments-style-rainbow_dash .kc { color: #2c5dcd; 
+font-weight: bold } /* Keyword.Constant */
+.pygments-style-rainbow_dash .kd { color: #2c5dcd; 
+font-weight: bold } /* Keyword.Declaration */
+.pygments-style-rainbow_dash .kn { color: #2c5dcd; 
+font-weight: bold } /* Keyword.Namespace */
+.pygments-style-rainbow_dash .kp { color: #2c5dcd } /* Keyword.Pseudo */
+.pygments-style-rainbow_dash .kr { color: #2c5dcd; 
+font-weight: bold } /* Keyword.Reserved */
+.pygments-style-rainbow_dash .kt { color: #5918bb; 
+font-weight: bold } /* Keyword.Type */
+.pygments-style-rainbow_dash .m { color: #5918bb; 
+font-weight: bold } /* Literal.Number */
+.pygments-style-rainbow_dash .s { color: #0c6 } /* Literal.String */
+.pygments-style-rainbow_dash .na { color: #2c5dcd; 
+font-style: italic } /* Name.Attribute */
+.pygments-style-rainbow_dash .nb { color: #5918bb; 
+font-weight: bold } /* Name.Builtin */
+.pygments-style-rainbow_dash .nc { text-decoration: underline } /* Name.Class */
+.pygments-style-rainbow_dash .no { color: #318495 } /* Name.Constant */
+.pygments-style-rainbow_dash .nd { color: #ff8000; 
+font-weight: bold } /* Name.Decorator */
+.pygments-style-rainbow_dash .ni { color: #5918bb; 
+font-weight: bold } /* Name.Entity */
+.pygments-style-rainbow_dash .ne { color: #5918bb; 
+font-weight: bold } /* Name.Exception */
+.pygments-style-rainbow_dash .nf { color: #ff8000; 
+font-weight: bold } /* Name.Function */
+.pygments-style-rainbow_dash .nt { color: #2c5dcd; 
+font-weight: bold } /* Name.Tag */
+.pygments-style-rainbow_dash .ow { color: #2c5dcd; 
+font-weight: bold } /* Operator.Word */
+.pygments-style-rainbow_dash .w { color: #cbcbcb } /* Text.Whitespace */
+.pygments-style-rainbow_dash .mb { color: #5918bb; 
+font-weight: bold } /* Literal.Number.Bin */
+.pygments-style-rainbow_dash .mf { color: #5918bb; 
+font-weight: bold } /* Literal.Number.Float */
+.pygments-style-rainbow_dash .mh { color: #5918bb; 
+font-weight: bold } /* Literal.Number.Hex */
+.pygments-style-rainbow_dash .mi { color: #5918bb; 
+font-weight: bold } /* Literal.Number.Integer */
+.pygments-style-rainbow_dash .mo { color: #5918bb; 
+font-weight: bold } /* Literal.Number.Oct */
+.pygments-style-rainbow_dash .sa { color: #0c6 } /* Literal.String.Affix */
+.pygments-style-rainbow_dash .sb { color: #0c6 } /* Literal.String.Backtick */
+.pygments-style-rainbow_dash .sc { color: #0c6 } /* Literal.String.Char */
+.pygments-style-rainbow_dash .dl { color: #0c6 } /* Literal.String.Delimiter */
+.pygments-style-rainbow_dash .sd { color: #0c6; 
+font-style: italic } /* Literal.String.Doc */
+.pygments-style-rainbow_dash .s2 { color: #0c6 } /* Literal.String.Double */
+.pygments-style-rainbow_dash .se { color: #c5060b; 
+font-weight: bold } /* Literal.String.Escape */
+.pygments-style-rainbow_dash .sh { color: #0c6 } /* Literal.String.Heredoc */
+.pygments-style-rainbow_dash .si { color: #0c6 } /* Literal.String.Interpol */
+.pygments-style-rainbow_dash .sx { color: #318495 } /* Literal.String.Other */
+.pygments-style-rainbow_dash .sr { color: #0c6 } /* Literal.String.Regex */
+.pygments-style-rainbow_dash .s1 { color: #0c6 } /* Literal.String.Single */
+.pygments-style-rainbow_dash .ss { color: #c5060b; 
+font-weight: bold } /* Literal.String.Symbol */
+.pygments-style-rainbow_dash .bp { color: #5918bb; 
+font-weight: bold } /* Name.Builtin.Pseudo */
+.pygments-style-rainbow_dash .fm { color: #ff8000; 
+font-weight: bold } /* Name.Function.Magic */
+.pygments-style-rainbow_dash .il { color: #5918bb; 
+font-weight: bold } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/perldoc.css` & `plumage-4.0.0/plumage/static/css/pygments/sas.css`

 * *Files 25% similar despite different names*

```diff
@@ -1,148 +1,114 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-.pygments-style-perldoc .hll { background-color: #ffc; }
-
-.pygments-style-perldoc {
-  background: #eed;
-}
-.pygments-style-perldoc .c { color: #228b22; } /* Comment */
-.pygments-style-perldoc .err {
-  color: #a61717;
-  background-color: #e3d2d2;
-} /* Error */
-.pygments-style-perldoc .k {
-  color: #8b008b;
-  font-weight: bold;
-} /* Keyword */
-.pygments-style-perldoc .ch { color: #228b22; } /* Comment.Hashbang */
-.pygments-style-perldoc .cm { color: #228b22; } /* Comment.Multiline */
-.pygments-style-perldoc .cp { color: #1e889b; } /* Comment.Preproc */
-.pygments-style-perldoc .cpf { color: #228b22; } /* Comment.PreprocFile */
-.pygments-style-perldoc .c1 { color: #228b22; } /* Comment.Single */
-.pygments-style-perldoc .cs {
-  color: #8b008b;
-  font-weight: bold;
-} /* Comment.Special */
-.pygments-style-perldoc .gd { color: #a00; } /* Generic.Deleted */
-.pygments-style-perldoc .ge { font-style: italic; } /* Generic.Emph */
-.pygments-style-perldoc .gr { color: #a00; } /* Generic.Error */
-.pygments-style-perldoc .gh {
-  color: #000080;
-  font-weight: bold;
-} /* Generic.Heading */
-.pygments-style-perldoc .gi { color: #0a0; } /* Generic.Inserted */
-.pygments-style-perldoc .go { color: #888; } /* Generic.Output */
-.pygments-style-perldoc .gp { color: #555; } /* Generic.Prompt */
-.pygments-style-perldoc .gs { font-weight: bold; } /* Generic.Strong */
-.pygments-style-perldoc .gu {
-  color: #800080;
-  font-weight: bold;
-} /* Generic.Subheading */
-.pygments-style-perldoc .gt { color: #a00; } /* Generic.Traceback */
-.pygments-style-perldoc .kc {
-  color: #8b008b;
-  font-weight: bold;
-} /* Keyword.Constant */
-.pygments-style-perldoc .kd {
-  color: #8b008b;
-  font-weight: bold;
-} /* Keyword.Declaration */
-.pygments-style-perldoc .kn {
-  color: #8b008b;
-  font-weight: bold;
-} /* Keyword.Namespace */
-.pygments-style-perldoc .kp {
-  color: #8b008b;
-  font-weight: bold;
-} /* Keyword.Pseudo */
-.pygments-style-perldoc .kr {
-  color: #8b008b;
-  font-weight: bold;
-} /* Keyword.Reserved */
-.pygments-style-perldoc .kt {
-  color: #00688b;
-  font-weight: bold;
-} /* Keyword.Type */
-.pygments-style-perldoc .m { color: #b452cd; } /* Literal.Number */
-.pygments-style-perldoc .s { color: #cd5555; } /* Literal.String */
-.pygments-style-perldoc .na { color: #658b00; } /* Name.Attribute */
-.pygments-style-perldoc .nb { color: #658b00; } /* Name.Builtin */
-.pygments-style-perldoc .nc {
-  color: #008b45;
-  font-weight: bold;
-} /* Name.Class */
-.pygments-style-perldoc .no { color: #00688b; } /* Name.Constant */
-.pygments-style-perldoc .nd { color: #707a7c; } /* Name.Decorator */
-.pygments-style-perldoc .ne {
-  color: #008b45;
-  font-weight: bold;
-} /* Name.Exception */
-.pygments-style-perldoc .nf { color: #008b45; } /* Name.Function */
-.pygments-style-perldoc .nn {
-  color: #008b45;
-  text-decoration: underline;
-} /* Name.Namespace */
-.pygments-style-perldoc .nt {
-  color: #8b008b;
-  font-weight: bold;
-} /* Name.Tag */
-.pygments-style-perldoc .nv { color: #00688b; } /* Name.Variable */
-.pygments-style-perldoc .ow { color: #8b008b; } /* Operator.Word */
-.pygments-style-perldoc .w { color: #bbb; } /* Text.Whitespace */
-.pygments-style-perldoc .mb { color: #b452cd; } /* Literal.Number.Bin */
-.pygments-style-perldoc .mf { color: #b452cd; } /* Literal.Number.Float */
-.pygments-style-perldoc .mh { color: #b452cd; } /* Literal.Number.Hex */
-.pygments-style-perldoc .mi { color: #b452cd; } /* Literal.Number.Integer */
-.pygments-style-perldoc .mo { color: #b452cd; } /* Literal.Number.Oct */
-.pygments-style-perldoc .sa { color: #cd5555; } /* Literal.String.Affix */
-.pygments-style-perldoc .sb { color: #cd5555; } /* Literal.String.Backtick */
-.pygments-style-perldoc .sc { color: #cd5555; } /* Literal.String.Char */
-.pygments-style-perldoc .dl { color: #cd5555; } /* Literal.String.Delimiter */
-.pygments-style-perldoc .sd { color: #cd5555; } /* Literal.String.Doc */
-.pygments-style-perldoc .s2 { color: #cd5555; } /* Literal.String.Double */
-.pygments-style-perldoc .se { color: #cd5555; } /* Literal.String.Escape */
-.pygments-style-perldoc .sh {
-  color: #1c7e71;
-  font-style: italic;
-} /* Literal.String.Heredoc */
-.pygments-style-perldoc .si { color: #cd5555; } /* Literal.String.Interpol */
-.pygments-style-perldoc .sx { color: #cb6c20; } /* Literal.String.Other */
-.pygments-style-perldoc .sr { color: #1c7e71; } /* Literal.String.Regex */
-.pygments-style-perldoc .s1 { color: #cd5555; } /* Literal.String.Single */
-.pygments-style-perldoc .ss { color: #cd5555; } /* Literal.String.Symbol */
-.pygments-style-perldoc .bp { color: #658b00; } /* Name.Builtin.Pseudo */
-.pygments-style-perldoc .fm { color: #008b45; } /* Name.Function.Magic */
-.pygments-style-perldoc .vc { color: #00688b; } /* Name.Variable.Class */
-.pygments-style-perldoc .vg { color: #00688b; } /* Name.Variable.Global */
-.pygments-style-perldoc .vi { color: #00688b; } /* Name.Variable.Instance */
-.pygments-style-perldoc .vm { color: #00688b; } /* Name.Variable.Magic */
-.pygments-style-perldoc .il { color: #b452cd; } /* Literal.Number.Integer.Long */
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+.pygments-style-sas .hll { background-color: #ffc }
+
+.pygments-style-sas { background: #fff; 
+}
+
+.pygments-style-sas .c { color: #080; 
+font-style: italic } /* Comment */
+.pygments-style-sas .err { color: #a61717; 
+background-color: #e3d2d2 } /* Error */
+.pygments-style-sas .g { color: #2c2cff } /* Generic */
+.pygments-style-sas .k { color: #2c2cff } /* Keyword */
+.pygments-style-sas .x { background-color: #ffffe0 } /* Other */
+.pygments-style-sas .ch { color: #080; 
+font-style: italic } /* Comment.Hashbang */
+.pygments-style-sas .cm { color: #080; 
+font-style: italic } /* Comment.Multiline */
+.pygments-style-sas .cp { color: #080; 
+font-style: italic } /* Comment.Preproc */
+.pygments-style-sas .cpf { color: #080; 
+font-style: italic } /* Comment.PreprocFile */
+.pygments-style-sas .c1 { color: #080; 
+font-style: italic } /* Comment.Single */
+.pygments-style-sas .cs { color: #080; 
+font-style: italic } /* Comment.Special */
+.pygments-style-sas .gd { color: #2c2cff } /* Generic.Deleted */
+.pygments-style-sas .ge { color: #080 } /* Generic.Emph */
+.pygments-style-sas .ges { color: #2c2cff } /* Generic.EmphStrong */
+.pygments-style-sas .gr { color: #d30202 } /* Generic.Error */
+.pygments-style-sas .gh { color: #2c2cff } /* Generic.Heading */
+.pygments-style-sas .gi { color: #2c2cff } /* Generic.Inserted */
+.pygments-style-sas .go { color: #2c2cff } /* Generic.Output */
+.pygments-style-sas .gp { color: #2c2cff } /* Generic.Prompt */
+.pygments-style-sas .gs { color: #2c2cff } /* Generic.Strong */
+.pygments-style-sas .gu { color: #2c2cff } /* Generic.Subheading */
+.pygments-style-sas .gt { color: #2c2cff } /* Generic.Traceback */
+.pygments-style-sas .kc { color: #2c2cff; 
+font-weight: bold } /* Keyword.Constant */
+.pygments-style-sas .kd { color: #2c2cff } /* Keyword.Declaration */
+.pygments-style-sas .kn { color: #2c2cff } /* Keyword.Namespace */
+.pygments-style-sas .kp { color: #2c2cff } /* Keyword.Pseudo */
+.pygments-style-sas .kr { color: #353580; 
+font-weight: bold } /* Keyword.Reserved */
+.pygments-style-sas .kt { color: #2c2cff } /* Keyword.Type */
+.pygments-style-sas .m { color: #2c8553; 
+font-weight: bold } /* Literal.Number */
+.pygments-style-sas .s { color: #800080 } /* Literal.String */
+.pygments-style-sas .nb { color: #2c2cff } /* Name.Builtin */
+.pygments-style-sas .nf { font-weight: bold; 
+font-style: italic } /* Name.Function */
+.pygments-style-sas .nv { color: #2c2cff; 
+font-weight: bold } /* Name.Variable */
+.pygments-style-sas .w { color: #bbb } /* Text.Whitespace */
+.pygments-style-sas .mb { color: #2c8553; 
+font-weight: bold } /* Literal.Number.Bin */
+.pygments-style-sas .mf { color: #2c8553; 
+font-weight: bold } /* Literal.Number.Float */
+.pygments-style-sas .mh { color: #2c8553; 
+font-weight: bold } /* Literal.Number.Hex */
+.pygments-style-sas .mi { color: #2c8553; 
+font-weight: bold } /* Literal.Number.Integer */
+.pygments-style-sas .mo { color: #2c8553; 
+font-weight: bold } /* Literal.Number.Oct */
+.pygments-style-sas .sa { color: #800080 } /* Literal.String.Affix */
+.pygments-style-sas .sb { color: #800080 } /* Literal.String.Backtick */
+.pygments-style-sas .sc { color: #800080 } /* Literal.String.Char */
+.pygments-style-sas .dl { color: #800080 } /* Literal.String.Delimiter */
+.pygments-style-sas .sd { color: #800080 } /* Literal.String.Doc */
+.pygments-style-sas .s2 { color: #800080 } /* Literal.String.Double */
+.pygments-style-sas .se { color: #800080 } /* Literal.String.Escape */
+.pygments-style-sas .sh { color: #800080 } /* Literal.String.Heredoc */
+.pygments-style-sas .si { color: #800080 } /* Literal.String.Interpol */
+.pygments-style-sas .sx { color: #800080 } /* Literal.String.Other */
+.pygments-style-sas .sr { color: #800080 } /* Literal.String.Regex */
+.pygments-style-sas .s1 { color: #800080 } /* Literal.String.Single */
+.pygments-style-sas .ss { color: #800080 } /* Literal.String.Symbol */
+.pygments-style-sas .bp { color: #2c2cff } /* Name.Builtin.Pseudo */
+.pygments-style-sas .fm { font-weight: bold; 
+font-style: italic } /* Name.Function.Magic */
+.pygments-style-sas .vc { color: #2c2cff; 
+font-weight: bold } /* Name.Variable.Class */
+.pygments-style-sas .vg { color: #2c2cff; 
+font-weight: bold } /* Name.Variable.Global */
+.pygments-style-sas .vi { color: #2c2cff; 
+font-weight: bold } /* Name.Variable.Instance */
+.pygments-style-sas .vm { color: #2c2cff; 
+font-weight: bold } /* Name.Variable.Magic */
+.pygments-style-sas .il { color: #2c8553; 
+font-weight: bold } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/solarized-dark.css` & `plumage-4.0.0/plumage/static/css/pygments/solarized-dark.css`

 * *Files 6% similar despite different names*

```diff
@@ -1,144 +1,122 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #586e75;
-  background-color: #073642;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos {
-  color: #586e75;
-  background-color: #073642;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-.pygments-style-solarized-dark .hll { background-color: #073642; }
-
-.pygments-style-solarized-dark {
-  background: #002b36;
-  color: #839496;
-}
-
-.pygments-style-solarized-dark .c {
-  color: #586e75;
-  font-style: italic;
-} /* Comment */
-.pygments-style-solarized-dark .err {
-  color: #839496;
-  background-color: #dc322f;
-} /* Error */
-.pygments-style-solarized-dark .esc { color: #839496; } /* Escape */
-.pygments-style-solarized-dark .g { color: #839496; } /* Generic */
-.pygments-style-solarized-dark .k { color: #859900; } /* Keyword */
-.pygments-style-solarized-dark .l { color: #839496; } /* Literal */
-.pygments-style-solarized-dark .n { color: #839496; } /* Name */
-.pygments-style-solarized-dark .o { color: #586e75; } /* Operator */
-.pygments-style-solarized-dark .x { color: #839496; } /* Other */
-.pygments-style-solarized-dark .p { color: #839496; } /* Punctuation */
-.pygments-style-solarized-dark .ch {
-  color: #586e75;
-  font-style: italic;
-} /* Comment.Hashbang */
-.pygments-style-solarized-dark .cm {
-  color: #586e75;
-  font-style: italic;
-} /* Comment.Multiline */
-.pygments-style-solarized-dark .cp { color: #d33682; } /* Comment.Preproc */
-.pygments-style-solarized-dark .cpf { color: #586e75; } /* Comment.PreprocFile */
-.pygments-style-solarized-dark .c1 {
-  color: #586e75;
-  font-style: italic;
-} /* Comment.Single */
-.pygments-style-solarized-dark .cs {
-  color: #586e75;
-  font-style: italic;
-} /* Comment.Special */
-.pygments-style-solarized-dark .gd { color: #dc322f; } /* Generic.Deleted */
-.pygments-style-solarized-dark .ge {
-  color: #839496;
-  font-style: italic;
-} /* Generic.Emph */
-.pygments-style-solarized-dark .gr { color: #dc322f; } /* Generic.Error */
-.pygments-style-solarized-dark .gh {
-  color: #839496;
-  font-weight: bold;
-} /* Generic.Heading */
-.pygments-style-solarized-dark .gi { color: #859900; } /* Generic.Inserted */
-.pygments-style-solarized-dark .go { color: #839496; } /* Generic.Output */
-.pygments-style-solarized-dark .gp { color: #839496; } /* Generic.Prompt */
-.pygments-style-solarized-dark .gs {
-  color: #839496;
-  font-weight: bold;
-} /* Generic.Strong */
-.pygments-style-solarized-dark .gu {
-  color: #839496;
-  text-decoration: underline;
-} /* Generic.Subheading */
-.pygments-style-solarized-dark .gt { color: #268bd2; } /* Generic.Traceback */
-.pygments-style-solarized-dark .kc { color: #2aa198; } /* Keyword.Constant */
-.pygments-style-solarized-dark .kd { color: #2aa198; } /* Keyword.Declaration */
-.pygments-style-solarized-dark .kn { color: #cb4b16; } /* Keyword.Namespace */
-.pygments-style-solarized-dark .kp { color: #859900; } /* Keyword.Pseudo */
-.pygments-style-solarized-dark .kr { color: #859900; } /* Keyword.Reserved */
-.pygments-style-solarized-dark .kt { color: #b58900; } /* Keyword.Type */
-.pygments-style-solarized-dark .ld { color: #839496; } /* Literal.Date */
-.pygments-style-solarized-dark .m { color: #2aa198; } /* Literal.Number */
-.pygments-style-solarized-dark .s { color: #2aa198; } /* Literal.String */
-.pygments-style-solarized-dark .na { color: #839496; } /* Name.Attribute */
-.pygments-style-solarized-dark .nb { color: #268bd2; } /* Name.Builtin */
-.pygments-style-solarized-dark .nc { color: #268bd2; } /* Name.Class */
-.pygments-style-solarized-dark .no { color: #268bd2; } /* Name.Constant */
-.pygments-style-solarized-dark .nd { color: #268bd2; } /* Name.Decorator */
-.pygments-style-solarized-dark .ni { color: #268bd2; } /* Name.Entity */
-.pygments-style-solarized-dark .ne { color: #268bd2; } /* Name.Exception */
-.pygments-style-solarized-dark .nf { color: #268bd2; } /* Name.Function */
-.pygments-style-solarized-dark .nl { color: #268bd2; } /* Name.Label */
-.pygments-style-solarized-dark .nn { color: #268bd2; } /* Name.Namespace */
-.pygments-style-solarized-dark .nx { color: #839496; } /* Name.Other */
-.pygments-style-solarized-dark .py { color: #839496; } /* Name.Property */
-.pygments-style-solarized-dark .nt { color: #268bd2; } /* Name.Tag */
-.pygments-style-solarized-dark .nv { color: #268bd2; } /* Name.Variable */
-.pygments-style-solarized-dark .ow { color: #859900; } /* Operator.Word */
-.pygments-style-solarized-dark .w { color: #839496; } /* Text.Whitespace */
-.pygments-style-solarized-dark .mb { color: #2aa198; } /* Literal.Number.Bin */
-.pygments-style-solarized-dark .mf { color: #2aa198; } /* Literal.Number.Float */
-.pygments-style-solarized-dark .mh { color: #2aa198; } /* Literal.Number.Hex */
-.pygments-style-solarized-dark .mi { color: #2aa198; } /* Literal.Number.Integer */
-.pygments-style-solarized-dark .mo { color: #2aa198; } /* Literal.Number.Oct */
-.pygments-style-solarized-dark .sa { color: #2aa198; } /* Literal.String.Affix */
-.pygments-style-solarized-dark .sb { color: #2aa198; } /* Literal.String.Backtick */
-.pygments-style-solarized-dark .sc { color: #2aa198; } /* Literal.String.Char */
-.pygments-style-solarized-dark .dl { color: #2aa198; } /* Literal.String.Delimiter */
-.pygments-style-solarized-dark .sd { color: #586e75; } /* Literal.String.Doc */
-.pygments-style-solarized-dark .s2 { color: #2aa198; } /* Literal.String.Double */
-.pygments-style-solarized-dark .se { color: #2aa198; } /* Literal.String.Escape */
-.pygments-style-solarized-dark .sh { color: #2aa198; } /* Literal.String.Heredoc */
-.pygments-style-solarized-dark .si { color: #2aa198; } /* Literal.String.Interpol */
-.pygments-style-solarized-dark .sx { color: #2aa198; } /* Literal.String.Other */
-.pygments-style-solarized-dark .sr { color: #cb4b16; } /* Literal.String.Regex */
-.pygments-style-solarized-dark .s1 { color: #2aa198; } /* Literal.String.Single */
-.pygments-style-solarized-dark .ss { color: #2aa198; } /* Literal.String.Symbol */
-.pygments-style-solarized-dark .bp { color: #268bd2; } /* Name.Builtin.Pseudo */
-.pygments-style-solarized-dark .fm { color: #268bd2; } /* Name.Function.Magic */
-.pygments-style-solarized-dark .vc { color: #268bd2; } /* Name.Variable.Class */
-.pygments-style-solarized-dark .vg { color: #268bd2; } /* Name.Variable.Global */
-.pygments-style-solarized-dark .vi { color: #268bd2; } /* Name.Variable.Instance */
-.pygments-style-solarized-dark .vm { color: #268bd2; } /* Name.Variable.Magic */
-.pygments-style-solarized-dark .il { color: #2aa198; } /* Literal.Number.Integer.Long */
+td.linenos .normal { color: #586e75; 
+background-color: #073642; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos { color: #586e75; 
+background-color: #073642; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+.pygments-style-solarized-dark .hll { background-color: #073642 }
+
+.pygments-style-solarized-dark { background: #002b36; 
+color: #839496 }
+
+.pygments-style-solarized-dark .c { color: #586e75; 
+font-style: italic } /* Comment */
+.pygments-style-solarized-dark .err { color: #839496; 
+background-color: #dc322f } /* Error */
+.pygments-style-solarized-dark .esc { color: #839496 } /* Escape */
+.pygments-style-solarized-dark .g { color: #839496 } /* Generic */
+.pygments-style-solarized-dark .k { color: #859900 } /* Keyword */
+.pygments-style-solarized-dark .l { color: #839496 } /* Literal */
+.pygments-style-solarized-dark .n { color: #839496 } /* Name */
+.pygments-style-solarized-dark .o { color: #586e75 } /* Operator */
+.pygments-style-solarized-dark .x { color: #839496 } /* Other */
+.pygments-style-solarized-dark .p { color: #839496 } /* Punctuation */
+.pygments-style-solarized-dark .ch { color: #586e75; 
+font-style: italic } /* Comment.Hashbang */
+.pygments-style-solarized-dark .cm { color: #586e75; 
+font-style: italic } /* Comment.Multiline */
+.pygments-style-solarized-dark .cp { color: #d33682 } /* Comment.Preproc */
+.pygments-style-solarized-dark .cpf { color: #586e75 } /* Comment.PreprocFile */
+.pygments-style-solarized-dark .c1 { color: #586e75; 
+font-style: italic } /* Comment.Single */
+.pygments-style-solarized-dark .cs { color: #586e75; 
+font-style: italic } /* Comment.Special */
+.pygments-style-solarized-dark .gd { color: #dc322f } /* Generic.Deleted */
+.pygments-style-solarized-dark .ge { color: #839496; 
+font-style: italic } /* Generic.Emph */
+.pygments-style-solarized-dark .ges { color: #839496; 
+font-weight: bold; 
+font-style: italic } /* Generic.EmphStrong */
+.pygments-style-solarized-dark .gr { color: #dc322f } /* Generic.Error */
+.pygments-style-solarized-dark .gh { color: #839496; 
+font-weight: bold } /* Generic.Heading */
+.pygments-style-solarized-dark .gi { color: #859900 } /* Generic.Inserted */
+.pygments-style-solarized-dark .go { color: #839496 } /* Generic.Output */
+.pygments-style-solarized-dark .gp { color: #268bd2; 
+font-weight: bold } /* Generic.Prompt */
+.pygments-style-solarized-dark .gs { color: #839496; 
+font-weight: bold } /* Generic.Strong */
+.pygments-style-solarized-dark .gu { color: #839496; 
+text-decoration: underline } /* Generic.Subheading */
+.pygments-style-solarized-dark .gt { color: #268bd2 } /* Generic.Traceback */
+.pygments-style-solarized-dark .kc { color: #2aa198 } /* Keyword.Constant */
+.pygments-style-solarized-dark .kd { color: #2aa198 } /* Keyword.Declaration */
+.pygments-style-solarized-dark .kn { color: #cb4b16 } /* Keyword.Namespace */
+.pygments-style-solarized-dark .kp { color: #859900 } /* Keyword.Pseudo */
+.pygments-style-solarized-dark .kr { color: #859900 } /* Keyword.Reserved */
+.pygments-style-solarized-dark .kt { color: #b58900 } /* Keyword.Type */
+.pygments-style-solarized-dark .ld { color: #839496 } /* Literal.Date */
+.pygments-style-solarized-dark .m { color: #2aa198 } /* Literal.Number */
+.pygments-style-solarized-dark .s { color: #2aa198 } /* Literal.String */
+.pygments-style-solarized-dark .na { color: #839496 } /* Name.Attribute */
+.pygments-style-solarized-dark .nb { color: #268bd2 } /* Name.Builtin */
+.pygments-style-solarized-dark .nc { color: #268bd2 } /* Name.Class */
+.pygments-style-solarized-dark .no { color: #268bd2 } /* Name.Constant */
+.pygments-style-solarized-dark .nd { color: #268bd2 } /* Name.Decorator */
+.pygments-style-solarized-dark .ni { color: #268bd2 } /* Name.Entity */
+.pygments-style-solarized-dark .ne { color: #268bd2 } /* Name.Exception */
+.pygments-style-solarized-dark .nf { color: #268bd2 } /* Name.Function */
+.pygments-style-solarized-dark .nl { color: #268bd2 } /* Name.Label */
+.pygments-style-solarized-dark .nn { color: #268bd2 } /* Name.Namespace */
+.pygments-style-solarized-dark .nx { color: #839496 } /* Name.Other */
+.pygments-style-solarized-dark .py { color: #839496 } /* Name.Property */
+.pygments-style-solarized-dark .nt { color: #268bd2 } /* Name.Tag */
+.pygments-style-solarized-dark .nv { color: #268bd2 } /* Name.Variable */
+.pygments-style-solarized-dark .ow { color: #859900 } /* Operator.Word */
+.pygments-style-solarized-dark .pm { color: #839496 } /* Punctuation.Marker */
+.pygments-style-solarized-dark .w { color: #839496 } /* Text.Whitespace */
+.pygments-style-solarized-dark .mb { color: #2aa198 } /* Literal.Number.Bin */
+.pygments-style-solarized-dark .mf { color: #2aa198 } /* Literal.Number.Float */
+.pygments-style-solarized-dark .mh { color: #2aa198 } /* Literal.Number.Hex */
+.pygments-style-solarized-dark .mi { color: #2aa198 } /* Literal.Number.Integer */
+.pygments-style-solarized-dark .mo { color: #2aa198 } /* Literal.Number.Oct */
+.pygments-style-solarized-dark .sa { color: #2aa198 } /* Literal.String.Affix */
+.pygments-style-solarized-dark .sb { color: #2aa198 } /* Literal.String.Backtick */
+.pygments-style-solarized-dark .sc { color: #2aa198 } /* Literal.String.Char */
+.pygments-style-solarized-dark .dl { color: #2aa198 } /* Literal.String.Delimiter */
+.pygments-style-solarized-dark .sd { color: #586e75 } /* Literal.String.Doc */
+.pygments-style-solarized-dark .s2 { color: #2aa198 } /* Literal.String.Double */
+.pygments-style-solarized-dark .se { color: #2aa198 } /* Literal.String.Escape */
+.pygments-style-solarized-dark .sh { color: #2aa198 } /* Literal.String.Heredoc */
+.pygments-style-solarized-dark .si { color: #2aa198 } /* Literal.String.Interpol */
+.pygments-style-solarized-dark .sx { color: #2aa198 } /* Literal.String.Other */
+.pygments-style-solarized-dark .sr { color: #cb4b16 } /* Literal.String.Regex */
+.pygments-style-solarized-dark .s1 { color: #2aa198 } /* Literal.String.Single */
+.pygments-style-solarized-dark .ss { color: #2aa198 } /* Literal.String.Symbol */
+.pygments-style-solarized-dark .bp { color: #268bd2 } /* Name.Builtin.Pseudo */
+.pygments-style-solarized-dark .fm { color: #268bd2 } /* Name.Function.Magic */
+.pygments-style-solarized-dark .vc { color: #268bd2 } /* Name.Variable.Class */
+.pygments-style-solarized-dark .vg { color: #268bd2 } /* Name.Variable.Global */
+.pygments-style-solarized-dark .vi { color: #268bd2 } /* Name.Variable.Instance */
+.pygments-style-solarized-dark .vm { color: #268bd2 } /* Name.Variable.Magic */
+.pygments-style-solarized-dark .il { color: #2aa198 } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/solarized-light.css` & `plumage-4.0.0/plumage/static/css/pygments/solarized-light.css`

 * *Files 14% similar despite different names*

```diff
@@ -1,144 +1,122 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #93a1a1;
-  background-color: #eee8d5;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos {
-  color: #93a1a1;
-  background-color: #eee8d5;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-.pygments-style-solarized-light .hll { background-color: #eee8d5; }
-
-.pygments-style-solarized-light {
-  background: #fdf6e3;
-  color: #657b83;
-}
-
-.pygments-style-solarized-light .c {
-  color: #93a1a1;
-  font-style: italic;
-} /* Comment */
-.pygments-style-solarized-light .err {
-  color: #657b83;
-  background-color: #dc322f;
-} /* Error */
-.pygments-style-solarized-light .esc { color: #657b83; } /* Escape */
-.pygments-style-solarized-light .g { color: #657b83; } /* Generic */
-.pygments-style-solarized-light .k { color: #859900; } /* Keyword */
-.pygments-style-solarized-light .l { color: #657b83; } /* Literal */
-.pygments-style-solarized-light .n { color: #657b83; } /* Name */
-.pygments-style-solarized-light .o { color: #93a1a1; } /* Operator */
-.pygments-style-solarized-light .x { color: #657b83; } /* Other */
-.pygments-style-solarized-light .p { color: #657b83; } /* Punctuation */
-.pygments-style-solarized-light .ch {
-  color: #93a1a1;
-  font-style: italic;
-} /* Comment.Hashbang */
-.pygments-style-solarized-light .cm {
-  color: #93a1a1;
-  font-style: italic;
-} /* Comment.Multiline */
-.pygments-style-solarized-light .cp { color: #d33682; } /* Comment.Preproc */
-.pygments-style-solarized-light .cpf { color: #93a1a1; } /* Comment.PreprocFile */
-.pygments-style-solarized-light .c1 {
-  color: #93a1a1;
-  font-style: italic;
-} /* Comment.Single */
-.pygments-style-solarized-light .cs {
-  color: #93a1a1;
-  font-style: italic;
-} /* Comment.Special */
-.pygments-style-solarized-light .gd { color: #dc322f; } /* Generic.Deleted */
-.pygments-style-solarized-light .ge {
-  color: #657b83;
-  font-style: italic;
-} /* Generic.Emph */
-.pygments-style-solarized-light .gr { color: #dc322f; } /* Generic.Error */
-.pygments-style-solarized-light .gh {
-  color: #657b83;
-  font-weight: bold;
-} /* Generic.Heading */
-.pygments-style-solarized-light .gi { color: #859900; } /* Generic.Inserted */
-.pygments-style-solarized-light .go { color: #657b83; } /* Generic.Output */
-.pygments-style-solarized-light .gp { color: #657b83; } /* Generic.Prompt */
-.pygments-style-solarized-light .gs {
-  color: #657b83;
-  font-weight: bold;
-} /* Generic.Strong */
-.pygments-style-solarized-light .gu {
-  color: #657b83;
-  text-decoration: underline;
-} /* Generic.Subheading */
-.pygments-style-solarized-light .gt { color: #268bd2; } /* Generic.Traceback */
-.pygments-style-solarized-light .kc { color: #2aa198; } /* Keyword.Constant */
-.pygments-style-solarized-light .kd { color: #2aa198; } /* Keyword.Declaration */
-.pygments-style-solarized-light .kn { color: #cb4b16; } /* Keyword.Namespace */
-.pygments-style-solarized-light .kp { color: #859900; } /* Keyword.Pseudo */
-.pygments-style-solarized-light .kr { color: #859900; } /* Keyword.Reserved */
-.pygments-style-solarized-light .kt { color: #b58900; } /* Keyword.Type */
-.pygments-style-solarized-light .ld { color: #657b83; } /* Literal.Date */
-.pygments-style-solarized-light .m { color: #2aa198; } /* Literal.Number */
-.pygments-style-solarized-light .s { color: #2aa198; } /* Literal.String */
-.pygments-style-solarized-light .na { color: #657b83; } /* Name.Attribute */
-.pygments-style-solarized-light .nb { color: #268bd2; } /* Name.Builtin */
-.pygments-style-solarized-light .nc { color: #268bd2; } /* Name.Class */
-.pygments-style-solarized-light .no { color: #268bd2; } /* Name.Constant */
-.pygments-style-solarized-light .nd { color: #268bd2; } /* Name.Decorator */
-.pygments-style-solarized-light .ni { color: #268bd2; } /* Name.Entity */
-.pygments-style-solarized-light .ne { color: #268bd2; } /* Name.Exception */
-.pygments-style-solarized-light .nf { color: #268bd2; } /* Name.Function */
-.pygments-style-solarized-light .nl { color: #268bd2; } /* Name.Label */
-.pygments-style-solarized-light .nn { color: #268bd2; } /* Name.Namespace */
-.pygments-style-solarized-light .nx { color: #657b83; } /* Name.Other */
-.pygments-style-solarized-light .py { color: #657b83; } /* Name.Property */
-.pygments-style-solarized-light .nt { color: #268bd2; } /* Name.Tag */
-.pygments-style-solarized-light .nv { color: #268bd2; } /* Name.Variable */
-.pygments-style-solarized-light .ow { color: #859900; } /* Operator.Word */
-.pygments-style-solarized-light .w { color: #657b83; } /* Text.Whitespace */
-.pygments-style-solarized-light .mb { color: #2aa198; } /* Literal.Number.Bin */
-.pygments-style-solarized-light .mf { color: #2aa198; } /* Literal.Number.Float */
-.pygments-style-solarized-light .mh { color: #2aa198; } /* Literal.Number.Hex */
-.pygments-style-solarized-light .mi { color: #2aa198; } /* Literal.Number.Integer */
-.pygments-style-solarized-light .mo { color: #2aa198; } /* Literal.Number.Oct */
-.pygments-style-solarized-light .sa { color: #2aa198; } /* Literal.String.Affix */
-.pygments-style-solarized-light .sb { color: #2aa198; } /* Literal.String.Backtick */
-.pygments-style-solarized-light .sc { color: #2aa198; } /* Literal.String.Char */
-.pygments-style-solarized-light .dl { color: #2aa198; } /* Literal.String.Delimiter */
-.pygments-style-solarized-light .sd { color: #93a1a1; } /* Literal.String.Doc */
-.pygments-style-solarized-light .s2 { color: #2aa198; } /* Literal.String.Double */
-.pygments-style-solarized-light .se { color: #2aa198; } /* Literal.String.Escape */
-.pygments-style-solarized-light .sh { color: #2aa198; } /* Literal.String.Heredoc */
-.pygments-style-solarized-light .si { color: #2aa198; } /* Literal.String.Interpol */
-.pygments-style-solarized-light .sx { color: #2aa198; } /* Literal.String.Other */
-.pygments-style-solarized-light .sr { color: #cb4b16; } /* Literal.String.Regex */
-.pygments-style-solarized-light .s1 { color: #2aa198; } /* Literal.String.Single */
-.pygments-style-solarized-light .ss { color: #2aa198; } /* Literal.String.Symbol */
-.pygments-style-solarized-light .bp { color: #268bd2; } /* Name.Builtin.Pseudo */
-.pygments-style-solarized-light .fm { color: #268bd2; } /* Name.Function.Magic */
-.pygments-style-solarized-light .vc { color: #268bd2; } /* Name.Variable.Class */
-.pygments-style-solarized-light .vg { color: #268bd2; } /* Name.Variable.Global */
-.pygments-style-solarized-light .vi { color: #268bd2; } /* Name.Variable.Instance */
-.pygments-style-solarized-light .vm { color: #268bd2; } /* Name.Variable.Magic */
-.pygments-style-solarized-light .il { color: #2aa198; } /* Literal.Number.Integer.Long */
+td.linenos .normal { color: #93a1a1; 
+background-color: #eee8d5; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos { color: #93a1a1; 
+background-color: #eee8d5; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+.pygments-style-solarized-light .hll { background-color: #eee8d5 }
+
+.pygments-style-solarized-light { background: #fdf6e3; 
+color: #657b83 }
+
+.pygments-style-solarized-light .c { color: #93a1a1; 
+font-style: italic } /* Comment */
+.pygments-style-solarized-light .err { color: #657b83; 
+background-color: #dc322f } /* Error */
+.pygments-style-solarized-light .esc { color: #657b83 } /* Escape */
+.pygments-style-solarized-light .g { color: #657b83 } /* Generic */
+.pygments-style-solarized-light .k { color: #859900 } /* Keyword */
+.pygments-style-solarized-light .l { color: #657b83 } /* Literal */
+.pygments-style-solarized-light .n { color: #657b83 } /* Name */
+.pygments-style-solarized-light .o { color: #93a1a1 } /* Operator */
+.pygments-style-solarized-light .x { color: #657b83 } /* Other */
+.pygments-style-solarized-light .p { color: #657b83 } /* Punctuation */
+.pygments-style-solarized-light .ch { color: #93a1a1; 
+font-style: italic } /* Comment.Hashbang */
+.pygments-style-solarized-light .cm { color: #93a1a1; 
+font-style: italic } /* Comment.Multiline */
+.pygments-style-solarized-light .cp { color: #d33682 } /* Comment.Preproc */
+.pygments-style-solarized-light .cpf { color: #93a1a1 } /* Comment.PreprocFile */
+.pygments-style-solarized-light .c1 { color: #93a1a1; 
+font-style: italic } /* Comment.Single */
+.pygments-style-solarized-light .cs { color: #93a1a1; 
+font-style: italic } /* Comment.Special */
+.pygments-style-solarized-light .gd { color: #dc322f } /* Generic.Deleted */
+.pygments-style-solarized-light .ge { color: #657b83; 
+font-style: italic } /* Generic.Emph */
+.pygments-style-solarized-light .ges { color: #657b83; 
+font-weight: bold; 
+font-style: italic } /* Generic.EmphStrong */
+.pygments-style-solarized-light .gr { color: #dc322f } /* Generic.Error */
+.pygments-style-solarized-light .gh { color: #657b83; 
+font-weight: bold } /* Generic.Heading */
+.pygments-style-solarized-light .gi { color: #859900 } /* Generic.Inserted */
+.pygments-style-solarized-light .go { color: #657b83 } /* Generic.Output */
+.pygments-style-solarized-light .gp { color: #268bd2; 
+font-weight: bold } /* Generic.Prompt */
+.pygments-style-solarized-light .gs { color: #657b83; 
+font-weight: bold } /* Generic.Strong */
+.pygments-style-solarized-light .gu { color: #657b83; 
+text-decoration: underline } /* Generic.Subheading */
+.pygments-style-solarized-light .gt { color: #268bd2 } /* Generic.Traceback */
+.pygments-style-solarized-light .kc { color: #2aa198 } /* Keyword.Constant */
+.pygments-style-solarized-light .kd { color: #2aa198 } /* Keyword.Declaration */
+.pygments-style-solarized-light .kn { color: #cb4b16 } /* Keyword.Namespace */
+.pygments-style-solarized-light .kp { color: #859900 } /* Keyword.Pseudo */
+.pygments-style-solarized-light .kr { color: #859900 } /* Keyword.Reserved */
+.pygments-style-solarized-light .kt { color: #b58900 } /* Keyword.Type */
+.pygments-style-solarized-light .ld { color: #657b83 } /* Literal.Date */
+.pygments-style-solarized-light .m { color: #2aa198 } /* Literal.Number */
+.pygments-style-solarized-light .s { color: #2aa198 } /* Literal.String */
+.pygments-style-solarized-light .na { color: #657b83 } /* Name.Attribute */
+.pygments-style-solarized-light .nb { color: #268bd2 } /* Name.Builtin */
+.pygments-style-solarized-light .nc { color: #268bd2 } /* Name.Class */
+.pygments-style-solarized-light .no { color: #268bd2 } /* Name.Constant */
+.pygments-style-solarized-light .nd { color: #268bd2 } /* Name.Decorator */
+.pygments-style-solarized-light .ni { color: #268bd2 } /* Name.Entity */
+.pygments-style-solarized-light .ne { color: #268bd2 } /* Name.Exception */
+.pygments-style-solarized-light .nf { color: #268bd2 } /* Name.Function */
+.pygments-style-solarized-light .nl { color: #268bd2 } /* Name.Label */
+.pygments-style-solarized-light .nn { color: #268bd2 } /* Name.Namespace */
+.pygments-style-solarized-light .nx { color: #657b83 } /* Name.Other */
+.pygments-style-solarized-light .py { color: #657b83 } /* Name.Property */
+.pygments-style-solarized-light .nt { color: #268bd2 } /* Name.Tag */
+.pygments-style-solarized-light .nv { color: #268bd2 } /* Name.Variable */
+.pygments-style-solarized-light .ow { color: #859900 } /* Operator.Word */
+.pygments-style-solarized-light .pm { color: #657b83 } /* Punctuation.Marker */
+.pygments-style-solarized-light .w { color: #657b83 } /* Text.Whitespace */
+.pygments-style-solarized-light .mb { color: #2aa198 } /* Literal.Number.Bin */
+.pygments-style-solarized-light .mf { color: #2aa198 } /* Literal.Number.Float */
+.pygments-style-solarized-light .mh { color: #2aa198 } /* Literal.Number.Hex */
+.pygments-style-solarized-light .mi { color: #2aa198 } /* Literal.Number.Integer */
+.pygments-style-solarized-light .mo { color: #2aa198 } /* Literal.Number.Oct */
+.pygments-style-solarized-light .sa { color: #2aa198 } /* Literal.String.Affix */
+.pygments-style-solarized-light .sb { color: #2aa198 } /* Literal.String.Backtick */
+.pygments-style-solarized-light .sc { color: #2aa198 } /* Literal.String.Char */
+.pygments-style-solarized-light .dl { color: #2aa198 } /* Literal.String.Delimiter */
+.pygments-style-solarized-light .sd { color: #93a1a1 } /* Literal.String.Doc */
+.pygments-style-solarized-light .s2 { color: #2aa198 } /* Literal.String.Double */
+.pygments-style-solarized-light .se { color: #2aa198 } /* Literal.String.Escape */
+.pygments-style-solarized-light .sh { color: #2aa198 } /* Literal.String.Heredoc */
+.pygments-style-solarized-light .si { color: #2aa198 } /* Literal.String.Interpol */
+.pygments-style-solarized-light .sx { color: #2aa198 } /* Literal.String.Other */
+.pygments-style-solarized-light .sr { color: #cb4b16 } /* Literal.String.Regex */
+.pygments-style-solarized-light .s1 { color: #2aa198 } /* Literal.String.Single */
+.pygments-style-solarized-light .ss { color: #2aa198 } /* Literal.String.Symbol */
+.pygments-style-solarized-light .bp { color: #268bd2 } /* Name.Builtin.Pseudo */
+.pygments-style-solarized-light .fm { color: #268bd2 } /* Name.Function.Magic */
+.pygments-style-solarized-light .vc { color: #268bd2 } /* Name.Variable.Class */
+.pygments-style-solarized-light .vg { color: #268bd2 } /* Name.Variable.Global */
+.pygments-style-solarized-light .vi { color: #268bd2 } /* Name.Variable.Instance */
+.pygments-style-solarized-light .vm { color: #268bd2 } /* Name.Variable.Magic */
+.pygments-style-solarized-light .il { color: #2aa198 } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/stata-dark.css` & `plumage-4.0.0/plumage/static/css/pygments/stata-light.css`

 * *Files 25% similar despite different names*

```diff
@@ -1,144 +1,96 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-.pygments-style-stata-dark .hll { background-color: #49483e; }
-
-.pygments-style-stata-dark {
-  background: #232629;
-  color: #ccc;
-}
-
-.pygments-style-stata-dark .c {
-  color: #777;
-  font-style: italic;
-} /* Comment */
-.pygments-style-stata-dark .err {
-  color: #a61717;
-  background-color: #e3d2d2;
-} /* Error */
-.pygments-style-stata-dark .k {
-  color: #7686bb;
-  font-weight: bold;
-} /* Keyword */
-.pygments-style-stata-dark .ch {
-  color: #777;
-  font-style: italic;
-} /* Comment.Hashbang */
-.pygments-style-stata-dark .cm {
-  color: #777;
-  font-style: italic;
-} /* Comment.Multiline */
-.pygments-style-stata-dark .cp {
-  color: #777;
-  font-style: italic;
-} /* Comment.Preproc */
-.pygments-style-stata-dark .cpf {
-  color: #777;
-  font-style: italic;
-} /* Comment.PreprocFile */
-.pygments-style-stata-dark .c1 {
-  color: #777;
-  font-style: italic;
-} /* Comment.Single */
-.pygments-style-stata-dark .cs {
-  color: #777;
-  font-style: italic;
-} /* Comment.Special */
-.pygments-style-stata-dark .gp { color: #fff; } /* Generic.Prompt */
-.pygments-style-stata-dark .kc {
-  color: #7686bb;
-  font-weight: bold;
-} /* Keyword.Constant */
-.pygments-style-stata-dark .kd {
-  color: #7686bb;
-  font-weight: bold;
-} /* Keyword.Declaration */
-.pygments-style-stata-dark .kn {
-  color: #7686bb;
-  font-weight: bold;
-} /* Keyword.Namespace */
-.pygments-style-stata-dark .kp {
-  color: #7686bb;
-  font-weight: bold;
-} /* Keyword.Pseudo */
-.pygments-style-stata-dark .kr {
-  color: #7686bb;
-  font-weight: bold;
-} /* Keyword.Reserved */
-.pygments-style-stata-dark .kt {
-  color: #7686bb;
-  font-weight: bold;
-} /* Keyword.Type */
-.pygments-style-stata-dark .m { color: #4fb8cc; } /* Literal.Number */
-.pygments-style-stata-dark .s { color: #51cc99; } /* Literal.String */
-.pygments-style-stata-dark .nf { color: #6a6aff; } /* Name.Function */
-.pygments-style-stata-dark .nx { color: #e2828e; } /* Name.Other */
-.pygments-style-stata-dark .nv {
-  color: #7ab4db;
-  font-weight: bold;
-} /* Name.Variable */
-.pygments-style-stata-dark .w { color: #bbb; } /* Text.Whitespace */
-.pygments-style-stata-dark .mb { color: #4fb8cc; } /* Literal.Number.Bin */
-.pygments-style-stata-dark .mf { color: #4fb8cc; } /* Literal.Number.Float */
-.pygments-style-stata-dark .mh { color: #4fb8cc; } /* Literal.Number.Hex */
-.pygments-style-stata-dark .mi { color: #4fb8cc; } /* Literal.Number.Integer */
-.pygments-style-stata-dark .mo { color: #4fb8cc; } /* Literal.Number.Oct */
-.pygments-style-stata-dark .sa { color: #51cc99; } /* Literal.String.Affix */
-.pygments-style-stata-dark .sb { color: #51cc99; } /* Literal.String.Backtick */
-.pygments-style-stata-dark .sc { color: #51cc99; } /* Literal.String.Char */
-.pygments-style-stata-dark .dl { color: #51cc99; } /* Literal.String.Delimiter */
-.pygments-style-stata-dark .sd { color: #51cc99; } /* Literal.String.Doc */
-.pygments-style-stata-dark .s2 { color: #51cc99; } /* Literal.String.Double */
-.pygments-style-stata-dark .se { color: #51cc99; } /* Literal.String.Escape */
-.pygments-style-stata-dark .sh { color: #51cc99; } /* Literal.String.Heredoc */
-.pygments-style-stata-dark .si { color: #51cc99; } /* Literal.String.Interpol */
-.pygments-style-stata-dark .sx { color: #51cc99; } /* Literal.String.Other */
-.pygments-style-stata-dark .sr { color: #51cc99; } /* Literal.String.Regex */
-.pygments-style-stata-dark .s1 { color: #51cc99; } /* Literal.String.Single */
-.pygments-style-stata-dark .ss { color: #51cc99; } /* Literal.String.Symbol */
-.pygments-style-stata-dark .fm { color: #6a6aff; } /* Name.Function.Magic */
-.pygments-style-stata-dark .vc {
-  color: #7ab4db;
-  font-weight: bold;
-} /* Name.Variable.Class */
-.pygments-style-stata-dark .vg {
-  color: #be646c;
-  font-weight: bold;
-} /* Name.Variable.Global */
-.pygments-style-stata-dark .vi {
-  color: #7ab4db;
-  font-weight: bold;
-} /* Name.Variable.Instance */
-.pygments-style-stata-dark .vm {
-  color: #7ab4db;
-  font-weight: bold;
-} /* Name.Variable.Magic */
-.pygments-style-stata-dark .il { color: #4fb8cc; } /* Literal.Number.Integer.Long */
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+.pygments-style-stata-light .hll { background-color: #ffc }
+
+.pygments-style-stata-light { background: #fff; 
+color: #111 }
+
+.pygments-style-stata-light .c { color: #080; 
+font-style: italic } /* Comment */
+.pygments-style-stata-light .err { color: #a61717; 
+background-color: #e3d2d2 } /* Error */
+.pygments-style-stata-light .k { color: #353580; 
+font-weight: bold } /* Keyword */
+.pygments-style-stata-light .ch { color: #080; 
+font-style: italic } /* Comment.Hashbang */
+.pygments-style-stata-light .cm { color: #080; 
+font-style: italic } /* Comment.Multiline */
+.pygments-style-stata-light .cp { color: #080; 
+font-style: italic } /* Comment.Preproc */
+.pygments-style-stata-light .cpf { color: #080; 
+font-style: italic } /* Comment.PreprocFile */
+.pygments-style-stata-light .c1 { color: #080; 
+font-style: italic } /* Comment.Single */
+.pygments-style-stata-light .cs { color: #080; 
+font-style: italic } /* Comment.Special */
+.pygments-style-stata-light .kc { color: #353580; 
+font-weight: bold } /* Keyword.Constant */
+.pygments-style-stata-light .kd { color: #353580; 
+font-weight: bold } /* Keyword.Declaration */
+.pygments-style-stata-light .kn { color: #353580; 
+font-weight: bold } /* Keyword.Namespace */
+.pygments-style-stata-light .kp { color: #353580; 
+font-weight: bold } /* Keyword.Pseudo */
+.pygments-style-stata-light .kr { color: #353580; 
+font-weight: bold } /* Keyword.Reserved */
+.pygments-style-stata-light .kt { color: #353580; 
+font-weight: bold } /* Keyword.Type */
+.pygments-style-stata-light .m { color: #2c2cff } /* Literal.Number */
+.pygments-style-stata-light .s { color: #7a2424 } /* Literal.String */
+.pygments-style-stata-light .nf { color: #2c2cff } /* Name.Function */
+.pygments-style-stata-light .nx { color: #be646c } /* Name.Other */
+.pygments-style-stata-light .nv { color: #35baba; 
+font-weight: bold } /* Name.Variable */
+.pygments-style-stata-light .w { color: #bbb } /* Text.Whitespace */
+.pygments-style-stata-light .mb { color: #2c2cff } /* Literal.Number.Bin */
+.pygments-style-stata-light .mf { color: #2c2cff } /* Literal.Number.Float */
+.pygments-style-stata-light .mh { color: #2c2cff } /* Literal.Number.Hex */
+.pygments-style-stata-light .mi { color: #2c2cff } /* Literal.Number.Integer */
+.pygments-style-stata-light .mo { color: #2c2cff } /* Literal.Number.Oct */
+.pygments-style-stata-light .sa { color: #7a2424 } /* Literal.String.Affix */
+.pygments-style-stata-light .sb { color: #7a2424 } /* Literal.String.Backtick */
+.pygments-style-stata-light .sc { color: #7a2424 } /* Literal.String.Char */
+.pygments-style-stata-light .dl { color: #7a2424 } /* Literal.String.Delimiter */
+.pygments-style-stata-light .sd { color: #7a2424 } /* Literal.String.Doc */
+.pygments-style-stata-light .s2 { color: #7a2424 } /* Literal.String.Double */
+.pygments-style-stata-light .se { color: #7a2424 } /* Literal.String.Escape */
+.pygments-style-stata-light .sh { color: #7a2424 } /* Literal.String.Heredoc */
+.pygments-style-stata-light .si { color: #7a2424 } /* Literal.String.Interpol */
+.pygments-style-stata-light .sx { color: #7a2424 } /* Literal.String.Other */
+.pygments-style-stata-light .sr { color: #7a2424 } /* Literal.String.Regex */
+.pygments-style-stata-light .s1 { color: #7a2424 } /* Literal.String.Single */
+.pygments-style-stata-light .ss { color: #7a2424 } /* Literal.String.Symbol */
+.pygments-style-stata-light .fm { color: #2c2cff } /* Name.Function.Magic */
+.pygments-style-stata-light .vc { color: #35baba; 
+font-weight: bold } /* Name.Variable.Class */
+.pygments-style-stata-light .vg { color: #b5565e; 
+font-weight: bold } /* Name.Variable.Global */
+.pygments-style-stata-light .vi { color: #35baba; 
+font-weight: bold } /* Name.Variable.Instance */
+.pygments-style-stata-light .vm { color: #35baba; 
+font-weight: bold } /* Name.Variable.Magic */
+.pygments-style-stata-light .il { color: #2c2cff } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/stata-light.css` & `plumage-4.0.0/plumage/static/css/pygments/stata.css`

 * *Files 10% similar despite different names*

```diff
@@ -25,119 +25,119 @@
 
 span.linenos.special {
   color: #000;
   background-color: #ffffc0;
   padding-left: 5px;
   padding-right: 5px;
 }
-.pygments-style-stata-light .hll { background-color: #ffc; }
+.pygments-style-stata .hll { background-color: #ffc; }
 
-.pygments-style-stata-light {
+.pygments-style-stata {
   background: #fff;
   color: #111;
 }
 
-.pygments-style-stata-light .c {
+.pygments-style-stata .c {
   color: #080;
   font-style: italic;
 } /* Comment */
-.pygments-style-stata-light .err {
+.pygments-style-stata .err {
   color: #a61717;
   background-color: #e3d2d2;
 } /* Error */
-.pygments-style-stata-light .k {
+.pygments-style-stata .k {
   color: #353580;
   font-weight: bold;
 } /* Keyword */
-.pygments-style-stata-light .ch {
+.pygments-style-stata .ch {
   color: #080;
   font-style: italic;
 } /* Comment.Hashbang */
-.pygments-style-stata-light .cm {
+.pygments-style-stata .cm {
   color: #080;
   font-style: italic;
 } /* Comment.Multiline */
-.pygments-style-stata-light .cp {
+.pygments-style-stata .cp {
   color: #080;
   font-style: italic;
 } /* Comment.Preproc */
-.pygments-style-stata-light .cpf {
+.pygments-style-stata .cpf {
   color: #080;
   font-style: italic;
 } /* Comment.PreprocFile */
-.pygments-style-stata-light .c1 {
+.pygments-style-stata .c1 {
   color: #080;
   font-style: italic;
 } /* Comment.Single */
-.pygments-style-stata-light .cs {
+.pygments-style-stata .cs {
   color: #080;
   font-style: italic;
 } /* Comment.Special */
-.pygments-style-stata-light .kc {
+.pygments-style-stata .kc {
   color: #353580;
   font-weight: bold;
 } /* Keyword.Constant */
-.pygments-style-stata-light .kd {
+.pygments-style-stata .kd {
   color: #353580;
   font-weight: bold;
 } /* Keyword.Declaration */
-.pygments-style-stata-light .kn {
+.pygments-style-stata .kn {
   color: #353580;
   font-weight: bold;
 } /* Keyword.Namespace */
-.pygments-style-stata-light .kp {
+.pygments-style-stata .kp {
   color: #353580;
   font-weight: bold;
 } /* Keyword.Pseudo */
-.pygments-style-stata-light .kr {
+.pygments-style-stata .kr {
   color: #353580;
   font-weight: bold;
 } /* Keyword.Reserved */
-.pygments-style-stata-light .kt {
+.pygments-style-stata .kt {
   color: #353580;
   font-weight: bold;
 } /* Keyword.Type */
-.pygments-style-stata-light .m { color: #2c2cff; } /* Literal.Number */
-.pygments-style-stata-light .s { color: #7a2424; } /* Literal.String */
-.pygments-style-stata-light .nf { color: #2c2cff; } /* Name.Function */
-.pygments-style-stata-light .nx { color: #be646c; } /* Name.Other */
-.pygments-style-stata-light .nv {
+.pygments-style-stata .m { color: #2c2cff; } /* Literal.Number */
+.pygments-style-stata .s { color: #7a2424; } /* Literal.String */
+.pygments-style-stata .nf { color: #2c2cff; } /* Name.Function */
+.pygments-style-stata .nx { color: #be646c; } /* Name.Other */
+.pygments-style-stata .nv {
   color: #35baba;
   font-weight: bold;
 } /* Name.Variable */
-.pygments-style-stata-light .w { color: #bbb; } /* Text.Whitespace */
-.pygments-style-stata-light .mb { color: #2c2cff; } /* Literal.Number.Bin */
-.pygments-style-stata-light .mf { color: #2c2cff; } /* Literal.Number.Float */
-.pygments-style-stata-light .mh { color: #2c2cff; } /* Literal.Number.Hex */
-.pygments-style-stata-light .mi { color: #2c2cff; } /* Literal.Number.Integer */
-.pygments-style-stata-light .mo { color: #2c2cff; } /* Literal.Number.Oct */
-.pygments-style-stata-light .sa { color: #7a2424; } /* Literal.String.Affix */
-.pygments-style-stata-light .sb { color: #7a2424; } /* Literal.String.Backtick */
-.pygments-style-stata-light .sc { color: #7a2424; } /* Literal.String.Char */
-.pygments-style-stata-light .dl { color: #7a2424; } /* Literal.String.Delimiter */
-.pygments-style-stata-light .sd { color: #7a2424; } /* Literal.String.Doc */
-.pygments-style-stata-light .s2 { color: #7a2424; } /* Literal.String.Double */
-.pygments-style-stata-light .se { color: #7a2424; } /* Literal.String.Escape */
-.pygments-style-stata-light .sh { color: #7a2424; } /* Literal.String.Heredoc */
-.pygments-style-stata-light .si { color: #7a2424; } /* Literal.String.Interpol */
-.pygments-style-stata-light .sx { color: #7a2424; } /* Literal.String.Other */
-.pygments-style-stata-light .sr { color: #7a2424; } /* Literal.String.Regex */
-.pygments-style-stata-light .s1 { color: #7a2424; } /* Literal.String.Single */
-.pygments-style-stata-light .ss { color: #7a2424; } /* Literal.String.Symbol */
-.pygments-style-stata-light .fm { color: #2c2cff; } /* Name.Function.Magic */
-.pygments-style-stata-light .vc {
+.pygments-style-stata .w { color: #bbb; } /* Text.Whitespace */
+.pygments-style-stata .mb { color: #2c2cff; } /* Literal.Number.Bin */
+.pygments-style-stata .mf { color: #2c2cff; } /* Literal.Number.Float */
+.pygments-style-stata .mh { color: #2c2cff; } /* Literal.Number.Hex */
+.pygments-style-stata .mi { color: #2c2cff; } /* Literal.Number.Integer */
+.pygments-style-stata .mo { color: #2c2cff; } /* Literal.Number.Oct */
+.pygments-style-stata .sa { color: #7a2424; } /* Literal.String.Affix */
+.pygments-style-stata .sb { color: #7a2424; } /* Literal.String.Backtick */
+.pygments-style-stata .sc { color: #7a2424; } /* Literal.String.Char */
+.pygments-style-stata .dl { color: #7a2424; } /* Literal.String.Delimiter */
+.pygments-style-stata .sd { color: #7a2424; } /* Literal.String.Doc */
+.pygments-style-stata .s2 { color: #7a2424; } /* Literal.String.Double */
+.pygments-style-stata .se { color: #7a2424; } /* Literal.String.Escape */
+.pygments-style-stata .sh { color: #7a2424; } /* Literal.String.Heredoc */
+.pygments-style-stata .si { color: #7a2424; } /* Literal.String.Interpol */
+.pygments-style-stata .sx { color: #7a2424; } /* Literal.String.Other */
+.pygments-style-stata .sr { color: #7a2424; } /* Literal.String.Regex */
+.pygments-style-stata .s1 { color: #7a2424; } /* Literal.String.Single */
+.pygments-style-stata .ss { color: #7a2424; } /* Literal.String.Symbol */
+.pygments-style-stata .fm { color: #2c2cff; } /* Name.Function.Magic */
+.pygments-style-stata .vc {
   color: #35baba;
   font-weight: bold;
 } /* Name.Variable.Class */
-.pygments-style-stata-light .vg {
+.pygments-style-stata .vg {
   color: #b5565e;
   font-weight: bold;
 } /* Name.Variable.Global */
-.pygments-style-stata-light .vi {
+.pygments-style-stata .vi {
   color: #35baba;
   font-weight: bold;
 } /* Name.Variable.Instance */
-.pygments-style-stata-light .vm {
+.pygments-style-stata .vm {
   color: #35baba;
   font-weight: bold;
 } /* Name.Variable.Magic */
-.pygments-style-stata-light .il { color: #2c2cff; } /* Literal.Number.Integer.Long */
+.pygments-style-stata .il { color: #2c2cff; } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/trac.css` & `plumage-4.0.0/plumage/static/css/pygments/trac.css`

 * *Files 8% similar despite different names*

```diff
@@ -1,148 +1,114 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
-}
-.pygments-style-trac .hll { background-color: #ffc; }
-
-.pygments-style-trac {
-  background: #fff;
-}
-
-.pygments-style-trac .c {
-  color: #998;
-  font-style: italic;
-} /* Comment */
-.pygments-style-trac .err {
-  color: #a61717;
-  background-color: #e3d2d2;
-} /* Error */
-.pygments-style-trac .k { font-weight: bold; } /* Keyword */
-.pygments-style-trac .o { font-weight: bold; } /* Operator */
-.pygments-style-trac .ch {
-  color: #998;
-  font-style: italic;
-} /* Comment.Hashbang */
-.pygments-style-trac .cm {
-  color: #998;
-  font-style: italic;
-} /* Comment.Multiline */
-.pygments-style-trac .cp {
-  color: #999;
-  font-weight: bold;
-} /* Comment.Preproc */
-.pygments-style-trac .cpf {
-  color: #998;
-  font-style: italic;
-} /* Comment.PreprocFile */
-.pygments-style-trac .c1 {
-  color: #998;
-  font-style: italic;
-} /* Comment.Single */
-.pygments-style-trac .cs {
-  color: #999;
-  font-weight: bold;
-  font-style: italic;
-} /* Comment.Special */
-.pygments-style-trac .gd {
-  color: #000;
-  background-color: #fdd;
-} /* Generic.Deleted */
-.pygments-style-trac .ge { font-style: italic; } /* Generic.Emph */
-.pygments-style-trac .gr { color: #a00; } /* Generic.Error */
-.pygments-style-trac .gh { color: #999; } /* Generic.Heading */
-.pygments-style-trac .gi {
-  color: #000;
-  background-color: #dfd;
-} /* Generic.Inserted */
-.pygments-style-trac .go { color: #888; } /* Generic.Output */
-.pygments-style-trac .gp { color: #555; } /* Generic.Prompt */
-.pygments-style-trac .gs { font-weight: bold; } /* Generic.Strong */
-.pygments-style-trac .gu { color: #aaa; } /* Generic.Subheading */
-.pygments-style-trac .gt { color: #a00; } /* Generic.Traceback */
-.pygments-style-trac .kc { font-weight: bold; } /* Keyword.Constant */
-.pygments-style-trac .kd { font-weight: bold; } /* Keyword.Declaration */
-.pygments-style-trac .kn { font-weight: bold; } /* Keyword.Namespace */
-.pygments-style-trac .kp { font-weight: bold; } /* Keyword.Pseudo */
-.pygments-style-trac .kr { font-weight: bold; } /* Keyword.Reserved */
-.pygments-style-trac .kt {
-  color: #458;
-  font-weight: bold;
-} /* Keyword.Type */
-.pygments-style-trac .m { color: #099; } /* Literal.Number */
-.pygments-style-trac .s { color: #b84; } /* Literal.String */
-.pygments-style-trac .na { color: #008080; } /* Name.Attribute */
-.pygments-style-trac .nb { color: #999; } /* Name.Builtin */
-.pygments-style-trac .nc {
-  color: #458;
-  font-weight: bold;
-} /* Name.Class */
-.pygments-style-trac .no { color: #008080; } /* Name.Constant */
-.pygments-style-trac .ni { color: #800080; } /* Name.Entity */
-.pygments-style-trac .ne {
-  color: #900;
-  font-weight: bold;
-} /* Name.Exception */
-.pygments-style-trac .nf {
-  color: #900;
-  font-weight: bold;
-} /* Name.Function */
-.pygments-style-trac .nn { color: #555; } /* Name.Namespace */
-.pygments-style-trac .nt { color: #000080; } /* Name.Tag */
-.pygments-style-trac .nv { color: #008080; } /* Name.Variable */
-.pygments-style-trac .ow { font-weight: bold; } /* Operator.Word */
-.pygments-style-trac .w { color: #bbb; } /* Text.Whitespace */
-.pygments-style-trac .mb { color: #099; } /* Literal.Number.Bin */
-.pygments-style-trac .mf { color: #099; } /* Literal.Number.Float */
-.pygments-style-trac .mh { color: #099; } /* Literal.Number.Hex */
-.pygments-style-trac .mi { color: #099; } /* Literal.Number.Integer */
-.pygments-style-trac .mo { color: #099; } /* Literal.Number.Oct */
-.pygments-style-trac .sa { color: #b84; } /* Literal.String.Affix */
-.pygments-style-trac .sb { color: #b84; } /* Literal.String.Backtick */
-.pygments-style-trac .sc { color: #b84; } /* Literal.String.Char */
-.pygments-style-trac .dl { color: #b84; } /* Literal.String.Delimiter */
-.pygments-style-trac .sd { color: #b84; } /* Literal.String.Doc */
-.pygments-style-trac .s2 { color: #b84; } /* Literal.String.Double */
-.pygments-style-trac .se { color: #b84; } /* Literal.String.Escape */
-.pygments-style-trac .sh { color: #b84; } /* Literal.String.Heredoc */
-.pygments-style-trac .si { color: #b84; } /* Literal.String.Interpol */
-.pygments-style-trac .sx { color: #b84; } /* Literal.String.Other */
-.pygments-style-trac .sr { color: #808000; } /* Literal.String.Regex */
-.pygments-style-trac .s1 { color: #b84; } /* Literal.String.Single */
-.pygments-style-trac .ss { color: #b84; } /* Literal.String.Symbol */
-.pygments-style-trac .bp { color: #999; } /* Name.Builtin.Pseudo */
-.pygments-style-trac .fm {
-  color: #900;
-  font-weight: bold;
-} /* Name.Function.Magic */
-.pygments-style-trac .vc { color: #008080; } /* Name.Variable.Class */
-.pygments-style-trac .vg { color: #008080; } /* Name.Variable.Global */
-.pygments-style-trac .vi { color: #008080; } /* Name.Variable.Instance */
-.pygments-style-trac .vm { color: #008080; } /* Name.Variable.Magic */
-.pygments-style-trac .il { color: #099; } /* Literal.Number.Integer.Long */
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
+}
+.pygments-style-trac .hll { background-color: #ffc }
+
+.pygments-style-trac { background: #fff; 
+}
+
+.pygments-style-trac .c { color: #998; 
+font-style: italic } /* Comment */
+.pygments-style-trac .err { color: #a61717; 
+background-color: #e3d2d2 } /* Error */
+.pygments-style-trac .k { font-weight: bold } /* Keyword */
+.pygments-style-trac .o { font-weight: bold } /* Operator */
+.pygments-style-trac .ch { color: #998; 
+font-style: italic } /* Comment.Hashbang */
+.pygments-style-trac .cm { color: #998; 
+font-style: italic } /* Comment.Multiline */
+.pygments-style-trac .cp { color: #999; 
+font-weight: bold } /* Comment.Preproc */
+.pygments-style-trac .cpf { color: #998; 
+font-style: italic } /* Comment.PreprocFile */
+.pygments-style-trac .c1 { color: #998; 
+font-style: italic } /* Comment.Single */
+.pygments-style-trac .cs { color: #999; 
+font-weight: bold; 
+font-style: italic } /* Comment.Special */
+.pygments-style-trac .gd { color: #000; 
+background-color: #fdd } /* Generic.Deleted */
+.pygments-style-trac .ge { font-style: italic } /* Generic.Emph */
+.pygments-style-trac .ges { font-weight: bold; 
+font-style: italic } /* Generic.EmphStrong */
+.pygments-style-trac .gr { color: #a00 } /* Generic.Error */
+.pygments-style-trac .gh { color: #999 } /* Generic.Heading */
+.pygments-style-trac .gi { color: #000; 
+background-color: #dfd } /* Generic.Inserted */
+.pygments-style-trac .go { color: #888 } /* Generic.Output */
+.pygments-style-trac .gp { color: #555 } /* Generic.Prompt */
+.pygments-style-trac .gs { font-weight: bold } /* Generic.Strong */
+.pygments-style-trac .gu { color: #aaa } /* Generic.Subheading */
+.pygments-style-trac .gt { color: #a00 } /* Generic.Traceback */
+.pygments-style-trac .kc { font-weight: bold } /* Keyword.Constant */
+.pygments-style-trac .kd { font-weight: bold } /* Keyword.Declaration */
+.pygments-style-trac .kn { font-weight: bold } /* Keyword.Namespace */
+.pygments-style-trac .kp { font-weight: bold } /* Keyword.Pseudo */
+.pygments-style-trac .kr { font-weight: bold } /* Keyword.Reserved */
+.pygments-style-trac .kt { color: #458; 
+font-weight: bold } /* Keyword.Type */
+.pygments-style-trac .m { color: #099 } /* Literal.Number */
+.pygments-style-trac .s { color: #b84 } /* Literal.String */
+.pygments-style-trac .na { color: #008080 } /* Name.Attribute */
+.pygments-style-trac .nb { color: #999 } /* Name.Builtin */
+.pygments-style-trac .nc { color: #458; 
+font-weight: bold } /* Name.Class */
+.pygments-style-trac .no { color: #008080 } /* Name.Constant */
+.pygments-style-trac .ni { color: #800080 } /* Name.Entity */
+.pygments-style-trac .ne { color: #900; 
+font-weight: bold } /* Name.Exception */
+.pygments-style-trac .nf { color: #900; 
+font-weight: bold } /* Name.Function */
+.pygments-style-trac .nn { color: #555 } /* Name.Namespace */
+.pygments-style-trac .nt { color: #000080 } /* Name.Tag */
+.pygments-style-trac .nv { color: #008080 } /* Name.Variable */
+.pygments-style-trac .ow { font-weight: bold } /* Operator.Word */
+.pygments-style-trac .w { color: #bbb } /* Text.Whitespace */
+.pygments-style-trac .mb { color: #099 } /* Literal.Number.Bin */
+.pygments-style-trac .mf { color: #099 } /* Literal.Number.Float */
+.pygments-style-trac .mh { color: #099 } /* Literal.Number.Hex */
+.pygments-style-trac .mi { color: #099 } /* Literal.Number.Integer */
+.pygments-style-trac .mo { color: #099 } /* Literal.Number.Oct */
+.pygments-style-trac .sa { color: #b84 } /* Literal.String.Affix */
+.pygments-style-trac .sb { color: #b84 } /* Literal.String.Backtick */
+.pygments-style-trac .sc { color: #b84 } /* Literal.String.Char */
+.pygments-style-trac .dl { color: #b84 } /* Literal.String.Delimiter */
+.pygments-style-trac .sd { color: #b84 } /* Literal.String.Doc */
+.pygments-style-trac .s2 { color: #b84 } /* Literal.String.Double */
+.pygments-style-trac .se { color: #b84 } /* Literal.String.Escape */
+.pygments-style-trac .sh { color: #b84 } /* Literal.String.Heredoc */
+.pygments-style-trac .si { color: #b84 } /* Literal.String.Interpol */
+.pygments-style-trac .sx { color: #b84 } /* Literal.String.Other */
+.pygments-style-trac .sr { color: #808000 } /* Literal.String.Regex */
+.pygments-style-trac .s1 { color: #b84 } /* Literal.String.Single */
+.pygments-style-trac .ss { color: #b84 } /* Literal.String.Symbol */
+.pygments-style-trac .bp { color: #999 } /* Name.Builtin.Pseudo */
+.pygments-style-trac .fm { color: #900; 
+font-weight: bold } /* Name.Function.Magic */
+.pygments-style-trac .vc { color: #008080 } /* Name.Variable.Class */
+.pygments-style-trac .vg { color: #008080 } /* Name.Variable.Global */
+.pygments-style-trac .vi { color: #008080 } /* Name.Variable.Instance */
+.pygments-style-trac .vm { color: #008080 } /* Name.Variable.Magic */
+.pygments-style-trac .il { color: #099 } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/vim.css` & `plumage-4.0.0/plumage/static/css/pygments/vim.css`

 * *Files 16% similar despite different names*

```diff
@@ -1,137 +1,118 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
-.pygments-style-vim .hll { background-color: #222; }
+.pygments-style-vim .hll { background-color: #222 }
 
-.pygments-style-vim {
-  background: #000;
-  color: #ccc;
-}
-.pygments-style-vim .c { color: #000080; } /* Comment */
-.pygments-style-vim .err {
-  color: #ccc;
-  border: 1px solid #f00;
-} /* Error */
-.pygments-style-vim .esc { color: #ccc; } /* Escape */
-.pygments-style-vim .g { color: #ccc; } /* Generic */
-.pygments-style-vim .k { color: #cdcd00; } /* Keyword */
-.pygments-style-vim .l { color: #ccc; } /* Literal */
-.pygments-style-vim .n { color: #ccc; } /* Name */
-.pygments-style-vim .o { color: #39c; } /* Operator */
-.pygments-style-vim .x { color: #ccc; } /* Other */
-.pygments-style-vim .p { color: #ccc; } /* Punctuation */
-.pygments-style-vim .ch { color: #000080; } /* Comment.Hashbang */
-.pygments-style-vim .cm { color: #000080; } /* Comment.Multiline */
-.pygments-style-vim .cp { color: #000080; } /* Comment.Preproc */
-.pygments-style-vim .cpf { color: #000080; } /* Comment.PreprocFile */
-.pygments-style-vim .c1 { color: #000080; } /* Comment.Single */
-.pygments-style-vim .cs {
-  color: #cd0000;
-  font-weight: bold;
-} /* Comment.Special */
-.pygments-style-vim .gd { color: #cd0000; } /* Generic.Deleted */
-.pygments-style-vim .ge {
-  color: #ccc;
-  font-style: italic;
-} /* Generic.Emph */
-.pygments-style-vim .gr { color: #f00; } /* Generic.Error */
-.pygments-style-vim .gh {
-  color: #000080;
-  font-weight: bold;
-} /* Generic.Heading */
-.pygments-style-vim .gi { color: #00cd00; } /* Generic.Inserted */
-.pygments-style-vim .go { color: #888; } /* Generic.Output */
-.pygments-style-vim .gp {
-  color: #000080;
-  font-weight: bold;
-} /* Generic.Prompt */
-.pygments-style-vim .gs {
-  color: #ccc;
-  font-weight: bold;
-} /* Generic.Strong */
-.pygments-style-vim .gu {
-  color: #800080;
-  font-weight: bold;
-} /* Generic.Subheading */
-.pygments-style-vim .gt { color: #04d; } /* Generic.Traceback */
-.pygments-style-vim .kc { color: #cdcd00; } /* Keyword.Constant */
-.pygments-style-vim .kd { color: #00cd00; } /* Keyword.Declaration */
-.pygments-style-vim .kn { color: #cd00cd; } /* Keyword.Namespace */
-.pygments-style-vim .kp { color: #cdcd00; } /* Keyword.Pseudo */
-.pygments-style-vim .kr { color: #cdcd00; } /* Keyword.Reserved */
-.pygments-style-vim .kt { color: #00cd00; } /* Keyword.Type */
-.pygments-style-vim .ld { color: #ccc; } /* Literal.Date */
-.pygments-style-vim .m { color: #cd00cd; } /* Literal.Number */
-.pygments-style-vim .s { color: #cd0000; } /* Literal.String */
-.pygments-style-vim .na { color: #ccc; } /* Name.Attribute */
-.pygments-style-vim .nb { color: #cd00cd; } /* Name.Builtin */
-.pygments-style-vim .nc { color: #00cdcd; } /* Name.Class */
-.pygments-style-vim .no { color: #ccc; } /* Name.Constant */
-.pygments-style-vim .nd { color: #ccc; } /* Name.Decorator */
-.pygments-style-vim .ni { color: #ccc; } /* Name.Entity */
-.pygments-style-vim .ne {
-  color: #669;
-  font-weight: bold;
-} /* Name.Exception */
-.pygments-style-vim .nf { color: #ccc; } /* Name.Function */
-.pygments-style-vim .nl { color: #ccc; } /* Name.Label */
-.pygments-style-vim .nn { color: #ccc; } /* Name.Namespace */
-.pygments-style-vim .nx { color: #ccc; } /* Name.Other */
-.pygments-style-vim .py { color: #ccc; } /* Name.Property */
-.pygments-style-vim .nt { color: #ccc; } /* Name.Tag */
-.pygments-style-vim .nv { color: #00cdcd; } /* Name.Variable */
-.pygments-style-vim .ow { color: #cdcd00; } /* Operator.Word */
-.pygments-style-vim .w { color: #ccc; } /* Text.Whitespace */
-.pygments-style-vim .mb { color: #cd00cd; } /* Literal.Number.Bin */
-.pygments-style-vim .mf { color: #cd00cd; } /* Literal.Number.Float */
-.pygments-style-vim .mh { color: #cd00cd; } /* Literal.Number.Hex */
-.pygments-style-vim .mi { color: #cd00cd; } /* Literal.Number.Integer */
-.pygments-style-vim .mo { color: #cd00cd; } /* Literal.Number.Oct */
-.pygments-style-vim .sa { color: #cd0000; } /* Literal.String.Affix */
-.pygments-style-vim .sb { color: #cd0000; } /* Literal.String.Backtick */
-.pygments-style-vim .sc { color: #cd0000; } /* Literal.String.Char */
-.pygments-style-vim .dl { color: #cd0000; } /* Literal.String.Delimiter */
-.pygments-style-vim .sd { color: #cd0000; } /* Literal.String.Doc */
-.pygments-style-vim .s2 { color: #cd0000; } /* Literal.String.Double */
-.pygments-style-vim .se { color: #cd0000; } /* Literal.String.Escape */
-.pygments-style-vim .sh { color: #cd0000; } /* Literal.String.Heredoc */
-.pygments-style-vim .si { color: #cd0000; } /* Literal.String.Interpol */
-.pygments-style-vim .sx { color: #cd0000; } /* Literal.String.Other */
-.pygments-style-vim .sr { color: #cd0000; } /* Literal.String.Regex */
-.pygments-style-vim .s1 { color: #cd0000; } /* Literal.String.Single */
-.pygments-style-vim .ss { color: #cd0000; } /* Literal.String.Symbol */
-.pygments-style-vim .bp { color: #cd00cd; } /* Name.Builtin.Pseudo */
-.pygments-style-vim .fm { color: #ccc; } /* Name.Function.Magic */
-.pygments-style-vim .vc { color: #00cdcd; } /* Name.Variable.Class */
-.pygments-style-vim .vg { color: #00cdcd; } /* Name.Variable.Global */
-.pygments-style-vim .vi { color: #00cdcd; } /* Name.Variable.Instance */
-.pygments-style-vim .vm { color: #00cdcd; } /* Name.Variable.Magic */
-.pygments-style-vim .il { color: #cd00cd; } /* Literal.Number.Integer.Long */
+.pygments-style-vim { background: #000; 
+color: #ccc }
+.pygments-style-vim .c { color: #000080 } /* Comment */
+.pygments-style-vim .err { color: #ccc; 
+border: 1px solid #F00 } /* Error */
+.pygments-style-vim .esc { color: #ccc } /* Escape */
+.pygments-style-vim .g { color: #ccc } /* Generic */
+.pygments-style-vim .k { color: #cdcd00 } /* Keyword */
+.pygments-style-vim .l { color: #ccc } /* Literal */
+.pygments-style-vim .n { color: #ccc } /* Name */
+.pygments-style-vim .o { color: #39c } /* Operator */
+.pygments-style-vim .x { color: #ccc } /* Other */
+.pygments-style-vim .p { color: #ccc } /* Punctuation */
+.pygments-style-vim .ch { color: #000080 } /* Comment.Hashbang */
+.pygments-style-vim .cm { color: #000080 } /* Comment.Multiline */
+.pygments-style-vim .cp { color: #000080 } /* Comment.Preproc */
+.pygments-style-vim .cpf { color: #000080 } /* Comment.PreprocFile */
+.pygments-style-vim .c1 { color: #000080 } /* Comment.Single */
+.pygments-style-vim .cs { color: #cd0000; 
+font-weight: bold } /* Comment.Special */
+.pygments-style-vim .gd { color: #cd0000 } /* Generic.Deleted */
+.pygments-style-vim .ge { color: #ccc; 
+font-style: italic } /* Generic.Emph */
+.pygments-style-vim .ges { color: #ccc; 
+font-weight: bold; 
+font-style: italic } /* Generic.EmphStrong */
+.pygments-style-vim .gr { color: #F00 } /* Generic.Error */
+.pygments-style-vim .gh { color: #000080; 
+font-weight: bold } /* Generic.Heading */
+.pygments-style-vim .gi { color: #00cd00 } /* Generic.Inserted */
+.pygments-style-vim .go { color: #888 } /* Generic.Output */
+.pygments-style-vim .gp { color: #000080; 
+font-weight: bold } /* Generic.Prompt */
+.pygments-style-vim .gs { color: #ccc; 
+font-weight: bold } /* Generic.Strong */
+.pygments-style-vim .gu { color: #800080; 
+font-weight: bold } /* Generic.Subheading */
+.pygments-style-vim .gt { color: #04D } /* Generic.Traceback */
+.pygments-style-vim .kc { color: #cdcd00 } /* Keyword.Constant */
+.pygments-style-vim .kd { color: #00cd00 } /* Keyword.Declaration */
+.pygments-style-vim .kn { color: #cd00cd } /* Keyword.Namespace */
+.pygments-style-vim .kp { color: #cdcd00 } /* Keyword.Pseudo */
+.pygments-style-vim .kr { color: #cdcd00 } /* Keyword.Reserved */
+.pygments-style-vim .kt { color: #00cd00 } /* Keyword.Type */
+.pygments-style-vim .ld { color: #ccc } /* Literal.Date */
+.pygments-style-vim .m { color: #cd00cd } /* Literal.Number */
+.pygments-style-vim .s { color: #cd0000 } /* Literal.String */
+.pygments-style-vim .na { color: #ccc } /* Name.Attribute */
+.pygments-style-vim .nb { color: #cd00cd } /* Name.Builtin */
+.pygments-style-vim .nc { color: #00cdcd } /* Name.Class */
+.pygments-style-vim .no { color: #ccc } /* Name.Constant */
+.pygments-style-vim .nd { color: #ccc } /* Name.Decorator */
+.pygments-style-vim .ni { color: #ccc } /* Name.Entity */
+.pygments-style-vim .ne { color: #669; 
+font-weight: bold } /* Name.Exception */
+.pygments-style-vim .nf { color: #ccc } /* Name.Function */
+.pygments-style-vim .nl { color: #ccc } /* Name.Label */
+.pygments-style-vim .nn { color: #ccc } /* Name.Namespace */
+.pygments-style-vim .nx { color: #ccc } /* Name.Other */
+.pygments-style-vim .py { color: #ccc } /* Name.Property */
+.pygments-style-vim .nt { color: #ccc } /* Name.Tag */
+.pygments-style-vim .nv { color: #00cdcd } /* Name.Variable */
+.pygments-style-vim .ow { color: #cdcd00 } /* Operator.Word */
+.pygments-style-vim .pm { color: #ccc } /* Punctuation.Marker */
+.pygments-style-vim .w { color: #ccc } /* Text.Whitespace */
+.pygments-style-vim .mb { color: #cd00cd } /* Literal.Number.Bin */
+.pygments-style-vim .mf { color: #cd00cd } /* Literal.Number.Float */
+.pygments-style-vim .mh { color: #cd00cd } /* Literal.Number.Hex */
+.pygments-style-vim .mi { color: #cd00cd } /* Literal.Number.Integer */
+.pygments-style-vim .mo { color: #cd00cd } /* Literal.Number.Oct */
+.pygments-style-vim .sa { color: #cd0000 } /* Literal.String.Affix */
+.pygments-style-vim .sb { color: #cd0000 } /* Literal.String.Backtick */
+.pygments-style-vim .sc { color: #cd0000 } /* Literal.String.Char */
+.pygments-style-vim .dl { color: #cd0000 } /* Literal.String.Delimiter */
+.pygments-style-vim .sd { color: #cd0000 } /* Literal.String.Doc */
+.pygments-style-vim .s2 { color: #cd0000 } /* Literal.String.Double */
+.pygments-style-vim .se { color: #cd0000 } /* Literal.String.Escape */
+.pygments-style-vim .sh { color: #cd0000 } /* Literal.String.Heredoc */
+.pygments-style-vim .si { color: #cd0000 } /* Literal.String.Interpol */
+.pygments-style-vim .sx { color: #cd0000 } /* Literal.String.Other */
+.pygments-style-vim .sr { color: #cd0000 } /* Literal.String.Regex */
+.pygments-style-vim .s1 { color: #cd0000 } /* Literal.String.Single */
+.pygments-style-vim .ss { color: #cd0000 } /* Literal.String.Symbol */
+.pygments-style-vim .bp { color: #cd00cd } /* Name.Builtin.Pseudo */
+.pygments-style-vim .fm { color: #ccc } /* Name.Function.Magic */
+.pygments-style-vim .vc { color: #00cdcd } /* Name.Variable.Class */
+.pygments-style-vim .vg { color: #00cdcd } /* Name.Variable.Global */
+.pygments-style-vim .vi { color: #00cdcd } /* Name.Variable.Instance */
+.pygments-style-vim .vm { color: #00cdcd } /* Name.Variable.Magic */
+.pygments-style-vim .il { color: #cd00cd } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/vs.css` & `plumage-4.0.0/plumage/static/css/pygments/vs.css`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,68 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
-.pygments-style-vs .hll { background-color: #ffc; }
+.pygments-style-vs .hll { background-color: #ffc }
 
-.pygments-style-vs {
-  background: #fff;
+.pygments-style-vs { background: #fff; 
 }
-.pygments-style-vs .c { color: #008000; } /* Comment */
-.pygments-style-vs .err { border: 1px solid #f00; } /* Error */
-.pygments-style-vs .k { color: #00f; } /* Keyword */
-.pygments-style-vs .ch { color: #008000; } /* Comment.Hashbang */
-.pygments-style-vs .cm { color: #008000; } /* Comment.Multiline */
-.pygments-style-vs .cp { color: #00f; } /* Comment.Preproc */
-.pygments-style-vs .cpf { color: #008000; } /* Comment.PreprocFile */
-.pygments-style-vs .c1 { color: #008000; } /* Comment.Single */
-.pygments-style-vs .cs { color: #008000; } /* Comment.Special */
-.pygments-style-vs .ge { font-style: italic; } /* Generic.Emph */
-.pygments-style-vs .gh { font-weight: bold; } /* Generic.Heading */
-.pygments-style-vs .gp { font-weight: bold; } /* Generic.Prompt */
-.pygments-style-vs .gs { font-weight: bold; } /* Generic.Strong */
-.pygments-style-vs .gu { font-weight: bold; } /* Generic.Subheading */
-.pygments-style-vs .kc { color: #00f; } /* Keyword.Constant */
-.pygments-style-vs .kd { color: #00f; } /* Keyword.Declaration */
-.pygments-style-vs .kn { color: #00f; } /* Keyword.Namespace */
-.pygments-style-vs .kp { color: #00f; } /* Keyword.Pseudo */
-.pygments-style-vs .kr { color: #00f; } /* Keyword.Reserved */
-.pygments-style-vs .kt { color: #2b91af; } /* Keyword.Type */
-.pygments-style-vs .s { color: #a31515; } /* Literal.String */
-.pygments-style-vs .nc { color: #2b91af; } /* Name.Class */
-.pygments-style-vs .ow { color: #00f; } /* Operator.Word */
-.pygments-style-vs .sa { color: #a31515; } /* Literal.String.Affix */
-.pygments-style-vs .sb { color: #a31515; } /* Literal.String.Backtick */
-.pygments-style-vs .sc { color: #a31515; } /* Literal.String.Char */
-.pygments-style-vs .dl { color: #a31515; } /* Literal.String.Delimiter */
-.pygments-style-vs .sd { color: #a31515; } /* Literal.String.Doc */
-.pygments-style-vs .s2 { color: #a31515; } /* Literal.String.Double */
-.pygments-style-vs .se { color: #a31515; } /* Literal.String.Escape */
-.pygments-style-vs .sh { color: #a31515; } /* Literal.String.Heredoc */
-.pygments-style-vs .si { color: #a31515; } /* Literal.String.Interpol */
-.pygments-style-vs .sx { color: #a31515; } /* Literal.String.Other */
-.pygments-style-vs .sr { color: #a31515; } /* Literal.String.Regex */
-.pygments-style-vs .s1 { color: #a31515; } /* Literal.String.Single */
-.pygments-style-vs .ss { color: #a31515; } /* Literal.String.Symbol */
+.pygments-style-vs .c { color: #008000 } /* Comment */
+.pygments-style-vs .err { border: 1px solid #F00 } /* Error */
+.pygments-style-vs .k { color: #00f } /* Keyword */
+.pygments-style-vs .ch { color: #008000 } /* Comment.Hashbang */
+.pygments-style-vs .cm { color: #008000 } /* Comment.Multiline */
+.pygments-style-vs .cp { color: #00f } /* Comment.Preproc */
+.pygments-style-vs .cpf { color: #008000 } /* Comment.PreprocFile */
+.pygments-style-vs .c1 { color: #008000 } /* Comment.Single */
+.pygments-style-vs .cs { color: #008000 } /* Comment.Special */
+.pygments-style-vs .ge { font-style: italic } /* Generic.Emph */
+.pygments-style-vs .ges { font-weight: bold; 
+font-style: italic } /* Generic.EmphStrong */
+.pygments-style-vs .gh { font-weight: bold } /* Generic.Heading */
+.pygments-style-vs .gp { font-weight: bold } /* Generic.Prompt */
+.pygments-style-vs .gs { font-weight: bold } /* Generic.Strong */
+.pygments-style-vs .gu { font-weight: bold } /* Generic.Subheading */
+.pygments-style-vs .kc { color: #00f } /* Keyword.Constant */
+.pygments-style-vs .kd { color: #00f } /* Keyword.Declaration */
+.pygments-style-vs .kn { color: #00f } /* Keyword.Namespace */
+.pygments-style-vs .kp { color: #00f } /* Keyword.Pseudo */
+.pygments-style-vs .kr { color: #00f } /* Keyword.Reserved */
+.pygments-style-vs .kt { color: #2b91af } /* Keyword.Type */
+.pygments-style-vs .s { color: #a31515 } /* Literal.String */
+.pygments-style-vs .nc { color: #2b91af } /* Name.Class */
+.pygments-style-vs .ow { color: #00f } /* Operator.Word */
+.pygments-style-vs .sa { color: #a31515 } /* Literal.String.Affix */
+.pygments-style-vs .sb { color: #a31515 } /* Literal.String.Backtick */
+.pygments-style-vs .sc { color: #a31515 } /* Literal.String.Char */
+.pygments-style-vs .dl { color: #a31515 } /* Literal.String.Delimiter */
+.pygments-style-vs .sd { color: #a31515 } /* Literal.String.Doc */
+.pygments-style-vs .s2 { color: #a31515 } /* Literal.String.Double */
+.pygments-style-vs .se { color: #a31515 } /* Literal.String.Escape */
+.pygments-style-vs .sh { color: #a31515 } /* Literal.String.Heredoc */
+.pygments-style-vs .si { color: #a31515 } /* Literal.String.Interpol */
+.pygments-style-vs .sx { color: #a31515 } /* Literal.String.Other */
+.pygments-style-vs .sr { color: #a31515 } /* Literal.String.Regex */
+.pygments-style-vs .s1 { color: #a31515 } /* Literal.String.Single */
+.pygments-style-vs .ss { color: #a31515 } /* Literal.String.Symbol */
```

### Comparing `plumage-3.1.0/plumage/static/css/pygments/xcode.css` & `plumage-4.0.0/plumage/static/css/pygments/rrt.css`

 * *Files 27% similar despite different names*

```diff
@@ -1,97 +1,108 @@
-pre {
-  line-height: 125%;
+pre { line-height: 125%; 
 }
 
-td.linenos pre {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
+td.linenos .normal { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-span.linenos {
-  color: #000;
-  background-color: #f0f0f0;
-  padding-left: 5px;
-  padding-right: 5px;
+span.linenos { color: inherit; 
+background-color: transparent; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-td.linenos pre.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
+td.linenos .special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
 
-span.linenos.special {
-  color: #000;
-  background-color: #ffffc0;
-  padding-left: 5px;
-  padding-right: 5px;
+span.linenos.special { color: #000; 
+background-color: #ffffc0; 
+padding-left: 5px; 
+padding-right: 5px; 
 }
-.pygments-style-xcode .hll { background-color: #ffc; }
+.pygments-style-rrt .hll { background-color: #00f }
 
-.pygments-style-xcode {
-  background: #fff;
-}
-.pygments-style-xcode .c { color: #177500; } /* Comment */
-.pygments-style-xcode .err { color: #000; } /* Error */
-.pygments-style-xcode .k { color: #a90d91; } /* Keyword */
-.pygments-style-xcode .l { color: #1c01ce; } /* Literal */
-.pygments-style-xcode .n { color: #000; } /* Name */
-.pygments-style-xcode .o { color: #000; } /* Operator */
-.pygments-style-xcode .ch { color: #177500; } /* Comment.Hashbang */
-.pygments-style-xcode .cm { color: #177500; } /* Comment.Multiline */
-.pygments-style-xcode .cp { color: #633820; } /* Comment.Preproc */
-.pygments-style-xcode .cpf { color: #177500; } /* Comment.PreprocFile */
-.pygments-style-xcode .c1 { color: #177500; } /* Comment.Single */
-.pygments-style-xcode .cs { color: #177500; } /* Comment.Special */
-.pygments-style-xcode .kc { color: #a90d91; } /* Keyword.Constant */
-.pygments-style-xcode .kd { color: #a90d91; } /* Keyword.Declaration */
-.pygments-style-xcode .kn { color: #a90d91; } /* Keyword.Namespace */
-.pygments-style-xcode .kp { color: #a90d91; } /* Keyword.Pseudo */
-.pygments-style-xcode .kr { color: #a90d91; } /* Keyword.Reserved */
-.pygments-style-xcode .kt { color: #a90d91; } /* Keyword.Type */
-.pygments-style-xcode .ld { color: #1c01ce; } /* Literal.Date */
-.pygments-style-xcode .m { color: #1c01ce; } /* Literal.Number */
-.pygments-style-xcode .s { color: #c41a16; } /* Literal.String */
-.pygments-style-xcode .na { color: #836c28; } /* Name.Attribute */
-.pygments-style-xcode .nb { color: #a90d91; } /* Name.Builtin */
-.pygments-style-xcode .nc { color: #3f6e75; } /* Name.Class */
-.pygments-style-xcode .no { color: #000; } /* Name.Constant */
-.pygments-style-xcode .nd { color: #000; } /* Name.Decorator */
-.pygments-style-xcode .ni { color: #000; } /* Name.Entity */
-.pygments-style-xcode .ne { color: #000; } /* Name.Exception */
-.pygments-style-xcode .nf { color: #000; } /* Name.Function */
-.pygments-style-xcode .nl { color: #000; } /* Name.Label */
-.pygments-style-xcode .nn { color: #000; } /* Name.Namespace */
-.pygments-style-xcode .nx { color: #000; } /* Name.Other */
-.pygments-style-xcode .py { color: #000; } /* Name.Property */
-.pygments-style-xcode .nt { color: #000; } /* Name.Tag */
-.pygments-style-xcode .nv { color: #000; } /* Name.Variable */
-.pygments-style-xcode .ow { color: #000; } /* Operator.Word */
-.pygments-style-xcode .mb { color: #1c01ce; } /* Literal.Number.Bin */
-.pygments-style-xcode .mf { color: #1c01ce; } /* Literal.Number.Float */
-.pygments-style-xcode .mh { color: #1c01ce; } /* Literal.Number.Hex */
-.pygments-style-xcode .mi { color: #1c01ce; } /* Literal.Number.Integer */
-.pygments-style-xcode .mo { color: #1c01ce; } /* Literal.Number.Oct */
-.pygments-style-xcode .sa { color: #c41a16; } /* Literal.String.Affix */
-.pygments-style-xcode .sb { color: #c41a16; } /* Literal.String.Backtick */
-.pygments-style-xcode .sc { color: #2300ce; } /* Literal.String.Char */
-.pygments-style-xcode .dl { color: #c41a16; } /* Literal.String.Delimiter */
-.pygments-style-xcode .sd { color: #c41a16; } /* Literal.String.Doc */
-.pygments-style-xcode .s2 { color: #c41a16; } /* Literal.String.Double */
-.pygments-style-xcode .se { color: #c41a16; } /* Literal.String.Escape */
-.pygments-style-xcode .sh { color: #c41a16; } /* Literal.String.Heredoc */
-.pygments-style-xcode .si { color: #c41a16; } /* Literal.String.Interpol */
-.pygments-style-xcode .sx { color: #c41a16; } /* Literal.String.Other */
-.pygments-style-xcode .sr { color: #c41a16; } /* Literal.String.Regex */
-.pygments-style-xcode .s1 { color: #c41a16; } /* Literal.String.Single */
-.pygments-style-xcode .ss { color: #c41a16; } /* Literal.String.Symbol */
-.pygments-style-xcode .bp { color: #5b269a; } /* Name.Builtin.Pseudo */
-.pygments-style-xcode .fm { color: #000; } /* Name.Function.Magic */
-.pygments-style-xcode .vc { color: #000; } /* Name.Variable.Class */
-.pygments-style-xcode .vg { color: #000; } /* Name.Variable.Global */
-.pygments-style-xcode .vi { color: #000; } /* Name.Variable.Instance */
-.pygments-style-xcode .vm { color: #000; } /* Name.Variable.Magic */
-.pygments-style-xcode .il { color: #1c01ce; } /* Literal.Number.Integer.Long */
+.pygments-style-rrt { background: #000; 
+color: #ddd }
+.pygments-style-rrt .c { color: #0f0 } /* Comment */
+.pygments-style-rrt .err { color: #ddd } /* Error */
+.pygments-style-rrt .esc { color: #ddd } /* Escape */
+.pygments-style-rrt .g { color: #ddd } /* Generic */
+.pygments-style-rrt .k { color: #f00 } /* Keyword */
+.pygments-style-rrt .l { color: #ddd } /* Literal */
+.pygments-style-rrt .n { color: #ddd } /* Name */
+.pygments-style-rrt .o { color: #ddd } /* Operator */
+.pygments-style-rrt .x { color: #ddd } /* Other */
+.pygments-style-rrt .p { color: #ddd } /* Punctuation */
+.pygments-style-rrt .ch { color: #0f0 } /* Comment.Hashbang */
+.pygments-style-rrt .cm { color: #0f0 } /* Comment.Multiline */
+.pygments-style-rrt .cp { color: #e5e5e5 } /* Comment.Preproc */
+.pygments-style-rrt .cpf { color: #0f0 } /* Comment.PreprocFile */
+.pygments-style-rrt .c1 { color: #0f0 } /* Comment.Single */
+.pygments-style-rrt .cs { color: #0f0 } /* Comment.Special */
+.pygments-style-rrt .gd { color: #ddd } /* Generic.Deleted */
+.pygments-style-rrt .ge { color: #ddd } /* Generic.Emph */
+.pygments-style-rrt .ges { color: #ddd } /* Generic.EmphStrong */
+.pygments-style-rrt .gr { color: #ddd } /* Generic.Error */
+.pygments-style-rrt .gh { color: #ddd } /* Generic.Heading */
+.pygments-style-rrt .gi { color: #ddd } /* Generic.Inserted */
+.pygments-style-rrt .go { color: #ddd } /* Generic.Output */
+.pygments-style-rrt .gp { color: #ddd } /* Generic.Prompt */
+.pygments-style-rrt .gs { color: #ddd } /* Generic.Strong */
+.pygments-style-rrt .gu { color: #ddd } /* Generic.Subheading */
+.pygments-style-rrt .gt { color: #ddd } /* Generic.Traceback */
+.pygments-style-rrt .kc { color: #f00 } /* Keyword.Constant */
+.pygments-style-rrt .kd { color: #f00 } /* Keyword.Declaration */
+.pygments-style-rrt .kn { color: #f00 } /* Keyword.Namespace */
+.pygments-style-rrt .kp { color: #f00 } /* Keyword.Pseudo */
+.pygments-style-rrt .kr { color: #f00 } /* Keyword.Reserved */
+.pygments-style-rrt .kt { color: #ee82ee } /* Keyword.Type */
+.pygments-style-rrt .ld { color: #ddd } /* Literal.Date */
+.pygments-style-rrt .m { color: #f0f } /* Literal.Number */
+.pygments-style-rrt .s { color: #87ceeb } /* Literal.String */
+.pygments-style-rrt .na { color: #ddd } /* Name.Attribute */
+.pygments-style-rrt .nb { color: #ddd } /* Name.Builtin */
+.pygments-style-rrt .nc { color: #ddd } /* Name.Class */
+.pygments-style-rrt .no { color: #7fffd4 } /* Name.Constant */
+.pygments-style-rrt .nd { color: #ddd } /* Name.Decorator */
+.pygments-style-rrt .ni { color: #ddd } /* Name.Entity */
+.pygments-style-rrt .ne { color: #ddd } /* Name.Exception */
+.pygments-style-rrt .nf { color: #ff0 } /* Name.Function */
+.pygments-style-rrt .nl { color: #ddd } /* Name.Label */
+.pygments-style-rrt .nn { color: #ddd } /* Name.Namespace */
+.pygments-style-rrt .nx { color: #ddd } /* Name.Other */
+.pygments-style-rrt .py { color: #ddd } /* Name.Property */
+.pygments-style-rrt .nt { color: #ddd } /* Name.Tag */
+.pygments-style-rrt .nv { color: #eedd82 } /* Name.Variable */
+.pygments-style-rrt .ow { color: #ddd } /* Operator.Word */
+.pygments-style-rrt .pm { color: #ddd } /* Punctuation.Marker */
+.pygments-style-rrt .w { color: #ddd } /* Text.Whitespace */
+.pygments-style-rrt .mb { color: #f0f } /* Literal.Number.Bin */
+.pygments-style-rrt .mf { color: #f0f } /* Literal.Number.Float */
+.pygments-style-rrt .mh { color: #f0f } /* Literal.Number.Hex */
+.pygments-style-rrt .mi { color: #f0f } /* Literal.Number.Integer */
+.pygments-style-rrt .mo { color: #f0f } /* Literal.Number.Oct */
+.pygments-style-rrt .sa { color: #87ceeb } /* Literal.String.Affix */
+.pygments-style-rrt .sb { color: #87ceeb } /* Literal.String.Backtick */
+.pygments-style-rrt .sc { color: #87ceeb } /* Literal.String.Char */
+.pygments-style-rrt .dl { color: #87ceeb } /* Literal.String.Delimiter */
+.pygments-style-rrt .sd { color: #87ceeb } /* Literal.String.Doc */
+.pygments-style-rrt .s2 { color: #87ceeb } /* Literal.String.Double */
+.pygments-style-rrt .se { color: #87ceeb } /* Literal.String.Escape */
+.pygments-style-rrt .sh { color: #87ceeb } /* Literal.String.Heredoc */
+.pygments-style-rrt .si { color: #87ceeb } /* Literal.String.Interpol */
+.pygments-style-rrt .sx { color: #87ceeb } /* Literal.String.Other */
+.pygments-style-rrt .sr { color: #87ceeb } /* Literal.String.Regex */
+.pygments-style-rrt .s1 { color: #87ceeb } /* Literal.String.Single */
+.pygments-style-rrt .ss { color: #87ceeb } /* Literal.String.Symbol */
+.pygments-style-rrt .bp { color: #ddd } /* Name.Builtin.Pseudo */
+.pygments-style-rrt .fm { color: #ff0 } /* Name.Function.Magic */
+.pygments-style-rrt .vc { color: #eedd82 } /* Name.Variable.Class */
+.pygments-style-rrt .vg { color: #eedd82 } /* Name.Variable.Global */
+.pygments-style-rrt .vi { color: #eedd82 } /* Name.Variable.Instance */
+.pygments-style-rrt .vm { color: #eedd82 } /* Name.Variable.Magic */
+.pygments-style-rrt .il { color: #f0f } /* Literal.Number.Integer.Long */
```

### Comparing `plumage-3.1.0/plumage/static/favicon/android-chrome-192x192.png` & `plumage-4.0.0/plumage/static/favicon/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `plumage-3.1.0/plumage/static/favicon/android-chrome-512x512.png` & `plumage-4.0.0/plumage/static/favicon/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `plumage-3.1.0/plumage/static/favicon/apple-touch-icon.png` & `plumage-4.0.0/plumage/static/favicon/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `plumage-3.1.0/plumage/static/favicon/favicon.ico` & `plumage-4.0.0/plumage/static/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `plumage-3.1.0/plumage/static/favicon/mstile-144x144.png` & `plumage-4.0.0/plumage/static/favicon/mstile-144x144.png`

 * *Files identical despite different names*

### Comparing `plumage-3.1.0/plumage/static/favicon/mstile-150x150.png` & `plumage-4.0.0/plumage/static/favicon/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `plumage-3.1.0/plumage/static/favicon/mstile-310x150.png` & `plumage-4.0.0/plumage/static/favicon/mstile-310x150.png`

 * *Files identical despite different names*

### Comparing `plumage-3.1.0/plumage/static/favicon/mstile-310x310.png` & `plumage-4.0.0/plumage/static/favicon/mstile-310x310.png`

 * *Files identical despite different names*

### Comparing `plumage-3.1.0/plumage/static/favicon/mstile-70x70.png` & `plumage-4.0.0/plumage/static/favicon/mstile-70x70.png`

 * *Files identical despite different names*

### Comparing `plumage-3.1.0/plumage/static/favicon/safari-pinned-tab.svg` & `plumage-4.0.0/plumage/static/favicon/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `plumage-3.1.0/plumage/static/img/creampaper.jpeg` & `plumage-4.0.0/plumage/static/img/creampaper.jpeg`

 * *Files identical despite different names*

### Comparing `plumage-3.1.0/plumage/static/img/fabric_plaid.jpeg` & `plumage-4.0.0/plumage/static/img/fabric_plaid.jpeg`

 * *Files identical despite different names*

### Comparing `plumage-3.1.0/plumage/static/img/feather-alt-solid.svg` & `plumage-4.0.0/plumage/static/img/feather-alt-solid.svg`

 * *Files identical despite different names*

### Comparing `plumage-3.1.0/plumage/static/img/magnifier.png` & `plumage-4.0.0/plumage/static/img/magnifier.png`

 * *Files identical despite different names*

### Comparing `plumage-3.1.0/plumage/static/img/play-button.png` & `plumage-4.0.0/plumage/static/img/play-button.png`

 * *Files identical despite different names*

### Comparing `plumage-3.1.0/plumage/static/js/application.js` & `plumage-4.0.0/plumage/static/js/application.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -30,16 +30,16 @@
         // YouTube URL parser. Source: https://stackoverflow.com/questions/2964678/jquery-youtube-url-validation-with-regex/10315969#10315969
         function parse_youtube_url(url) {
             var p = /^(?:https?:\/\/)?(?:www\.)?(?:youtu\.be\/|youtube\.com\/(?:embed\/|v\/|watch\?v=|watch\?.+&v=))((\w|-){11})(?:\S+)?$/;
             return (url.match(p)) ? RegExp.$1 : false;
         };
 
         // Activate zoom on content images in the main column and add an icon overlay
-        // (but ignore link icons from the footer and emoji).
-        $("#content img:not(.link-icon,.emojione)").each(function() {
+        // (but ignore link icons from the footer).
+        $("#content img:not(.link-icon)").each(function() {
             // Until we properly generate thumbnails and their links on Pelican's side, we just link an image to itself.
             if ($(this).parents('a').length == 0) {
                 $(this).wrap(
                     $('<a/>').attr('href', $(this).attr('src'))
                 );
             };
             // Add a special class for images linking to videos
```

### Comparing `plumage-3.1.0/plumage/static/js/jquery.mglass.js` & `plumage-4.0.0/plumage/static/js/jquery.mglass.js`

 * *Files identical despite different names*

### Comparing `plumage-3.1.0/plumage/templates/archives.html` & `plumage-4.0.0/plumage/templates/archives.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 {% extends "base.html" %}
-{% block title %}Archives{% endblock %}
+{% block title %}Archives{% endblock title %}
 {% block top_center %}
     <h1>
         <a href="{{ SITEURL }}/{{ ARCHIVES_SAVE_AS }}"
            rel="bookmark"
            title="Permalink to archives">Archives</a>
     </h1>
-{% endblock %}
+{% endblock top_center %}
 {% block content %}
     {# Compute the spanning years all articles covers #}
     {% set year_range = [] %}
     {% for year in range(dates[-1].date.year, dates[0].date.year + 1) %}
         {# Gather all articles from current year #}
         {% set yearly_articles = [] %}
         {% for article in dates %}
@@ -22,15 +22,15 @@
         {# Ignore empty years #}
         {% if yearly_articles|length > 0 %}
             {% if year_range.append({'year': year, 'articles': yearly_articles}) %}
             {% endif %}
         {% endif %}
     {% endfor %}
     <div class="accordion"
-         id="accordianArchives"
+         id="accordionArchives"
          role="tablist"
          aria-multiselectable="true">
         {% for yearly_group in year_range|sort(reverse = True, attribute = 'year')  %}
             <div class="card">
                 <h4 class="card-header" role="tab" id="heading{{ yearly_group.year }}">
                     <button type="button"
                             data-bs-toggle="collapse"
@@ -43,30 +43,30 @@
                         <span class="visually-hidden">articles</span>
                     </button>
                 </h4>
                 <div id="collapse{{ yearly_group.year }}"
                      class="collapse {% if loop.first %}show{% endif %}"
                      role="tabpanel"
                      aria-labelledby="heading{{ yearly_group.year }}"
-                     data-bs-parent="#accordianArchives">
+                     data-bs-parent="#accordionArchives">
                     <div class="card-body">
                         {% set current_month = False %}
                         {% for article in yearly_group.articles %}
                             {% if article.date.month != current_month %}
                                 {% set current_month = article.date.month %}
                                 {% if not loop.first %}</dl>{% endif %}
                                 <dl class="row">
-                                {% endif %}
-                                <dt class="col-sm-2">
-                                    <abbr class="published" title="{{ article.date.isoformat() }}">{{ article.date.strftime('%b. %d') }}</abbr>
-                                </dt>
-                                <dd class="col-sm-10">
-                                    <a href="{{ SITEURL }}/{{ article.url }}">{{ article.title }}</a>
-                                </dd>
-                                {% if loop.last %}</dl>{% endif %}
-                            {% endfor %}
-                        </div>
+                            {% endif %}
+                            <dt class="col-sm-2">
+                                <abbr class="published" title="{{ article.date.isoformat() }}">{{ article.date.strftime('%b. %d') }}</abbr>
+                            </dt>
+                            <dd class="col-sm-10">
+                                <a href="{{ SITEURL }}/{{ article.url }}">{{ article.title }}</a>
+                            </dd>
+                            {% if loop.last %}</dl>{% endif %}
+                        {% endfor %}
                     </div>
                 </div>
-            {% endfor %}
-        </div>
-    {% endblock %}
+            </div>
+        {% endfor %}
+    </div>
+{% endblock content %}
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-{% extends "base.html" %} {% block title %}Archives{% endblock %} {% block
-top_center %}
+{% extends "base.html" %} {% block title %}Archives{% endblock title %} {%
+block top_center %}
 ************ _AA_rr_cc_hh_ii_vv_ee_ss ************
-{% endblock %} {% block content %} {# Compute the spanning years all articles
-covers #} {% set year_range = [] %} {% for year in range(dates[-1].date.year,
-dates[0].date.year + 1) %} {# Gather all articles from current year #} {% set
-yearly_articles = [] %} {% for article in dates %} {% if article.date.year ==
-year %} {% if yearly_articles.append(article) %} {% endif %} {% endif %} {%
-endfor %} {# Ignore empty years #} {% if yearly_articles|length > 0 %} {% if
-year_range.append({'year': year, 'articles': yearly_articles}) %} {% endif %}
-{% endif %} {% endfor %}
+{% endblock top_center %} {% block content %} {# Compute the spanning years all
+articles covers #} {% set year_range = [] %} {% for year in range(dates[-
+1].date.year, dates[0].date.year + 1) %} {# Gather all articles from current
+year #} {% set yearly_articles = [] %} {% for article in dates %} {% if
+article.date.year == year %} {% if yearly_articles.append(article) %} {% endif
+%} {% endif %} {% endfor %} {# Ignore empty years #} {% if
+yearly_articles|length > 0 %} {% if year_range.append({'year': year,
+'articles': yearly_articles}) %} {% endif %} {% endif %} {% endfor %}
 {% for yearly_group in year_range|sort(reverse = True, attribute = 'year') %}
 ****** {{{{ yyeeaarrllyy__ggrroouupp..yyeeaarr }}}} {{{{ yyeeaarrllyy__ggrroouupp..aarrttiicclleess||lleennggtthh }}}} aarrttiicclleess ******
 {% set current_month = False %} {% for article in yearly_group.articles %} {%
 if article.date.month != current_month %} {% set current_month =
 article.date.month %} {% if not loop.first %}
 {% endif %}
 {% endif %}
 {% endif %} {% endfor %}
 {% endfor %}
-{% endblock %}
+{% endblock content %}
```

### Comparing `plumage-3.1.0/plumage/templates/article.html` & `plumage-4.0.0/plumage/templates/article.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,102 +1,94 @@
 {% extends "base.html" %}
 {% set has_right = True %}
-{% block title %}{{ article.title|striptags|e }}{% endblock %}
+{% block title %}{{ article.title|striptags|e }}{% endblock title %}
 {% block head %}
-    {% if article.tags %}<meta name="keywords"
-      content="{{ article.tags|join(', ', attribute='name')|e }}">{% endif %}
-{% endblock %}
+    {% if article.tags %}
+        <meta name="keywords"
+              content="{{ article.tags|join(', ', attribute='name') |e }}">
+    {% endif %}
+{% endblock head %}
 {% block top_center %}
     <h1>
         <a href="{{ SITEURL }}/{{ article.url }}"
            rel="bookmark"
            title="Permalink to {{ article.title|striptags|e }}">{{ article.title }}</a>
     </h1>
-{% endblock %}
+{% endblock top_center %}
 {% block right_sidebar %}
-
-        <ul class="list-group list-group-flush list-group-item-dark small fw-light">
-            <li class="list-group-item bg-transparent">
-                <abbr title="{{ article.date.isoformat() }}"><i class="fas fa-calendar"></i> {{ article.locale_date }}</abbr>
+    <ul class="list-group list-group-flush">
+        <li class="list-group-item">
+            <abbr title="{{ article.date.isoformat() }}">
+                <i class="bi bi-calendar-event-fill"></i>
+                {{ article.locale_date }}
+            </abbr>
+        </li>
+        {% if AUTHOR_SAVE_AS and article.authors %}
+            <li class="list-group-item">
+                <address>
+                    <i class="bi bi-person-circle"></i> By
+                    {% for author in article.authors %}
+                        <a href="{{ SITEURL }}/{{ author.url }}" rel="author">{{ author.name }}</a>
+                    {% endfor %}
+                </address>
             </li>
-            {% if AUTHOR_SAVE_AS and article.authors %}
-                <li class="list-group-item bg-transparent">
-                    <address>
-                        <i class="fas fa-user"></i> By
-                        {% for author in article.authors %}
-                            <a href="{{ SITEURL }}/{{ author.url }}" rel="author">{{ author.name }}</a>
+        {% endif %}
+        {% if article.category or article.tags %}
+            <li class="list-group-item">
+                <ul class="list-inline">
+                    {% if article.category %}
+                        {% for category, articles in categories %}
+                            {% if category.url == article.category.url %}
+                                <li class="list-inline-item">{{ m.render_tag(category, counter=articles|length() , kind='category') }}</li>
+                            {% endif %}
                         {% endfor %}
-                    </address>
-                </li>
-            {% endif %}
-            {% if article.category or article.tags %}
-                <li class="list-group-item bg-transparent">
-                    <ul class="list-inline">
-                        {% if article.category %}
-                            {% for category, articles in categories %}
-                                {% if category.url == article.category.url %}
-                                    {% set article_counter = articles|length() %}
-                                    <li class="list-inline-item">
-                                        <a href="{{ SITEURL }}/{{ article.category.url }}"
-                                           rel="tag"
-                                           class="badge text-bg-info"
-                                           data-bs-toggle="tooltip"
-                                           title="{{ article_counter }} article{{ 's' if article_counter > 1 else '' }} in this category">
-                                                {{ article.category }}
-                                        </a>
-                                    </li>
+                    {% endif %}
+                    {% if article.tags %}
+                        {% set article_tags = [] %}
+                        {% for tag, articles in tags %}
+                            {% for t in article.tags %}
+                                {% if tag.url == t.url %}
+                                    {% if article_tags.append({'name': tag.name, 'url': tag.url, 'articles': articles|length()}) %}{% endif %}
                                 {% endif %}
                             {% endfor %}
-                        {% endif %}
-                        {% if article.tags %}
-                            {% set article_tags = [] %}
-                            {% for tag, articles in tags %}
-                                {% for t in article.tags %}
-                                    {% if tag.url == t.url %}
-                                        {% if article_tags.append({'name': tag.name, 'url': tag.url, 'articles': articles|length()}) %}
-                                        {% endif %}
-                                    {% endif %}
-                                {% endfor %}
-                            {% endfor %}
-                            {# Sort by tag frequency, then alphabetically #}
-                            {% for tag in article_tags|sort(attribute='name')|sort(reverse=True, attribute='articles') %}
-                                <li class="list-inline-item">
-                                    {{ m.render_tag(tag) }}
-                                </li>
-                            {% endfor %}
-                        {% endif %}
-                    </ul>
-                </li>
-            {% endif %}
-            {% if ARTICLE_EDIT_LINK %}
-                <li class="list-group-item bg-transparent text-center">
-                    Found a typo? Fix it now:<br/>
-                    <a class="btn btn-outline-info btn-sm border-0 d-block stretched-link"
-                       href="{{ ARTICLE_EDIT_LINK % {'slug': article.slug} }}"><i class="fas fa-edit fa-fw"></i> Edit article on GitHub</a>
-                </li>
-            {% endif %}
-            {% if article.prev_article or article.next_article %}
-                <li class="list-group-item bg-transparent">
-                    <nav class="nav nav-pills nav-fill">
-                        <a class="nav-link btn btn-outline-primary border-0 {% if not article.prev_article %} disabled{% endif %}"
-                           {% if article.prev_article %} href="{{ SITEURL }}/{{ article.prev_article.url }}" title="{{ article.prev_article.title|striptags|e }}" {% endif %}
-                           rel="prev">
-                            <span aria-hidden="true">←</span> Older
-                        </a>
-                        <a class="nav-link btn btn-outline-primary border-0 {% if not article.next_article %} disabled{% endif %}"
-                           {% if article.next_article %} href="{{ SITEURL }}/{{ article.next_article.url }}" title="{{ article.next_article.title|striptags|e }}" {% endif %}
-                           rel="next">
-                            Newer <span aria-hidden="true">→</span>
-                        </a>
-                    </nav>
-                </li>
-            {% endif %}
-        </ul>
-
-{% endblock %}
+                        {% endfor %}
+                        {# Sort by tag frequency, then alphabetically #}
+                        {% for tag in article_tags|sort(attribute='name')|sort(reverse=True, attribute='articles') %}
+                            <li class="list-inline-item">{{ m.render_tag(tag, counter=articles|length() ) }}</li>
+                        {% endfor %}
+                    {% endif %}
+                </ul>
+            </li>
+        {% endif %}
+        {% if ARTICLE_EDIT_LINK %}
+            <li class="list-group-item">
+                Found a typo? Fix it now:
+                <br />
+                <a href="{{ ARTICLE_EDIT_LINK % {'slug': article.slug} }}">
+                    <i class="bi bi-pencil-square"></i> Edit article on GitHub</a>
+            </li>
+        {% endif %}
+        {% if article.prev_article or article.next_article %}
+            <li class="list-group-item">
+                <nav class="nav nav-underline nav-justified">
+                    <a class="nav-link {% if not article.prev_article %}disabled{% endif %}"
+                       {% if article.prev_article %} href="{{ SITEURL }}/{{ article.prev_article.url }}" title="{{ article.prev_article.title|striptags|e }}" {% endif %}
+                       rel="prev">
+                        <span aria-hidden="true">←</span> Older
+                    </a>
+                    <a class="nav-link {% if not article.next_article %}disabled{% endif %}"
+                       {% if article.next_article %} href="{{ SITEURL }}/{{ article.next_article.url }}" title="{{ article.next_article.title|striptags|e }}" {% endif %}
+                       rel="next">
+                        Newer <span aria-hidden="true">→</span>
+                    </a>
+                </nav>
+            </li>
+        {% endif %}
+    </ul>
+{% endblock right_sidebar %}
 {% block content %}
     {% import 'translations.html' as translations with context %}
     {{ translations.translations_for(article) }}
     {{ article.content }}
     {# Fetch content related to the current article from either related-posts
     or simila-posts plugin. The latter teakes precedence as it produces more
     robust results. #}
@@ -113,15 +105,15 @@
         <div class="list-group bg-body-tertiary">
             {% for related_post in related %}
                 <a class="list-group-item list-group-item-action"
                    href="{{ SITEURL }}/{{ related_post.url }}">
                     <div class="d-flex w-100 justify-content-between">
                         <h5>{{ related_post.title }}</h5>
                         <abbr class="small published" title="{{ related_post.date.isoformat() }}">
-                            {{ related_post.date.strftime('%Y') }}
+                            {{ related_post.date.strftime("%Y") }}
                         </abbr>
                     </div>
                     <small>{{ related_post.summary|striptags|e }}</small>
                 </a>
             {% endfor %}
         </div>
     {% endif %}
@@ -140,8 +132,8 @@
                     s.setAttribute('data-timestamp', +new Date());
                     (d.head || d.body).appendChild(s);
                 })();
             </script>
             <noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus</a>.</noscript>
         </div>
     {% endif %}
-{% endblock %}
+{% endblock content %}
```

### Comparing `plumage-3.1.0/plumage/templates/authors.html` & `plumage-4.0.0/plumage/templates/authors.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 {% extends "base.html" %}
-{% block title %}All authors{% endblock %}
+{% block title %}All authors{% endblock title %}
 {% block top_center %}
     <h1>
         <a href="{{ SITEURL }}/{{ AUTHORS_SAVE_AS }}"
            rel="bookmark"
            title="Permalink to author list">Authors</a>
     </h1>
-{% endblock %}
+{% endblock top_center %}
 {% block content %}
     {% set all_authors = [] %}
     {% for author, articles in authors %}
         {% if all_authors.append({'name': author.name, 'url': author.url, 'articles': articles|length()}) %}
         {% endif %}
     {% endfor %}
     <dl class="row">
@@ -20,8 +20,8 @@
                 <a href="{{ SITEURL }}/{{ author.url }}" class="badge text-bg-info">{{ author.name }}</a>
             </dt>
             <dd class="col-sm-10">
                 <a href="{{ SITEURL }}/{{ author.url }}">{{ author.articles }} article{{ 's' if author.articles > 1 else '' }}</a>
             </dd>
         {% endfor %}
     </dl>
-{% endblock %}
+{% endblock content %}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-{% extends "base.html" %} {% block title %}All authors{% endblock %} {% block
-top_center %}
+{% extends "base.html" %} {% block title %}All authors{% endblock title %} {%
+block top_center %}
 ************ _AA_uu_tt_hh_oo_rr_ss ************
-{% endblock %} {% block content %} {% set all_authors = [] %} {% for author,
-articles in authors %} {% if all_authors.append({'name': author.name, 'url':
-author.url, 'articles': articles|length()}) %} {% endif %} {% endfor %}
+{% endblock top_center %} {% block content %} {% set all_authors = [] %} {% for
+author, articles in authors %} {% if all_authors.append({'name': author.name,
+'url': author.url, 'articles': articles|length()}) %} {% endif %} {% endfor %}
 {# Sort by number of articles, then alphabetically #} {% for author in
 all_authors|sort(attribute='name')|sort(reverse=True, attribute='articles') %}
-{% endblock %}
+{% endblock content %}
```

### Comparing `plumage-3.1.0/plumage/templates/base.html` & `plumage-4.0.0/plumage/templates/base.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!doctype html>
+<!DOCTYPE html>
 {% import 'macros.html' as m %}
 <html lang="{{ DEFAULT_LANG }}">
     <head>
         <meta charset="utf-8" />
         <meta http-equiv="X-UA-Compatible" content="IE=edge">
         <meta name="viewport" content="width=device-width, initial-scale=1">
         {% if (page in hidden_articles) or (page in drafts) or (page in hidden_pages) or (page in draft_pages) %}
@@ -18,64 +18,63 @@
         <meta name="author" content="{{ AUTHOR|e }}" />
         <meta name="generator" content="Pelican v{{ PELICAN_VERSION }}" />
         {% assets filters="libsass,postcss,cssmin", output="css/main.min.css",
             "css/mglass.scss", "css/main.scss", "css/pygments/" + CODE_STYLE + ".css", "css/code.scss" %}
             <link rel="stylesheet" href="{{ SITEURL }}/{{ ASSET_URL }}" />
         {% endassets %}
         <link rel="stylesheet"
-              href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css"
-              integrity="sha512-SzlrxWUlpfuzQ+pcUCosxcglQRNAq/DZjVsC0lE40xsADsfeQoEypE+enwcOiGjk/bSuGGKHEyjSoQ1zVisanQ=="
+              href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap-icons/1.11.3/font/bootstrap-icons.min.css"
+              integrity="sha512-dPXYcDub/aeb08c63jRq/k6GaKccl256JQy/AnOq7CAnEZ9FzSL9wSbcZkMp4R26vBsMLFYH4kQ67/bbV8XaCQ=="
               crossorigin="anonymous"
-              referrerpolicy="no-referrer"/>
+              referrerpolicy="no-referrer" />
         <link rel="stylesheet"
               href="https://cdnjs.cloudflare.com/ajax/libs/magnific-popup.js/1.1.0/magnific-popup.min.css"
               integrity="sha512-+EoPw+Fiwh6eSeRK7zwIKG2MA8i3rV/DGa3tdttQGgWyatG/SkncT53KHQaS5Jh9MNOT3dmFL0FjTY08And/Cw=="
               crossorigin="anonymous"
-              referrerpolicy="no-referrer"/>
-        {% block extra_css %}{% endblock %}
+              referrerpolicy="no-referrer" />
+        {% block extra_css %}
+        {% endblock extra_css %}
         {% include "analytics.html" %}
-        <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.3/jquery.min.js"
-                integrity="sha512-STof4xm1wgkfm7heWqFJVn58Hm3EtS31XFaagaa8VMReCXAkQnJZ+jEy8PCC/iT18dFy95WcExNHFTqLyp72eQ=="
+        <!-- TODO: move scripts to the bottom of the page, as per Bootstrap canonical example -->
+        <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.7.1/jquery.min.js"
+                integrity="sha512-v2CJ7UaYy4JwqLDIrZUI/4hqeoQieOmAZNXBeQyjo21dadnwR+8ZaIJVT8EE2iyI61OV8e6M8PP2/4hpQINQ/g=="
                 crossorigin="anonymous"
                 referrerpolicy="no-referrer"></script>
-        <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.0-alpha1/js/bootstrap.bundle.min.js"
-                integrity="sha512-Sct/LCTfkoqr7upmX9VZKEzXuRk5YulFoDTunGapYJdlCwA+Rl4RhgcPCLf7awTNLmIVrszTPNUFu4MSesep5Q=="
+        <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.3/js/bootstrap.bundle.min.js"
+                integrity="sha512-7Pi/otdlbbCR+LnW+F7PwFcSDJOuUJB3OxtEHbg4vSMvzvJjde4Po1v4BR9Gdc9aXNUNFVUY+SK51wWT8WF0Gg=="
                 crossorigin="anonymous"
                 referrerpolicy="no-referrer"></script>
         <script src="https://cdnjs.cloudflare.com/ajax/libs/magnific-popup.js/1.1.0/jquery.magnific-popup.min.js"
                 integrity="sha512-IsNh5E3eYy3tr/JiX2Yx4vsCujtkhwl7SLqgnwLNgf04Hrt9BT9SXlLlZlWx+OK4ndzAoALhsMNcCmkggjZB1w=="
                 crossorigin="anonymous"></script>
         {% assets filters="closure_js", output="js/main.min.js", "js/jquery.mglass.js", "js/application.js" %}
             <script src="{{ SITEURL }}/{{ ASSET_URL }}"></script>
         {% endassets %}
-        {% block extra_js %}{% endblock %}
+        {% block extra_js %}
+        {% endblock extra_js %}
         <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
         <link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
         <link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
         <link rel="manifest" href="/site.webmanifest">
         <link rel="mask-icon" href="/safari-pinned-tab.svg" color="#5bbad5">
         <meta name="msapplication-TileColor" content="#ffc40d">
         <meta name="theme-color" content="#ffffff">
         <!-- Feeds -->
         {% set all_feeds = [] %}
         {% if FEED_ALL_ATOM %}
-            {% if all_feeds.append({'kind': 'Atom', 'url': FEED_ALL_ATOM, 'name': 'All posts'}) %}
-            {% endif %}
+            {% if all_feeds.append({'kind': 'Atom', 'url': FEED_ALL_ATOM, 'name': 'All posts'}) %}{% endif %}
         {% endif %}
         {% if FEED_ALL_RSS %}
-            {% if all_feeds.append({'kind': 'RSS', 'url': FEED_ALL_RSS, 'name': 'All posts'}) %}
-            {% endif %}
+            {% if all_feeds.append({'kind': 'RSS', 'url': FEED_ALL_RSS, 'name': 'All posts'}) %}{% endif %}
         {% endif %}
         {% if FEED_ATOM %}
-            {% if all_feeds.append({'kind': 'Atom', 'url': FEED_ATOM, 'name': 'Latest posts'}) %}
-            {% endif %}
+            {% if all_feeds.append({'kind': 'Atom', 'url': FEED_ATOM, 'name': 'Latest posts'}) %}{% endif %}
         {% endif %}
         {% if FEED_RSS %}
-            {% if all_feeds.append({'kind': 'RSS', 'url': FEED_RSS, 'name': 'Latest posts'}) %}
-            {% endif %}
+            {% if all_feeds.append({'kind': 'RSS', 'url': FEED_RSS, 'name': 'Latest posts'}) %}{% endif %}
         {% endif %}
         {% if CATEGORY_FEED_ATOM and category is defined %}
             {% if all_feeds.append({'kind': 'Atom', 'url': CATEGORY_FEED_ATOM.format(slug=category.slug), 'name': 'Category: ' + category.name}) %}
             {% endif %}
         {% endif %}
         {% if CATEGORY_FEED_RSS and category is defined %}
             {% if all_feeds.append({'kind': 'RSS', 'url': CATEGORY_FEED_RSS.format(slug=category.slug), 'name': 'Category: ' + category.name}) %}
@@ -89,28 +88,31 @@
             {% if all_feeds.append({'kind': 'RSS', 'url': TAG_FEED_RSS.format(slug=tag.slug), 'name': 'Tag: ' + tag.name}) %}
             {% endif %}
         {% endif %}
         {% for feed in all_feeds %}
             <link href="{{ FEED_DOMAIN }}/{{ feed.url }}"
                   type="application/{{ feed.kind|lower }}+xml"
                   rel="alternate"
-                  title="{{ SITENAME|e }} - {{ feed.name|e }} - {{ feed.kind }} Feed"/>
+                  title="{{ SITENAME|e }} - {{ feed.name|e }} - {{ feed.kind }} Feed" />
         {% endfor %}
-        {% block head %}{% endblock %}
+        {% block head %}
+        {% endblock head %}
     </head>
     <body class="bg-transparent pt-4">
         <div class="container">
             {% if SITE_THUMBNAIL %}
                 <a href="{{ SITEURL }}" class="avatar-container float-start mx-4">
-                    <div class="avatar {% if SITE_THUMBNAIL_TEXT %} animate{% endif %}">
+                    <div class="avatar {% if SITE_THUMBNAIL_TEXT %}animate{% endif %}">
                         <div class="side">
                             <img src="{{ SITE_THUMBNAIL }}" class="img-fluid" />
                         </div>
                         {% if SITE_THUMBNAIL_TEXT %}
-                            <div class="side back text-center pt-2 px-1 small">{{ SITE_THUMBNAIL_TEXT }}</div>
+                            <div class="side back position-relative text-center pt-2 px-1 small">
+                                <span class="position-absolute top-50 start-0 translate-middle-y">{{ SITE_THUMBNAIL_TEXT }}</span>
+                            </div>
                         {% endif %}
                     </div>
                 </a>
             {% endif %}
             <h1>
                 <a href="{{ SITEURL }}" class="text-body-emphasis text-decoration-none">{{ SITENAME }}</a>
                 <small class="text-body-tertiary"><small>{{ SITESUBTITLE }}</small></small>
@@ -128,36 +130,36 @@
                         aria-label="Toggle navigation">
                     <span class="navbar-toggler-icon"></span>
                 </button>
                 <div class="collapse navbar-collapse mx-4" id="plumage-navbar-collapse-1">
                     <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                         {% for title, link in MENUITEMS %}
                             {% set active_page = link == ("/%s"|format(output_file)).strip('index.html') -%}
-                            <li class="nav-item {% if active_page %} active{% endif %}">
+                            <li class="nav-item {% if active_page %}active{% endif %}">
                                 <a class="nav-link" href="{{ link }}">
                                     {{ title }}
                                     {% if active_page %}<span class="visually-hidden">(current)</span>{% endif %}
                                 </a>
                             </li>
                         {% endfor %}
                         {% if DISPLAY_PAGES_ON_MENU %}
                             {% for p in pages %}
                                 {% set active_page = (p == page) -%}
-                                <li class="nav-item {% if active_page %} active{% endif %}">
+                                <li class="nav-item {% if active_page %}active{% endif %}">
                                     <a class="nav-link" href="{{ SITEURL }}/{{ p.url }}">
                                         {{ p.title }}
                                         {% if active_page %}<span class="visually-hidden">(current)</span>{% endif %}
                                     </a>
                                 </li>
                             {% endfor %}
                         {% endif %}
                         {% if DISPLAY_CATEGORIES_ON_MENU %}
                             {% for c, null in categories %}
                                 {% set active_category = (c == category) -%}
-                                <li class="nav-item {% if active_page %} active{% endif %}">
+                                <li class="nav-item {% if active_page %}active{% endif %}">
                                     <a class="nav-link" href="{{ SITEURL }}/{{ c.url }}">
                                         {{ c.name }}
                                         {% if active_category %}<span class="visually-hidden">(current)</span>{% endif %}
                                     </a>
                                 </li>
                             {% endfor %}
                         {% endif %}
@@ -174,33 +176,36 @@
                 </div>
             </nav>
         </div>
         <div class="container mt-5">
             {% set has_left_content = has_left or LEFT_SIDEBAR is defined %}
             {% set has_right_content = has_right or RIGHT_SIDEBAR is defined %}
             <div class="row">
-                <div class=" {% if (has_left_content and has_right_content) or LAYOUT == 'full-width' %} col-md-6 {% elif has_left_content or has_right_content %} col-md-9 {% else %} col-md-12 {% endif %} {% if has_left_content %} offset-md-3{% endif %}">
-                    {% block top_center %}{% endblock %}
+                <div class=" {% if (has_left_content and has_right_content) or LAYOUT == 'full-width' %} col-md-6 {% elif has_left_content or has_right_content %} col-md-9 {% else %} col-md-12 {% endif %} {% if has_left_content %}offset-md-3{% endif %}">
+                    {% block top_center %}
+                    {% endblock top_center %}
                 </div>
             </div>
             <div class="row">
                 {% if LAYOUT != 'full-width' and has_left_content %}
                     <div class="col-md-3">
-                        {% block left_sidebar %}{% endblock %}
+                        {% block left_sidebar %}
+                        {% endblock left_sidebar %}
                         {{ LEFT_SIDEBAR }}
                     </div>
                 {% endif %}
                 <main id="content"
                      role="main"
                      class=" {% if LAYOUT == 'full-width' %} offset-md-1 {% elif has_left_content and has_right_content %} col-md-6 {% elif has_left_content or has_right_content %} col-md-9 {% else %} col-md-12 {% endif %}">
                     {% block content %}{% endblock %}
                 </main>
                 {% if LAYOUT != 'full-width' and has_right_content %}
                     <div class="col-md-3">
-                        {% block right_sidebar %}{% endblock %}
+                        {% block right_sidebar %}
+                        {% endblock right_sidebar %}
                         {{ RIGHT_SIDEBAR }}
                     </div>
                 {% endif %}
             </div>
         </div>
         {# TODO: make footer sticky #}
         <footer class="container-fluid mt-5 p-4 small fw-light">
@@ -223,38 +228,41 @@
                 {% endfor %}
                 <div class="col-md-2">
                     <h6>Browse content by</h6>
                     <ul class="list-unstyled">
                         {% if CATEGORIES_SAVE_AS %}
                             <li>
                                 <a href="{{ SITEURL }}/{{ CATEGORIES_SAVE_AS }}">
-                                    <i class="fas fa-th-list fa-fw"></i>
+                                    <i class="bi bi-list-task"></i>
                                     Categories
                                 </a>
                             </li>
                         {% endif %}
                         {% if AUTHORS_SAVE_AS %}
                             <li>
                                 <a href="{{ SITEURL }}/{{ AUTHORS_SAVE_AS }}">
-                                    <i class="fas fa-users fa-fw"></i>
+                                    <i class="bi bi-people-fill"></i>
                                     Authors
                                 </a>
                             </li>
                         {% endif %}
                         {% if ARCHIVES_SAVE_AS %}
                             <li>
                                 <a href="{{ SITEURL }}/{{ ARCHIVES_SAVE_AS }}">
-                                    <i class="far fa-calendar-alt fa-fw"></i>
+                                    <i class="bi bi-calendar3"></i>
                                     Dates
                                 </a>
                             </li>
                         {% endif %}
                         {% if TAGS_SAVE_AS %}
                             <li>
-                                <a href="{{ SITEURL }}/{{ TAGS_SAVE_AS }}"><i class="fas fa-tags fa-fw"></i> Tags</a>
+                                <a href="{{ SITEURL }}/{{ TAGS_SAVE_AS }}">
+                                    <i class="bi bi-tags-fill"></i>
+                                    Tags
+                                </a>
                             </li>
                         {% endif %}
                     </ul>
                 </div>
                 <div class="col-md-2 text-body-tertiary">
                     <h6>Copyright notice</h6>
                     {% set date_start = dates[-1].date.year if dates else None %}
@@ -283,15 +291,16 @@
                 <div class="col-md-2">
                     {% if all_feeds %}
                         <h6>Feeds</h6>
                         <ul class="list-unstyled small">
                             {% for feed in all_feeds %}
                                 <li>
                                     <a href="{{ FEED_DOMAIN }}/{{ feed.url }}">
-                                        <i class="fas fa-{{ feed.kind|lower }} fa-fw"></i> {{ feed.name }} ({{ feed.kind }})
+                                        <i class="bi {% if feed.kind == 'RSS' %} bi-rss-fill {% else %} bi-rss {% endif %}"></i>
+                                        {{ feed.name }} ({{ feed.kind }})
                                     </a>
                                 </li>
                             {% endfor %}
                         </ul>
                     {% endif %}
                 </div>
             </div>
@@ -299,15 +308,15 @@
                 <div class="offset-3 col-6 small text-muted text-center">
                     Site generated by <a class="text-dark" href="https://getpelican.com">Pelican</a>.
                     <br/>
                     <a class="text-dark" href="https://github.com/kdeldycke/plumage">Plumage</a>
                     theme by <a class="text-dark" href="https://kevin.deldycke.com">Kevin Deldycke</a>.
                 </div>
                 <div class="col-3 text-end d-flex flex-column">
-                    <a class="mt-auto" href="#"><i class="fas fa-arrow-up"></i> Back to top</a>
+                    <a class="mt-auto" href="#"><i class="bi bi-arrow-bar-up"></i> Back to top</a>
                 </div>
             </div>
         </footer>
         {% if STORK_SEARCH %}
             <script src="https://files.stork-search.net/releases/v1.6.0/stork.js"></script>
             <script>
                 stork.register("sitesearch", "{{ SITEURL }}/search-index.st")
```

#### html2text {}

```diff
@@ -3,38 +3,38 @@
 or (page in draft_pages) %}
 {% else %}
 {% endif %}
 {% assets filters="libsass,postcss,cssmin", output="css/main.min.css", "css/
 mglass.scss", "css/main.scss", "css/pygments/" + CODE_STYLE + ".css", "css/
 code.scss" %}
 {% endassets %}
-{% block extra_css %}{% endblock %} {% include "analytics.html" %}
+{% block extra_css %} {% endblock extra_css %} {% include "analytics.html" %}
 {% assets filters="closure_js", output="js/main.min.js", "js/jquery.mglass.js",
 "js/application.js" %}
-{% endassets %} {% block extra_js %}{% endblock %}
+{% endassets %} {% block extra_js %} {% endblock extra_js %}
 {% set all_feeds = [] %} {% if FEED_ALL_ATOM %} {% if all_feeds.append({'kind':
-'Atom', 'url': FEED_ALL_ATOM, 'name': 'All posts'}) %} {% endif %} {% endif %}
+'Atom', 'url': FEED_ALL_ATOM, 'name': 'All posts'}) %}{% endif %} {% endif %}
 {% if FEED_ALL_RSS %} {% if all_feeds.append({'kind': 'RSS', 'url':
-FEED_ALL_RSS, 'name': 'All posts'}) %} {% endif %} {% endif %} {% if FEED_ATOM
+FEED_ALL_RSS, 'name': 'All posts'}) %}{% endif %} {% endif %} {% if FEED_ATOM
 %} {% if all_feeds.append({'kind': 'Atom', 'url': FEED_ATOM, 'name': 'Latest
-posts'}) %} {% endif %} {% endif %} {% if FEED_RSS %} {% if all_feeds.append(
-{'kind': 'RSS', 'url': FEED_RSS, 'name': 'Latest posts'}) %} {% endif %} {%
+posts'}) %}{% endif %} {% endif %} {% if FEED_RSS %} {% if all_feeds.append(
+{'kind': 'RSS', 'url': FEED_RSS, 'name': 'Latest posts'}) %}{% endif %} {%
 endif %} {% if CATEGORY_FEED_ATOM and category is defined %} {% if
 all_feeds.append({'kind': 'Atom', 'url': CATEGORY_FEED_ATOM.format
 (slug=category.slug), 'name': 'Category: ' + category.name}) %} {% endif %} {%
 endif %} {% if CATEGORY_FEED_RSS and category is defined %} {% if
 all_feeds.append({'kind': 'RSS', 'url': CATEGORY_FEED_RSS.format
 (slug=category.slug), 'name': 'Category: ' + category.name}) %} {% endif %} {%
 endif %} {% if TAG_FEED_ATOM and tag is defined %} {% if all_feeds.append(
 {'kind': 'Atom', 'url': TAG_FEED_ATOM.format(slug=tag.slug), 'name': 'Tag: ' +
 tag.name}) %} {% endif %} {% endif %} {% if TAG_FEED_RSS and tag is defined %}
 {% if all_feeds.append({'kind': 'RSS', 'url': TAG_FEED_RSS.format
 (slug=tag.slug), 'name': 'Tag: ' + tag.name}) %} {% endif %} {% endif %} {% for
 feed in all_feeds %}
-{% endfor %} {% block head %}{% endblock %}
+{% endfor %} {% block head %} {% endblock head %}
 {% if SITE_THUMBNAIL %}
 _[_{_{_ _S_I_T_E___T_H_U_M_B_N_A_I_L_ _}_}_]
 _{_%_ _i_f_ _S_I_T_E___T_H_U_M_B_N_A_I_L___T_E_X_T_ _%_}
 _{_{_ _S_I_T_E___T_H_U_M_B_N_A_I_L___T_E_X_T_ _}_}
 _{_%_ _e_n_d_i_f_ _%_}
 {% endif %}
 ************ _{{_{{_ _SS_II_TT_EE_NN_AA_MM_EE_ _}}_}} {{{{ SSIITTEESSUUBBTTIITTLLEE }}}} ************
@@ -50,20 +50,20 @@
     * _{_{_ _c_._n_a_m_e_ _}_}_ _{_%_ _i_f_ _a_c_t_i_v_e___c_a_t_e_g_o_r_y_ _%_}_(_c_u_r_r_e_n_t_)_{_%_ _e_n_d_i_f_ _%_}
     * {% endfor %} {% endif %}
 {% if STORK_SEARCH %}
 [                    ]
 {% endif %}
 {% set has_left_content = has_left or LEFT_SIDEBAR is defined %} {% set
 has_right_content = has_right or RIGHT_SIDEBAR is defined %}
-{% block top_center %}{% endblock %}
+{% block top_center %} {% endblock top_center %}
 {% if LAYOUT != 'full-width' and has_left_content %}
-{% block left_sidebar %}{% endblock %} {{ LEFT_SIDEBAR }}
+{% block left_sidebar %} {% endblock left_sidebar %} {{ LEFT_SIDEBAR }}
 {% endif %} {% block content %}{% endblock %} {% if LAYOUT != 'full-width' and
 has_right_content %}
-{% block right_sidebar %}{% endblock %} {{ RIGHT_SIDEBAR }}
+{% block right_sidebar %} {% endblock right_sidebar %} {{ RIGHT_SIDEBAR }}
 {% endif %}
 {# TODO: make footer sticky #}
 {% set SOCIAL_WIDGET_NAME = SOCIAL_WIDGET_NAME or 'Social' %} {% set
 LINKS_WIDGET_NAME = LINKS_WIDGET_NAME or 'Links' %} {% for group_title,
 group_links in ((SOCIAL_WIDGET_NAME, SOCIAL), (LINKS_WIDGET_NAME, LINKS)) %}
 {% if group_links %}
 ** {{{{ ggrroouupp__ttiittllee }}}} **
```

### Comparing `plumage-3.1.0/plumage/templates/categories.html` & `plumage-4.0.0/plumage/templates/categories.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 {% extends "base.html" %}
-{% block title %}All categories{% endblock %}
+{% block title %}All categories{% endblock title %}
 {% block top_center %}
     <h1>
         <a href="{{ SITEURL }}/{{ CATEGORIES_SAVE_AS }}"
            rel="bookmark"
            title="Permalink to category list">Categories</a>
     </h1>
-{% endblock %}
+{% endblock top_center %}
 {% block content %}
     {% set all_categories = [] %}
     {% for category, articles in categories %}
-        {% if all_categories.append({'name': category.name, 'url': category.url, 'articles': articles|length()}) %}
-        {% endif %}
+        {% if all_categories.append({'name': category.name, 'url': category.url, 'articles': articles|length()}) %}{% endif %}
     {% endfor %}
     <dl class="row">
         {# Sort by category frequency, then alphabetically #}
         {% for category in all_categories|sort(attribute='name')|sort(reverse=True, attribute='articles') %}
             <dt class="col-sm-2">
-                <a href="{{ SITEURL }}/{{ category.url }}" class="badge text-bg-info">{{ category.name }}</a>
+                <a href="{{ SITEURL }}/{{ category.url }}" class="badge category">{{ category.name }}</a>
             </dt>
             <dd class="col-sm-10">
                 <a href="{{ SITEURL }}/{{ category.url }}">{{ category.articles }} article{{ 's' if category.articles > 1 else '' }}</a>
             </dd>
         {% endfor %}
     </dl>
-{% endblock %}
+{% endblock content %}
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-{% extends "base.html" %} {% block title %}All categories{% endblock %} {%
-block top_center %}
+{% extends "base.html" %} {% block title %}All categories{% endblock title %}
+{% block top_center %}
 ************ _CC_aa_tt_ee_gg_oo_rr_ii_ee_ss ************
-{% endblock %} {% block content %} {% set all_categories = [] %} {% for
-category, articles in categories %} {% if all_categories.append({'name':
-category.name, 'url': category.url, 'articles': articles|length()}) %} {% endif
+{% endblock top_center %} {% block content %} {% set all_categories = [] %} {%
+for category, articles in categories %} {% if all_categories.append({'name':
+category.name, 'url': category.url, 'articles': articles|length()}) %}{% endif
 %} {% endfor %}
 {# Sort by category frequency, then alphabetically #} {% for category in
 all_categories|sort(attribute='name')|sort(reverse=True, attribute='articles')
 %}
-{% endblock %}
+{% endblock content %}
```

### Comparing `plumage-3.1.0/plumage/templates/category.html` & `plumage-4.0.0/plumage/templates/category.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 {% extends "base.html" %}
-{% block title %}{{ category }}{% endblock %}
+{% block title %}{{ category }}{% endblock title %}
 {% block top_center %}
     <h1>
         <a href="{{ SITEURL }}/{{ category.url }}"
            rel="bookmark"
            title="Permalink to {{ category|e }} articles">{{ category }} articles</a>
     </h1>
-{% endblock %}
+{% endblock top_center %}
 {% block content %}
     <dl class="row">
         {% for article in articles %}
             <dt class="col-sm-3">
                 <abbr class="published" title="{{ article.date.isoformat() }}">{{ article.locale_date }}</abbr>
             </dt>
             <dd class="col-sm-9">
                 <a href="{{ SITEURL }}/{{ article.url }}">{{ article.title }}</a>
             </dd>
         {% endfor %}
     </dl>
-{% endblock %}
+{% endblock content %}
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
-{% extends "base.html" %} {% block title %}{{ category }}{% endblock %} {%
-block top_center %}
+{% extends "base.html" %} {% block title %}{{ category }}{% endblock title %}
+{% block top_center %}
 ************ _{{_{{_ _cc_aa_tt_ee_gg_oo_rr_yy_ _}}_}}_ _aa_rr_tt_ii_cc_ll_ee_ss ************
-{% endblock %} {% block content %}
+{% endblock top_center %} {% block content %}
 {% for article in articles %}
-{% endblock %}
+{% endblock content %}
```

### Comparing `plumage-3.1.0/plumage/templates/index.html` & `plumage-4.0.0/plumage/templates/tag.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 {% extends "base.html" %}
+{% block title %}{{ tag }}{% endblock title %}
+{% block top_center %}
+    <h1>
+        <a href="{{ SITEURL }}/{{ tag.url }}"
+           rel="bookmark"
+           title="Permalink to {{ tag|e }} articles">{{ tag }} articles</a>
+    </h1>
+{% endblock top_center %}
 {% block content %}
-    {% block content_title %}<h2>Articles</h2>{% endblock %}
-    {% for article in articles_page.object_list %}
-        <article>
-            <header>
-                <h2>
-                    <a href="{{ SITEURL }}/{{ article.url }}"
-                       rel="bookmark"
-                       title="Permalink to {{ article.title|striptags|e }}">{{ article.title }}</a>
-                </h2>
-            </header>
-            <div>{{ article.summary|striptags }}</div>
-            <div>
-                <a class="btn btn-primary" href="{{ SITEURL }}/{{ article.url }}"><strong>➟ Read more</strong></a>
-            </div>
-        </article>
-        <hr/>
-    {% endfor %}
-    {% include 'pagination.html' %}
+    <dl class="row">
+        {% for article in articles %}
+            <dt class="col-sm-3">
+                <abbr class="published" title="{{ article.date.isoformat() }}">{{ article.locale_date }}</abbr>
+            </dt>
+            <dd class="col-sm-9">
+                <a href="{{ SITEURL }}/{{ article.url }}">{{ article.title }}</a>
+            </dd>
+        {% endfor %}
+    </dl>
 {% endblock content %}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,8 +1,6 @@
-{% extends "base.html" %} {% block content %} {% block content_title %}
-********** AArrttiicclleess **********
-{% endblock %} {% for article in articles_page.object_list %}
-********** _{{_{{_ _aa_rr_tt_ii_cc_ll_ee_.._tt_ii_tt_ll_ee_ _}}_}} **********
-{{ article.summary|striptags }}
-_?â_?_?_ _RR_ee_aa_dd_ _mm_oo_rr_ee
-===============================================================================
-{% endfor %} {% include 'pagination.html' %} {% endblock content %}
+{% extends "base.html" %} {% block title %}{{ tag }}{% endblock title %} {%
+block top_center %}
+************ _{{_{{_ _tt_aa_gg_ _}}_}}_ _aa_rr_tt_ii_cc_ll_ee_ss ************
+{% endblock top_center %} {% block content %}
+{% for article in articles %}
+{% endblock content %}
```

### Comparing `plumage-3.1.0/plumage/templates/macros.html` & `plumage-4.0.0/plumage/templates/macros.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,67 @@
-{% macro render_tag(tag) -%}
+{% macro render_tag(tag, counter, kind='tag') -%}
+    {# A tag or a category can be pass as argument as they share the same data structure #}
+    {% set kind = 'tag' if kind == 'tag' else 'category' %}
     <a href="{{ SITEURL }}/{{ tag.url }}"
-       class="badge text-bg-secondary"
+       rel="tag"
+       class="badge {{ kind }}"
        data-bs-toggle="tooltip"
-       title="{{ tag.articles }} article{{ 's' if tag.articles > 1 else '' }} with this tag">{{ tag.name }}</a>
+       {% if counter is defined %} title="{{ counter }} article{{ 's' if counter > 1 else '' }} with this {{ kind }}" {% endif %}>{{ tag.name }}</a>
 {%- endmacro %}
 {% macro render_link_icon(link, label, favicon=True) -%}
     {% set icon = [] %}
     {% set favicon = False if favicon == False else True %}
     {% set protocol = link.split(':', 1)[0] %}
     {% if protocol == 'mailto' %}
-        {% if icon.append('envelope') %}
-        {% endif %}
+        {% if icon.append('envelope-fill') %}{% endif %}
     {% elif protocol.startswith('http') %}
         {% set domain = link.split('%s://' % protocol, 1)[1].split('/', 1)[0] %}
         {% set SITE_ICONS = {
-        'apple': ['apple.com']
-        , 'bitbucket': ['bitbucket.org', 'bitbucket.com']
-        , 'dropbox': ['dropbox.com']
-        , 'facebook-square': ['facebook.com']
-        , 'github': ['github.com']
-        , 'hacker-news': ['news.ycombinator.com']
-        , 'linkedin': ['linkedin.com']
-        , 'stack-overflow': ['stackoverflow.com']
-        , 'stack-exchange': ['stackexchange.com']
-        , 'twitter': ['twitter.com']
-        , 'youtube': ['youtube.com']
-        }
-        %}
+            "apple": [
+                "apple.com"
+            ],
+            "dropbox": [
+                "dropbox.com"
+            ],
+            "facebook": [
+                "facebook.com"
+            ],
+            "github": [
+                "github.com"
+            ],
+            "linkedin": [
+                "linkedin.com"
+            ],
+            "stack-overflow": [
+                "stackexchange.com",
+                "stackoverflow.com"
+            ],
+            "twitter": [
+                "twitter.com"
+            ],
+            "youtube": [
+                "youtube.com"
+            ]
+        } %}
         {% for (site_icon, site_domains) in SITE_ICONS.items() %}
             {% for site_domain in site_domains %}
                 {% if domain.startswith(site_domain) %}
-                    {% if icon.append(site_icon) %}
-                    {% endif %}
+                    {% if icon.append(site_icon) %}{% endif %}
                 {% endif %}
             {% endfor %}
         {% endfor %}
     {% endif %}
     <a href="{{ link }}">
         {% if icon %}
-            <i class="fab {{ 'fa-%s' % icon[0] }} fa-fw"></i>
+            <i class="bi {{ 'bi-%s' % icon[0] }}"></i>
         {% elif domain and favicon %}
             <img src="https://www.google.com/s2/favicons?domain={{ domain }}"
                  width="16"
                  height="16"
                  class="link-icon"
-                 alt="{{ domain }} icon"/>
+                 alt="{{ domain }} icon" />
         {% else %}
-            <i class="fas fa-external-link-alt fa-fw"></i>
+            <i class="bi bi-box-arrow-up-right"></i>
         {% endif %}
         {{ label }}
     </a>
 {%- endmacro %}
```

#### html2text {}

```diff
@@ -1,18 +1,21 @@
-{% macro render_tag(tag) -%} _{_{_ _t_a_g_._n_a_m_e_ _}_} {%- endmacro %} {% macro
-render_link_icon(link, label, favicon=True) -%} {% set icon = [] %} {% set
-favicon = False if favicon == False else True %} {% set protocol = link.split
-(':', 1)[0] %} {% if protocol == 'mailto' %} {% if icon.append('envelope') %}
-{% endif %} {% elif protocol.startswith('http') %} {% set domain = link.split
-('%s://' % protocol, 1)[1].split('/', 1)[0] %} {% set SITE_ICONS = { 'apple':
-['apple.com'] , 'bitbucket': ['bitbucket.org', 'bitbucket.com'] , 'dropbox':
-['dropbox.com'] , 'facebook-square': ['facebook.com'] , 'github':
-['github.com'] , 'hacker-news': ['news.ycombinator.com'] , 'linkedin':
-['linkedin.com'] , 'stack-overflow': ['stackoverflow.com'] , 'stack-exchange':
-['stackexchange.com'] , 'twitter': ['twitter.com'] , 'youtube': ['youtube.com']
-} %} {% for (site_icon, site_domains) in SITE_ICONS.items() %} {% for
+{% macro render_tag(tag, counter, kind='tag') -%} {# A tag or a category can be
+pass as argument as they share the same data structure #} {% set kind = 'tag'
+if kind == 'tag' else 'category' %}
+% if counter is defined %} title="{{ counter }} article{{ 's' if counter > 1
+else '' }} with this {{ kind }}" {% endif %}>{{ tag.name }}
+ {%- endmacro %} {% macro render_link_icon(link, label, favicon=True) -%} {%
+set icon = [] %} {% set favicon = False if favicon == False else True %} {% set
+protocol = link.split(':', 1)[0] %} {% if protocol == 'mailto' %} {% if
+icon.append('envelope-fill') %}{% endif %} {% elif protocol.startswith('http')
+%} {% set domain = link.split('%s://' % protocol, 1)[1].split('/', 1)[0] %} {%
+set SITE_ICONS = { "apple": [ "apple.com" ], "dropbox": [ "dropbox.com" ],
+"facebook": [ "facebook.com" ], "github": [ "github.com" ], "linkedin":
+[ "linkedin.com" ], "stack-overflow": [ "stackexchange.com",
+"stackoverflow.com" ], "twitter": [ "twitter.com" ], "youtube": [ "youtube.com"
+] } %} {% for (site_icon, site_domains) in SITE_ICONS.items() %} {% for
 site_domain in site_domains %} {% if domain.startswith(site_domain) %} {% if
-icon.append(site_icon) %} {% endif %} {% endif %} {% endfor %} {% endfor %} {%
+icon.append(site_icon) %}{% endif %} {% endif %} {% endfor %} {% endfor %} {%
 endif %}
 _{_%_ _i_f_ _i_c_o_n_ _%_}_ _{_%_ _e_l_i_f_ _d_o_m_a_i_n_ _a_n_d_ _f_a_v_i_c_o_n_ _%_}_ _[_{_{_ _d_o_m_a_i_n_ _}_}_ _i_c_o_n_]_{_%_ _e_l_s_e_ _%_}_ _{_%
 _e_n_d_i_f_ _%_}_ _{_{_ _l_a_b_e_l_ _}_}
 {%- endmacro %}
```

### Comparing `plumage-3.1.0/plumage/templates/pagination.html` & `plumage-4.0.0/plumage/templates/pagination.html`

 * *Files 11% similar despite different names*

```diff
@@ -3,21 +3,21 @@
         <ul class="pagination justify-content-center">
             {% if articles_page.has_previous() %}
                 <li class="page-item">
                     <a class="page-link"
                        href="{{ SITEURL }}/{{ articles_previous_page.url }}"
                        aria-label="Previous"
                        rel="prev">
-                        <span aria-hidden="true">&larr;</span>
+                        <span aria-hidden="true">←</span>
                     </a>
                 </li>
             {% else %}
                 <li class="page-item disabled">
                     <span class="page-link" aria-label="Previous" rel="prev">
-                        <span aria-hidden="true">&larr;</span>
+                        <span aria-hidden="true">←</span>
                     </span>
                 </li>
             {% endif %}
             {% for num in articles_paginator.page_range %}
                 {% set linked_pages = [
                 1, 2, articles_page.number - 1, articles_page.number,
                 articles_page.number + 1, articles_paginator.num_pages - 1,
@@ -41,20 +41,20 @@
             {% endfor %}
             {% if articles_page.has_next() %}
                 <li class="page-item">
                     <a class="page-link"
                        href="{{ SITEURL }}/{{ articles_next_page.url }}"
                        aria-label="Next"
                        rel="next">
-                        <span aria-hidden="true">&rarr;</span>
+                        <span aria-hidden="true">→</span>
                     </a>
                 </li>
             {% else %}
                 <li class="page-item disabled">
                     <span class="page-link" aria-label="Next" rel="next">
-                        <span aria-hidden="true">&rarr;</span>
+                        <span aria-hidden="true">→</span>
                     </span>
                 </li>
             {% endif %}
         </ul>
     </nav>
 {% endif %}
```

### Comparing `plumage-3.1.0/plumage/templates/period_archives.html` & `plumage-4.0.0/plumage/templates/period_archives.html`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 {% macro period_url() -%}
     {# Ugly hack to get period archive URL. The {{ url }} variable doesn't return what I expected.
     The issue is being discussed at: https://github.com/getpelican/pelican/issues/2773
     #}
     {% set url_parts = output_file.split('index.html', 1) %}
     {{- url_parts[0] -}}
 {%- endmacro %}
-{% block title %}{{ period_label() }} archives{% endblock %}
+{% block title %}{{ period_label() }} archives{% endblock title %}
 {% block top_center %}
     <h1>
         <a href="{{ SITEURL }}/{{ period_url() }}"
            rel="bookmark"
            title="Permalink to {{ period_label()|e }} archives">
             {{ period_label() }} archives
         </a>
     </h1>
-{% endblock %}
+{% endblock top_center %}
 {% block content %}
     <dl class="row">
         {% for article in dates %}
             <dt class="col-sm-3">
                 <abbr class="published" title="{{ article.date.isoformat() }}">{{ article.locale_date }}</abbr>
             </dt>
             <dd class="col-sm-9">
                 <a href="{{ SITEURL }}/{{ article.url }}">{{ article.title }}</a>
             </dd>
         {% endfor %}
     </dl>
-{% endblock %}
+{% endblock content %}
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% extends "base.html" %} {% macro period_label() %} {{ period|reverse|join('
 ') }} {% endmacro %} {% macro period_url() -%} {# Ugly hack to get period
 archive URL. The {{ url }} variable doesn't return what I expected. The issue
 is being discussed at: https://github.com/getpelican/pelican/issues/2773 #} {%
 set url_parts = output_file.split('index.html', 1) %} {{- url_parts[0] -}} {%-
-endmacro %} {% block title %}{{ period_label() }} archives{% endblock %} {%
-block top_center %}
+endmacro %} {% block title %}{{ period_label() }} archives{% endblock title %}
+{% block top_center %}
 ************ _{{_{{_ _pp_ee_rr_ii_oo_dd____ll_aa_bb_ee_ll_((_))_ _}}_}}_ _aa_rr_cc_hh_ii_vv_ee_ss ************
-{% endblock %} {% block content %}
+{% endblock top_center %} {% block content %}
 {% for article in dates %}
-{% endblock %}
+{% endblock content %}
```

### Comparing `plumage-3.1.0/plumage/templates/projects.html` & `plumage-4.0.0/plumage/templates/projects.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,56 @@
-{% set LAYOUT = 'full-width' %}
+{% set LAYOUT = "full-width" %}
 {% extends "base.html" %}
 {# Map URL substring matches to link's icon, then label.
 Sorted by priority: the first items takes precedence over those at the end. #}
 {% set ICONS = [
-('github.com',                'fab fa-github-alt',     'Git repository'),
-('bitbucket.org',             'fab fa-bitbucket',      'Mercurial repository'),
-('youtube.com',               'fas fa-play',           'Play video'),
-('ohloh.net',                 'fas fa-bar-chart-o',    'Contribution statistics'),
-('stackoverflow.com',         'fab fa-stack-overflow', 'Community support'),
-('stackexchange.com',         'fab fa-stack-exchange', 'Community support'),
-('twitter.com',               'fab fa-twitter',        'Social media activities'),
-('bugs.launchpad.net',        'fas fa-bug',            'Reported bugs'),
-('trac.wordpress.org',        'fas fa-bug',            'Reported bugs'),
-('sourceforge.net/apps/trac', 'fas fa-bug',            'Reported bugs'),
-('bugs.debian.org',           'fas fa-bug',            'Reported bugs'),
-('bugs.kde.org',              'fas fa-bug',            'Reported bugs'),
-('mantis',                    'fas fa-bug',            'Reported bugs'),
-('ticket=on',                 'fas fa-bug',            'Reported bugs'),
-('gmane.org',                 'fas fa-envelope-o',     'Mailing-list participation'),
-('type_of_search=mlists',     'fas fa-envelope-o',     'Mailing-list participation'),
-(SITEURL,                     'fas fa-bullhorn',       'Announcement on this blog'),
-]
-%}
+    ('github.com',                'github',         'Git repository'),
+    ('youtube.com',               'play-fill',      'Play video'),
+    ('ohloh.net',                 'graph-up',       'Contribution statistics'),
+    ('stackoverflow.com',         'stack-overflow', 'Community support'),
+    ('stackexchange.com',         'stack-overflow', 'Community support'),
+    ('twitter.com',               'twitter',        'Social media activities'),
+    ('bugs.launchpad.net',        'bug-fill',       'Reported bugs'),
+    ('trac.wordpress.org',        'bug-fill',       'Reported bugs'),
+    ('sourceforge.net/apps/trac', 'bug-fill',       'Reported bugs'),
+    ('bugs.debian.org',           'bug-fill',       'Reported bugs'),
+    ('bugs.kde.org',              'bug-fill',       'Reported bugs'),
+    ('mantis',                    'bug-fill',       'Reported bugs'),
+    ('ticket=on',                 'bug-fill',       'Reported bugs'),
+    ('gmane.org',                 'envelope-fill',  'Mailing-list participation'),
+    ('type_of_search=mlists',     'envelope-fill',  'Mailing-list participation'),
+    (SITEURL,                     'megaphone-fill', 'Announcement on this blog'),
+] %}
 {% macro render_card(all_tags, project) %}
     <div class="card">
-        {% if project.inactive %}
-            <div class="corner-banner shadow-sm bg-danger text-white fw-bold">Inactive</div>
-        {% endif %}
+        {% if project.inactive %}<div class="corner-banner shadow-sm bg-danger text-white fw-bold">Inactive</div>{% endif %}
         {% if project.thumb %}
             {% if project.thumb_link %}<a href="{{ project.thumb_link }}">{% endif %}
-            <img class="card-img-top"
-                 alt="{{ project.name }} thumbnail"
-                 src="{{ project.thumb }}"/>
-            {% if project.thumb_link %}</a>{% endif %}
+                <img class="card-img-top"
+                     alt="{{ project.name }} thumbnail"
+                     src="{{ project.thumb }}" />
+                {% if project.thumb_link %}</a>{% endif %}
         {% endif %}
         <div class="card-body">
             <h4 class="card-title">{{ project.name }}</h4>
             {% if project.roles or project.tools %}
                 <p class="card-text">
                     <ul class="list-inline">
                         {% for role in project.roles %}
                             <li class="list-inline-item">
                                 <span class="badge text-bg-success">{{ role }}</span>
                             </li>
                         {% endfor %}
                         {# Sort by tag frequency, then alphabetically #}
                         {% for tag in all_tags|sort(attribute='name')|sort(reverse=True, attribute='articles') %}
-                            {% if tag.name in project.tools %}
-                                <li class="list-inline-item">{{ m.render_tag(tag) }}</li>
-                            {% endif %}
+                            {% if tag.name in project.tools %}<li class="list-inline-item">{{ m.render_tag(tag) }}</li>{% endif %}
                         {% endfor %}
                         {% set tag_names = [] %}
                         {% for tag in all_tags %}
-                            {% if tag_names.append(tag.name) %}
-                            {% endif %}
+                            {% if tag_names.append(tag.name) %}{% endif %}
                         {% endfor %}
                         {% for tool in project.tools %}
                             {% if tool not in tag_names %}
                                 <li class="list-inline-item">
                                     <span class="badge text-bg-secondary">{{ tool }}</span>
                                 </li>
                             {% endif %}
@@ -66,61 +59,54 @@
                 </p>
             {% endif %}
             {% if project.desc %}<p class="card-text">{{ project.desc }}</p>{% endif %}
             {% if project.links %}
                 <p class="card-text">
                     {% for link in project.links %}
                         {# Default icon in case of no match #}
-                        {% set matches = [('', 'fas fa-home', 'Project home')] %}
+                        {% set matches = [('', 'house-fill', 'Project home')] %}
                         {% for rule in ICONS|reverse %}
                             {% if rule[0] and link.find(rule[0]) != -1 %}
-                                {% if matches.append(rule) %}
-                                {% endif %}
+                                {% if matches.append(rule) %}{% endif %}
                             {% endif %}
                         {% endfor %}
-                        <a href="{{ link }}" title="{{ matches[-1][2]|e }}">
-                            <span class="fa-stack" style="vertical-align: top;">
-                                <i class="fas fa-circle fa-stack-2x"></i>
-                                <i class="{{ matches[-1][1] }} fa-stack-1x fa-inverse"></i>
-                            </span>
+                        <a class="btn btn-light rounded-circle p-2"
+                           href="{{ link }}"
+                           title="{{ matches[-1][2]|e }}">
+                            <i class="bi bi-{{ matches[-1][1] }}"></i>
                         </a>
                     {% endfor %}
                 </p>
             {% endif %}
         </div>
     </div>
 {% endmacro %}
 {% macro render_projects(projects) %}
     {% set all_tags = [] %}
     {% for tag, articles in tags %}
-        {% if all_tags.append({'name': tag.name, 'url': tag.url, 'articles': articles|length()}) %}
-        {% endif %}
+        {% if all_tags.append({'name': tag.name, 'url': tag.url, 'articles': articles|length()}) %}{% endif %}
     {% endfor %}
     {% if projects is defined %}
         <div class="row" data-masonry='{"percentPosition": true }'>
-            {% block project_pre_content %}{% endblock %}
+            {% block project_pre_content %}{% endblock project_pre_content %}
             {% set active_projects = [] %}
             {% set inactive_projects = [] %}
             {% for project in projects %}
                 {% if project.inactive %}
-                    {% if inactive_projects.append(project) %}
-                    {% endif %}
+                    {% if inactive_projects.append(project) %}{% endif %}
                 {% else %}
-                    {% if active_projects.append(project) %}
-                    {% endif %}
+                    {% if active_projects.append(project) %}{% endif %}
                 {% endif %}
             {% endfor %}
             {% for project_list in [active_projects, inactive_projects] %}
                 {% for project in project_list %}
-                    <div class="col-sm-6 col-lg-4 mb-4">
-                        {{ render_card(all_tags, project) }}
-                    </div>
+                    <div class="col-sm-6 col-lg-4 mb-4">{{ render_card(all_tags, project) }}</div>
                 {% endfor %}
             {% endfor %}
-            {% block project_post_content %}{% endblock %}
+            {% block project_post_content %}{% endblock project_post_content %}
         </div>
     {% endif %}
 {% endmacro %}
 {% macro render_project_group(group, projects) %}
     {{ group.pre }}
     {{ render_projects(projects) }}
     {{ group.post }}
@@ -130,14 +116,14 @@
             integrity="sha512-JRlcvSZAXT8+5SQQAvklXGJuxXTouyq8oIMaYERZQasB8SBDHZaUbeASsJWpk0UUrf89DP3/aefPPrlMR1h1yQ=="
             crossorigin="anonymous"
             referrerpolicy="no-referrer"></script>
 {% endblock extra_js %}
 {% block content %}
     {% if PROJECT_GROUPS is defined %}
         {% for group in PROJECT_GROUPS %}
-            {{ render_project_group(group, PROJECTS|selectattr("group", "sameas", group.id)) }}
+            {{ render_project_group(group, PROJECTS|selectattr("group", "sameas", group.id) ) }}
         {% endfor %}
-        {{ render_projects(PROJECTS|rejectattr("group", "defined")) }}
+        {{ render_projects(PROJECTS|rejectattr("group", "defined") ) }}
     {% else %}
         {{ render_projects(PROJECTS) }}
     {% endif %}
-{% endblock %}
+{% endblock content %}
```

#### html2text {}

```diff
@@ -1,63 +1,61 @@
-{% set LAYOUT = 'full-width' %} {% extends "base.html" %} {# Map URL substring
+{% set LAYOUT = "full-width" %} {% extends "base.html" %} {# Map URL substring
 matches to link's icon, then label. Sorted by priority: the first items takes
-precedence over those at the end. #} {% set ICONS = [ ('github.com', 'fab fa-
-github-alt', 'Git repository'), ('bitbucket.org', 'fab fa-bitbucket',
-'Mercurial repository'), ('youtube.com', 'fas fa-play', 'Play video'),
-('ohloh.net', 'fas fa-bar-chart-o', 'Contribution statistics'),
-('stackoverflow.com', 'fab fa-stack-overflow', 'Community support'),
-('stackexchange.com', 'fab fa-stack-exchange', 'Community support'),
-('twitter.com', 'fab fa-twitter', 'Social media activities'),
-('bugs.launchpad.net', 'fas fa-bug', 'Reported bugs'), ('trac.wordpress.org',
-'fas fa-bug', 'Reported bugs'), ('sourceforge.net/apps/trac', 'fas fa-bug',
-'Reported bugs'), ('bugs.debian.org', 'fas fa-bug', 'Reported bugs'),
-('bugs.kde.org', 'fas fa-bug', 'Reported bugs'), ('mantis', 'fas fa-bug',
-'Reported bugs'), ('ticket=on', 'fas fa-bug', 'Reported bugs'), ('gmane.org',
-'fas fa-envelope-o', 'Mailing-list participation'), ('type_of_search=mlists',
-'fas fa-envelope-o', 'Mailing-list participation'), (SITEURL, 'fas fa-
-bullhorn', 'Announcement on this blog'), ] %} {% macro render_card(all_tags,
-project) %}
+precedence over those at the end. #} {% set ICONS = [ ('github.com', 'github',
+'Git repository'), ('youtube.com', 'play-fill', 'Play video'), ('ohloh.net',
+'graph-up', 'Contribution statistics'), ('stackoverflow.com', 'stack-overflow',
+'Community support'), ('stackexchange.com', 'stack-overflow', 'Community
+support'), ('twitter.com', 'twitter', 'Social media activities'),
+('bugs.launchpad.net', 'bug-fill', 'Reported bugs'), ('trac.wordpress.org',
+'bug-fill', 'Reported bugs'), ('sourceforge.net/apps/trac', 'bug-fill',
+'Reported bugs'), ('bugs.debian.org', 'bug-fill', 'Reported bugs'),
+('bugs.kde.org', 'bug-fill', 'Reported bugs'), ('mantis', 'bug-fill', 'Reported
+bugs'), ('ticket=on', 'bug-fill', 'Reported bugs'), ('gmane.org', 'envelope-
+fill', 'Mailing-list participation'), ('type_of_search=mlists', 'envelope-
+fill', 'Mailing-list participation'), (SITEURL, 'megaphone-fill', 'Announcement
+on this blog'), ] %} {% macro render_card(all_tags, project) %}
 {% if project.inactive %}
 Inactive
 {% endif %} {% if project.thumb %} {% if project.thumb_link %}_{_%_ _e_n_d_i_f_ _%_}_ _[_{
 _{_ _p_r_o_j_e_c_t_._n_a_m_e_ _}_}_ _t_h_u_m_b_n_a_i_l_]_{_%_ _i_f_ _p_r_o_j_e_c_t_._t_h_u_m_b___l_i_n_k_ _%_}{% endif %} {% endif %}
 ****** {{{{ pprroojjeecctt..nnaammee }}}} ******
 {% if project.roles or project.tools %}
     * {% for role in project.roles %}
     * {{ role }}
     * {% endfor %} {# Sort by tag frequency, then alphabetically #} {% for tag
       in all_tags|sort(attribute='name')|sort(reverse=True,
       attribute='articles') %} {% if tag.name in project.tools %}
     * {{ m.render_tag(tag) }}
     * {% endif %} {% endfor %} {% set tag_names = [] %} {% for tag in all_tags
-      %} {% if tag_names.append(tag.name) %} {% endif %} {% endfor %} {% for
+      %} {% if tag_names.append(tag.name) %}{% endif %} {% endfor %} {% for
       tool in project.tools %} {% if tool not in tag_names %}
     * {{ tool }}
     * {% endif %} {% endfor %}
 {% endif %} {% if project.desc %}
 {{ project.desc }}
 {% endif %} {% if project.links %}
 {% for link in project.links %} {# Default icon in case of no match #} {% set
-matches = [('', 'fas fa-home', 'Project home')] %} {% for rule in ICONS|reverse
+matches = [('', 'house-fill', 'Project home')] %} {% for rule in ICONS|reverse
 %} {% if rule[0] and link.find(rule[0]) != -1 %} {% if matches.append(rule) %}
 {% endif %} {% endif %} {% endfor %} {% endfor %}
 {% endif %}
 {% endmacro %} {% macro render_projects(projects) %} {% set all_tags = [] %} {%
 for tag, articles in tags %} {% if all_tags.append({'name': tag.name, 'url':
-tag.url, 'articles': articles|length()}) %} {% endif %} {% endfor %} {% if
+tag.url, 'articles': articles|length()}) %}{% endif %} {% endfor %} {% if
 projects is defined %}
-{% block project_pre_content %}{% endblock %} {% set active_projects = [] %} {%
-set inactive_projects = [] %} {% for project in projects %} {% if
-project.inactive %} {% if inactive_projects.append(project) %} {% endif %} {%
-else %} {% if active_projects.append(project) %} {% endif %} {% endif %} {%
-endfor %} {% for project_list in [active_projects, inactive_projects] %} {% for
-project in project_list %}
+{% block project_pre_content %}{% endblock project_pre_content %} {% set
+active_projects = [] %} {% set inactive_projects = [] %} {% for project in
+projects %} {% if project.inactive %} {% if inactive_projects.append(project)
+%}{% endif %} {% else %} {% if active_projects.append(project) %}{% endif %} {%
+endif %} {% endfor %} {% for project_list in [active_projects,
+inactive_projects] %} {% for project in project_list %}
 {{ render_card(all_tags, project) }}
-{% endfor %} {% endfor %} {% block project_post_content %}{% endblock %}
+{% endfor %} {% endfor %} {% block project_post_content %}{% endblock
+project_post_content %}
 {% endif %} {% endmacro %} {% macro render_project_group(group, projects) %} {
 { group.pre }} {{ render_projects(projects) }} {{ group.post }} {% endmacro %}
 {% block extra_js %}
 {% endblock extra_js %} {% block content %} {% if PROJECT_GROUPS is defined %}
 {% for group in PROJECT_GROUPS %} {{ render_project_group(group,
-PROJECTS|selectattr("group", "sameas", group.id)) }} {% endfor %} {
-{ render_projects(PROJECTS|rejectattr("group", "defined")) }} {% else %} {
-{ render_projects(PROJECTS) }} {% endif %} {% endblock %}
+PROJECTS|selectattr("group", "sameas", group.id) ) }} {% endfor %} {
+{ render_projects(PROJECTS|rejectattr("group", "defined") ) }} {% else %} {
+{ render_projects(PROJECTS) }} {% endif %} {% endblock content %}
```

### Comparing `plumage-3.1.0/plumage/templates/tags.html` & `plumage-4.0.0/plumage/templates/tags.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 {% extends "base.html" %}
-{% block title %}All tags{% endblock %}
+{% block title %}All tags{% endblock title %}
 {% block top_center %}
     <h1>
         <a href="{{ SITEURL }}/{{ TAGS_SAVE_AS }}"
            rel="bookmark"
            title="Permalink to tag list">Tags</a>
     </h1>
-{% endblock %}
+{% endblock top_center %}
 {% block content %}
     {% set all_tags = [] %}
     {% for tag, articles in tags %}
-        {% if all_tags.append({'name': tag.name, 'url': tag.url, 'articles': articles|length()}) %}
-        {% endif %}
+        {% if all_tags.append({'name': tag.name, 'url': tag.url, 'articles': articles|length()}) %}{% endif %}
     {% endfor %}
     {% set tier_1 = [] %}
     {% set tier_2 = [] %}
     {% set tier_3 = [] %}
     {% set total_tags = all_tags|sum(attribute = 'articles') %}
     {# Sort by tag frequency, then alphabetically #}
     {% for tag in all_tags|sort(attribute='name')|sort(reverse=True, attribute='articles') %}
         {% if tier_1|sum(attribute = 'articles') < total_tags / 3.0 or tier_1[-1].articles == tag.articles %}
-            {% if tier_1.append(tag) %}
-            {% endif %}
+            {% if tier_1.append(tag) %}{% endif %}
         {% elif tier_2|sum(attribute = 'articles') < total_tags / 3.0 or tier_2[-1].articles == tag.articles %}
-            {% if tier_2.append(tag) %}
-            {% endif %}
+            {% if tier_2.append(tag) %}{% endif %}
         {% else %}
-            {% if tier_3.append(tag) %}
-            {% endif %}
+            {% if tier_3.append(tag) %}{% endif %}
         {% endif %}
     {% endfor %}
     {% for (tier_name, tier_tags) in [("Top", tier_1), ("Middle", tier_2), ("Lower", tier_3)] %}
         <h2>{{ tier_name }} tier</h2>
         <ul class="list-inline">
-            {% for tag in tier_tags %}
-                <li class="list-inline-item">{{ m.render_tag(tag) }}</li>
-            {% endfor %}
+            {% for tag in tier_tags %}<li class="list-inline-item">{{ m.render_tag(tag, counter=tag.articles) }}</li>{% endfor %}
         </ul>
     {% endfor %}
-{% endblock %}
+{% endblock content %}
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-{% extends "base.html" %} {% block title %}All tags{% endblock %} {% block
-top_center %}
+{% extends "base.html" %} {% block title %}All tags{% endblock title %} {%
+block top_center %}
 ************ _TT_aa_gg_ss ************
-{% endblock %} {% block content %} {% set all_tags = [] %} {% for tag, articles
-in tags %} {% if all_tags.append({'name': tag.name, 'url': tag.url, 'articles':
-articles|length()}) %} {% endif %} {% endfor %} {% set tier_1 = [] %} {% set
-tier_2 = [] %} {% set tier_3 = [] %} {% set total_tags = all_tags|sum(attribute
-= 'articles') %} {# Sort by tag frequency, then alphabetically #} {% for tag in
-all_tags|sort(attribute='name')|sort(reverse=True, attribute='articles') %} {%
-if tier_1|sum(attribute = 'articles') < total_tags / 3.0 or tier_1[-1].articles
-== tag.articles %} {% if tier_1.append(tag) %} {% endif %} {% elif tier_2|sum
-(attribute = 'articles') < total_tags / 3.0 or tier_2[-1].articles ==
-tag.articles %} {% if tier_2.append(tag) %} {% endif %} {% else %} {% if
-tier_3.append(tag) %} {% endif %} {% endif %} {% endfor %} {% for (tier_name,
-tier_tags) in [("Top", tier_1), ("Middle", tier_2), ("Lower", tier_3)] %}
+{% endblock top_center %} {% block content %} {% set all_tags = [] %} {% for
+tag, articles in tags %} {% if all_tags.append({'name': tag.name, 'url':
+tag.url, 'articles': articles|length()}) %}{% endif %} {% endfor %} {% set
+tier_1 = [] %} {% set tier_2 = [] %} {% set tier_3 = [] %} {% set total_tags =
+all_tags|sum(attribute = 'articles') %} {# Sort by tag frequency, then
+alphabetically #} {% for tag in all_tags|sort(attribute='name')|sort
+(reverse=True, attribute='articles') %} {% if tier_1|sum(attribute =
+'articles') < total_tags / 3.0 or tier_1[-1].articles == tag.articles %} {% if
+tier_1.append(tag) %}{% endif %} {% elif tier_2|sum(attribute = 'articles') <
+total_tags / 3.0 or tier_2[-1].articles == tag.articles %} {% if tier_2.append
+(tag) %}{% endif %} {% else %} {% if tier_3.append(tag) %}{% endif %} {% endif
+%} {% endfor %} {% for (tier_name, tier_tags) in [("Top", tier_1), ("Middle",
+tier_2), ("Lower", tier_3)] %}
 ********** {{{{ ttiieerr__nnaammee }}}} ttiieerr **********
     * {% for tag in tier_tags %}
-    * {{ m.render_tag(tag) }}
+    * {{ m.render_tag(tag, counter=tag.articles) }}
     * {% endfor %}
-{% endfor %} {% endblock %}
+{% endfor %} {% endblock content %}
```

### Comparing `plumage-3.1.0/plumage/webassets.py` & `plumage-4.0.0/plumage/webassets.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,96 +10,128 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 
+import importlib
 import os
 from pathlib import Path
 from shutil import which
 from textwrap import indent
 from typing import Any
 
 from pynpm import NPMPackage
 
 from . import PLUMAGE_ROOT, logger
 
 """Setup the `webassets <https://github.com/miracle2k/webassets>`_ plugin for Pelican.
-
-Takes care of:
-
-    - Installing PostCSS CLI and its dependency with ``npm``.
-    - Locating the PostCSS CLI binary on the filesystem.
-    - Registering PostCSS to the webassets plugin.
 """
 
 
 CONFIG_DEFAULTS: dict[str, str] = {
     # No need to force a compressed rendering, a minification pass is applied
     # at the end of the pipeline. See:
     # https://webassets.readthedocs.io/en/latest/builtin_filters.html#webassets.filter.libsass.LibSass
     # "LIBSASS_STYLE": "compressed",
 }
 """Default configuration for `webassets <https://github.com/miracle2k/webassets>`_.
 
-See the
-`list of configuration parameters for each filter<https://webassets.readthedocs.io/en/latest/builtin_filters.html>`_.
+See the `list of configuration parameters for each filter
+<https://webassets.readthedocs.io/en/latest/builtin_filters.html>`_.
 """
 
 
-CLI_NAME = "postcss"
+POSTCSS_CLI_NAME = "postcss"
 """Name of the PostCSS CLI binary."""
 
+CLOSURE_JAR_NAME = "closure.jar"
+"""Name of the Closure CLI jar file."""
 
-def setup_webassets(conf: dict[str, Any]) -> dict[str, Any]:
-    """Setup pelican-webassets plugin configuration."""
-    # Update the default configuration with user-defined values.
-    webassets_conf = CONFIG_DEFAULTS.copy()
-    webassets_conf.update(dict(conf.get("WEBASSETS_CONFIG", {})))
 
+def postcss_config():
+    """Produce the default configuration for PostCSS.
+
+    Takes care of:
+
+        - Installing PostCSS CLI and its dependency with ``npm``.
+        - Locating the PostCSS CLI binary on the filesystem.
+        - Registering PostCSS to the webassets plugin.
+    """
     # The dependency definition file relative to Plumage's install path takes
     # precedence.
     node_deps_file = PLUMAGE_ROOT.joinpath("package.json").resolve()
     node_bin_path = node_deps_file.parent / "node_modules" / ".bin"
     cli_search_path = [
         str(node_bin_path),
     ]
 
     # Check if the path exist in any of the environment locations.
-    env_path = os.pathsep.join(cli_search_path + [os.getenv("PATH")])
-    postcss_bin = which(CLI_NAME, path=env_path)
+    env_path = os.pathsep.join([*cli_search_path, os.getenv("PATH")])
+    postcss_bin = which(POSTCSS_CLI_NAME, path=env_path)
 
     if not postcss_bin:
-        logger.warning(f"{CLI_NAME} CLI not found.")
+        logger.warning(f"{POSTCSS_CLI_NAME} CLI not found.")
 
         # Install Node dependencies.
         logger.info(
             f"Install Plumage's Node.js dependencies from {node_deps_file}:\n"
-            f"{indent(node_deps_file.read_text(), ' ' * 2)}"
+            f"{indent(node_deps_file.read_text(), ' ' * 2)}",
         )
         pkg = NPMPackage(node_deps_file)
         try:
             pkg.install()
         except FileNotFoundError:
             logger.error("npm CLI not found.")
             raise
 
-        postcss_bin = which(CLI_NAME, path=env_path)
+        postcss_bin = which(POSTCSS_CLI_NAME, path=env_path)
         assert postcss_bin
 
-    # Register PostCSS to webassets plugin.
-    postcss_bin = Path(postcss_bin).resolve()
-    logger.info(f"{CLI_NAME} CLI found at {postcss_bin}")
-    if "POSTCSS_BIN" not in webassets_conf:
-        webassets_conf["POSTCSS_BIN"] = str(postcss_bin)
-
-    # Force usage of autoprefixer via PostCSS.
-    if "POSTCSS_EXTRA_ARGS" not in webassets_conf:
-        webassets_conf["POSTCSS_EXTRA_ARGS"] = ["--use", "autoprefixer"]
+    logger.info(f"{POSTCSS_CLI_NAME} CLI found at {postcss_bin}")
+
+    return {
+        "POSTCSS_BIN": postcss_bin,
+        # Force usage of autoprefixer via PostCSS.
+        "POSTCSS_EXTRA_ARGS": ["--use", "autoprefixer"],
+    }
+
+
+def closure_config():
+    """Locate the Closure CLI jar file provided by the ``closure`` package.
+
+    .. warning::
+
+        We need to locate the ``closure`` Python package without loading it, as it is
+        old and unmaintained and produce the following error on calling
+        ``import closure``:
+
+            .. code-block:: pytb
+                Traceback (most recent call last):
+                File "<string>", line 1, in <module>
+                File ".../python3.12/site-packages/closure/__init__.py", line 3, in <module>
+                    from pkg_resources import resource_filename
+                ModuleNotFoundError: No module named 'pkg_resources'
+    """
+    package = importlib.util.find_spec("closure")
+    closure_jar = (Path(package.origin).parent / CLOSURE_JAR_NAME).resolve()
+    logger.info(f"{CLOSURE_JAR_NAME} JAR file found at {closure_jar}")
+    return {
+        "CLOSURE_COMPRESSOR_PATH": str(closure_jar),
+    }
+
+
+def setup_webassets(conf: dict[str, Any]) -> dict[str, Any]:
+    """Setup pelican-webassets plugin configuration."""
+    # Merge static and dynamic configurations to produce webassets' defaults.
+    default_conf = CONFIG_DEFAULTS.copy() | postcss_config() | closure_config()
+
+    # Update the default configuration with user-defined values.
+    webassets_conf = default_conf | dict(conf.get("WEBASSETS_CONFIG", {}))
 
     # Save updated configuration in Pelican settings in the form of ``(key, value)``
     # instead of a ``dict`` as expected by ``webassets`` plugin. See:
     # https://github.com/pelican-plugins/webassets/blob/2.0.0/README.md#webassets_config
     conf["WEBASSETS_CONFIG"] = list(webassets_conf.items())
 
     return conf
```

### Comparing `plumage-3.1.0/pyproject.toml` & `plumage-4.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,100 @@
 [tool.poetry]
 # Docs: https://python-poetry.org/docs/pyproject/
 name = "plumage"
-version = "3.1.0"
+version = "4.0.0"
 description = "Clean and tidy theme for Pelican."
 license = 'GPL-2.0-or-later'
 authors = ["Kevin Deldycke <kevin@deldycke.com>"]
 readme = "readme.md"
 homepage = 'https://github.com/kdeldycke/plumage'
 repository = 'https://github.com/kdeldycke/plumage'
 documentation = 'https://github.com/kdeldycke/plumage#settings'
 keywords = [
     'pelican',
     'pelican-theme',
     'stork',
     'static-search',
     'masonry',
+    'myst',
     'theme',
     'bootstrap',
     'jquery',
-    'font-awesome',
 ]
 classifiers = [
     # See: https://pypi.org/pypi?%3Aaction=list_classifiers
     'Development Status :: 5 - Production/Stable',
     'Environment :: Plugins',
     'Environment :: Web Environment',
     'Framework :: Pelican :: Themes',
     'Intended Audience :: Developers',
     'Intended Audience :: Information Technology',
     'Operating System :: OS Independent',
     'Programming Language :: JavaScript',
     'Programming Language :: Other',
     'Topic :: Internet :: WWW/HTTP',
+    'Topic :: Internet :: WWW/HTTP :: Indexing/Search',
     'Topic :: Text Processing :: Markup :: HTML',
+    'Topic :: Text Processing :: Markup :: Markdown',
     'Typing :: Typed',
 ]
 
 [tool.poetry.urls]
 "Funding" = "https://github.com/sponsors/kdeldycke"
 "Issues" = "https://github.com/kdeldycke/plumage/issues"
 "Changelog" = "https://github.com/kdeldycke/plumage/blob/main/changelog.md#changelog"
 
 [tool.poetry.dependencies]
 # List of python versions and their support status:
 # https://en.wikipedia.org/wiki/History_of_Python#Support
-python = "^3.8"
-closure = "^20191111"          # XXX Unmaintained!
-cssmin = "^0.2.0"              # XXX Unmaintained!
-libsass = "^0.22.0"
-Markdown = "^3.4.1"
+python = "^3.9"
+closure = "^20191111"            # XXX Unmaintained!
+cssmin = "^0.2.0"                # XXX Unmaintained!
+libsass = "^0.23.0"
 pelican = "^4.8.0"
+pelican-myst-reader = "^1.3.0b1"
+# pelican-myst-reader = { git = "https://github.com/ashwinvis/myst-reader.git", branch = "main" }
+# pelican-myst-reader = { path = "../myst-reader/", develop = false } # XXX Dev!
 pelican-webassets = "^2.0.0"
-pygments = "^2.14.0"
-pymdown-extensions = "^10.0.1"
-pynpm = "^0.1.2"
+pynpm = "^0.2.0"
 pyquery = "^2.0.0"
 
 [tool.poetry.group.dev.dependencies]
-bump2version = "^1.0.1"
 djlint = "^1.30.2"
 mypy = "^1.1"
-types-Pygments = "^2.14.0"
 
 [tool.mypy]
 warn_unused_configs = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_return_any = true
 warn_unreachable = true
 pretty = true
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
 module = ["pyquery", "pynpm", "pelican.*"]
 
+[tool.bumpversion]
+current_version = "4.0.0"
+allow_dirty = true
+
+[[tool.bumpversion.files]]
+# Update Python package version in any __init__.py file.
+glob = "./**/__init__.py"
+ignore_missing_version = true
+
+[[tool.bumpversion.files]]
+# Update version in Poetry section.
+filename = "./pyproject.toml"
+search = 'version = "{current_version}"'
+replace = 'version = "{new_version}"'
+
+[[tool.bumpversion.files]]
+# Update the version in standard Markdown changelog.
+filename = "./changelog.md"
+search = "## [{current_version} (unreleased)]("
+replace = "## [{new_version} (unreleased)]("
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `plumage-3.1.0/readme.md` & `plumage-4.0.0/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 
 - Standard Pelican views:
 
   |      ![Plumage article view](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/article.jpeg)      | ![Plumage categories view](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/categories.jpeg) | ![Plumage tiered tag list view](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/tiered-tags.jpeg) |
   | :------------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------: |
   |                                                       Article                                                        |                                                    Categories                                                    |                                                    Tiered tag list                                                     |
   |     ![Plumage archive view](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/archives.jpeg)      |        ![Plumage tag view](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/tag.jpeg)        |       ![Plumage authors view](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/authors.jpeg)       |
-  |                                             Collapsable yearly archives                                              |                                                 Tagged articles                                                  |                                                        Authors                                                         |
+  |                                             Collapsible yearly archives                                              |                                                 Tagged articles                                                  |                                                        Authors                                                         |
   | ![Plumage archive view](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/browse-content-by.jpeg) |                                                                                                                  |                                                                                                                        |
   |                                               Faceted article browsing                                               |                                                                                                                  |                                                                                                                        |
 
 - Projects template:
 
   |             ![Plumage projects: code showcase](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/projects-code.jpeg)              |             ![Plumage projects: videos showcase](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/projects-videos.jpeg)              |             ![Plumage projects: themes showcase](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/projects-themes.jpeg)              |
   | :--------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------: |
   | Code showcase ([source](https://github.com/kdeldycke/kevin-deldycke-blog/blob/ebe0d17a59730457c3016dff77fdfa799a80d756/content/templates/code.html)) | Videos showcase ([source](https://github.com/kdeldycke/kevin-deldycke-blog/blob/f778998376fa5c68f1a02129884b89592b641777/content/templates/videos.html)) | Themes showcase ([source](https://github.com/kdeldycke/kevin-deldycke-blog/blob/f778998376fa5c68f1a02129884b89592b641777/content/templates/themes.html)) |
 
-- Based on [Bootstrap v4](https://getbootstrap.com).
+- Based on [Bootstrap v5](https://getbootstrap.com).
 
 - [Code syntax highlighting](#code-syntax-highlighting) with [30+ styles](https://github.com/pygments/pygments/tree/master/pygments/styles).
 
 - Site-wide static search via [Stork](https://stork-search.net).
 
 - Bare YouTube links in articles gets rendered as embedded videos:
 
@@ -54,28 +54,27 @@
 
   ![Plumage disqus comments](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/disqus.jpeg)
 
 ## Plugins
 
 Plumage has built-in support for the following plugins and extensions:
 
-| Plugin name                                                                                                      | Type               | Status   | Notes                                                                                                         |
-| :--------------------------------------------------------------------------------------------------------------- | :----------------- | :------- | :------------------------------------------------------------------------------------------------------------ |
-| [`pelican-image-process`](https://github.com/pelican-plugins/image-process)                                      | Pelican plugin     | Optional | Embed a hack to [fix parsing of external images](https://github.com/pelican-plugins/image-process/issues/33). |
-| [`pelican-neighbors`](https://github.com/pelican-plugins/neighbors)                                              | Pelican plugin     | Optional |                                                                                                               |
-| [`pelican-related-posts`](https://github.com/pelican-plugins/related-posts)                                      | Pelican plugin     | Optional |                                                                                                               |
-| [`pelican-similar-posts`](https://github.com/pelican-plugins/similar-posts)                                      | Pelican plugin     | Optional |                                                                                                               |
-| [`pelican-search`](https://github.com/pelican-plugins/search)                                                    | Pelican plugin     | Optional |                                                                                                               |
-| [`pelican-webassets`](https://github.com/pelican-plugins/webassets)                                              | Pelican plugin     | Required |                                                                                                               |
-| [`markdown.extensions.admonition`](https://python-markdown.github.io/extensions/admonition/)                     | Markdown extension | Optional | Re-style admonitions into [alerts](https://getbootstrap.com/docs/4.5/components/alerts/).                     |
-| [`markdown.extensions.codehilite`](https://python-markdown.github.io/extensions/code_hilite/)                    | Markdown extension | Optional | Style highlighted code with Pygment style.                                                                    |
-| [`markdown.extensions.toc`](https://python-markdown.github.io/extensions/toc/#usage)                             | Markdown extension | Optional | Adds permalink anchors to article's subtitles.                                                                |
-| [`pymdownx.emoji`](https://facelessuser.github.io/pymdown-extensions/extensions/emoji/#default-emoji-generators) | Markdown extension | Optional | Style `emojione` set for proper integration into text.                                                        |
-| [`pymdownx.highlight`](https://facelessuser.github.io/pymdown-extensions/extensions/highlight/)                  | Markdown extension | Optional | Style highlighted code with Pygment style.                                                                    |
-| [`typogrify`](https://pypi.python.org/pypi/typogrify)                                                            | Pelican builtin    | Optional | Style ampersands.                                                                                             |
+| Plugin name                                                                                     | Type               | Status   | Notes                                                                                                         |
+| :---------------------------------------------------------------------------------------------- | :----------------- | :------- | :------------------------------------------------------------------------------------------------------------ |
+| [`pelican-image-process`](https://github.com/pelican-plugins/image-process)                     | Pelican plugin     | Optional | Embed a hack to [fix parsing of external images](https://github.com/pelican-plugins/image-process/issues/33). |
+| [`pelican-neighbors`](https://github.com/pelican-plugins/neighbors)                             | Pelican plugin     | Optional |                                                                                                               |
+| [`pelican-related-posts`](https://github.com/pelican-plugins/related-posts)                     | Pelican plugin     | Optional |                                                                                                               |
+| [`pelican-similar-posts`](https://github.com/pelican-plugins/similar-posts)                     | Pelican plugin     | Optional |                                                                                                               |
+| [`pelican-search`](https://github.com/pelican-plugins/search)                                   | Pelican plugin     | Optional |                                                                                                               |
+| [`pelican-webassets`](https://github.com/pelican-plugins/webassets)                             | Pelican plugin     | Required |                                                                                                               |
+| [`markdown.extensions.admonition`](https://python-markdown.github.io/extensions/admonition/)    | Markdown extension | Optional | Re-style admonitions into [alerts](https://getbootstrap.com/docs/4.5/components/alerts/).                     |
+| [`markdown.extensions.codehilite`](https://python-markdown.github.io/extensions/code_hilite/)   | Markdown extension | Optional | Style highlighted code with Pygment style.                                                                    |
+| [`markdown.extensions.toc`](https://python-markdown.github.io/extensions/toc/#usage)            | Markdown extension | Optional | Adds permalink anchors to article's subtitles.                                                                |
+| [`pymdownx.highlight`](https://facelessuser.github.io/pymdown-extensions/extensions/highlight/) | Markdown extension | Optional | Style highlighted code with Pygment style.                                                                    |
+| [`typogrify`](https://pypi.python.org/pypi/typogrify)                                           | Pelican builtin    | Optional | Style ampersands.                                                                                             |
 
 ## Installation
 
 Install this theme using the `main` branch of this Github repo.
 
 If you're already using `poetry` to manage dependency of Pelican project, you need to run just
 
@@ -90,37 +89,32 @@
 ```
 
 Once added, run `poetry update` to reflect this new dependency.
 
 **Note:** If you haven't used `poetry` in the project yet, you need to do so before adding `plumage`.
 You can do that by first [installing `poetry`](https://python-poetry.org/docs/#installation) on your system and then running `poetry init` inside the project folder.
 
-Then, once you're done installing the `plumage` module, update your `pelicanconf.py` file to reference the module and requied extra plugins:
+Then, once you're done installing the `plumage` module, update your `pelicanconf.py` file to reference the module:
 
 ```python
 import plumage
 
 THEME = plumage.get_path()
-
-PLUGINS = [
-    (…)
-    "pelican.plugins.webassets",
-]
 ```
 
 On first run, Plumage will try to install [Node.js package dependencies](https://github.com/kdeldycke/plumage/blob/main/plumage/package.json) via the `npm` CLI:
 
 ```shell-session
 $ poetry run pelican --verbose ./content
 (…)
 WARNING: postcss CLI not found.
 -> Install Plumage's Node.js dependencies from (…)/plumage/package.json:
   |   {
   |     "name": "plumage-webassets-pipeline",
-  |     "description": "Plumage depdencies for the webassets compilation pipeline.",
+  |     "description": "Plumage dependencies for the webassets compilation pipeline.",
   |     "dependencies": {
   |       "postcss-cli": "^8.3.1"
   |     }
   |   }
   |
 
 up to date, audited 96 packages in 984ms
@@ -128,30 +122,30 @@
 found 0 vulnerabilities
 -> postcss CLI found at (…)/plumage/node_modules/.bin/postcss
 (…)
 ```
 
 ## Settings
 
-Plumage can be customized by adding these optionnal parameters to your
+Plumage can be customized by adding these optional parameters to your
 `pelicanconf.py` file:
 
 | Setting name                                                                                  | Default value | Description                                                                                                                                                    |
 | :-------------------------------------------------------------------------------------------- | :------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `ARTICLE_EDIT_LINK`                                                                           |               | Generate an edit link besides each article. Can use `%(slug)s` to include dynamic article's slug in the link.                                                  |
 | `CODE_STYLE`                                                                                  | `"monokai"`   | Pygments' style ID. Choose one from `poetry run pygmentize -L styles`.                                                                                         |
 | `COPYRIGHT`                                                                                   |               | Additional copyright statement to add in the third column of the footer.                                                                                       |
-| `DISCLAIMER`                                                                                  |               | Overide the disclaimer notice that gets displayed at the fourth column of the footer.                                                                          |
+| `DISCLAIMER`                                                                                  |               | Override the disclaimer notice that gets displayed at the fourth column of the footer.                                                                         |
 | [`DISQUS_SITENAME`](http://docs.getpelican.com/en/stable/settings.html#DISQUS_SITENAME)       |               | Pelican can handle Disqus comments. Specify the Disqus sitename identifier here.                                                                               |
 | `FAVICON_LINKS`                                                                               | `True`        | Fetch link's icons from [Google's favicons webservice](https://www.google.com/s2/favicons).                                                                    |
 | [`GOOGLE_ANALYTICS`](http://docs.getpelican.com/en/stable/settings.html#GOOGLE_ANALYTICS)     |               | Set to `UA-XXXXXX-Y` Property's tracking ID to activate Google Analytics.                                                                                      |
 | `LEFT_SIDEBAR`                                                                                |               | HTML content to put as-is in the left sidebar.                                                                                                                 |
 | [`LINKS_WIDGET_NAME`](http://docs.getpelican.com/en/stable/settings.html#LINKS_WIDGET_NAME)   | `"Links"`     | Allows override of the name of the links widget.                                                                                                               |
 | [`LINKS`](http://docs.getpelican.com/en/stable/settings.html#LINKS)                           |               | A list of tuples (Title, URL) for links to appear in the second column of the footer.                                                                          |
-| [`MANUAL_LINKS`](http://docs.getpelican.com/en/stable/settings.html#MANUAL_LINKS)             |               | When enabling this, you must pass the links (in LINKS & SOCIAL settins) not as tuples anymore, but as list, where every entry is formatted as you like         |
+| [`MANUAL_LINKS`](http://docs.getpelican.com/en/stable/settings.html#MANUAL_LINKS)             |               | When enabling this, you must pass the links (in LINKS & SOCIAL settings) not as tuples anymore, but as list, where every entry is formatted as you like        |
 | [`MENUITEMS`](http://docs.getpelican.com/en/stable/settings.html#MENUITEMS)                   |               | A list of tuples (Title, URL) for additional menu items to appear at the beginning of the main menu.                                                           |
 | `RIGHT_SIDEBAR`                                                                               |               | HTML content to put as-is in the right sidebar.                                                                                                                |
 | [`SITESUBTITLE`](http://docs.getpelican.com/en/stable/settings.html#SITESUBTITLE)             |               | A subtitle to appear in the header.                                                                                                                            |
 | `SITE_THUMBNAIL_TEXT`                                                                         |               | Text displayed behind site's thumbnail.                                                                                                                        |
 | `SITE_THUMBNAIL`                                                                              |               | Site's thumbnail URL as displayed in the header. Should be a square image of at least 80x80 pixels.                                                            |
 | [`SOCIAL_WIDGET_NAME`](http://docs.getpelican.com/en/stable/settings.html#SOCIAL_WIDGET_NAME) | `"Social"`    | Allows override of the name of the “social” widget.                                                                                                            |
 | [`SOCIAL`](http://docs.getpelican.com/en/stable/settings.html#SOCIAL)                         |               | A list of tuples (Title, URL) to appear in the first columns of the footer.                                                                                    |
@@ -310,14 +304,24 @@
 ```
 ````
 
 Into this:
 
 ![Plumage PyMdown Extensions' Highlight rendering](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/highlight-rendering.jpeg)
 
+## CSS customization
+
+TODO: document all kind customization below
+
+### Python code transforms at generation via `pyquery`
+
+### Use of `extra_css`
+
+### Custom `main.scss`
+
 ## FAQ
 
 ### How can I disable the zoom on images?
 
 All images of an article are zoomable by default. You can deactivate the
 magnifying glass per-image by adding a `noZoom` CSS class. So instead of the
 following Markdown code:
@@ -345,15 +349,15 @@
 (GPLv2+)](https://github.com/kdeldycke/plumage/blob/main/LICENSE).
 
 Copyright (C) 2012-2020 [Kevin Deldycke](https://kevin.deldycke.com) and
 [contributors](https://github.com/kdeldycke/plumage/graphs/contributors).
 
 ## Third-party assets
 
-The theme embed copies of some external softwares, scripts, libraries and
+The theme embed copies of some external software, scripts, libraries and
 artworks:
 
 ```text
 jQuery MGlass v1.1
 Copyright (c) 2012 Younès El Biache
 Distributed under a MIT license
 Source: https://github.com/younes0/jQuery-MGlass
```

#### html2text {}

```diff
@@ -12,15 +12,15 @@
 ----------------------------------------------------------------------------: |
 :------------------------------------------------------------------------------
 --------------------------------------: | | Article | Categories | Tiered tag
 list | | ![Plumage archive view](https://raw.githubusercontent.com/kdeldycke/
 plumage/main/screenshots/archives.jpeg) | ![Plumage tag view](https://
 raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/tag.jpeg) | !
 [Plumage authors view](https://raw.githubusercontent.com/kdeldycke/plumage/
-main/screenshots/authors.jpeg) | | Collapsable yearly archives | Tagged
+main/screenshots/authors.jpeg) | | Collapsible yearly archives | Tagged
 articles | Authors | | ![Plumage archive view](https://
 raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/browse-content-
 by.jpeg) | | | | Faceted article browsing | | | - Projects template: | !
 [Plumage projects: code showcase](https://raw.githubusercontent.com/kdeldycke/
 plumage/main/screenshots/projects-code.jpeg) | ![Plumage projects: videos
 showcase](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/
 projects-videos.jpeg) | ![Plumage projects: themes showcase](https://
@@ -33,15 +33,15 @@
 ------------------------------------------------------------------------------
 -: | | Code showcase ([source](https://github.com/kdeldycke/kevin-deldycke-
 blog/blob/ebe0d17a59730457c3016dff77fdfa799a80d756/content/templates/
 code.html)) | Videos showcase ([source](https://github.com/kdeldycke/kevin-
 deldycke-blog/blob/f778998376fa5c68f1a02129884b89592b641777/content/templates/
 videos.html)) | Themes showcase ([source](https://github.com/kdeldycke/kevin-
 deldycke-blog/blob/f778998376fa5c68f1a02129884b89592b641777/content/templates/
-themes.html)) | - Based on [Bootstrap v4](https://getbootstrap.com). - [Code
+themes.html)) | - Based on [Bootstrap v5](https://getbootstrap.com). - [Code
 syntax highlighting](#code-syntax-highlighting) with [30+ styles](https://
 github.com/pygments/pygments/tree/master/pygments/styles). - Site-wide static
 search via [Stork](https://stork-search.net). - Bare YouTube links in articles
 gets rendered as embedded videos: ![Plumage YouTube link](https://
 raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/youtube-link.jpeg)
 - Direct link to edit articles on GitHub: ![Plumage GitHub edit link](https://
 raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/github-edit-
@@ -50,37 +50,34 @@
 screenshots/magnifying-glass.jpeg) ![Plumage image zoom](https://
 raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/zoom.jpeg) -
 External assets (Bootstrap, Jquery, etc...) uses [CDNjs ](https://cdnjs.com/
 about). - Disqus integration: ![Plumage disqus comments](https://
 raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/disqus.jpeg) ##
 Plugins Plumage has built-in support for the following plugins and extensions:
 | Plugin name | Type | Status | Notes | | :------------------------------------
---------------------------------------------------------------------------- | :
------------------ | :------- | :-----------------------------------------------
-------------------------------------------------------------- | | [`pelican-
-image-process`](https://github.com/pelican-plugins/image-process) | Pelican
-plugin | Optional | Embed a hack to [fix parsing of external images](https://
-github.com/pelican-plugins/image-process/issues/33). | | [`pelican-neighbors`]
-(https://github.com/pelican-plugins/neighbors) | Pelican plugin | Optional | |
-| [`pelican-related-posts`](https://github.com/pelican-plugins/related-posts) |
-Pelican plugin | Optional | | | [`pelican-similar-posts`](https://github.com/
-pelican-plugins/similar-posts) | Pelican plugin | Optional | | | [`pelican-
-search`](https://github.com/pelican-plugins/search) | Pelican plugin | Optional
-| | | [`pelican-webassets`](https://github.com/pelican-plugins/webassets) |
-Pelican plugin | Required | | | [`markdown.extensions.admonition`](https://
-python-markdown.github.io/extensions/admonition/) | Markdown extension |
-Optional | Re-style admonitions into [alerts](https://getbootstrap.com/docs/
-4.5/components/alerts/). | | [`markdown.extensions.codehilite`](https://python-
+---------------------------------------------------------- | :----------------
+- | :------- | :---------------------------------------------------------------
+--------------------------------------------- | | [`pelican-image-process`]
+(https://github.com/pelican-plugins/image-process) | Pelican plugin | Optional
+| Embed a hack to [fix parsing of external images](https://github.com/pelican-
+plugins/image-process/issues/33). | | [`pelican-neighbors`](https://github.com/
+pelican-plugins/neighbors) | Pelican plugin | Optional | | | [`pelican-related-
+posts`](https://github.com/pelican-plugins/related-posts) | Pelican plugin |
+Optional | | | [`pelican-similar-posts`](https://github.com/pelican-plugins/
+similar-posts) | Pelican plugin | Optional | | | [`pelican-search`](https://
+github.com/pelican-plugins/search) | Pelican plugin | Optional | | | [`pelican-
+webassets`](https://github.com/pelican-plugins/webassets) | Pelican plugin |
+Required | | | [`markdown.extensions.admonition`](https://python-
+markdown.github.io/extensions/admonition/) | Markdown extension | Optional |
+Re-style admonitions into [alerts](https://getbootstrap.com/docs/4.5/
+components/alerts/). | | [`markdown.extensions.codehilite`](https://python-
 markdown.github.io/extensions/code_hilite/) | Markdown extension | Optional |
 Style highlighted code with Pygment style. | | [`markdown.extensions.toc`]
 (https://python-markdown.github.io/extensions/toc/#usage) | Markdown extension
 | Optional | Adds permalink anchors to article's subtitles. | |
-[`pymdownx.emoji`](https://facelessuser.github.io/pymdown-extensions/
-extensions/emoji/#default-emoji-generators) | Markdown extension | Optional |
-Style `emojione` set for proper integration into text. | |
 [`pymdownx.highlight`](https://facelessuser.github.io/pymdown-extensions/
 extensions/highlight/) | Markdown extension | Optional | Style highlighted code
 with Pygment style. | | [`typogrify`](https://pypi.python.org/pypi/typogrify) |
 Pelican builtin | Optional | Style ampersands. | ## Installation Install this
 theme using the `main` branch of this Github repo. If you're already using
 `poetry` to manage dependency of Pelican project, you need to run just
 ```shell-session poetry add git+https://github.com/kdeldycke/plumage#main ```
@@ -88,50 +85,49 @@
 section of the `pyproject.toml` file. ``` plumage = {git = "https://github.com/
 kdeldycke/plumage", rev = "main"} ``` Once added, run `poetry update` to
 reflect this new dependency. **Note:** If you haven't used `poetry` in the
 project yet, you need to do so before adding `plumage`. You can do that by
 first [installing `poetry`](https://python-poetry.org/docs/#installation) on
 your system and then running `poetry init` inside the project folder. Then,
 once you're done installing the `plumage` module, update your `pelicanconf.py`
-file to reference the module and requied extra plugins: ```python import
-plumage THEME = plumage.get_path() PLUGINS = [ (â¦)
-"pelican.plugins.webassets", ] ``` On first run, Plumage will try to install
-[Node.js package dependencies](https://github.com/kdeldycke/plumage/blob/main/
-plumage/package.json) via the `npm` CLI: ```shell-session $ poetry run pelican
---verbose ./content (â¦) WARNING: postcss CLI not found. -> Install Plumage's
-Node.js dependencies from (â¦)/plumage/package.json: | { | "name": "plumage-
-webassets-pipeline", | "description": "Plumage depdencies for the webassets
-compilation pipeline.", | "dependencies": { | "postcss-cli": "^8.3.1" | } | } |
-up to date, audited 96 packages in 984ms found 0 vulnerabilities -> postcss CLI
-found at (â¦)/plumage/node_modules/.bin/postcss (â¦) ``` ## Settings Plumage
-can be customized by adding these optionnal parameters to your `pelicanconf.py`
-file: | Setting name | Default value | Description | | :-----------------------
---------------------------------------------------------------------- | :------
------- | :---------------------------------------------------------------------
--------------------------------------------------------------------------------
---------- | | `ARTICLE_EDIT_LINK` | | Generate an edit link besides each
-article. Can use `%(slug)s` to include dynamic article's slug in the link. | |
-`CODE_STYLE` | `"monokai"` | Pygments' style ID. Choose one from `poetry run
-pygmentize -L styles`. | | `COPYRIGHT` | | Additional copyright statement to
-add in the third column of the footer. | | `DISCLAIMER` | | Overide the
-disclaimer notice that gets displayed at the fourth column of the footer. | |
-[`DISQUS_SITENAME`](http://docs.getpelican.com/en/stable/
-settings.html#DISQUS_SITENAME) | | Pelican can handle Disqus comments. Specify
-the Disqus sitename identifier here. | | `FAVICON_LINKS` | `True` | Fetch
-link's icons from [Google's favicons webservice](https://www.google.com/s2/
-favicons). | | [`GOOGLE_ANALYTICS`](http://docs.getpelican.com/en/stable/
-settings.html#GOOGLE_ANALYTICS) | | Set to `UA-XXXXXX-Y` Property's tracking ID
-to activate Google Analytics. | | `LEFT_SIDEBAR` | | HTML content to put as-is
-in the left sidebar. | | [`LINKS_WIDGET_NAME`](http://docs.getpelican.com/en/
-stable/settings.html#LINKS_WIDGET_NAME) | `"Links"` | Allows override of the
-name of the links widget. | | [`LINKS`](http://docs.getpelican.com/en/stable/
+file to reference the module: ```python import plumage THEME = plumage.get_path
+() ``` On first run, Plumage will try to install [Node.js package dependencies]
+(https://github.com/kdeldycke/plumage/blob/main/plumage/package.json) via the
+`npm` CLI: ```shell-session $ poetry run pelican --verbose ./content (â¦)
+WARNING: postcss CLI not found. -> Install Plumage's Node.js dependencies from
+(â¦)/plumage/package.json: | { | "name": "plumage-webassets-pipeline", |
+"description": "Plumage dependencies for the webassets compilation pipeline.",
+| "dependencies": { | "postcss-cli": "^8.3.1" | } | } | up to date, audited 96
+packages in 984ms found 0 vulnerabilities -> postcss CLI found at (â¦)/
+plumage/node_modules/.bin/postcss (â¦) ``` ## Settings Plumage can be
+customized by adding these optional parameters to your `pelicanconf.py` file: |
+Setting name | Default value | Description | | :-------------------------------
+------------------------------------------------------------- | :------------ |
+:------------------------------------------------------------------------------
+------------------------------------------------------------------------------
+- | | `ARTICLE_EDIT_LINK` | | Generate an edit link besides each article. Can
+use `%(slug)s` to include dynamic article's slug in the link. | | `CODE_STYLE`
+| `"monokai"` | Pygments' style ID. Choose one from `poetry run pygmentize -
+L styles`. | | `COPYRIGHT` | | Additional copyright statement to add in the
+third column of the footer. | | `DISCLAIMER` | | Override the disclaimer notice
+that gets displayed at the fourth column of the footer. | | [`DISQUS_SITENAME`]
+(http://docs.getpelican.com/en/stable/settings.html#DISQUS_SITENAME) | |
+Pelican can handle Disqus comments. Specify the Disqus sitename identifier
+here. | | `FAVICON_LINKS` | `True` | Fetch link's icons from [Google's favicons
+webservice](https://www.google.com/s2/favicons). | | [`GOOGLE_ANALYTICS`](http:
+//docs.getpelican.com/en/stable/settings.html#GOOGLE_ANALYTICS) | | Set to `UA-
+XXXXXX-Y` Property's tracking ID to activate Google Analytics. | |
+`LEFT_SIDEBAR` | | HTML content to put as-is in the left sidebar. | |
+[`LINKS_WIDGET_NAME`](http://docs.getpelican.com/en/stable/
+settings.html#LINKS_WIDGET_NAME) | `"Links"` | Allows override of the name of
+the links widget. | | [`LINKS`](http://docs.getpelican.com/en/stable/
 settings.html#LINKS) | | A list of tuples (Title, URL) for links to appear in
 the second column of the footer. | | [`MANUAL_LINKS`](http://
 docs.getpelican.com/en/stable/settings.html#MANUAL_LINKS) | | When enabling
-this, you must pass the links (in LINKS & SOCIAL settins) not as tuples
+this, you must pass the links (in LINKS & SOCIAL settings) not as tuples
 anymore, but as list, where every entry is formatted as you like | |
 [`MENUITEMS`](http://docs.getpelican.com/en/stable/settings.html#MENUITEMS) | |
 A list of tuples (Title, URL) for additional menu items to appear at the
 beginning of the main menu. | | `RIGHT_SIDEBAR` | | HTML content to put as-is
 in the right sidebar. | | [`SITESUBTITLE`](http://docs.getpelican.com/en/
 stable/settings.html#SITESUBTITLE) | | A subtitle to appear in the header. | |
 `SITE_THUMBNAIL_TEXT` | | Text displayed behind site's thumbnail. | |
@@ -192,32 +188,34 @@
 linenums="5 1 3" filename="~/code/foo.log"} $ cat ./example.markdown This is
 the content of the file: â java â rust â haskell â javascript $ cat ./
 addendum.txt This is extra content. $ find ./ -iname "*.markdown" -print -exec
 bash -c 'cat ./addendum.txt >> "{}"' \; ./example.markdown $ cat ./
 example.markdown This is the content of the file: â java â rust â haskell
 â javascript This is extra content. ``` ```` Into this: ![Plumage PyMdown
 Extensions' Highlight rendering](https://raw.githubusercontent.com/kdeldycke/
-plumage/main/screenshots/highlight-rendering.jpeg) ## FAQ ### How can I disable
-the zoom on images? All images of an article are zoomable by default. You can
-deactivate the magnifying glass per-image by adding a `noZoom` CSS class. So
-instead of the following Markdown code: ```markdown ![Image title](/folder/
-image.png) ``` You have to use the following template to deactivate the zoom of
-an image: ```markdown ![Image title](/folder/image.png){: .noZoom} ``` ### Why
-is the search not working? The [official Pelican's `search` plugin](https://
-github.com/pelican-plugins/search) needs to be installed. TODO: Activate search
-field automaticcaly if the plugin is present. ## License This software is
-licensed under the [GNU General Public License v2 or later (GPLv2+)](https://
-github.com/kdeldycke/plumage/blob/main/LICENSE). Copyright (C) 2012-2020 [Kevin
-Deldycke](https://kevin.deldycke.com) and [contributors](https://github.com/
-kdeldycke/plumage/graphs/contributors). ## Third-party assets The theme embed
-copies of some external softwares, scripts, libraries and artworks: ```text
-jQuery MGlass v1.1 Copyright (c) 2012 YounÃ¨s El Biache Distributed under a MIT
-license Source: https://github.com/younes0/jQuery-MGlass ``` ```text Fabric
-(Plaid) Copyright (c) 2012 James Basoo Distributed under a Creative Commons
-Attribution-ShareAlike 3.0 Unported license Source: https://subtlepatterns.com/
-fabric-plaid/ ``` ```text Cream paper Copyright (c) 2012 Devin Holmes
-Distributed under a Creative Commons Attribution-ShareAlike 3.0 Unported
-license Source: https://subtlepatterns.com/cream-paper/ ``` ```text Feather-alt
-icon v5.1.0 Copyright (c) 2020 Font Awesome project Distributed under a
-Creative Commons Attribution 4.0 International license Source: https://
-fontawesome.com/icons/feather-alt?style=solid ``` ```text Macro shot of White
-Feather Source: https://unsplash.com/photos/Sw7f58YJbc0 ```
+plumage/main/screenshots/highlight-rendering.jpeg) ## CSS customization TODO:
+document all kind customization below ### Python code transforms at generation
+via `pyquery` ### Use of `extra_css` ### Custom `main.scss` ## FAQ ### How can
+I disable the zoom on images? All images of an article are zoomable by default.
+You can deactivate the magnifying glass per-image by adding a `noZoom` CSS
+class. So instead of the following Markdown code: ```markdown ![Image title](/
+folder/image.png) ``` You have to use the following template to deactivate the
+zoom of an image: ```markdown ![Image title](/folder/image.png){: .noZoom} ```
+### Why is the search not working? The [official Pelican's `search` plugin]
+(https://github.com/pelican-plugins/search) needs to be installed. TODO:
+Activate search field automaticcaly if the plugin is present. ## License This
+software is licensed under the [GNU General Public License v2 or later
+(GPLv2+)](https://github.com/kdeldycke/plumage/blob/main/LICENSE). Copyright
+(C) 2012-2020 [Kevin Deldycke](https://kevin.deldycke.com) and [contributors]
+(https://github.com/kdeldycke/plumage/graphs/contributors). ## Third-party
+assets The theme embed copies of some external software, scripts, libraries and
+artworks: ```text jQuery MGlass v1.1 Copyright (c) 2012 YounÃ¨s El Biache
+Distributed under a MIT license Source: https://github.com/younes0/jQuery-
+MGlass ``` ```text Fabric (Plaid) Copyright (c) 2012 James Basoo Distributed
+under a Creative Commons Attribution-ShareAlike 3.0 Unported license Source:
+https://subtlepatterns.com/fabric-plaid/ ``` ```text Cream paper Copyright (c)
+2012 Devin Holmes Distributed under a Creative Commons Attribution-ShareAlike
+3.0 Unported license Source: https://subtlepatterns.com/cream-paper/ ```
+```text Feather-alt icon v5.1.0 Copyright (c) 2020 Font Awesome project
+Distributed under a Creative Commons Attribution 4.0 International license
+Source: https://fontawesome.com/icons/feather-alt?style=solid ``` ```text Macro
+shot of White Feather Source: https://unsplash.com/photos/Sw7f58YJbc0 ```
```

### Comparing `plumage-3.1.0/PKG-INFO` & `plumage-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: plumage
-Version: 3.1.0
+Version: 4.0.0
 Summary: Clean and tidy theme for Pelican.
 Home-page: https://github.com/kdeldycke/plumage
 License: GPL-2.0-or-later
-Keywords: pelican,pelican-theme,stork,static-search,masonry,theme,bootstrap,jquery,font-awesome
+Keywords: pelican,pelican-theme,stork,static-search,masonry,myst,theme,bootstrap,jquery
 Author: Kevin Deldycke
 Author-email: kevin@deldycke.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Pelican :: Themes
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Other
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Text Processing :: Markup :: HTML
+Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Typing :: Typed
-Requires-Dist: Markdown (>=3.4.1,<4.0.0)
 Requires-Dist: closure (>=20191111,<20191112)
 Requires-Dist: cssmin (>=0.2.0,<0.3.0)
-Requires-Dist: libsass (>=0.22.0,<0.23.0)
+Requires-Dist: libsass (>=0.23.0,<0.24.0)
 Requires-Dist: pelican (>=4.8.0,<5.0.0)
+Requires-Dist: pelican-myst-reader (>=1.3.0b1,<2.0.0)
 Requires-Dist: pelican-webassets (>=2.0.0,<3.0.0)
-Requires-Dist: pygments (>=2.14.0,<3.0.0)
-Requires-Dist: pymdown-extensions (>=10.0.1,<11.0.0)
-Requires-Dist: pynpm (>=0.1.2,<0.2.0)
+Requires-Dist: pynpm (>=0.2.0,<0.3.0)
 Requires-Dist: pyquery (>=2.0.0,<3.0.0)
 Project-URL: Changelog, https://github.com/kdeldycke/plumage/blob/main/changelog.md#changelog
 Project-URL: Documentation, https://github.com/kdeldycke/plumage#settings
 Project-URL: Funding, https://github.com/sponsors/kdeldycke
 Project-URL: Issues, https://github.com/kdeldycke/plumage/issues
 Project-URL: Repository, https://github.com/kdeldycke/plumage
 Description-Content-Type: text/markdown
@@ -59,25 +59,25 @@
 
 - Standard Pelican views:
 
   |      ![Plumage article view](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/article.jpeg)      | ![Plumage categories view](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/categories.jpeg) | ![Plumage tiered tag list view](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/tiered-tags.jpeg) |
   | :------------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------: |
   |                                                       Article                                                        |                                                    Categories                                                    |                                                    Tiered tag list                                                     |
   |     ![Plumage archive view](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/archives.jpeg)      |        ![Plumage tag view](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/tag.jpeg)        |       ![Plumage authors view](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/authors.jpeg)       |
-  |                                             Collapsable yearly archives                                              |                                                 Tagged articles                                                  |                                                        Authors                                                         |
+  |                                             Collapsible yearly archives                                              |                                                 Tagged articles                                                  |                                                        Authors                                                         |
   | ![Plumage archive view](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/browse-content-by.jpeg) |                                                                                                                  |                                                                                                                        |
   |                                               Faceted article browsing                                               |                                                                                                                  |                                                                                                                        |
 
 - Projects template:
 
   |             ![Plumage projects: code showcase](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/projects-code.jpeg)              |             ![Plumage projects: videos showcase](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/projects-videos.jpeg)              |             ![Plumage projects: themes showcase](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/projects-themes.jpeg)              |
   | :--------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------: |
   | Code showcase ([source](https://github.com/kdeldycke/kevin-deldycke-blog/blob/ebe0d17a59730457c3016dff77fdfa799a80d756/content/templates/code.html)) | Videos showcase ([source](https://github.com/kdeldycke/kevin-deldycke-blog/blob/f778998376fa5c68f1a02129884b89592b641777/content/templates/videos.html)) | Themes showcase ([source](https://github.com/kdeldycke/kevin-deldycke-blog/blob/f778998376fa5c68f1a02129884b89592b641777/content/templates/themes.html)) |
 
-- Based on [Bootstrap v4](https://getbootstrap.com).
+- Based on [Bootstrap v5](https://getbootstrap.com).
 
 - [Code syntax highlighting](#code-syntax-highlighting) with [30+ styles](https://github.com/pygments/pygments/tree/master/pygments/styles).
 
 - Site-wide static search via [Stork](https://stork-search.net).
 
 - Bare YouTube links in articles gets rendered as embedded videos:
 
@@ -99,28 +99,27 @@
 
   ![Plumage disqus comments](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/disqus.jpeg)
 
 ## Plugins
 
 Plumage has built-in support for the following plugins and extensions:
 
-| Plugin name                                                                                                      | Type               | Status   | Notes                                                                                                         |
-| :--------------------------------------------------------------------------------------------------------------- | :----------------- | :------- | :------------------------------------------------------------------------------------------------------------ |
-| [`pelican-image-process`](https://github.com/pelican-plugins/image-process)                                      | Pelican plugin     | Optional | Embed a hack to [fix parsing of external images](https://github.com/pelican-plugins/image-process/issues/33). |
-| [`pelican-neighbors`](https://github.com/pelican-plugins/neighbors)                                              | Pelican plugin     | Optional |                                                                                                               |
-| [`pelican-related-posts`](https://github.com/pelican-plugins/related-posts)                                      | Pelican plugin     | Optional |                                                                                                               |
-| [`pelican-similar-posts`](https://github.com/pelican-plugins/similar-posts)                                      | Pelican plugin     | Optional |                                                                                                               |
-| [`pelican-search`](https://github.com/pelican-plugins/search)                                                    | Pelican plugin     | Optional |                                                                                                               |
-| [`pelican-webassets`](https://github.com/pelican-plugins/webassets)                                              | Pelican plugin     | Required |                                                                                                               |
-| [`markdown.extensions.admonition`](https://python-markdown.github.io/extensions/admonition/)                     | Markdown extension | Optional | Re-style admonitions into [alerts](https://getbootstrap.com/docs/4.5/components/alerts/).                     |
-| [`markdown.extensions.codehilite`](https://python-markdown.github.io/extensions/code_hilite/)                    | Markdown extension | Optional | Style highlighted code with Pygment style.                                                                    |
-| [`markdown.extensions.toc`](https://python-markdown.github.io/extensions/toc/#usage)                             | Markdown extension | Optional | Adds permalink anchors to article's subtitles.                                                                |
-| [`pymdownx.emoji`](https://facelessuser.github.io/pymdown-extensions/extensions/emoji/#default-emoji-generators) | Markdown extension | Optional | Style `emojione` set for proper integration into text.                                                        |
-| [`pymdownx.highlight`](https://facelessuser.github.io/pymdown-extensions/extensions/highlight/)                  | Markdown extension | Optional | Style highlighted code with Pygment style.                                                                    |
-| [`typogrify`](https://pypi.python.org/pypi/typogrify)                                                            | Pelican builtin    | Optional | Style ampersands.                                                                                             |
+| Plugin name                                                                                     | Type               | Status   | Notes                                                                                                         |
+| :---------------------------------------------------------------------------------------------- | :----------------- | :------- | :------------------------------------------------------------------------------------------------------------ |
+| [`pelican-image-process`](https://github.com/pelican-plugins/image-process)                     | Pelican plugin     | Optional | Embed a hack to [fix parsing of external images](https://github.com/pelican-plugins/image-process/issues/33). |
+| [`pelican-neighbors`](https://github.com/pelican-plugins/neighbors)                             | Pelican plugin     | Optional |                                                                                                               |
+| [`pelican-related-posts`](https://github.com/pelican-plugins/related-posts)                     | Pelican plugin     | Optional |                                                                                                               |
+| [`pelican-similar-posts`](https://github.com/pelican-plugins/similar-posts)                     | Pelican plugin     | Optional |                                                                                                               |
+| [`pelican-search`](https://github.com/pelican-plugins/search)                                   | Pelican plugin     | Optional |                                                                                                               |
+| [`pelican-webassets`](https://github.com/pelican-plugins/webassets)                             | Pelican plugin     | Required |                                                                                                               |
+| [`markdown.extensions.admonition`](https://python-markdown.github.io/extensions/admonition/)    | Markdown extension | Optional | Re-style admonitions into [alerts](https://getbootstrap.com/docs/4.5/components/alerts/).                     |
+| [`markdown.extensions.codehilite`](https://python-markdown.github.io/extensions/code_hilite/)   | Markdown extension | Optional | Style highlighted code with Pygment style.                                                                    |
+| [`markdown.extensions.toc`](https://python-markdown.github.io/extensions/toc/#usage)            | Markdown extension | Optional | Adds permalink anchors to article's subtitles.                                                                |
+| [`pymdownx.highlight`](https://facelessuser.github.io/pymdown-extensions/extensions/highlight/) | Markdown extension | Optional | Style highlighted code with Pygment style.                                                                    |
+| [`typogrify`](https://pypi.python.org/pypi/typogrify)                                           | Pelican builtin    | Optional | Style ampersands.                                                                                             |
 
 ## Installation
 
 Install this theme using the `main` branch of this Github repo.
 
 If you're already using `poetry` to manage dependency of Pelican project, you need to run just
 
@@ -135,37 +134,32 @@
 ```
 
 Once added, run `poetry update` to reflect this new dependency.
 
 **Note:** If you haven't used `poetry` in the project yet, you need to do so before adding `plumage`.
 You can do that by first [installing `poetry`](https://python-poetry.org/docs/#installation) on your system and then running `poetry init` inside the project folder.
 
-Then, once you're done installing the `plumage` module, update your `pelicanconf.py` file to reference the module and requied extra plugins:
+Then, once you're done installing the `plumage` module, update your `pelicanconf.py` file to reference the module:
 
 ```python
 import plumage
 
 THEME = plumage.get_path()
-
-PLUGINS = [
-    (…)
-    "pelican.plugins.webassets",
-]
 ```
 
 On first run, Plumage will try to install [Node.js package dependencies](https://github.com/kdeldycke/plumage/blob/main/plumage/package.json) via the `npm` CLI:
 
 ```shell-session
 $ poetry run pelican --verbose ./content
 (…)
 WARNING: postcss CLI not found.
 -> Install Plumage's Node.js dependencies from (…)/plumage/package.json:
   |   {
   |     "name": "plumage-webassets-pipeline",
-  |     "description": "Plumage depdencies for the webassets compilation pipeline.",
+  |     "description": "Plumage dependencies for the webassets compilation pipeline.",
   |     "dependencies": {
   |       "postcss-cli": "^8.3.1"
   |     }
   |   }
   |
 
 up to date, audited 96 packages in 984ms
@@ -173,30 +167,30 @@
 found 0 vulnerabilities
 -> postcss CLI found at (…)/plumage/node_modules/.bin/postcss
 (…)
 ```
 
 ## Settings
 
-Plumage can be customized by adding these optionnal parameters to your
+Plumage can be customized by adding these optional parameters to your
 `pelicanconf.py` file:
 
 | Setting name                                                                                  | Default value | Description                                                                                                                                                    |
 | :-------------------------------------------------------------------------------------------- | :------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `ARTICLE_EDIT_LINK`                                                                           |               | Generate an edit link besides each article. Can use `%(slug)s` to include dynamic article's slug in the link.                                                  |
 | `CODE_STYLE`                                                                                  | `"monokai"`   | Pygments' style ID. Choose one from `poetry run pygmentize -L styles`.                                                                                         |
 | `COPYRIGHT`                                                                                   |               | Additional copyright statement to add in the third column of the footer.                                                                                       |
-| `DISCLAIMER`                                                                                  |               | Overide the disclaimer notice that gets displayed at the fourth column of the footer.                                                                          |
+| `DISCLAIMER`                                                                                  |               | Override the disclaimer notice that gets displayed at the fourth column of the footer.                                                                         |
 | [`DISQUS_SITENAME`](http://docs.getpelican.com/en/stable/settings.html#DISQUS_SITENAME)       |               | Pelican can handle Disqus comments. Specify the Disqus sitename identifier here.                                                                               |
 | `FAVICON_LINKS`                                                                               | `True`        | Fetch link's icons from [Google's favicons webservice](https://www.google.com/s2/favicons).                                                                    |
 | [`GOOGLE_ANALYTICS`](http://docs.getpelican.com/en/stable/settings.html#GOOGLE_ANALYTICS)     |               | Set to `UA-XXXXXX-Y` Property's tracking ID to activate Google Analytics.                                                                                      |
 | `LEFT_SIDEBAR`                                                                                |               | HTML content to put as-is in the left sidebar.                                                                                                                 |
 | [`LINKS_WIDGET_NAME`](http://docs.getpelican.com/en/stable/settings.html#LINKS_WIDGET_NAME)   | `"Links"`     | Allows override of the name of the links widget.                                                                                                               |
 | [`LINKS`](http://docs.getpelican.com/en/stable/settings.html#LINKS)                           |               | A list of tuples (Title, URL) for links to appear in the second column of the footer.                                                                          |
-| [`MANUAL_LINKS`](http://docs.getpelican.com/en/stable/settings.html#MANUAL_LINKS)             |               | When enabling this, you must pass the links (in LINKS & SOCIAL settins) not as tuples anymore, but as list, where every entry is formatted as you like         |
+| [`MANUAL_LINKS`](http://docs.getpelican.com/en/stable/settings.html#MANUAL_LINKS)             |               | When enabling this, you must pass the links (in LINKS & SOCIAL settings) not as tuples anymore, but as list, where every entry is formatted as you like        |
 | [`MENUITEMS`](http://docs.getpelican.com/en/stable/settings.html#MENUITEMS)                   |               | A list of tuples (Title, URL) for additional menu items to appear at the beginning of the main menu.                                                           |
 | `RIGHT_SIDEBAR`                                                                               |               | HTML content to put as-is in the right sidebar.                                                                                                                |
 | [`SITESUBTITLE`](http://docs.getpelican.com/en/stable/settings.html#SITESUBTITLE)             |               | A subtitle to appear in the header.                                                                                                                            |
 | `SITE_THUMBNAIL_TEXT`                                                                         |               | Text displayed behind site's thumbnail.                                                                                                                        |
 | `SITE_THUMBNAIL`                                                                              |               | Site's thumbnail URL as displayed in the header. Should be a square image of at least 80x80 pixels.                                                            |
 | [`SOCIAL_WIDGET_NAME`](http://docs.getpelican.com/en/stable/settings.html#SOCIAL_WIDGET_NAME) | `"Social"`    | Allows override of the name of the “social” widget.                                                                                                            |
 | [`SOCIAL`](http://docs.getpelican.com/en/stable/settings.html#SOCIAL)                         |               | A list of tuples (Title, URL) to appear in the first columns of the footer.                                                                                    |
@@ -355,14 +349,24 @@
 ```
 ````
 
 Into this:
 
 ![Plumage PyMdown Extensions' Highlight rendering](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/highlight-rendering.jpeg)
 
+## CSS customization
+
+TODO: document all kind customization below
+
+### Python code transforms at generation via `pyquery`
+
+### Use of `extra_css`
+
+### Custom `main.scss`
+
 ## FAQ
 
 ### How can I disable the zoom on images?
 
 All images of an article are zoomable by default. You can deactivate the
 magnifying glass per-image by adding a `noZoom` CSS class. So instead of the
 following Markdown code:
@@ -390,15 +394,15 @@
 (GPLv2+)](https://github.com/kdeldycke/plumage/blob/main/LICENSE).
 
 Copyright (C) 2012-2020 [Kevin Deldycke](https://kevin.deldycke.com) and
 [contributors](https://github.com/kdeldycke/plumage/graphs/contributors).
 
 ## Third-party assets
 
-The theme embed copies of some external softwares, scripts, libraries and
+The theme embed copies of some external software, scripts, libraries and
 artworks:
 
 ```text
 jQuery MGlass v1.1
 Copyright (c) 2012 Younès El Biache
 Distributed under a MIT license
 Source: https://github.com/younes0/jQuery-MGlass
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
-Metadata-Version: 2.1 Name: plumage Version: 3.1.0 Summary: Clean and tidy
+Metadata-Version: 2.1 Name: plumage Version: 4.0.0 Summary: Clean and tidy
 theme for Pelican. Home-page: https://github.com/kdeldycke/plumage License:
 GPL-2.0-or-later Keywords: pelican,pelican-theme,stork,static-
-search,masonry,theme,bootstrap,jquery,font-awesome Author: Kevin Deldycke
-Author-email: kevin@deldycke.com Requires-Python: >=3.8,<4.0 Classifier:
-Development Status :: 5 - Production/Stable Classifier: Environment :: Plugins
-Classifier: Environment :: Web Environment Classifier: Framework :: Pelican ::
-Themes Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Information Technology Classifier: License :: OSI Approved :: GNU
-General Public License v2 or later (GPLv2+) Classifier: Operating System :: OS
+search,masonry,myst,theme,bootstrap,jquery Author: Kevin Deldycke Author-email:
+kevin@deldycke.com Requires-Python: >=3.9,<4.0 Classifier: Development Status
+:: 5 - Production/Stable Classifier: Environment :: Plugins Classifier:
+Environment :: Web Environment Classifier: Framework :: Pelican :: Themes
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Information Technology Classifier: License :: OSI Approved :: GNU General
+Public License v2 or later (GPLv2+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: JavaScript Classifier:
 Programming Language :: Other Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Internet :: WWW/HTTP Classifier: Topic :: Text Processing :: Markup :: HTML
-Classifier: Typing :: Typed Requires-Dist: Markdown (>=3.4.1,<4.0.0) Requires-
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
+Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/
+Search Classifier: Topic :: Text Processing :: Markup :: HTML Classifier: Topic
+:: Text Processing :: Markup :: Markdown Classifier: Typing :: Typed Requires-
 Dist: closure (>=20191111,<20191112) Requires-Dist: cssmin (>=0.2.0,<0.3.0)
-Requires-Dist: libsass (>=0.22.0,<0.23.0) Requires-Dist: pelican
-(>=4.8.0,<5.0.0) Requires-Dist: pelican-webassets (>=2.0.0,<3.0.0) Requires-
-Dist: pygments (>=2.14.0,<3.0.0) Requires-Dist: pymdown-extensions
-(>=10.0.1,<11.0.0) Requires-Dist: pynpm (>=0.1.2,<0.2.0) Requires-Dist: pyquery
-(>=2.0.0,<3.0.0) Project-URL: Changelog, https://github.com/kdeldycke/plumage/
-blob/main/changelog.md#changelog Project-URL: Documentation, https://
-github.com/kdeldycke/plumage#settings Project-URL: Funding, https://github.com/
-sponsors/kdeldycke Project-URL: Issues, https://github.com/kdeldycke/plumage/
-issues Project-URL: Repository, https://github.com/kdeldycke/plumage
-Description-Content-Type: text/markdown
+Requires-Dist: libsass (>=0.23.0,<0.24.0) Requires-Dist: pelican
+(>=4.8.0,<5.0.0) Requires-Dist: pelican-myst-reader (>=1.3.0b1,<2.0.0)
+Requires-Dist: pelican-webassets (>=2.0.0,<3.0.0) Requires-Dist: pynpm
+(>=0.2.0,<0.3.0) Requires-Dist: pyquery (>=2.0.0,<3.0.0) Project-URL:
+Changelog, https://github.com/kdeldycke/plumage/blob/main/
+changelog.md#changelog Project-URL: Documentation, https://github.com/
+kdeldycke/plumage#settings Project-URL: Funding, https://github.com/sponsors/
+kdeldycke Project-URL: Issues, https://github.com/kdeldycke/plumage/issues
+Project-URL: Repository, https://github.com/kdeldycke/plumage Description-
+Content-Type: text/markdown
                           _[_P_l_u_m_a_g_e_,_ _a_ _P_e_l_i_c_a_n_ _t_h_e_m_e_]
 Plumage is a clean and tidy theme for [Pelican](https://getpelican.com), a
 static site generator. I initially created this theme for [my blog](https://
 kevin.deldycke.com), but it is now generic enough to be used by anyone. ##
 Features - Standard Pelican views: | ![Plumage article view](https://
 raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/article.jpeg) | !
 [Plumage categories view](https://raw.githubusercontent.com/kdeldycke/plumage/
@@ -40,15 +41,15 @@
 ----------------------------------------------------------------------------: |
 :------------------------------------------------------------------------------
 --------------------------------------: | | Article | Categories | Tiered tag
 list | | ![Plumage archive view](https://raw.githubusercontent.com/kdeldycke/
 plumage/main/screenshots/archives.jpeg) | ![Plumage tag view](https://
 raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/tag.jpeg) | !
 [Plumage authors view](https://raw.githubusercontent.com/kdeldycke/plumage/
-main/screenshots/authors.jpeg) | | Collapsable yearly archives | Tagged
+main/screenshots/authors.jpeg) | | Collapsible yearly archives | Tagged
 articles | Authors | | ![Plumage archive view](https://
 raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/browse-content-
 by.jpeg) | | | | Faceted article browsing | | | - Projects template: | !
 [Plumage projects: code showcase](https://raw.githubusercontent.com/kdeldycke/
 plumage/main/screenshots/projects-code.jpeg) | ![Plumage projects: videos
 showcase](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/
 projects-videos.jpeg) | ![Plumage projects: themes showcase](https://
@@ -61,15 +62,15 @@
 ------------------------------------------------------------------------------
 -: | | Code showcase ([source](https://github.com/kdeldycke/kevin-deldycke-
 blog/blob/ebe0d17a59730457c3016dff77fdfa799a80d756/content/templates/
 code.html)) | Videos showcase ([source](https://github.com/kdeldycke/kevin-
 deldycke-blog/blob/f778998376fa5c68f1a02129884b89592b641777/content/templates/
 videos.html)) | Themes showcase ([source](https://github.com/kdeldycke/kevin-
 deldycke-blog/blob/f778998376fa5c68f1a02129884b89592b641777/content/templates/
-themes.html)) | - Based on [Bootstrap v4](https://getbootstrap.com). - [Code
+themes.html)) | - Based on [Bootstrap v5](https://getbootstrap.com). - [Code
 syntax highlighting](#code-syntax-highlighting) with [30+ styles](https://
 github.com/pygments/pygments/tree/master/pygments/styles). - Site-wide static
 search via [Stork](https://stork-search.net). - Bare YouTube links in articles
 gets rendered as embedded videos: ![Plumage YouTube link](https://
 raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/youtube-link.jpeg)
 - Direct link to edit articles on GitHub: ![Plumage GitHub edit link](https://
 raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/github-edit-
@@ -78,37 +79,34 @@
 screenshots/magnifying-glass.jpeg) ![Plumage image zoom](https://
 raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/zoom.jpeg) -
 External assets (Bootstrap, Jquery, etc...) uses [CDNjs ](https://cdnjs.com/
 about). - Disqus integration: ![Plumage disqus comments](https://
 raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/disqus.jpeg) ##
 Plugins Plumage has built-in support for the following plugins and extensions:
 | Plugin name | Type | Status | Notes | | :------------------------------------
---------------------------------------------------------------------------- | :
------------------ | :------- | :-----------------------------------------------
-------------------------------------------------------------- | | [`pelican-
-image-process`](https://github.com/pelican-plugins/image-process) | Pelican
-plugin | Optional | Embed a hack to [fix parsing of external images](https://
-github.com/pelican-plugins/image-process/issues/33). | | [`pelican-neighbors`]
-(https://github.com/pelican-plugins/neighbors) | Pelican plugin | Optional | |
-| [`pelican-related-posts`](https://github.com/pelican-plugins/related-posts) |
-Pelican plugin | Optional | | | [`pelican-similar-posts`](https://github.com/
-pelican-plugins/similar-posts) | Pelican plugin | Optional | | | [`pelican-
-search`](https://github.com/pelican-plugins/search) | Pelican plugin | Optional
-| | | [`pelican-webassets`](https://github.com/pelican-plugins/webassets) |
-Pelican plugin | Required | | | [`markdown.extensions.admonition`](https://
-python-markdown.github.io/extensions/admonition/) | Markdown extension |
-Optional | Re-style admonitions into [alerts](https://getbootstrap.com/docs/
-4.5/components/alerts/). | | [`markdown.extensions.codehilite`](https://python-
+---------------------------------------------------------- | :----------------
+- | :------- | :---------------------------------------------------------------
+--------------------------------------------- | | [`pelican-image-process`]
+(https://github.com/pelican-plugins/image-process) | Pelican plugin | Optional
+| Embed a hack to [fix parsing of external images](https://github.com/pelican-
+plugins/image-process/issues/33). | | [`pelican-neighbors`](https://github.com/
+pelican-plugins/neighbors) | Pelican plugin | Optional | | | [`pelican-related-
+posts`](https://github.com/pelican-plugins/related-posts) | Pelican plugin |
+Optional | | | [`pelican-similar-posts`](https://github.com/pelican-plugins/
+similar-posts) | Pelican plugin | Optional | | | [`pelican-search`](https://
+github.com/pelican-plugins/search) | Pelican plugin | Optional | | | [`pelican-
+webassets`](https://github.com/pelican-plugins/webassets) | Pelican plugin |
+Required | | | [`markdown.extensions.admonition`](https://python-
+markdown.github.io/extensions/admonition/) | Markdown extension | Optional |
+Re-style admonitions into [alerts](https://getbootstrap.com/docs/4.5/
+components/alerts/). | | [`markdown.extensions.codehilite`](https://python-
 markdown.github.io/extensions/code_hilite/) | Markdown extension | Optional |
 Style highlighted code with Pygment style. | | [`markdown.extensions.toc`]
 (https://python-markdown.github.io/extensions/toc/#usage) | Markdown extension
 | Optional | Adds permalink anchors to article's subtitles. | |
-[`pymdownx.emoji`](https://facelessuser.github.io/pymdown-extensions/
-extensions/emoji/#default-emoji-generators) | Markdown extension | Optional |
-Style `emojione` set for proper integration into text. | |
 [`pymdownx.highlight`](https://facelessuser.github.io/pymdown-extensions/
 extensions/highlight/) | Markdown extension | Optional | Style highlighted code
 with Pygment style. | | [`typogrify`](https://pypi.python.org/pypi/typogrify) |
 Pelican builtin | Optional | Style ampersands. | ## Installation Install this
 theme using the `main` branch of this Github repo. If you're already using
 `poetry` to manage dependency of Pelican project, you need to run just
 ```shell-session poetry add git+https://github.com/kdeldycke/plumage#main ```
@@ -116,50 +114,49 @@
 section of the `pyproject.toml` file. ``` plumage = {git = "https://github.com/
 kdeldycke/plumage", rev = "main"} ``` Once added, run `poetry update` to
 reflect this new dependency. **Note:** If you haven't used `poetry` in the
 project yet, you need to do so before adding `plumage`. You can do that by
 first [installing `poetry`](https://python-poetry.org/docs/#installation) on
 your system and then running `poetry init` inside the project folder. Then,
 once you're done installing the `plumage` module, update your `pelicanconf.py`
-file to reference the module and requied extra plugins: ```python import
-plumage THEME = plumage.get_path() PLUGINS = [ (â¦)
-"pelican.plugins.webassets", ] ``` On first run, Plumage will try to install
-[Node.js package dependencies](https://github.com/kdeldycke/plumage/blob/main/
-plumage/package.json) via the `npm` CLI: ```shell-session $ poetry run pelican
---verbose ./content (â¦) WARNING: postcss CLI not found. -> Install Plumage's
-Node.js dependencies from (â¦)/plumage/package.json: | { | "name": "plumage-
-webassets-pipeline", | "description": "Plumage depdencies for the webassets
-compilation pipeline.", | "dependencies": { | "postcss-cli": "^8.3.1" | } | } |
-up to date, audited 96 packages in 984ms found 0 vulnerabilities -> postcss CLI
-found at (â¦)/plumage/node_modules/.bin/postcss (â¦) ``` ## Settings Plumage
-can be customized by adding these optionnal parameters to your `pelicanconf.py`
-file: | Setting name | Default value | Description | | :-----------------------
---------------------------------------------------------------------- | :------
------- | :---------------------------------------------------------------------
--------------------------------------------------------------------------------
---------- | | `ARTICLE_EDIT_LINK` | | Generate an edit link besides each
-article. Can use `%(slug)s` to include dynamic article's slug in the link. | |
-`CODE_STYLE` | `"monokai"` | Pygments' style ID. Choose one from `poetry run
-pygmentize -L styles`. | | `COPYRIGHT` | | Additional copyright statement to
-add in the third column of the footer. | | `DISCLAIMER` | | Overide the
-disclaimer notice that gets displayed at the fourth column of the footer. | |
-[`DISQUS_SITENAME`](http://docs.getpelican.com/en/stable/
-settings.html#DISQUS_SITENAME) | | Pelican can handle Disqus comments. Specify
-the Disqus sitename identifier here. | | `FAVICON_LINKS` | `True` | Fetch
-link's icons from [Google's favicons webservice](https://www.google.com/s2/
-favicons). | | [`GOOGLE_ANALYTICS`](http://docs.getpelican.com/en/stable/
-settings.html#GOOGLE_ANALYTICS) | | Set to `UA-XXXXXX-Y` Property's tracking ID
-to activate Google Analytics. | | `LEFT_SIDEBAR` | | HTML content to put as-is
-in the left sidebar. | | [`LINKS_WIDGET_NAME`](http://docs.getpelican.com/en/
-stable/settings.html#LINKS_WIDGET_NAME) | `"Links"` | Allows override of the
-name of the links widget. | | [`LINKS`](http://docs.getpelican.com/en/stable/
+file to reference the module: ```python import plumage THEME = plumage.get_path
+() ``` On first run, Plumage will try to install [Node.js package dependencies]
+(https://github.com/kdeldycke/plumage/blob/main/plumage/package.json) via the
+`npm` CLI: ```shell-session $ poetry run pelican --verbose ./content (â¦)
+WARNING: postcss CLI not found. -> Install Plumage's Node.js dependencies from
+(â¦)/plumage/package.json: | { | "name": "plumage-webassets-pipeline", |
+"description": "Plumage dependencies for the webassets compilation pipeline.",
+| "dependencies": { | "postcss-cli": "^8.3.1" | } | } | up to date, audited 96
+packages in 984ms found 0 vulnerabilities -> postcss CLI found at (â¦)/
+plumage/node_modules/.bin/postcss (â¦) ``` ## Settings Plumage can be
+customized by adding these optional parameters to your `pelicanconf.py` file: |
+Setting name | Default value | Description | | :-------------------------------
+------------------------------------------------------------- | :------------ |
+:------------------------------------------------------------------------------
+------------------------------------------------------------------------------
+- | | `ARTICLE_EDIT_LINK` | | Generate an edit link besides each article. Can
+use `%(slug)s` to include dynamic article's slug in the link. | | `CODE_STYLE`
+| `"monokai"` | Pygments' style ID. Choose one from `poetry run pygmentize -
+L styles`. | | `COPYRIGHT` | | Additional copyright statement to add in the
+third column of the footer. | | `DISCLAIMER` | | Override the disclaimer notice
+that gets displayed at the fourth column of the footer. | | [`DISQUS_SITENAME`]
+(http://docs.getpelican.com/en/stable/settings.html#DISQUS_SITENAME) | |
+Pelican can handle Disqus comments. Specify the Disqus sitename identifier
+here. | | `FAVICON_LINKS` | `True` | Fetch link's icons from [Google's favicons
+webservice](https://www.google.com/s2/favicons). | | [`GOOGLE_ANALYTICS`](http:
+//docs.getpelican.com/en/stable/settings.html#GOOGLE_ANALYTICS) | | Set to `UA-
+XXXXXX-Y` Property's tracking ID to activate Google Analytics. | |
+`LEFT_SIDEBAR` | | HTML content to put as-is in the left sidebar. | |
+[`LINKS_WIDGET_NAME`](http://docs.getpelican.com/en/stable/
+settings.html#LINKS_WIDGET_NAME) | `"Links"` | Allows override of the name of
+the links widget. | | [`LINKS`](http://docs.getpelican.com/en/stable/
 settings.html#LINKS) | | A list of tuples (Title, URL) for links to appear in
 the second column of the footer. | | [`MANUAL_LINKS`](http://
 docs.getpelican.com/en/stable/settings.html#MANUAL_LINKS) | | When enabling
-this, you must pass the links (in LINKS & SOCIAL settins) not as tuples
+this, you must pass the links (in LINKS & SOCIAL settings) not as tuples
 anymore, but as list, where every entry is formatted as you like | |
 [`MENUITEMS`](http://docs.getpelican.com/en/stable/settings.html#MENUITEMS) | |
 A list of tuples (Title, URL) for additional menu items to appear at the
 beginning of the main menu. | | `RIGHT_SIDEBAR` | | HTML content to put as-is
 in the right sidebar. | | [`SITESUBTITLE`](http://docs.getpelican.com/en/
 stable/settings.html#SITESUBTITLE) | | A subtitle to appear in the header. | |
 `SITE_THUMBNAIL_TEXT` | | Text displayed behind site's thumbnail. | |
@@ -220,32 +217,34 @@
 linenums="5 1 3" filename="~/code/foo.log"} $ cat ./example.markdown This is
 the content of the file: â java â rust â haskell â javascript $ cat ./
 addendum.txt This is extra content. $ find ./ -iname "*.markdown" -print -exec
 bash -c 'cat ./addendum.txt >> "{}"' \; ./example.markdown $ cat ./
 example.markdown This is the content of the file: â java â rust â haskell
 â javascript This is extra content. ``` ```` Into this: ![Plumage PyMdown
 Extensions' Highlight rendering](https://raw.githubusercontent.com/kdeldycke/
-plumage/main/screenshots/highlight-rendering.jpeg) ## FAQ ### How can I disable
-the zoom on images? All images of an article are zoomable by default. You can
-deactivate the magnifying glass per-image by adding a `noZoom` CSS class. So
-instead of the following Markdown code: ```markdown ![Image title](/folder/
-image.png) ``` You have to use the following template to deactivate the zoom of
-an image: ```markdown ![Image title](/folder/image.png){: .noZoom} ``` ### Why
-is the search not working? The [official Pelican's `search` plugin](https://
-github.com/pelican-plugins/search) needs to be installed. TODO: Activate search
-field automaticcaly if the plugin is present. ## License This software is
-licensed under the [GNU General Public License v2 or later (GPLv2+)](https://
-github.com/kdeldycke/plumage/blob/main/LICENSE). Copyright (C) 2012-2020 [Kevin
-Deldycke](https://kevin.deldycke.com) and [contributors](https://github.com/
-kdeldycke/plumage/graphs/contributors). ## Third-party assets The theme embed
-copies of some external softwares, scripts, libraries and artworks: ```text
-jQuery MGlass v1.1 Copyright (c) 2012 YounÃ¨s El Biache Distributed under a MIT
-license Source: https://github.com/younes0/jQuery-MGlass ``` ```text Fabric
-(Plaid) Copyright (c) 2012 James Basoo Distributed under a Creative Commons
-Attribution-ShareAlike 3.0 Unported license Source: https://subtlepatterns.com/
-fabric-plaid/ ``` ```text Cream paper Copyright (c) 2012 Devin Holmes
-Distributed under a Creative Commons Attribution-ShareAlike 3.0 Unported
-license Source: https://subtlepatterns.com/cream-paper/ ``` ```text Feather-alt
-icon v5.1.0 Copyright (c) 2020 Font Awesome project Distributed under a
-Creative Commons Attribution 4.0 International license Source: https://
-fontawesome.com/icons/feather-alt?style=solid ``` ```text Macro shot of White
-Feather Source: https://unsplash.com/photos/Sw7f58YJbc0 ```
+plumage/main/screenshots/highlight-rendering.jpeg) ## CSS customization TODO:
+document all kind customization below ### Python code transforms at generation
+via `pyquery` ### Use of `extra_css` ### Custom `main.scss` ## FAQ ### How can
+I disable the zoom on images? All images of an article are zoomable by default.
+You can deactivate the magnifying glass per-image by adding a `noZoom` CSS
+class. So instead of the following Markdown code: ```markdown ![Image title](/
+folder/image.png) ``` You have to use the following template to deactivate the
+zoom of an image: ```markdown ![Image title](/folder/image.png){: .noZoom} ```
+### Why is the search not working? The [official Pelican's `search` plugin]
+(https://github.com/pelican-plugins/search) needs to be installed. TODO:
+Activate search field automaticcaly if the plugin is present. ## License This
+software is licensed under the [GNU General Public License v2 or later
+(GPLv2+)](https://github.com/kdeldycke/plumage/blob/main/LICENSE). Copyright
+(C) 2012-2020 [Kevin Deldycke](https://kevin.deldycke.com) and [contributors]
+(https://github.com/kdeldycke/plumage/graphs/contributors). ## Third-party
+assets The theme embed copies of some external software, scripts, libraries and
+artworks: ```text jQuery MGlass v1.1 Copyright (c) 2012 YounÃ¨s El Biache
+Distributed under a MIT license Source: https://github.com/younes0/jQuery-
+MGlass ``` ```text Fabric (Plaid) Copyright (c) 2012 James Basoo Distributed
+under a Creative Commons Attribution-ShareAlike 3.0 Unported license Source:
+https://subtlepatterns.com/fabric-plaid/ ``` ```text Cream paper Copyright (c)
+2012 Devin Holmes Distributed under a Creative Commons Attribution-ShareAlike
+3.0 Unported license Source: https://subtlepatterns.com/cream-paper/ ```
+```text Feather-alt icon v5.1.0 Copyright (c) 2020 Font Awesome project
+Distributed under a Creative Commons Attribution 4.0 International license
+Source: https://fontawesome.com/icons/feather-alt?style=solid ``` ```text Macro
+shot of White Feather Source: https://unsplash.com/photos/Sw7f58YJbc0 ```
```

