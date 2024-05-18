# Comparing `tmp/normcap-0.5.6.tar.gz` & `tmp/normcap-0.5.7.tar.gz`

## Comparing `normcap-0.5.6.tar` & `normcap-0.5.7.tar`

### file list

```diff
@@ -1,225 +1,225 @@
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 normcap-0.5.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0    20040 2020-02-02 00:00:00.000000 normcap-0.5.6/CHANGELOG
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 normcap-0.5.6/mkdocs.yml
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 normcap-0.5.6/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 normcap-0.5.6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 normcap-0.5.6/.github/ISSUE_TEMPLATE/detection_quality.yml
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 normcap-0.5.6/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0    10582 2020-02-02 00:00:00.000000 normcap-0.5.6/.github/workflows/cicd.yaml
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 normcap-0.5.6/adr/001-choose-transparent-windows-as-main-gui.md
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 normcap-0.5.6/adr/002-choose-windows-with-screenshots-as-main-gui.md
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 normcap-0.5.6/adr/003-use-system-tray-as-main-application.md
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 normcap-0.5.6/adr/004-do-not-implement-hotkey.md
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 normcap-0.5.6/adr/005-use-hatch-instead-poetry.md
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 normcap-0.5.6/adr/006-use-jeepney-for-dbus-calls.md
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 normcap-0.5.6/adr/README.md
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/build.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/deps.py
--rwxr-xr-x   0        0        0     4854 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/l10n.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/metainfo
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap-128.png
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap-16.png
--rw-r--r--   0        0        0    26067 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap-256.png
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap-32.png
--rw-r--r--   0        0        0    45156 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap-512.png
--rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap-64.png
--rw-r--r--   0        0        0   160026 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap.icns
--rw-r--r--   0        0        0   206511 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap.ico
--rw-r--r--   0        0        0    24936 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap.svg
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap_install.bmp
--rw-r--r--   0        0        0    29592 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap_install.icns
--rw-r--r--   0        0        0     9186 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap_install.png
--rw-r--r--   0        0        0    29784 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap_install.svg
--rw-r--r--   0        0        0   615402 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap_install_bg.bmp
--rw-r--r--   0        0        0    12552 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap_install_bg.png
--rw-r--r--   0        0        0    24064 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap_install_bg.svg
--rw-r--r--   0        0        0   114514 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap_install_top.bmp
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/platforms/__init__.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/platforms/linux_briefcase.py
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/platforms/macos_briefcase.py
--rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/platforms/utils.py
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/platforms/windows_briefcase.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 normcap-0.5.6/docs/contribute.md
--rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 normcap-0.5.6/docs/faqs.md
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 normcap-0.5.6/docs/index.md
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 normcap-0.5.6/docs/support.md
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 normcap-0.5.6/docs/usage.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/__init__.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/__main__.py
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/app.py
--rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/utils.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/__init__.py
--rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/main.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/structures.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/system_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/handlers/__init__.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/handlers/pbcopy.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/handlers/qtclipboard.py
--rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/handlers/windll.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/handlers/wlclipboard.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/handlers/xclip.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/handlers/xsel.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/__init__.py
--rw-r--r--   0        0        0     7955 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/constants.py
--rw-r--r--   0        0        0     7094 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/dbus.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/downloader.py
--rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/introduction.py
--rw-r--r--   0        0        0     9362 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/language_manager.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/loading_indicator.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/localization.py
--rw-r--r--   0        0        0    14197 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/menu_button.py
--rw-r--r--   0        0        0     4362 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/models.py
--rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/notification.py
--rw-r--r--   0        0        0   312761 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/resources.py
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/settings.py
--rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/system_info.py
--rw-r--r--   0        0        0    24259 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/tray.py
--rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/update_check.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/utils.py
--rw-r--r--   0        0        0    13254 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/window.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/__init__.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/enhance.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/recognize.py
--rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/structures.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/tesseract.py
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/transformer.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/transformers/__init__.py
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/transformers/email.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/transformers/multi_line.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/transformers/paragraph.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/transformers/single_line.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/transformers/url.py
--rw-r--r--   0        0        0     9831 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/transformers/url_tlds.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/__init__.py
--rw-r--r--   0        0        0    13773 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/icons/normcap.png
--rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/icons/notification.png
--rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/icons/parse.png
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/icons/raw.png
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/icons/resources.qrc
--rw-r--r--   0        0        0    17968 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/icons/settings.png
--rw-r--r--   0        0        0    15317 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/icons/tray.png
--rw-r--r--   0        0        0    16742 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/icons/tray_done.png
--rw-r--r--   0        0        0    16316 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/icons/tray_processing.png
--rw-r--r--   0        0        0   145973 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/darwin-intro-1.png
--rw-r--r--   0        0        0   148696 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/darwin-intro-2.png
--rw-r--r--   0        0        0    98495 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/darwin-intro-3.png
--rw-r--r--   0        0        0   139526 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/darwin-intro-4.png
--rw-r--r--   0        0        0   455444 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/linux-intro-1.png
--rw-r--r--   0        0        0   466217 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/linux-intro-2.png
--rw-r--r--   0        0        0   299322 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/linux-intro-3.png
--rw-r--r--   0        0        0   399984 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/linux-intro-4.png
--rw-r--r--   0        0        0   415812 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/win32-intro-1.png
--rw-r--r--   0        0        0   425024 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/win32-intro-2.png
--rw-r--r--   0        0        0   267555 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/win32-intro-3.png
--rw-r--r--   0        0        0   408697 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/win32-intro-4.png
--rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/README.md
--rw-r--r--   0        0        0    12682 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/messages.pot
--rw-r--r--   0        0        0     7813 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     7929 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/es_ES/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/hi_IN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     7924 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/it_IT/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/pl_PL/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     7846 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/pt_PT/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0    10324 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/ru_RU/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/sv_SE/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/uk_UA/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/tessdata/.keep
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/tessdata/LICENSE.txt
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/tessdata/README.txt
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/__init__.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/main.py
--rw-r--r--   0        0        0     8741 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/permissions.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/post_processing.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/structures.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/system_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/handlers/__init__.py
--rw-r--r--   0        0        0     8293 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/handlers/dbus_portal.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/handlers/dbus_shell.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/handlers/grim.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/handlers/qt.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/__init__.py
--rw-r--r--   0        0        0     8124 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/conftest.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/test_app.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/test_main.py
--rw-r--r--   0        0        0    13257 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/__init__.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/test_normcap.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/test_settings_menu.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/test_tray_menu.py
--rw-r--r--   0        0        0    37267 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/00_parse_urls.png
--rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/01_parse_colored_url.png
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/02_detect_window_title.png
--rw-r--r--   0        0        0    35832 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/03_parse_emails.png
--rw-r--r--   0        0        0    61232 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/04_parse_email_skip_invalid.png
--rw-r--r--   0        0        0     8012 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/05_detect_text_with_low_contrast.png
--rw-r--r--   0        0        0    33416 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/06_detect_special_characters.png
--rw-r--r--   0        0        0   152224 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/07_parse_paragraphs_of_text.png
--rw-r--r--   0        0        0   168233 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/08_paragraphs.png
--rw-r--r--   0        0        0   277892 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/09_two_columns.png
--rw-r--r--   0        0        0    95751 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/10_font_sizes.png
--rw-r--r--   0        0        0    23053 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/11_paragraph_with_bullet_points.png
--rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/12_not_a_url.png
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/__init__.py
--rw-r--r--   0        0        0     9832 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_clipboard/__init__.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_clipboard/test_main.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_clipboard/test_system_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_clipboard/test_handlers/__init__.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_clipboard/test_handlers/test_pbcopy.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_clipboard/test_handlers/test_qtclipboard.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_clipboard/test_handlers/test_windll.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_clipboard/test_handlers/test_wlclipboard.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_clipboard/test_handlers/test_xclip.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/__init__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_constants.py
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_downloader.py
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_introduction.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_language_manager.py
--rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_loading_indicator.py
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_menu_button.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_models.py
--rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_notification.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_resources.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_settings.py
--rw-r--r--   0        0        0     8895 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_system_info.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_tray.py
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_update_check.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_utils.py
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_window.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/__init__.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/test_enhance.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/test_recognize.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/test_structures.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/test_tesseract.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/test_transformer.py
--rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/testcases/00_eng.png
--rw-r--r--   0        0        0    26208 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/testcases/01_chi_sim.png
--rw-r--r--   0        0        0    20815 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/testcases/02_jpn.png
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/testcases/__init__.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/testcases/data.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/testimages/color.png
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/testimages/dark.png
--rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/testimages/light.png
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/transformers/test_email.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/transformers/test_paragraph.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/transformers/test_single_line.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/transformers/test_url.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_screengrab/split_full_desktop_to_screens.png
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_screengrab/test_main.py
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_screengrab/test_permissions.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_screengrab/test_post_processing.py
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_screengrab/test_system_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_screengrab/test_handlers/__init__.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_screengrab/test_handlers/test_dbus_portal.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_screengrab/test_handlers/test_grim.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_screengrab/test_handlers/test_qt.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 normcap-0.5.6/.gitignore
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 normcap-0.5.6/LICENSE
--rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 normcap-0.5.6/README.md
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 normcap-0.5.6/hatch_build.py
--rw-r--r--   0        0        0    10155 2020-02-02 00:00:00.000000 normcap-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     9269 2020-02-02 00:00:00.000000 normcap-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 normcap-0.5.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    20527 2020-02-02 00:00:00.000000 normcap-0.5.7/CHANGELOG
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 normcap-0.5.7/mkdocs.yml
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 normcap-0.5.7/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 normcap-0.5.7/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 normcap-0.5.7/.github/ISSUE_TEMPLATE/detection_quality.yml
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 normcap-0.5.7/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0    10582 2020-02-02 00:00:00.000000 normcap-0.5.7/.github/workflows/cicd.yaml
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 normcap-0.5.7/adr/001-choose-transparent-windows-as-main-gui.md
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 normcap-0.5.7/adr/002-choose-windows-with-screenshots-as-main-gui.md
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 normcap-0.5.7/adr/003-use-system-tray-as-main-application.md
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 normcap-0.5.7/adr/004-do-not-implement-hotkey.md
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 normcap-0.5.7/adr/005-use-hatch-instead-poetry.md
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 normcap-0.5.7/adr/006-use-jeepney-for-dbus-calls.md
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 normcap-0.5.7/adr/README.md
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/build.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/deps.py
+-rwxr-xr-x   0        0        0     4854 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/l10n.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/metainfo
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/imgs/normcap-128.png
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/imgs/normcap-16.png
+-rw-r--r--   0        0        0    26067 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/imgs/normcap-256.png
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/imgs/normcap-32.png
+-rw-r--r--   0        0        0    45156 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/imgs/normcap-512.png
+-rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/imgs/normcap-64.png
+-rw-r--r--   0        0        0   160026 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/imgs/normcap.icns
+-rw-r--r--   0        0        0   206511 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/imgs/normcap.ico
+-rw-r--r--   0        0        0    24936 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/imgs/normcap.svg
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/imgs/normcap_install.bmp
+-rw-r--r--   0        0        0    29592 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/imgs/normcap_install.icns
+-rw-r--r--   0        0        0     9186 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/imgs/normcap_install.png
+-rw-r--r--   0        0        0    29784 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/imgs/normcap_install.svg
+-rw-r--r--   0        0        0   615402 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/imgs/normcap_install_bg.bmp
+-rw-r--r--   0        0        0    12552 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/imgs/normcap_install_bg.png
+-rw-r--r--   0        0        0    24064 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/imgs/normcap_install_bg.svg
+-rw-r--r--   0        0        0   114514 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/imgs/normcap_install_top.bmp
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/platforms/__init__.py
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/platforms/linux_briefcase.py
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/platforms/macos_briefcase.py
+-rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/platforms/utils.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 normcap-0.5.7/bundle/platforms/windows_briefcase.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 normcap-0.5.7/docs/contribute.md
+-rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 normcap-0.5.7/docs/faqs.md
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 normcap-0.5.7/docs/index.md
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 normcap-0.5.7/docs/support.md
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 normcap-0.5.7/docs/usage.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/__init__.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/__main__.py
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/app.py
+-rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/utils.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/clipboard/__init__.py
+-rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/clipboard/main.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/clipboard/structures.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/clipboard/system_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/clipboard/handlers/__init__.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/clipboard/handlers/pbcopy.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/clipboard/handlers/qtclipboard.py
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/clipboard/handlers/windll.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/clipboard/handlers/wlclipboard.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/clipboard/handlers/xclip.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/clipboard/handlers/xsel.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/gui/__init__.py
+-rw-r--r--   0        0        0     7955 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/gui/constants.py
+-rw-r--r--   0        0        0     7094 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/gui/dbus.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/gui/downloader.py
+-rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/gui/introduction.py
+-rw-r--r--   0        0        0     9362 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/gui/language_manager.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/gui/loading_indicator.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/gui/localization.py
+-rw-r--r--   0        0        0    14197 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/gui/menu_button.py
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/gui/models.py
+-rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/gui/notification.py
+-rw-r--r--   0        0        0   312761 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/gui/resources.py
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/gui/settings.py
+-rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/gui/system_info.py
+-rw-r--r--   0        0        0    24259 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/gui/tray.py
+-rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/gui/update_check.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/gui/utils.py
+-rw-r--r--   0        0        0    14161 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/gui/window.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/ocr/__init__.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/ocr/enhance.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/ocr/recognize.py
+-rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/ocr/structures.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/ocr/tesseract.py
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/ocr/transformer.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/ocr/transformers/__init__.py
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/ocr/transformers/email.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/ocr/transformers/multi_line.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/ocr/transformers/paragraph.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/ocr/transformers/single_line.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/ocr/transformers/url.py
+-rw-r--r--   0        0        0     9831 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/ocr/transformers/url_tlds.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/__init__.py
+-rw-r--r--   0        0        0    13773 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/icons/normcap.png
+-rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/icons/notification.png
+-rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/icons/parse.png
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/icons/raw.png
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/icons/resources.qrc
+-rw-r--r--   0        0        0    17968 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/icons/settings.png
+-rw-r--r--   0        0        0    15317 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/icons/tray.png
+-rw-r--r--   0        0        0    16742 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/icons/tray_done.png
+-rw-r--r--   0        0        0    16316 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/icons/tray_processing.png
+-rw-r--r--   0        0        0   145973 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/images/darwin-intro-1.png
+-rw-r--r--   0        0        0   148696 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/images/darwin-intro-2.png
+-rw-r--r--   0        0        0    98495 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/images/darwin-intro-3.png
+-rw-r--r--   0        0        0   139526 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/images/darwin-intro-4.png
+-rw-r--r--   0        0        0   455444 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/images/linux-intro-1.png
+-rw-r--r--   0        0        0   466217 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/images/linux-intro-2.png
+-rw-r--r--   0        0        0   299322 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/images/linux-intro-3.png
+-rw-r--r--   0        0        0   399984 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/images/linux-intro-4.png
+-rw-r--r--   0        0        0   415812 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/images/win32-intro-1.png
+-rw-r--r--   0        0        0   425024 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/images/win32-intro-2.png
+-rw-r--r--   0        0        0   267555 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/images/win32-intro-3.png
+-rw-r--r--   0        0        0   408697 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/images/win32-intro-4.png
+-rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/locales/README.md
+-rw-r--r--   0        0        0    12682 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/locales/messages.pot
+-rw-r--r--   0        0        0     7813 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/locales/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     7929 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/locales/es_ES/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     8149 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/locales/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/locales/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     7924 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/locales/it_IT/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/locales/pl_PL/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     7846 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/locales/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/locales/pt_PT/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    10324 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/locales/ru_RU/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/locales/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/locales/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/locales/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/tessdata/.keep
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/tessdata/LICENSE.txt
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/resources/tessdata/README.txt
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/screengrab/__init__.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/screengrab/main.py
+-rw-r--r--   0        0        0     8741 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/screengrab/permissions.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/screengrab/post_processing.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/screengrab/structures.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/screengrab/system_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/screengrab/handlers/__init__.py
+-rw-r--r--   0        0        0     8341 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/screengrab/handlers/dbus_portal.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/screengrab/handlers/dbus_shell.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/screengrab/handlers/grim.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 normcap-0.5.7/normcap/screengrab/handlers/qt.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/__init__.py
+-rw-r--r--   0        0        0     8124 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/conftest.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/test_app.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/test_main.py
+-rw-r--r--   0        0        0    13257 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/integration/test_normcap.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/integration/test_settings_menu.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/integration/test_tray_menu.py
+-rw-r--r--   0        0        0    37267 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/integration/testcases/00_parse_urls.png
+-rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/integration/testcases/01_parse_colored_url.png
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/integration/testcases/02_detect_window_title.png
+-rw-r--r--   0        0        0    35832 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/integration/testcases/03_parse_emails.png
+-rw-r--r--   0        0        0    61232 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/integration/testcases/04_parse_email_skip_invalid.png
+-rw-r--r--   0        0        0     8012 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/integration/testcases/05_detect_text_with_low_contrast.png
+-rw-r--r--   0        0        0    33416 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/integration/testcases/06_detect_special_characters.png
+-rw-r--r--   0        0        0   152224 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/integration/testcases/07_parse_paragraphs_of_text.png
+-rw-r--r--   0        0        0   168233 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/integration/testcases/08_paragraphs.png
+-rw-r--r--   0        0        0   277892 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/integration/testcases/09_two_columns.png
+-rw-r--r--   0        0        0    95751 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/integration/testcases/10_font_sizes.png
+-rw-r--r--   0        0        0    23053 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/integration/testcases/11_paragraph_with_bullet_points.png
+-rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/integration/testcases/12_not_a_url.png
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/integration/testcases/__init__.py
+-rw-r--r--   0        0        0     9832 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/integration/testcases/data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_clipboard/__init__.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_clipboard/test_main.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_clipboard/test_system_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_clipboard/test_handlers/__init__.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_clipboard/test_handlers/test_pbcopy.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_clipboard/test_handlers/test_qtclipboard.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_clipboard/test_handlers/test_windll.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_clipboard/test_handlers/test_wlclipboard.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_clipboard/test_handlers/test_xclip.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_gui/__init__.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_gui/test_constants.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_gui/test_downloader.py
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_gui/test_introduction.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_gui/test_language_manager.py
+-rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_gui/test_loading_indicator.py
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_gui/test_menu_button.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_gui/test_models.py
+-rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_gui/test_notification.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_gui/test_resources.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_gui/test_settings.py
+-rw-r--r--   0        0        0     8895 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_gui/test_system_info.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_gui/test_tray.py
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_gui/test_update_check.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_gui/test_utils.py
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_gui/test_window.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_ocr/__init__.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_ocr/test_enhance.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_ocr/test_recognize.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_ocr/test_structures.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_ocr/test_tesseract.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_ocr/test_transformer.py
+-rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_ocr/testcases/00_eng.png
+-rw-r--r--   0        0        0    26208 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_ocr/testcases/01_chi_sim.png
+-rw-r--r--   0        0        0    20815 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_ocr/testcases/02_jpn.png
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_ocr/testcases/__init__.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_ocr/testcases/data.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_ocr/testimages/color.png
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_ocr/testimages/dark.png
+-rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_ocr/testimages/light.png
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_ocr/transformers/test_email.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_ocr/transformers/test_paragraph.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_ocr/transformers/test_single_line.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_ocr/transformers/test_url.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_screengrab/split_full_desktop_to_screens.png
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_screengrab/test_main.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_screengrab/test_permissions.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_screengrab/test_post_processing.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_screengrab/test_system_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_screengrab/test_handlers/__init__.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_screengrab/test_handlers/test_dbus_portal.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_screengrab/test_handlers/test_grim.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 normcap-0.5.7/tests/tests_screengrab/test_handlers/test_qt.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 normcap-0.5.7/.gitignore
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 normcap-0.5.7/LICENSE
+-rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 normcap-0.5.7/README.md
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 normcap-0.5.7/hatch_build.py
+-rw-r--r--   0        0        0    10155 2020-02-02 00:00:00.000000 normcap-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     9269 2020-02-02 00:00:00.000000 normcap-0.5.7/PKG-INFO
```

### Comparing `normcap-0.5.6/.pre-commit-config.yaml` & `normcap-0.5.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/CHANGELOG` & `normcap-0.5.7/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 <!-- vim: syntax=Markdown -->
 
 # Changelog
 
+## v0.5.7 (2024-05-18)
+
+- All: Add french translation. Thanks, [@NathanBnm](https://github.com/NathanBnm)! ([#648](https://github.com/dynobo/normcap/pull/648))
+- Linux: Fix crash on wayland in case of user's home directory contains special character. Thanks, [@supersonictw](https://github.com/supersonictw)! ([#643](https://github.com/dynobo/normcap/issues/643))
+- Linux: Fix issue on Ubuntu/Unity where the window doesn't show up. ([#651](https://github.com/dynobo/normcap/pull/651))
+
 ## v0.5.6 (2024-05-08)
 
 - All: Fix minor typos in translations. ([#641](https://github.com/dynobo/normcap/pull/641))
 - Linux: Fix clipboard on Wayland desktops other than GNOME. ([#640](https://github.com/dynobo/normcap/pull/640))
 
 ## v0.5.5 (2024-05-07)
```

### Comparing `normcap-0.5.6/mkdocs.yml` & `normcap-0.5.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/.github/ISSUE_TEMPLATE/bug_report.yml` & `normcap-0.5.7/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/.github/ISSUE_TEMPLATE/detection_quality.yml` & `normcap-0.5.7/.github/ISSUE_TEMPLATE/detection_quality.yml`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/.github/ISSUE_TEMPLATE/feature_request.yml` & `normcap-0.5.7/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/.github/workflows/cicd.yaml` & `normcap-0.5.7/.github/workflows/cicd.yaml`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/adr/001-choose-transparent-windows-as-main-gui.md` & `normcap-0.5.7/adr/001-choose-transparent-windows-as-main-gui.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/adr/002-choose-windows-with-screenshots-as-main-gui.md` & `normcap-0.5.7/adr/002-choose-windows-with-screenshots-as-main-gui.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/adr/003-use-system-tray-as-main-application.md` & `normcap-0.5.7/adr/003-use-system-tray-as-main-application.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/adr/004-do-not-implement-hotkey.md` & `normcap-0.5.7/adr/004-do-not-implement-hotkey.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/adr/005-use-hatch-instead-poetry.md` & `normcap-0.5.7/adr/005-use-hatch-instead-poetry.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/adr/006-use-jeepney-for-dbus-calls.md` & `normcap-0.5.7/adr/006-use-jeepney-for-dbus-calls.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/adr/README.md` & `normcap-0.5.7/adr/README.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/build.py` & `normcap-0.5.7/bundle/build.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/deps.py` & `normcap-0.5.7/bundle/deps.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/l10n.py` & `normcap-0.5.7/bundle/l10n.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/metainfo` & `normcap-0.5.7/bundle/metainfo`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/imgs/normcap-128.png` & `normcap-0.5.7/bundle/imgs/normcap-128.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/imgs/normcap-16.png` & `normcap-0.5.7/bundle/imgs/normcap-16.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/imgs/normcap-256.png` & `normcap-0.5.7/bundle/imgs/normcap-256.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/imgs/normcap-32.png` & `normcap-0.5.7/bundle/imgs/normcap-32.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/imgs/normcap-512.png` & `normcap-0.5.7/bundle/imgs/normcap-512.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/imgs/normcap-64.png` & `normcap-0.5.7/bundle/imgs/normcap-64.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/imgs/normcap.icns` & `normcap-0.5.7/bundle/imgs/normcap.icns`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/imgs/normcap.ico` & `normcap-0.5.7/bundle/imgs/normcap.ico`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/imgs/normcap.svg` & `normcap-0.5.7/bundle/imgs/normcap.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/imgs/normcap_install.bmp` & `normcap-0.5.7/bundle/imgs/normcap_install.bmp`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/imgs/normcap_install.icns` & `normcap-0.5.7/bundle/imgs/normcap_install.icns`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/imgs/normcap_install.png` & `normcap-0.5.7/bundle/imgs/normcap_install.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/imgs/normcap_install.svg` & `normcap-0.5.7/bundle/imgs/normcap_install.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/imgs/normcap_install_bg.bmp` & `normcap-0.5.7/bundle/imgs/normcap_install_bg.bmp`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/imgs/normcap_install_bg.png` & `normcap-0.5.7/bundle/imgs/normcap_install_bg.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/imgs/normcap_install_bg.svg` & `normcap-0.5.7/bundle/imgs/normcap_install_bg.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/imgs/normcap_install_top.bmp` & `normcap-0.5.7/bundle/imgs/normcap_install_top.bmp`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/platforms/linux_briefcase.py` & `normcap-0.5.7/bundle/platforms/linux_briefcase.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/platforms/macos_briefcase.py` & `normcap-0.5.7/bundle/platforms/macos_briefcase.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/platforms/utils.py` & `normcap-0.5.7/bundle/platforms/utils.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/bundle/platforms/windows_briefcase.py` & `normcap-0.5.7/bundle/platforms/windows_briefcase.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/docs/contribute.md` & `normcap-0.5.7/docs/contribute.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/docs/faqs.md` & `normcap-0.5.7/docs/faqs.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/docs/index.md` & `normcap-0.5.7/docs/index.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,29 +3,29 @@
   - navigation
   - toc
 ---
 
 <div class="grid" markdown>
 
 <div markdown>
-# NormCap v0.5.6 {.md-title}
+# NormCap v0.5.7 {.md-title}
 
 <p class="md-subtitle">OCR-powered screenshot tool to capture text<br> instead of images.</p>
 
 Packages with the
 [latest changes](https://github.com/dynobo/normcap/blob/main/CHANGELOG) for your system:
 
 <div class="annotate" markdown>
-- [Download for **Windows**](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64-Windows.msi)
+- [Download for **Windows**](https://github.com/dynobo/normcap/releases/download/v0.5.7/NormCap-0.5.7-x86_64-Windows.msi)
   <small>x86_64, ~120 MB</small>
-- [Download for **Linux**](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64.AppImage)
+- [Download for **Linux**](https://github.com/dynobo/normcap/releases/download/v0.5.7/NormCap-0.5.7-x86_64.AppImage)
   <small>x86_64, ~90 MB</small>
-- [Download for **macOS**](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64-macOS.dmg)
+- [Download for **macOS**](https://github.com/dynobo/normcap/releases/download/v0.5.7/NormCap-0.5.7-x86_64-macOS.dmg)
   <small>x86_64, ~80 MB</small>
-- [Download for **macOS (M1)**](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-arm64-macOS.dmg)
+- [Download for **macOS (M1)**](https://github.com/dynobo/normcap/releases/download/v0.5.7/NormCap-0.5.7-arm64-macOS.dmg)
   <small>arm64, ~65 MB</small>
 </div>
 
 ... or install via
 [FlatHub](https://flathub.org/apps/details/com.github.dynobo.normcap),
 [AUR](https://aur.archlinux.org/packages/normcap) or
 [PyPi](https://pypi.org/project/normcap/).
```

### Comparing `normcap-0.5.6/docs/support.md` & `normcap-0.5.7/docs/support.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/docs/usage.md` & `normcap-0.5.7/docs/usage.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/app.py` & `normcap-0.5.7/normcap/app.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/utils.py` & `normcap-0.5.7/normcap/utils.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/clipboard/main.py` & `normcap-0.5.7/normcap/clipboard/main.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/clipboard/structures.py` & `normcap-0.5.7/normcap/clipboard/structures.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/clipboard/system_info.py` & `normcap-0.5.7/normcap/clipboard/system_info.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/clipboard/handlers/pbcopy.py` & `normcap-0.5.7/normcap/clipboard/handlers/pbcopy.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/clipboard/handlers/qtclipboard.py` & `normcap-0.5.7/normcap/clipboard/handlers/qtclipboard.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/clipboard/handlers/windll.py` & `normcap-0.5.7/normcap/clipboard/handlers/windll.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/clipboard/handlers/wlclipboard.py` & `normcap-0.5.7/normcap/clipboard/handlers/wlclipboard.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/clipboard/handlers/xclip.py` & `normcap-0.5.7/normcap/clipboard/handlers/xclip.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/clipboard/handlers/xsel.py` & `normcap-0.5.7/normcap/clipboard/handlers/xsel.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/gui/constants.py` & `normcap-0.5.7/normcap/gui/constants.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/gui/dbus.py` & `normcap-0.5.7/normcap/gui/dbus.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/gui/downloader.py` & `normcap-0.5.7/normcap/gui/downloader.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/gui/introduction.py` & `normcap-0.5.7/normcap/gui/introduction.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/gui/language_manager.py` & `normcap-0.5.7/normcap/gui/language_manager.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/gui/loading_indicator.py` & `normcap-0.5.7/normcap/gui/loading_indicator.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/gui/menu_button.py` & `normcap-0.5.7/normcap/gui/menu_button.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/gui/models.py` & `normcap-0.5.7/normcap/gui/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,21 +112,21 @@
 
     @property
     def size(self) -> tuple[int, int]:
         """Width and height of rect."""
         return (self.width, self.height)
 
     # ONHOLD: Annotate as Self with Python 3.11
-    def scale(self, scale_factor: float):  # noqa: ANN201
+    def scale(self, factor: float):  # noqa: ANN201
         """Create an integer-scaled copy of the Rect."""
         return Rect(
-            top=int(self.top * scale_factor),
-            bottom=int(self.bottom * scale_factor),
-            left=int(self.left * scale_factor),
-            right=int(self.right * scale_factor),
+            top=int(self.top * factor),
+            bottom=int(self.bottom * factor),
+            left=int(self.left * factor),
+            right=int(self.right * factor),
         )
 
 
 @dataclass()
 class Screen(Rect):
     """Extends Rect with screen specific properties."""
```

### Comparing `normcap-0.5.6/normcap/gui/notification.py` & `normcap-0.5.7/normcap/gui/notification.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/gui/resources.py` & `normcap-0.5.7/normcap/gui/resources.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/gui/settings.py` & `normcap-0.5.7/normcap/gui/settings.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/gui/system_info.py` & `normcap-0.5.7/normcap/gui/system_info.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/gui/tray.py` & `normcap-0.5.7/normcap/gui/tray.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/gui/update_check.py` & `normcap-0.5.7/normcap/gui/update_check.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/gui/utils.py` & `normcap-0.5.7/normcap/gui/utils.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/gui/window.py` & `normcap-0.5.7/normcap/gui/window.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,20 @@
         self.screen_ = screen
 
         self.com = Communicate(parent=self)
         self.color: QtGui.QColor = QtGui.QColor(str(settings.value("color")))
 
         self.setWindowTitle(f"NormCap [{screen.index}]")
         self.setWindowIcon(QtGui.QIcon(":normcap"))
+        self.setWindowFlags(
+            QtGui.Qt.WindowType.FramelessWindowHint
+            | QtGui.Qt.WindowType.CustomizeWindowHint
+            | QtGui.Qt.WindowType.WindowStaysOnTopHint
+        )
+        self.setFocusPolicy(QtCore.Qt.FocusPolicy.StrongFocus)
         self.setAnimated(False)
         self.setEnabled(True)
 
         self.selection_rect: QtCore.QRect = QtCore.QRect()
 
         self._add_image_container()
         self._add_ui_container()
@@ -95,79 +101,86 @@
 
     def _draw_background_image(self) -> None:
         """Draw screenshot as background image."""
         pixmap = QtGui.QPixmap()
         pixmap.convertFromImage(self.screen_.screenshot)
         self.image_container.setPixmap(pixmap)
 
-    def _move_to_position_on_wayland(self) -> None:
+    def _move_to_screen_on_wayland(self) -> None:
         """Move window to respective monitor on Wayland.
 
         In Wayland, the compositor has the responsibility for positioning windows, the
         client itself can't do this. However, there are DE dependent workarounds.
         """
-        if system_info.desktop_environment() == DesktopEnvironment.GNOME:
-            result = dbus.move_windows_via_window_calls_extension(
-                title_id=self.windowTitle(), position=self.screen_
-            )
-            if not result:
-                dbus.move_window_via_gnome_shell_eval(
-                    title_id=self.windowTitle(), position=self.screen_
+
+        def move_to_screen(win: Window) -> None:
+            if system_info.desktop_environment() == DesktopEnvironment.GNOME:
+                result = dbus.move_windows_via_window_calls_extension(
+                    title_id=win.windowTitle(), position=win.screen_
+                )
+                if not result:
+                    dbus.move_window_via_gnome_shell_eval(
+                        title_id=win.windowTitle(), position=win.screen_
+                    )
+            elif system_info.desktop_environment() == DesktopEnvironment.KDE:
+                dbus.move_window_via_kde_kwin_scripting(
+                    title_id=win.windowTitle(), position=win.screen_
+                )
+            else:
+                logger.warning(
+                    "No window move method for %s", system_info.desktop_environment()
                 )
-        elif system_info.desktop_environment() == DesktopEnvironment.KDE:
-            dbus.move_window_via_kde_kwin_scripting(
-                title_id=self.windowTitle(), position=self.screen_
-            )
-        else:
-            logger.warning(
-                "No window move method for %s", system_info.desktop_environment()
-            )
+
+        # Delay move to ensure window is active & registered in window manager.
+        QtCore.QTimer.singleShot(20, lambda: move_to_screen(win=self))
 
     def set_fullscreen(self) -> None:
         """Set window to full screen using platform specific methods."""
+        # TODO: Test in Multi Display setups with different scaling
+        # TODO: Test in Multi Display setups with different position
+        # TODO: Position in Multi Display probably problematic!
         logger.debug("Set window of screen %s to fullscreen", self.screen_.index)
 
         if not self.screen_.screenshot:
             raise ValueError("Screenshot is missing on screen %s", self.screen_)
 
-        self.setWindowFlags(
-            QtGui.Qt.WindowType.FramelessWindowHint
-            | QtGui.Qt.WindowType.CustomizeWindowHint
-            | QtGui.Qt.WindowType.WindowStaysOnTopHint
-        )
-        self.setFocusPolicy(QtCore.Qt.FocusPolicy.StrongFocus)
-
-        # Moving window to corresponding monitor
         # Using scaled window dims to fit sizing with dpr in case scaling is enabled
         # See: https://github.com/dynobo/normcap/issues/397
-        # TODO: Test in Multi Display setups with different scalings
-        # TODO: Test in Multi Display setups with differen position
-        # TODO: Position in Multi Display probably problematic!
         if (
             system_info.display_manager_is_wayland()
             and self.screen_.size == self.screen_.screenshot.size().toTuple()
             and self.screen_.device_pixel_ratio != 1
         ):
+            # TODO: Check if still necessary on latest supported Ubuntu.
+            # If not, remove Screen.scale() and this condition.
             self.setGeometry(*self.screen_.scale().geometry)
         else:
             self.setGeometry(*self.screen_.geometry)
 
-        # On unity, setting min/max window size breaks fullscreen.
         if system_info.desktop_environment() != DesktopEnvironment.UNITY:
+            # On some DEs, setting a fixed window size can enforce the correct size.
+            # However, on Unity, it breaks the full screen view.
             self.setMinimumSize(self.geometry().size())
             self.setMaximumSize(self.geometry().size())
 
-        self.showFullScreen()
+        if system_info.desktop_environment == DesktopEnvironment.UNITY:
+            # For unknown reason .showFullScreen() on Ubuntu 24.04 does not show the
+            # window. Showing the Window in normal state upfront seems to help.
+            # (It seems like .setWindowState(WindowFullScreen) should not be set before
+            # .setVisible(True) on that system. Might be a QT bug.)
+            self.show()
 
+        self.showFullScreen()
         self.setFocus()
 
+        # On Wayland, setting geometry doesn't move the window to the right screen, as
+        # only the compositor is allowed to do this. In case of multi-display setups, we
+        # need to use hacks to position the window:
         if system_info.display_manager_is_wayland():
-            # Movement is delayed to ensure the window is fully active and
-            # registered within the window manager
-            QtCore.QTimer.singleShot(20, lambda: self._move_to_position_on_wayland())
+            self._move_to_screen_on_wayland()
 
     def clear_selection(self) -> None:
         self.selection_rect = QtCore.QRect()
         self.ui_container.rect = self.selection_rect
         self.update()
 
     def get_capture_mode(self) -> CaptureMode:
```

### Comparing `normcap-0.5.6/normcap/ocr/enhance.py` & `normcap-0.5.7/normcap/ocr/enhance.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/ocr/recognize.py` & `normcap-0.5.7/normcap/ocr/recognize.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/ocr/structures.py` & `normcap-0.5.7/normcap/ocr/structures.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/ocr/tesseract.py` & `normcap-0.5.7/normcap/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/ocr/transformer.py` & `normcap-0.5.7/normcap/ocr/transformer.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/ocr/transformers/email.py` & `normcap-0.5.7/normcap/ocr/transformers/email.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/ocr/transformers/multi_line.py` & `normcap-0.5.7/normcap/ocr/transformers/multi_line.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/ocr/transformers/paragraph.py` & `normcap-0.5.7/normcap/ocr/transformers/paragraph.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/ocr/transformers/single_line.py` & `normcap-0.5.7/normcap/ocr/transformers/single_line.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/ocr/transformers/url.py` & `normcap-0.5.7/normcap/ocr/transformers/url.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/ocr/transformers/url_tlds.py` & `normcap-0.5.7/normcap/ocr/transformers/url_tlds.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/icons/normcap.png` & `normcap-0.5.7/normcap/resources/icons/normcap.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/icons/notification.png` & `normcap-0.5.7/normcap/resources/icons/notification.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/icons/parse.png` & `normcap-0.5.7/normcap/resources/icons/parse.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/icons/raw.png` & `normcap-0.5.7/normcap/resources/icons/raw.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/icons/resources.qrc` & `normcap-0.5.7/normcap/resources/icons/resources.qrc`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/icons/settings.png` & `normcap-0.5.7/normcap/resources/icons/settings.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/icons/tray.png` & `normcap-0.5.7/normcap/resources/icons/tray.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/icons/tray_done.png` & `normcap-0.5.7/normcap/resources/icons/tray_done.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/icons/tray_processing.png` & `normcap-0.5.7/normcap/resources/icons/tray_processing.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/images/darwin-intro-1.png` & `normcap-0.5.7/normcap/resources/images/darwin-intro-1.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/images/darwin-intro-2.png` & `normcap-0.5.7/normcap/resources/images/darwin-intro-2.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/images/darwin-intro-3.png` & `normcap-0.5.7/normcap/resources/images/darwin-intro-3.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/images/darwin-intro-4.png` & `normcap-0.5.7/normcap/resources/images/darwin-intro-4.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/images/linux-intro-1.png` & `normcap-0.5.7/normcap/resources/images/linux-intro-1.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/images/linux-intro-2.png` & `normcap-0.5.7/normcap/resources/images/linux-intro-2.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/images/linux-intro-3.png` & `normcap-0.5.7/normcap/resources/images/linux-intro-3.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/images/linux-intro-4.png` & `normcap-0.5.7/normcap/resources/images/linux-intro-4.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/images/win32-intro-1.png` & `normcap-0.5.7/normcap/resources/images/win32-intro-1.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/images/win32-intro-2.png` & `normcap-0.5.7/normcap/resources/images/win32-intro-2.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/images/win32-intro-3.png` & `normcap-0.5.7/normcap/resources/images/win32-intro-3.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/images/win32-intro-4.png` & `normcap-0.5.7/normcap/resources/images/win32-intro-4.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/locales/README.md` & `normcap-0.5.7/normcap/resources/locales/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,144 +13,144 @@
 
 <!-- Generated automatically! -->
 
 | Locale                                   | Progress | Translated |
 | :--------------------------------------- | -------: | ---------: |
 | [de_DE](./de_DE/LC_MESSAGES/messages.po) |     100% |   68 of 68 |
 | [es_ES](./es_ES/LC_MESSAGES/messages.po) |     100% |   68 of 68 |
-| [fr_FR](./fr_FR/LC_MESSAGES/messages.po) |       8% |    6 of 68 |
+| [fr_FR](./fr_FR/LC_MESSAGES/messages.po) |     100% |   68 of 68 |
 | [hi_IN](./hi_IN/LC_MESSAGES/messages.po) |       8% |    6 of 68 |
 | [it_IT](./it_IT/LC_MESSAGES/messages.po) |     100% |   68 of 68 |
 | [pl_PL](./pl_PL/LC_MESSAGES/messages.po) |       8% |    6 of 68 |
 | [pt_BR](./pt_BR/LC_MESSAGES/messages.po) |     100% |   68 of 68 |
 | [pt_PT](./pt_PT/LC_MESSAGES/messages.po) |       8% |    6 of 68 |
 | [ru_RU](./ru_RU/LC_MESSAGES/messages.po) |     100% |   68 of 68 |
 | [sv_SE](./sv_SE/LC_MESSAGES/messages.po) |     100% |   68 of 68 |
 | [uk_UA](./uk_UA/LC_MESSAGES/messages.po) |     100% |   68 of 68 |
 | [zh_CN](./zh_CN/LC_MESSAGES/messages.po) |       8% |    6 of 68 |
 
 ## Proofread existing translations
 
 1. Open one of the translations (`.po`-files) linked in the "Status" table above.
 1. In the file, each string is represented by its English text (`msgid`-field), its
-    translation into the target language (`msgstr`-field) and maybe a translator
-    comment (`#` lines above).
+   translation into the target language (`msgstr`-field) and maybe a translator
+   comment (`#` lines above).
 1. Read the `msgstr`'s one by one and check them for wording, spelling and punctuation.
 1. Propose any changes preferably right away as Pull Request, or if you don't feel
-    comfortable in doing that, report your finding as
-    [new issue](https://github.com/dynobo/normcap/issues/new).
+   comfortable in doing that, report your finding as
+   [new issue](https://github.com/dynobo/normcap/issues/new).
 
 _NOTE:_: Details about the `.po`-file format can be found in the
 [official specification](https://www.gnu.org/software/gettext/manual/html_node/PO-Files.html), if needed.
 
 ## Test existing translations in NormCap
 
 1. Pick a translation from the "Status" table which is fairly complete
 1. Run NormCap (>= `v0.5.0beta1`) with that language, either by changing your system's
-    language to the target language or by starting NormCap with an environment variable
-    set:
+   language to the target language or by starting NormCap with an environment variable
+   set:
     - on Linux:
         - Python package:
-            ```
-            LANGUAGE=<LOCALE_NAME> normcap
-            ```
+          ```
+          LANGUAGE=<LOCALE_NAME> normcap
+          ```
         - AppImage:
-            ```
-            LANGUAGE=<LOCALE_NAME> NormCap-[...].AppImage
-            ```
+          ```
+          LANGUAGE=<LOCALE_NAME> NormCap-[...].AppImage
+          ```
         - FlatPak:
-            ```
-            LANGUAGE=<LOCALE_NAME> flatpak run --command=normcap com.github.dynobo.normcap
-            ```
+          ```
+          LANGUAGE=<LOCALE_NAME> flatpak run --command=normcap com.github.dynobo.normcap
+          ```
     - on macOS:
         - DMG:
-            ```
-            LANG=<LOCALE_NAME> /Applications/NormCap.app/Contents/MacOS/NormCap
-            ```
+          ```
+          LANG=<LOCALE_NAME> /Applications/NormCap.app/Contents/MacOS/NormCap
+          ```
     - on Windows:
         - Python package:
-            ```
-            set LANG=<LOCALE_NAME>
-            normcap
-            ```
+          ```
+          set LANG=<LOCALE_NAME>
+          normcap
+          ```
         - MSI installed:
-            ```
-            set LANG=<LOCALE_NAME>
-            %LOCALAPPDATA%\Programs\NormCap\NormCap.exe
-            ```
+          ```
+          set LANG=<LOCALE_NAME>
+          %LOCALAPPDATA%\Programs\NormCap\NormCap.exe
+          ```
 1. Navigate through the user interface and proofread any text. Pay special attention to
-    whether the presentation of the text looks good. (E.g. strings are too long/short,
-    wrong line breaks, ...)
+   whether the presentation of the text looks good. (E.g. strings are too long/short,
+   wrong line breaks, ...)
 1. Propose any changes preferably right away as Pull Request, or if you don't feel
-    comfortable in doing that, report your finding as
-    [new issue](https://github.com/dynobo/normcap/issues/new).
+   comfortable in doing that, report your finding as
+   [new issue](https://github.com/dynobo/normcap/issues/new).
 
 ## Improve existing translations
 
 1. Identify the file that corresponds to the local you want to edit. You can click the
-    link in the table above, or you can navigate manually to the file at
-    `./normcap/resources/locales/<LOCALE_NAME>/LC_MESSAGES/messages.po`
+   link in the table above, or you can navigate manually to the file at
+   `./normcap/resources/locales/<LOCALE_NAME>/LC_MESSAGES/messages.po`
 1. Open this `messages.po` file and edit the translations. If you like, use the
-    [Free PO-Editor](https://pofile.net/free-po-editor) for easier editing.
-    \
-    **Important:**
+   [Free PO-Editor](https://pofile.net/free-po-editor) for easier editing.
+   \
+   **Important:**
     - Never translate any variables which are written in curly brackets, e.g. `{count}`!
     - Don't bother with updating the header section at the top, it will get overwritten
-        automatically.
+      automatically.
 1. Propose the changed file in a new Pull Request. \
-    (In case you are not familiar with
-    git, you can also always propose a correction or change via a
-    [new issue](https://github.com/dynobo/normcap/issues/new).)
+   (In case you are not familiar with
+   git, you can also always propose a correction or change via a
+   [new issue](https://github.com/dynobo/normcap/issues/new).)
 
 ## Add new translation
 
 _Important:_ If you want to contribute with a new locale, but the process below seems to
 complicated for you, do not hesitate to request the creation of a new, empty `.po` file
 via [opening a new issue](https://github.com/dynobo/normcap/issues/new)!
 
 _Prerequisite:_ Follow the general
 [setup of the development environment](../../../README.md#Development) and activate the
 virtual Python environment via `hatch shell`.
 
 _Note_: All commands should be run in the repository's root directory.
 
 1. Research the `LOCALE_NAME` (e.g. `en_EN` or `de_AT`) of the language which shall be
-    added. `gettext`'s
-    [locale names](https://www.gnu.org/software/gettext/manual/html_node/Locale-Names.html)
-    should be specified in the format `<language-code>_<COUNTRY_CODE>`. Visit the
-    lists of available
-    [language codes](https://www.gnu.org/software/gettext/manual/html_node/Usual-Language-Codes.html)
-    and
-    [country codes](https://www.gnu.org/software/gettext/manual/html_node/Country-Codes.html)
-    to identify possible values.
+   added. `gettext`'s
+   [locale names](https://www.gnu.org/software/gettext/manual/html_node/Locale-Names.html)
+   should be specified in the format `<language-code>_<COUNTRY_CODE>`. Visit the
+   lists of available
+   [language codes](https://www.gnu.org/software/gettext/manual/html_node/Usual-Language-Codes.html)
+   and
+   [country codes](https://www.gnu.org/software/gettext/manual/html_node/Country-Codes.html)
+   to identify possible values.
 1. Run the following command to create an initial `messages.po`-file for the language.
-    Make sure to replace `<LOCALE_NAME>` by the string identified in step 1.
-    ```sh
-    hatch run create-locale <LOCALE_NAME>
-    ```
+   Make sure to replace `<LOCALE_NAME>` by the string identified in step 1.
+   ```sh
+   hatch run create-locale <LOCALE_NAME>
+   ```
 1. Edit the file `./normcap/resources/locales/<LOCALE_NAME>/LC_MESSAGES/messages.po`
-    which was created in step 2. Add your translations as the respective `msgstr`. If
-    you like, use the [Free PO-Editor](https://pofile.net/free-po-editor) for easier
-    editing. \
-    **Important:**
+   which was created in step 2. Add your translations as the respective `msgstr`. If
+   you like, use the [Free PO-Editor](https://pofile.net/free-po-editor) for easier
+   editing. \
+   **Important:**
     - Never translate any variables which are written in curly brackets, e.g. `{count}`!
     - Don't bother with updating the header section at the top, it will get overwritten
-        automatically.
+      automatically.
 1. Compile the new `.po` file to the machine-readable `.mo` file:
-    ```sh
-    hatch run locales-compile
-    ```
+   ```sh
+   hatch run locales-compile
+   ```
 1. To test your translation, run NormCap with the `LANGUAGE` environment variable set:
-    ```sh
-    LANGUAGE=<LOCALE_NAME> python normcap/app.py
-    ```
+   ```sh
+   LANGUAGE=<LOCALE_NAME> python normcap/app.py
+   ```
 1. Propose the inclusion of your new `.po`-file via a pull request to `main`.
 
 ## Update template and languages files
 
 This is only necessary, when translatable strings in NormCap's source code got changed
 (created, modified or deleted).
 
 1. Generate `.pot` file and update all existing `.po` files:
-    ```sh
-    hatch run locales-update
-    ```
+   ```sh
+   hatch run locales-update
+   ```
```

### Comparing `normcap-0.5.6/normcap/resources/locales/messages.pot` & `normcap-0.5.7/normcap/resources/locales/messages.pot`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/locales/de_DE/LC_MESSAGES/messages.mo` & `normcap-0.5.7/normcap/resources/locales/de_DE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/locales/es_ES/LC_MESSAGES/messages.mo` & `normcap-0.5.7/normcap/resources/locales/es_ES/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/locales/fr_FR/LC_MESSAGES/messages.mo` & `normcap-0.5.7/normcap/resources/locales/hi_IN/LC_MESSAGES/messages.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,17 +1,17 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2024-05-06 21:18+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language: fr_FR\n"
-"Language-Team: fr_FR <LL@li.org>\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Language: hi_IN\n"
+"Language-Team: hi_IN <LL@li.org>\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.15.0\n"
 
 msgid "1 URL captured"
 msgid_plural "{count} URLs captured"
```

### Comparing `normcap-0.5.6/normcap/resources/locales/hi_IN/LC_MESSAGES/messages.mo` & `normcap-0.5.7/normcap/resources/locales/pt_PT/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,16 +1,16 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2024-05-06 21:18+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language: hi_IN\n"
-"Language-Team: hi_IN <LL@li.org>\n"
+"Language: pt_PT\n"
+"Language-Team: pt_PT <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.15.0\n"
 
 msgid "1 URL captured"
```

### Comparing `normcap-0.5.6/normcap/resources/locales/it_IT/LC_MESSAGES/messages.mo` & `normcap-0.5.7/normcap/resources/locales/it_IT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/locales/pl_PL/LC_MESSAGES/messages.mo` & `normcap-0.5.7/normcap/resources/locales/pl_PL/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/locales/pt_BR/LC_MESSAGES/messages.mo` & `normcap-0.5.7/normcap/resources/locales/pt_BR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/locales/ru_RU/LC_MESSAGES/messages.mo` & `normcap-0.5.7/normcap/resources/locales/ru_RU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/locales/sv_SE/LC_MESSAGES/messages.mo` & `normcap-0.5.7/normcap/resources/locales/sv_SE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/locales/uk_UA/LC_MESSAGES/messages.mo` & `normcap-0.5.7/normcap/resources/locales/uk_UA/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/locales/zh_CN/LC_MESSAGES/messages.mo` & `normcap-0.5.7/normcap/resources/locales/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/tessdata/LICENSE.txt` & `normcap-0.5.7/normcap/resources/tessdata/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/resources/tessdata/README.txt` & `normcap-0.5.7/normcap/resources/tessdata/README.txt`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/screengrab/__init__.py` & `normcap-0.5.7/normcap/screengrab/__init__.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/screengrab/main.py` & `normcap-0.5.7/normcap/screengrab/main.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/screengrab/permissions.py` & `normcap-0.5.7/normcap/screengrab/permissions.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/screengrab/post_processing.py` & `normcap-0.5.7/normcap/screengrab/post_processing.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/screengrab/structures.py` & `normcap-0.5.7/normcap/screengrab/structures.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/screengrab/system_info.py` & `normcap-0.5.7/normcap/screengrab/system_info.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/screengrab/handlers/dbus_portal.py` & `normcap-0.5.7/normcap/screengrab/handlers/dbus_portal.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 import random
 import re
 import sys
 from pathlib import Path
 from typing import Optional
-from urllib.parse import urlparse
+from urllib.parse import unquote, urlparse
 
 from PySide6 import QtCore, QtDBus, QtGui
 
 from normcap.screengrab import system_info
 from normcap.screengrab.post_processing import split_full_desktop_to_screens
 
 logger = logging.getLogger(__name__)
@@ -195,16 +195,17 @@
     portal.on_exception.disconnect(_exception_triggered)
 
     for error in exceptions:
         raise error
 
     uri = result[0]
     parsed_uri = urlparse(uri)
+    parsed_path = unquote(parsed_uri.path)
 
-    image_path = Path(parsed_uri.path)
+    image_path = Path(parsed_path)
     image = QtGui.QImage(image_path)
 
     # XDG Portal save the image file to the users xdg-pictures directory. To not let
     # them pile up, we try to remove it:
     try:
         image_path.unlink()
     except PermissionError:
```

### Comparing `normcap-0.5.6/normcap/screengrab/handlers/dbus_shell.py` & `normcap-0.5.7/normcap/screengrab/handlers/dbus_shell.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/screengrab/handlers/grim.py` & `normcap-0.5.7/normcap/screengrab/handlers/grim.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/normcap/screengrab/handlers/qt.py` & `normcap-0.5.7/normcap/screengrab/handlers/qt.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/conftest.py` & `normcap-0.5.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/test_app.py` & `normcap-0.5.7/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/test_main.py` & `normcap-0.5.7/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/test_utils.py` & `normcap-0.5.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/integration/test_normcap.py` & `normcap-0.5.7/tests/integration/test_normcap.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/integration/test_settings_menu.py` & `normcap-0.5.7/tests/integration/test_settings_menu.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/integration/test_tray_menu.py` & `normcap-0.5.7/tests/integration/test_tray_menu.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/integration/testcases/00_parse_urls.png` & `normcap-0.5.7/tests/integration/testcases/00_parse_urls.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/integration/testcases/01_parse_colored_url.png` & `normcap-0.5.7/tests/integration/testcases/01_parse_colored_url.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/integration/testcases/02_detect_window_title.png` & `normcap-0.5.7/tests/integration/testcases/02_detect_window_title.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/integration/testcases/03_parse_emails.png` & `normcap-0.5.7/tests/integration/testcases/03_parse_emails.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/integration/testcases/04_parse_email_skip_invalid.png` & `normcap-0.5.7/tests/integration/testcases/04_parse_email_skip_invalid.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/integration/testcases/05_detect_text_with_low_contrast.png` & `normcap-0.5.7/tests/integration/testcases/05_detect_text_with_low_contrast.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/integration/testcases/06_detect_special_characters.png` & `normcap-0.5.7/tests/integration/testcases/06_detect_special_characters.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/integration/testcases/07_parse_paragraphs_of_text.png` & `normcap-0.5.7/tests/integration/testcases/07_parse_paragraphs_of_text.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/integration/testcases/08_paragraphs.png` & `normcap-0.5.7/tests/integration/testcases/08_paragraphs.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/integration/testcases/09_two_columns.png` & `normcap-0.5.7/tests/integration/testcases/09_two_columns.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/integration/testcases/10_font_sizes.png` & `normcap-0.5.7/tests/integration/testcases/10_font_sizes.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/integration/testcases/11_paragraph_with_bullet_points.png` & `normcap-0.5.7/tests/integration/testcases/11_paragraph_with_bullet_points.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/integration/testcases/12_not_a_url.png` & `normcap-0.5.7/tests/integration/testcases/12_not_a_url.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/integration/testcases/data.py` & `normcap-0.5.7/tests/integration/testcases/data.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_clipboard/test_main.py` & `normcap-0.5.7/tests/tests_clipboard/test_main.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_clipboard/test_system_info.py` & `normcap-0.5.7/tests/tests_clipboard/test_system_info.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_clipboard/test_handlers/test_pbcopy.py` & `normcap-0.5.7/tests/tests_clipboard/test_handlers/test_pbcopy.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_clipboard/test_handlers/test_qtclipboard.py` & `normcap-0.5.7/tests/tests_clipboard/test_handlers/test_qtclipboard.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_clipboard/test_handlers/test_windll.py` & `normcap-0.5.7/tests/tests_clipboard/test_handlers/test_windll.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_clipboard/test_handlers/test_wlclipboard.py` & `normcap-0.5.7/tests/tests_clipboard/test_handlers/test_wlclipboard.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_clipboard/test_handlers/test_xclip.py` & `normcap-0.5.7/tests/tests_clipboard/test_handlers/test_xclip.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_gui/test_downloader.py` & `normcap-0.5.7/tests/tests_gui/test_downloader.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_gui/test_introduction.py` & `normcap-0.5.7/tests/tests_gui/test_introduction.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_gui/test_language_manager.py` & `normcap-0.5.7/tests/tests_gui/test_language_manager.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_gui/test_loading_indicator.py` & `normcap-0.5.7/tests/tests_gui/test_loading_indicator.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_gui/test_menu_button.py` & `normcap-0.5.7/tests/tests_gui/test_menu_button.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_gui/test_models.py` & `normcap-0.5.7/tests/tests_gui/test_models.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_gui/test_notification.py` & `normcap-0.5.7/tests/tests_gui/test_notification.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_gui/test_resources.py` & `normcap-0.5.7/tests/tests_gui/test_resources.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_gui/test_settings.py` & `normcap-0.5.7/tests/tests_gui/test_settings.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_gui/test_system_info.py` & `normcap-0.5.7/tests/tests_gui/test_system_info.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_gui/test_tray.py` & `normcap-0.5.7/tests/tests_gui/test_tray.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_gui/test_update_check.py` & `normcap-0.5.7/tests/tests_gui/test_update_check.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_gui/test_utils.py` & `normcap-0.5.7/tests/tests_gui/test_utils.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_gui/test_window.py` & `normcap-0.5.7/tests/tests_gui/test_window.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_ocr/test_enhance.py` & `normcap-0.5.7/tests/tests_ocr/test_enhance.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_ocr/test_recognize.py` & `normcap-0.5.7/tests/tests_ocr/test_recognize.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_ocr/test_structures.py` & `normcap-0.5.7/tests/tests_ocr/test_structures.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_ocr/test_tesseract.py` & `normcap-0.5.7/tests/tests_ocr/test_tesseract.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_ocr/test_transformer.py` & `normcap-0.5.7/tests/tests_ocr/test_transformer.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_ocr/testcases/00_eng.png` & `normcap-0.5.7/tests/tests_ocr/testcases/00_eng.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_ocr/testcases/01_chi_sim.png` & `normcap-0.5.7/tests/tests_ocr/testcases/01_chi_sim.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_ocr/testcases/02_jpn.png` & `normcap-0.5.7/tests/tests_ocr/testcases/02_jpn.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_ocr/testcases/data.py` & `normcap-0.5.7/tests/tests_ocr/testcases/data.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_ocr/testimages/color.png` & `normcap-0.5.7/tests/tests_ocr/testimages/color.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_ocr/testimages/dark.png` & `normcap-0.5.7/tests/tests_ocr/testimages/dark.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_ocr/testimages/light.png` & `normcap-0.5.7/tests/tests_ocr/testimages/light.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_ocr/transformers/test_email.py` & `normcap-0.5.7/tests/tests_ocr/transformers/test_email.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_ocr/transformers/test_paragraph.py` & `normcap-0.5.7/tests/tests_ocr/transformers/test_paragraph.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_ocr/transformers/test_single_line.py` & `normcap-0.5.7/tests/tests_ocr/transformers/test_single_line.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_ocr/transformers/test_url.py` & `normcap-0.5.7/tests/tests_ocr/transformers/test_url.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_screengrab/split_full_desktop_to_screens.png` & `normcap-0.5.7/tests/tests_screengrab/split_full_desktop_to_screens.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_screengrab/test_main.py` & `normcap-0.5.7/tests/tests_screengrab/test_main.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_screengrab/test_permissions.py` & `normcap-0.5.7/tests/tests_screengrab/test_permissions.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_screengrab/test_post_processing.py` & `normcap-0.5.7/tests/tests_screengrab/test_post_processing.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_screengrab/test_system_info.py` & `normcap-0.5.7/tests/tests_screengrab/test_system_info.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_screengrab/test_handlers/test_dbus_portal.py` & `normcap-0.5.7/tests/tests_screengrab/test_handlers/test_dbus_portal.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_screengrab/test_handlers/test_grim.py` & `normcap-0.5.7/tests/tests_screengrab/test_handlers/test_grim.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/tests/tests_screengrab/test_handlers/test_qt.py` & `normcap-0.5.7/tests/tests_screengrab/test_handlers/test_qt.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/.gitignore` & `normcap-0.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/LICENSE` & `normcap-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `normcap-0.5.6/README.md` & `normcap-0.5.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -28,34 +28,34 @@
 
 Choose **_one_** of the options for a prebuilt release. If you encounter an issue please
 take a look at the [FAQs](https://dynobo.github.io/normcap/#faqs) or
 [report](https://github.com/dynobo/normcap/issues) it.
 
 #### Windows
 
-- [NormCap-0.5.6-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64-Windows.msi)
+- [NormCap-0.5.7-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.5.7/NormCap-0.5.7-x86_64-Windows.msi)
   (Installer)
 
 #### Linux
 
-- [NormCap-0.5.6-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64.AppImage)
+- [NormCap-0.5.7-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.5.7/NormCap-0.5.7-x86_64.AppImage)
   (Binary)
 - [`normcap` @ AUR](https://aur.archlinux.org/packages/normcap) (Arch/Manjaro)
 - [com.github.dynobo.normcap @ FlatHub](https://flathub.org/apps/details/com.github.dynobo.normcap)
   (FlatPak)
 
 #### macOS
 
 Note: You have to allow the unsigned application on first start: "System Preferences" →
 "Security & Privacy" → "General" → "Open anyway". You also have to allow NormCap to take
 screenshots. ([#135](https://github.com/dynobo/normcap/issues/135))
 
-- [NormCap-0.5.6-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64-macOS.dmg)
+- [NormCap-0.5.7-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.5.7/NormCap-0.5.7-x86_64-macOS.dmg)
   (Installer for x86/64)
-- [NormCap-0.5.6-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-arm64-macOS.dmg)
+- [NormCap-0.5.7-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.5.7/NormCap-0.5.7-arm64-macOS.dmg)
   (Installer for M1)
 
 ## Install Python package
 
 As an _alternative_ to a prebuilt package from above you can install the
 [NormCap Python package](https://pypi.org/project/normcap/) for **Python >=3.9**, but it
 is a bit more complicated:
```

#### html2text {}

```diff
@@ -21,28 +21,28 @@
 /github.com/dynobo/normcap/releases) | [Changelog](https://github.com/dynobo/
 normcap/blob/main/CHANGELOG) [![Screencast](https://user-
 images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-
 cef1cb5dbc47.gif)](https://raw.githubusercontent.com/dynobo/normcap/main/
 assets/normcap.gif) ## Quickstart Choose **_one_** of the options for a
 prebuilt release. If you encounter an issue please take a look at the [FAQs]
 (https://dynobo.github.io/normcap/#faqs) or [report](https://github.com/dynobo/
-normcap/issues) it. #### Windows - [NormCap-0.5.6-x86_64-Windows.msi](https://
-github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64-
-Windows.msi) (Installer) #### Linux - [NormCap-0.5.6-x86_64.AppImage](https://
-github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-
+normcap/issues) it. #### Windows - [NormCap-0.5.7-x86_64-Windows.msi](https://
+github.com/dynobo/normcap/releases/download/v0.5.7/NormCap-0.5.7-x86_64-
+Windows.msi) (Installer) #### Linux - [NormCap-0.5.7-x86_64.AppImage](https://
+github.com/dynobo/normcap/releases/download/v0.5.7/NormCap-0.5.7-
 x86_64.AppImage) (Binary) - [`normcap` @ AUR](https://aur.archlinux.org/
 packages/normcap) (Arch/Manjaro) - [com.github.dynobo.normcap @ FlatHub](https:
 //flathub.org/apps/details/com.github.dynobo.normcap) (FlatPak) #### macOS
 Note: You have to allow the unsigned application on first start: "System
 Preferences" â "Security & Privacy" â "General" â "Open anyway". You also
 have to allow NormCap to take screenshots. ([#135](https://github.com/dynobo/
-normcap/issues/135)) - [NormCap-0.5.6-x86_64-macOS.dmg](https://github.com/
-dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64-macOS.dmg)
-(Installer for x86/64) - [NormCap-0.5.6-arm64-macOS.dmg](https://github.com/
-dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-arm64-macOS.dmg)
+normcap/issues/135)) - [NormCap-0.5.7-x86_64-macOS.dmg](https://github.com/
+dynobo/normcap/releases/download/v0.5.7/NormCap-0.5.7-x86_64-macOS.dmg)
+(Installer for x86/64) - [NormCap-0.5.7-arm64-macOS.dmg](https://github.com/
+dynobo/normcap/releases/download/v0.5.7/NormCap-0.5.7-arm64-macOS.dmg)
 (Installer for M1) ## Install Python package As an _alternative_ to a prebuilt
 package from above you can install the [NormCap Python package](https://
 pypi.org/project/normcap/) for **Python >=3.9**, but it is a bit more
 complicated: #### On Linux ```sh # Install dependencies (Ubuntu/Debian) sudo
 apt install build-essential tesseract-ocr tesseract-ocr-eng libtesseract-dev
 libleptonica-dev wl-clipboard ## Install dependencies (Arch) sudo pacman -
 S tesseract tesseract-data-eng wl-clipboard ## Install dependencies (Fedora)
```

### Comparing `normcap-0.5.6/pyproject.toml` & `normcap-0.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "normcap"
-version = "0.5.6"
+version = "0.5.7"
 description = "OCR-powered screen-capture tool to capture information instead of images."
 keywords = ["screenshot", "ocr", "capture", "clipboard"]
 readme = "README.md"
 requires-python = ">=3.9,<3.12"
 license = "GPL-3.0-or-later"
 authors = [{ name = "dynobo", email = "dynobo@mailbox.org" }]
 classifiers = [
@@ -226,15 +226,15 @@
 no_show = true
 cluster = true
 max_cluster_size = 1
 
 [tool.briefcase]
 project_name = "NormCap"
 bundle = "eu.dynobo"
-version = "0.5.6"
+version = "0.5.7"
 url = "https://github.com/dynobo/normcap"
 license = "GPLv3"
 author = 'dynobo'
 author_email = "dynobo@mailbox.org"
 
 [tool.briefcase.app.normcap]
 formal_name = "NormCap"
@@ -341,15 +341,15 @@
 """
 
 [tool.briefcase.app.normcap.windows]
 use_full_install_path = false
 
 
 [tool.tbump.version]
-current = "0.5.6"
+current = "0.5.7"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (\-
```

### Comparing `normcap-0.5.6/PKG-INFO` & `normcap-0.5.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: normcap
-Version: 0.5.6
+Version: 0.5.7
 Summary: OCR-powered screen-capture tool to capture information instead of images.
 Project-URL: Homepage, https://dynobo.github.io/normcap/
 Project-URL: Issues, https://github.com/dynobo/normcap/issues
 Project-URL: Source Code, https://github.com/dynobo/normcap
 Project-URL: FAQs, https://dynobo.github.io/normcap/#faqs
 Project-URL: Changelog, https://github.com/dynobo/normcap/blob/main/CHANGELOG
 Author-email: dynobo <dynobo@mailbox.org>
@@ -60,34 +60,34 @@
 
 Choose **_one_** of the options for a prebuilt release. If you encounter an issue please
 take a look at the [FAQs](https://dynobo.github.io/normcap/#faqs) or
 [report](https://github.com/dynobo/normcap/issues) it.
 
 #### Windows
 
-- [NormCap-0.5.6-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64-Windows.msi)
+- [NormCap-0.5.7-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.5.7/NormCap-0.5.7-x86_64-Windows.msi)
   (Installer)
 
 #### Linux
 
-- [NormCap-0.5.6-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64.AppImage)
+- [NormCap-0.5.7-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.5.7/NormCap-0.5.7-x86_64.AppImage)
   (Binary)
 - [`normcap` @ AUR](https://aur.archlinux.org/packages/normcap) (Arch/Manjaro)
 - [com.github.dynobo.normcap @ FlatHub](https://flathub.org/apps/details/com.github.dynobo.normcap)
   (FlatPak)
 
 #### macOS
 
 Note: You have to allow the unsigned application on first start: "System Preferences" →
 "Security & Privacy" → "General" → "Open anyway". You also have to allow NormCap to take
 screenshots. ([#135](https://github.com/dynobo/normcap/issues/135))
 
-- [NormCap-0.5.6-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64-macOS.dmg)
+- [NormCap-0.5.7-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.5.7/NormCap-0.5.7-x86_64-macOS.dmg)
   (Installer for x86/64)
-- [NormCap-0.5.6-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-arm64-macOS.dmg)
+- [NormCap-0.5.7-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.5.7/NormCap-0.5.7-arm64-macOS.dmg)
   (Installer for M1)
 
 ## Install Python package
 
 As an _alternative_ to a prebuilt package from above you can install the
 [NormCap Python package](https://pypi.org/project/normcap/) for **Python >=3.9**, but it
 is a bit more complicated:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: normcap Version: 0.5.6 Summary: OCR-powered screen-
+Metadata-Version: 2.3 Name: normcap Version: 0.5.7 Summary: OCR-powered screen-
 capture tool to capture information instead of images. Project-URL: Homepage,
 https://dynobo.github.io/normcap/ Project-URL: Issues, https://github.com/
 dynobo/normcap/issues Project-URL: Source Code, https://github.com/dynobo/
 normcap Project-URL: FAQs, https://dynobo.github.io/normcap/#faqs Project-URL:
 Changelog, https://github.com/dynobo/normcap/blob/main/CHANGELOG Author-email:
 dynobo
 mailbox.org> License-Expression: GPL-3.0-or-later License-File: LICENSE
@@ -41,28 +41,28 @@
 /github.com/dynobo/normcap/releases) | [Changelog](https://github.com/dynobo/
 normcap/blob/main/CHANGELOG) [![Screencast](https://user-
 images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-
 cef1cb5dbc47.gif)](https://raw.githubusercontent.com/dynobo/normcap/main/
 assets/normcap.gif) ## Quickstart Choose **_one_** of the options for a
 prebuilt release. If you encounter an issue please take a look at the [FAQs]
 (https://dynobo.github.io/normcap/#faqs) or [report](https://github.com/dynobo/
-normcap/issues) it. #### Windows - [NormCap-0.5.6-x86_64-Windows.msi](https://
-github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64-
-Windows.msi) (Installer) #### Linux - [NormCap-0.5.6-x86_64.AppImage](https://
-github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-
+normcap/issues) it. #### Windows - [NormCap-0.5.7-x86_64-Windows.msi](https://
+github.com/dynobo/normcap/releases/download/v0.5.7/NormCap-0.5.7-x86_64-
+Windows.msi) (Installer) #### Linux - [NormCap-0.5.7-x86_64.AppImage](https://
+github.com/dynobo/normcap/releases/download/v0.5.7/NormCap-0.5.7-
 x86_64.AppImage) (Binary) - [`normcap` @ AUR](https://aur.archlinux.org/
 packages/normcap) (Arch/Manjaro) - [com.github.dynobo.normcap @ FlatHub](https:
 //flathub.org/apps/details/com.github.dynobo.normcap) (FlatPak) #### macOS
 Note: You have to allow the unsigned application on first start: "System
 Preferences" â "Security & Privacy" â "General" â "Open anyway". You also
 have to allow NormCap to take screenshots. ([#135](https://github.com/dynobo/
-normcap/issues/135)) - [NormCap-0.5.6-x86_64-macOS.dmg](https://github.com/
-dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64-macOS.dmg)
-(Installer for x86/64) - [NormCap-0.5.6-arm64-macOS.dmg](https://github.com/
-dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-arm64-macOS.dmg)
+normcap/issues/135)) - [NormCap-0.5.7-x86_64-macOS.dmg](https://github.com/
+dynobo/normcap/releases/download/v0.5.7/NormCap-0.5.7-x86_64-macOS.dmg)
+(Installer for x86/64) - [NormCap-0.5.7-arm64-macOS.dmg](https://github.com/
+dynobo/normcap/releases/download/v0.5.7/NormCap-0.5.7-arm64-macOS.dmg)
 (Installer for M1) ## Install Python package As an _alternative_ to a prebuilt
 package from above you can install the [NormCap Python package](https://
 pypi.org/project/normcap/) for **Python >=3.9**, but it is a bit more
 complicated: #### On Linux ```sh # Install dependencies (Ubuntu/Debian) sudo
 apt install build-essential tesseract-ocr tesseract-ocr-eng libtesseract-dev
 libleptonica-dev wl-clipboard ## Install dependencies (Arch) sudo pacman -
 S tesseract tesseract-data-eng wl-clipboard ## Install dependencies (Fedora)
```

