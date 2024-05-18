# Comparing `tmp/torchsense-0.0.4.tar.gz` & `tmp/torchsense-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchsense-0.0.4.tar", last modified: Thu May 16 08:24:09 2024, max compression
+gzip compressed data, was "torchsense-0.0.5.tar", last modified: Sat May 18 12:32:33 2024, max compression
```

## Comparing `torchsense-0.0.4.tar` & `torchsense-0.0.5.tar`

### file list

```diff
@@ -1,71 +1,80 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 08:24:09.154198 torchsense-0.0.4/
--rw-rw-rw-   0        0        0     1090 2024-05-05 06:37:08.000000 torchsense-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1665 2024-05-16 08:24:09.152194 torchsense-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2839 2024-05-14 01:10:06.000000 torchsense-0.0.4/README.md
--rw-rw-rw-   0        0        0      573 2024-05-16 08:23:49.000000 torchsense-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 08:24:09.154198 torchsense-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-16 08:24:08.952910 torchsense-0.0.4/tests/
--rw-rw-rw-   0        0        0     1445 2024-05-15 16:08:03.000000 torchsense-0.0.4/tests/test_model.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:24:08.952910 torchsense-0.0.4/torchsense/
--rw-rw-rw-   0        0        0        2 2024-05-16 08:20:27.000000 torchsense-0.0.4/torchsense/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:24:08.989338 torchsense-0.0.4/torchsense/datasets/
--rw-rw-rw-   0        0        0        0 2024-05-05 06:50:01.000000 torchsense-0.0.4/torchsense/datasets/__init__.py
--rw-rw-rw-   0        0        0     4719 2024-05-15 12:44:20.000000 torchsense-0.0.4/torchsense/datasets/custom_folder.py
--rw-rw-rw-   0        0        0     5076 2024-05-13 11:17:11.000000 torchsense-0.0.4/torchsense/datasets/dataset2.py
--rw-rw-rw-   0        0        0    11046 2024-05-15 12:44:20.000000 torchsense-0.0.4/torchsense/datasets/folder.py
--rw-rw-rw-   0        0        0     2505 2024-05-13 11:17:11.000000 torchsense-0.0.4/torchsense/datasets/utils.py
--rw-rw-rw-   0        0        0     4281 2024-05-13 11:17:11.000000 torchsense-0.0.4/torchsense/datasets/vision.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:24:09.113258 torchsense-0.0.4/torchsense/models/
--rw-rw-rw-   0        0        0     4213 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/Autoencode.py
--rw-rw-rw-   0        0        0     4213 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/Autoencoder.py
--rw-rw-rw-   0        0        0     6353 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/LSTM.py
--rw-rw-rw-   0        0        0      130 2024-05-15 15:59:59.000000 torchsense-0.0.4/torchsense/models/__init__.py
--rw-rw-rw-   0        0        0     3531 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/alexnet.py
--rw-rw-rw-   0        0        0    12106 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/attention.py
--rw-rw-rw-   0        0        0    12316 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/cct.py
--rw-rw-rw-   0        0        0      780 2024-05-15 11:05:37.000000 torchsense-0.0.4/torchsense/models/cnn4.py
--rw-rw-rw-   0        0        0     5012 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/deeplab.py
--rw-rw-rw-   0        0        0     5672 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/deeplabv3p.py
--rw-rw-rw-   0        0        0     5216 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/densenet.py
--rw-rw-rw-   0        0        0     4632 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/googlenet.py
--rw-rw-rw-   0        0        0    11215 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/inceptionv3.py
--rw-rw-rw-   0        0        0    18657 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/inceptionv4.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:24:09.121255 torchsense-0.0.4/torchsense/models/lit_model/
--rw-rw-rw-   0        0        0      142 2024-05-15 11:43:35.000000 torchsense-0.0.4/torchsense/models/lit_model/__init__.py
--rw-rw-rw-   0        0        0     2345 2024-05-15 11:39:31.000000 torchsense-0.0.4/torchsense/models/lit_model/litclassmodel.py
--rw-rw-rw-   0        0        0     2342 2024-05-15 11:43:35.000000 torchsense-0.0.4/torchsense/models/lit_model/litregressmodel.py
--rw-rw-rw-   0        0        0     5629 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/mobilenet.py
--rw-rw-rw-   0        0        0     7696 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/mobilenetv1.py
--rw-rw-rw-   0        0        0     7973 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/mobilenetv2.py
--rw-rw-rw-   0        0        0     9749 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/mobilenetv3.py
--rw-rw-rw-   0        0        0     9920 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/nasnet.py
--rw-rw-rw-   0        0        0     4028 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/preactresnet.py
--rw-rw-rw-   0        0        0     6796 2024-05-15 16:06:20.000000 torchsense-0.0.4/torchsense/models/resnet.py
--rw-rw-rw-   0        0        0     4440 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/resnext.py
--rw-rw-rw-   0        0        0     7217 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/rir.py
--rw-rw-rw-   0        0        0     5759 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/sealex.py
--rw-rw-rw-   0        0        0     5458 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/senet.py
--rw-rw-rw-   0        0        0     7695 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/shufflenet.py
--rw-rw-rw-   0        0        0     4953 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/shufflenetv2.py
--rw-rw-rw-   0        0        0     3840 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/simple_vit_1d.py
--rw-rw-rw-   0        0        0     2540 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/squeezenet.py
--rw-rw-rw-   0        0        0     7722 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/stochasticdepth.py
--rw-rw-rw-   0        0        0     4170 2024-05-14 01:33:19.000000 torchsense-0.0.4/torchsense/models/unet.py
--rw-rw-rw-   0        0        0     2114 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/vgg.py
--rw-rw-rw-   0        0        0     6935 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/vit.py
--rw-rw-rw-   0        0        0     3358 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/wideresidual.py
--rw-rw-rw-   0        0        0     6339 2024-05-05 06:37:08.000000 torchsense-0.0.4/torchsense/models/xception.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:24:09.129684 torchsense-0.0.4/torchsense/trainer/
--rw-rw-rw-   0        0        0       48 2024-05-13 12:49:15.000000 torchsense-0.0.4/torchsense/trainer/__init__.py
--rw-rw-rw-   0        0        0      727 2024-05-15 11:43:35.000000 torchsense-0.0.4/torchsense/trainer/trainer.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:24:09.129684 torchsense-0.0.4/torchsense/transforms/
--rw-rw-rw-   0        0        0        0 2024-05-05 06:49:52.000000 torchsense-0.0.4/torchsense/transforms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:24:09.129684 torchsense-0.0.4/torchsense/utils/
--rw-rw-rw-   0        0        0        0 2024-05-13 11:12:46.000000 torchsense-0.0.4/torchsense/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:24:09.137734 torchsense-0.0.4/torchsense.egg-info/
--rw-rw-rw-   0        0        0     1665 2024-05-16 08:24:08.000000 torchsense-0.0.4/torchsense.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1774 2024-05-16 08:24:08.000000 torchsense-0.0.4/torchsense.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 08:24:08.000000 torchsense-0.0.4/torchsense.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 08:24:08.000000 torchsense-0.0.4/torchsense.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-16 08:24:08.000000 torchsense-0.0.4/torchsense.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 12:32:33.129955 torchsense-0.0.5/
+-rw-rw-rw-   0        0        0     1090 2024-05-05 06:37:08.000000 torchsense-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1665 2024-05-18 12:32:33.128078 torchsense-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3065 2024-05-16 08:38:02.000000 torchsense-0.0.5/README.md
+-rw-rw-rw-   0        0        0      573 2024-05-18 12:32:20.000000 torchsense-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-18 12:32:33.129955 torchsense-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-18 12:32:32.975534 torchsense-0.0.5/tests/
+-rw-rw-rw-   0        0        0     1445 2024-05-15 16:08:03.000000 torchsense-0.0.5/tests/test_model.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:32:32.977753 torchsense-0.0.5/torchsense/
+-rw-rw-rw-   0        0        0        2 2024-05-16 08:20:27.000000 torchsense-0.0.5/torchsense/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:32:33.001491 torchsense-0.0.5/torchsense/datasets/
+-rw-rw-rw-   0        0        0        0 2024-05-05 06:50:01.000000 torchsense-0.0.5/torchsense/datasets/__init__.py
+-rw-rw-rw-   0        0        0     4811 2024-05-18 11:16:08.000000 torchsense-0.0.5/torchsense/datasets/custom.py
+-rw-rw-rw-   0        0        0     5076 2024-05-13 11:17:11.000000 torchsense-0.0.5/torchsense/datasets/dataset2.py
+-rw-rw-rw-   0        0        0    11200 2024-05-18 11:24:48.000000 torchsense-0.0.5/torchsense/datasets/folder.py
+-rw-rw-rw-   0        0        0     3433 2024-05-18 11:28:37.000000 torchsense-0.0.5/torchsense/datasets/utils.py
+-rw-rw-rw-   0        0        0     4344 2024-05-18 09:04:23.000000 torchsense-0.0.5/torchsense/datasets/vision.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:32:33.097710 torchsense-0.0.5/torchsense/models/
+-rw-rw-rw-   0        0        0     4213 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/Autoencode.py
+-rw-rw-rw-   0        0        0     4213 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/Autoencoder.py
+-rw-rw-rw-   0        0        0     6353 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/LSTM.py
+-rw-rw-rw-   0        0        0      130 2024-05-15 15:59:59.000000 torchsense-0.0.5/torchsense/models/__init__.py
+-rw-rw-rw-   0        0        0     3531 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/alexnet.py
+-rw-rw-rw-   0        0        0    12106 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/attention.py
+-rw-rw-rw-   0        0        0    12316 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/cct.py
+-rw-rw-rw-   0        0        0      780 2024-05-15 11:05:37.000000 torchsense-0.0.5/torchsense/models/cnn4.py
+-rw-rw-rw-   0        0        0     5012 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/deeplab.py
+-rw-rw-rw-   0        0        0     5672 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/deeplabv3p.py
+-rw-rw-rw-   0        0        0     5216 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/densenet.py
+-rw-rw-rw-   0        0        0    11223 2024-05-17 10:48:08.000000 torchsense-0.0.5/torchsense/models/gan_g.py
+-rw-rw-rw-   0        0        0     4632 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/googlenet.py
+-rw-rw-rw-   0        0        0    11215 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/inceptionv3.py
+-rw-rw-rw-   0        0        0    18657 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/inceptionv4.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:32:33.105927 torchsense-0.0.5/torchsense/models/lit_model/
+-rw-rw-rw-   0        0        0      215 2024-05-17 13:37:52.000000 torchsense-0.0.5/torchsense/models/lit_model/__init__.py
+-rw-rw-rw-   0        0        0     2345 2024-05-15 11:39:31.000000 torchsense-0.0.5/torchsense/models/lit_model/lit_classify.py
+-rw-rw-rw-   0        0        0     2231 2024-05-17 13:37:52.000000 torchsense-0.0.5/torchsense/models/lit_model/lit_multimodal.py
+-rw-rw-rw-   0        0        0     2228 2024-05-17 08:53:55.000000 torchsense-0.0.5/torchsense/models/lit_model/lit_regression.py
+-rw-rw-rw-   0        0        0     5629 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/mobilenet.py
+-rw-rw-rw-   0        0        0     7696 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/mobilenetv1.py
+-rw-rw-rw-   0        0        0     7973 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/mobilenetv2.py
+-rw-rw-rw-   0        0        0     9749 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/mobilenetv3.py
+-rw-rw-rw-   0        0        0     9920 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/nasnet.py
+-rw-rw-rw-   0        0        0     4028 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/preactresnet.py
+-rw-rw-rw-   0        0        0     6796 2024-05-15 16:06:20.000000 torchsense-0.0.5/torchsense/models/resnet.py
+-rw-rw-rw-   0        0        0     4440 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/resnext.py
+-rw-rw-rw-   0        0        0     7217 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/rir.py
+-rw-rw-rw-   0        0        0     5759 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/sealex.py
+-rw-rw-rw-   0        0        0     5458 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/senet.py
+-rw-rw-rw-   0        0        0     7695 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/shufflenet.py
+-rw-rw-rw-   0        0        0     4953 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/shufflenetv2.py
+-rw-rw-rw-   0        0        0     3840 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/simple_vit_1d.py
+-rw-rw-rw-   0        0        0     2540 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/squeezenet.py
+-rw-rw-rw-   0        0        0     7722 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/stochasticdepth.py
+-rw-rw-rw-   0        0        0     4170 2024-05-14 01:33:19.000000 torchsense-0.0.5/torchsense/models/unet.py
+-rw-rw-rw-   0        0        0     2114 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/vgg.py
+-rw-rw-rw-   0        0        0     6935 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/vit.py
+-rw-rw-rw-   0        0        0     3358 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/wideresidual.py
+-rw-rw-rw-   0        0        0     6339 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/xception.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:32:33.110021 torchsense-0.0.5/torchsense/trainer/
+-rw-rw-rw-   0        0        0       48 2024-05-13 12:49:15.000000 torchsense-0.0.5/torchsense/trainer/__init__.py
+-rw-rw-rw-   0        0        0      913 2024-05-17 13:37:52.000000 torchsense-0.0.5/torchsense/trainer/trainer.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:32:33.115322 torchsense-0.0.5/torchsense/transforms/
+-rw-rw-rw-   0        0        0      261 2024-05-18 12:25:32.000000 torchsense-0.0.5/torchsense/transforms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:32:33.122915 torchsense-0.0.5/torchsense/transforms/augmentations/
+-rw-rw-rw-   0        0        0        0 2024-05-05 06:49:52.000000 torchsense-0.0.5/torchsense/transforms/augmentations/__init__.py
+-rw-rw-rw-   0        0        0      713 2024-05-18 12:32:20.000000 torchsense-0.0.5/torchsense/transforms/augmentations/interpolate.py
+-rw-rw-rw-   0        0        0      612 2024-05-18 11:19:22.000000 torchsense-0.0.5/torchsense/transforms/augmentations/normalize.py
+-rw-rw-rw-   0        0        0      800 2024-05-18 11:31:59.000000 torchsense-0.0.5/torchsense/transforms/augmentations/to_tensor.py
+-rw-rw-rw-   0        0        0      379 2024-05-18 12:29:31.000000 torchsense-0.0.5/torchsense/transforms/augmentations/utils.py
+-rw-rw-rw-   0        0        0     6047 2024-05-18 07:44:50.000000 torchsense-0.0.5/torchsense/transforms/compose.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:32:33.124150 torchsense-0.0.5/torchsense/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-13 11:12:46.000000 torchsense-0.0.5/torchsense/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:32:33.126668 torchsense-0.0.5/torchsense.egg-info/
+-rw-rw-rw-   0        0        0     1665 2024-05-18 12:32:32.000000 torchsense-0.0.5/torchsense.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2113 2024-05-18 12:32:32.000000 torchsense-0.0.5/torchsense.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 12:32:32.000000 torchsense-0.0.5/torchsense.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 12:32:32.000000 torchsense-0.0.5/torchsense.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-18 12:32:32.000000 torchsense-0.0.5/torchsense.egg-info/top_level.txt
```

### Comparing `torchsense-0.0.4/LICENSE` & `torchsense-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/PKG-INFO` & `torchsense-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchsense
-Version: 0.0.4
+Version: 0.0.5
 Summary: Torchsense is a library for sensor data processing with PyTorch
 Author-email: Xingwei Wang <wxwjkl123@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Xingwei Wang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `torchsense-0.0.4/README.md` & `torchsense-0.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 
+
 # TorchSense
+
 <div>
 <a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-ee4c2c?logo=pytorch&logoColor=white"></a>
 <a href="https://pytorchlightning.ai/"><img alt="Lightning" src="https://img.shields.io/badge/-Lightning-792ee5?logo=pytorchlightning&logoColor=white"></a>
 
 </div>
 
 ## Description
@@ -36,20 +38,24 @@
     └── class_y
         ├── 123.ext
         ├── nsdf3.ext
         └── ...
         └── asd932_.ext
 ```
 
-
-## How to run
-torchsense provide two-way to run model
 ### Train model with default configuration
 
-```python 
+<details>
+<summary>Show details</summary>
+
+you can only use our data loader
+
+- the only you need to input are `list1`and `data_path`
+
+```python
 # ensure you already install torch and lightning
 from torchsense.datasets.folder import SensorFolder
 from torch.utils.data import DataLoader
 
 # you need to input
 list1 = [key1,key2,key3] # example ["acc", "mix_mic", "mic"]
 root_data = "data1" # data1 root path
@@ -61,16 +67,26 @@
 test_loader = DataLoader(test_set, batch_size=1, shuffle=False)
 
 for i, batch in enumerate(train_loader):
     acc, mix, mic = batch[0]
     # ... train your self
 ```
 
-now model only support .mat file
+</details>
+
+
+
 ### Train model with custom configuration
+
+<details>
+<summary>Show details</summary>
+
+you can only use our trainer or model
+
+- the only you need to input are `model`or`dataset`
 ```python
 import torch
 from torchsense.trainer import Trainer
 from torchsense.models.cnn4 import CNN4
 
 
 def train():
@@ -88,10 +104,12 @@
     )
 
     model = CNN4()
     trainer = Trainer(model, max_epochs=5)
     trainer.fit(train_loader, val_loader)
 ```
 
+</details>
+
 ## Thanks
 
 u-net parts reference [milesial](https://github.com/milesial/Pytorch-UNet/tree/master)
```

#### html2text {}

```diff
@@ -4,29 +4,31 @@
 It provides I/O, signal and data processing functions, datasets, model
 implementations and application components. ## Installation #### Pip ```bash #
 clone project git clone https://github.com/xibrer/torchsense.git # pip install
 pip install torchsense ``` ## Project Structure The directory structure of new
 project looks like this: ``` data/ âââ class_x â âââ xxx.ext â
 âââ xxy.ext â âââ ... â âââ xxz.ext âââ class_y
 âââ 123.ext âââ nsdf3.ext âââ ... âââ asd932_.ext ```
-## How to run torchsense provide two-way to run model ### Train model with
-default configuration ```python # ensure you already install torch and
-lightning from torchsense.datasets.folder import SensorFolder from
-torch.utils.data import DataLoader # you need to input list1 = [key1,key2,key3]
-# example ["acc", "mix_mic", "mic"] root_data = "data1" # data1 root path # as
-normal data = ImageFolder(root=root_data, params=list1) train_set, test_set =
-data.train_test_split(0.5) train_loader = DataLoader(train_set, batch_size=1,
-shuffle=True) test_loader = DataLoader(test_set, batch_size=1, shuffle=False)
-for i, batch in enumerate(train_loader): acc, mix, mic = batch[0] # ... train
-your self ``` now model only support .mat file ### Train model with custom
-configuration ```python import torch from torchsense.trainer import Trainer
-from torchsense.models.cnn4 import CNN4 def train(): from torchvision.datasets
-import MNIST from torchvision.transforms import ToTensor train_set = MNIST
-(root="./tmp/data1/MNIST", train=True, transform=ToTensor(), download=True)
-val_set = MNIST(root="./tmp/data1/MNIST", train=False, transform=ToTensor(),
-download=False) train_loader = torch.utils.data.DataLoader( train_set,
-batch_size=64, shuffle=True, pin_memory=torch.cuda.is_available(),
-num_workers=0 ) val_loader = torch.utils.data.DataLoader( val_set,
-batch_size=64, shuffle=False, pin_memory=torch.cuda.is_available(),
-num_workers=0 ) model = CNN4() trainer = Trainer(model, max_epochs=5)
-trainer.fit(train_loader, val_loader) ``` ## Thanks u-net parts reference
-[milesial](https://github.com/milesial/Pytorch-UNet/tree/master)
+### Train model with default configuration Show details you can only use our
+data loader - the only you need to input are `list1`and `data_path` ```python #
+ensure you already install torch and lightning from torchsense.datasets.folder
+import SensorFolder from torch.utils.data import DataLoader # you need to input
+list1 = [key1,key2,key3] # example ["acc", "mix_mic", "mic"] root_data =
+"data1" # data1 root path # as normal data = ImageFolder(root=root_data,
+params=list1) train_set, test_set = data.train_test_split(0.5) train_loader =
+DataLoader(train_set, batch_size=1, shuffle=True) test_loader = DataLoader
+(test_set, batch_size=1, shuffle=False) for i, batch in enumerate
+(train_loader): acc, mix, mic = batch[0] # ... train your self ``` ### Train
+model with custom configuration Show details you can only use our trainer or
+model - the only you need to input are `model`or`dataset` ```python import
+torch from torchsense.trainer import Trainer from torchsense.models.cnn4 import
+CNN4 def train(): from torchvision.datasets import MNIST from
+torchvision.transforms import ToTensor train_set = MNIST(root="./tmp/data1/
+MNIST", train=True, transform=ToTensor(), download=True) val_set = MNIST
+(root="./tmp/data1/MNIST", train=False, transform=ToTensor(), download=False)
+train_loader = torch.utils.data.DataLoader( train_set, batch_size=64,
+shuffle=True, pin_memory=torch.cuda.is_available(), num_workers=0 ) val_loader
+= torch.utils.data.DataLoader( val_set, batch_size=64, shuffle=False,
+pin_memory=torch.cuda.is_available(), num_workers=0 ) model = CNN4() trainer =
+Trainer(model, max_epochs=5) trainer.fit(train_loader, val_loader) ``` ##
+Thanks u-net parts reference [milesial](https://github.com/milesial/Pytorch-
+UNet/tree/master)
```

### Comparing `torchsense-0.0.4/pyproject.toml` & `torchsense-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "torchsense"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     {name = "Xingwei Wang", email = "wxwjkl123@gmail.com"},
 ]
 description = "Torchsense is a library for sensor data processing with PyTorch"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
 dependencies = [
```

### Comparing `torchsense-0.0.4/tests/test_model.py` & `torchsense-0.0.5/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/datasets/custom_folder.py` & `torchsense-0.0.5/torchsense/datasets/custom.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,18 +40,18 @@
         class_to_idx (dict): Dict with items (class_name, class_index).
         imgs (list): List of (image path, class_index) tuples
     """
 
     def __init__(
             self,
             root: str,
-            params: list = None,
-            transform: Optional[Callable] = None,
+            params: Tuple[List[str], Optional[List[str]]],
+            transform: Union[Optional[Callable], List[Callable]] = None,
             target_transform: Optional[Callable] = None,
-            loader: Callable[[str], Any] = default_loader,
+            loader: Callable[[str, Any], Any] = default_loader,
             is_valid_file: Optional[Callable[[str], bool]] = None,
             allow_empty: bool = False,
     ):
         super().__init__(
             root,
             params,
             loader,
@@ -95,18 +95,18 @@
         class_to_idx (dict): Dict with items (class_name, class_index).
         imgs (list): List of (image path, class_index) tuples
     """
 
     def __init__(
             self,
             root: str,
-            params: list = None,
+            params: Tuple[List[str], Optional[List[str]]] = None,
             transform: Optional[Callable] = None,
             target_transform: Optional[Callable] = None,
-            loader: Callable[[str], Any] = default_loader,
+            loader: Callable[[str, Any], Any] = default_loader,
             is_valid_file: Optional[Callable[[str], bool]] = None,
             allow_empty: bool = False,
     ):
         super().__init__(
             root,
             params,
             loader,
```

### Comparing `torchsense-0.0.4/torchsense/datasets/dataset2.py` & `torchsense-0.0.5/torchsense/datasets/dataset2.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/datasets/folder.py` & `torchsense-0.0.5/torchsense/datasets/folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import os
 import os.path
 from pathlib import Path
 from typing import Any, Callable, cast, Dict, List, Optional, Tuple, Union
 
-from PIL import Image
 from torch.utils.data import random_split
-
 from .vision import VisionDataset
-from .utils import load_file
 
 
 def has_file_allowed_extension(filename: str, extensions: Union[str, Tuple[str, ...]]) -> bool:
     """Checks if a file is an allowed extension.
 
     Args:
         filename (string): path to a file
@@ -135,18 +132,18 @@
         samples (list): List of (sample path, class_index) tuples
         targets (list): The class_index value for each image in the dataset
     """
 
     def __init__(
             self,
             root: Union[str, Path],
-            params: list,
-            loader: Callable[[str], Any],
+            params: Tuple[List[str], Optional[List[str]]],
+            loader: Callable[[str, Any], Any],
             extensions: Optional[Tuple[str, ...]] = None,
-            transform: Optional[Callable] = None,
+            transform: Union[Optional[Callable], List[Callable]] = None,
             target_transform: Optional[Callable] = None,
             is_valid_file: Optional[Callable[[str], bool]] = None,
             allow_empty: bool = False,
     ) -> None:
         super().__init__(root, transform=transform, target_transform=target_transform)
         classes, class_to_idx = self.find_classes(self.root)
         samples = self.make_dataset(
@@ -231,31 +228,35 @@
             FileNotFoundError: If ``dir`` has no class folders.
 
         Returns:
             (Tuple[List[str], Dict[str, int]]): List of all classes and dictionary mapping each class to an index.
         """
         return find_classes(directory)
 
-    def __getitem__(self, index: int) -> Tuple[Any, Any]:
+    def __getitem__(self, index: int) -> Tuple[Any, Any, Any]:
         """
         Args:
             index (int): Index
 
         Returns:
             tuple: (sample, target) where target is class_index of the target class.
         """
-        path, target = self.samples[index]
-        sample = self.loader(path, self.params)
+        path, labels = self.samples[index]
+        sample, target = self.loader(path, self.params)
+        if len(sample) == 1:
+            sample = sample[0]
+        if len(target) == 1:
+            target = target[0]
         if self.transform is not None:
-            sample = self.transform(sample)
+            for i in range(len(self.transform)):
+                sample[i] = self.transform[i](sample[i])
         if self.target_transform is not None:
             target = self.target_transform(target)
-        if len(sample) == 1:
-            sample = sample[0]
-        return sample, target
+
+        return sample, target, labels
 
     def __len__(self) -> int:
         return len(self.samples)
 
     def train_test_split(self, val_ratio):
         """
         划分训练集和验证集的函数，接收一个参数：`val_ratio`（验证集的比例）。
```

### Comparing `torchsense-0.0.4/torchsense/datasets/utils.py` & `torchsense-0.0.5/torchsense/datasets/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any, Callable, cast, Dict, List, Optional, Tuple, Union
 import numpy as np
+import torch
 from h5py import File
 
 
 def load_file(file_path, keys):
     file_extension = file_path.split('.')[-1].lower()
 
     if file_extension == '.txt':
@@ -48,36 +49,63 @@
         return get_meta_data(all_mat_data, list_j)
 
     except NotImplementedError:
         all_mat_data = File(path)
         return get_meta_data(all_mat_data, list_j)
 
 
-def get_meta_data(raw_data: Union[Dict[str, Any], File], keys: List[str] = None) -> Tuple:
+def get_meta_data(
+        raw_data: Union[Dict[str, Any], File],
+        keys: Tuple[List[str], Optional[List[str]]]
+) -> Tuple:
+    def parse_key(key: str) -> Tuple[str, Optional[int]]:
+        if '[' in key and ']' in key:
+            key_name = key[:key.index('[')]
+            row_str = key[key.index('[') + 1:key.index(']')]
+            if row_str.isdigit():
+                return key_name, int(row_str)
+        return key, None
+
     if keys is None:
-        # If list_j is empty, return all values in data1 as a tuple
+        # If keys is None, return all values in raw_data as a tuple
         # Remove meta info
         if '__header__' in raw_data:
             del raw_data['__header__']
         if '__version__' in raw_data:
             del raw_data['__version__']
         if '__globals__' in raw_data:
             del raw_data['__globals__']
         return tuple(raw_data.values())
     else:
-        # 初始化一个空列表
-        values = []
-        for key in keys:
-            # 检查当前的键是否在 raw_data 字典中
-            if key in raw_data:
-                value = raw_data[key]
-                values.append(value)
-        tuple_values = tuple(values)
+        inputs, targets = keys
+        input_values = []
+        target_values = []
+
+        # 提取inputs并处理特定行
+        for key in inputs:
+            key_name, row = parse_key(key)
+            if key_name in raw_data:
+                value = raw_data[key_name]
+                if row is not None and len(value) > row:
+                    input_values.append(value[row])
+                else:
+                    input_values.append(value)
+
+        # 提取targets
+        for key in targets:
+            key_name, row = parse_key(key)
+            if key_name in raw_data:
+                value = raw_data[key_name]
+                if row is not None and len(value) > row:
+                    target_values.append(value[row])
+                else:
+                    target_values.append(value)
+
         # 将列表转换为元组
-        return tuple_values
+        return input_values, target_values
 
 
 def load_npz_file(path, keys):
     npz_data = np.load(path)
     return tuple(npz_data[key] for key in keys if key in npz_data)
 
 # 使用示例
```

### Comparing `torchsense-0.0.4/torchsense/datasets/vision.py` & `torchsense-0.0.5/torchsense/datasets/vision.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 
         :attr:`transforms` and the combination of :attr:`transform` and :attr:`target_transform` are mutually exclusive.
     """
 
     _repr_indent = 4
 
     def __init__(
-        self,
-        root: Union[str, Path] = None,  # type: ignore[assignment]
-        transforms: Optional[Callable] = None,
-        transform: Optional[Callable] = None,
-        target_transform: Optional[Callable] = None,
+            self,
+            root: Union[str, Path] = None,  # type: ignore[assignment]
+            transforms: Optional[Callable] = None,
+            transform: Union[Optional[Callable], List[Callable]] = None,
+            target_transform: Optional[Callable] = None,
     ) -> None:
         if isinstance(root, str):
             root = os.path.expanduser(root)
         self.root = root
 
         has_transforms = transforms is not None
         has_separate_transform = transform is not None or target_transform is not None
@@ -79,15 +79,16 @@
         return [f"{head}{lines[0]}"] + ["{}{}".format(" " * len(head), line) for line in lines[1:]]
 
     def extra_repr(self) -> str:
         return ""
 
 
 class StandardTransform:
-    def __init__(self, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None) -> None:
+    def __init__(self, transform: Optional[Callable] = None,
+                 target_transform: Optional[Callable] = None) -> None:
         self.transform = transform
         self.target_transform = target_transform
 
     def __call__(self, input: Any, target: Any) -> Tuple[Any, Any]:
         if self.transform is not None:
             input = self.transform(input)
         if self.target_transform is not None:
@@ -101,8 +102,8 @@
     def __repr__(self) -> str:
         body = [self.__class__.__name__]
         if self.transform is not None:
             body += self._format_transform_repr(self.transform, "Transform: ")
         if self.target_transform is not None:
             body += self._format_transform_repr(self.target_transform, "Target transform: ")
 
-        return "\n".join(body)
+        return "\n".join(body)
```

### Comparing `torchsense-0.0.4/torchsense/models/Autoencode.py` & `torchsense-0.0.5/torchsense/models/Autoencode.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/Autoencoder.py` & `torchsense-0.0.5/torchsense/models/Autoencoder.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/LSTM.py` & `torchsense-0.0.5/torchsense/models/LSTM.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/alexnet.py` & `torchsense-0.0.5/torchsense/models/alexnet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/attention.py` & `torchsense-0.0.5/torchsense/models/attention.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/cct.py` & `torchsense-0.0.5/torchsense/models/cct.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/cnn4.py` & `torchsense-0.0.5/torchsense/models/cnn4.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/deeplab.py` & `torchsense-0.0.5/torchsense/models/deeplab.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/deeplabv3p.py` & `torchsense-0.0.5/torchsense/models/deeplabv3p.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/densenet.py` & `torchsense-0.0.5/torchsense/models/densenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/googlenet.py` & `torchsense-0.0.5/torchsense/models/googlenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/inceptionv3.py` & `torchsense-0.0.5/torchsense/models/inceptionv3.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/inceptionv4.py` & `torchsense-0.0.5/torchsense/models/inceptionv4.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/lit_model/litclassmodel.py` & `torchsense-0.0.5/torchsense/models/lit_model/lit_classify.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/lit_model/litregressmodel.py` & `torchsense-0.0.5/torchsense/models/lit_model/lit_regression.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,22 +14,22 @@
         self.model.apply(self.weights_init)
         self.loss_fn = torch.nn.MSELoss()
 
     def forward(self, x: torch.Tensor):
         return self.model(x)
 
     def _calculate_loss(self, batch, mode="train"):
-        x, y = batch
+        x = tuple(batch[0])
+        y = batch[1]
         preds = self.model(x)
-        # print(preds.max())
+
         loss = self.loss_fn(preds, y)
-        # acc = (preds.argmax(dim=-1) == y).float().mean()
 
         self.log("%s_loss" % mode, loss, prog_bar=True)
-        # self.log("%s_acc" % mode, acc, prog_bar=True)
+
         return loss
 
     def configure_optimizers(self):
         optimizer = optim.AdamW(self.parameters(), lr=self.hparams.lr)
         lr_scheduler = optim.lr_scheduler.MultiStepLR(optimizer, milestones=[100, 150], gamma=0.1)
         # optimizer = optim.Adadelta(self.parameters(), lr=self.hparams.lr)
         # lr_scheduler = optim.lr_scheduler.StepLR(optimizer, step_size=1, gamma=self.hparams.gamma)
```

### Comparing `torchsense-0.0.4/torchsense/models/mobilenet.py` & `torchsense-0.0.5/torchsense/models/mobilenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/mobilenetv1.py` & `torchsense-0.0.5/torchsense/models/mobilenetv1.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/mobilenetv2.py` & `torchsense-0.0.5/torchsense/models/mobilenetv2.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/mobilenetv3.py` & `torchsense-0.0.5/torchsense/models/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/nasnet.py` & `torchsense-0.0.5/torchsense/models/nasnet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/preactresnet.py` & `torchsense-0.0.5/torchsense/models/preactresnet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/resnet.py` & `torchsense-0.0.5/torchsense/models/resnet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/resnext.py` & `torchsense-0.0.5/torchsense/models/resnext.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/rir.py` & `torchsense-0.0.5/torchsense/models/rir.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/rnn.py` & `torchsense-0.0.5/torchsense/models/rnn.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/senet.py` & `torchsense-0.0.5/torchsense/models/senet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/shufflenet.py` & `torchsense-0.0.5/torchsense/models/shufflenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/shufflenetv2.py` & `torchsense-0.0.5/torchsense/models/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/simple_vit_1d.py` & `torchsense-0.0.5/torchsense/models/simple_vit_1d.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/squeezenet.py` & `torchsense-0.0.5/torchsense/models/squeezenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/stochasticdepth.py` & `torchsense-0.0.5/torchsense/models/stochasticdepth.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/unet.py` & `torchsense-0.0.5/torchsense/models/unet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/vgg.py` & `torchsense-0.0.5/torchsense/models/vgg.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/vit.py` & `torchsense-0.0.5/torchsense/models/vit.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/wideresidual.py` & `torchsense-0.0.5/torchsense/models/wideresidual.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/models/xception.py` & `torchsense-0.0.5/torchsense/models/xception.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.4/torchsense/trainer/trainer.py` & `torchsense-0.0.5/torchsense/trainer/trainer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-from torchsense.models.lit_model import LitRegressModel,LitClassModel
+from torchsense.models.lit_model import (LitRegressModel,
+                                         LitClassModel,
+                                         LitMultimodalModel)
 import lightning as L
 
 
 class Trainer:
     def __init__(self, model, task="r", max_epochs=5, accelerator="auto"):
         if task == "r":
             self.model = LitRegressModel(model)
         elif task == "c":
             self.model = LitClassModel(model)
+        elif task == "m":
+            self.model = LitMultimodalModel(model)
         else:
             raise ValueError("task must be either 'r' or 'c'")
         self.max_epochs = max_epochs
         self.accelerator = accelerator
 
     def fit(self, train_loader, val_loader):
         trainer = L.Trainer(
```

### Comparing `torchsense-0.0.4/torchsense.egg-info/PKG-INFO` & `torchsense-0.0.5/torchsense.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchsense
-Version: 0.0.4
+Version: 0.0.5
 Summary: Torchsense is a library for sensor data processing with PyTorch
 Author-email: Xingwei Wang <wxwjkl123@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Xingwei Wang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `torchsense-0.0.4/torchsense.egg-info/SOURCES.txt` & `torchsense-0.0.5/torchsense.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 torchsense/__init__.py
 torchsense.egg-info/PKG-INFO
 torchsense.egg-info/SOURCES.txt
 torchsense.egg-info/dependency_links.txt
 torchsense.egg-info/requires.txt
 torchsense.egg-info/top_level.txt
 torchsense/datasets/__init__.py
-torchsense/datasets/custom_folder.py
+torchsense/datasets/custom.py
 torchsense/datasets/dataset2.py
 torchsense/datasets/folder.py
 torchsense/datasets/utils.py
 torchsense/datasets/vision.py
 torchsense/models/Autoencode.py
 torchsense/models/Autoencoder.py
 torchsense/models/LSTM.py
@@ -21,14 +21,15 @@
 torchsense/models/alexnet.py
 torchsense/models/attention.py
 torchsense/models/cct.py
 torchsense/models/cnn4.py
 torchsense/models/deeplab.py
 torchsense/models/deeplabv3p.py
 torchsense/models/densenet.py
+torchsense/models/gan_g.py
 torchsense/models/googlenet.py
 torchsense/models/inceptionv3.py
 torchsense/models/inceptionv4.py
 torchsense/models/mobilenet.py
 torchsense/models/mobilenetv1.py
 torchsense/models/mobilenetv2.py
 torchsense/models/mobilenetv3.py
@@ -47,13 +48,20 @@
 torchsense/models/stochasticdepth.py
 torchsense/models/unet.py
 torchsense/models/vgg.py
 torchsense/models/vit.py
 torchsense/models/wideresidual.py
 torchsense/models/xception.py
 torchsense/models/lit_model/__init__.py
-torchsense/models/lit_model/litclassmodel.py
-torchsense/models/lit_model/litregressmodel.py
+torchsense/models/lit_model/lit_classify.py
+torchsense/models/lit_model/lit_multimodal.py
+torchsense/models/lit_model/lit_regression.py
 torchsense/trainer/__init__.py
 torchsense/trainer/trainer.py
 torchsense/transforms/__init__.py
+torchsense/transforms/compose.py
+torchsense/transforms/augmentations/__init__.py
+torchsense/transforms/augmentations/interpolate.py
+torchsense/transforms/augmentations/normalize.py
+torchsense/transforms/augmentations/to_tensor.py
+torchsense/transforms/augmentations/utils.py
 torchsense/utils/__init__.py
```

