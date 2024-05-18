# Comparing `tmp/pyprland-2.2.9.tar.gz` & `tmp/pyprland-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprland-2.2.9.tar", max compression
+gzip compressed data, was "pyprland-2.3.0.tar", max compression
```

## Comparing `pyprland-2.2.9.tar` & `pyprland-2.3.0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.2.9/LICENSE
--rw-r--r--   0        0        0     4458 2024-04-14 21:04:51.031595 pyprland-2.2.9/README.md
--rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.9/pyprland/__init__.py
--rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.9/pyprland/adapters/__init__.py
--rw-r--r--   0        0        0      400 2024-04-05 20:13:47.397221 pyprland-2.2.9/pyprland/adapters/colors.py
--rw-r--r--   0        0        0     4377 2024-03-03 01:47:24.894367 pyprland-2.2.9/pyprland/adapters/menus.py
--rw-r--r--   0        0        0     1395 2024-04-08 20:00:16.866561 pyprland-2.2.9/pyprland/adapters/units.py
--rwxr-xr-x   0        0        0    17129 2024-04-19 17:18:47.257998 pyprland-2.2.9/pyprland/command.py
--rw-r--r--   0        0        0     7746 2024-04-19 16:25:06.663994 pyprland-2.2.9/pyprland/common.py
--rw-r--r--   0        0        0     7233 2024-04-19 16:13:14.787837 pyprland-2.2.9/pyprland/ipc.py
--rw-r--r--   0        0        0       45 2024-03-03 01:47:24.897701 pyprland-2.2.9/pyprland/plugins/__init__.py
--rw-r--r--   0        0        0      106 2024-03-03 01:47:24.897701 pyprland-2.2.9/pyprland/plugins/experimental.py
--rw-r--r--   0        0        0     1647 2024-04-19 16:13:14.787837 pyprland-2.2.9/pyprland/plugins/expose.py
--rw-r--r--   0        0        0     1386 2024-03-30 16:09:04.631012 pyprland-2.2.9/pyprland/plugins/fetch_client_menu.py
--rw-r--r--   0        0        0     2018 2024-04-14 20:56:27.261784 pyprland-2.2.9/pyprland/plugins/gbar.py
--rw-r--r--   0        0        0     2589 2024-04-09 20:50:41.034540 pyprland-2.2.9/pyprland/plugins/interface.py
--rw-r--r--   0        0        0     7972 2024-03-03 01:47:24.917701 pyprland-2.2.9/pyprland/plugins/layout_center.py
--rw-r--r--   0        0        0     1677 2024-03-03 01:47:24.901034 pyprland-2.2.9/pyprland/plugins/lost_windows.py
--rw-r--r--   0        0        0     1760 2024-04-19 16:13:14.787837 pyprland-2.2.9/pyprland/plugins/magnify.py
--rw-r--r--   0        0        0     8680 2024-04-13 18:26:06.759226 pyprland-2.2.9/pyprland/plugins/monitors.py
--rw-r--r--   0        0        0     3922 2024-03-03 01:47:24.904368 pyprland-2.2.9/pyprland/plugins/monitors_v0.py
--rw-r--r--   0        0        0     2071 2024-04-19 16:25:06.663994 pyprland-2.2.9/pyprland/plugins/pyprland.py
--rw-r--r--   0        0        0    26354 2024-04-19 16:48:51.098660 pyprland-2.2.9/pyprland/plugins/scratchpads/__init__.py
--rw-r--r--   0        0        0     2641 2024-04-12 17:24:50.007112 pyprland-2.2.9/pyprland/plugins/scratchpads/animations.py
--rw-r--r--   0        0        0     2106 2024-04-12 17:23:41.858277 pyprland-2.2.9/pyprland/plugins/scratchpads/helpers.py
--rw-r--r--   0        0        0     3436 2024-04-12 17:21:22.436949 pyprland-2.2.9/pyprland/plugins/scratchpads/lookup.py
--rw-r--r--   0        0        0     4268 2024-04-19 16:46:31.746537 pyprland-2.2.9/pyprland/plugins/scratchpads/objects.py
--rw-r--r--   0        0        0     1058 2024-03-03 01:47:24.907701 pyprland-2.2.9/pyprland/plugins/shift_monitors.py
--rw-r--r--   0        0        0     4161 2024-04-09 15:53:04.519223 pyprland-2.2.9/pyprland/plugins/shortcuts_menu.py
--rw-r--r--   0        0        0     4062 2024-04-19 16:13:14.787837 pyprland-2.2.9/pyprland/plugins/system_notifier.py
--rw-r--r--   0        0        0      519 2024-03-03 01:47:24.911034 pyprland-2.2.9/pyprland/plugins/toggle_dpms.py
--rw-r--r--   0        0        0     1063 2024-03-03 01:47:24.917701 pyprland-2.2.9/pyprland/plugins/toggle_special.py
--rw-r--r--   0        0        0     5335 2024-04-13 18:20:53.870052 pyprland-2.2.9/pyprland/plugins/wallpapers.py
--rw-r--r--   0        0        0     2547 2024-04-19 16:13:14.787837 pyprland-2.2.9/pyprland/plugins/workspaces_follow_focus.py
--rw-r--r--   0        0        0      725 2024-04-19 17:18:47.247997 pyprland-2.2.9/pyproject.toml
--rw-r--r--   0        0        0     4997 1970-01-01 00:00:00.000000 pyprland-2.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.3.0/LICENSE
+-rw-r--r--   0        0        0     5427 2024-05-18 15:13:31.365799 pyprland-2.3.0/README.md
+-rw-r--r--   0        0        0       24 2024-05-16 19:14:17.152144 pyprland-2.3.0/pyprland/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-16 19:14:17.148810 pyprland-2.3.0/pyprland/adapters/__init__.py
+-rw-r--r--   0        0        0      386 2024-05-16 19:14:17.148810 pyprland-2.3.0/pyprland/adapters/colors.py
+-rw-r--r--   0        0        0     4848 2024-05-18 13:01:21.799747 pyprland-2.3.0/pyprland/adapters/menus.py
+-rw-r--r--   0        0        0     1462 2024-05-16 20:28:22.384986 pyprland-2.3.0/pyprland/adapters/units.py
+-rw-r--r--   0        0        0    18462 2024-05-17 22:31:04.698344 pyprland-2.3.0/pyprland/command.py
+-rw-r--r--   0        0        0     8470 2024-05-17 21:59:35.557745 pyprland-2.3.0/pyprland/common.py
+-rw-r--r--   0        0        0     8086 2024-05-17 22:07:11.198968 pyprland-2.3.0/pyprland/ipc.py
+-rw-r--r--   0        0        0       49 2024-05-16 19:14:17.152144 pyprland-2.3.0/pyprland/plugins/__init__.py
+-rw-r--r--   0        0        0      115 2024-05-16 19:14:17.152144 pyprland-2.3.0/pyprland/plugins/experimental.py
+-rw-r--r--   0        0        0     1658 2024-05-16 20:12:25.826075 pyprland-2.3.0/pyprland/plugins/expose.py
+-rw-r--r--   0        0        0     1370 2024-05-16 19:14:17.152144 pyprland-2.3.0/pyprland/plugins/fetch_client_menu.py
+-rw-r--r--   0        0        0     2723 2024-05-17 21:51:17.035559 pyprland-2.3.0/pyprland/plugins/gbar.py
+-rw-r--r--   0        0        0     2655 2024-05-16 20:24:49.329951 pyprland-2.3.0/pyprland/plugins/interface.py
+-rw-r--r--   0        0        0     8084 2024-05-18 12:50:01.915976 pyprland-2.3.0/pyprland/plugins/layout_center.py
+-rw-r--r--   0        0        0     1731 2024-05-16 20:31:35.359564 pyprland-2.3.0/pyprland/plugins/lost_windows.py
+-rw-r--r--   0        0        0     2514 2024-05-18 12:40:23.740738 pyprland-2.3.0/pyprland/plugins/magnify.py
+-rw-r--r--   0        0        0    11159 2024-05-18 15:09:44.027753 pyprland-2.3.0/pyprland/plugins/monitors.py
+-rw-r--r--   0        0        0     3817 2024-05-16 19:14:17.152144 pyprland-2.3.0/pyprland/plugins/monitors_v0.py
+-rw-r--r--   0        0        0     3121 2024-05-16 20:27:48.054173 pyprland-2.3.0/pyprland/plugins/pyprland.py
+-rw-r--r--   0        0        0    31607 2024-05-18 13:08:09.554633 pyprland-2.3.0/pyprland/plugins/scratchpads/__init__.py
+-rw-r--r--   0        0        0     2842 2024-05-17 17:55:08.207991 pyprland-2.3.0/pyprland/plugins/scratchpads/animations.py
+-rw-r--r--   0        0        0     2702 2024-05-18 12:34:55.300430 pyprland-2.3.0/pyprland/plugins/scratchpads/helpers.py
+-rw-r--r--   0        0        0     4036 2024-05-18 13:07:36.207295 pyprland-2.3.0/pyprland/plugins/scratchpads/lookup.py
+-rw-r--r--   0        0        0     5997 2024-05-18 13:08:46.975391 pyprland-2.3.0/pyprland/plugins/scratchpads/objects.py
+-rw-r--r--   0        0        0     1103 2024-05-16 20:02:45.022300 pyprland-2.3.0/pyprland/plugins/shift_monitors.py
+-rw-r--r--   0        0        0     4245 2024-05-18 12:58:41.979853 pyprland-2.3.0/pyprland/plugins/shortcuts_menu.py
+-rw-r--r--   0        0        0     4804 2024-05-16 20:40:18.898697 pyprland-2.3.0/pyprland/plugins/system_notifier.py
+-rw-r--r--   0        0        0      570 2024-05-16 19:14:17.152144 pyprland-2.3.0/pyprland/plugins/toggle_dpms.py
+-rw-r--r--   0        0        0     1120 2024-05-16 19:55:58.745845 pyprland-2.3.0/pyprland/plugins/toggle_special.py
+-rw-r--r--   0        0        0     5610 2024-05-17 21:59:53.718191 pyprland-2.3.0/pyprland/plugins/wallpapers.py
+-rw-r--r--   0        0        0     2496 2024-05-16 19:55:44.465502 pyprland-2.3.0/pyprland/plugins/workspaces_follow_focus.py
+-rw-r--r--   0        0        0     1459 2024-05-17 22:24:00.284438 pyprland-2.3.0/pyprland/types.py
+-rw-r--r--   0        0        0       42 2024-05-18 15:39:48.487505 pyprland-2.3.0/pyprland/version.py
+-rw-r--r--   0        0        0     2124 2024-05-18 15:39:48.484172 pyprland-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5966 1970-01-01 00:00:00.000000 pyprland-2.3.0/PKG-INFO
```

### Comparing `pyprland-2.2.9/LICENSE` & `pyprland-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.9/README.md` & `pyprland-2.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -13,267 +13,328 @@
 000000c0: 636f 6d2f 6879 7072 776d 2f48 7970 726c  com/hyprwm/Hyprl
 000000d0: 616e 6429 0a5b 215b 4469 7363 6f72 645d  and).[![Discord]
 000000e0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
 000000f0: 656c 6473 2e69 6f2f 6469 7363 6f72 642f  elds.io/discord/
 00000100: 3130 3535 3939 3032 3134 3431 3131 3639  1055990214411169
 00000110: 3839 323f 6c61 6265 6c3d 6469 7363 6f72  892?label=discor
 00000120: 6429 5d28 6874 7470 733a 2f2f 6469 7363  d)](https://disc
-00000130: 6f72 642e 6767 2f7a 7a57 7176 634b 524d  ord.gg/zzWqvcKRM
-00000140: 7929 0a0a 5b44 6f63 756d 656e 7461 7469  y)..[Documentati
-00000150: 6f6e 5d28 6874 7470 733a 2f2f 6769 7468  on](https://gith
-00000160: 7562 2e63 6f6d 2f68 7970 726c 616e 642d  ub.com/hyprland-
-00000170: 636f 6d6d 756e 6974 792f 7079 7072 6c61  community/pyprla
-00000180: 6e64 2f77 696b 6929 20e2 80a2 205b 4469  nd/wiki) ... [Di
-00000190: 7363 7573 7369 6f6e 735d 2868 7474 7073  scussions](https
-000001a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6879  ://github.com/hy
-000001b0: 7072 6c61 6e64 2d63 6f6d 6d75 6e69 7479  prland-community
-000001c0: 2f70 7970 726c 616e 642f 6469 7363 7573  /pyprland/discus
-000001d0: 7369 6f6e 7329 20e2 80a2 205b 4368 616e  sions) ... [Chan
-000001e0: 6765 7320 4869 7374 6f72 795d 2868 7474  ges History](htt
-000001f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000200: 6879 7072 6c61 6e64 2d63 6f6d 6d75 6e69  hyprland-communi
-00000210: 7479 2f70 7970 726c 616e 642f 7265 6c65  ty/pyprland/rele
-00000220: 6173 6573 2920 e280 a220 5b53 6861 7265  ases) ... [Share
-00000230: 2059 6f75 7220 5365 7475 705d 2868 7474   Your Setup](htt
-00000240: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000250: 6879 7072 6c61 6e64 2d63 6f6d 6d75 6e69  hyprland-communi
-00000260: 7479 2f70 7970 726c 616e 642f 6469 7363  ty/pyprland/disc
-00000270: 7573 7369 6f6e 732f 3436 290a 0a0a 2323  ussions/46)...##
-00000280: 2045 6e68 616e 6365 2079 6f75 7220 4879   Enhance your Hy
-00000290: 7072 6c61 6e64 2065 7870 6572 6965 6e63  prland experienc
-000002a0: 6520 7769 7468 2050 7970 726c 616e 640a  e with Pyprland.
-000002b0: 0a57 656c 636f 6d65 2074 6f20 5079 7072  .Welcome to Pypr
-000002c0: 6c61 6e64 2c20 796f 7572 2067 6174 6577  land, your gatew
-000002d0: 6179 2074 6f20 6578 7465 6e64 696e 6720  ay to extending 
-000002e0: 7468 6520 6361 7061 6269 6c69 7469 6573  the capabilities
-000002f0: 206f 6620 5b48 7970 726c 616e 645d 2868   of [Hyprland](h
-00000300: 7474 7073 3a2f 2f68 7970 726c 616e 642e  ttps://hyprland.
-00000310: 6f72 672f 292e 2050 7970 726c 616e 6420  org/). Pyprland 
-00000320: 6f66 6665 7273 2061 2070 6c65 7468 6f72  offers a plethor
-00000330: 6120 6f66 2070 6c75 6769 6e73 2064 6573  a of plugins des
-00000340: 6967 6e65 6420 666f 7220 7369 6d70 6c69  igned for simpli
-00000350: 6369 7479 2061 6e64 2065 6666 6963 6965  city and efficie
-00000360: 6e63 792c 2061 6c6c 6f77 696e 6720 796f  ncy, allowing yo
-00000370: 7520 746f 2073 7570 6572 6368 6172 6765  u to supercharge
-00000380: 2079 6f75 7220 7072 6f64 7563 7469 7669   your productivi
-00000390: 7479 2061 6e64 2063 7573 746f 6d69 7a65  ty and customize
-000003a0: 2079 6f75 7220 7573 6572 2065 7870 6572   your user exper
-000003b0: 6965 6e63 652e 0a0a 2d20 4578 706c 6f72  ience...- Explor
-000003c0: 6520 6f75 7220 7661 7269 6574 7920 6f66  e our variety of
-000003d0: 205b 706c 7567 696e 735d 2868 7474 7073   [plugins](https
-000003e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6879  ://github.com/hy
-000003f0: 7072 6c61 6e64 2d63 6f6d 6d75 6e69 7479  prland-community
-00000400: 2f70 7970 726c 616e 642f 7769 6b69 2f50  /pyprland/wiki/P
-00000410: 6c75 6769 6e73 2920 746f 2074 6169 6c6f  lugins) to tailo
-00000420: 7220 796f 7572 2048 7970 726c 616e 6420  r your Hyprland 
-00000430: 7365 7475 7020 746f 2079 6f75 7220 6c69  setup to your li
-00000440: 6b69 6e67 2e0a 2d20 4e65 7720 7573 6572  king..- New user
-00000450: 732c 2063 6865 636b 2074 6865 205b 6765  s, check the [ge
-00000460: 7474 696e 6720 7374 6172 7465 645d 2868  tting started](h
-00000470: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000480: 6d2f 6879 7072 6c61 6e64 2d63 6f6d 6d75  m/hyprland-commu
-00000490: 6e69 7479 2f70 7970 726c 616e 642f 7769  nity/pyprland/wi
-000004a0: 6b69 2f47 6574 7469 6e67 2d73 7461 7274  ki/Getting-start
-000004b0: 6564 2920 6775 6964 652e 0a0a 0a23 2320  ed) guide....## 
-000004c0: 4162 6f75 7420 5079 7072 6c61 6e64 0a0a  About Pyprland..
-000004d0: 5b21 5b50 6163 6b61 6769 6e67 2053 7461  [![Packaging Sta
-000004e0: 7475 735d 2868 7474 7073 3a2f 2f72 6570  tus](https://rep
-000004f0: 6f6c 6f67 792e 6f72 672f 6261 6467 652f  ology.org/badge/
-00000500: 7665 7274 6963 616c 2d61 6c6c 7265 706f  vertical-allrepo
-00000510: 732f 7079 7072 6c61 6e64 2e73 7667 295d  s/pyprland.svg)]
-00000520: 2868 7474 7073 3a2f 2f72 6570 6f6c 6f67  (https://repolog
-00000530: 792e 6f72 672f 7072 6f6a 6563 742f 7079  y.org/project/py
-00000540: 7072 6c61 6e64 2f76 6572 7369 6f6e 7329  prland/versions)
-00000550: 0a0a f09f 8e89 2048 6561 7220 7768 6174  ...... Hear what
-00000560: 206f 7468 6572 7320 6172 6520 7361 7969   others are sayi
-00000570: 6e67 3a0a 2d20 5b22 4974 206a 7573 7420  ng:.- ["It just 
-00000580: 776f 726b 7320 7665 7279 2076 6572 7920  works very very 
-00000590: 7765 6c6c 2220 2d20 5468 6520 4c69 6e75  well" - The Linu
-000005a0: 7820 4361 7374 2028 7669 6465 6f29 5d28  x Cast (video)](
-000005b0: 6874 7470 733a 2f2f 796f 7574 752e 6265  https://youtu.be
-000005c0: 2f43 6a6e 3053 4679 7975 6359 3f73 693d  /Cjn0SFyyucY?si=
-000005d0: 6847 6230 544d 3949 4476 6c62 6344 3641  hGb0TM9IDvlbcD6A
-000005e0: 2674 3d31 3331 2920 2d20 4665 6272 7561  &t=131) - Februa
-000005f0: 7279 2032 3032 340a 2d20 5b59 6f75 204e  ry 2024.- [You N
-00000600: 4545 4420 5468 6973 2069 6e20 796f 7572  EED This in your
-00000610: 2048 7970 726c 616e 6420 436f 6e66 6967   Hyprland Config
-00000620: 202d 204c 6962 7265 5068 6f65 6e69 7820   - LibrePhoenix 
-00000630: 2876 6964 656f 295d 2868 7474 7073 3a2f  (video)](https:/
-00000640: 2f77 7777 2e79 6f75 7475 6265 2e63 6f6d  /www.youtube.com
-00000650: 2f77 6174 6368 3f76 3d43 7747 6c6d 2d72  /watch?v=CwGlm-r
-00000660: 706f 6b34 2920 2d20 4f63 746f 6265 7220  pok4) - October 
-00000670: 3230 3233 2028 2a4e 6f77 205b 544f 4d4c  2023 (*Now [TOML
-00000680: 5d28 6874 7470 733a 2f2f 746f 6d6c 2e69  ](https://toml.i
-00000690: 6f2f 656e 2f29 2066 6f72 6d61 7420 6973  o/en/) format is
-000006a0: 2070 7265 6665 7272 6564 206f 7665 7220   preferred over 
-000006b0: 5b4a 534f 4e5d 2868 7474 7073 3a2f 2f77  [JSON](https://w
-000006c0: 7777 2e77 3373 6368 6f6f 6c73 2e63 6f6d  ww.w3schools.com
-000006d0: 2f6a 732f 6a73 5f6a 736f 6e5f 696e 7472  /js/js_json_intr
-000006e0: 6f2e 6173 7029 290a 0a23 2320 436f 6e74  o.asp))..## Cont
-000006f0: 7269 6275 7469 6e67 0a0a 4368 6563 6b20  ributing..Check 
-00000700: 6f75 7420 7468 6520 5b63 7265 6174 696e  out the [creatin
-00000710: 6720 6120 7075 6c6c 2072 6571 7565 7374  g a pull request
-00000720: 5d28 6874 7470 733a 2f2f 646f 6373 2e67  ](https://docs.g
-00000730: 6974 6875 622e 636f 6d2f 6672 2f70 756c  ithub.com/fr/pul
-00000740: 6c2d 7265 7175 6573 7473 2f63 6f6c 6c61  l-requests/colla
-00000750: 626f 7261 7469 6e67 2d77 6974 682d 7075  borating-with-pu
-00000760: 6c6c 2d72 6571 7565 7374 732f 7072 6f70  ll-requests/prop
-00000770: 6f73 696e 672d 6368 616e 6765 732d 746f  osing-changes-to
-00000780: 2d79 6f75 722d 776f 726b 2d77 6974 682d  -your-work-with-
-00000790: 7075 6c6c 2d72 6571 7565 7374 732f 6372  pull-requests/cr
-000007a0: 6561 7469 6e67 2d61 2d70 756c 6c2d 7265  eating-a-pull-re
-000007b0: 7175 6573 7429 2064 6f63 756d 656e 7420  quest) document 
-000007c0: 666f 7220 6775 6964 616e 6365 2e0a 0a2d  for guidance...-
-000007d0: 2052 6570 6f72 7420 6275 6773 206f 7220   Report bugs or 
-000007e0: 7072 6f70 6f73 6520 6665 6174 7572 6573  propose features
-000007f0: 205b 6865 7265 5d28 6874 7470 733a 2f2f   [here](https://
-00000800: 6769 7468 7562 2e63 6f6d 2f68 7970 726c  github.com/hyprl
-00000810: 616e 642d 636f 6d6d 756e 6974 792f 7079  and-community/py
-00000820: 7072 6c61 6e64 2f69 7373 7565 7329 0a2d  prland/issues).-
-00000830: 2049 6d70 726f 7665 206f 7572 205b 7769   Improve our [wi
-00000840: 6b69 5d28 6874 7470 733a 2f2f 6769 7468  ki](https://gith
-00000850: 7562 2e63 6f6d 2f68 7970 726c 616e 642d  ub.com/hyprland-
-00000860: 636f 6d6d 756e 6974 792f 7079 7072 6c61  community/pyprla
-00000870: 6e64 2f77 696b 6929 0a0a 616e 6420 6966  nd/wiki)..and if
-00000880: 2079 6f75 2068 6176 6520 636f 6469 6e67   you have coding
-00000890: 2073 6b69 6c6c 7320 796f 7520 6361 6e20   skills you can 
-000008a0: 616c 736f 0a0a 2d20 456e 6861 6e63 6520  also..- Enhance 
-000008b0: 7468 6520 636f 7665 7261 6765 206f 6620  the coverage of 
-000008c0: 6f75 7220 5b74 6573 7473 5d28 6874 7470  our [tests](http
-000008d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
-000008e0: 7970 726c 616e 642d 636f 6d6d 756e 6974  yprland-communit
-000008f0: 792f 7079 7072 6c61 6e64 2f74 7265 652f  y/pyprland/tree/
-00000900: 6d61 696e 2f74 6573 7473 290a 2d20 5072  main/tests).- Pr
-00000910: 6f70 6f73 6520 2620 7772 6974 6520 6e65  opose & write ne
-00000920: 7720 706c 7567 696e 7320 6f72 2065 6e68  w plugins or enh
-00000930: 616e 6365 6d65 6e74 730a 0a23 2320 4465  ancements..## De
-00000940: 7065 6e64 656e 6369 6573 0a0a 2d20 2a2a  pendencies..- **
-00000950: 4879 7072 6c61 6e64 2a2a 203e 3d20 302e  Hyprland** >= 0.
-00000960: 3337 0a2d 202a 2a50 7974 686f 6e2a 2a20  37.- **Python** 
-00000970: 3e3d 2033 2e31 310a 2020 2020 2d20 2a2a  >= 3.11.    - **
-00000980: 6169 6f66 696c 6573 2a2a 0a0a 2323 204c  aiofiles**..## L
-00000990: 6174 6573 7420 6d61 6a6f 7220 6368 616e  atest major chan
-000009a0: 6765 730a 0a3e 205b 216e 6f74 655d 0a3e  ges..> [!note].>
-000009b0: 2043 6865 636b 2074 6865 205b 5265 6c65   Check the [Rele
-000009c0: 6173 6573 2063 6861 6e67 6520 6c6f 675d  ases change log]
-000009d0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000009e0: 636f 6d2f 6879 7072 6c61 6e64 2d63 6f6d  com/hyprland-com
-000009f0: 6d75 6e69 7479 2f70 7970 726c 616e 642f  munity/pyprland/
-00000a00: 7265 6c65 6173 6573 2920 666f 7220 6d6f  releases) for mo
-00000a10: 7265 2069 6e66 6f72 6d61 7469 6f6e 0a0a  re information..
-00000a20: 2323 2320 322e 320a 0a2d 2041 6464 6564  ### 2.2..- Added
-00000a30: 205b 7761 6c6c 7061 7065 7273 5d28 6874   [wallpapers](ht
-00000a40: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000a50: 2f68 7970 726c 616e 642d 636f 6d6d 756e  /hyprland-commun
-00000a60: 6974 792f 7079 7072 6c61 6e64 2f77 696b  ity/pyprland/wik
-00000a70: 692f 7761 6c6c 7061 7065 7273 2920 616e  i/wallpapers) an
-00000a80: 6420 5b73 7973 7465 6d5f 6e6f 7469 6669  d [system_notifi
-00000a90: 6572 5d28 6874 7470 733a 2f2f 6769 7468  er](https://gith
-00000aa0: 7562 2e63 6f6d 2f68 7970 726c 616e 642d  ub.com/hyprland-
-00000ab0: 636f 6d6d 756e 6974 792f 7079 7072 6c61  community/pyprla
-00000ac0: 6e64 2f77 696b 692f 7379 7374 656d 5f6e  nd/wiki/system_n
-00000ad0: 6f74 6966 6965 7229 2070 6c75 6769 6e73  otifier) plugins
-00000ae0: 2e0a 2d20 5265 6661 6374 6f72 2069 6e20  ..- Refactor in 
-00000af0: 322e 322e 350a 2020 2d20 7570 6461 7465  2.2.5.  - update
-00000b00: 6420 7468 6520 7379 6e74 6178 2066 6f72  d the syntax for
-00000b10: 205b 7761 6c6c 7061 7065 7273 5d28 6874   [wallpapers](ht
-00000b20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000b30: 2f68 7970 726c 616e 642d 636f 6d6d 756e  /hyprland-commun
-00000b40: 6974 792f 7079 7072 6c61 6e64 2f77 696b  ity/pyprland/wik
-00000b50: 692f 7761 6c6c 7061 7065 7273 290a 2020  i/wallpapers).  
-00000b60: 2d20 6465 7072 6563 6174 6564 2060 636c  - deprecated `cl
-00000b70: 6173 735f 6d61 7463 6860 2069 6e20 5b73  ass_match` in [s
-00000b80: 6372 6174 6368 7061 6473 5d28 6874 7470  cratchpads](http
-00000b90: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
-00000ba0: 7970 726c 616e 642d 636f 6d6d 756e 6974  yprland-communit
-00000bb0: 792f 7079 7072 6c61 6e64 2f77 696b 692f  y/pyprland/wiki/
-00000bc0: 7363 7261 7463 6870 6164 7329 0a2d 2041  scratchpads).- A
-00000bd0: 6464 6564 205b 6762 6172 5d28 6874 7470  dded [gbar](http
-00000be0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
-00000bf0: 7970 726c 616e 642d 636f 6d6d 756e 6974  yprland-communit
-00000c00: 792f 7079 7072 6c61 6e64 2f77 696b 692f  y/pyprland/wiki/
-00000c10: 6762 6172 2920 696e 2032 2e32 2e36 0a23  gbar) in 2.2.6.#
-00000c20: 2323 2032 2e31 0a0a 2d20 5265 7175 6972  ## 2.1..- Requir
-00000c30: 6573 2048 7970 726c 616e 6420 3e3d 2030  es Hyprland >= 0
-00000c40: 2e33 370a 2d20 5b4d 6f6e 6974 6f72 735d  .37.- [Monitors]
-00000c50: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000c60: 636f 6d2f 6879 7072 6c61 6e64 2d63 6f6d  com/hyprland-com
-00000c70: 6d75 6e69 7479 2f70 7970 726c 616e 642f  munity/pyprland/
-00000c80: 7769 6b69 2f6d 6f6e 6974 6f72 7329 2070  wiki/monitors) p
-00000c90: 6c75 6769 6e20 696d 7072 6f76 656d 656e  lugin improvemen
-00000ca0: 7473 2e0a 0a23 2323 2032 2e30 0a0a 2d20  ts...### 2.0..- 
-00000cb0: 4e65 7720 6465 7065 6e64 656e 6379 3a20  New dependency: 
-00000cc0: 5b61 696f 6669 6c65 735d 2868 7474 7073  [aiofiles](https
-00000cd0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-00000ce0: 6563 742f 6169 6f66 696c 6573 2f29 0a2d  ect/aiofiles/).-
-00000cf0: 2041 6464 6564 205b 6879 7374 6572 6573   Added [hysteres
-00000d00: 6973 5d28 6874 7470 733a 2f2f 6769 7468  is](https://gith
-00000d10: 7562 2e63 6f6d 2f68 7970 726c 616e 642d  ub.com/hyprland-
-00000d20: 636f 6d6d 756e 6974 792f 7079 7072 6c61  community/pyprla
-00000d30: 6e64 2f77 696b 692f 7363 7261 7463 6870  nd/wiki/scratchp
-00000d40: 6164 7323 6879 7374 6572 6573 6973 2d6f  ads#hysteresis-o
-00000d50: 7074 696f 6e61 6c29 2073 7570 706f 7274  ptional) support
-00000d60: 2066 6f72 205b 7363 7261 7463 6870 6164   for [scratchpad
-00000d70: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
-00000d80: 622e 636f 6d2f 6879 7072 6c61 6e64 2d63  b.com/hyprland-c
-00000d90: 6f6d 6d75 6e69 7479 2f70 7970 726c 616e  ommunity/pyprlan
-00000da0: 642f 7769 6b69 2f73 6372 6174 6368 7061  d/wiki/scratchpa
-00000db0: 6473 292e 0a0a 2323 2320 312e 3130 0a0a  ds)...### 1.10..
-00000dc0: 2d20 4e65 7720 5b66 6574 6368 5f63 6c69  - New [fetch_cli
-00000dd0: 656e 745f 6d65 6e75 5d28 6874 7470 733a  ent_menu](https:
-00000de0: 2f2f 6769 7468 7562 2e63 6f6d 2f68 7970  //github.com/hyp
-00000df0: 726c 616e 642d 636f 6d6d 756e 6974 792f  rland-community/
-00000e00: 7079 7072 6c61 6e64 2f77 696b 692f 6665  pyprland/wiki/fe
-00000e10: 7463 685f 636c 6965 6e74 5f6d 656e 7529  tch_client_menu)
-00000e20: 2061 6e64 205b 7368 6f72 7463 7574 735f   and [shortcuts_
-00000e30: 6d65 6e75 5d28 6874 7470 733a 2f2f 6769  menu](https://gi
-00000e40: 7468 7562 2e63 6f6d 2f68 7970 726c 616e  thub.com/hyprlan
-00000e50: 642d 636f 6d6d 756e 6974 792f 7079 7072  d-community/pypr
-00000e60: 6c61 6e64 2f77 696b 692f 7368 6f72 7463  land/wiki/shortc
-00000e70: 7574 735f 6d65 6e75 2920 706c 7567 696e  uts_menu) plugin
-00000e80: 732e 0a0a 2323 2320 312e 390a 0a2d 2049  s...### 1.9..- I
-00000e90: 6e74 726f 6475 6365 6420 5b73 686f 7274  ntroduced [short
-00000ea0: 6375 7473 5f6d 656e 755d 2868 7474 7073  cuts_menu](https
-00000eb0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6879  ://github.com/hy
-00000ec0: 7072 6c61 6e64 2d63 6f6d 6d75 6e69 7479  prland-community
-00000ed0: 2f70 7970 726c 616e 642f 7769 6b69 2f73  /pyprland/wiki/s
-00000ee0: 686f 7274 6375 7473 5f6d 656e 7529 2070  hortcuts_menu) p
-00000ef0: 6c75 6769 6e2e 0a0a 2323 2320 312e 380a  lugin...### 1.8.
-00000f00: 0a2d 2052 6571 7569 7265 7320 4879 7072  .- Requires Hypr
-00000f10: 6c61 6e64 203e 3d20 302e 3330 0a2d 2041  land >= 0.30.- A
-00000f20: 6464 6564 205b 6c61 796f 7574 5f63 656e  dded [layout_cen
-00000f30: 7465 725d 2868 7474 7073 3a2f 2f67 6974  ter](https://git
-00000f40: 6875 622e 636f 6d2f 6879 7072 6c61 6e64  hub.com/hyprland
-00000f50: 2d63 6f6d 6d75 6e69 7479 2f70 7970 726c  -community/pyprl
-00000f60: 616e 642f 7769 6b69 2f6c 6179 6f75 745f  and/wiki/layout_
-00000f70: 6365 6e74 6572 2920 706c 7567 696e 2e0a  center) plugin..
-00000f80: 0a23 2320 5374 6172 2048 6973 746f 7279  .## Star History
-00000f90: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
-00000fa0: 3a2f 2f73 7461 722d 6869 7374 6f72 792e  ://star-history.
-00000fb0: 636f 6d2f 2366 6465 7633 312f 7079 7072  com/#fdev31/pypr
-00000fc0: 6c61 6e64 2644 6174 6522 3e0a 2020 3c70  land&Date">.  <p
-00000fd0: 6963 7475 7265 3e0a 2020 2020 3c73 6f75  icture>.    <sou
-00000fe0: 7263 6520 6d65 6469 613d 2228 7072 6566  rce media="(pref
-00000ff0: 6572 732d 636f 6c6f 722d 7363 6865 6d65  ers-color-scheme
-00001000: 3a20 6461 726b 2922 2073 7263 7365 743d  : dark)" srcset=
-00001010: 2268 7474 7073 3a2f 2f61 7069 2e73 7461  "https://api.sta
-00001020: 722d 6869 7374 6f72 792e 636f 6d2f 7376  r-history.com/sv
-00001030: 673f 7265 706f 733d 6664 6576 3331 2f70  g?repos=fdev31/p
-00001040: 7970 726c 616e 6426 7479 7065 3d54 696d  yprland&type=Tim
-00001050: 656c 696e 6526 7468 656d 653d 6461 726b  eline&theme=dark
-00001060: 2220 2f3e 0a20 2020 203c 736f 7572 6365  " />.    <source
-00001070: 206d 6564 6961 3d22 2870 7265 6665 7273   media="(prefers
-00001080: 2d63 6f6c 6f72 2d73 6368 656d 653a 206c  -color-scheme: l
-00001090: 6967 6874 2922 2073 7263 7365 743d 2268  ight)" srcset="h
-000010a0: 7474 7073 3a2f 2f61 7069 2e73 7461 722d  ttps://api.star-
-000010b0: 6869 7374 6f72 792e 636f 6d2f 7376 673f  history.com/svg?
-000010c0: 7265 706f 733d 6664 6576 3331 2f70 7970  repos=fdev31/pyp
-000010d0: 726c 616e 6426 7479 7065 3d54 696d 656c  rland&type=Timel
-000010e0: 696e 6522 202f 3e0a 2020 2020 3c69 6d67  ine" />.    <img
-000010f0: 2061 6c74 3d22 5374 6172 2048 6973 746f   alt="Star Histo
-00001100: 7279 2043 6861 7274 2220 7372 633d 2268  ry Chart" src="h
-00001110: 7474 7073 3a2f 2f61 7069 2e73 7461 722d  ttps://api.star-
-00001120: 6869 7374 6f72 792e 636f 6d2f 7376 673f  history.com/svg?
-00001130: 7265 706f 733d 6664 6576 3331 2f70 7970  repos=fdev31/pyp
-00001140: 726c 616e 6426 7479 7065 3d54 696d 656c  rland&type=Timel
-00001150: 696e 6522 202f 3e0a 2020 3c2f 7069 6374  ine" />.  </pict
-00001160: 7572 653e 0a3c 2f61 3e0a                 ure>.</a>.
+00000130: 6f72 642e 636f 6d2f 6368 616e 6e65 6c73  ord.com/channels
+00000140: 2f31 3035 3539 3930 3231 3434 3131 3136  /105599021441116
+00000150: 3938 3932 2f31 3233 3039 3732 3135 3433  9892/12309721543
+00000160: 3330 3231 3835 3236 290a 0a5b 446f 6375  30218526)..[Docu
+00000170: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
+00000180: 3a2f 2f67 6974 6875 622e 636f 6d2f 6879  ://github.com/hy
+00000190: 7072 6c61 6e64 2d63 6f6d 6d75 6e69 7479  prland-community
+000001a0: 2f70 7970 726c 616e 642f 7769 6b69 2920  /pyprland/wiki) 
+000001b0: e280 a220 5b44 6973 6375 7373 696f 6e73  ... [Discussions
+000001c0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000001d0: 2e63 6f6d 2f68 7970 726c 616e 642d 636f  .com/hyprland-co
+000001e0: 6d6d 756e 6974 792f 7079 7072 6c61 6e64  mmunity/pyprland
+000001f0: 2f64 6973 6375 7373 696f 6e73 2920 e280  /discussions) ..
+00000200: a220 5b43 6861 6e67 6573 2048 6973 746f  . [Changes Histo
+00000210: 7279 5d28 6874 7470 733a 2f2f 6769 7468  ry](https://gith
+00000220: 7562 2e63 6f6d 2f68 7970 726c 616e 642d  ub.com/hyprland-
+00000230: 636f 6d6d 756e 6974 792f 7079 7072 6c61  community/pyprla
+00000240: 6e64 2f72 656c 6561 7365 7329 20e2 80a2  nd/releases) ...
+00000250: 205b 5368 6172 6520 596f 7572 2053 6574   [Share Your Set
+00000260: 7570 5d28 6874 7470 733a 2f2f 6769 7468  up](https://gith
+00000270: 7562 2e63 6f6d 2f68 7970 726c 616e 642d  ub.com/hyprland-
+00000280: 636f 6d6d 756e 6974 792f 7079 7072 6c61  community/pyprla
+00000290: 6e64 2f64 6973 6375 7373 696f 6e73 2f34  nd/discussions/4
+000002a0: 3629 0a0a 0a23 2320 456e 6861 6e63 6520  6)...## Enhance 
+000002b0: 796f 7572 2048 7970 726c 616e 6420 6578  your Hyprland ex
+000002c0: 7065 7269 656e 6365 2077 6974 6820 5079  perience with Py
+000002d0: 7072 6c61 6e64 0a0a 5765 6c63 6f6d 6520  prland..Welcome 
+000002e0: 746f 2050 7970 726c 616e 642c 2079 6f75  to Pyprland, you
+000002f0: 7220 6761 7465 7761 7920 746f 2065 7874  r gateway to ext
+00000300: 656e 6469 6e67 2074 6865 2063 6170 6162  ending the capab
+00000310: 696c 6974 6965 7320 6f66 205b 4879 7072  ilities of [Hypr
+00000320: 6c61 6e64 5d28 6874 7470 733a 2f2f 6879  land](https://hy
+00000330: 7072 6c61 6e64 2e6f 7267 2f29 2e20 5079  prland.org/). Py
+00000340: 7072 6c61 6e64 206f 6666 6572 7320 6120  prland offers a 
+00000350: 706c 6574 686f 7261 206f 6620 706c 7567  plethora of plug
+00000360: 696e 7320 6465 7369 676e 6564 2066 6f72  ins designed for
+00000370: 2073 696d 706c 6963 6974 7920 616e 6420   simplicity and 
+00000380: 6566 6669 6369 656e 6379 2c20 616c 6c6f  efficiency, allo
+00000390: 7769 6e67 2079 6f75 2074 6f20 7375 7065  wing you to supe
+000003a0: 7263 6861 7267 6520 796f 7572 2070 726f  rcharge your pro
+000003b0: 6475 6374 6976 6974 7920 616e 6420 6375  ductivity and cu
+000003c0: 7374 6f6d 697a 6520 796f 7572 2075 7365  stomize your use
+000003d0: 7220 6578 7065 7269 656e 6365 2e0a 0a59  r experience...Y
+000003e0: 6f75 2063 616e 2074 6869 6e6b 206f 6620  ou can think of 
+000003f0: 6974 2061 7320 6120 2a47 6e6f 6d65 2074  it as a *Gnome t
+00000400: 7765 616b 2074 6f6f 6c2a 2062 7574 2066  weak tool* but f
+00000410: 6f72 2048 7970 726c 616e 6420 7573 6572  or Hyprland user
+00000420: 7320 2869 6e76 6f6c 7665 7320 6564 6974  s (involves edit
+00000430: 696e 6720 7465 7874 2066 696c 6573 292e  ing text files).
+00000440: 2057 6974 6820 6120 2231 3030 2522 2070   With a "100%" p
+00000450: 6c75 6769 6e2d 6261 7365 6420 6172 6368  lugin-based arch
+00000460: 6974 6563 7475 7265 2c20 5079 7072 6c61  itecture, Pyprla
+00000470: 6e64 2069 7320 6465 7369 676e 6564 2074  nd is designed t
+00000480: 6f20 6265 206c 6967 6874 7765 6967 6874  o be lightweight
+00000490: 2061 6e64 2065 6173 7920 746f 2075 7365   and easy to use
+000004a0: 2e0a 0a4e 6f74 6520 7468 6174 2075 7361  ...Note that usa
+000004b0: 6765 206f 6620 5079 7468 6f6e 2061 6e64  ge of Python and
+000004c0: 2061 7263 6869 7465 6374 7572 6520 6f66   architecture of
+000004d0: 2074 6865 2073 6f66 7477 6172 6520 656e   the software en
+000004e0: 636f 7572 6167 6573 2075 7369 6e67 206d  courages using m
+000004f0: 616e 7920 706c 7567 696e 7320 7769 7468  any plugins with
+00000500: 206c 6974 746c 6520 696d 7061 6374 206f   little impact o
+00000510: 6e20 7468 6520 666f 6f74 7072 696e 7420  n the footprint 
+00000520: 616e 6420 7065 7266 6f72 6d61 6e63 652e  and performance.
+00000530: 0a0a 436f 6e74 7269 6275 7469 6f6e 732c  ..Contributions,
+00000540: 2073 7567 6765 7374 696f 6e73 2c20 6275   suggestions, bu
+00000550: 6720 7265 706f 7274 7320 616e 6420 636f  g reports and co
+00000560: 6d6d 656e 7473 2061 7265 2077 656c 636f  mments are welco
+00000570: 6d65 2e0a 0a2d 2045 7870 6c6f 7265 206f  me...- Explore o
+00000580: 7572 2076 6172 6965 7479 206f 6620 5b70  ur variety of [p
+00000590: 6c75 6769 6e73 5d28 6874 7470 733a 2f2f  lugins](https://
+000005a0: 6769 7468 7562 2e63 6f6d 2f68 7970 726c  github.com/hyprl
+000005b0: 616e 642d 636f 6d6d 756e 6974 792f 7079  and-community/py
+000005c0: 7072 6c61 6e64 2f77 696b 692f 506c 7567  prland/wiki/Plug
+000005d0: 696e 7329 2074 6f20 7461 696c 6f72 2079  ins) to tailor y
+000005e0: 6f75 7220 4879 7072 6c61 6e64 2073 6574  our Hyprland set
+000005f0: 7570 2074 6f20 796f 7572 206c 696b 696e  up to your likin
+00000600: 672e 0a2d 204e 6577 2075 7365 7273 2c20  g..- New users, 
+00000610: 6368 6563 6b20 7468 6520 5b67 6574 7469  check the [getti
+00000620: 6e67 2073 7461 7274 6564 5d28 6874 7470  ng started](http
+00000630: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
+00000640: 7970 726c 616e 642d 636f 6d6d 756e 6974  yprland-communit
+00000650: 792f 7079 7072 6c61 6e64 2f77 696b 692f  y/pyprland/wiki/
+00000660: 4765 7474 696e 672d 7374 6172 7465 6429  Getting-started)
+00000670: 2067 7569 6465 2e0a 0a0a 3c64 6574 6169   guide....<detai
+00000680: 6c73 3e0a 3c73 756d 6d61 7279 3e0a 4162  ls>.<summary>.Ab
+00000690: 6f75 7420 5079 7072 6c61 6e64 0a3c 2f73  out Pyprland.</s
+000006a0: 756d 6d61 7279 3e0a 0a4c 6174 6573 7420  ummary>..Latest 
+000006b0: 7374 6162 6c65 2069 733a 202a 2a32 2e32  stable is: **2.2
+000006c0: 2e32 302a 2a0a 0a5b 215b 5061 636b 6167  .20**..[![Packag
+000006d0: 696e 6720 5374 6174 7573 5d28 6874 7470  ing Status](http
+000006e0: 733a 2f2f 7265 706f 6c6f 6779 2e6f 7267  s://repology.org
+000006f0: 2f62 6164 6765 2f76 6572 7469 6361 6c2d  /badge/vertical-
+00000700: 616c 6c72 6570 6f73 2f70 7970 726c 616e  allrepos/pyprlan
+00000710: 642e 7376 6729 5d28 6874 7470 733a 2f2f  d.svg)](https://
+00000720: 7265 706f 6c6f 6779 2e6f 7267 2f70 726f  repology.org/pro
+00000730: 6a65 6374 2f70 7970 726c 616e 642f 7665  ject/pyprland/ve
+00000740: 7273 696f 6e73 290a 0af0 9f8e 8920 4865  rsions)...... He
+00000750: 6172 2077 6861 7420 6f74 6865 7273 2061  ar what others a
+00000760: 7265 2073 6179 696e 673a 0a2d 205b 2249  re saying:.- ["I
+00000770: 7420 6a75 7374 2077 6f72 6b73 2076 6572  t just works ver
+00000780: 7920 7665 7279 2077 656c 6c22 202d 2054  y very well" - T
+00000790: 6865 204c 696e 7578 2043 6173 7420 2876  he Linux Cast (v
+000007a0: 6964 656f 295d 2868 7474 7073 3a2f 2f79  ideo)](https://y
+000007b0: 6f75 7475 2e62 652f 436a 6e30 5346 7979  outu.be/Cjn0SFyy
+000007c0: 7563 593f 7369 3d68 4762 3054 4d39 4944  ucY?si=hGb0TM9ID
+000007d0: 766c 6263 4436 4126 743d 3133 3129 202d  vlbcD6A&t=131) -
+000007e0: 2046 6562 7275 6172 7920 3230 3234 0a2d   February 2024.-
+000007f0: 205b 596f 7520 4e45 4544 2054 6869 7320   [You NEED This 
+00000800: 696e 2079 6f75 7220 4879 7072 6c61 6e64  in your Hyprland
+00000810: 2043 6f6e 6669 6720 2d20 4c69 6272 6550   Config - LibreP
+00000820: 686f 656e 6978 2028 7669 6465 6f29 5d28  hoenix (video)](
+00000830: 6874 7470 733a 2f2f 7777 772e 796f 7574  https://www.yout
+00000840: 7562 652e 636f 6d2f 7761 7463 683f 763d  ube.com/watch?v=
+00000850: 4377 476c 6d2d 7270 6f6b 3429 202d 204f  CwGlm-rpok4) - O
+00000860: 6374 6f62 6572 2032 3032 3320 282a 4e6f  ctober 2023 (*No
+00000870: 7720 5b54 4f4d 4c5d 2868 7474 7073 3a2f  w [TOML](https:/
+00000880: 2f74 6f6d 6c2e 696f 2f65 6e2f 2920 666f  /toml.io/en/) fo
+00000890: 726d 6174 2069 7320 7072 6566 6572 7265  rmat is preferre
+000008a0: 6420 6f76 6572 205b 4a53 4f4e 5d28 6874  d over [JSON](ht
+000008b0: 7470 733a 2f2f 7777 772e 7733 7363 686f  tps://www.w3scho
+000008c0: 6f6c 732e 636f 6d2f 6a73 2f6a 735f 6a73  ols.com/js/js_js
+000008d0: 6f6e 5f69 6e74 726f 2e61 7370 2929 0a3c  on_intro.asp)).<
+000008e0: 2f64 6574 6169 6c73 3e0a 0a3c 6465 7461  /details>..<deta
+000008f0: 696c 733e 0a0a 3c73 756d 6d61 7279 3e0a  ils>..<summary>.
+00000900: 436f 6e74 7269 6275 7469 6e67 0a3c 2f73  Contributing.</s
+00000910: 756d 6d61 7279 3e0a 0a43 6865 636b 206f  ummary>..Check o
+00000920: 7574 2074 6865 205b 6372 6561 7469 6e67  ut the [creating
+00000930: 2061 2070 756c 6c20 7265 7175 6573 745d   a pull request]
+00000940: 2868 7474 7073 3a2f 2f64 6f63 732e 6769  (https://docs.gi
+00000950: 7468 7562 2e63 6f6d 2f66 722f 7075 6c6c  thub.com/fr/pull
+00000960: 2d72 6571 7565 7374 732f 636f 6c6c 6162  -requests/collab
+00000970: 6f72 6174 696e 672d 7769 7468 2d70 756c  orating-with-pul
+00000980: 6c2d 7265 7175 6573 7473 2f70 726f 706f  l-requests/propo
+00000990: 7369 6e67 2d63 6861 6e67 6573 2d74 6f2d  sing-changes-to-
+000009a0: 796f 7572 2d77 6f72 6b2d 7769 7468 2d70  your-work-with-p
+000009b0: 756c 6c2d 7265 7175 6573 7473 2f63 7265  ull-requests/cre
+000009c0: 6174 696e 672d 612d 7075 6c6c 2d72 6571  ating-a-pull-req
+000009d0: 7565 7374 2920 646f 6375 6d65 6e74 2066  uest) document f
+000009e0: 6f72 2067 7569 6461 6e63 652e 0a0a 2d20  or guidance...- 
+000009f0: 5265 706f 7274 2062 7567 7320 6f72 2070  Report bugs or p
+00000a00: 726f 706f 7365 2066 6561 7475 7265 7320  ropose features 
+00000a10: 5b68 6572 655d 2868 7474 7073 3a2f 2f67  [here](https://g
+00000a20: 6974 6875 622e 636f 6d2f 6879 7072 6c61  ithub.com/hyprla
+00000a30: 6e64 2d63 6f6d 6d75 6e69 7479 2f70 7970  nd-community/pyp
+00000a40: 726c 616e 642f 6973 7375 6573 290a 2d20  rland/issues).- 
+00000a50: 496d 7072 6f76 6520 6f75 7220 5b77 696b  Improve our [wik
+00000a60: 695d 2868 7474 7073 3a2f 2f67 6974 6875  i](https://githu
+00000a70: 622e 636f 6d2f 6879 7072 6c61 6e64 2d63  b.com/hyprland-c
+00000a80: 6f6d 6d75 6e69 7479 2f70 7970 726c 616e  ommunity/pyprlan
+00000a90: 642f 7769 6b69 290a 0a61 6e64 2069 6620  d/wiki)..and if 
+00000aa0: 796f 7520 6861 7665 2063 6f64 696e 6720  you have coding 
+00000ab0: 736b 696c 6c73 2079 6f75 2063 616e 2061  skills you can a
+00000ac0: 6c73 6f0a 0a2d 2045 6e68 616e 6365 2074  lso..- Enhance t
+00000ad0: 6865 2063 6f76 6572 6167 6520 6f66 206f  he coverage of o
+00000ae0: 7572 205b 7465 7374 735d 2868 7474 7073  ur [tests](https
+00000af0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6879  ://github.com/hy
+00000b00: 7072 6c61 6e64 2d63 6f6d 6d75 6e69 7479  prland-community
+00000b10: 2f70 7970 726c 616e 642f 7472 6565 2f6d  /pyprland/tree/m
+00000b20: 6169 6e2f 7465 7374 7329 0a2d 2050 726f  ain/tests).- Pro
+00000b30: 706f 7365 2026 2077 7269 7465 206e 6577  pose & write new
+00000b40: 2070 6c75 6769 6e73 206f 7220 656e 6861   plugins or enha
+00000b50: 6e63 656d 656e 7473 0a0a 3c2f 6465 7461  ncements..</deta
+00000b60: 696c 733e 0a0a 3c64 6574 6169 6c73 3e0a  ils>..<details>.
+00000b70: 3c73 756d 6d61 7279 3e0a 4465 7065 6e64  <summary>.Depend
+00000b80: 656e 6369 6573 0a3c 2f73 756d 6d61 7279  encies.</summary
+00000b90: 3e0a 0a2d 202a 2a48 7970 726c 616e 642a  >..- **Hyprland*
+00000ba0: 2a20 3e3d 2030 2e33 370a 2d20 2a2a 5079  * >= 0.37.- **Py
+00000bb0: 7468 6f6e 2a2a 203e 3d20 332e 3131 0a20  thon** >= 3.11. 
+00000bc0: 2020 202d 202a 2a61 696f 6669 6c65 732a     - **aiofiles*
+00000bd0: 2a0a 3c2f 6465 7461 696c 733e 0a0a 3c64  *.</details>..<d
+00000be0: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
+00000bf0: 3e0a 4c61 7465 7374 206d 616a 6f72 2063  >.Latest major c
+00000c00: 6861 6e67 6573 0a3c 2f73 756d 6d61 7279  hanges.</summary
+00000c10: 3e0a 0a43 6865 636b 2074 6865 205b 5265  >..Check the [Re
+00000c20: 6c65 6173 6573 2063 6861 6e67 6520 6c6f  leases change lo
+00000c30: 675d 2868 7474 7073 3a2f 2f67 6974 6875  g](https://githu
+00000c40: 622e 636f 6d2f 6879 7072 6c61 6e64 2d63  b.com/hyprland-c
+00000c50: 6f6d 6d75 6e69 7479 2f70 7970 726c 616e  ommunity/pyprlan
+00000c60: 642f 7265 6c65 6173 6573 2920 666f 7220  d/releases) for 
+00000c70: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+00000c80: 0a0a 2323 2320 322e 320a 0a2d 2041 6464  ..### 2.2..- Add
+00000c90: 6564 205b 7761 6c6c 7061 7065 7273 5d28  ed [wallpapers](
+00000ca0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000cb0: 6f6d 2f68 7970 726c 616e 642d 636f 6d6d  om/hyprland-comm
+00000cc0: 756e 6974 792f 7079 7072 6c61 6e64 2f77  unity/pyprland/w
+00000cd0: 696b 692f 7761 6c6c 7061 7065 7273 2920  iki/wallpapers) 
+00000ce0: 616e 6420 5b73 7973 7465 6d5f 6e6f 7469  and [system_noti
+00000cf0: 6669 6572 5d28 6874 7470 733a 2f2f 6769  fier](https://gi
+00000d00: 7468 7562 2e63 6f6d 2f68 7970 726c 616e  thub.com/hyprlan
+00000d10: 642d 636f 6d6d 756e 6974 792f 7079 7072  d-community/pypr
+00000d20: 6c61 6e64 2f77 696b 692f 7379 7374 656d  land/wiki/system
+00000d30: 5f6e 6f74 6966 6965 7229 2070 6c75 6769  _notifier) plugi
+00000d40: 6e73 2e0a 2d20 4465 7072 6563 6174 6564  ns..- Deprecated
+00000d50: 205b 636c 6173 735f 6d61 7463 685d 2868   [class_match](h
+00000d60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000d70: 6d2f 6879 7072 6c61 6e64 2d63 6f6d 6d75  m/hyprland-commu
+00000d80: 6e69 7479 2f70 7970 726c 616e 642f 7769  nity/pyprland/wi
+00000d90: 6b69 2f73 6372 6174 6368 7061 6473 5f6e  ki/scratchpads_n
+00000da0: 6f6e 7374 616e 6461 7264 2920 696e 205b  onstandard) in [
+00000db0: 7363 7261 7463 6870 6164 735d 2868 7474  scratchpads](htt
+00000dc0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000dd0: 6879 7072 6c61 6e64 2d63 6f6d 6d75 6e69  hyprland-communi
+00000de0: 7479 2f70 7970 726c 616e 642f 7769 6b69  ty/pyprland/wiki
+00000df0: 2f73 6372 6174 6368 7061 6473 290a 2d20  /scratchpads).- 
+00000e00: 4164 6465 6420 5b67 6261 725d 2868 7474  Added [gbar](htt
+00000e10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000e20: 6879 7072 6c61 6e64 2d63 6f6d 6d75 6e69  hyprland-communi
+00000e30: 7479 2f70 7970 726c 616e 642f 7769 6b69  ty/pyprland/wiki
+00000e40: 2f67 6261 7229 2069 6e20 322e 322e 360a  /gbar) in 2.2.6.
+00000e50: 2d20 5b73 6372 6174 6368 7061 6473 5d28  - [scratchpads](
+00000e60: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000e70: 6f6d 2f68 7970 726c 616e 642d 636f 6d6d  om/hyprland-comm
+00000e80: 756e 6974 792f 7079 7072 6c61 6e64 2f77  unity/pyprland/w
+00000e90: 696b 692f 7363 7261 7463 6870 6164 7329  iki/scratchpads)
+00000ea0: 2073 7570 706f 7274 7320 6d75 6c74 6970   supports multip
+00000eb0: 6c65 2063 6c69 656e 7420 7769 6e64 6f77  le client window
+00000ec0: 7320 2875 7369 6e67 2032 2e32 2e31 3920  s (using 2.2.19 
+00000ed0: 6973 2072 6563 6f6d 6d65 6e64 6564 290a  is recommended).
+00000ee0: 2d20 5b4d 6f6e 6974 6f72 735d 2868 7474  - [Monitors](htt
+00000ef0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000f00: 6879 7072 6c61 6e64 2d63 6f6d 6d75 6e69  hyprland-communi
+00000f10: 7479 2f70 7970 726c 616e 642f 7769 6b69  ty/pyprland/wiki
+00000f20: 2f6d 6f6e 6974 6f72 7329 2061 6e64 205b  /monitors) and [
+00000f30: 7363 7261 7463 6870 6164 735d 2868 7474  scratchpads](htt
+00000f40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000f50: 6879 7072 6c61 6e64 2d63 6f6d 6d75 6e69  hyprland-communi
+00000f60: 7479 2f70 7970 726c 616e 642f 7769 6b69  ty/pyprland/wiki
+00000f70: 2f73 6372 6174 6368 7061 6473 2920 7375  /scratchpads) su
+00000f80: 7070 6f72 7473 2072 6f74 6174 696f 6e20  pports rotation 
+00000f90: 696e 2032 2e32 2e31 330a 2d20 496d 7072  in 2.2.13.- Impr
+00000fa0: 6f76 6520 5b4e 6978 2073 7570 706f 7274  ove [Nix support
+00000fb0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000fc0: 2e63 6f6d 2f68 7970 726c 616e 642d 636f  .com/hyprland-co
+00000fd0: 6d6d 756e 6974 792f 7079 7072 6c61 6e64  mmunity/pyprland
+00000fe0: 2f77 696b 692f 4e69 7829 0a0a 0a23 2323  /wiki/Nix)...###
+00000ff0: 2032 2e31 0a0a 2d20 5265 7175 6972 6573   2.1..- Requires
+00001000: 2048 7970 726c 616e 6420 3e3d 2030 2e33   Hyprland >= 0.3
+00001010: 370a 2d20 5b4d 6f6e 6974 6f72 735d 2868  7.- [Monitors](h
+00001020: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001030: 6d2f 6879 7072 6c61 6e64 2d63 6f6d 6d75  m/hyprland-commu
+00001040: 6e69 7479 2f70 7970 726c 616e 642f 7769  nity/pyprland/wi
+00001050: 6b69 2f6d 6f6e 6974 6f72 7329 2070 6c75  ki/monitors) plu
+00001060: 6769 6e20 696d 7072 6f76 656d 656e 7473  gin improvements
+00001070: 2e0a 0a23 2323 2032 2e30 0a0a 2d20 4e65  ...### 2.0..- Ne
+00001080: 7720 6465 7065 6e64 656e 6379 3a20 5b61  w dependency: [a
+00001090: 696f 6669 6c65 735d 2868 7474 7073 3a2f  iofiles](https:/
+000010a0: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+000010b0: 742f 6169 6f66 696c 6573 2f29 0a2d 2041  t/aiofiles/).- A
+000010c0: 6464 6564 205b 6879 7374 6572 6573 6973  dded [hysteresis
+000010d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000010e0: 2e63 6f6d 2f68 7970 726c 616e 642d 636f  .com/hyprland-co
+000010f0: 6d6d 756e 6974 792f 7079 7072 6c61 6e64  mmunity/pyprland
+00001100: 2f77 696b 692f 7363 7261 7463 6870 6164  /wiki/scratchpad
+00001110: 7323 6879 7374 6572 6573 6973 2d6f 7074  s#hysteresis-opt
+00001120: 696f 6e61 6c29 2073 7570 706f 7274 2066  ional) support f
+00001130: 6f72 205b 7363 7261 7463 6870 6164 735d  or [scratchpads]
+00001140: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001150: 636f 6d2f 6879 7072 6c61 6e64 2d63 6f6d  com/hyprland-com
+00001160: 6d75 6e69 7479 2f70 7970 726c 616e 642f  munity/pyprland/
+00001170: 7769 6b69 2f73 6372 6174 6368 7061 6473  wiki/scratchpads
+00001180: 292e 0a0a 2323 2320 312e 3130 0a0a 2d20  )...### 1.10..- 
+00001190: 4e65 7720 5b66 6574 6368 5f63 6c69 656e  New [fetch_clien
+000011a0: 745f 6d65 6e75 5d28 6874 7470 733a 2f2f  t_menu](https://
+000011b0: 6769 7468 7562 2e63 6f6d 2f68 7970 726c  github.com/hyprl
+000011c0: 616e 642d 636f 6d6d 756e 6974 792f 7079  and-community/py
+000011d0: 7072 6c61 6e64 2f77 696b 692f 6665 7463  prland/wiki/fetc
+000011e0: 685f 636c 6965 6e74 5f6d 656e 7529 2061  h_client_menu) a
+000011f0: 6e64 205b 7368 6f72 7463 7574 735f 6d65  nd [shortcuts_me
+00001200: 6e75 5d28 6874 7470 733a 2f2f 6769 7468  nu](https://gith
+00001210: 7562 2e63 6f6d 2f68 7970 726c 616e 642d  ub.com/hyprland-
+00001220: 636f 6d6d 756e 6974 792f 7079 7072 6c61  community/pyprla
+00001230: 6e64 2f77 696b 692f 7368 6f72 7463 7574  nd/wiki/shortcut
+00001240: 735f 6d65 6e75 2920 706c 7567 696e 732e  s_menu) plugins.
+00001250: 0a0a 2323 2320 312e 390a 0a2d 2049 6e74  ..### 1.9..- Int
+00001260: 726f 6475 6365 6420 5b73 686f 7274 6375  roduced [shortcu
+00001270: 7473 5f6d 656e 755d 2868 7474 7073 3a2f  ts_menu](https:/
+00001280: 2f67 6974 6875 622e 636f 6d2f 6879 7072  /github.com/hypr
+00001290: 6c61 6e64 2d63 6f6d 6d75 6e69 7479 2f70  land-community/p
+000012a0: 7970 726c 616e 642f 7769 6b69 2f73 686f  yprland/wiki/sho
+000012b0: 7274 6375 7473 5f6d 656e 7529 2070 6c75  rtcuts_menu) plu
+000012c0: 6769 6e2e 0a0a 2323 2320 312e 380a 0a2d  gin...### 1.8..-
+000012d0: 2052 6571 7569 7265 7320 4879 7072 6c61   Requires Hyprla
+000012e0: 6e64 203e 3d20 302e 3330 0a2d 2041 6464  nd >= 0.30.- Add
+000012f0: 6564 205b 6c61 796f 7574 5f63 656e 7465  ed [layout_cente
+00001300: 725d 2868 7474 7073 3a2f 2f67 6974 6875  r](https://githu
+00001310: 622e 636f 6d2f 6879 7072 6c61 6e64 2d63  b.com/hyprland-c
+00001320: 6f6d 6d75 6e69 7479 2f70 7970 726c 616e  ommunity/pyprlan
+00001330: 642f 7769 6b69 2f6c 6179 6f75 745f 6365  d/wiki/layout_ce
+00001340: 6e74 6572 2920 706c 7567 696e 2e0a 0a3c  nter) plugin...<
+00001350: 2f64 6574 6169 6c73 3e0a 0a3c 6120 6872  /details>..<a hr
+00001360: 6566 3d22 6874 7470 733a 2f2f 7374 6172  ef="https://star
+00001370: 2d68 6973 746f 7279 2e63 6f6d 2f23 6664  -history.com/#fd
+00001380: 6576 3331 2f70 7970 726c 616e 6426 4461  ev31/pyprland&Da
+00001390: 7465 223e 0a20 203c 7069 6374 7572 653e  te">.  <picture>
+000013a0: 0a20 2020 203c 736f 7572 6365 206d 6564  .    <source med
+000013b0: 6961 3d22 2870 7265 6665 7273 2d63 6f6c  ia="(prefers-col
+000013c0: 6f72 2d73 6368 656d 653a 2064 6172 6b29  or-scheme: dark)
+000013d0: 2220 7372 6373 6574 3d22 6874 7470 733a  " srcset="https:
+000013e0: 2f2f 6170 692e 7374 6172 2d68 6973 746f  //api.star-histo
+000013f0: 7279 2e63 6f6d 2f73 7667 3f72 6570 6f73  ry.com/svg?repos
+00001400: 3d66 6465 7633 312f 7079 7072 6c61 6e64  =fdev31/pyprland
+00001410: 2674 7970 653d 5469 6d65 6c69 6e65 2674  &type=Timeline&t
+00001420: 6865 6d65 3d64 6172 6b22 202f 3e0a 2020  heme=dark" />.  
+00001430: 2020 3c73 6f75 7263 6520 6d65 6469 613d    <source media=
+00001440: 2228 7072 6566 6572 732d 636f 6c6f 722d  "(prefers-color-
+00001450: 7363 6865 6d65 3a20 6c69 6768 7429 2220  scheme: light)" 
+00001460: 7372 6373 6574 3d22 6874 7470 733a 2f2f  srcset="https://
+00001470: 6170 692e 7374 6172 2d68 6973 746f 7279  api.star-history
+00001480: 2e63 6f6d 2f73 7667 3f72 6570 6f73 3d66  .com/svg?repos=f
+00001490: 6465 7633 312f 7079 7072 6c61 6e64 2674  dev31/pyprland&t
+000014a0: 7970 653d 5469 6d65 6c69 6e65 2220 2f3e  ype=Timeline" />
+000014b0: 0a20 2020 203c 696d 6720 616c 743d 2253  .    <img alt="S
+000014c0: 7461 7220 4869 7374 6f72 7920 4368 6172  tar History Char
+000014d0: 7422 2073 7263 3d22 6874 7470 733a 2f2f  t" src="https://
+000014e0: 6170 692e 7374 6172 2d68 6973 746f 7279  api.star-history
+000014f0: 2e63 6f6d 2f73 7667 3f72 6570 6f73 3d66  .com/svg?repos=f
+00001500: 6465 7633 312f 7079 7072 6c61 6e64 2674  dev31/pyprland&t
+00001510: 7970 653d 5469 6d65 6c69 6e65 2220 2f3e  ype=Timeline" />
+00001520: 0a20 203c 2f70 6963 7475 7265 3e0a 3c2f  .  </picture>.</
+00001530: 613e 0a                                  a>.
```

### Comparing `pyprland-2.2.9/pyprland/adapters/units.py` & `pyprland-2.3.0/pyprland/adapters/units.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,45 @@
-" Unit conversion & co "
-from typing import Any
+"""Conversion functions for units used in Pyprland & plugins."""
 
+from ..common import is_rotated
+from ..types import MonitorInfo
+
+
+def convert_monitor_dimension(size: int | str, ref_value: int, monitor: MonitorInfo) -> int:
+    """Convert `size` into pixels (given a reference value applied to a `monitor`).
 
-def convert_monitor_dimension(
-    size: int | str, ref_value, monitor: dict[str, Any]
-) -> int:
-    """Convert `size` into pixels (given a reference value applied to a `monitor`)
     if size is an integer, assumed pixels & return it
     if size is a string, expects a "%" or "px" suffix
     else throws an error
     """
-
     if isinstance(size, int):
         return size
 
     if isinstance(size, str):
         if size.endswith("%"):
             p = int(size[:-1])
             return int(ref_value / monitor["scale"] * p / 100)
         if size.endswith("px"):
             return int(size[:-2])
 
-    raise ValueError(f"Unsupported format: {size} (applied to {ref_value})")
+    msg = f"Unsupported format: {size} (applied to {ref_value})"
+    raise ValueError(msg)
 
 
-def convert_coords(coords: str, monitor: dict[str, Any]):
-    """
-    Converts a string like "X Y" to coordinates relative to monitor
+def convert_coords(coords: str, monitor: MonitorInfo) -> list[int]:
+    """Convert a string like "X Y" to coordinates relative to monitor.
+
     Supported formats for X, Y:
     - Percentage: "V%". V in [0; 100]
     - Pixels: "Vpx". V should fit in your screen and not be zero
 
     Example:
     "10% 20%", monitor 800x600 => 80, 120
     """
-
     return [
-        convert_monitor_dimension(name, monitor[ref], monitor)
+        convert_monitor_dimension(name, monitor[ref], monitor)  # type: ignore
         for (name, ref) in zip(
             [coord.strip() for coord in coords.split()],
-            (
-                ("height", "width")
-                if monitor["transform"] in (1, 3)
-                else ("width", "height")
-            ),
+            (("height", "width") if is_rotated(monitor) else ("width", "height")),
+            strict=False,
         )
     ]
```

### Comparing `pyprland-2.2.9/pyprland/command.py` & `pyprland-2.3.0/pyprland/command.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,452 +1,466 @@
-#!/bin/env python
-""" Pyprland - an Hyprland companion app (cli client & daemon) """
+"""Pyprland - an Hyprland companion app (cli client & daemon)."""
+
 import asyncio
 import importlib
 import itertools
-from functools import partial
-from typing import Self, Callable
-import tomllib
 import json
 import os
 import sys
+import tomllib
+from collections.abc import Callable
+from functools import partial
+from typing import Any, Self
 
-from pyprland.common import (
-    PyprError,
-    get_logger,
-    init_logger,
-    merge,
-    run_interactive_program,
-)
+from pyprland.common import IPC_FOLDER, get_logger, init_logger, merge, run_interactive_program
 from pyprland.ipc import get_event_stream, notify_error, notify_fatal, notify_info
 from pyprland.ipc import init as ipc_init
 from pyprland.plugins.interface import Plugin
+from pyprland.types import PyprError
+from pyprland.version import VERSION
 
-try:
-    CONTROL = f'/tmp/hypr/{ os.environ["HYPRLAND_INSTANCE_SIGNATURE"] }/.pyprland.sock'
-except KeyError:
-    print(
-        "This is a fatal error, assuming we are running documentation generation hence ignoring it"
-    )
-
+CONTROL = f"{IPC_FOLDER}/.pyprland.sock"
 OLD_CONFIG_FILE = "~/.config/hypr/pyprland.json"
 CONFIG_FILE = "~/.config/hypr/pyprland.toml"
 
 PYPR_DEMO = os.environ.get("PYPR_DEMO", False)
 
 __all__: list[str] = []
 
 
 class Pyprland:
-    "Main app object"
+    """Main app object."""
+
     server: asyncio.Server
     event_reader: asyncio.StreamReader
     stopped = False
     config: dict[str, dict] = {}
-    tasks: None | asyncio.TaskGroup = None
+    tasks: list[asyncio.Task] = []
+    tasks_group: None | asyncio.TaskGroup = None
     instance: Self | None = None
     log_handler: Callable[[Plugin, str, tuple], None]
 
     @classmethod
-    def _set_instance(cls, instance):
-        "Set instance reference into class (for testing/debugging only)"
+    def _set_instance(cls, instance: Self) -> None:
+        """Set instance reference into class (for testing/debugging only)."""
         cls.instance = instance
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.pyprland_mutex_event = asyncio.Event()
         self.pyprland_mutex_event.set()
         self.config = {}
         self.plugins: dict[str, Plugin] = {}
         self.log = get_logger()
-        self.queues = {}
+        self.queues: dict[str, asyncio.Queue] = {}
         self._set_instance(self)
 
-    async def initialize(self):
-        "Initializes the main structures"
+    async def initialize(self) -> None:
+        """Initialize the main structures."""
         await self.load_config()  # ensure sockets are connected first
 
-    async def __open_config(self, config_filename=""):
-        """Loads config file as self.config"""
+    async def __open_config(self, config_filename: str = "") -> dict[str, Any]:
+        """Load config file as self.config."""
         if config_filename:
-            fname = os.path.expandvars(os.path.expanduser(config_filename))
+            fname = os.path.expanduser(os.path.expandvars(config_filename))
+            if os.path.isdir(fname):
+                config: dict[str, Any] = {}
+                for toml_file in sorted(os.listdir(fname)):
+                    if not toml_file.endswith(".toml"):
+                        continue
+                    merge(config, self.__load_config_file(f"{fname}/{toml_file}"))
+                return config
         else:
             if os.path.exists(OLD_CONFIG_FILE) and not os.path.exists(CONFIG_FILE):
                 self.log.warning("Consider changing your configuration to TOML format.")
             self.config.clear()
-            fname = os.path.expanduser(CONFIG_FILE)
+            fname = os.path.expanduser(os.path.expandvars(CONFIG_FILE))
 
-        try:
-            config = self.__load_config_file(fname)
-        except tomllib.TOMLDecodeError as e:
-            self.log.critical("Problem reading %s: %s", fname, e)
-            await notify_error(f"Pyprland failed to read config: {e}")
-            raise PyprError() from e
-        except FileNotFoundError as e:
-            self.log.critical("Unable to open %s: %s", fname, e)
-            await notify_error(f"Pyprland failed to read config: {e}")
-            raise PyprError() from e
+        config = self.__load_config_file(fname)
 
         if not config_filename:
             for extra_config in list(config["pyprland"].get("include", [])):
                 merge(config, await self.__open_config(extra_config))
             self.config.update(config)
         return config
 
-    def __load_config_file(self, fname):
-        """Loads a configuration file and returns it as a dictionary"""
+    def __load_config_file(self, fname: str) -> dict[str, Any]:
+        """Load a configuration file and returns it as a dictionary."""
         config = {}
         if os.path.exists(fname):
             self.log.info("Loading %s", fname)
             with open(fname, "rb") as f:
-                config = tomllib.load(f)
+                try:
+                    config = tomllib.load(f)
+                except tomllib.TOMLDecodeError as e:
+                    self.log.critical("Problem reading %s: %s", fname, e)
+                    raise PyprError from e
         elif os.path.exists(os.path.expanduser(OLD_CONFIG_FILE)):
             self.log.info("Loading %s", OLD_CONFIG_FILE)
             with open(os.path.expanduser(OLD_CONFIG_FILE), encoding="utf-8") as f:
                 config = json.loads(f.read())
         else:
             self.log.critical("Config file not found! Please create %s", fname)
-            raise PyprError()
+            raise PyprError
         return config
 
-    async def _load_single_plugin(self, name, init) -> bool:
-        "Load a single plugin, optionally calling `init`"
+    async def _load_single_plugin(self, name: str, init: bool) -> bool:
+        """Load a single plugin, optionally calling `init`."""
         if "." in name:
             modname = name
         elif "external:" in name:
             modname = name.replace("external:", "")
         else:
             modname = f"pyprland.plugins.{name}"
         try:
             plug = importlib.import_module(modname).Extension(name)
             if init:
                 await plug.init()
                 self.queues[name] = asyncio.Queue()
-                if self.tasks:
-                    self.tasks.create_task(self._plugin_runner_loop(name))
+                if self.tasks_group:
+                    self.tasks_group.create_task(self._plugin_runner_loop(name))
             self.plugins[name] = plug
         except ModuleNotFoundError as e:
-            self.log.error("Unable to locate plugin called '%s'", name)
-            await notify_info(
-                f'Config requires plugin "{name}" but pypr can\'t find it: {e}'
-            )
+            self.log.exception("Unable to locate plugin called '%s'", name)
+            await notify_info(f'Config requires plugin "{name}" but pypr can\'t find it: {e}')
             return False
         except Exception as e:
             await notify_info(f"Error loading plugin {name}: {e}")
-            self.log.error("Error loading plugin %s:", name, exc_info=True)
-            raise PyprError() from e
+            self.log.exception("Error loading plugin %s:", name)
+            raise PyprError from e
         return True
 
-    async def __load_plugins_config(self, init=True):
-        """Loads the plugins mentioned in the config.
+    async def __load_plugins_config(self, init: bool = True) -> None:
+        """Load the plugins mentioned in the config.
+
         If init is `True`, call the `init()` method on each plugin.
         """
-
         sys.path.extend(self.config["pyprland"].get("plugins_paths", []))
 
         init_pyprland = "pyprland" not in self.plugins
 
         for name in ["pyprland"] + self.config["pyprland"]["plugins"]:
-            if name not in self.plugins:
-                if not await self._load_single_plugin(name, init):
-                    continue
+            if name not in self.plugins and not await self._load_single_plugin(name, init):
+                continue
             if init:
                 try:
                     await self.plugins[name].load_config(self.config)
                     await asyncio.wait_for(self.plugins[name].on_reload(), timeout=5.0)
-                except asyncio.TimeoutError:
+                except TimeoutError:
                     self.plugins[name].log.info("timed out on reload")
-                except PyprError:
-                    raise
                 except Exception as e:
                     await notify_info(f"Error initializing plugin {name}: {e}")
-                    self.log.error("Error initializing plugin %s:", name, exc_info=True)
-                    raise PyprError() from e
+                    self.log.exception("Error initializing plugin %s:", name)
+                    raise PyprError from e
                 else:
                     self.plugins[name].log.info("configured")
         if init_pyprland:
             plug = self.plugins["pyprland"]
             plug.set_commands(reload=self.load_config)  # type: ignore
 
-    async def load_config(self, init=True):
-        """loads the configuration (new plugins will be added & config updated)
-
-        if `init` is true, also initializes the plugins"""
+    async def load_config(self, init: bool = True) -> None:
+        """Load the configuration (new plugins will be added & config updated).
 
+        if `init` is true, also initializes the plugins
+        """
         await self.__open_config()
         assert self.config
         await self.__load_plugins_config(init=init)
         colored_logs = self.config["pyprland"].get("colored_handlers_log", True)
-        self.log_handler = (
-            self.colored_log_handler if colored_logs else self.plain_log_handler
-        )  # pylint: disable=attribute-defined-outside-init
-
-    def plain_log_handler(self, plugin, name, params):
-        "log a handler method without color"
-        plugin.log.debug(f"{name}{params}")
+        self.log_handler = self.colored_log_handler if colored_logs else self.plain_log_handler
 
-    def colored_log_handler(self, plugin, name, params):
-        "log a handler method with color"
+    def plain_log_handler(self, plugin: Plugin, name: str, params: tuple[str]) -> None:
+        """Log a handler method without color."""
+        plugin.log.debug("%s%s", name, params)
+
+    def colored_log_handler(self, plugin: Plugin, name: str, params: tuple[str]) -> None:
+        """Log a handler method with color."""
         color = 33 if name.startswith("run_") else 30
-        plugin.log.debug(f"\033[{color};1m%s%s\033[0m", name, params)
+        plugin.log.debug("\033[%s;1m%s%s\033[0m", color, name, params)
 
-    async def _run_plugin_handler(self, plugin, full_name, params):
-        "Runs a single handler on a plugin"
+    async def _run_plugin_handler(self, plugin: Plugin, full_name: str, params: tuple[str]) -> None:
+        """Run a single handler on a plugin."""
         self.log_handler(plugin, full_name, params)
         try:
             await getattr(plugin, full_name)(*params)
         except AssertionError as e:
-            self.log.error(
-                "This could be a bug in Pyprland, if you think so, report on https://github.com/fdev31/pyprland/issues"
-            )
-            self.log.exception(e)
-            await notify_error(
-                f"Pypr integrity check failed on {plugin.name}::{full_name}: {e}"
-            )
+            self.log.exception("This could be a bug in Pyprland, if you think so, report on https://github.com/fdev31/pyprland/issues")
+            await notify_error(f"Pypr integrity check failed on {plugin.name}::{full_name}: {e}")
         except Exception as e:  # pylint: disable=W0718
-            self.log.warning("%s::%s(%s) failed:", plugin.name, full_name, params)
-            self.log.exception(e)
+            self.log.exception("%s::%s(%s) failed:", plugin.name, full_name, params)
             await notify_error(f"Pypr error {plugin.name}::{full_name}: {e}")
 
-    async def _callHandler(self, full_name, *params, notify=""):
-        "Call an event handler with params"
+    async def _call_handler(self, full_name: str, *params: str, notify: str = "") -> bool:
+        """Call an event handler with params."""
         handled = False
         for plugin in self.plugins.values():
             if hasattr(plugin, full_name):
                 handled = True
                 task = partial(self._run_plugin_handler, plugin, full_name, params)
                 if plugin == "pyprland":
                     await task()
-                else:
+                elif not plugin.aborted:
                     await self.queues[plugin.name].put(task)
         if notify and not handled:
             await notify_info(f'"{notify}" not found')
         return handled
 
-    async def read_events_loop(self):
-        "Consumes the event loop and calls corresponding handlers"
+    async def read_events_loop(self) -> None:
+        """Consume the event loop and calls corresponding handlers."""
         while not self.stopped:
             try:
                 data = (await self.event_reader.readline()).decode()
-            except RuntimeError as e:
-                self.log.error("Aborting event loop: %s", e)
+            except RuntimeError:
+                self.log.exception("Aborting event loop")
                 return
             except UnicodeDecodeError:
-                self.log.error("Invalid unicode while reading events")
+                self.log.exception("Invalid unicode while reading events")
                 continue
             if not data:
                 self.log.critical("Reader starved")
                 return
             cmd, params = data.split(">>", 1)
             full_name = f"event_{cmd}"
 
             # self.log.debug("[%s] %s", cmd, params.strip())
-            await self._callHandler(full_name, params.rstrip("\n"))
+            await self._call_handler(full_name, params.rstrip("\n"))
 
-    async def read_command(self, reader, writer) -> None:
-        "Receives a socket command"
+    async def exit_plugins(self) -> None:
+        """Exit all plugins."""
+        for plugin in self.plugins.values():
+            if not plugin.aborted:
+                plugin.aborted = True
+                await asyncio.wait_for(plugin.exit(), timeout=2.0)
+
+    async def read_command(self, reader: asyncio.StreamReader, writer: asyncio.StreamWriter) -> None:
+        """Receive a socket command."""
         data = (await reader.readline()).decode()
         if not data:
             self.log.critical("Server starved")
             data = "exit"
         data = data.strip()
         if data == "exit":
+
+            async def _abort() -> None:
+                await self.exit_plugins()
+                # cancel the task group
+                for task in self.tasks:
+                    task.cancel()
+                writer.close()
+                await writer.wait_closed()
+                for q in self.queues.values():
+                    await q.put(None)
+                self.server.close()
+                # Ensure the process exits
+                await asyncio.sleep(1)
+                if os.path.exists(CONTROL):
+                    os.unlink(CONTROL)
+                os._exit(0)
+
             self.stopped = True
-            writer.close()
-            await writer.wait_closed()
-            self.server.close()
+            asyncio.create_task(_abort())
             return
         args = data.split(None, 1)
         if len(args) == 1:
             cmd = args[0]
             args = []
         else:
             cmd = args[0]
             args = args[1:]
 
         full_name = f"run_{cmd}"
 
         if PYPR_DEMO:
-            os.system(f"notify-send -t 4000 '{data}'")
+            os.system(f"notify-send -t 4000 '{data}'")  # noqa: ASYNC102
 
-        if not await self._callHandler(full_name, *args, notify=cmd):
+        if not await self._call_handler(full_name, *args, notify=cmd):
             self.log.warning("No such command: %s", cmd)
 
-    async def serve(self):
-        "Runs the server"
-        try:
-            async with self.server:
-                await self.server.serve_forever()
-        finally:
-            await asyncio.gather(*(plugin.exit() for plugin in self.plugins.values()))
+    async def serve(self) -> None:
+        """Run the server."""
+        async with self.server:
+            await self.server.wait_closed()
 
-    async def _plugin_runner_loop(self, name):
-        "Runs tasks for a given plugin indefinitely"
+    async def _plugin_runner_loop(self, name: str) -> None:
+        """Run tasks for a given plugin indefinitely."""
         q = self.queues[name]
         is_pyprland = name == "pyprland"
 
         while not self.stopped:
             if not is_pyprland:
                 await self.pyprland_mutex_event.wait()
             try:
                 task = await q.get()
+                if task is None:
+                    return
                 if is_pyprland:
                     self.pyprland_mutex_event.clear()
-            except RuntimeError as e:
-                self.log.error("Aborting [%s] loop: %s", name, e)
+            except RuntimeError:
+                self.log.exception("Aborting [%s] loop", name)
                 return
             try:
                 await asyncio.wait_for(task(), timeout=12.0)
-            except asyncio.TimeoutError:
-                self.log.error("Timeout running plugin %s::%s", name, task)
-            except Exception as e:  # pylint: disable=W0718
-                self.log.error(
-                    "Unhandled error running plugin %s::%s: %s", name, task, e
-                )
+            except TimeoutError:
+                self.log.exception("Timeout running plugin %s::%s", name, task)
+            except Exception:  # pylint: disable=W0718
+                self.log.exception("Unhandled error running plugin %s::%s", name, task)
             if is_pyprland and q.empty():
                 self.pyprland_mutex_event.set()
 
-    async def plugins_runner(self):
-        "Runs plugins' task using the created `tasks` TaskGroup attribute"
+    async def plugins_runner(self) -> None:
+        """Run plugins' task using the created `tasks` TaskGroup attribute."""
         async with asyncio.TaskGroup() as group:
-            self.tasks = group
+            self.tasks_group = group
             for name in self.plugins:
-                group.create_task(self._plugin_runner_loop(name))
+                self.tasks.append(group.create_task(self._plugin_runner_loop(name)))
 
-    async def run(self):
-        "Runs the server and the event listener"
+    async def run(self) -> None:
+        """Run the server and the event listener."""
         await asyncio.gather(
             asyncio.create_task(self.serve()),
             asyncio.create_task(self.read_events_loop()),
             asyncio.create_task(self.plugins_runner()),
         )
 
 
-async def run_daemon():
-    "Runs the server / daemon"
-    manager = Pyprland()
+async def get_event_stream_with_retry(max_retry: int = 10) -> tuple[asyncio.StreamReader, asyncio.StreamWriter] | tuple[None, Exception]:
+    """Obtain the event stream, retrying if it fails.
+
+    If retry count is exhausted, returns (None, exception).
+    """
     err_count = itertools.count()
-    manager.server = await asyncio.start_unix_server(manager.read_command, CONTROL)
-    max_retry = 10
     while True:
         attempt = next(err_count)
         try:
-            events_reader, events_writer = await get_event_stream()
+            return await get_event_stream()
         except Exception as e:  # pylint: disable=W0718
             if attempt > max_retry:
-                manager.log.critical("Failed to open hyprland event stream: %s.", e)
-                await notify_fatal("Failed to open hyprland event stream")
-                raise PyprError() from e
-            manager.log.warning(
-                "Failed to get event stream: %s, retry %s/%s...", e, attempt, max_retry
-            )
+                return None, e
             await asyncio.sleep(1)
-        else:
-            break
 
-    manager.event_reader = events_reader
 
-    try:
-        await manager.initialize()
-    except PyprError as e:
-        if bool(str(e)):
-            await notify_fatal(f"Pypr failed to start: {e}")
-        else:
-            await notify_fatal("Pypr failed to start!")
+async def run_daemon() -> None:
+    """Run the server / daemon."""
+    manager = Pyprland()
+    manager.server = await asyncio.start_unix_server(manager.read_command, CONTROL)
+
+    events_reader, events_writer = await get_event_stream_with_retry()
+    if events_reader is None:
+        manager.log.critical("Failed to open hyprland event stream: %s.", events_writer)
+        await notify_fatal("Failed to open hyprland event stream")
+        raise PyprError from events_writer
+
+    manager.event_reader = events_reader
 
-        raise SystemExit(1) from e
-    except Exception as e:
-        manager.log.critical("Failed to load config.", exc_info=True)
-        await notify_fatal(f"Pypr couldn't load config: {e}")
-        raise SystemExit(1) from e
+    await manager.initialize()
 
     manager.log.debug("[ initialized ]".center(80, "="))
+
     try:
         await manager.run()
     except KeyboardInterrupt:
         print("Interrupted")
     except asyncio.CancelledError:
         manager.log.critical("cancelled")
     else:
+        await manager.exit_plugins()
+        assert isinstance(events_writer, asyncio.StreamWriter)
         events_writer.close()
         await events_writer.wait_closed()
         manager.server.close()
         await manager.server.wait_closed()
 
 
-def show_help(manager):
-    "show the documentation"
+def show_help(manager: Pyprland) -> None:
+    """Show the documentation."""
 
-    def format_doc(txt):
+    def format_doc(txt: str) -> str:
         return txt.split("\n")[0]
 
     print(
         """Syntax: pypr [command]
 
 If the command is ommited, runs the daemon which will start every configured plugin.
 
 Available commands:
 """
     )
+    builtins_docs = {
+        "dumpjson": "Dump the configuration in JSON format.",
+        "edit": "Edit the configuration file.",
+        "exit": "Exit the daemon.",
+        "help": "Show this help.",
+        "version": "Show the version.",
+    }
+    for name, doc in builtins_docs.items():
+        print(f" {name:20s} {doc}")
+
     for plug in manager.plugins.values():
         for name in dir(plug):
             if not name.startswith("run_"):
                 continue
             fn = getattr(plug, name)
             if callable(fn):
                 doc_txt = format_doc(fn.__doc__) if fn.__doc__ else "N/A"
                 print(f" {name[4:]:20s} {doc_txt} [{plug.name}]")
 
 
-async def run_client():
-    "Runs the client (CLI)"
+async def run_client() -> None:
+    """Run the client (CLI)."""
     manager = Pyprland()
 
     if sys.argv[1] == "version":
-        print("2.2.9")  # Automatically updated version
-        return
+        print(VERSION)
+        return None
 
     if sys.argv[1] == "edit":
         editor = os.environ.get("EDITOR", os.environ.get("VISUAL", "vi"))
         filename = os.path.expanduser(CONFIG_FILE)
         run_interactive_program(f'{editor} "{filename}"')
         sys.argv[1] = "reload"
 
-    if sys.argv[1] in ("--help", "-h", "help"):
+    if sys.argv[1] in {"--help", "-h", "help"}:
         await manager.load_config(init=False)
         return show_help(manager)
 
+    if sys.argv[1] in ("dumpjson"):
+        await manager.load_config(init=False)
+        # Dump manager.config in TOML format
+        print(json.dumps(manager.config, indent=2))
+        return None
+
     try:
         _, writer = await asyncio.open_unix_connection(CONTROL)
     except (ConnectionRefusedError, FileNotFoundError) as e:
         manager.log.critical("Failed to open control socket, is pypr daemon running ?")
         await notify_error("Pypr can't connect, is daemon running ?")
-        raise PyprError() from e
+        raise PyprError from e
 
     args = sys.argv[1:]
     args[0] = args[0].replace("-", "_")
     writer.write((" ".join(args)).encode())
     await writer.drain()
     writer.close()
     await writer.wait_closed()
 
 
-def use_param(txt):
-    """Checks if parameter `txt` is in sys.argv
+def use_param(txt: str) -> str:
+    """Check if parameter `txt` is in sys.argv.
+
     if found, removes it from sys.argv & returns the argument value
     """
     v = ""
     if txt in sys.argv:
         i = sys.argv.index(txt)
         v = sys.argv[i + 1]
         del sys.argv[i : i + 2]
     return v
 
 
-def main():
-    "runs the command"
+def main() -> None:
+    """Run the command."""
     debug_flag = use_param("--debug")
     if debug_flag:
         init_logger(filename=debug_flag, force_debug=True)
     else:
         init_logger()
     ipc_init()
     log = get_logger("startup")
@@ -473,13 +487,13 @@
         except PyprError:
             log.critical("Command failed.")
         except json.decoder.JSONDecodeError as e:
             log.critical("Invalid JSON syntax in the config file: %s", e.args[0])
         except Exception:  # pylint: disable=W0718
             log.critical("Unhandled exception:", exc_info=True)
         finally:
-            if invoke_daemon:
+            if invoke_daemon and os.path.exists(CONTROL):
                 os.unlink(CONTROL)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyprland-2.2.9/pyprland/common.py` & `pyprland-2.3.0/pyprland/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,67 @@
-""" Shared utilities: logging """
+"""Shared utilities: logging."""
 
+import fcntl
+import logging
 import os
-import re
 import pty
-import sys
-import fcntl
-import struct
+import re
 import select
-import termios
-import logging
+import struct
 import subprocess
+import sys
+import termios
 from dataclasses import dataclass, field
+from typing import Any, cast
+
+from .types import MonitorInfo, VersionInfo
 
 __all__ = [
     "DEBUG",
-    "get_logger",
-    "state",
-    "PyprError",
     "apply_variables",
+    "get_logger",
     "merge",
     "run_interactive_program",
+    "state",
 ]
 
 DEBUG = os.environ.get("DEBUG", False)
 
+HYPRLAND_INSTANCE_SIGNATURE = os.environ["HYPRLAND_INSTANCE_SIGNATURE"]
+
+MINIMUM_ADDR_LEN = 10
+
+try:
+    IPC_FOLDER = (
+        f'{os.environ["XDG_RUNTIME_DIR"]}/hypr/{HYPRLAND_INSTANCE_SIGNATURE}'
+        if os.path.exists(f'{os.environ["XDG_RUNTIME_DIR"]}/hypr/{HYPRLAND_INSTANCE_SIGNATURE}')
+        else f"/tmp/hypr/{HYPRLAND_INSTANCE_SIGNATURE}"  # noqa: S108
+    )
+except KeyError:
+    print("This is a fatal error, assuming we are running documentation generation or testing in a sandbox, hence ignoring it")
+    IPC_FOLDER = "/fake"
 
-def set_terminal_size(descriptor, rows, cols):
-    "Set the terminal size"
+
+def set_terminal_size(descriptor: int, rows: int, cols: int) -> None:
+    """Set the terminal size."""
     fcntl.ioctl(descriptor, termios.TIOCSWINSZ, struct.pack("HHHH", rows, cols, 0, 0))
 
 
-def set_raw_mode(descriptor):
-    "Set a file descriptor in raw mode"
+def set_raw_mode(descriptor: int) -> None:
+    """Set a file descriptor in raw mode."""
     # Get the current terminal attributes
     attrs = termios.tcgetattr(descriptor)
     # Set the terminal to raw mode
     attrs[3] &= ~termios.ICANON  # Disable canonical mode (line buffering)
     attrs[3] &= ~termios.ECHO  # Disable echoing of input characters
     termios.tcsetattr(descriptor, termios.TCSANOW, attrs)
 
 
-def run_interactive_program(command):
-    "Run an interactive program in a blocking way"
+def run_interactive_program(command: str) -> None:
+    """Run an interactive program in a blocking way."""
     # Create a pseudo-terminal
     master, slave = pty.openpty()
 
     # Start the program in the pseudo-terminal
     process = subprocess.Popen(  # pylint: disable=consider-using-with
         command, shell=True, stdin=slave, stdout=slave, stderr=slave
     )
@@ -81,94 +97,82 @@
     except OSError:
         pass
     finally:
         # Restore terminal settings
         termios.tcsetattr(sys.stdin, termios.TCSANOW, termios.tcgetattr(0))
 
 
-def merge(merged, obj2):
-    """
-    Merges the content of d2 into d1
-    Eg:
-        merge({"a": {"b": 1}}, {"a": {"c": 2}}) == {"a": {"b": 1, "c": 2}}
+def merge(merged: dict[str, Any], obj2: dict[str, Any]) -> dict[str, Any]:
+    """Merge the content of d2 into d1.
 
     Args:
-    - merged (dict): First dictionary to merge (will be updated).
-    - obj2 (dict): Second dictionary to merge
+        merged (dict): Dictionary to merge into
+        obj2 (dict): Dictionary to merge from
 
     Returns:
-    - dict: Merged dictionary
+        `merged` dictionary with the merged content
+
+    Eg:
+        merge({"a": {"b": 1}}, {"a": {"c": 2}}) == {"a": {"b": 1, "c": 2}}
+
     """
     for key, value in obj2.items():
         if key in merged and isinstance(merged[key], dict) and isinstance(value, dict):
             # If both values are dictionaries, recursively merge them
             merge(merged[key], value)
-        elif (
-            key in merged and isinstance(merged[key], list) and isinstance(value, list)
-        ):
+        elif key in merged and isinstance(merged[key], list) and isinstance(value, list):
             # If both values are lists, concatenate them
             merged[key] += value
         else:
             # Otherwise, update the value or add the key-value pair
             merged[key] = value
     return merged
 
 
-class PyprError(Exception):
-    """Used for errors which already triggered logging"""
-
-
 class LogObjects:
-    """Reusable objects for loggers"""
+    """Reusable objects for loggers."""
 
     handlers: list[logging.Handler] = []
 
 
-def init_logger(filename=None, force_debug=False):
-    """initializes the logging system"""
+def init_logger(filename: str | None = None, force_debug: bool = False) -> None:
+    """Initialize the logging system."""
     global DEBUG
     if force_debug:
         DEBUG = True
 
     class ScreenLogFormatter(logging.Formatter):
-        "A custom formatter, adding colors"
-        LOG_FORMAT = (
-            r"%(name)25s - %(message)s // %(filename)s:%(lineno)d"
-            if DEBUG
-            else r"%(message)s"
-        )
+        """A custom formatter, adding colors."""
+
+        LOG_FORMAT = r"%(name)25s - %(message)s // %(filename)s:%(lineno)d" if DEBUG else r"%(message)s"
         RESET_ANSI = "\x1b[0m"
 
         FORMATTERS = {
             logging.DEBUG: logging.Formatter(LOG_FORMAT + RESET_ANSI),
             logging.INFO: logging.Formatter(LOG_FORMAT + RESET_ANSI),
             logging.WARNING: logging.Formatter("\x1b[33;20m" + LOG_FORMAT + RESET_ANSI),
             logging.ERROR: logging.Formatter("\x1b[31;20m" + LOG_FORMAT + RESET_ANSI),
             logging.CRITICAL: logging.Formatter("\x1b[31;1m" + LOG_FORMAT + RESET_ANSI),
         }
 
-        def format(self, record):
+        def format(self, record: logging.LogRecord) -> str:
             return self.FORMATTERS[record.levelno].format(record)
 
     logging.basicConfig()
     if filename:
         file_handler = logging.FileHandler(filename)
-        file_handler.setFormatter(
-            logging.Formatter(
-                fmt=r"%(asctime)s [%(levelname)s] %(name)s :: %(message)s :: %(filename)s:%(lineno)d"
-            )
-        )
+        file_handler.setFormatter(logging.Formatter(fmt=r"%(asctime)s [%(levelname)s] %(name)s :: %(message)s :: %(filename)s:%(lineno)d"))
         LogObjects.handlers.append(file_handler)
     stream_handler = logging.StreamHandler()
     stream_handler.setFormatter(ScreenLogFormatter())
     LogObjects.handlers.append(stream_handler)
 
 
-def get_logger(name="pypr", level=None) -> logging.Logger:
-    """Returns a named logger
+def get_logger(name: str = "pypr", level: int | None = None) -> logging.Logger:
+    """Return a named logger.
 
     Args:
         name (str): logger's name
         level (int): logger's level (auto if not set)
     """
     logger = logging.getLogger(name)
     if level is None:
@@ -178,24 +182,18 @@
     logger.propagate = False
     for handler in LogObjects.handlers:
         logger.addHandler(handler)
     logger.info('Logger "%s" initialized', name)
     return logger
 
 
-@dataclass(order=True)
-class VersionInfo:
-    major: int = 0
-    minor: int = 0
-    micro: int = 0
-
-
 @dataclass
 class SharedState:
-    "Stores commonly requested properties"
+    """Stores commonly requested properties."""
+
     active_workspace: str = ""  # workspace name
     active_monitor: str = ""  # monitor name
     active_window: str = ""  # window address
     variables: dict = field(default_factory=dict)
     monitors: list[str] = field(default_factory=list)
     hyprland_version: VersionInfo = field(default_factory=VersionInfo)
 
@@ -205,52 +203,58 @@
 Exposes most-commonly accessed attributes to avoid specific IPC requests
 - `active_monitor` monitor's name
 - `active_workspace` workspace's name
 - `active_window` window's address
 """
 
 
-def prepare_for_quotes(text: str):
-    "Escapes double quotes in text"
+def prepare_for_quotes(text: str) -> str:
+    """Escapes double quotes in text."""
     return text.replace('"', '\\"')
 
 
-def apply_variables(template: str, variables: dict[str, str]):
-    """Replace [var_name] with content from supplied variables
+def apply_variables(template: str, variables: dict[str, str]) -> str:
+    """Replace [var_name] with content from supplied variables.
+
     Args:
         template: the string template
         variables: a dict containing the variables to replace
     """
     pattern = r"\[([^\[\]]+)\]"
 
-    def replace(match):
+    def replace(match: re.Match[str]) -> str:
         var_name = match.group(1)
         return variables.get(var_name, match.group(0))
 
     return re.sub(pattern, replace, template)
 
 
-def apply_filter(text, filt_cmd: str):
-    """Apply filters to text
-    Currently supports only "s" command fom vim/ed"""
+def apply_filter(text: str, filt_cmd: str) -> str:
+    """Apply filters to text.
+
+    Currently supports only "s" command fom vim/ed
+    """
     if not filt_cmd:
         return text
     if filt_cmd[0] == "s":  # vi-like substitute
         (_, base, replacement, opts) = filt_cmd.split(filt_cmd[1])
         return re.sub(base, replacement, text, count=0 if "g" in opts else 1)
     return text
 
 
 class CastBoolMixin:
-    "Adds `cast_bool` method"
+    """Adds `cast_bool` method."""
 
     log: logging.Logger
 
-    def cast_bool(self, value, default_value=False):
-        "recovers wrong typing on boolean values"
+    def cast_bool(self, value: str | bool | None, default_value: bool = False) -> bool:
+        """Recovers wrong typing on boolean values."""
         if isinstance(value, str):
             lv = value.lower().strip()
-            r = lv not in ("false", "no", "off")
-            self.log.warning(
-                "Invalid value for boolean option: %s, considering it %s", value, r
-            )
-        return default_value if value is None else value
+            r = lv not in {"false", "no", "off"}
+            self.log.warning("Invalid value for boolean option: %s, considering it %s", value, r)
+        return default_value if value is None else cast(bool, value)
+
+
+def is_rotated(monitor: MonitorInfo) -> bool:
+    """Return True if the monitor is rotated."""
+    return monitor["transform"] in {1, 3, 5, 7}
```

### Comparing `pyprland-2.2.9/pyprland/ipc.py` & `pyprland-2.3.0/pyprland/ipc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,245 +1,241 @@
-#!/bin/env python
-""" Interact with hyprland using sockets """
+"""Interact with hyprland using sockets."""
 
 __all__ = [
-    "get_focused_monitor_props",
     "get_client_props",
+    "get_focused_monitor_props",
+    "hyprctl",
+    "hyprctl_json",
     "notify",
     "notify_error",
     "notify_info",
-    "hyprctl",
-    "hyprctlJSON",
 ]
 
 import asyncio
 import json
 import time
-import os
-from typing import Any
-from logging import Logger
+from collections.abc import Callable, Iterable
 from functools import partial
+from logging import Logger
+from typing import Any, cast
 
-from .common import PyprError, get_logger
+from .common import IPC_FOLDER, MINIMUM_ADDR_LEN, get_logger
+from .types import ClientInfo, MonitorInfo, PyprError
 
 log: Logger | None = None
 
-try:
-    HYPRCTL = f'/tmp/hypr/{ os.environ["HYPRLAND_INSTANCE_SIGNATURE"] }/.socket.sock'
-    EVENTS = f'/tmp/hypr/{ os.environ["HYPRLAND_INSTANCE_SIGNATURE"] }/.socket2.sock'
-except KeyError:
-    print(
-        "This is a fatal error, assuming we are running documentation generation hence ignoring it"
-    )
+HYPRCTL = f"{IPC_FOLDER}/.socket.sock"
+EVENTS = f"{IPC_FOLDER}/.socket2.sock"
 
 
-async def notify(text, duration=3, color="ff1010", icon=-1, logger=None):
-    "Uses hyprland notification system"
-    await hyprctl(
-        f"{icon} {int(duration*1000)} rgb({color})  {text}", "notify", logger=logger
-    )
+async def notify(text: str, duration: int = 3, color: str = "ff1010", icon: int = -1, logger: None | Logger = None) -> None:
+    """Hyprland notification system."""
+    await hyprctl(f"{icon} {int(duration * 1000)} rgb({color})  {text}", "notify", logger=logger)
 
 
 notify_fatal = partial(notify, icon=3, duration=10)
 notify_error = partial(notify, icon=0, duration=5)
 notify_info = partial(notify, icon=1, duration=5)
 
 
-async def get_event_stream():
-    "Returns a new event socket connection"
+async def get_event_stream() -> tuple[asyncio.StreamReader, asyncio.StreamWriter]:
+    """Return a new event socket connection."""
     return await asyncio.open_unix_connection(EVENTS)
 
 
-def retry_on_reset(func):
-    "wrapper to retry on reset"
+def retry_on_reset(func: Callable) -> Callable:
+    """Retry on reset wrapper."""
 
-    async def wrapper(*args, logger, **kwargs):
+    async def wrapper(*args, logger: Logger, **kwargs) -> Any:  # noqa: ANN401
         exc = None
         for count in range(3):
             try:
                 return await func(*args, **kwargs, logger=logger)
-            except ConnectionResetError as e:
+            except ConnectionResetError as e:  # noqa: PERF203
                 exc = e
                 logger.warning("ipc connection problem, retrying...")
                 await asyncio.sleep(0.5 * count)
         logger.error("ipc connection failed.")
-        raise ConnectionResetError() from exc
+        raise ConnectionResetError from exc
 
     return wrapper
 
 
 cached_responses: dict[str, list[Any]] = {
     # <command name>: [expiration_date, payload, retention_time]
-    "monitors": [0, None, 0.3],
+    "monitors": [0, None, 0.03],
     # "workspaces": [0, None, 0.1],
     # "clients": [0, None, 0.02],
 }
 
 
 @retry_on_reset
-async def hyprctlJSON(
-    command: str, logger=None
-) -> list[dict[str, Any]] | dict[str, Any]:
+async def hyprctl_json(command: str, logger: Logger | None = None) -> list[dict[str, Any]] | dict[str, Any]:
     """Run an IPC command and return the JSON output."""
-    logger = logger or log
+    logger = cast(Logger, logger or log)
     now = time.time()
     cached = command in cached_responses and cached_responses[command][0] > now
     if cached:
-        logger.debug(f"{command} (CACHE HIT)")
+        logger.debug("%s (CACHE HIT)", command)
         return cached_responses[command][1]  # type: ignore
     logger.debug(command)
     try:
         ctl_reader, ctl_writer = await asyncio.open_unix_connection(HYPRCTL)
     except FileNotFoundError as e:
         logger.critical("hyprctl socket not found! is it running ?")
-        raise PyprError() from e
+        raise PyprError from e
     ctl_writer.write(f"-j/{command}".encode())
     await ctl_writer.drain()
     resp = await ctl_reader.read()
     ctl_writer.close()
     await ctl_writer.wait_closed()
     ret = json.loads(resp)
-    assert isinstance(ret, (list, dict))
+    assert isinstance(ret, list | dict)
     if command in cached_responses:  # should fill the cache
         cached_responses[command][0] = now + cached_responses[command][2]
         cached_responses[command][1] = ret
     return ret
 
 
-def _format_command(command_list, default_base_command):
-    "helper function to format BATCH commands"
+def _format_command(command_list: list[str] | list[list[str]], default_base_command: str) -> Iterable[str]:
+    """Format a list of commands to be sent to Hyprland.
+
+    Args:
+        command_list: list of commands to send
+            Each command can be a string or a tuple with the command and the base command
+        default_base_command: type of command to send
+    """
     for command in command_list:
         if isinstance(command, str):
             yield f"{default_base_command} {command}"
         else:
             yield f"{command[1]} {command[0]}"
 
 
 @retry_on_reset
-async def hyprctl(
-    command: str | list[str], base_command: str = "dispatch", logger=None
-) -> bool:
+async def hyprctl(command: str | list[str], base_command: str = "dispatch", logger: Logger | None = None) -> bool:
     """Run an IPC command. Returns success value.
 
     Args:
         command: single command (str) or list of commands to send to Hyprland
         base_command: type of command to send
+        logger: logger to use in case of error
 
     Returns:
         True on success
     """
-    logger = logger or log
+    logger = cast(Logger, logger or log)
     logger.debug("%s %s", base_command, command)
     try:
         ctl_reader, ctl_writer = await asyncio.open_unix_connection(HYPRCTL)
     except FileNotFoundError as e:
         logger.critical("hyprctl socket not found! is it running ?")
-        raise PyprError() from e
+        raise PyprError from e
 
     if isinstance(command, list):
         nb_cmds = len(command)
-        ctl_writer.write(
-            f"[[BATCH]] {' ; '.join(_format_command(command, base_command))}".encode()
-        )
+        ctl_writer.write(f"[[BATCH]] {' ; '.join(_format_command(command, base_command))}".encode())
     else:
         nb_cmds = 1
         ctl_writer.write(f"/{base_command} {command}".encode())
     await ctl_writer.drain()
     resp = await ctl_reader.read(100)
     ctl_writer.close()
     await ctl_writer.wait_closed()
     r: bool = resp == b"ok" * nb_cmds
     if not r:
         logger.error("FAILED %s", resp)
     return r
 
 
-async def get_focused_monitor_props(logger=None, name=None) -> dict[str, Any]:
-    """Returns focused monitor data if `name` is not defined, else use monitor's name
+async def get_focused_monitor_props(logger: Logger | None = None, name: str | None = None) -> MonitorInfo:
+    """Return focused monitor data if `name` is not defined, else use monitor's name.
 
     Args:
         logger: logger to use in case of error
-        name [optional]: monitor name
+        name: (optional) monitor name
 
     Returns:
-
         dict() with the focused monitor properties
     """
     if name:
 
-        def match_fn(mon):
+        def match_fn(mon: MonitorInfo) -> bool:
             return mon["name"] == name
 
     else:
 
-        def match_fn(mon):
-            return mon.get("focused")
+        def match_fn(mon: MonitorInfo) -> bool:
+            return cast(bool, mon.get("focused"))
 
-    for monitor in await hyprctlJSON("monitors", logger=logger):
-        assert isinstance(monitor, dict)
-        if match_fn(monitor):
-            return monitor
-    raise RuntimeError("no focused monitor")
+    for monitor in await hyprctl_json("monitors", logger=logger):
+        if match_fn(cast(MonitorInfo, monitor)):
+            return monitor  # type: ignore
+    msg = "no focused monitor"
+    raise RuntimeError(msg)
 
 
-async def get_client_props(logger=None, match_fn=None, **kw):
-    """
-    Returns the properties of a client that matches the given `match_fn` (or default to equality) given the keyword arguments
+async def get_client_props(
+    logger: Logger | None = None, match_fn: Callable | None = None, clients: list[ClientInfo] | None = None, **kw
+) -> ClientInfo | None:
+    """Return the properties of a client that matches the given `match_fn` (or default to equality) given the keyword arguments.
 
     Eg.
         # will return the properties of the client with address "0x1234"
         get_client_props(logger, addr="0x1234")
 
         # will return the properties of the client with initialClass containing "fooBar"
         get_client_props(logger, match_fn=lambda x, y: y in x), initialClass="fooBar")
 
     Args:
-
         logger: logger to use in case of error
         match_fn: function to match the client properties, takes 2 arguments (client_value, config_value)
+        clients: list of clients to search in
+        kw: keyword arguments to match the client properties
 
         Any other keyword argument will be used to match the client properties. Only one keyword argument is allowed.
         `addr` aliases `address` and `cls` aliases `class`
 
         Note: the address of the client must include the "0x" prefix
     """
     assert kw
 
     addr = kw.get("addr")
     klass = kw.get("cls")
 
     if addr:
-        assert len(addr) > 2, "Client address is invalid"
+        assert len(addr) > MINIMUM_ADDR_LEN, "Client address is invalid"
         prop_name = "address"
         prop_value = addr
     elif klass:
         prop_name = "class"
         prop_value = klass
     else:
         prop_name, prop_value = next(iter(kw.items()))
 
     if match_fn is None:
 
-        def match_fn(value1, value2):
-            return value1 == value2
+        def match_fn(value1: Any, value2: Any) -> bool:  # noqa: ANN401
+            return bool(value1 == value2)
 
-    for client in await hyprctlJSON("clients", logger=logger):
+    for client in clients or await hyprctl_json("clients", logger=logger):
         assert isinstance(client, dict)
         if match_fn(client.get(prop_name), prop_value):
-            return client
+            return client  # type: ignore
+    return None
 
 
-def init():
-    "initialize logging"
+def init() -> None:
+    """Initialize logging."""
     global log
     log = get_logger("ipc")
 
 
-def getCtrlObjects(logger):
-    "Returns (hyprctl, hyprctlJSON, notify) configured for the given logger"
+def get_controls(logger: Logger) -> tuple[Callable, Callable, Callable, Callable, Callable]:
+    """Return (hyprctl, hyprctl_json, notify) configured for the given logger."""
     return (
         partial(hyprctl, logger=logger),
-        partial(hyprctlJSON, logger=logger),
+        partial(hyprctl_json, logger=logger),
         partial(notify, logger=logger),
         partial(notify_info, logger=logger),
         partial(notify_error, logger=logger),
     )
```

### Comparing `pyprland-2.2.9/pyprland/plugins/expose.py` & `pyprland-2.3.0/pyprland/plugins/expose.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,41 @@
-""" expose Brings every client window to screen for selection
-"""
+"""expose Brings every client window to screen for selection."""
 
+from ..common import CastBoolMixin, state
+from ..types import ClientInfo
 from .interface import Plugin
-from ..common import state, CastBoolMixin
 
 
 class Extension(CastBoolMixin, Plugin):  # pylint: disable=missing-class-docstring
-    exposed: list[dict] = []
+    """Expose all clients on the active workspace."""
+
+    exposed: list[ClientInfo] = []
 
     @property
-    def exposed_clients(self):
-        "Returns the list of clients currently using exposed mode"
+    def exposed_clients(self) -> list[ClientInfo]:
+        """Returns the list of clients currently using exposed mode."""
         if self.cast_bool(self.config.get("include_special"), False):
             return self.exposed
         return [c for c in self.exposed if c["workspace"]["id"] > 0]
 
-    async def run_expose(self):
+    async def run_expose(self) -> None:
         """Expose every client on the active workspace.
-        If expose is active restores everything and move to the focused window"""
+
+        If expose is active restores everything and move to the focused window
+        """
         if self.exposed:
-            commands = []
-            for client in self.exposed_clients:
-                commands.append(
-                    f"movetoworkspacesilent {client['workspace']['id']},address:{client['address']}"
-                )
+            commands = [f"movetoworkspacesilent {client['workspace']['id']},address:{client['address']}" for client in self.exposed_clients]
             commands.extend(
-                [
+                (
                     "togglespecialworkspace exposed",
                     f"focuswindow address:{state.active_window}",
-                ]
+                )
             )
             await self.hyprctl(commands)
             self.exposed = []
         else:
             self.exposed = await self.get_clients(workspace_bl=state.active_workspace)
             commands = []
             for client in self.exposed_clients:
-                commands.append(
-                    f"movetoworkspacesilent special:exposed,address:{client['address']}"
-                )
+                commands.append(f"movetoworkspacesilent special:exposed,address:{client['address']}")
             commands.append("togglespecialworkspace exposed")
             await self.hyprctl(commands)
```

### Comparing `pyprland-2.2.9/pyprland/plugins/fetch_client_menu.py` & `pyprland-2.3.0/pyprland/plugins/fetch_client_menu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,39 @@
-" Select a client window and move it to the active workspace"
+"""Select a client window and move it to the active workspace."""
 
-from .interface import Plugin
 from ..adapters.menus import MenuMixin
 from ..common import state
+from .interface import Plugin
 
 
 class Extension(MenuMixin, Plugin):
-    "Shows a menu with shortcuts"
+    """Shows a menu with shortcuts."""
 
     _windows_origins: dict[str, str] = {}
 
     # Commands
 
-    async def run_unfetch_client(self):
-        "Returns a window back to its origin"
+    async def run_unfetch_client(self) -> None:
+        """Return a window back to its origin."""
         addr = state.active_window
         try:
             origin = self._windows_origins[addr]
         except KeyError:
             await self.notify_error("unknown window origin")
         else:
             await self.hyprctl(f"movetoworkspacesilent {origin},address:{addr}")
 
-    async def run_fetch_client_menu(self):
-        "Select a client window and move it to the active workspace"
+    async def run_fetch_client_menu(self) -> None:
+        """Select a client window and move it to the active workspace."""
         await self.ensure_menu_configured()
 
         clients = await self.get_clients(workspace_bl=state.active_workspace)
 
         separator = self.config.get("separator", "|")
 
-        choice = await self.menu.run(
-            [f"{i+1} {separator} {c['title']}" for i, c in enumerate(clients)]
-        )
+        choice = await self.menu.run([f"{i + 1} {separator} {c['title']}" for i, c in enumerate(clients)])
 
         if choice:
             num = int(choice.split(None, 1)[0]) - 1
             addr = clients[num]["address"]
             self._windows_origins[addr] = clients[num]["workspace"]["name"]
-            await self.hyprctl(
-                f"movetoworkspace {state.active_workspace},address:{addr}"
-            )
+            await self.hyprctl(f"movetoworkspace {state.active_workspace},address:{addr}")
```

### Comparing `pyprland-2.2.9/pyprland/plugins/gbar.py` & `pyprland-2.3.0/pyprland/plugins/gbar.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,81 @@
-" Run gbar on the first available display from a list of displays"
+"""Run gbar on the first available display from a list of displays."""
 
 import asyncio
+import contextlib
 
-from .interface import Plugin
 from ..common import state
+from .interface import Plugin
 
 
 class Extension(Plugin):
-    "Manage gBar application"
+    """Manage gBar application."""
+
     monitors: set[str]
     proc = None
-    cur_monitor = ""
+    cur_monitor: str | None = ""
+
+    ongoing_task: asyncio.Task | None = None
+
+    def _run_gbar(self, cmd: str) -> None:
+        """Create ongoing task restarting gbar in case of crash."""
+
+        async def _run_loop() -> None:
+            while True:
+                self.proc = await asyncio.create_subprocess_shell(cmd)
+                await self.proc.wait()
+                self.notify_error("gBar crashed, restarting")
+
+        if self.ongoing_task:
+            self.ongoing_task.cancel()
+        self.ongoing_task = asyncio.create_task(_run_loop())
 
-    async def run_gbar(self, args):
-        "Starts gBar on the first available monitor"
+    async def run_gbar(self, args: str) -> None:
+        """Start gBar on the first available monitor."""
         if args.startswith("re"):
             self.kill()
             await self.on_reload()
 
-    async def on_reload(self):
-        "Initializes if not done"
+    async def on_reload(self) -> None:
+        """Initialize if not done."""
         if not self.proc:
             self.cur_monitor = await self.get_best_monitor()
             if not self.cur_monitor:
                 first_mon = next(iter(state.monitors))
-                await self.notify_info(
-                    f"gBar: No preferred monitor found, using {first_mon}"
-                )
+                await self.notify_info(f"gBar: No preferred monitor found, using {first_mon}")
                 cmd = f"gBar bar {first_mon}"
             else:
                 cmd = f"gBar bar {self.cur_monitor}"
             self.log.info("starting gBar: %s", cmd)
-            self.proc = await asyncio.create_subprocess_shell(cmd)
+            self._run_gbar(cmd)
 
-    async def get_best_monitor(self):
-        "get best monitor according to preferred list"
-        preferred = self.config.get("monitors", [])
+    async def get_best_monitor(self) -> str:
+        """Get best monitor according to preferred list."""
+        preferred: list[str] = self.config.get("monitors", [])
         for monitor in preferred:
             if monitor in state.monitors:
                 return monitor
+        return ""
 
-    async def event_monitoradded(self, monitor):
-        "Switch bar in case the monitor is preferred"
+    async def event_monitoradded(self, monitor: str) -> None:
+        """Switch bar in case the monitor is preferred."""
         if self.cur_monitor:
             preferred = self.config.get("monitors", [])
             cur_idx = preferred.index(self.cur_monitor) if self.cur_monitor else 999
             new_idx = preferred.index(monitor)
             if 0 <= new_idx < cur_idx:
                 self.kill()
                 await self.on_reload()
 
-    async def exit(self):
-        "Kill the process"
+    async def exit(self) -> None:
+        """Kill the process."""
         self.kill()
 
-    def kill(self):
-        "Kill the process"
+    def kill(self) -> None:
+        """Kill the process."""
         if self.proc:
-            try:
+            if self.ongoing_task:
+                self.ongoing_task.cancel()
+                self.ongoing_task = None
+            with contextlib.suppress(ProcessLookupError):
                 self.proc.kill()
-            except ProcessLookupError:
-                pass
             self.proc = None
```

### Comparing `pyprland-2.2.9/pyprland/plugins/interface.py` & `pyprland-2.3.0/pyprland/plugins/interface.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-" Common plugin interface "
-from typing import Any, cast, Callable
+"""Common plugin interface."""
+
+import contextlib
+from collections.abc import Callable
+from typing import Any, cast
 
 from ..common import get_logger
-from ..ipc import getCtrlObjects
+from ..ipc import get_controls
+from ..types import ClientInfo
 
 
 class Plugin:
-    """Base class for any pyprland plugin"""
+    """Base class for any pyprland plugin."""
+
+    aborted = False
 
-    hyprctlJSON: Callable
-    " `pyprland.ipc.hyprctlJSON` using the pluggin's logger "
+    hyprctl_json: Callable
+    " `pyprland.ipc.hyprctl_json` using the pluggin's logger "
 
     hyprctl: Callable
     " `pyprland.ipc.hyprctl` using the pluggin's logger "
 
     notify: Callable
     " `pyprland.ipc.notify` using the pluggin's logger "
 
@@ -22,64 +28,57 @@
 
     notify_error: Callable
     " `pyprland.ipc.notify_error` using the pluggin's logger "
 
     config: dict[str, Any]
     " This plugin configuration section as a dict object "
 
-    def __init__(self, name: str):
-        "create a new plugin `name` and the matching logger"
+    def __init__(self, name: str) -> None:
+        """Create a new plugin `name` and the matching logger."""
         self.name = name
         """ the plugin name """
         self.log = get_logger(name)
         """ the logger to use for this plugin """
-        ctrl = getCtrlObjects(self.log)
+        ctrl = get_controls(self.log)
         (
             self.hyprctl,
-            self.hyprctlJSON,  # pylint: disable=invalid-name
+            self.hyprctl_json,  # pylint: disable=invalid-name
             self.notify,
             self.notify_info,
             self.notify_error,
         ) = ctrl
         self.config = {}
 
     # Functions to override
 
-    async def init(self):
-        """
-        This should contain the code you would normally add to `__init__`.
+    async def init(self) -> None:
+        """Initialize the plugin.
+
         Note that the `config` attribute isn't ready yet when this is called.
         """
 
-    async def on_reload(self):
-        """
-        Add the code which requires the `config` attribute here.
+    async def on_reload(self) -> None:
+        """Add the code which requires the `config` attribute here.
+
         This is called on *init* and *reload*
         """
 
-    async def exit(self):
-        "empty exit function"
+    async def exit(self) -> None:
+        """Empty exit function."""
 
     # Generic implementations
 
-    async def load_config(self, config: dict[str, Any]):
-        "Loads the configuration section from the passed `config`"
+    async def load_config(self, config: dict[str, Any]) -> None:
+        """Load the configuration section from the passed `config`."""
         self.config.clear()
-        try:
+        with contextlib.suppress(KeyError):
             self.config.update(config[self.name])
-        except KeyError:
-            pass
 
-    async def get_clients(self, mapped=True, workspace=None, workspace_bl=None):
-        "Return the client list, optionally returns only mapped clients or from a given workspace"
+    async def get_clients(self, mapped: bool = True, workspace: None | str = None, workspace_bl: str | None = None) -> list[ClientInfo]:
+        """Return the client list, optionally returns only mapped clients or from a given workspace."""
         return [
             client
-            for client in cast(list[dict[str, Any]], await self.hyprctlJSON("clients"))
+            for client in cast(list[ClientInfo], await self.hyprctl_json("clients"))
             if (not mapped or client["mapped"])
-            and (
-                workspace is None or cast(str, client["workspace"]["name"]) == workspace
-            )
-            and (
-                workspace_bl is None
-                or cast(str, client["workspace"]["name"]) != workspace_bl
-            )
+            and (workspace is None or cast(str, client["workspace"]["name"]) == workspace)
+            and (workspace_bl is None or cast(str, client["workspace"]["name"]) != workspace_bl)
         ]
```

### Comparing `pyprland-2.2.9/pyprland/plugins/layout_center.py` & `pyprland-2.3.0/pyprland/plugins/layout_center.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,74 +1,68 @@
-"""
-Implements a "Centered" layout:
+"""Implements a "Centered" layout.
+
 - windows are normally tiled but one
 - the active window is floating and centered
 - you can cycle the active window, keeping the same layout type
 - layout can be toggled any time
 """
 
-from typing import Any, cast
 from collections import defaultdict
+from typing import Any, cast
 
+from ..common import CastBoolMixin, state
+from ..types import ClientInfo
 from .interface import Plugin
-from ..common import state, CastBoolMixin
 
 
 class Extension(CastBoolMixin, Plugin):
-    "Manages a layout with one centered window on top of others"
+    """Manages a layout with one centered window on top of others."""
 
-    workspace_info: dict[str, dict[str, Any]] = defaultdict(
-        lambda: {"enabled": False, "addr": ""}
-    )
+    workspace_info: dict[str, dict[str, Any]] = defaultdict(lambda: {"enabled": False, "addr": ""})
     last_index = 0
 
     # Events
 
-    async def event_openwindow(self, windescr):
-        "Re-set focus to main if a window is opened"
+    async def event_openwindow(self, windescr: str) -> None:
+        """Re-set focus to main if a window is opened."""
         if not self.enabled:
             return
         win_addr = "0x" + windescr.split(",", 1)[0]
         for i, cli in enumerate(await self.get_clients()):
             if cli["address"] == win_addr and not cli["floating"]:
                 await self.hyprctl(f"focuswindow address:{self.main_window_addr}")
                 self.last_index = i
                 break
 
-    async def event_activewindowv2(self, _):
-        "keep track of focused client"
-        if (
-            self.cast_bool(self.config.get("captive_focus"))
-            and self.enabled
-            and state.active_window != self.main_window_addr
-            and len(
-                [
-                    c
-                    for c in await self.get_clients()
-                    if c["address"] == state.active_window
-                ]
-            )
-            > 0
-        ):
-            await self.hyprctl(f"focuswindow address:{self.main_window_addr}")
+    async def event_activewindowv2(self, _: str) -> None:
+        """Keep track of focused client."""
+        captive = self.cast_bool(self.config.get("captive_focus"))
+        is_not_active = state.active_window != self.main_window_addr
+        if captive and self.enabled and is_not_active:
+            try:
+                next(c for c in await self.get_clients() if c["address"] == state.active_window)
+            except StopIteration:
+                pass
+            else:
+                await self.hyprctl(f"focuswindow address:{self.main_window_addr}")
 
-    async def event_closewindow(self, addr):
-        "Disable when the main window is closed"
+    async def event_closewindow(self, addr: str) -> None:
+        """Disable when the main window is closed."""
         addr = "0x" + addr
         clients = [c for c in await self.get_clients() if c["address"] != addr]
         if self.enabled and await self._sanity_check(clients):
             closed_main = self.main_window_addr == addr
             if self.enabled and closed_main:
                 self.log.debug("main window closed, focusing next")
                 await self._run_changefocus(1)
 
     # Command
 
-    async def run_layout_center(self, what):
-        "<toggle|next|prev> turn on/off or change the active window"
+    async def run_layout_center(self, what: str) -> None:
+        """<toggle|next|prev> turn on/off or change the active window."""
         if what == "toggle":
             await self._run_toggle()
         elif what == "next":
             await self._run_changefocus(1, default_override="next")
         elif what == "prev":
             await self._run_changefocus(-1, default_override="prev")
         elif what == "next2":
@@ -76,73 +70,67 @@
         elif what == "prev2":
             await self._run_changefocus(-1, default_override="prev2")
         else:
             await self.notify_error(f"unknown layout_center command: {what}")
 
     # Utils
 
-    async def get_clients(self):  # pylint: disable=arguments-differ
-        "Return the client list in the currently active workspace"
-        clients = await super().get_clients(
-            mapped=True, workspace=state.active_workspace
-        )
+    async def get_clients(self, *_) -> list[ClientInfo]:  # pylint: disable=arguments-differ
+        """Return the client list in the currently active workspace."""
+        clients = await super().get_clients(mapped=True, workspace=state.active_workspace)
         clients.sort(key=lambda c: c["address"])
         return clients
 
-    async def unprepare_window(self, clients=None):
-        "Set the window as normal"
+    async def unprepare_window(self, clients: list[ClientInfo] | None = None) -> None:
+        """Set the window as normal."""
         if not clients:
             clients = await self.get_clients()
         addr = self.main_window_addr
         for cli in clients:
             if cli["address"] == addr and cli["floating"]:
                 await self.hyprctl(f"togglefloating address:{addr}")
 
-    async def prepare_window(self, clients=None):
-        "Set the window as centered"
+    async def prepare_window(self, clients: list[ClientInfo] | None = None) -> None:
+        """Set the window as centered."""
         if not clients:
             clients = await self.get_clients()
         addr = self.main_window_addr
         for cli in clients:
             if cli["address"] == addr and not cli["floating"]:
                 await self.hyprctl(f"togglefloating address:{addr}")
         width = 100
         height = 100
         x, y = self.offset
         margin = self.margin
         scale = 1
-        for monitor in cast(list[dict[str, Any]], await self.hyprctlJSON("monitors")):
+        for monitor in cast(list[dict[str, Any]], await self.hyprctl_json("monitors")):
             scale = monitor["scale"]
             if monitor["focused"]:
                 width = monitor["width"] - (2 * margin)
                 height = monitor["height"] - (2 * margin)
                 x += monitor["x"] + margin
                 y += monitor["y"] + margin
                 break
-        await self.hyprctl(
-            f"resizewindowpixel exact {int(width/scale)} {int(height/scale)},address:{addr}"
-        )
-        await self.hyprctl(
-            f"movewindowpixel exact {int(x/scale)} {int(y/scale)},address:{addr}"
-        )
+        await self.hyprctl(f"resizewindowpixel exact {int(width / scale)} {int(height / scale)},address:{addr}")
+        await self.hyprctl(f"movewindowpixel exact {int(x / scale)} {int(y / scale)},address:{addr}")
 
     # Subcommands
 
-    async def _sanity_check(self, clients=None):
-        "Auto-disable if needed & return enabled status"
+    async def _sanity_check(self, clients: list[ClientInfo] | None = None) -> bool:
+        """Auto-disable if needed & return enabled status."""
         clients = clients or await self.get_clients()
-        if len(clients) < 2:
+        if len(clients) < 2:  # noqa: PLR2004
             # If < 2 clients, disable the layout & stop
             self.log.info("disabling (clients starvation)")
             await self.unprepare_window()
             self.enabled = False
         return self.enabled
 
-    async def _run_changefocus(self, direction, default_override=None):
-        "Change the focus in the given direction (-1 or 1)"
+    async def _run_changefocus(self, direction: int, default_override: str | None = None) -> None:
+        """Change the focus in the given direction (-1 or 1)."""
         if self.enabled:
             clients = await self.get_clients()
             if await self._sanity_check(clients):
                 addresses = [c["address"] for c in clients]
                 try:
                     idx = addresses.index(self.main_window_addr)
                 except ValueError:
@@ -154,68 +142,61 @@
                     index = 0
                 new_client = clients[index]
                 await self.unprepare_window(clients)
                 self.main_window_addr = new_client["address"]
                 await self.hyprctl(f"focuswindow address:{self.main_window_addr}")
                 self.last_index = index
                 await self.prepare_window(clients)
-        else:
+        elif default_override:
             command = self.config.get(default_override)
             if command:
                 await self.hyprctl(command)
 
-    async def _run_toggle(self):
-        "toggle the center layout"
+    async def _run_toggle(self) -> None:
+        """Toggle the center layout."""
         disabled = not self.enabled
         if disabled:
             self.main_window_addr = state.active_window
             await self.prepare_window()
         else:
             await self.unprepare_window()
 
         self.enabled = disabled
 
     # Properties
 
     @property
-    def offset(self):
-        "Returns the centered window offset"
-        offset = self.config.get("offset", [0, 0])
+    def offset(self) -> tuple[int, int]:
+        """Returns the centered window offset."""
+        offset = self.config.get("offset", (0, 0))
         if isinstance(offset, str):
             x, y = (int(i) for i in self.config["offset"].split() if i.strip())
-            return [x, y]
-        return offset
+            return (x, y)
+        return cast(tuple[int, int], offset)
 
     @property
-    def margin(self):
-        "Returns the margin of the centered window"
-        return self.config.get("margin", 60)
+    def margin(self) -> int:
+        """Returns the margin of the centered window."""
+        return cast(int, self.config.get("margin", 60))
 
     # enabled
-    def get_enabled(self):
-        "Is center layout enabled on the active workspace ?"
-        return self.workspace_info[state.active_workspace]["enabled"]
-
-    def set_enabled(self, value):
-        "set if center layout enabled on the active workspace"
+    @property
+    def enabled(self) -> bool:
+        """Is center layout enabled on the active workspace ?."""
+        return cast(bool, self.workspace_info[state.active_workspace]["enabled"])
+
+    @enabled.setter
+    def enabled(self, value: bool) -> None:
+        """Set if center layout enabled on the active workspace."""
         self.workspace_info[state.active_workspace]["enabled"] = value
 
-    enabled = property(
-        get_enabled, set_enabled, doc="centered layout enabled on this workspace"
-    )
-    del get_enabled, set_enabled
-
     # main_window_addr
-    def get_main_window_addr(self):
-        "get active workspace's centered window address"
-        return self.workspace_info[state.active_workspace]["addr"]
 
-    def set_main_window_addr(self, value):
-        "set active workspace's centered window address"
+    @property
+    def main_window_addr(self) -> str:
+        """Get active workspace's centered window address."""
+        return cast(str, self.workspace_info[state.active_workspace]["addr"])
+
+    @main_window_addr.setter
+    def main_window_addr(self, value: str) -> None:
+        """Set active workspace's centered window address."""
         self.workspace_info[state.active_workspace]["addr"] = value
-
-    main_window_addr = property(
-        get_main_window_addr,
-        set_main_window_addr,
-        doc="active workspace's centered window address",
-    )
-    del get_main_window_addr, set_main_window_addr
```

### Comparing `pyprland-2.2.9/pyprland/plugins/lost_windows.py` & `pyprland-2.3.0/pyprland/plugins/lost_windows.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,31 @@
-" Moves unreachable client windows to the currently focused workspace"
+"""Moves unreachable client windows to the currently focused workspace."""
+
 from typing import Any, cast
 
+from ..types import ClientInfo, MonitorInfo
 from .interface import Plugin
 
 
-def contains(monitor, window):
-    "Tell if a window is visible in a monitor"
-    if not (
-        window["at"][0] > monitor["x"]
-        and window["at"][0] < monitor["x"] + monitor["width"]
-    ):
-        return False
-    if not (
-        window["at"][1] > monitor["y"]
-        and window["at"][1] < monitor["y"] + monitor["height"]
-    ):
+def contains(monitor: MonitorInfo, window: ClientInfo) -> bool:
+    """Tell if a window is visible in a monitor."""
+    if not (window["at"][0] > monitor["x"] and window["at"][0] < monitor["x"] + monitor["width"]):
         return False
-    return True
+    return bool(window["at"][1] > monitor["y"] and window["at"][1] < monitor["y"] + monitor["height"])
 
 
 class Extension(Plugin):  # pylint: disable=missing-class-docstring
-    async def run_attract_lost(self):
-        """Brings lost floating windows to the current workspace"""
-        monitors = cast(list, await self.hyprctlJSON("monitors"))
+    """Moves unreachable client windows to the currently focused workspace."""
+
+    async def run_attract_lost(self) -> None:
+        """Brings lost floating windows to the current workspace."""
+        monitors = cast(list, await self.hyprctl_json("monitors"))
         windows = cast(list, await self.get_clients())
-        lost = [
-            win
-            for win in windows
-            if win["floating"] and not any(contains(mon, win) for mon in monitors)
-        ]
-        focused: dict[str, Any] = [mon for mon in monitors if mon["focused"]][0]
+        lost = [win for win in windows if win["floating"] and not any(contains(mon, win) for mon in monitors)]
+        focused: dict[str, Any] = next(mon for mon in monitors if mon["focused"])
         interval = focused["width"] / (1 + len(lost))
         interval_y = focused["height"] / (1 + len(lost))
         batch = []
         workspace: int = focused["activeWorkspace"]["id"]
         margin = interval // 2
         margin_y = interval_y // 2
         for i, window in enumerate(lost):
```

### Comparing `pyprland-2.2.9/pyprland/plugins/magnify.py` & `pyprland-2.3.0/pyprland/plugins/magnify.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,71 @@
-" Toggles workspace zooming "
+"""Toggles workspace zooming."""
+
 import asyncio
+from collections.abc import Iterable
 
 from .interface import Plugin
 
 
 class Extension(Plugin):  # pylint: disable=missing-class-docstring
+    """Control workspace zooming."""
+
     zoomed = False
 
-    cur_factor = 1
+    cur_factor = 1.0
 
-    def ease_out_quad(self, step, start, end, duration):
+    def ease_out_quad(self, step: int, start: int, end: int, duration: int) -> int:
         """Easing function for animations."""
-        step /= duration
+        step //= duration
         return -end * step * (step - 2) + start
 
-    def animated_eased_zoom(self, start, end, duration):
-        """Helper function to animate zoom"""
+    def animated_eased_zoom(self, start: int, end: int, duration: int) -> Iterable[int]:
+        """Add easing to an animation.
+
+        This function is a generator that yields the next value of the animation
+
+        Args:
+            start (float): starting value
+            end (float): ending value
+            duration (int): duration of the animation
+        """
         for i in range(duration):
             yield self.ease_out_quad(i, start, end - start, duration)
 
-    async def run_zoom(self, *args):
-        """[factor] zooms to "factor" or toggles zoom level if factor is ommited"""
+    async def run_zoom(self, *args) -> None:
+        """[factor] zooms to "factor" or toggles zoom level if factor is omitted.
+
+        If factor is omitted, it toggles between the configured zoom level and no zoom.
+        """
         duration = self.config.get("duration", 15)
         animated = bool(duration)
         prev_factor = self.cur_factor
+        expo = False
         if args:  # set or update the factor
             relative = args[0][0] in "+-"
-            value = int(args[0])
+            expo = args[0][1] in "+-"
+            value = float(args[0][1:]) if expo else float(args[0])
 
             # compute the factor
             if relative:
                 self.cur_factor += value
             else:
                 self.cur_factor = value
 
             # sanity check
             self.cur_factor = max(self.cur_factor, 1)
+        elif self.zoomed:
+            self.cur_factor = 1
         else:
-            if self.zoomed:
-                self.cur_factor = 1
-            else:
-                self.cur_factor = int(self.config.get("factor", 2))
+            self.cur_factor = float(self.config.get("factor", 2.0))
+
+        self.cur_factor = max(self.cur_factor, 1)
 
         if animated:
-            start = prev_factor * 10
-            end = self.cur_factor * 10
+            start = (2.0 ** (prev_factor - 1) if expo else prev_factor) * 10
+            end = (2.0 ** (self.cur_factor - 1) if expo else self.cur_factor) * 10
             for i in self.animated_eased_zoom(start, end, duration):
-                await self.hyprctl(f"misc:cursor_zoom_factor {i/10}", "keyword")
+                await self.hyprctl(f"misc:cursor_zoom_factor {i / 10}", "keyword")
                 await asyncio.sleep(1.0 / 60)
         self.zoomed = self.cur_factor != 1
-        await self.hyprctl(f"misc:cursor_zoom_factor {self.cur_factor}", "keyword")
+        factor = 2 ** (self.cur_factor - 1) if expo else self.cur_factor
+        await self.hyprctl(f"misc:cursor_zoom_factor {factor}", "keyword")
```

### Comparing `pyprland-2.2.9/pyprland/plugins/monitors.py` & `pyprland-2.3.0/pyprland/plugins/monitors.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,162 +1,195 @@
-" The monitors plugin "
+"""The monitors plugin."""
+
 import asyncio
 from collections import defaultdict
 from copy import deepcopy
 from typing import Any, cast
 
+from ..common import CastBoolMixin, is_rotated, state
+from ..types import MonitorInfo
 from .interface import Plugin
-from ..common import CastBoolMixin
 
 
-def trim_offset(monitors):
-    "Makes the monitor set layout start at 0,0"
+def trim_offset(monitors: list[MonitorInfo]) -> None:
+    """Make the monitor set layout start at 0,0."""
     off_x = None
     off_y = None
     for mon in monitors:
         if off_x is None:
             off_x = mon["x"]
 
         if off_y is None:
             off_y = mon["y"]
 
         off_x = min(mon["x"], off_x)
         off_y = min(mon["y"], off_y)
 
+    assert off_x is not None
+    assert off_y is not None
+
     for mon in monitors:
         mon["x"] -= off_x
         mon["y"] -= off_y
 
 
-def clean_pos(position):
-    "Harmonize position format"
+def clean_pos(position: str) -> str:
+    """Harmonize position format."""
     return position.lower().replace("_", "").replace("-", "")
 
 
-def get_XY(place, main_mon, other_mon):
-    """Get the XY position of a monitor according to another (after `place` is applied)
+def scale_and_rotate_mon(monitor: MonitorInfo) -> tuple[int, int]:
+    """Scale and rotate the monitor dimensions."""
+    width = int(monitor["width"] / monitor["scale"])
+    height = int(monitor["height"] / monitor["scale"])
+    if is_rotated(monitor):
+        width, height = height, width
+    return width, height
+
+
+def get_xy(place: str, main_mon: MonitorInfo, other_mon: MonitorInfo) -> tuple[int, int]:
+    """Get the XY position of a monitor according to another (after `place` is applied).
+
     Place syntax: "<top|left|bottom|right> [center|middle|end] of" (without spaces)
     """
-    align_x = False
-    scaled_m_w = int(main_mon["width"] / main_mon["scale"])
-    scaled_m_h = int(main_mon["height"] / main_mon["scale"])
-    scaled_om_w = int(other_mon["width"] / other_mon["scale"])
-    scaled_om_h = int(other_mon["height"] / other_mon["scale"])
-    if place.startswith("top"):
-        x = other_mon["x"]
-        y = other_mon["y"] - scaled_m_h
+    align_x = False  # if alignment is on X axis, else on Y axis
+    scaled_m_w, scaled_m_h = scale_and_rotate_mon(main_mon)
+    scaled_om_w, scaled_om_h = scale_and_rotate_mon(other_mon)
+
+    if place[0] in ("t", "b"):  # top or bottom
         align_x = True
-    elif place.startswith("bottom"):
         x = other_mon["x"]
-        y = other_mon["y"] + scaled_om_h
-        align_x = True
-    elif place.startswith("left"):
-        x = other_mon["x"] - scaled_m_w
-        y = other_mon["y"]
-    elif place.startswith("right"):
-        x = other_mon["x"] + scaled_om_w
+        y = other_mon["y"] - scaled_m_h if place[0] == "t" else other_mon["y"] + scaled_om_h
+    else:  # left or right
         y = other_mon["y"]
-    else:
-        return None
+        x = other_mon["x"] - scaled_m_w if place[0] == "l" else other_mon["x"] + scaled_om_w
 
     centered = "middle" in place or "center" in place
 
     if align_x:
         if centered:
             x += int((scaled_om_w - scaled_m_w) / 2)
         elif "end" in place:
             x += int(scaled_om_w - scaled_m_w)
-    else:
-        if centered:
-            y += int((scaled_om_h - scaled_m_h) / 2)
-        elif "end" in place:
-            y += scaled_m_h - scaled_om_h
+    elif centered:
+        y += int((scaled_om_h - scaled_m_h) / 2)
+    elif "end" in place:
+        y += scaled_m_h - scaled_om_h
+
     return (x, y)
 
 
-def build_graph(config):
-    "make a sorted graph based on the cleaned_config"
+def build_graph(config: dict[str, dict[str, list[str]]]) -> dict[str, list[str]]:
+    """Make a sorted graph based on the cleaned_config."""
     graph = defaultdict(list)
     for name1, positions in config.items():
         for pos, names in positions.items():
-            tldr_direction = pos.startswith("left") or pos.startswith("top")
+            tldr_direction = pos.startswith(("left", "top"))
             for name2 in names:
                 if tldr_direction:
                     graph[name1].append(name2)
                 else:
                     graph[name2].append(name1)
     return graph
 
 
 class Extension(CastBoolMixin, Plugin):  # pylint: disable=missing-class-docstring
-    _mon_by_pat_cache: dict[str, dict] = {}
+    """Control monitors layout."""
+
+    _mon_by_pat_cache: dict[str, MonitorInfo] = {}
 
-    async def on_reload(self):
+    async def on_reload(self) -> None:
+        """Reload the plugin."""
         self._clear_mon_by_pat_cache()
+        monitors = await self.hyprctl_json("monitors")
         if self.cast_bool(self.config.get("startup_relayout"), True):
-            await self.run_relayout()
+            await self.run_relayout(monitors)
 
-    # Command
+        for mon in state.monitors:
+            await self._hotplug_command(name=mon, monitors=monitors)
 
-    async def run_relayout(
-        self,
-    ):
-        "Recompute & apply every monitors's layout"
+    # Command
 
+    async def run_relayout(self, monitors: list[MonitorInfo] | None = None) -> bool:
+        """Recompute & apply every monitors's layout."""
         self._clear_mon_by_pat_cache()
 
-        monitors = cast(list[dict], await self.hyprctlJSON("monitors"))
+        if monitors is None:
+            monitors = cast(list[MonitorInfo], await self.hyprctl_json("monitors"))
 
         cleaned_config = self.resolve_names(monitors)
         if cleaned_config:
             self.log.debug("Using %s", cleaned_config)
         else:
             self.log.debug("No configuration item is applicable")
         graph = build_graph(cleaned_config)
         need_change = self._update_positions(monitors, graph, cleaned_config)
-        every_monitor = {v["name"]: v for v in await self.hyprctlJSON("monitors all")}
+        every_monitor = {v["name"]: v for v in await self.hyprctl_json("monitors all")}
         if need_change:
             trim_offset(monitors)
 
             for monitor in sorted(monitors, key=lambda x: x["x"] + x["y"]):
                 name = monitor["name"]
                 this_mon = every_monitor[name]
                 resolution = f"{this_mon['width']}x{this_mon['height']}@{this_mon['refreshRate']}"
                 scale = this_mon["scale"]
                 position = f"{monitor['x']}x{monitor['y']}"
+                transform = this_mon["transform"]
 
                 await self.hyprctl(
-                    f"monitor {name},{resolution},{position},{scale}", "keyword"
+                    f"monitor {name},{resolution},{position},{scale},transform,{transform}",
+                    "keyword",
                 )
+            return True
+        return False
 
     # Event handlers
 
-    async def event_monitoradded(self, _) -> None:
-        "Triggers when a monitor is plugged"
+    async def event_monitoradded(self, name: str) -> None:
+        """Triggers when a monitor is plugged."""
         await asyncio.sleep(self.config.get("new_monitor_delay", 1.0))
-        await self.run_relayout()
+        monitors = await self.hyprctl_json("monitors")
+        await self._hotplug_command(monitors, name)
+
+        if not await self.run_relayout(monitors):
+            default_command = self.config.get("unknown")
+            if default_command:
+                await asyncio.create_subprocess_shell(default_command)
 
     # Utils
 
-    def _clear_mon_by_pat_cache(self):
-        "clear the cache"
-        self._mon_by_pat_cache = {}
+    async def _hotplug_command(self, monitors: list[MonitorInfo], name: str) -> None:
+        """Run the hotplug command for the monitor."""
+        monitors_by_descr = {m["description"]: m for m in monitors}
+        monitors_by_name = {m["name"]: m for m in monitors}
+        for descr, command in self.config.get("hotplug_commands", {}).items():
+            mon = self._get_mon_by_pat(descr, monitors_by_descr, monitors_by_name)
+            if mon and mon["name"] == name:
+                await asyncio.create_subprocess_shell(command)
+                break
+        single_command = self.config.get("hotplug_command")
+        if single_command:
+            await asyncio.create_subprocess_shell(single_command)
+
+    def _clear_mon_by_pat_cache(self) -> None:
+        """Clear the cache."""
+        self._mon_by_pat_cache: dict[str, MonitorInfo] = {}
 
-    def _get_mon_by_pat(self, pat, description_db, name_db):
-        """Returns a (plugged) monitor object given its pattern or none if not found"""
+    def _get_mon_by_pat(self, pat: str, description_db: dict[str, MonitorInfo], name_db: dict[str, MonitorInfo]) -> MonitorInfo | None:
+        """Return a (plugged) monitor object given its pattern or none if not found."""
         cached = self._mon_by_pat_cache.get(pat)
         if cached is None:
             cached = name_db.get(pat)
             if cached is None:
                 for full_descr in description_db:
                     if pat in full_descr:
                         cached = description_db[full_descr]
                         break
             if cached:
-                self._mon_by_pat_cache[pat] = cast(dict[str, dict], cached)
+                self._mon_by_pat_cache[pat] = cached
         return cached
 
     _flipped_positions = {
         "topof": "bottomof",
         "bottomof": "topof",
         "leftof": "rightof",
         "rightof": "leftof",
@@ -170,73 +203,84 @@
         "rightcenterof": "leftcenterof",
         "topendof": "bottomendof",
         "bottomendof": "topendof",
         "leftendof": "rightendof",
         "rightendof": "leftendof",
     }
 
-    def _update_positions(self, monitors, graph, config):
-        "Apply configuration to monitors_by_name using graph"
+    def _update_positions(self, monitors: list[MonitorInfo], graph: dict[str, list[str]], config: dict[str, dict[str, list[str]]]) -> bool:
+        """Apply configuration to monitors_by_name using graph."""
         monitors_by_name = {m["name"]: m for m in monitors}
         requires_update = False
         for _ in range(len(monitors_by_name) ** 2):
             changed = False
             for name in reversed(graph):
                 mon1 = monitors_by_name[name]
                 for name2 in graph[name]:
                     mon2 = monitors_by_name[name2]
                     for pos, _ in self.get_matching_config(name, name2, config):
-                        x, y = get_XY(self._flipped_positions[pos], mon2, mon1)
+                        try:
+                            x, y = get_xy(self._flipped_positions[pos.lower()], mon2, mon1)
+                        except TypeError:
+                            self.log.exception("Invalid position %s", pos)
+                            continue
                         if x != mon2["x"]:
                             changed = True
                             requires_update = True
                             mon2["x"] = x
                         if y != mon2["y"]:
                             changed = True
                             requires_update = True
                             mon2["y"] = y
             if not changed:
                 break
         return requires_update
 
-    def get_matching_config(self, name1, name2, config):
-        "Returns rules matching name1 or name2 (relative to name1), looking up config"
+    def get_matching_config(self, name1: str, name2: str, config: dict[str, dict[str, list[str]]]) -> list[tuple[str, str]]:
+        """Return rules matching name1 or name2 (relative to name1), looking up config.
+
+        Returns a list of tuples (position, name) where name is the other monitor's name.
+        """
         results = []
-        ref_set = set((name1, name2))
+        ref_set = {name1, name2}
         for name_a, positions in config.items():
             for pos, names in positions.items():
                 lpos = clean_pos(pos)
                 for name_b in names:
-                    if set((name_a, name_b)) == ref_set:
+                    if {name_a, name_b} == ref_set:
                         if name_a == name1:
                             results.append((lpos, name_b))
                         else:
                             results.append((self._flipped_positions[lpos], name_a))
         return results
 
-    def resolve_names(self, monitors):
-        "change partial descriptions used in config for monitor names"
+    def resolve_names(self, monitors: list[MonitorInfo]) -> dict[str, Any]:
+        """Change partial descriptions used in config for monitor names.
+
+        Args:
+            monitors: list of plugged monitors
+        Returns:
+            dict: cleaned config
+        """
         placement_rules = deepcopy(self.config.get("placement", {}))
         monitors_by_descr = {m["description"]: m for m in monitors}
         cleaned_config: dict[str, dict[str, Any]] = {}
         plugged_monitors = {m["name"]: m for m in monitors}
         for descr1, placement in placement_rules.items():
             mon = self._get_mon_by_pat(descr1, monitors_by_descr, plugged_monitors)
             if not mon:
                 continue
             name = mon["name"]
             if name not in plugged_monitors:
                 continue
             cleaned_config[name] = {}
             for position, descr_list in placement.items():
                 if isinstance(descr_list, str):
-                    descr_list = [descr_list]
+                    descr_list = [descr_list]  # noqa: PLW2901
                 resolved = []
                 for p in descr_list:
                     r = self._get_mon_by_pat(p, monitors_by_descr, plugged_monitors)
                     if r:
                         resolved.append(r["name"])
                 if resolved:
-                    cleaned_config[name][clean_pos(position)] = [
-                        r for r in resolved if r in plugged_monitors
-                    ]
+                    cleaned_config[name][clean_pos(position)] = [r for r in resolved if r in plugged_monitors]
         return cleaned_config
```

### Comparing `pyprland-2.2.9/pyprland/plugins/monitors_v0.py` & `pyprland-2.3.0/pyprland/plugins/monitors_v0.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # pylint: disable=duplicate-code
-" The monitors plugin "
+"The monitors plugin"
+
 import asyncio
 import subprocess
 from typing import Any, cast
 
 from .interface import Plugin
 
 
@@ -19,49 +20,41 @@
     other_monitors = [mon for mon in monitors if mon["name"] != screenid]
     for mon in other_monitors:
         min_x = min(min_x, mon["x"])
         min_y = min(min_y, mon["y"])
     x_offset = -min_x
     y_offset = -min_y
     for mon in other_monitors:
-        command.extend(
-            [
-                "--output",
-                mon["name"],
-                "--pos",
-                f"{mon['x']+x_offset},{mon['y']+y_offset}",
-            ]
-        )
-
-    command.extend(
-        ["--output", screenid, "--pos", f"{pos_x+x_offset},{pos_y+y_offset}"]
-    )
+        command.extend([
+            "--output",
+            mon["name"],
+            "--pos",
+            f"{mon['x'] + x_offset},{mon['y'] + y_offset}",
+        ])
+
+    command.extend(["--output", screenid, "--pos", f"{pos_x + x_offset},{pos_y + y_offset}"])
     subprocess.call(command)
 
 
 class Extension(Plugin):  # pylint: disable=missing-class-docstring
     async def load_config(self, config) -> None:
         await super().load_config(config)
         await self.run_relayout()
 
     async def run_relayout(self):
         "Recompute & apply every monitors's layout"
-        monitors = cast(list[dict], await self.hyprctlJSON("monitors"))
+        monitors = cast(list[dict], await self.hyprctl_json("monitors"))
         for monitor in monitors:
-            await self.event_monitoradded(
-                monitor["name"], no_default=True, monitors=monitors
-            )
-
-    async def event_monitoradded(
-        self, monitor_name, no_default=False, monitors: list | None = None
-    ) -> None:
+            await self.event_monitoradded(monitor["name"], no_default=True, monitors=monitors)
+
+    async def event_monitoradded(self, monitor_name, no_default=False, monitors: list | None = None) -> None:
         "Triggers when a monitor is plugged"
 
         if not monitors:
-            monitors = cast(list, await self.hyprctlJSON("monitors"))
+            monitors = cast(list, await self.hyprctl_json("monitors"))
 
         assert monitors
 
         for mon in monitors:
             if mon["name"].startswith(monitor_name):
                 mon_description = mon["description"]
                 break
@@ -73,17 +66,15 @@
             return
 
         if not no_default:
             default_command = self.config.get("unknown")
             if default_command:
                 await asyncio.create_subprocess_shell(default_command)
 
-    def _place_monitors(
-        self, monitor_name: str, mon_description: str, monitors: list[dict[str, Any]]
-    ):
+    def _place_monitors(self, monitor_name: str, mon_description: str, monitors: list[dict[str, Any]]):
         "place a given monitor according to config"
         mon_by_name = {m["name"]: m for m in monitors}
         newmon = mon_by_name[monitor_name]
         for mon_pattern, conf in self.config["placement"].items():
             if mon_pattern in mon_description:
                 for placement, other_mon_description in conf.items():
                     ref = mon_by_name.get(other_mon_description)
```

### Comparing `pyprland-2.2.9/pyprland/plugins/pyprland.py` & `pyprland-2.3.0/pyprland/plugins/pyprland.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,75 @@
-" Not a real Plugin - provides some core features and some caching of commonly requested structures "
+"""Not a real Plugin - provides some core features and some caching of commonly requested structures."""
+
+import json
+
+from ..common import MINIMUM_ADDR_LEN, state
+from ..types import VersionInfo
 from .interface import Plugin
-from ..common import state, VersionInfo
 
 
 class Extension(Plugin):
-    "Internal built-in plugin allowing caching states and implementing special commands"
+    """Internal built-in plugin allowing caching states and implementing special commands."""
 
-    async def init(self):
-        "initializes the plugin"
+    async def init(self) -> None:
+        """Initialize the plugin."""
         state.active_window = ""
-        version = (await self.hyprctlJSON("version"))["tag"]
         try:
-            state.hyprland_version = VersionInfo(
-                *(int(i) for i in version[1:].split(".")[:3])
-            )
-        except Exception:
-            self.log.error("Fail to parse hyprctl version.")
+            version_info = await self.hyprctl_json("version")
+        except json.JSONDecodeError:
+            self.log.exception("Fail to parse hyprctl version")
+            await self.notify_error("Error: 'hyprctl version': incorrect JSON data")
+            version = "v0.0.0"
+        else:
+            if version_info.get("tag"):
+                version = version_info["tag"].split("-", 1)[0]
+            else:
+                version = "v9.9.9"
+                self.log.warning("No tag available, assuming a recent git version.")
+
+        try:
+            state.hyprland_version = VersionInfo(*(int(i) for i in version[1:].split(".")[:3]))
+        except Exception:  # pylint: disable=broad-except
+            self.log.exception('Fail to parse version tag "%s"', version)
+            await self.notify_error(f"Failed to parse hyprctl version tag: {version}")
+            state.hyprland_version = VersionInfo(0, 0, 0)
 
-        state.active_workspace = (await self.hyprctlJSON("activeworkspace"))["name"]
-        monitors = await self.hyprctlJSON("monitors")
+        state.active_workspace = (await self.hyprctl_json("activeworkspace"))["name"]
+        monitors = await self.hyprctl_json("monitors")
         state.monitors = [mon["name"] for mon in monitors]
         state.active_monitor = next(mon["name"] for mon in monitors if mon["focused"])
 
-    async def event_monitoradded(self, name):
-        "track monitor"
+    async def event_monitoradded(self, name: str) -> None:
+        """Track monitor."""
         state.monitors.append(name)
 
-    async def event_monitorremoved(self, name):
-        "track monitor"
+    async def event_monitorremoved(self, name: str) -> None:
+        """Track monitor."""
         state.monitors.remove(name)
 
-    async def on_reload(self):
+    async def on_reload(self) -> None:
+        """Reload the plugin."""
         state.variables = self.config.get("variables", {})
 
-    async def event_activewindowv2(self, addr):
-        "keep track of focused client"
-        state.active_window = "0x" + addr
-        self.log.debug("active_window = %s", state.active_window)
+    async def event_activewindowv2(self, addr: str) -> None:
+        """Keep track of the focused client."""
+        if not addr or len(addr) < MINIMUM_ADDR_LEN:
+            self.log.warning("Active window is incorrect: %s.", addr)
+            state.active_window = ""
+        else:
+            state.active_window = "0x" + addr
+            self.log.debug("active_window = %s", state.active_window)
 
-    async def event_workspace(self, wrkspace):
-        "track the active workspace"
+    async def event_workspace(self, wrkspace: str) -> None:
+        """Track the active workspace."""
         state.active_workspace = wrkspace
         self.log.debug("active_workspace = %s", state.active_workspace)
 
-    async def event_focusedmon(self, mon):
-        "track the active workspace"
+    async def event_focusedmon(self, mon: str) -> None:
+        """Track the active workspace."""
         state.active_monitor, state.active_workspace = mon.rsplit(",", 1)
         self.log.debug("active_monitor = %s", state.active_monitor)
 
-    def set_commands(self, **cmd_map):
-        "Set some commands, made available as run_`name` methods"
+    def set_commands(self, **cmd_map) -> None:
+        """Set some commands, made available as run_`name` methods."""
         for name, fn in cmd_map.items():
             setattr(self, f"run_{name}", fn)
```

### Comparing `pyprland-2.2.9/pyprland/plugins/scratchpads/__init__.py` & `pyprland-2.3.0/pyprland/plugins/scratchpads/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,92 @@
-" Scratchpads addon "
-import time
+"""Scratchpads addon."""
+
 import asyncio
+import contextlib
+import time
+from dataclasses import dataclass
 from functools import partial
+from typing import cast
 
-from ...ipc import notify_error, get_client_props, get_focused_monitor_props
-from ..interface import Plugin
-from ...common import state, CastBoolMixin, apply_variables
 from ...adapters.units import convert_coords, convert_monitor_dimension
-
+from ...common import MINIMUM_ADDR_LEN, CastBoolMixin, apply_variables, is_rotated, state
+from ...ipc import get_client_props, get_focused_monitor_props, notify_error
+from ...types import ClientInfo, MonitorInfo
+from ..interface import Plugin
 from .animations import Animations
-from .objects import Scratch
+from .helpers import get_active_space_identifier, get_all_space_identifiers, get_match_fn
 from .lookup import ScratchDB
-from .helpers import (
-    get_active_space_identifier,
-    get_all_space_identifiers,
-    get_match_fn,
-)
+from .objects import Scratch
 
 AFTER_SHOW_INHIBITION = 0.3  # 300ms of ignorance after a show
 DEFAULT_MARGIN = 60  # in pixels
-DEFAULT_HIDE_DELAY = 0.2
-DEFAULT_HYSTERESIS = 0.4  # In seconds
+DEFAULT_HIDE_DELAY = 0.2  # in seconds
+DEFAULT_HYSTERESIS = 0.4  # in seconds
+
+
+@dataclass
+class FocusTracker:
+    """Focus tracking object."""
+
+    prev_focused_window: str
+    prev_focused_window_wrkspc: str
+
+    def clear(self) -> None:
+        """Clear the tracking."""
+        self.prev_focused_window = ""
+        self.prev_focused_window_wrkspc = ""
+
+
+def get_animation_type(scratch: Scratch) -> str:
+    """Get the animation type or an empty string if not set."""
+    return (scratch.conf.get("animation") or "").lower()
 
 
 class Extension(CastBoolMixin, Plugin):  # pylint: disable=missing-class-docstring {{{
+    """Scratchpads addon."""
+
     procs: dict[str, asyncio.subprocess.Process] = {}  # pylint: disable=no-member
     scratches = ScratchDB()
 
-    focused_window_tracking: dict[str, str] = {}
-
     workspace = ""  # Currently active workspace
     monitor = ""  # Currently active monitor
 
     _hysteresis_tasks: dict[str, asyncio.Task]  # non-blocking tasks
+    focused_window_tracking: dict[str, FocusTracker] = {}
+    previously_focused_window: str = ""
+    last_focused: Scratch | None = None
 
-    def __init__(self, name):
+    def __init__(self, name: str) -> None:
         super().__init__(name)
         self._hysteresis_tasks = {}
         self.get_client_props = partial(get_client_props, logger=self.log)
         Scratch.get_client_props = self.get_client_props
-        self.get_focused_monitor_props = partial(
-            get_focused_monitor_props, logger=self.log
-        )
+        self.get_focused_monitor_props = partial(get_focused_monitor_props, logger=self.log)
 
     async def exit(self) -> None:
-        "exit hook"
+        """Exit hook."""
 
-        async def die_in_piece(scratch: Scratch):
+        async def die_in_piece(scratch: Scratch) -> None:
             if scratch.uid in self.procs:
                 proc = self.procs[scratch.uid]
                 proc.terminate()
                 for _ in range(10):
-                    if not await scratch.isAlive():
+                    if not await scratch.is_alive():
                         break
                     await asyncio.sleep(0.1)
-                if await scratch.isAlive():
+                if await scratch.is_alive():
                     proc.kill()
                 await proc.wait()
 
-        await asyncio.gather(
-            *(die_in_piece(scratch) for scratch in self.scratches.values())
-        )
+        await asyncio.gather(*(die_in_piece(scratch) for scratch in self.scratches.values()))
 
     async def on_reload(self) -> None:
-        "config loader"
+        """Config loader."""
         # Create new scratches with fresh config items
-        scratches = {
-            name: Scratch(name, options) for name, options in self.config.items()
-        }
+        scratches = {name: Scratch(name, options) for name, options in self.config.items()}
 
         scratches_to_spawn = set()
         for name in scratches:
             scratch = self.scratches.get(name)
             if scratch:  # if existing scratch exists, overrides the conf object
                 scratch.set_config(scratches[name].conf)
             else:
@@ -81,576 +96,634 @@
                 if not is_lazy:
                     scratches_to_spawn.add(name)
 
         for name in scratches_to_spawn:
             if await self.ensure_alive(name):
                 scratch = self.scratches.get(name)
                 assert scratch
-                scratch.meta["should_hide"] = True
+                scratch.meta.should_hide = True
             else:
                 self.log.error("Failure starting %s", name)
 
-        for scratch in list(self.scratches.getByState("configured")):
+        for scratch in list(self.scratches.get_by_state("configured")):
             assert scratch
-            self.scratches.clearState(scratch, "configured")
+            self.scratches.clear_state(scratch, "configured")
 
-    async def _configure_windowrules(self, scratch):
-        "Setting up initial client window state (sets windowrules)"
-        configured = self.scratches.hasState(scratch, "configured")
-        if configured:
-            return
-        self.scratches.setState(scratch, "configured")
+    async def _unset_windowrules(self, scratch: Scratch) -> None:
+        """Unset the windowrules."""
+        defined_class = scratch.conf.get("class", "")
+        if defined_class:
+            await self.hyprctl(f"windowrule unset,^({defined_class})$", "keyword")
+
+    async def _configure_windowrules(self, scratch: Scratch) -> None:
+        """Set initial client window state (sets windowrules)."""
+        self.scratches.set_state(scratch, "configured")
         animation_type: str = scratch.conf.get("animation", "fromTop").lower()
         defined_class: str = scratch.conf.get("class", "")
+        skipped_windowrules = scratch.conf.get("skip_windowrules", [])
         if defined_class:
-            monitor = await self.get_focused_monitor_props(
-                name=scratch.conf.get("force_monitor")
-            )
+            monitor = await self.get_focused_monitor_props(name=scratch.conf.get("force_monitor"))
             width, height = convert_coords(scratch.conf.get("size", "80% 80%"), monitor)
 
-            ipc_commands = [
-                f"windowrule float,^({defined_class})$",
-                f"windowrule workspace special:scratch_{scratch.uid} silent,^({defined_class})$",
-            ]
+            ipc_commands = []
+
+            if "float" not in skipped_windowrules:
+                ipc_commands.append(f"windowrule float,^({defined_class})$")
+            if "workspace" not in skipped_windowrules:
+                ipc_commands.append(f"windowrule workspace special:scratch_{scratch.uid} silent,^({defined_class})$")
+            set_aspect = "aspect" not in skipped_windowrules
 
             if animation_type:
                 margin_x = (monitor["width"] - width) // 2
                 margin_y = (monitor["height"] - height) // 2
 
+                if is_rotated(monitor):
+                    margin_x, margin_y = margin_y, margin_x
+
                 t_pos = {
                     "fromtop": f"{margin_x} -200%",
                     "frombottom": f"{margin_x} 200%",
                     "fromright": f"200% {margin_y}",
                     "fromleft": f"-200% {margin_y}",
                 }[animation_type]
-                ipc_commands.append(f"windowrule move {t_pos},^({defined_class})$")
+                if set_aspect:
+                    ipc_commands.append(f"windowrule move {t_pos},^({defined_class})$")
 
-            ipc_commands.append(f"windowrule size {width} {height},^({defined_class})$")
+            if set_aspect:
+                ipc_commands.append(f"windowrule size {width} {height},^({defined_class})$")
 
             await self.hyprctl(ipc_commands, "keyword")
 
-    async def __wait_for_client(self, item, use_proc=True) -> bool:
-        """Waits for a client to be up and running
+    async def __wait_for_client(self, scratch: Scratch, use_proc: bool = True) -> bool:
+        """Wait for a client to be up and running.
+
         if `match_by=` is used, will use the match criteria, else the process's PID will be used.
         """
-        self.log.info("==> Wait for %s spawning", item.uid)
+        self.log.info("==> Wait for %s spawning", scratch.uid)
         interval_range = [0.1] * 10 + [0.2] * 20 + [0.5] * 15
         for interval in interval_range:
             await asyncio.sleep(interval)
-            is_alive = await item.isAlive()
+            is_alive = await scratch.is_alive()
 
             # skips the checks if the process isn't started (just wait)
             if is_alive or not use_proc:
-                match_by = item.conf.get("match_by", "pid")
-                if match_by != "pid":
-                    info = await self.get_client_props(
-                        match_fn=get_match_fn(match_by, item.conf[match_by]),
-                        **{match_by: item.conf[match_by]},
-                    )
-                else:
-                    info = await self.get_client_props(pid=item.pid)
+                info = await scratch.fetch_matching_client()
                 if info:
-                    await item.updateClientInfo(info)
+                    await scratch.update_client_info(info)
                     self.log.info(
                         "=> %s client (proc:%s, addr:%s) detected on time",
-                        item.uid,
-                        item.pid,
-                        item.full_address,
+                        scratch.uid,
+                        scratch.pid,
+                        scratch.full_address,
                     )
-                    self.scratches.register(item)
-                    self.scratches.clearState(item, "respawned")
+                    self.scratches.register(scratch)
+                    self.scratches.clear_state(scratch, "respawned")
                     return True
             if use_proc and not is_alive:
                 return False
         return False
 
-    async def _start_scratch_nopid(self, item) -> bool:
-        "Ensure alive, PWA version"
-        uid = item.uid
-        started = "nopid" in item.meta
-        if not await item.isAlive():
+    async def _start_scratch_nopid(self, scratch: Scratch) -> bool:
+        """Ensure alive, PWA version."""
+        uid = scratch.uid
+        started = scratch.meta.no_pid
+        if not await scratch.is_alive():
             started = False
         if not started:
-            self.scratches.reset(item)
+            self.scratches.reset(scratch)
             await self.start_scratch_command(uid)
-            r = await self.__wait_for_client(item, use_proc=False)
-            item.meta["nopid"] = r
+            r = await self.__wait_for_client(scratch, use_proc=False)
+            scratch.meta.no_pid = r
             return r
         return True
 
-    async def _start_scratch(self, item):
-        "Ensure alive, standard version"
-        uid = item.uid
+    async def _start_scratch(self, scratch: Scratch) -> bool:
+        """Ensure alive, standard version."""
+        uid = scratch.uid
         if uid in self.procs:
-            try:
+            with contextlib.suppress(ProcessLookupError):
                 self.procs[uid].kill()
-            except ProcessLookupError:
-                pass
-        self.scratches.reset(item)
+        self.scratches.reset(scratch)
         await self.start_scratch_command(uid)
         self.log.info("starting %s", uid)
-        if not await self.__wait_for_client(item):
-            self.log.error("⚠ Failed spawning %s as proc %s", uid, item.pid)
-            if await item.isAlive():
+        if not await self.__wait_for_client(scratch):
+            self.log.error("⚠ Failed spawning %s as proc %s", uid, scratch.pid)
+            if await scratch.is_alive():
                 error = "The command didn't open a window"
             else:
                 await self.procs[uid].communicate()
                 code = self.procs[uid].returncode
-                if code:
-                    error = f"The command failed with code {code}"
-                else:
-                    error = "The command terminated sucessfully, is it already running?"
-            self.log.error('"%s": %s', item.conf["command"], error)
+                error = f"The command failed with code {code}" if code else "The command terminated successfully, is it already running?"
+            self.log.error('"%s": %s', scratch.conf["command"], error)
             await notify_error(error)
             return False
         return True
 
-    async def ensure_alive(self, uid):
-        """Ensure the scratchpad is started
+    async def ensure_alive(self, uid: str) -> bool:
+        """Ensure the scratchpad is started.
+
         Returns true if started
         """
         item = self.scratches.get(name=uid)
-        await self._configure_windowrules(item)
         assert item
 
         if self.cast_bool(item.conf.get("process_tracking"), True):
-            if not await item.isAlive():
+            if not await item.is_alive():
+                await self._configure_windowrules(item)
                 self.log.info("%s is not running, starting...", uid)
                 if not await self._start_scratch(item):
                     await notify_error(f'Failed to show scratch "{item.uid}"')
                     return False
+            await self._unset_windowrules(item)
             return True
 
         return await self._start_scratch_nopid(item)
 
     async def start_scratch_command(self, name: str) -> None:
-        "spawns a given scratchpad's process"
+        """Spawn a given scratchpad's process."""
         scratch = self.scratches.get(name)
         assert scratch
-        self.scratches.setState(scratch, "respawned")
+        self.scratches.set_state(scratch, "respawned")
         old_pid = self.procs[name].pid if name in self.procs else 0
         command = apply_variables(scratch.conf["command"], state.variables)
         proc = await asyncio.create_subprocess_shell(command)
         self.procs[name] = proc
         pid = proc.pid
         scratch.reset(pid)
         self.scratches.register(scratch, pid=pid)
-        self.log.info(
-            "scratch %s (%s) has pid %s", scratch.uid, scratch.conf.get("command"), pid
-        )
+        self.log.info("scratch %s (%s) has pid %s", scratch.uid, scratch.conf.get("command"), pid)
         if old_pid:
             self.scratches.clear(pid=old_pid)
 
-    async def updateScratchInfo(self, orig_scratch: Scratch | None = None) -> None:
-        """Update every scratchpads information if no `scratch` given,
-        else update a specific scratchpad info"""
+    async def update_scratch_info(self, orig_scratch: Scratch | None = None) -> None:
+        """Update Scratchpad information.
+
+        If `scratch` is given, update only this scratchpad.
+        Else, update every scratchpad.
+        """
         pid = orig_scratch.pid if orig_scratch else None
-        for client in await self.hyprctlJSON("clients"):
+        for client in await self.hyprctl_json("clients"):
             assert isinstance(client, dict)
             if pid and pid != client["pid"]:
                 continue
             # if no address registered, register it
             # + update client info in any case
             scratch = self.scratches.get(addr=client["address"][2:])
             if not scratch and client["pid"]:
                 scratch = self.scratches.get(pid=client["pid"])
             if scratch:
                 self.scratches.register(scratch, addr=client["address"][2:])
-                await scratch.updateClientInfo(client)
+                await scratch.update_client_info(cast(ClientInfo, client))
                 break
         else:
             self.log.info("Didn't update scratch info %s", self)
 
     # Events {{{
-    async def event_monitorremoved(self, monitor_name) -> None:
-        "Hides scratchpads on the removed screen"
+    async def event_closewindow(self, addr: str) -> None:
+        """Close window hook."""
+        # removes this address from the extra_addr
+        addr = "0x" + addr
+        for scratch in self.scratches.values():
+            if addr in scratch.extra_addr:
+                scratch.extra_addr.remove(addr)
+
+    async def event_monitorremoved(self, monitor_name: str) -> None:
+        """Hides scratchpads on the removed screen."""
         for scratch in self.scratches.values():
             if scratch.monitor == monitor_name:
                 await self.run_hide(scratch.uid, autohide=True)
 
-    async def event_configreloaded(self, _nothing):
-        "Re-apply windowrules when hyprland is restarted"
-        for scratch in list(self.scratches.getByState("configured")):
-            self.scratches.clearState(scratch, "configured")
+    async def event_configreloaded(self, _nothing: str) -> None:
+        """Re-apply windowrules when hyprland is restarted."""
+        for scratch in list(self.scratches.get_by_state("configured")):
             await self._configure_windowrules(scratch)
 
-    async def event_activewindowv2(self, addr) -> None:
-        "active windows hook"
+    async def event_activewindowv2(self, addr: str) -> None:
+        """Active windows hook."""
+        full_address = "" if not addr or len(addr) < MINIMUM_ADDR_LEN else "0x" + addr
         for uid, scratch in self.scratches.items():
             if not scratch.client_info:
                 continue
-            if scratch.address == addr:
+            if scratch.have_address(full_address):
+                self.last_focused = scratch
                 self.cancel_task(uid)
-            else:
-                if scratch.visible and scratch.conf.get("unfocus") == "hide":
-                    last_shown = scratch.meta.get("last_shown", 0)
-                    if last_shown + AFTER_SHOW_INHIBITION > time.time():
-                        self.log.debug(
-                            "(SKIPPED) hide %s because another client is active",
-                            uid,
-                        )
-                        continue
+            elif scratch.visible and scratch.conf.get("unfocus") == "hide":
+                last_shown = scratch.meta.last_shown
+                if last_shown + AFTER_SHOW_INHIBITION > time.time():
+                    self.log.debug(
+                        "(SKIPPED) hide %s because another client is active",
+                        uid,
+                    )
+                    continue
 
-                    hysteresis = scratch.conf.get("hysteresis", DEFAULT_HYSTERESIS)
-                    if hysteresis:
-                        self.cancel_task(uid)
-
-                        async def _task(scratch, delay):
-                            await asyncio.sleep(delay)
-                            if state.active_window == scratch.full_address:
-                                self.log.debug(
-                                    "Skipped hidding %s because client got the focus back",
-                                    scratch.uid,
-                                )
-                                return
-                            self.log.debug(
-                                "hide %s because another client is active", scratch.uid
-                            )
-                            await self.run_hide(scratch.uid, autohide=True)
-
-                            try:
-                                del self._hysteresis_tasks[scratch.uid]
-                            except KeyError:
-                                pass
-
-                        self._hysteresis_tasks[scratch.uid] = asyncio.create_task(
-                            _task(scratch, hysteresis)
-                        )
-                    else:
-                        self.log.debug("hide %s because another client is active", uid)
-                        await self.run_hide(uid, autohide=True)
-
-    async def _alternative_lookup(self):
-        "if not matching by pid, use specific matching and return True"
-        class_lookup_hack = [
-            s
-            for s in self.scratches.getByState("respawned")
-            if s.conf.get("match_by", "pid") != "pid"
-        ]
+                await self._hysteresis_handling(scratch)
+        self.previously_focused_window = full_address
+
+    async def _hysteresis_handling(self, scratch: Scratch) -> None:
+        """Hysteresis handling."""
+        hysteresis = scratch.conf.get("hysteresis", DEFAULT_HYSTERESIS)
+        if hysteresis:
+            self.cancel_task(scratch.uid)
+
+            async def _task(scratch: Scratch, delay: float) -> None:
+                await asyncio.sleep(delay)
+                self.log.debug("hide %s because another client is active", scratch.uid)
+                await self.run_hide(scratch.uid, autohide=True)
+
+                with contextlib.suppress(KeyError):
+                    del self._hysteresis_tasks[scratch.uid]
+
+            self._hysteresis_tasks[scratch.uid] = asyncio.create_task(_task(scratch, hysteresis))
+        else:
+            self.log.debug("hide %s because another client is active", scratch.uid)
+            await self.run_hide(scratch.uid, autohide=True)
+
+    async def _alternative_lookup(self) -> bool:
+        """If not matching by pid, use specific matching and return True."""
+        class_lookup_hack = [s for s in self.scratches.get_by_state("respawned") if s.conf.get("match_by", "pid") != "pid"]
         if not class_lookup_hack:
             return False
         self.log.debug("Lookup hack triggered")
-        # hack to update the client info from the provided match_by attribute
-        clients = await self.hyprctlJSON("clients")
+        clients = cast(list[ClientInfo], await self.hyprctl_json("clients"))
         for pending_scratch in class_lookup_hack:
-            match_by = pending_scratch.conf["match_by"]
-            match_value = pending_scratch.conf[match_by]
+            match_by, match_value = pending_scratch.get_match_props()
             match_fn = get_match_fn(match_by, match_value)
             for client in clients:
                 assert isinstance(client, dict)
                 if match_fn(client[match_by], match_value):
                     self.scratches.register(pending_scratch, addr=client["address"][2:])
                     self.log.debug("client class found: %s", client)
-                    await pending_scratch.updateClientInfo(client)
+                    await pending_scratch.update_client_info(client)
         return True
 
-    async def event_openwindow(self, params) -> None:
-        "open windows hook"
+    async def event_openwindow(self, params: str) -> None:
+        """Open windows hook."""
         addr, _wrkspc, _kls, _title = params.split(",", 3)
         item = self.scratches.get(addr=addr)
-        rs = list(self.scratches.getByState("respawned"))
-        if rs and not item:
-            # hack for windows which aren't related to the process (see #8)
+        respawned = list(self.scratches.get_by_state("respawned"))
+        if item:
+            # ensure initialized (no-op if already initialized)
+            await item.initialize(self)
+        elif respawned:
+            # NOTE: for windows which aren't related to the process (see #8)
             if not await self._alternative_lookup():
                 self.log.info("Updating Scratch info")
-                await self.updateScratchInfo()
-            item = self.scratches.get(addr=addr)
-            if item and item.meta["should_hide"]:
+                await self.update_scratch_info()
+            if item and item.meta.should_hide:
                 await self.run_hide(item.uid, force=True)
-        if item:
-            await item.initialize(self)
 
     # }}}
-    def cancel_task(self, uid):
-        "cancel a task"
+    def cancel_task(self, uid: str) -> bool:
+        """Cancel a task."""
         task = self._hysteresis_tasks.get(uid)
         if task:
             task.cancel()
             self.log.debug("Canceled previous task for %s", uid)
             if uid in self._hysteresis_tasks:
                 del self._hysteresis_tasks[uid]
             return True
         return False
 
     # Commands {{{
-    async def run_toggle(self, uid_or_uids: str) -> None:
-        """<name> toggles visibility of scratchpad "name" """
-        if " " in uid_or_uids:
-            uids = list(filter(bool, map(str.strip, uid_or_uids.split())))
+
+    async def run_attach(self) -> None:
+        """Attach the focused window to the last focused scratchpad."""
+        if not self.last_focused:
+            await self.notify_error("No scratchpad was focused")
+            return
+        focused = state.active_window
+        scratch = self.last_focused
+        if focused == scratch.full_address:
+            await self.notify_info("Scratch can't attach to itself")
+            return
+        if not scratch.visible:
+            await self.run_show(scratch.uid)
+
+        if state.active_window in scratch.extra_addr:
+            scratch.extra_addr.remove(focused)
         else:
-            uids = [uid_or_uids.strip()]
+            scratch.extra_addr.add(focused)
+
+    async def run_toggle(self, uid_or_uids: str) -> None:
+        """<name> toggles visibility of scratchpad "name"."""
+        uids = list(filter(bool, map(str.strip, uid_or_uids.split()))) if " " in uid_or_uids else [uid_or_uids.strip()]
 
         for uid in uids:
             self.cancel_task(uid)
 
         assert len(uids) > 0
         first_scratch = self.scratches.get(uids[0])
         if not first_scratch:
             self.log.warning("%s doesn't exist, can't toggle.", uids[0])
-            await notify_error(
-                f"Scratchpad '{uids[0]}' not found, check your configuration & the toggle parameter"
-            )
+            await notify_error(f"Scratchpad '{uids[0]}' not found, check your configuration & the toggle parameter")
             return
 
+        self.log.debug(
+            "visibility_check: %s == %s",
+            first_scratch.meta.space_identifier,
+            get_active_space_identifier(),
+        )
         if self.cast_bool(first_scratch.conf.get("alt_toggle")):
             # Needs to be on any monitor (if workspace matches)
-            extra_visibility_check = first_scratch.meta[
-                "space_identifier"
-            ] in await get_all_space_identifiers(await self.hyprctlJSON("monitors"))
-        else:
-            self.log.debug(
-                "visibility_check: %s == %s",
-                first_scratch.meta["space_identifier"],
-                get_active_space_identifier(),
+            extra_visibility_check = first_scratch.meta.space_identifier in await get_all_space_identifiers(
+                await self.hyprctl_json("monitors")
             )
+        else:
             # Needs to be on the active monitor+workspace
             extra_visibility_check = (
-                first_scratch.meta["space_identifier"] == get_active_space_identifier()
+                first_scratch.meta.space_identifier == get_active_space_identifier()
             )  # visible on the currently focused monitor
 
         is_visible = first_scratch.visible and (
             first_scratch.conf.get("force_monitor") or extra_visibility_check
         )  # always showing on the same monitor
         tasks = []
 
         for uid in uids:
             item = self.scratches.get(uid)
             if not item:
                 self.log.warning("%s is not configured", uid)
             else:
-                self.log.debug(
-                    "%s is visible = %s (but %s)", uid, item.visible, is_visible
-                )
-                if is_visible and await item.isAlive():
+                self.log.debug("%s visibility: %s and %s", uid, is_visible, item.visible)
+                if is_visible and await item.is_alive():
                     tasks.append(partial(self.run_hide, uid))
                 else:
                     tasks.append(partial(self.run_show, uid))
         await asyncio.gather(*(asyncio.create_task(t()) for t in tasks))
 
-    async def get_offsets(self, scratch, monitor=None):
-        "Return offset from config or use margin as a ref"
+    async def get_offsets(self, scratch: Scratch, monitor: MonitorInfo | None = None) -> tuple[int, int]:
+        """Return offset from config or use margin as a ref."""
         offset = scratch.conf.get("offset")
-        rotated = monitor["transform"] in (1, 3)
-        aspect = (
-            reversed(scratch.client_info["size"])
-            if rotated
-            else scratch.client_info["size"]
-        )
-
         if monitor is None:
-            monitor = await get_focused_monitor_props(
-                self.log, name=scratch.conf.get("force_monitor")
-            )
+            monitor = await get_focused_monitor_props(self.log, name=scratch.conf.get("force_monitor"))
+        rotated = is_rotated(monitor)
+        aspect = reversed(scratch.client_info["size"]) if rotated else scratch.client_info["size"]
 
         if offset:
-            return [convert_monitor_dimension(offset, ref, monitor) for ref in aspect]
+            return cast(tuple[int, int], (convert_monitor_dimension(offset, ref, monitor) for ref in aspect))
 
         # compute from client size & margin
         margin = scratch.conf.get("margin", DEFAULT_MARGIN)
 
-        mon_size = (
-            [monitor["height"], monitor["width"]]
-            if rotated
-            else [monitor["width"], monitor["height"]]
-        )
+        mon_size = [monitor["height"], monitor["width"]] if rotated else [monitor["width"], monitor["height"]]
 
         margins = [convert_monitor_dimension(margin, dim, monitor) for dim in mon_size]
-        return map(int, [(a + m) / monitor["scale"] for a, m in zip(aspect, margins)])
+        scaled = map(int, [(a + m) / monitor["scale"] for a, m in zip(aspect, margins, strict=False)])
+        return cast(tuple[int, int], scaled)
 
-    async def _hide_transition(self, scratch, monitor):
-        "animate hiding a scratchpad"
+    async def _hide_transition(self, scratch: Scratch, monitor: MonitorInfo) -> bool:
+        """Animate hiding a scratchpad."""
+        animation_type: str = get_animation_type(scratch)
 
-        animation_type: str = scratch.conf.get("animation", "").lower()
         if not animation_type:
             return False
 
-        off_x, off_y = await self.get_offsets(scratch, monitor)
-        await self._slide_animation(animation_type, scratch, off_x, off_y)
-        await asyncio.sleep(
-            scratch.conf.get("hide_delay", DEFAULT_HIDE_DELAY)
-        )  # await for animation to finish
+        await self._slide_animation(animation_type, scratch, await self.get_offsets(scratch, monitor))
+        await asyncio.sleep(scratch.conf.get("hide_delay", DEFAULT_HIDE_DELAY))  # await for animation to finish
         return True
 
-    async def _slide_animation(self, animation_type, scratch, off_x, off_y):
-        "Slides the window `offset` pixels respecting `animation_type`"
-        addr = "address:" + scratch.full_address
-        if animation_type == "fromtop":
-            await self.hyprctl(f"movewindowpixel 0 {-off_y},{addr}")
-        elif animation_type == "frombottom":
-            await self.hyprctl(f"movewindowpixel 0 {off_y},{addr}")
-        elif animation_type == "fromleft":
-            await self.hyprctl(f"movewindowpixel {-off_x} 0,{addr}")
-        elif animation_type == "fromright":
-            await self.hyprctl(f"movewindowpixel {off_x} 0,{addr}")
-
-    async def run_show(self, uid) -> None:
-        """<name> shows scratchpad "name" """
-        item = self.scratches.get(uid)
+    async def _slide_animation(
+        self,
+        animation_type: str,
+        scratch: Scratch,
+        offset: tuple[int, int],
+        only_secondary: bool = False,
+    ) -> None:
+        """Slides the window `offset` pixels respecting `animation_type`."""
+        addresses = [] if only_secondary else [scratch.full_address]
+        addresses.extend(scratch.extra_addr)
+        off_x, off_y = offset
+
+        animation_actions = {
+            "fromright": f"movewindowpixel {off_x} 0",
+            "fromleft": f"movewindowpixel {-off_x} 0",
+            "frombottom": f"movewindowpixel 0 {off_y}",
+            "fromtop": f"movewindowpixel 0 {-off_y}",
+        }
+
+        for addr in addresses:
+            if animation_type in animation_actions:
+                await self.hyprctl(f"{animation_actions[animation_type]},address:{addr}")
 
-        if not item:
+    async def run_show(self, uid: str) -> None:
+        """<name> shows scratchpad "name"."""
+        scratch = self.scratches.get(uid)
+
+        if not scratch:
             self.log.warning("%s doesn't exist, can't hide.", uid)
-            await notify_error(
-                f"Scratchpad '{uid}' not found, check your configuration or the show parameter"
-            )
+            await notify_error(f"Scratchpad '{uid}' not found, check your configuration or the show parameter")
             return
 
-        self.focused_window_tracking[uid] = state.active_window
-
         self.cancel_task(uid)
 
         self.log.info("Showing %s", uid)
-        was_alive = await item.isAlive()
+        was_alive = await scratch.is_alive()
         if not await self.ensure_alive(uid):
             self.log.error("Failed to show %s, aborting.", uid)
             return
 
-        excluded = item.conf.get("excludes", [])
-        if excluded == "*":
-            excluded = [
-                scratch.uid for scratch in self.scratches.values() if scratch.uid != uid
-            ]
-        for e_uid in excluded:
-            scratch = self.scratches.get(e_uid)
-            assert scratch
-            if scratch.visible:
+        excluded_ids = scratch.conf.get("excludes", [])
+        if excluded_ids == "*":
+            excluded_ids = [excluded.uid for excluded in self.scratches.values() if excluded.uid != uid]
+        for e_uid in excluded_ids:
+            excluded = self.scratches.get(e_uid)
+            assert excluded
+            if excluded.visible:
                 await self.run_hide(e_uid, autohide=True)
-        await item.updateClientInfo()
-        await item.initialize(self)
 
-        item.visible = True
-        item.meta["space_identifier"] = get_active_space_identifier()
-        monitor = await self.get_focused_monitor_props(
-            name=item.conf.get("force_monitor")
-        )
+        await scratch.initialize(self)
+
+        scratch.visible = True
+        scratch.meta.space_identifier = get_active_space_identifier()
+        monitor = await self.get_focused_monitor_props(name=scratch.conf.get("force_monitor"))
 
         assert monitor
-        assert item.full_address, "No address !"
+        assert scratch.full_address, "No address !"
 
-        await self._show_transition(item, monitor, was_alive)
-        item.monitor = monitor["name"]
+        await self._show_transition(scratch, monitor, was_alive)
+        scratch.monitor = monitor["name"]
 
-    async def _show_transition(self, item, monitor, was_alive):
-        "perfoms the transition to visible state"
-        animation_type = item.conf.get("animation", "").lower()
-        forbid_special = not item.conf.get("allow_special_workspace", True)
+    async def _handle_multiwindow(self, scratch: Scratch, clients: list[ClientInfo]) -> None:
+        """Collect every matching client for the scratchpad and add them to extra_addr if needed."""
+        if not self.cast_bool(scratch.conf.get("multi"), True):
+            return
+        match_by, match_value = scratch.get_match_props()
+        match_fn = get_match_fn(match_by, match_value)
+        for client in clients:
+            if client["address"] == scratch.full_address:
+                continue
+            if match_fn(client[match_by], match_value):  # type: ignore
+                address = client["address"]
+                if address not in scratch.extra_addr:
+                    scratch.extra_addr.add(address)
+
+    async def _show_transition(self, scratch: Scratch, monitor: MonitorInfo, was_alive: bool) -> None:
+        """Performs the transition to visible state."""
+        forbid_special = not self.cast_bool(scratch.conf.get("allow_special_workspace"), True)
         wrkspc = (
             monitor["activeWorkspace"]["name"]
-            if forbid_special or not monitor["specialWorkspace"]["name"]
+            if forbid_special
+            or not monitor["specialWorkspace"]["name"]
+            or monitor["specialWorkspace"]["name"].startswith("special:scratch")
             else monitor["specialWorkspace"]["name"]
         )
+        if self.previously_focused_window:
+            self.focused_window_tracking[scratch.uid] = FocusTracker(self.previously_focused_window, wrkspc)
 
-        item.meta["last_shown"] = time.time()
+        scratch.meta.last_shown = time.time()
         # Start the transition
-        await self.hyprctl(
-            [
-                f"moveworkspacetomonitor special:scratch_{item.uid} {monitor['name']}",
-                f"movetoworkspacesilent {wrkspc},address:{item.full_address}",
-                f"alterzorder top,address:{item.full_address}",
-            ]
-        )
-        preserve_aspect = self.cast_bool(item.conf.get("preserve_aspect"))
+        preserve_aspect = self.cast_bool(scratch.conf.get("preserve_aspect"))
         should_set_aspect = (
-            not (preserve_aspect and was_alive) or item.monitor != state.active_monitor
+            not (preserve_aspect and was_alive) or scratch.monitor != state.active_monitor
         )  # not aspect preserving or it's newly spawned
         if should_set_aspect:
-            await self._fix_size(item, monitor)
-        await item.updateClientInfo()
+            await self._fix_size(scratch, monitor)
         position_fixed = False
         if should_set_aspect:
-            position_fixed = await self._fix_position(item, monitor)
-        if not position_fixed:
-            if animation_type:
-                if preserve_aspect and was_alive and not should_set_aspect:
-                    # Relative positioning
-                    if "size" not in item.client_info:
-                        await self.updateScratchInfo(item)
+            position_fixed = await self._fix_position(scratch, monitor)
+
+        clients = await self.hyprctl_json("clients")
+        await self._handle_multiwindow(scratch, clients)  # not very useful but cheap
+        # move
+        move_commands = [
+            f"moveworkspacetomonitor special:scratch_{scratch.uid} {monitor['name']}",
+            f"movetoworkspacesilent {wrkspc},address:{scratch.full_address}",
+            f"alterzorder top,address:{scratch.full_address}",
+        ]
+        for addr in scratch.extra_addr:
+            move_commands.extend(
+                [
+                    f"movetoworkspacesilent {wrkspc},address:{addr}",
+                    f"alterzorder top,address:{addr}",
+                ]
+            )
+
+        await self.hyprctl(move_commands)
+        await self._update_infos(scratch, clients)
 
-                    ox, oy = await self.get_offsets(item, monitor)
-                    await self._slide_animation(animation_type, item, -ox, -oy)
+        if not position_fixed:
+            relative_animation = preserve_aspect and was_alive and not should_set_aspect
+            await self._animate_show(scratch, monitor, relative_animation)
+        await self.hyprctl(f"focuswindow address:{scratch.full_address}")
+        scratch.meta.last_shown = time.time()
+        scratch.meta.monitor_info = monitor
+
+    async def _update_infos(self, scratch: Scratch, clients: list[ClientInfo]) -> None:
+        """Update the client info."""
+        try:
+            # update position, size & workspace information (workspace properties have been created)
+            await scratch.update_client_info(clients=clients)
+        except KeyError:
+            for alt_addr in scratch.extra_addr:
+                # get the client info for the extra addresses
+                try:
+                    client_info = await self.get_client_props(addr="0x" + alt_addr, clients=clients)
+                    if not client_info:
+                        continue
+                    await scratch.update_client_info(clients=clients, client_info=client_info)
+                except KeyError:
+                    pass
                 else:
-                    # Absolute positioning
-                    fn = getattr(Animations, animation_type)
-                    command = fn(
-                        monitor,
-                        item.client_info,
-                        "address:" + item.full_address,
-                        item.conf.get("margin", DEFAULT_MARGIN),
-                    )
-                    await self.hyprctl(command)
+                    break
             else:
-                self.log.warning(
-                    "No position and no animation provided for %s, don't know where to place it.",
-                    item.uid,
-                )
+                self.log.exception("Lost the client info for %s", scratch.uid)
 
-        await self.hyprctl(f"focuswindow address:{item.full_address}")
-        item.meta["last_shown"] = time.time()
-        item.meta["monitor_info"] = monitor
+    async def _animate_show(self, scratch: Scratch, monitor: MonitorInfo, relative_animation: bool) -> None:
+        """Animate the show transition."""
+        animation_type = get_animation_type(scratch)
+        if animation_type:
+            offset = tuple(-1 * n for n in await self.get_offsets(scratch, monitor))
+            if relative_animation:
+                # Relative positioning
+                if "size" not in scratch.client_info:
+                    await self.update_scratch_info(scratch)  # type: ignore
 
-    async def _fix_size(self, item, monitor):
-        "apply the `size` config parameter"
+                await self._slide_animation(animation_type, scratch, offset)
+            else:
+                # Absolute positioning
+                command = getattr(Animations, animation_type)(
+                    monitor,
+                    scratch.client_info,
+                    "address:" + scratch.full_address,
+                    scratch.conf.get("margin", DEFAULT_MARGIN),
+                )
+                await self.hyprctl(command)
+                await self._slide_animation(animation_type, scratch, offset, only_secondary=True)
+        else:
+            self.log.warning(
+                "No position and no animation provided for %s, don't know where to place it.",
+                scratch.uid,
+            )
 
-        size = item.conf.get("size")
+    async def _fix_size(self, scratch: Scratch, monitor: MonitorInfo) -> None:
+        """Apply the size from config."""
+        size = scratch.conf.get("size")
         if size:
             width, height = convert_coords(size, monitor)
-            max_size = item.conf.get("max_size")
+            max_size = scratch.conf.get("max_size")
             if max_size:
                 max_width, max_height = convert_coords(max_size, monitor)
                 width = min(max_width, width)
                 height = min(max_height, height)
-            await self.hyprctl(
-                f"resizewindowpixel exact {width} {height},address:{item.full_address}"
-            )
+            await self.hyprctl(f"resizewindowpixel exact {width} {height},address:{scratch.full_address}")
 
-    async def _fix_position(self, item, monitor):
-        "apply the `position` config parameter"
-
-        position = item.conf.get("position")
+    async def _fix_position(self, scratch: Scratch, monitor: MonitorInfo) -> bool:
+        """Apply the `position` config parameter."""
+        position = scratch.conf.get("position")
         if position:
             x_pos, y_pos = convert_coords(position, monitor)
             x_pos_abs, y_pos_abs = x_pos + monitor["x"], y_pos + monitor["y"]
-            await self.hyprctl(
-                f"movewindowpixel exact {x_pos_abs} {y_pos_abs},address:{item.full_address}"
-            )
+            await self.hyprctl(f"movewindowpixel exact {x_pos_abs} {y_pos_abs},address:{scratch.full_address}")
             return True
         return False
 
-    async def run_hide(self, uid: str, force=False, autohide=False) -> None:
-        """<name> hides scratchpad "name"
+    async def run_hide(self, uid: str, force: bool = False, autohide: bool = False) -> None:
+        """<name> hides scratchpad "name".
+
         if `autohide` is True, skips focus tracking
-        `force` ignores the visibility check"""
+        `force` ignores the visibility check
+        """
         scratch = self.scratches.get(uid)
+        active_window = state.active_window
+        active_workspace = state.active_workspace
 
         if not scratch:
-            await notify_error(
-                f"Scratchpad '{uid}' not found, check your configuration or the hide parameter"
-            )
+            await notify_error(f"Scratchpad '{uid}' not found, check your configuration or the hide parameter")
             self.log.warning("%s is not configured", uid)
             return
         if not scratch.visible and not force and not autohide:
             await notify_error(f"Scratchpad '{uid}' is not visible, will not hide.")
             self.log.warning("%s is already hidden", uid)
             return
+        # collects window which have been created by the app
+        if self.cast_bool(scratch.conf.get("multi"), True):
+            await self._handle_multiwindow(scratch, await self.hyprctl_json("clients"))
         scratch.visible = False
-        scratch.meta["should_hide"] = False
+        scratch.meta.should_hide = False
         self.log.info("Hiding %s", uid)
-        animated = await self._hide_transition(scratch, scratch.meta["monitor_info"])
+        await self._hide_transition(scratch, scratch.meta.monitor_info)
 
-        await self.hyprctl(
-            f"movetoworkspacesilent special:scratch_{uid},address:{scratch.full_address}"
-        )
+        await self.hyprctl(f"movetoworkspacesilent special:scratch_{uid},address:{scratch.full_address}")
 
-        if (
-            not autohide
-            and animated
-            and uid in self.focused_window_tracking
-            and self.cast_bool(scratch.conf.get("restore_focus"), True)
-        ):  # focus got lost when animating
-            await self.hyprctl(
-                f"focuswindow address:{self.focused_window_tracking[uid]}"
-            )
-            del self.focused_window_tracking[uid]
+        for addr in scratch.extra_addr:
+            await self.hyprctl(f"movetoworkspacesilent special:scratch_{uid},address:{addr}")
+            await asyncio.sleep(0.01)
+        await self._handle_focus_tracking(scratch, active_window, active_workspace)
+
+    async def _handle_focus_tracking(self, scratch: Scratch, active_window: str, active_workspace: str) -> None:
+        """Handle focus tracking."""
+        if not self.cast_bool(scratch.conf.get("smart_focus"), True):
+            return
+        for track in self.focused_window_tracking.values():
+            if scratch.have_address(track.prev_focused_window):
+                track.clear()
+        tracker = self.focused_window_tracking.get(scratch.uid)
+        if tracker and not tracker.prev_focused_window_wrkspc.startswith("special:"):
+            same_workspace = tracker.prev_focused_window_wrkspc == active_workspace
+            if scratch.have_address(active_window) and same_workspace and not scratch.have_address(tracker.prev_focused_window):
+                await self.hyprctl(f"focuswindow address:{tracker.prev_focused_window}")
 
     # }}}
 
 
 # }}}
+# }}}
```

### Comparing `pyprland-2.2.9/pyprland/plugins/scratchpads/helpers.py` & `pyprland-2.3.0/pyprland/plugins/scratchpads/helpers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,81 @@
-" Helper functions for the scratchpads plugin "
+"""Helper functions for the scratchpads plugin."""
 
 __all__ = [
+    "OverridableConfig",
     "get_active_space_identifier",
     "get_all_space_identifiers",
     "get_match_fn",
-    "OverridableConfig",
 ]
 
 import re
+from collections.abc import Callable
+from typing import Any
 
 from ...common import state
+from ...types import MonitorInfo
 
 
-def get_active_space_identifier():
-    "Returns a unique object for the workspace + monitor combination"
+def get_active_space_identifier() -> tuple[str, str]:
+    """Return a unique object for the workspace + monitor combination."""
     return (state.active_workspace, state.active_monitor)
 
 
-async def get_all_space_identifiers(monitors):
-    "Returns a list of every space identifiers (workspace + monitor) on active screens"
-    return [
-        (monitor["activeWorkspace"]["name"], monitor["name"]) for monitor in monitors
-    ]
+async def get_all_space_identifiers(monitors: list[MonitorInfo]) -> list[tuple[str, str]]:
+    """Return a list of every space identifiers (workspace + monitor) on active screens."""
+    return [(monitor["activeWorkspace"]["name"], monitor["name"]) for monitor in monitors]
 
 
 _match_fn_re_cache = {}
 
 
-def get_match_fn(prop_name, prop_value):
-    "Returns a function to match a client based on a property"
+def get_match_fn(prop_name: str, prop_value: float | bool | str | list) -> Callable[[Any, Any], bool]:
+    """Return a function to match a client based on a property."""
     assert prop_name  # may be used for more specific matching
     if isinstance(prop_value, str) and prop_value.startswith("re:"):
         # get regex from cache if possible:
         if prop_value not in _match_fn_re_cache:
             regex = re.compile(prop_value[3:])
-            _match_fn_re_cache[prop_value] = lambda value1, value2: regex.match(value1)
+
+            def _comp_function(value1: str, _value2: str) -> bool:
+                return bool(regex.match(value1))
+
+            _match_fn_re_cache[prop_value] = _comp_function
         return _match_fn_re_cache[prop_value]
     return lambda value1, value2: value1 == value2
 
 
-class OverridableConfig:
-    "A `dict`-like object allowing per-monitor overrides"
+class OverridableConfig(dict):
+    """A `dict`-like object allowing per-monitor overrides."""
 
-    def __init__(self, ref, monitor_override):
+    def __init__(
+        self, ref: dict[str, float | bool | list | str], monitor_override: dict[str, dict[str, float | bool | list | str]]
+    ) -> None:
         self.ref = ref
         self.mon_override = monitor_override
 
-    def __setitem__(self, name, value):
+    def __setitem__(self, name: str, value: float | bool | str | list) -> None:
         self.ref[name] = value
 
-    def __getitem__(self, name):
+    def __getitem__(self, name: str) -> float | bool | str | list:
         override = self.mon_override.get(state.active_monitor, {})
         if name in override:
             return override[name]
         return self.ref[name]
 
-    def __contains__(self, name):
+    def __contains__(self, name: object) -> bool:
+        assert isinstance(name, str)
         try:
             self[name]  # pylint: disable=pointless-statement
-            return True
         except KeyError:
             return False
+        return True
 
-    def get(self, name, default=None):
-        "get the attribute `name`"
+    def get(self, name: str, default: object = None) -> object | None:
+        """Get the attribute `name`."""
         try:
             return self[name]
         except KeyError:
             return default
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"{self.ref} {self.mon_override}"
```

### Comparing `pyprland-2.2.9/pyprland/plugins/scratchpads/objects.py` & `pyprland-2.3.0/pyprland/plugins/scratchpads/objects.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,123 +1,165 @@
-" Scratchpad object definition "
+"""Scratchpad object definition."""
 
 __all__ = ["Scratch"]
 
-import os
 import logging
-from typing import Callable, cast
-from collections import defaultdict
+import os
+from dataclasses import dataclass
+from typing import TYPE_CHECKING, Any, Protocol, cast
 
-from aiofiles import os as aios
 from aiofiles import open as aiopen
+from aiofiles import os as aios
 
+from ...common import CastBoolMixin, state
 from ...ipc import notify_error
-from ...common import CastBoolMixin, VersionInfo, state
+from ...types import ClientInfo, MonitorInfo, VersionInfo
 from .helpers import OverridableConfig, get_match_fn
 
+if TYPE_CHECKING:
+    from collections.abc import Callable
+
+    import pyprland.plugins.scratchpads.Extension as PyprlandPlugin
+
+    class ClientPropGetter(Protocol):
+        """type for the get_client_props function."""
+
+        async def __call__(self, match_fn: Callable | None = None, clients: list[ClientInfo] | None = None, **kw) -> ClientInfo | None:
+            pass
+
+
+@dataclass
+class MetaInfo:
+    """Meta properties."""
+
+    initialized: bool = False
+    should_hide: bool = False
+    no_pid: bool = False
+    last_shown: float | int = 0
+    space_identifier: tuple[str, str] = ("", "")
+    monitor_info: MonitorInfo = None  # type: ignore
+
 
 class Scratch(CastBoolMixin):  # {{{
-    "A scratchpad state including configuration & client state"
+    """A scratchpad state including configuration & client state."""
+
     log = logging.getLogger("scratch")
-    get_client_props: Callable
+    get_client_props: "ClientPropGetter"
+    client_info: ClientInfo
+    visible = False
+    uid = ""
+    monitor = ""
+    pid = -1
 
-    def __init__(self, uid, opts):
+    def __init__(self, uid: str, opts: dict[str, Any]) -> None:
         self.uid = uid
-        self.pid = 0
         self.set_config(OverridableConfig(opts, opts.get("monitor", {})))
-        self.visible = False
-        self.client_info = {}
-        self.meta = defaultdict(lambda: False)
-        self.monitor = ""
+        self.client_info: ClientInfo = {}  # type: ignore
+        self.meta = MetaInfo()
+        self.extra_addr: set[str] = set()  # additional client addresses
 
-    def set_config(self, opts):
-        "Apply constraints to the configuration"
+    def set_config(self, opts: dict[str, Any]) -> None:
+        """Apply constraints to the configuration."""
         if "class_match" in opts:  # NOTE: legacy, to be removed
             opts["match_by"] = "class"
         if self.cast_bool(opts.get("preserve_aspect")):
             opts["lazy"] = True
         if not opts.get("process_tracking", True):
             opts["lazy"] = True
             if "match_by" not in opts:
                 opts["match_by"] = "class"
         if state.hyprland_version < VersionInfo(0, 39, 0):
             opts["allow_special_workspace"] = False
 
         self.conf = opts
 
-    async def initialize(self, ex):
-        "Initialize the scratchpad"
-        if self.meta["initialized"]:
+    def have_address(self, addr: str) -> bool:
+        """Check if the address is the same as the client."""
+        return addr == self.full_address or addr in self.extra_addr
+
+    async def initialize(self, ex: "PyprlandPlugin") -> None:
+        """Initialize the scratchpad."""
+        if self.meta.initialized:
             return
-        self.meta["initialized"] = True
-        await self.updateClientInfo()
-        await ex.hyprctl(
-            f"movetoworkspacesilent special:scratch_{self.uid},address:{self.full_address}"
-        )
+        self.meta.initialized = True
+        await self.update_client_info()
+        await ex.hyprctl(f"movetoworkspacesilent special:scratch_{self.uid},address:{self.full_address}")
         if "class_match" in self.conf:  # NOTE: legacy, to be removed
             await notify_error(
                 f'scratchpad {self.uid} should use match_by="class" instead of the deprecated class_match',
                 logger=self.log,
             )
 
-    async def isAlive(self) -> bool:
-        "is the process running ?"
+    async def is_alive(self) -> bool:
+        """Is the process running ?."""
         if self.cast_bool(self.conf.get("process_tracking"), True):
             path = f"/proc/{self.pid}"
             if await aios.path.exists(path):
-                async with aiopen(
-                    os.path.join(path, "status"), mode="r", encoding="utf-8"
-                ) as f:
+                async with aiopen(os.path.join(path, "status"), mode="r", encoding="utf-8") as f:
                     for line in await f.readlines():
                         if line.startswith("State"):
                             proc_state = line.split()[1]
-                            return (
-                                proc_state not in "ZX"
-                            )  # not "Z (zombie)"or "X (dead)"
+                            return proc_state not in "ZX"  # not "Z (zombie)"or "X (dead)"
         else:
-            if "nopid" in self.meta:
-                match_by = self.conf["match_by"]
-                match_value = self.conf[match_by]
-                match_fn = get_match_fn(match_by, match_value)
-                return bool(
-                    await self.get_client_props(
-                        match_fn=match_fn, **{match_by: match_value}
-                    )
-                )
+            if self.meta.no_pid:
+                return bool(await self.fetch_matching_client())
             return False
 
         return False
 
+    async def fetch_matching_client(self, clients: list[ClientInfo] | None = None) -> ClientInfo | None:
+        """Fetch the first matching client properties."""
+        match_by, match_val = self.get_match_props()
+        return await self.get_client_props(
+            match_fn=get_match_fn(match_by, match_val),
+            clients=clients,
+            **{match_by: match_val},
+        )
+
+    def get_match_props(self) -> tuple[str, str | float]:
+        """Return the match properties for the scratchpad."""
+        match_by = self.conf.get("match_by", "pid")
+        return match_by, self.pid if match_by == "pid" else self.conf[match_by]
+
     def reset(self, pid: int) -> None:
-        "clear the object"
+        """Clear the object."""
         self.pid = pid
         self.visible = False
-        self.client_info = {}
-        self.meta["initialized"] = False
+        self.client_info = {}  # type: ignore
+        self.meta.initialized = False
 
     @property
     def address(self) -> str:
-        "Returns the client address"
-        return str(self.client_info.get("address", ""))[2:]
+        """Return the client address."""
+        return self.client_info.get("address", "")[2:]
 
     @property
     def full_address(self) -> str:
-        "Returns the client address"
+        """Return the client address."""
         return cast(str, self.client_info.get("address", ""))
 
-    async def updateClientInfo(self, client_info=None) -> None:
-        "update the internal client info property, if not provided, refresh based on the current address"
+    async def update_client_info(
+        self,
+        client_info: ClientInfo | None = None,
+        clients: list[ClientInfo] | None = None,
+    ) -> None:
+        """Update the internal client info property, if not provided, refresh based on the current address."""
         if client_info is None:
-            client_info = await self.get_client_props(addr=self.full_address)
+            client_info = await self.get_client_props(addr=self.full_address, clients=clients)
         if not isinstance(client_info, dict):
-            self.log.error(
-                "client_info of %s must be a dict: %s", self.address, client_info
-            )
-            raise AssertionError(f"Not a dict: {client_info}")
+            if client_info is None:
+                self.log.error("The client window %s vanished", self.full_address)
+                msg = f"Client window {self.full_address} not found"
+                raise KeyError(msg)
+            # Unexpected type:
+            self.log.error("client_info of %s must be a dict: %s", self.address, client_info)
+            msg = f"Not a dict: {client_info}"
+            raise TypeError(msg)
 
         self.client_info.update(client_info)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"{self.uid} {self.address} : {self.client_info} / {self.conf}"
 
 
 # }}}
+# }}}
```

### Comparing `pyprland-2.2.9/pyprland/plugins/shortcuts_menu.py` & `pyprland-2.3.0/pyprland/plugins/shortcuts_menu.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-" Shortcuts menu "
+"""Shortcuts menu."""
+
 import asyncio
+from typing import cast
 
-from .interface import Plugin
 from ..adapters.menus import MenuMixin
-from ..common import state, apply_variables, apply_filter, CastBoolMixin
+from ..common import CastBoolMixin, apply_filter, apply_variables, state
+from .interface import Plugin
 
 
 class Extension(CastBoolMixin, MenuMixin, Plugin):
-    "Shows a menu with shortcuts"
+    """Shows a menu with shortcuts."""
 
     # Commands
 
-    async def run_menu(self, name=""):
-        """[name] Shows the menu, if "name" is provided, will only show this sub-menu"""
+    async def run_menu(self, name: str = "") -> None:
+        """[name] Shows the menu, if "name" is provided, will only show this sub-menu."""
         await self.ensure_menu_configured()
         options = self.config["entries"]
         if name:
             for elt in name.split("."):
                 options = options[elt]
 
-        def _format_title(label, obj):
+        def _format_title(label: str, obj: str | list) -> str:
             if isinstance(obj, str):
                 suffix = self.config.get("command_end", "")
                 prefix = self.config.get("command_start", "")
             else:
                 suffix = self.config.get("submenu_end", "➜")
                 prefix = self.config.get("submenu_start", "")
 
@@ -37,65 +39,59 @@
                 break
             if isinstance(options, list):
                 self.log.info("interpreting %s", options)
                 await self._handle_chain(options)
                 break
             try:
                 formatted_options = {_format_title(k, v): v for k, v in options.items()}
-                if (
-                    self.cast_bool(self.config.get("skip_single"), True)
-                    and len(formatted_options) == 1
-                ):
-                    selection = list(formatted_options.keys())[0]
+                if self.cast_bool(self.config.get("skip_single"), True) and len(formatted_options) == 1:
+                    selection = next(iter(formatted_options.keys()))
                 else:
                     selection = await self.menu.run(formatted_options, selection)
                 options = formatted_options[selection]
             except KeyError:
                 self.log.info("menu command canceled")
                 break
 
     # Utils
 
-    async def _handle_chain(self, options):
-        "Handles a chain of special objects + final command string"
+    async def _handle_chain(self, options: list[str | dict]) -> None:
+        """Handle a chain of special objects + final command string."""
         variables: dict[str, str] = state.variables.copy()
         autovalidate = self.cast_bool(self.config.get("skip_single"), True)
         for option in options:
             if isinstance(option, str):
                 await self._run_command(option, variables)
             else:
                 choices = []
                 var_name = option["name"]
                 if option.get("command"):  # use the option to select some variable
-                    proc = await asyncio.create_subprocess_shell(
-                        option["command"], stdout=asyncio.subprocess.PIPE
-                    )
+                    proc = await asyncio.create_subprocess_shell(option["command"], stdout=asyncio.subprocess.PIPE)
                     assert proc.stdout
                     await proc.wait()
                     option_array = (await proc.stdout.read()).decode().split("\n")
-                    choices.extend(
-                        [
-                            apply_variables(line, variables).strip()
-                            for line in option_array
-                            if line.strip()
-                        ]
-                    )
+                    choices.extend([apply_variables(line, variables).strip() for line in option_array if line.strip()])
                 elif option.get("options"):
-                    choices.extend(
-                        apply_variables(txt, variables) for txt in option["options"]
-                    )
+                    choices.extend(apply_variables(txt, variables) for txt in option["options"])
                 if len(choices) == 0:
                     await self.notify_info("command didn't return anything")
                     return
 
                 if autovalidate and len(choices) == 1:
                     variables[var_name] = choices[0]
                 else:
                     selection = await self.menu.run(choices, var_name)
-                    variables[var_name] = apply_filter(selection, option.get("filter"))
+                    variables[var_name] = apply_filter(selection, cast(str, option.get("filter", "")))
                     self.log.debug("set %s = %s", var_name, variables[var_name])
 
-    async def _run_command(self, command, variables):
-        "Runs a shell `command`, optionally replacing `variables`"
+    async def _run_command(self, command: str, variables: dict[str, str]) -> None:
+        """Run a shell `command`, optionally replacing `variables`.
+
+        The command is run in a shell, and the variables are replaced using the `apply_variables` function.
+
+        Args:
+            command: The command to run.
+            variables: The variables to replace in the command.
+        """
         final_command = apply_variables(command, variables)
         self.log.info("Executing %s", final_command)
         await asyncio.create_subprocess_shell(final_command)
```

### Comparing `pyprland-2.2.9/pyprland/plugins/system_notifier.py` & `pyprland-2.3.0/pyprland/plugins/system_notifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,23 @@
-" Add system notifications based on journal logs "
-import re
+"""Add system notifications based on journal logs."""
+
 import asyncio
-from typing import cast
+import contextlib
+import re
 from copy import deepcopy
-from .interface import Plugin
-from ..common import apply_filter
+from typing import cast
+
 from ..adapters.colors import convert_color
+from ..common import apply_filter
+from .interface import Plugin
+
+try:
+    from asyncio.subprocess import Process
+except ImportError:
+    from asyncio import Process  # type: ignore
 
 builtin_parsers = {
     "journal": [
         {
             "pattern": r"([a-z0-9]+): Link UP$",
             "filter": r"s/.*\[\d+\]: ([a-z0-9]+): Link.*/\1 is active/",
             "color": "#00aa00",
@@ -29,91 +37,96 @@
             "filter": r"s/.*usb \d+-[0-9.]+: Product: (.*)/USB plugged: \1/",
         },
     ]
 }
 
 
 class Extension(Plugin):
-    "The plugin code"
+    """Notification system from live apps & logs."""
 
-    def __init__(self, name):
+    def __init__(self, name: str) -> None:
+        """Initialize the class."""
         super().__init__(name)
         self.tasks: list[asyncio.Task] = []
-        self.sources = {}
-        self.parsers = {}
+        self.sources: dict[str, Process] = {}
+        self.parsers: dict[str, asyncio.Queue] = {}
         self.running = True
 
-    async def on_reload(self):
+    async def on_reload(self) -> None:
+        """Reload the plugin."""
         await self.exit()
         self.running = True
         parsers = deepcopy(builtin_parsers)
         parsers.update(self.config.get("parsers", {}))
         for name, pprops in parsers.items():
             self.tasks.append(asyncio.create_task(self.start_parser(name, pprops)))
             self.parsers[name] = asyncio.Queue()
             self.log.debug("Loaded parser %s", name)
 
         for props in self.config.get("sources", []):
-            assert (
-                props["parser"] in self.parsers
-            ), f"{props['parser']} was not found in {self.parsers}"
+            assert props["parser"] in self.parsers, f"{props['parser']} was not found in {self.parsers}"
             self.log.debug("Loaded source %s => %s", props["command"], props["parser"])
             self.tasks.append(asyncio.create_task(self.start_source(props)))
 
-    async def exit(self):
-        "exit function"
+    async def exit(self) -> None:
+        """Exit function."""
         self.running = False
         for task in self.tasks:
             task.cancel()
-            try:
+            with contextlib.suppress(asyncio.CancelledError):
                 await task
-            except asyncio.CancelledError:
-                pass
         for source in self.sources.values():
             if source.pid is not None:
                 source.kill()
         self.tasks[:] = []
 
-    async def start_source(self, props):
-        "Start a source loop"
+    async def start_source(self, props: dict[str, str]) -> None:
+        """Start a source loop.
+
+        A source is a command that will be executed and its stdout will be read line by line.
 
-        parsers = (
-            [props["parser"]] if isinstance(props["parser"], str) else props["parser"]
-        )
+        Args:
+            props: A dictionary with the following keys:
+                - command: The command to execute.
+                - parser: The name of the parser to use.
+        """
+        parsers = [props["parser"]] if isinstance(props["parser"], str) else props["parser"]
         queues = [self.parsers[p] for p in parsers]
-        proc = await asyncio.create_subprocess_shell(
-            props["command"], stdout=asyncio.subprocess.PIPE
-        )
+        proc = await asyncio.create_subprocess_shell(props["command"], stdout=asyncio.subprocess.PIPE)
 
         self.sources[props["command"]] = proc
         assert proc.stdout
         await asyncio.sleep(1)
         # Read stdout line by line and push to parser
         while proc.returncode is None and self.running:
             line = (await proc.stdout.readline()).decode().strip()
             if line:
                 for q in queues:
                     await q.put(line)
 
-    async def start_parser(self, name, props: list):
-        "Start a parser loop"
+    async def start_parser(self, name: str, props: list) -> None:
+        """Start a parser loop.
+
+        Args:
+            name: The name of the parser.
+            props: A list of dictionaries with the following keys:
+                - pattern: A regex pattern to match.
+                - filter: A filter to apply to the matched line.
+                - color: The color to use in the notification.
+        """
         q = self.parsers[name]
-        rules = []
         default_color = self.config.get("default_color", "#5555AA")
-        for prop in props:
-            rules.append(
-                {
-                    "pattern": re.compile(prop["pattern"]),
-                    "filter": prop.get("filter"),
-                    "color": convert_color(prop.get("color", default_color)),
-                }
-            )
+        rules = [
+            {
+                "pattern": re.compile(prop["pattern"]),
+                "filter": prop.get("filter"),
+                "color": convert_color(prop.get("color", default_color)),
+            }
+            for prop in props
+        ]
         while self.running:
             content = await q.get()
             for rule in rules:
                 if rule["pattern"].search(content):
-                    if rule["filter"]:
-                        text = apply_filter(content, cast(str, rule["filter"]))
-                    else:
-                        text = content
+                    text = apply_filter(content, cast(str, rule["filter"])) if rule["filter"] else content
                     await self.notify(text, color=rule["color"])
                     await asyncio.sleep(0.01)
```

### Comparing `pyprland-2.2.9/pyprland/plugins/toggle_special.py` & `pyprland-2.3.0/pyprland/plugins/toggle_special.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-""" toggle_special allows having an "expose" like selection of windows in a special group
-"""
+"""toggle_special allows having an "expose" like selection of windows in a special group."""
 
 from typing import cast
 
-from .interface import Plugin
 from ..common import state
+from .interface import Plugin
 
 
 class Extension(Plugin):  # pylint: disable=missing-class-docstring
-    async def run_toggle_special(self, special_workspace="minimized"):
-        """[name] Toggles switching the focused window to the special workspace "name" (default: minimized)"""
-        aw = cast(dict, await self.hyprctlJSON("activewindow"))
+    """Toggle switching the focused window to a special workspace."""
+
+    async def run_toggle_special(self, special_workspace: str = "minimized") -> None:
+        """[name] Toggles switching the focused window to the special workspace "name" (default: minimized)."""
+        aw = cast(dict, await self.hyprctl_json("activewindow"))
         wid = aw["workspace"]["id"]
         assert isinstance(wid, int)
         if wid < 1:  # special workspace
             await self.hyprctl(
                 [
                     f"togglespecialworkspace {special_workspace}",
                     f"movetoworkspacesilent {state.active_workspace},address:{aw['address']}",
                     f"focuswindow address:{aw['address']}",
                 ]
             )
         else:
-            await self.hyprctl(
-                f"movetoworkspacesilent special:{special_workspace},address:{aw['address']}"
-            )
+            await self.hyprctl(f"movetoworkspacesilent special:{special_workspace},address:{aw['address']}")
```

### Comparing `pyprland-2.2.9/pyprland/plugins/wallpapers.py` & `pyprland-2.3.0/pyprland/plugins/wallpapers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,106 +1,107 @@
-" Plugin template "
-import random
+"""Plugin template."""
+
 import asyncio
 import os.path
+import random
+from collections.abc import AsyncIterator
 
 from aiofiles.os import listdir
 
+from ..common import CastBoolMixin, apply_variables, prepare_for_quotes, state
 from .interface import Plugin
-from ..common import CastBoolMixin, apply_variables, state, prepare_for_quotes
 
 
-async def get_files_with_ext(path, extensions, recurse=True):
-    "Returns files matching `extension` in given `path`. Can optionally `recurse` subfolders."
+def expand_path(path: str) -> str:
+    """Expand the path."""
+    return os.path.expanduser(os.path.expandvars(path))
+
+
+async def get_files_with_ext(path: str, extensions: list[str], recurse: bool = True) -> AsyncIterator[str]:
+    """Return files matching `extension` in given `path`. Can optionally `recurse` subfolders.."""
     for fname in await listdir(path):
         ext = fname.rsplit(".", 1)[-1]
         full_path = os.path.join(path, fname)
         if ext.lower() in extensions:
             yield full_path
         elif recurse and os.path.isdir(full_path):
             async for v in get_files_with_ext(full_path, extensions, True):
                 yield v
 
 
 class Extension(CastBoolMixin, Plugin):
-    "Manages the background image"
+    """Manages the background image."""
 
-    default_image_ext: set[str] | list[str] = set(("png", "jpg", "jpeg"))
+    default_image_ext: set[str] | list[str] = {"png", "jpg", "jpeg"}
     image_list: list[str] = []
     running = True
     proc: list = []
     loop = None
 
     next_background_event = asyncio.Event()
     cur_image = ""
 
-    async def on_reload(self):
-        "Re-build the image list"
+    async def on_reload(self) -> None:
+        """Re-build the image list."""
         cfg_path = self.config["path"]
-        paths = [cfg_path] if isinstance(cfg_path, str) else list(cfg_path)
+        paths = [expand_path(cfg_path)] if isinstance(cfg_path, str) else [expand_path(p) for p in cfg_path]
         extensions = self.config.get("extensions", self.default_image_ext)
 
         self.image_list = [
             os.path.join(path, fname)
             for path in paths
-            async for fname in get_files_with_ext(
-                path, extensions, recurse=self.cast_bool(self.config.get("recurse"))
-            )
+            async for fname in get_files_with_ext(path, extensions, recurse=self.cast_bool(self.config.get("recurse")))
         ]
 
         # Start the main loop if it's the first load of the config
         if self.loop is None:
             self.loop = asyncio.create_task(self.main_loop())
 
-    async def exit(self):
-        "terminates gracefully"
+    async def exit(self) -> None:
+        """Terminates gracefully."""
         self.running = False
         if self.loop:
             self.loop.cancel()
         await self.terminate()
 
-    async def event_monitoradded(self, _):
-        "When a new monitor is added, set the background"
+    async def event_monitoradded(self, _: str) -> None:
+        """When a new monitor is added, set the background."""
         self.next_background_event.set()
 
-    def select_next_image(self):
-        "Returns the next image (random is supported for now)"
+    def select_next_image(self) -> str:
+        """Return the next image (random is supported for now)."""
         choice = random.choice(self.image_list)
         if choice == self.cur_image:
             choice = random.choice(self.image_list)
         self.cur_image = choice
         return choice
 
-    async def _run_one(self, template, values):
-        "Runs one command"
+    async def _run_one(self, template: str, values: dict[str, str]) -> None:
+        """Run one command."""
         cmd = apply_variables(template, values)
         self.log.info("Running %s", cmd)
         self.proc.append(await asyncio.create_subprocess_shell(cmd))
 
-    async def main_loop(self):
-        "Main plugin loop, runs in the 'background'"
+    async def main_loop(self) -> None:
+        """Run the main plugin loop in the 'background'."""
         self.proc = []
         unique = self.config.get("unique", False)
         variables = state.variables.copy()
 
         while self.running:
             self.next_background_event.clear()
 
             # Define the command template based on the 'unique' flag
             cmd_template = self.config.get(
                 "command",
-                (
-                    'swaybg -o [output] -m fill -i "[file]"'
-                    if unique
-                    else 'swaybg -m fill -i "[file]"'
-                ),
+                ('swaybg -o [output] -m fill -i "[file]"' if unique else 'swaybg -m fill -i "[file]"'),
             )
 
             if unique:
-                monitors = await self.hyprctlJSON("monitors")
+                monitors = await self.hyprctl_json("monitors")
                 old_filename = None
                 for monitor in monitors:
                     filename = prepare_for_quotes(self.select_next_image())
                     while filename == old_filename:
                         filename = prepare_for_quotes(self.select_next_image())
                     variables.update({"file": filename, "output": monitor["name"]})
                     await self._run_one(cmd_template, variables)
@@ -123,25 +124,25 @@
                     asyncio.create_task(self.next_background_event.wait()),
                 ],
                 return_when=asyncio.FIRST_COMPLETED,
             )
 
             await self.terminate()
 
-    async def terminate(self):
-        "Exits existing process if any"
+    async def terminate(self) -> None:
+        """Exit existing process if any."""
         if self.proc:
             for proc in self.proc:
                 if proc.returncode is None:
                     proc.terminate()
                 await proc.wait()
         self.proc[:] = []
 
-    async def run_wall(self, arg):
-        "<next|clear> skip the current background image or stop displaying it"
+    async def run_wall(self, arg: str) -> None:
+        """<next|clear> skip the current background image or stop displaying it."""
         if arg.startswith("n"):
             self.next_background_event.set()
         elif arg.startswith("c"):
             clear_command = self.config.get("clear_command")
             if clear_command:
                 # call clear_command subprocess
                 proc = await asyncio.create_subprocess_shell(clear_command)
```

### Comparing `pyprland-2.2.9/pyprland/plugins/workspaces_follow_focus.py` & `pyprland-2.3.0/pyprland/plugins/workspaces_follow_focus.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,60 @@
-""" Force workspaces to follow the focus / mouse """
+"""Force workspaces to follow the focus / mouse."""
 
 from typing import cast
 
 from .interface import Plugin
 
 
 class Extension(Plugin):  # pylint: disable=missing-class-docstring
+    """Force workspaces to follow the focus / mouse."""
+
     workspace_list: list[int] = []
 
-    async def on_reload(self):
-        "rebuild workspaces list"
+    async def on_reload(self) -> None:
+        """Rebuild workspaces list."""
         self.workspace_list = list(range(1, self.config.get("max_workspaces", 10) + 1))
 
-    async def event_focusedmon(self, screenid_name):
-        "reacts to monitor changes"
+    async def event_focusedmon(self, screenid_name: str) -> None:
+        """Reacts to monitor changes."""
         monitor_id, workspace_name = screenid_name.split(",")
         # move every free workspace to the currently focused desktop
-        busy_workspaces = set(
-            mon["activeWorkspace"]["name"]
-            for mon in cast(list[dict], await self.hyprctlJSON("monitors"))
-            if mon["name"] != monitor_id
-        )
-        workspaces = [
-            w["name"]
-            for w in cast(list[dict], await self.hyprctlJSON("workspaces"))
-            if w["id"] > 0
-        ]
+        busy_workspaces = {
+            mon["activeWorkspace"]["name"] for mon in cast(list[dict], await self.hyprctl_json("monitors")) if mon["name"] != monitor_id
+        }
+        workspaces = [w["name"] for w in cast(list[dict], await self.hyprctl_json("workspaces")) if w["id"] > 0]
 
         batch: list[str] = []
         for n in workspaces:
             if n in busy_workspaces or n == workspace_name:
                 continue
             batch.append(f"moveworkspacetomonitor name:{n} {monitor_id}")
         await self.hyprctl(batch)
 
-    async def run_change_workspace(self, direction: str):
-        """<+1/-1> Switch workspaces of current monitor, avoiding displayed workspaces"""
+    async def run_change_workspace(self, direction: str) -> None:
+        """<+1/-1> Switch workspaces of current monitor, avoiding displayed workspaces."""
         increment = int(direction)
         # get focused screen info
-        monitors = await self.hyprctlJSON("monitors")
+        monitors = await self.hyprctl_json("monitors")
         assert isinstance(monitors, list)
         for monitor in monitors:
             if monitor["focused"]:
                 break
         else:
             self.log.error("Can not find a focused monitor")
             return
         assert isinstance(monitor, dict)
-        busy_workspaces = set(
-            m["activeWorkspace"]["id"] for m in monitors if m["id"] != monitor["id"]
-        )
+        busy_workspaces = {m["activeWorkspace"]["id"] for m in monitors if m["id"] != monitor["id"]}
         cur_workspace = monitor["activeWorkspace"]["id"]
-        available_workspaces = [
-            i for i in self.workspace_list if i not in busy_workspaces
-        ]
+        available_workspaces = [i for i in self.workspace_list if i not in busy_workspaces]
         try:
             idx = available_workspaces.index(cur_workspace)
         except ValueError:
             next_workspace = available_workspaces[0 if increment > 0 else -1]
         else:
-            next_workspace = available_workspaces[
-                (idx + increment) % len(available_workspaces)
-            ]
+            next_workspace = available_workspaces[(idx + increment) % len(available_workspaces)]
         await self.hyprctl(
             [
                 f"moveworkspacetomonitor {next_workspace},{monitor['name']}",
                 f"workspace {next_workspace}",
             ]
         )
```

### Comparing `pyprland-2.2.9/PKG-INFO` & `pyprland-2.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprland
-Version: 2.2.9
+Version: 2.3.0
 Summary: Hyperland plugin system - batteries included
 Home-page: https://github.com/hyprland-community/pyprland/
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,65 +13,92 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Description-Content-Type: text/markdown
 
 ![rect](https://github.com/hyprland-community/pyprland/assets/238622/3fab93b6-6445-4e7b-b757-035095b5c8e8)
 
 [![Hyprland](https://img.shields.io/badge/Made%20for-Hyprland-blue)](https://github.com/hyprwm/Hyprland)
-[![Discord](https://img.shields.io/discord/1055990214411169892?label=discord)](https://discord.gg/zzWqvcKRMy)
+[![Discord](https://img.shields.io/discord/1055990214411169892?label=discord)](https://discord.com/channels/1055990214411169892/1230972154330218526)
 
 [Documentation](https://github.com/hyprland-community/pyprland/wiki) • [Discussions](https://github.com/hyprland-community/pyprland/discussions) • [Changes History](https://github.com/hyprland-community/pyprland/releases) • [Share Your Setup](https://github.com/hyprland-community/pyprland/discussions/46)
 
 
 ## Enhance your Hyprland experience with Pyprland
 
 Welcome to Pyprland, your gateway to extending the capabilities of [Hyprland](https://hyprland.org/). Pyprland offers a plethora of plugins designed for simplicity and efficiency, allowing you to supercharge your productivity and customize your user experience.
 
+You can think of it as a *Gnome tweak tool* but for Hyprland users (involves editing text files). With a "100%" plugin-based architecture, Pyprland is designed to be lightweight and easy to use.
+
+Note that usage of Python and architecture of the software encourages using many plugins with little impact on the footprint and performance.
+
+Contributions, suggestions, bug reports and comments are welcome.
+
 - Explore our variety of [plugins](https://github.com/hyprland-community/pyprland/wiki/Plugins) to tailor your Hyprland setup to your liking.
 - New users, check the [getting started](https://github.com/hyprland-community/pyprland/wiki/Getting-started) guide.
 
 
-## About Pyprland
+<details>
+<summary>
+About Pyprland
+</summary>
+
+Latest stable is: **2.2.20**
 
 [![Packaging Status](https://repology.org/badge/vertical-allrepos/pyprland.svg)](https://repology.org/project/pyprland/versions)
 
 🎉 Hear what others are saying:
 - ["It just works very very well" - The Linux Cast (video)](https://youtu.be/Cjn0SFyyucY?si=hGb0TM9IDvlbcD6A&t=131) - February 2024
 - [You NEED This in your Hyprland Config - LibrePhoenix (video)](https://www.youtube.com/watch?v=CwGlm-rpok4) - October 2023 (*Now [TOML](https://toml.io/en/) format is preferred over [JSON](https://www.w3schools.com/js/js_json_intro.asp))
+</details>
 
-## Contributing
+<details>
+
+<summary>
+Contributing
+</summary>
 
 Check out the [creating a pull request](https://docs.github.com/fr/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) document for guidance.
 
 - Report bugs or propose features [here](https://github.com/hyprland-community/pyprland/issues)
 - Improve our [wiki](https://github.com/hyprland-community/pyprland/wiki)
 
 and if you have coding skills you can also
 
 - Enhance the coverage of our [tests](https://github.com/hyprland-community/pyprland/tree/main/tests)
 - Propose & write new plugins or enhancements
 
-## Dependencies
+</details>
+
+<details>
+<summary>
+Dependencies
+</summary>
 
 - **Hyprland** >= 0.37
 - **Python** >= 3.11
     - **aiofiles**
+</details>
 
-## Latest major changes
+<details>
+<summary>
+Latest major changes
+</summary>
 
-> [!note]
-> Check the [Releases change log](https://github.com/hyprland-community/pyprland/releases) for more information
+Check the [Releases change log](https://github.com/hyprland-community/pyprland/releases) for more information
 
 ### 2.2
 
 - Added [wallpapers](https://github.com/hyprland-community/pyprland/wiki/wallpapers) and [system_notifier](https://github.com/hyprland-community/pyprland/wiki/system_notifier) plugins.
-- Refactor in 2.2.5
-  - updated the syntax for [wallpapers](https://github.com/hyprland-community/pyprland/wiki/wallpapers)
-  - deprecated `class_match` in [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads)
+- Deprecated [class_match](https://github.com/hyprland-community/pyprland/wiki/scratchpads_nonstandard) in [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads)
 - Added [gbar](https://github.com/hyprland-community/pyprland/wiki/gbar) in 2.2.6
+- [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads) supports multiple client windows (using 2.2.19 is recommended)
+- [Monitors](https://github.com/hyprland-community/pyprland/wiki/monitors) and [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads) supports rotation in 2.2.13
+- Improve [Nix support](https://github.com/hyprland-community/pyprland/wiki/Nix)
+
+
 ### 2.1
 
 - Requires Hyprland >= 0.37
 - [Monitors](https://github.com/hyprland-community/pyprland/wiki/monitors) plugin improvements.
 
 ### 2.0
 
@@ -87,15 +114,15 @@
 - Introduced [shortcuts_menu](https://github.com/hyprland-community/pyprland/wiki/shortcuts_menu) plugin.
 
 ### 1.8
 
 - Requires Hyprland >= 0.30
 - Added [layout_center](https://github.com/hyprland-community/pyprland/wiki/layout_center) plugin.
 
-## Star History
+</details>
 
 <a href="https://star-history.com/#fdev31/pyprland&Date">
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=fdev31/pyprland&type=Timeline&theme=dark" />
     <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=fdev31/pyprland&type=Timeline" />
     <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=fdev31/pyprland&type=Timeline" />
   </picture>
```

