# Comparing `tmp/torchsense-0.0.5.tar.gz` & `tmp/torchsense-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchsense-0.0.5.tar", last modified: Sat May 18 12:32:33 2024, max compression
+gzip compressed data, was "torchsense-0.0.6.tar", last modified: Sat May 18 12:56:49 2024, max compression
```

## Comparing `torchsense-0.0.5.tar` & `torchsense-0.0.6.tar`

### file list

```diff
@@ -1,80 +1,102 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 12:32:33.129955 torchsense-0.0.5/
--rw-rw-rw-   0        0        0     1090 2024-05-05 06:37:08.000000 torchsense-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1665 2024-05-18 12:32:33.128078 torchsense-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3065 2024-05-16 08:38:02.000000 torchsense-0.0.5/README.md
--rw-rw-rw-   0        0        0      573 2024-05-18 12:32:20.000000 torchsense-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-18 12:32:33.129955 torchsense-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-18 12:32:32.975534 torchsense-0.0.5/tests/
--rw-rw-rw-   0        0        0     1445 2024-05-15 16:08:03.000000 torchsense-0.0.5/tests/test_model.py
-drwxrwxrwx   0        0        0        0 2024-05-18 12:32:32.977753 torchsense-0.0.5/torchsense/
--rw-rw-rw-   0        0        0        2 2024-05-16 08:20:27.000000 torchsense-0.0.5/torchsense/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 12:32:33.001491 torchsense-0.0.5/torchsense/datasets/
--rw-rw-rw-   0        0        0        0 2024-05-05 06:50:01.000000 torchsense-0.0.5/torchsense/datasets/__init__.py
--rw-rw-rw-   0        0        0     4811 2024-05-18 11:16:08.000000 torchsense-0.0.5/torchsense/datasets/custom.py
--rw-rw-rw-   0        0        0     5076 2024-05-13 11:17:11.000000 torchsense-0.0.5/torchsense/datasets/dataset2.py
--rw-rw-rw-   0        0        0    11200 2024-05-18 11:24:48.000000 torchsense-0.0.5/torchsense/datasets/folder.py
--rw-rw-rw-   0        0        0     3433 2024-05-18 11:28:37.000000 torchsense-0.0.5/torchsense/datasets/utils.py
--rw-rw-rw-   0        0        0     4344 2024-05-18 09:04:23.000000 torchsense-0.0.5/torchsense/datasets/vision.py
-drwxrwxrwx   0        0        0        0 2024-05-18 12:32:33.097710 torchsense-0.0.5/torchsense/models/
--rw-rw-rw-   0        0        0     4213 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/Autoencode.py
--rw-rw-rw-   0        0        0     4213 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/Autoencoder.py
--rw-rw-rw-   0        0        0     6353 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/LSTM.py
--rw-rw-rw-   0        0        0      130 2024-05-15 15:59:59.000000 torchsense-0.0.5/torchsense/models/__init__.py
--rw-rw-rw-   0        0        0     3531 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/alexnet.py
--rw-rw-rw-   0        0        0    12106 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/attention.py
--rw-rw-rw-   0        0        0    12316 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/cct.py
--rw-rw-rw-   0        0        0      780 2024-05-15 11:05:37.000000 torchsense-0.0.5/torchsense/models/cnn4.py
--rw-rw-rw-   0        0        0     5012 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/deeplab.py
--rw-rw-rw-   0        0        0     5672 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/deeplabv3p.py
--rw-rw-rw-   0        0        0     5216 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/densenet.py
--rw-rw-rw-   0        0        0    11223 2024-05-17 10:48:08.000000 torchsense-0.0.5/torchsense/models/gan_g.py
--rw-rw-rw-   0        0        0     4632 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/googlenet.py
--rw-rw-rw-   0        0        0    11215 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/inceptionv3.py
--rw-rw-rw-   0        0        0    18657 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/inceptionv4.py
-drwxrwxrwx   0        0        0        0 2024-05-18 12:32:33.105927 torchsense-0.0.5/torchsense/models/lit_model/
--rw-rw-rw-   0        0        0      215 2024-05-17 13:37:52.000000 torchsense-0.0.5/torchsense/models/lit_model/__init__.py
--rw-rw-rw-   0        0        0     2345 2024-05-15 11:39:31.000000 torchsense-0.0.5/torchsense/models/lit_model/lit_classify.py
--rw-rw-rw-   0        0        0     2231 2024-05-17 13:37:52.000000 torchsense-0.0.5/torchsense/models/lit_model/lit_multimodal.py
--rw-rw-rw-   0        0        0     2228 2024-05-17 08:53:55.000000 torchsense-0.0.5/torchsense/models/lit_model/lit_regression.py
--rw-rw-rw-   0        0        0     5629 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/mobilenet.py
--rw-rw-rw-   0        0        0     7696 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/mobilenetv1.py
--rw-rw-rw-   0        0        0     7973 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/mobilenetv2.py
--rw-rw-rw-   0        0        0     9749 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/mobilenetv3.py
--rw-rw-rw-   0        0        0     9920 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/nasnet.py
--rw-rw-rw-   0        0        0     4028 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/preactresnet.py
--rw-rw-rw-   0        0        0     6796 2024-05-15 16:06:20.000000 torchsense-0.0.5/torchsense/models/resnet.py
--rw-rw-rw-   0        0        0     4440 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/resnext.py
--rw-rw-rw-   0        0        0     7217 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/rir.py
--rw-rw-rw-   0        0        0     5759 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/sealex.py
--rw-rw-rw-   0        0        0     5458 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/senet.py
--rw-rw-rw-   0        0        0     7695 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/shufflenet.py
--rw-rw-rw-   0        0        0     4953 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/shufflenetv2.py
--rw-rw-rw-   0        0        0     3840 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/simple_vit_1d.py
--rw-rw-rw-   0        0        0     2540 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/squeezenet.py
--rw-rw-rw-   0        0        0     7722 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/stochasticdepth.py
--rw-rw-rw-   0        0        0     4170 2024-05-14 01:33:19.000000 torchsense-0.0.5/torchsense/models/unet.py
--rw-rw-rw-   0        0        0     2114 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/vgg.py
--rw-rw-rw-   0        0        0     6935 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/vit.py
--rw-rw-rw-   0        0        0     3358 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/wideresidual.py
--rw-rw-rw-   0        0        0     6339 2024-05-05 06:37:08.000000 torchsense-0.0.5/torchsense/models/xception.py
-drwxrwxrwx   0        0        0        0 2024-05-18 12:32:33.110021 torchsense-0.0.5/torchsense/trainer/
--rw-rw-rw-   0        0        0       48 2024-05-13 12:49:15.000000 torchsense-0.0.5/torchsense/trainer/__init__.py
--rw-rw-rw-   0        0        0      913 2024-05-17 13:37:52.000000 torchsense-0.0.5/torchsense/trainer/trainer.py
-drwxrwxrwx   0        0        0        0 2024-05-18 12:32:33.115322 torchsense-0.0.5/torchsense/transforms/
--rw-rw-rw-   0        0        0      261 2024-05-18 12:25:32.000000 torchsense-0.0.5/torchsense/transforms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 12:32:33.122915 torchsense-0.0.5/torchsense/transforms/augmentations/
--rw-rw-rw-   0        0        0        0 2024-05-05 06:49:52.000000 torchsense-0.0.5/torchsense/transforms/augmentations/__init__.py
--rw-rw-rw-   0        0        0      713 2024-05-18 12:32:20.000000 torchsense-0.0.5/torchsense/transforms/augmentations/interpolate.py
--rw-rw-rw-   0        0        0      612 2024-05-18 11:19:22.000000 torchsense-0.0.5/torchsense/transforms/augmentations/normalize.py
--rw-rw-rw-   0        0        0      800 2024-05-18 11:31:59.000000 torchsense-0.0.5/torchsense/transforms/augmentations/to_tensor.py
--rw-rw-rw-   0        0        0      379 2024-05-18 12:29:31.000000 torchsense-0.0.5/torchsense/transforms/augmentations/utils.py
--rw-rw-rw-   0        0        0     6047 2024-05-18 07:44:50.000000 torchsense-0.0.5/torchsense/transforms/compose.py
-drwxrwxrwx   0        0        0        0 2024-05-18 12:32:33.124150 torchsense-0.0.5/torchsense/utils/
--rw-rw-rw-   0        0        0        0 2024-05-13 11:12:46.000000 torchsense-0.0.5/torchsense/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 12:32:33.126668 torchsense-0.0.5/torchsense.egg-info/
--rw-rw-rw-   0        0        0     1665 2024-05-18 12:32:32.000000 torchsense-0.0.5/torchsense.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2113 2024-05-18 12:32:32.000000 torchsense-0.0.5/torchsense.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 12:32:32.000000 torchsense-0.0.5/torchsense.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 12:32:32.000000 torchsense-0.0.5/torchsense.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-18 12:32:32.000000 torchsense-0.0.5/torchsense.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 12:56:49.212965 torchsense-0.0.6/
+-rw-rw-rw-   0        0        0     3568 2024-05-13 12:22:11.000000 torchsense-0.0.6/.gitignore
+-rw-rw-rw-   0        0        0     1090 2024-05-05 06:37:08.000000 torchsense-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1665 2024-05-18 12:56:49.212965 torchsense-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3065 2024-05-16 08:38:02.000000 torchsense-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 12:56:49.071973 torchsense-0.0.6/examples/
+drwxrwxrwx   0        0        0        0 2024-05-18 12:56:49.043131 torchsense-0.0.6/examples/data1/
+drwxrwxrwx   0        0        0        0 2024-05-18 12:56:49.047472 torchsense-0.0.6/examples/data1/hsm/
+drwxrwxrwx   0        0        0        0 2024-05-18 12:56:49.097654 torchsense-0.0.6/examples/data1/hsm/1/
+-rw-rw-rw-   0        0        0   696720 2024-04-30 08:25:03.000000 torchsense-0.0.6/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-1.mat
+-rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:32.000000 torchsense-0.0.6/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-10.mat
+-rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:32.000000 torchsense-0.0.6/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-2.mat
+-rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:33.000000 torchsense-0.0.6/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-3.mat
+-rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:33.000000 torchsense-0.0.6/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-4.mat
+-rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:34.000000 torchsense-0.0.6/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-5.mat
+-rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:34.000000 torchsense-0.0.6/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-6.mat
+-rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:35.000000 torchsense-0.0.6/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-7.mat
+-rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:35.000000 torchsense-0.0.6/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-8.mat
+-rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:36.000000 torchsense-0.0.6/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-9.mat
+drwxrwxrwx   0        0        0        0 2024-05-18 12:56:49.047472 torchsense-0.0.6/examples/data2/
+drwxrwxrwx   0        0        0        0 2024-05-18 12:56:49.102158 torchsense-0.0.6/examples/data2/1/
+-rw-rw-rw-   0        0        0   361310 2024-05-12 13:57:33.000000 torchsense-0.0.6/examples/data2/1/test.mat
+-rw-rw-rw-   0        0        0   361310 2024-05-12 13:57:33.000000 torchsense-0.0.6/examples/data2/1/test2.mat
+-rw-rw-rw-   0        0        0      624 2024-05-18 11:17:29.000000 torchsense-0.0.6/examples/data_module4.py
+-rw-rw-rw-   0        0        0     1486 2024-05-18 12:45:06.000000 torchsense-0.0.6/examples/run.py
+-rw-rw-rw-   0        0        0     7646 2024-05-15 11:15:43.000000 torchsense-0.0.6/examples/train_fabric.py
+-rw-rw-rw-   0        0        0      573 2024-05-18 12:56:43.000000 torchsense-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-18 12:56:49.212965 torchsense-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-18 12:56:49.103821 torchsense-0.0.6/tests/
+-rw-rw-rw-   0        0        0     1445 2024-05-15 16:08:03.000000 torchsense-0.0.6/tests/test_model.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:56:49.103821 torchsense-0.0.6/torchsense/
+-rw-rw-rw-   0        0        0        2 2024-05-16 08:20:27.000000 torchsense-0.0.6/torchsense/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:56:49.123476 torchsense-0.0.6/torchsense/datasets/
+-rw-rw-rw-   0        0        0        0 2024-05-05 06:50:01.000000 torchsense-0.0.6/torchsense/datasets/__init__.py
+-rw-rw-rw-   0        0        0     4811 2024-05-18 11:16:08.000000 torchsense-0.0.6/torchsense/datasets/custom.py
+-rw-rw-rw-   0        0        0     5076 2024-05-13 11:17:11.000000 torchsense-0.0.6/torchsense/datasets/dataset2.py
+-rw-rw-rw-   0        0        0    11200 2024-05-18 11:24:48.000000 torchsense-0.0.6/torchsense/datasets/folder.py
+-rw-rw-rw-   0        0        0     3433 2024-05-18 11:28:37.000000 torchsense-0.0.6/torchsense/datasets/utils.py
+-rw-rw-rw-   0        0        0     4344 2024-05-18 09:04:23.000000 torchsense-0.0.6/torchsense/datasets/vision.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:56:49.185418 torchsense-0.0.6/torchsense/models/
+-rw-rw-rw-   0        0        0     4213 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/Autoencode.py
+-rw-rw-rw-   0        0        0     4213 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/Autoencoder.py
+-rw-rw-rw-   0        0        0     6353 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/LSTM.py
+-rw-rw-rw-   0        0        0      130 2024-05-15 15:59:59.000000 torchsense-0.0.6/torchsense/models/__init__.py
+-rw-rw-rw-   0        0        0     3531 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/alexnet.py
+-rw-rw-rw-   0        0        0    12106 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/attention.py
+-rw-rw-rw-   0        0        0    12316 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/cct.py
+-rw-rw-rw-   0        0        0      780 2024-05-15 11:05:37.000000 torchsense-0.0.6/torchsense/models/cnn4.py
+-rw-rw-rw-   0        0        0     5012 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/deeplab.py
+-rw-rw-rw-   0        0        0     5672 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/deeplabv3p.py
+-rw-rw-rw-   0        0        0     5216 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/densenet.py
+-rw-rw-rw-   0        0        0    11223 2024-05-17 10:48:08.000000 torchsense-0.0.6/torchsense/models/gan_g.py
+-rw-rw-rw-   0        0        0     4632 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/googlenet.py
+-rw-rw-rw-   0        0        0    11215 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/inceptionv3.py
+-rw-rw-rw-   0        0        0    18657 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/inceptionv4.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:56:49.192871 torchsense-0.0.6/torchsense/models/lit_model/
+-rw-rw-rw-   0        0        0      215 2024-05-17 13:37:52.000000 torchsense-0.0.6/torchsense/models/lit_model/__init__.py
+-rw-rw-rw-   0        0        0     2345 2024-05-15 11:39:31.000000 torchsense-0.0.6/torchsense/models/lit_model/lit_classify.py
+-rw-rw-rw-   0        0        0     2231 2024-05-17 13:37:52.000000 torchsense-0.0.6/torchsense/models/lit_model/lit_multimodal.py
+-rw-rw-rw-   0        0        0     2228 2024-05-17 08:53:55.000000 torchsense-0.0.6/torchsense/models/lit_model/lit_regression.py
+-rw-rw-rw-   0        0        0     5629 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/mobilenet.py
+-rw-rw-rw-   0        0        0     7696 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/mobilenetv1.py
+-rw-rw-rw-   0        0        0     7973 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/mobilenetv2.py
+-rw-rw-rw-   0        0        0     9749 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/mobilenetv3.py
+-rw-rw-rw-   0        0        0     9920 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/nasnet.py
+-rw-rw-rw-   0        0        0     4028 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/preactresnet.py
+-rw-rw-rw-   0        0        0     6796 2024-05-15 16:06:20.000000 torchsense-0.0.6/torchsense/models/resnet.py
+-rw-rw-rw-   0        0        0     4440 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/resnext.py
+-rw-rw-rw-   0        0        0     7217 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/rir.py
+-rw-rw-rw-   0        0        0     5759 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/sealex.py
+-rw-rw-rw-   0        0        0     5458 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/senet.py
+-rw-rw-rw-   0        0        0     7695 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/shufflenet.py
+-rw-rw-rw-   0        0        0     4953 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/shufflenetv2.py
+-rw-rw-rw-   0        0        0     3840 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/simple_vit_1d.py
+-rw-rw-rw-   0        0        0     2540 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/squeezenet.py
+-rw-rw-rw-   0        0        0     7722 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/stochasticdepth.py
+-rw-rw-rw-   0        0        0     4170 2024-05-14 01:33:19.000000 torchsense-0.0.6/torchsense/models/unet.py
+-rw-rw-rw-   0        0        0     2114 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/vgg.py
+-rw-rw-rw-   0        0        0     6935 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/vit.py
+-rw-rw-rw-   0        0        0     3358 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/wideresidual.py
+-rw-rw-rw-   0        0        0     6339 2024-05-05 06:37:08.000000 torchsense-0.0.6/torchsense/models/xception.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:56:49.196493 torchsense-0.0.6/torchsense/trainer/
+-rw-rw-rw-   0        0        0       48 2024-05-13 12:49:15.000000 torchsense-0.0.6/torchsense/trainer/__init__.py
+-rw-rw-rw-   0        0        0     1567 2024-05-18 12:54:58.000000 torchsense-0.0.6/torchsense/trainer/trainer.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:56:49.202041 torchsense-0.0.6/torchsense/transforms/
+-rw-rw-rw-   0        0        0      261 2024-05-18 12:25:32.000000 torchsense-0.0.6/torchsense/transforms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:56:49.209685 torchsense-0.0.6/torchsense/transforms/augmentations/
+-rw-rw-rw-   0        0        0        0 2024-05-05 06:49:52.000000 torchsense-0.0.6/torchsense/transforms/augmentations/__init__.py
+-rw-rw-rw-   0        0        0      713 2024-05-18 12:32:20.000000 torchsense-0.0.6/torchsense/transforms/augmentations/interpolate.py
+-rw-rw-rw-   0        0        0      612 2024-05-18 11:19:22.000000 torchsense-0.0.6/torchsense/transforms/augmentations/normalize.py
+-rw-rw-rw-   0        0        0      800 2024-05-18 11:31:59.000000 torchsense-0.0.6/torchsense/transforms/augmentations/to_tensor.py
+-rw-rw-rw-   0        0        0      379 2024-05-18 12:29:31.000000 torchsense-0.0.6/torchsense/transforms/augmentations/utils.py
+-rw-rw-rw-   0        0        0     6047 2024-05-18 07:44:50.000000 torchsense-0.0.6/torchsense/transforms/compose.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:56:49.211955 torchsense-0.0.6/torchsense/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-13 11:12:46.000000 torchsense-0.0.6/torchsense/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:56:49.212965 torchsense-0.0.6/torchsense.egg-info/
+-rw-rw-rw-   0        0        0     1665 2024-05-18 12:56:48.000000 torchsense-0.0.6/torchsense.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3254 2024-05-18 12:56:49.000000 torchsense-0.0.6/torchsense.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 12:56:48.000000 torchsense-0.0.6/torchsense.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 12:56:48.000000 torchsense-0.0.6/torchsense.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-18 12:56:48.000000 torchsense-0.0.6/torchsense.egg-info/top_level.txt
```

### Comparing `torchsense-0.0.5/LICENSE` & `torchsense-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/PKG-INFO` & `torchsense-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchsense
-Version: 0.0.5
+Version: 0.0.6
 Summary: Torchsense is a library for sensor data processing with PyTorch
 Author-email: Xingwei Wang <wxwjkl123@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Xingwei Wang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `torchsense-0.0.5/README.md` & `torchsense-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/pyproject.toml` & `torchsense-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "torchsense"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     {name = "Xingwei Wang", email = "wxwjkl123@gmail.com"},
 ]
 description = "Torchsense is a library for sensor data processing with PyTorch"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
 dependencies = [
```

### Comparing `torchsense-0.0.5/tests/test_model.py` & `torchsense-0.0.6/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/datasets/custom.py` & `torchsense-0.0.6/torchsense/datasets/custom.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/datasets/dataset2.py` & `torchsense-0.0.6/torchsense/datasets/dataset2.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/datasets/folder.py` & `torchsense-0.0.6/torchsense/datasets/folder.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/datasets/utils.py` & `torchsense-0.0.6/torchsense/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/datasets/vision.py` & `torchsense-0.0.6/torchsense/datasets/vision.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/Autoencode.py` & `torchsense-0.0.6/torchsense/models/Autoencode.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/Autoencoder.py` & `torchsense-0.0.6/torchsense/models/Autoencoder.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/LSTM.py` & `torchsense-0.0.6/torchsense/models/LSTM.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/alexnet.py` & `torchsense-0.0.6/torchsense/models/alexnet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/attention.py` & `torchsense-0.0.6/torchsense/models/attention.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/cct.py` & `torchsense-0.0.6/torchsense/models/cct.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/cnn4.py` & `torchsense-0.0.6/torchsense/models/cnn4.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/deeplab.py` & `torchsense-0.0.6/torchsense/models/deeplab.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/deeplabv3p.py` & `torchsense-0.0.6/torchsense/models/deeplabv3p.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/densenet.py` & `torchsense-0.0.6/torchsense/models/densenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/gan_g.py` & `torchsense-0.0.6/torchsense/models/gan_g.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/googlenet.py` & `torchsense-0.0.6/torchsense/models/googlenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/inceptionv3.py` & `torchsense-0.0.6/torchsense/models/inceptionv3.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/inceptionv4.py` & `torchsense-0.0.6/torchsense/models/inceptionv4.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/lit_model/lit_classify.py` & `torchsense-0.0.6/torchsense/models/lit_model/lit_classify.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/lit_model/lit_multimodal.py` & `torchsense-0.0.6/torchsense/models/lit_model/lit_multimodal.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/lit_model/lit_regression.py` & `torchsense-0.0.6/torchsense/models/lit_model/lit_regression.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/mobilenet.py` & `torchsense-0.0.6/torchsense/models/mobilenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/mobilenetv1.py` & `torchsense-0.0.6/torchsense/models/mobilenetv1.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/mobilenetv2.py` & `torchsense-0.0.6/torchsense/models/mobilenetv2.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/mobilenetv3.py` & `torchsense-0.0.6/torchsense/models/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/nasnet.py` & `torchsense-0.0.6/torchsense/models/nasnet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/preactresnet.py` & `torchsense-0.0.6/torchsense/models/preactresnet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/resnet.py` & `torchsense-0.0.6/torchsense/models/resnet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/resnext.py` & `torchsense-0.0.6/torchsense/models/resnext.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/rir.py` & `torchsense-0.0.6/torchsense/models/rir.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/rnn.py` & `torchsense-0.0.6/torchsense/models/rnn.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/senet.py` & `torchsense-0.0.6/torchsense/models/senet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/shufflenet.py` & `torchsense-0.0.6/torchsense/models/shufflenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/shufflenetv2.py` & `torchsense-0.0.6/torchsense/models/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/simple_vit_1d.py` & `torchsense-0.0.6/torchsense/models/simple_vit_1d.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/squeezenet.py` & `torchsense-0.0.6/torchsense/models/squeezenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/stochasticdepth.py` & `torchsense-0.0.6/torchsense/models/stochasticdepth.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/unet.py` & `torchsense-0.0.6/torchsense/models/unet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/vgg.py` & `torchsense-0.0.6/torchsense/models/vgg.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/vit.py` & `torchsense-0.0.6/torchsense/models/vit.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/wideresidual.py` & `torchsense-0.0.6/torchsense/models/wideresidual.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/models/xception.py` & `torchsense-0.0.6/torchsense/models/xception.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/transforms/augmentations/interpolate.py` & `torchsense-0.0.6/torchsense/transforms/augmentations/interpolate.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/transforms/augmentations/normalize.py` & `torchsense-0.0.6/torchsense/transforms/augmentations/normalize.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/transforms/augmentations/to_tensor.py` & `torchsense-0.0.6/torchsense/transforms/augmentations/to_tensor.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense/transforms/compose.py` & `torchsense-0.0.6/torchsense/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.5/torchsense.egg-info/PKG-INFO` & `torchsense-0.0.6/torchsense.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchsense
-Version: 0.0.5
+Version: 0.0.6
 Summary: Torchsense is a library for sensor data processing with PyTorch
 Author-email: Xingwei Wang <wxwjkl123@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Xingwei Wang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `torchsense-0.0.5/torchsense.egg-info/SOURCES.txt` & `torchsense-0.0.6/torchsense.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,26 @@
+.gitignore
 LICENSE
 README.md
 pyproject.toml
+examples/data_module4.py
+examples/run.py
+examples/train_fabric.py
+examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-1.mat
+examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-10.mat
+examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-2.mat
+examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-3.mat
+examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-4.mat
+examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-5.mat
+examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-6.mat
+examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-7.mat
+examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-8.mat
+examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-9.mat
+examples/data2/1/test.mat
+examples/data2/1/test2.mat
 tests/test_model.py
 torchsense/__init__.py
 torchsense.egg-info/PKG-INFO
 torchsense.egg-info/SOURCES.txt
 torchsense.egg-info/dependency_links.txt
 torchsense.egg-info/requires.txt
 torchsense.egg-info/top_level.txt
```

