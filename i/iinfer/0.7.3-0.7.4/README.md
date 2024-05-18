# Comparing `tmp/iinfer-0.7.3.tar.gz` & `tmp/iinfer-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iinfer-0.7.3.tar", last modified: Mon May  6 13:44:21 2024, max compression
+gzip compressed data, was "iinfer-0.7.4.tar", last modified: Sat May 18 12:21:49 2024, max compression
```

## Comparing `iinfer-0.7.3.tar` & `iinfer-0.7.4.tar`

### file list

```diff
@@ -1,217 +1,217 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.230419 iinfer-0.7.3/
--rw-rw-rw-   0        0        0     1117 2024-02-15 15:34:04.000000 iinfer-0.7.3/LICENSE
--rw-rw-rw-   0        0        0     5553 2024-05-06 13:44:21.229422 iinfer-0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     4619 2024-03-11 12:57:36.000000 iinfer-0.7.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.191863 iinfer-0.7.3/iinfer/
--rw-rw-rw-   0        0        0       69 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/__init__.py
--rw-rw-rw-   0        0        0      109 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.329862 iinfer-0.7.3/iinfer/app/
--rw-rw-rw-   0        0        0       73 2024-03-10 12:26:23.000000 iinfer-0.7.3/iinfer/app/__init__.py
--rw-rw-rw-   0        0        0    51232 2024-05-04 02:38:57.000000 iinfer-0.7.3/iinfer/app/app.py
--rw-rw-rw-   0        0        0    34708 2024-05-06 10:14:38.000000 iinfer-0.7.3/iinfer/app/client.py
--rw-rw-rw-   0        0        0    14034 2024-05-03 09:11:44.000000 iinfer-0.7.3/iinfer/app/common.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.336860 iinfer-0.7.3/iinfer/app/commons/
--rw-rw-rw-   0        0        0     5433 2024-02-26 12:32:33.000000 iinfer-0.7.3/iinfer/app/commons/convert.py
--rw-rw-rw-   0        0        0     7868 2024-05-04 02:31:10.000000 iinfer-0.7.3/iinfer/app/commons/module.py
--rw-rw-rw-   0        0        0     3613 2024-05-06 11:42:49.000000 iinfer-0.7.3/iinfer/app/gui.py
--rw-rw-rw-   0        0        0     5247 2024-04-11 12:30:41.000000 iinfer-0.7.3/iinfer/app/injection.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.379865 iinfer-0.7.3/iinfer/app/injections/
--rw-rw-rw-   0        0        0     2023 2024-04-11 11:13:52.000000 iinfer-0.7.3/iinfer/app/injections/after_cls_jadge_injection.py
--rw-rw-rw-   0        0        0     4500 2024-04-06 14:50:20.000000 iinfer-0.7.3/iinfer/app/injections/after_csv_injection.py
--rw-rw-rw-   0        0        0     6735 2024-05-02 03:57:31.000000 iinfer-0.7.3/iinfer/app/injections/after_det_filter_injection.py
--rw-rw-rw-   0        0        0     8540 2024-04-07 07:16:07.000000 iinfer-0.7.3/iinfer/app/injections/after_det_jadge_injection.py
--rw-rw-rw-   0        0        0     4790 2024-04-07 00:11:59.000000 iinfer-0.7.3/iinfer/app/injections/after_http_injection.py
--rw-rw-rw-   0        0        0     9077 2024-04-11 13:28:27.000000 iinfer-0.7.3/iinfer/app/injections/after_seg_bbox_injection.py
--rw-rw-rw-   0        0        0     8688 2024-04-11 13:41:09.000000 iinfer-0.7.3/iinfer/app/injections/after_seg_filter_injection.py
--rw-rw-rw-   0        0        0     1810 2024-02-25 07:58:13.000000 iinfer-0.7.3/iinfer/app/injections/before_grayimg_injection.py
--rw-rw-rw-   0        0        0    15606 2024-05-06 13:43:20.000000 iinfer-0.7.3/iinfer/app/install.py
--rw-rw-rw-   0        0        0   157617 2024-05-06 06:48:17.000000 iinfer-0.7.3/iinfer/app/options.py
--rw-rw-rw-   0        0        0     5309 2024-05-02 02:25:26.000000 iinfer-0.7.3/iinfer/app/postprocess.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.426863 iinfer-0.7.3/iinfer/app/postprocesses/
--rw-rw-rw-   0        0        0     1935 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/app/postprocesses/cls_jadge.py
--rw-rw-rw-   0        0        0     2393 2024-04-06 14:52:31.000000 iinfer-0.7.3/iinfer/app/postprocesses/csv.py
--rw-rw-rw-   0        0        0     4197 2024-03-10 09:01:15.000000 iinfer-0.7.3/iinfer/app/postprocesses/det_clip.py
--rw-rw-rw-   0        0        0     5063 2024-03-17 02:51:08.000000 iinfer-0.7.3/iinfer/app/postprocesses/det_face_store.py
--rw-rw-rw-   0        0        0     4444 2024-04-11 13:48:21.000000 iinfer-0.7.3/iinfer/app/postprocesses/det_filter.py
--rw-rw-rw-   0        0        0     5201 2024-04-07 07:20:08.000000 iinfer-0.7.3/iinfer/app/postprocesses/det_jadge.py
--rw-rw-rw-   0        0        0     3813 2024-04-07 00:25:09.000000 iinfer-0.7.3/iinfer/app/postprocesses/httpreq.py
--rw-rw-rw-   0        0        0     4369 2024-04-11 13:06:06.000000 iinfer-0.7.3/iinfer/app/postprocesses/seg_bbox.py
--rw-rw-rw-   0        0        0     4252 2024-04-11 12:27:14.000000 iinfer-0.7.3/iinfer/app/postprocesses/seg_filter.py
--rw-rw-rw-   0        0        0     6082 2024-05-03 06:19:11.000000 iinfer-0.7.3/iinfer/app/predict.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.503862 iinfer-0.7.3/iinfer/app/predicts/
--rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/app/predicts/__init__.py
--rw-rw-rw-   0        0        0     3511 2024-05-04 02:00:36.000000 iinfer-0.7.3/iinfer/app/predicts/diffusers_stablediffusion_txt2img.py
--rw-rw-rw-   0        0        0     7618 2024-05-04 02:00:29.000000 iinfer-0.7.3/iinfer/app/predicts/insightface_det.py
--rw-rw-rw-   0        0        0     4134 2024-05-04 02:00:22.000000 iinfer-0.7.3/iinfer/app/predicts/mmdet_det_YoloX.py
--rw-rw-rw-   0        0        0      384 2024-05-04 02:00:25.000000 iinfer-0.7.3/iinfer/app/predicts/mmdet_det_YoloX_Lite.py
--rw-rw-rw-   0        0        0     4712 2024-05-04 02:00:14.000000 iinfer-0.7.3/iinfer/app/predicts/mmpretrain_cls_swin.py
--rw-rw-rw-   0        0        0      418 2024-05-04 02:00:18.000000 iinfer-0.7.3/iinfer/app/predicts/mmpretrain_cls_swin_Lite.py
--rw-rw-rw-   0        0        0    10366 2024-05-04 02:00:10.000000 iinfer-0.7.3/iinfer/app/predicts/mmrotate_det_ReDet.py
--rw-rw-rw-   0        0        0     5712 2024-05-04 02:00:06.000000 iinfer-0.7.3/iinfer/app/predicts/mmseg_seg_PSPNet.py
--rw-rw-rw-   0        0        0      377 2024-05-02 14:44:28.000000 iinfer-0.7.3/iinfer/app/predicts/mmseg_seg_San.py
--rw-rw-rw-   0        0        0      386 2024-03-30 02:49:57.000000 iinfer-0.7.3/iinfer/app/predicts/mmseg_seg_SwinUpernet.py
--rw-rw-rw-   0        0        0     4647 2024-03-30 02:50:02.000000 iinfer-0.7.3/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py
--rw-rw-rw-   0        0        0     5301 2024-03-30 02:50:07.000000 iinfer-0.7.3/iinfer/app/predicts/onnx_det_TinyYoloV3.py
--rw-rw-rw-   0        0        0     5509 2024-03-30 02:50:11.000000 iinfer-0.7.3/iinfer/app/predicts/onnx_det_YoloV3.py
--rw-rw-rw-   0        0        0     9843 2024-03-30 02:50:23.000000 iinfer-0.7.3/iinfer/app/predicts/onnx_det_YoloX.py
--rw-rw-rw-   0        0        0     2887 2024-03-30 02:50:17.000000 iinfer-0.7.3/iinfer/app/predicts/onnx_det_YoloX_Lite.py
--rw-rw-rw-   0        0        0     2706 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/app/redis.py
--rw-rw-rw-   0        0        0    52240 2024-05-06 13:43:15.000000 iinfer-0.7.3/iinfer/app/server.py
--rw-rw-rw-   0        0        0    26325 2024-05-06 11:47:13.000000 iinfer-0.7.3/iinfer/app/web.py
--rw-rw-rw-   0        0        0       54 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/config.yml
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.530866 iinfer-0.7.3/iinfer/docker/
--rw-rw-rw-   0        0        0      835 2024-05-03 11:17:19.000000 iinfer-0.7.3/iinfer/docker/Dockerfile
--rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/docker/__init__.py
--rw-rw-rw-   0        0        0      131 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/docker/build.sh
--rw-rw-rw-   0        0        0      319 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/docker/docker-compose.yml
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.535862 iinfer-0.7.3/iinfer/extensions/
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.032858 iinfer-0.7.3/iinfer/extensions/configs/
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.550863 iinfer-0.7.3/iinfer/extensions/configs/mmdet/
--rw-rw-rw-   0        0        0      273 2024-05-03 08:33:49.000000 iinfer-0.7.3/iinfer/extensions/configs/mmdet/yolox_l_8xb8-300e_coco.py
--rw-rw-rw-   0        0        0     7908 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/extensions/configs/mmdet/yolox_s_8xb8-300e_coco.py
--rw-rw-rw-   0        0        0     1883 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/extensions/configs/mmdet/yolox_tiny_8xb8-300e_coco.py
--rw-rw-rw-   0        0        0     1276 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/extensions/configs/mmdet/yolox_tta.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.565857 iinfer-0.7.3/iinfer/extensions/configs/mmpretrain/
--rw-rw-rw-   0        0        0      252 2024-05-03 08:36:21.000000 iinfer-0.7.3/iinfer/extensions/configs/mmpretrain/swin-base_16xb64_in1k-384px.py
--rw-rw-rw-   0        0        0      253 2024-05-03 08:36:59.000000 iinfer-0.7.3/iinfer/extensions/configs/mmpretrain/swin-large_16xb64_in1k-384px.py
--rw-rw-rw-   0        0        0      231 2024-05-03 08:35:35.000000 iinfer-0.7.3/iinfer/extensions/configs/mmpretrain/swin-small_16xb64_in1k.py
--rw-rw-rw-   0        0        0      236 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/extensions/configs/mmpretrain/swin-tiny_16xb64_in1k.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.595859 iinfer-0.7.3/iinfer/extensions/configs/mmseg/
--rw-rw-rw-   0        0        0      139 2024-03-16 14:01:11.000000 iinfer-0.7.3/iinfer/extensions/configs/mmseg/pspnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-rw-rw-   0        0        0      277 2024-03-11 12:50:08.000000 iinfer-0.7.3/iinfer/extensions/configs/mmseg/pspnet_r18-d8_4xb2-80k_cityscapes-512x1024.py
--rw-rw-rw-   0        0        0      299 2024-03-11 13:57:39.000000 iinfer-0.7.3/iinfer/extensions/configs/mmseg/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-rw-rw-   0        0        0     2543 2024-05-03 02:44:50.000000 iinfer-0.7.3/iinfer/extensions/configs/mmseg/san-vit-b16_coco-stuff164k-640x640.py
--rw-rw-rw-   0        0        0     1065 2024-05-02 14:40:03.000000 iinfer-0.7.3/iinfer/extensions/configs/mmseg/san-vit-l14_coco-stuff164k-640x640.py
--rw-rw-rw-   0        0        0      614 2024-03-30 02:18:25.000000 iinfer-0.7.3/iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-rw-rw-   0        0        0      361 2024-03-30 02:17:37.000000 iinfer-0.7.3/iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in22k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-rw-rw-   0        0        0      501 2024-03-23 13:10:40.000000 iinfer-0.7.3/iinfer/extensions/configs/mmseg/swin-small-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-rw-rw-   0        0        0     1752 2024-03-23 13:24:30.000000 iinfer-0.7.3/iinfer/extensions/configs/mmseg/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.634860 iinfer-0.7.3/iinfer/extensions/injection/
--rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.7.3/iinfer/extensions/injection/after_cls_jadge_injection.json
--rw-rw-rw-   0        0        0       99 2024-04-11 14:24:51.000000 iinfer-0.7.3/iinfer/extensions/injection/after_csv_injection.json
--rw-rw-rw-   0        0        0      149 2024-05-02 13:46:36.000000 iinfer-0.7.3/iinfer/extensions/injection/after_det_filter_injection.json
--rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.7.3/iinfer/extensions/injection/after_det_jadge_injection.json
--rw-rw-rw-   0        0        0      176 2024-02-25 01:08:47.000000 iinfer-0.7.3/iinfer/extensions/injection/after_http_injection.json
--rw-rw-rw-   0        0        0      106 2024-05-02 14:15:04.000000 iinfer-0.7.3/iinfer/extensions/injection/after_seg_bbox_injection.json
--rw-rw-rw-   0        0        0      115 2024-04-07 03:42:37.000000 iinfer-0.7.3/iinfer/extensions/injection/after_seg_filter_injection.json
--rw-rw-rw-   0        0        0        2 2024-02-18 07:43:45.000000 iinfer-0.7.3/iinfer/extensions/injection/before_gray_injection.json
--rw-rw-rw-   0        0        0      684 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/extensions/label_coco.txt
--rw-rw-rw-   0        0        0      153 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/extensions/label_voc.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.955863 iinfer-0.7.3/iinfer/licenses/
--rw-rw-rw-   0        0        0     1089 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1121 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt
--rw-rw-rw-   0        0        0    10351 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt
--rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.bottle-websocket.0.2.9(MIT License).txt
--rw-rw-rw-   0        0        0     1080 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt
--rw-rw-rw-   0        0        0     1009 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt
--rw-rw-rw-   0        0        0     1320 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1090 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt
--rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt
--rw-rw-rw-   0        0        0     1523 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt
--rw-rw-rw-   0        0        0     1105 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt
--rw-rw-rw-   0        0        0     1093 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt
--rw-rw-rw-   0        0        0     1094 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt
--rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.gevent-websocket.0.10.1(Copyright 2011-2017 Jeffrey Gelens jeffrey@noppo.pro).txt
--rw-rw-rw-   0        0        0     1260 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt
--rw-rw-rw-   0        0        0     1464 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt
--rw-rw-rw-   0        0        0     1572 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt
--rw-rw-rw-   0        0        0     1117 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt
--rw-rw-rw-   0        0        0     3350 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt
--rw-rw-rw-   0        0        0     4928 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt
--rw-rw-rw-   0        0        0     1088 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt
--rw-rw-rw-   0        0        0    48691 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt
--rw-rw-rw-   0        0        0   154222 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt
--rw-rw-rw-   0        0        0      200 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.packaging.24.0(Apache Software License; BSD License).txt
--rw-rw-rw-   0        0        0    56516 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt
--rw-rw-rw-   0        0        0     1113 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt
--rw-rw-rw-   0        0        0     1642 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt
--rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt
--rw-rw-rw-   0        0        0     1041 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt
--rw-rw-rw-   0        0        0     2942 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt
--rw-rw-rw-   0        0        0     1095 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt
--rw-rw-rw-   0        0        0    10317 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt
--rw-rw-rw-   0        0        0    47742 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt
--rw-rw-rw-   0        0        0     1040 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt
--rw-rw-rw-   0        0        0     1084 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1100 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt
--rw-rw-rw-   0        0        0     1114 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt
--rw-rw-rw-   0        0        0     1349 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt
--rw-rw-rw-   0        0        0     1128 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt
--rw-rw-rw-   0        0        0     1495 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt
--rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt
--rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt
--rw-rw-rw-   0        0        0     6545 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/files.txt
--rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/logconf_client.yml
--rw-rw-rw-   0        0        0      630 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/logconf_gui.yml
--rw-rw-rw-   0        0        0      655 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/logconf_install.yml
--rw-rw-rw-   0        0        0      669 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/logconf_postprocess.yml
--rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/logconf_redis.yml
--rw-rw-rw-   0        0        0      650 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/logconf_server.yml
--rw-rw-rw-   0        0        0      630 2024-04-25 10:56:07.000000 iinfer-0.7.3/iinfer/logconf_web.yml
--rw-rw-rw-   0        0        0     1009 2024-05-06 07:29:42.000000 iinfer-0.7.3/iinfer/version.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.959860 iinfer-0.7.3/iinfer/web/
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.046859 iinfer-0.7.3/iinfer/web/assets/
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.979862 iinfer-0.7.3/iinfer/web/assets/bootstrap/
--rw-rw-rw-   0        0        0    78749 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js
--rw-rw-rw-   0        0        0    80421 2024-02-18 08:27:56.000000 iinfer-0.7.3/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js
--rw-rw-rw-   0        0        0   155851 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css
--rw-rw-rw-   0        0        0   232914 2024-02-18 08:28:29.000000 iinfer-0.7.3/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.024860 iinfer-0.7.3/iinfer/web/assets/iinfer/
--rw-rw-rw-   0        0        0     5860 2024-05-06 08:38:02.000000 iinfer-0.7.3/iinfer/web/assets/iinfer/filer_modal.js
--rw-rw-rw-   0        0        0    17895 2024-05-06 07:34:09.000000 iinfer-0.7.3/iinfer/web/assets/iinfer/list_cmd.js
--rw-rw-rw-   0        0        0     6656 2024-05-06 07:47:25.000000 iinfer-0.7.3/iinfer/web/assets/iinfer/list_pipe.js
--rw-rw-rw-   0        0        0     6108 2024-05-06 08:52:26.000000 iinfer-0.7.3/iinfer/web/assets/iinfer/main.js
--rw-rw-rw-   0        0        0      433 2024-05-06 08:59:02.000000 iinfer-0.7.3/iinfer/web/assets/iinfer/open_capture.js
--rw-rw-rw-   0        0        0      453 2024-05-06 08:59:20.000000 iinfer-0.7.3/iinfer/web/assets/iinfer/open_output_json.js
--rw-rw-rw-   0        0        0      127 2024-04-18 14:57:44.000000 iinfer-0.7.3/iinfer/web/assets/iinfer/svfiler.css
--rw-rw-rw-   0        0        0    25087 2024-05-06 11:21:46.000000 iinfer-0.7.3/iinfer/web/assets/iinfer/svfiler.js
--rw-rw-rw-   0        0        0     1299 2024-05-06 11:27:57.000000 iinfer-0.7.3/iinfer/web/assets/iinfer/view_raw.js
--rw-rw-rw-   0        0        0     6234 2024-05-06 11:33:29.000000 iinfer-0.7.3/iinfer/web/assets/iinfer/view_result.js
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.068859 iinfer-0.7.3/iinfer/web/assets/jquery/
--rw-rw-rw-   0        0        0    86600 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery/jquery.min.3.2.0.js
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.079861 iinfer-0.7.3/iinfer/web/assets/jquery-resizable/
--rw-rw-rw-   0        0        0     3448 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.109858 iinfer-0.7.3/iinfer/web/assets/jquery-ui/
--rw-rw-rw-   0        0        0    14615 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/AUTHORS.txt
--rw-rw-rw-   0        0        0     1860 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.153007 iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/
--rw-rw-rw-   0        0        0     7142 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png
--rw-rw-rw-   0        0        0     7126 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png
--rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png
--rw-rw-rw-   0        0        0     7163 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png
--rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png
--rw-rw-rw-   0        0        0     6539 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png
--rw-rw-rw-   0        0        0    32136 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/jquery-ui.min.css
--rw-rw-rw-   0        0        0   255089 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/jquery-ui.min.js
--rw-rw-rw-   0        0        0    15564 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css
--rw-rw-rw-   0        0        0    13895 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css
--rw-rw-rw-   0        0        0     1886 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/package.json
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.046859 iinfer-0.7.3/iinfer/web/assets/lightbox2/
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.159007 iinfer-0.7.3/iinfer/web/assets/lightbox2/css/
--rw-rw-rw-   0        0        0     2532 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/lightbox2/css/lightbox.min.css
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.184598 iinfer-0.7.3/iinfer/web/assets/lightbox2/images/
--rw-rw-rw-   0        0        0      280 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/lightbox2/images/close.png
--rw-rw-rw-   0        0        0     8476 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/lightbox2/images/loading.gif
--rw-rw-rw-   0        0        0     1350 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/lightbox2/images/next.png
--rw-rw-rw-   0        0        0     1360 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/lightbox2/images/prev.png
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.188115 iinfer-0.7.3/iinfer/web/assets/lightbox2/js/
--rw-rw-rw-   0        0        0     9768 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/lightbox2/js/lightbox.min.js
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.048860 iinfer-0.7.3/iinfer/web/assets/tree-menu/
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.192715 iinfer-0.7.3/iinfer/web/assets/tree-menu/css/
--rw-rw-rw-   0        0        0     1101 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/tree-menu/css/tree-menu.css
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.221422 iinfer-0.7.3/iinfer/web/assets/tree-menu/image/
--rw-rw-rw-   0        0        0      248 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/tree-menu/image/file.png
--rw-rw-rw-   0        0        0      284 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/tree-menu/image/folder-close.png
--rw-rw-rw-   0        0        0      301 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/tree-menu/image/folder-open.png
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.226422 iinfer-0.7.3/iinfer/web/assets/tree-menu/js/
--rw-rw-rw-   0        0        0     1029 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/tree-menu/js/tree-menu.js
--rw-rw-rw-   0        0        0    31077 2024-05-06 05:48:36.000000 iinfer-0.7.3/iinfer/web/gui.html
-drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.222862 iinfer-0.7.3/iinfer.egg-info/
--rw-rw-rw-   0        0        0     5553 2024-05-06 13:44:19.000000 iinfer-0.7.3/iinfer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8706 2024-05-06 13:44:19.000000 iinfer-0.7.3/iinfer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 13:44:19.000000 iinfer-0.7.3/iinfer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-06 13:44:19.000000 iinfer-0.7.3/iinfer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       88 2024-05-06 13:44:19.000000 iinfer-0.7.3/iinfer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-06 13:44:19.000000 iinfer-0.7.3/iinfer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 13:44:21.231421 iinfer-0.7.3/setup.cfg
--rw-rw-rw-   0        0        0     2181 2024-05-03 08:40:54.000000 iinfer-0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.865690 iinfer-0.7.4/
+-rw-rw-rw-   0        0        0     1117 2024-02-15 15:34:04.000000 iinfer-0.7.4/LICENSE
+-rw-rw-rw-   0        0        0     5553 2024-05-18 12:21:49.864690 iinfer-0.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4619 2024-03-11 12:57:36.000000 iinfer-0.7.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.160674 iinfer-0.7.4/iinfer/
+-rw-rw-rw-   0        0        0       69 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/__init__.py
+-rw-rw-rw-   0        0        0      109 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.238693 iinfer-0.7.4/iinfer/app/
+-rw-rw-rw-   0        0        0       73 2024-03-10 12:26:23.000000 iinfer-0.7.4/iinfer/app/__init__.py
+-rw-rw-rw-   0        0        0    38010 2024-05-18 10:07:37.000000 iinfer-0.7.4/iinfer/app/app.py
+-rw-rw-rw-   0        0        0    37331 2024-05-12 08:50:34.000000 iinfer-0.7.4/iinfer/app/client.py
+-rw-rw-rw-   0        0        0    14838 2024-05-12 02:19:33.000000 iinfer-0.7.4/iinfer/app/common.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.243690 iinfer-0.7.4/iinfer/app/commons/
+-rw-rw-rw-   0        0        0     5433 2024-02-26 12:32:33.000000 iinfer-0.7.4/iinfer/app/commons/convert.py
+-rw-rw-rw-   0        0        0     8720 2024-05-12 12:08:32.000000 iinfer-0.7.4/iinfer/app/commons/module.py
+-rw-rw-rw-   0        0        0     3613 2024-05-06 11:42:49.000000 iinfer-0.7.4/iinfer/app/gui.py
+-rw-rw-rw-   0        0        0     5247 2024-04-11 12:30:41.000000 iinfer-0.7.4/iinfer/app/injection.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.272693 iinfer-0.7.4/iinfer/app/injections/
+-rw-rw-rw-   0        0        0     2023 2024-04-11 11:13:52.000000 iinfer-0.7.4/iinfer/app/injections/after_cls_jadge_injection.py
+-rw-rw-rw-   0        0        0     4500 2024-04-06 14:50:20.000000 iinfer-0.7.4/iinfer/app/injections/after_csv_injection.py
+-rw-rw-rw-   0        0        0     6735 2024-05-02 03:57:31.000000 iinfer-0.7.4/iinfer/app/injections/after_det_filter_injection.py
+-rw-rw-rw-   0        0        0     8540 2024-04-07 07:16:07.000000 iinfer-0.7.4/iinfer/app/injections/after_det_jadge_injection.py
+-rw-rw-rw-   0        0        0     4790 2024-04-07 00:11:59.000000 iinfer-0.7.4/iinfer/app/injections/after_http_injection.py
+-rw-rw-rw-   0        0        0     9077 2024-04-11 13:28:27.000000 iinfer-0.7.4/iinfer/app/injections/after_seg_bbox_injection.py
+-rw-rw-rw-   0        0        0     8688 2024-04-11 13:41:09.000000 iinfer-0.7.4/iinfer/app/injections/after_seg_filter_injection.py
+-rw-rw-rw-   0        0        0     1810 2024-02-25 07:58:13.000000 iinfer-0.7.4/iinfer/app/injections/before_grayimg_injection.py
+-rw-rw-rw-   0        0        0    17772 2024-05-18 07:06:46.000000 iinfer-0.7.4/iinfer/app/install.py
+-rw-rw-rw-   0        0        0   172620 2024-05-18 09:56:20.000000 iinfer-0.7.4/iinfer/app/options.py
+-rw-rw-rw-   0        0        0     5309 2024-05-02 02:25:26.000000 iinfer-0.7.4/iinfer/app/postprocess.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.302692 iinfer-0.7.4/iinfer/app/postprocesses/
+-rw-rw-rw-   0        0        0     1935 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/app/postprocesses/cls_jadge.py
+-rw-rw-rw-   0        0        0     2393 2024-04-06 14:52:31.000000 iinfer-0.7.4/iinfer/app/postprocesses/csv.py
+-rw-rw-rw-   0        0        0     4197 2024-03-10 09:01:15.000000 iinfer-0.7.4/iinfer/app/postprocesses/det_clip.py
+-rw-rw-rw-   0        0        0     5063 2024-03-17 02:51:08.000000 iinfer-0.7.4/iinfer/app/postprocesses/det_face_store.py
+-rw-rw-rw-   0        0        0     4444 2024-04-11 13:48:21.000000 iinfer-0.7.4/iinfer/app/postprocesses/det_filter.py
+-rw-rw-rw-   0        0        0     5201 2024-04-07 07:20:08.000000 iinfer-0.7.4/iinfer/app/postprocesses/det_jadge.py
+-rw-rw-rw-   0        0        0     3813 2024-04-07 00:25:09.000000 iinfer-0.7.4/iinfer/app/postprocesses/httpreq.py
+-rw-rw-rw-   0        0        0     4369 2024-04-11 13:06:06.000000 iinfer-0.7.4/iinfer/app/postprocesses/seg_bbox.py
+-rw-rw-rw-   0        0        0     4252 2024-04-11 12:27:14.000000 iinfer-0.7.4/iinfer/app/postprocesses/seg_filter.py
+-rw-rw-rw-   0        0        0     6604 2024-05-18 08:12:24.000000 iinfer-0.7.4/iinfer/app/predict.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.356691 iinfer-0.7.4/iinfer/app/predicts/
+-rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/app/predicts/__init__.py
+-rw-rw-rw-   0        0        0     3675 2024-05-18 08:13:34.000000 iinfer-0.7.4/iinfer/app/predicts/diffusers_stablediffusionpipeline_txt2img.py
+-rw-rw-rw-   0        0        0     7583 2024-05-18 08:15:04.000000 iinfer-0.7.4/iinfer/app/predicts/insightface_det.py
+-rw-rw-rw-   0        0        0     7983 2024-05-18 07:12:31.000000 iinfer-0.7.4/iinfer/app/predicts/llamaindex_elyza_search.py
+-rw-rw-rw-   0        0        0     4067 2024-05-18 09:13:57.000000 iinfer-0.7.4/iinfer/app/predicts/mmdet_det_YoloX.py
+-rw-rw-rw-   0        0        0      384 2024-05-04 02:00:25.000000 iinfer-0.7.4/iinfer/app/predicts/mmdet_det_YoloX_Lite.py
+-rw-rw-rw-   0        0        0     4632 2024-05-18 08:10:46.000000 iinfer-0.7.4/iinfer/app/predicts/mmpretrain_cls_swin.py
+-rw-rw-rw-   0        0        0      418 2024-05-04 02:00:18.000000 iinfer-0.7.4/iinfer/app/predicts/mmpretrain_cls_swin_Lite.py
+-rw-rw-rw-   0        0        0     5645 2024-05-18 08:19:06.000000 iinfer-0.7.4/iinfer/app/predicts/mmseg_seg_PSPNet.py
+-rw-rw-rw-   0        0        0      377 2024-05-02 14:44:28.000000 iinfer-0.7.4/iinfer/app/predicts/mmseg_seg_San.py
+-rw-rw-rw-   0        0        0      386 2024-03-30 02:49:57.000000 iinfer-0.7.4/iinfer/app/predicts/mmseg_seg_SwinUpernet.py
+-rw-rw-rw-   0        0        0     4574 2024-05-18 08:19:33.000000 iinfer-0.7.4/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py
+-rw-rw-rw-   0        0        0     3326 2024-05-18 08:31:16.000000 iinfer-0.7.4/iinfer/app/predicts/onnx_det_TinyYoloV3.py
+-rw-rw-rw-   0        0        0     5411 2024-05-18 08:21:15.000000 iinfer-0.7.4/iinfer/app/predicts/onnx_det_YoloV3.py
+-rw-rw-rw-   0        0        0     9753 2024-05-18 08:48:24.000000 iinfer-0.7.4/iinfer/app/predicts/onnx_det_YoloX.py
+-rw-rw-rw-   0        0        0      369 2024-05-12 07:56:58.000000 iinfer-0.7.4/iinfer/app/predicts/onnx_det_YoloX_Lite.py
+-rw-rw-rw-   0        0        0     2706 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/app/redis.py
+-rw-rw-rw-   0        0        0    52569 2024-05-18 09:08:20.000000 iinfer-0.7.4/iinfer/app/server.py
+-rw-rw-rw-   0        0        0    27306 2024-05-18 12:19:05.000000 iinfer-0.7.4/iinfer/app/web.py
+-rw-rw-rw-   0        0        0       54 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/config.yml
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.367694 iinfer-0.7.4/iinfer/docker/
+-rw-rw-rw-   0        0        0      885 2024-05-11 09:05:19.000000 iinfer-0.7.4/iinfer/docker/Dockerfile
+-rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/docker/__init__.py
+-rw-rw-rw-   0        0        0      131 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/docker/build.sh
+-rw-rw-rw-   0        0        0      319 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/docker/docker-compose.yml
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.390689 iinfer-0.7.4/iinfer/extensions/
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.093654 iinfer-0.7.4/iinfer/extensions/configs/
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.417693 iinfer-0.7.4/iinfer/extensions/configs/mmdet/
+-rw-rw-rw-   0        0        0      273 2024-05-03 08:33:49.000000 iinfer-0.7.4/iinfer/extensions/configs/mmdet/yolox_l_8xb8-300e_coco.py
+-rw-rw-rw-   0        0        0     7908 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/extensions/configs/mmdet/yolox_s_8xb8-300e_coco.py
+-rw-rw-rw-   0        0        0     1883 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/extensions/configs/mmdet/yolox_tiny_8xb8-300e_coco.py
+-rw-rw-rw-   0        0        0     1276 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/extensions/configs/mmdet/yolox_tta.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.445692 iinfer-0.7.4/iinfer/extensions/configs/mmpretrain/
+-rw-rw-rw-   0        0        0      252 2024-05-03 08:36:21.000000 iinfer-0.7.4/iinfer/extensions/configs/mmpretrain/swin-base_16xb64_in1k-384px.py
+-rw-rw-rw-   0        0        0      253 2024-05-03 08:36:59.000000 iinfer-0.7.4/iinfer/extensions/configs/mmpretrain/swin-large_16xb64_in1k-384px.py
+-rw-rw-rw-   0        0        0      231 2024-05-03 08:35:35.000000 iinfer-0.7.4/iinfer/extensions/configs/mmpretrain/swin-small_16xb64_in1k.py
+-rw-rw-rw-   0        0        0      236 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/extensions/configs/mmpretrain/swin-tiny_16xb64_in1k.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.495693 iinfer-0.7.4/iinfer/extensions/configs/mmseg/
+-rw-rw-rw-   0        0        0      139 2024-03-16 14:01:11.000000 iinfer-0.7.4/iinfer/extensions/configs/mmseg/pspnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-rw-rw-   0        0        0      277 2024-03-11 12:50:08.000000 iinfer-0.7.4/iinfer/extensions/configs/mmseg/pspnet_r18-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-rw-rw-   0        0        0      299 2024-03-11 13:57:39.000000 iinfer-0.7.4/iinfer/extensions/configs/mmseg/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-rw-rw-   0        0        0     2543 2024-05-03 02:44:50.000000 iinfer-0.7.4/iinfer/extensions/configs/mmseg/san-vit-b16_coco-stuff164k-640x640.py
+-rw-rw-rw-   0        0        0     1065 2024-05-02 14:40:03.000000 iinfer-0.7.4/iinfer/extensions/configs/mmseg/san-vit-l14_coco-stuff164k-640x640.py
+-rw-rw-rw-   0        0        0      614 2024-03-30 02:18:25.000000 iinfer-0.7.4/iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-rw-rw-   0        0        0      361 2024-03-30 02:17:37.000000 iinfer-0.7.4/iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in22k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-rw-rw-   0        0        0      501 2024-03-23 13:10:40.000000 iinfer-0.7.4/iinfer/extensions/configs/mmseg/swin-small-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-rw-rw-   0        0        0     1752 2024-03-23 13:24:30.000000 iinfer-0.7.4/iinfer/extensions/configs/mmseg/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.535695 iinfer-0.7.4/iinfer/extensions/injection/
+-rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.7.4/iinfer/extensions/injection/after_cls_jadge_injection.json
+-rw-rw-rw-   0        0        0       99 2024-04-11 14:24:51.000000 iinfer-0.7.4/iinfer/extensions/injection/after_csv_injection.json
+-rw-rw-rw-   0        0        0      149 2024-05-02 13:46:36.000000 iinfer-0.7.4/iinfer/extensions/injection/after_det_filter_injection.json
+-rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.7.4/iinfer/extensions/injection/after_det_jadge_injection.json
+-rw-rw-rw-   0        0        0      176 2024-02-25 01:08:47.000000 iinfer-0.7.4/iinfer/extensions/injection/after_http_injection.json
+-rw-rw-rw-   0        0        0      106 2024-05-02 14:15:04.000000 iinfer-0.7.4/iinfer/extensions/injection/after_seg_bbox_injection.json
+-rw-rw-rw-   0        0        0      115 2024-04-07 03:42:37.000000 iinfer-0.7.4/iinfer/extensions/injection/after_seg_filter_injection.json
+-rw-rw-rw-   0        0        0        2 2024-02-18 07:43:45.000000 iinfer-0.7.4/iinfer/extensions/injection/before_gray_injection.json
+-rw-rw-rw-   0        0        0      684 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/extensions/label_coco.txt
+-rw-rw-rw-   0        0        0      153 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/extensions/label_voc.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.736696 iinfer-0.7.4/iinfer/licenses/
+-rw-rw-rw-   0        0        0     1089 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1121 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt
+-rw-rw-rw-   0        0        0    10351 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt
+-rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.bottle-websocket.0.2.9(MIT License).txt
+-rw-rw-rw-   0        0        0     1080 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt
+-rw-rw-rw-   0        0        0     1009 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt
+-rw-rw-rw-   0        0        0     1320 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1090 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt
+-rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1523 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt
+-rw-rw-rw-   0        0        0     1105 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt
+-rw-rw-rw-   0        0        0     1093 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1094 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt
+-rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.gevent-websocket.0.10.1(Copyright 2011-2017 Jeffrey Gelens jeffrey@noppo.pro).txt
+-rw-rw-rw-   0        0        0     1260 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt
+-rw-rw-rw-   0        0        0     1464 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt
+-rw-rw-rw-   0        0        0     1572 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt
+-rw-rw-rw-   0        0        0     1117 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt
+-rw-rw-rw-   0        0        0     3350 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt
+-rw-rw-rw-   0        0        0     4928 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt
+-rw-rw-rw-   0        0        0     1088 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt
+-rw-rw-rw-   0        0        0    48691 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt
+-rw-rw-rw-   0        0        0   154222 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt
+-rw-rw-rw-   0        0        0      200 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.packaging.24.0(Apache Software License; BSD License).txt
+-rw-rw-rw-   0        0        0    56516 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt
+-rw-rw-rw-   0        0        0     1113 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1642 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt
+-rw-rw-rw-   0        0        0     1041 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt
+-rw-rw-rw-   0        0        0     2942 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt
+-rw-rw-rw-   0        0        0     1095 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt
+-rw-rw-rw-   0        0        0    10317 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt
+-rw-rw-rw-   0        0        0    47742 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1040 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1084 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1100 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1114 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt
+-rw-rw-rw-   0        0        0     1349 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt
+-rw-rw-rw-   0        0        0     1128 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1495 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt
+-rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt
+-rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt
+-rw-rw-rw-   0        0        0     6545 2024-03-27 11:58:45.000000 iinfer-0.7.4/iinfer/licenses/files.txt
+-rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/logconf_client.yml
+-rw-rw-rw-   0        0        0      630 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/logconf_gui.yml
+-rw-rw-rw-   0        0        0      655 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/logconf_install.yml
+-rw-rw-rw-   0        0        0      669 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/logconf_postprocess.yml
+-rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/logconf_redis.yml
+-rw-rw-rw-   0        0        0      650 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/logconf_server.yml
+-rw-rw-rw-   0        0        0      630 2024-04-25 10:56:07.000000 iinfer-0.7.4/iinfer/logconf_web.yml
+-rw-rw-rw-   0        0        0     1010 2024-05-18 11:33:16.000000 iinfer-0.7.4/iinfer/version.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.742692 iinfer-0.7.4/iinfer/web/
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.099121 iinfer-0.7.4/iinfer/web/assets/
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.758691 iinfer-0.7.4/iinfer/web/assets/bootstrap/
+-rw-rw-rw-   0        0        0    78749 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js
+-rw-rw-rw-   0        0        0    80421 2024-02-18 08:27:56.000000 iinfer-0.7.4/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js
+-rw-rw-rw-   0        0        0   155851 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css
+-rw-rw-rw-   0        0        0   232914 2024-02-18 08:28:29.000000 iinfer-0.7.4/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.784693 iinfer-0.7.4/iinfer/web/assets/iinfer/
+-rw-rw-rw-   0        0        0     5860 2024-05-06 08:38:02.000000 iinfer-0.7.4/iinfer/web/assets/iinfer/filer_modal.js
+-rw-rw-rw-   0        0        0    18037 2024-05-18 11:48:19.000000 iinfer-0.7.4/iinfer/web/assets/iinfer/list_cmd.js
+-rw-rw-rw-   0        0        0     6656 2024-05-06 07:47:25.000000 iinfer-0.7.4/iinfer/web/assets/iinfer/list_pipe.js
+-rw-rw-rw-   0        0        0     6108 2024-05-06 08:52:26.000000 iinfer-0.7.4/iinfer/web/assets/iinfer/main.js
+-rw-rw-rw-   0        0        0      433 2024-05-06 08:59:02.000000 iinfer-0.7.4/iinfer/web/assets/iinfer/open_capture.js
+-rw-rw-rw-   0        0        0      453 2024-05-06 08:59:20.000000 iinfer-0.7.4/iinfer/web/assets/iinfer/open_output_json.js
+-rw-rw-rw-   0        0        0      127 2024-04-18 14:57:44.000000 iinfer-0.7.4/iinfer/web/assets/iinfer/svfiler.css
+-rw-rw-rw-   0        0        0    25087 2024-05-06 11:21:46.000000 iinfer-0.7.4/iinfer/web/assets/iinfer/svfiler.js
+-rw-rw-rw-   0        0        0     1299 2024-05-06 11:27:57.000000 iinfer-0.7.4/iinfer/web/assets/iinfer/view_raw.js
+-rw-rw-rw-   0        0        0     6234 2024-05-06 11:33:29.000000 iinfer-0.7.4/iinfer/web/assets/iinfer/view_result.js
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.787691 iinfer-0.7.4/iinfer/web/assets/jquery/
+-rw-rw-rw-   0        0        0    86600 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/jquery/jquery.min.3.2.0.js
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.790694 iinfer-0.7.4/iinfer/web/assets/jquery-resizable/
+-rw-rw-rw-   0        0        0     3448 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.810690 iinfer-0.7.4/iinfer/web/assets/jquery-ui/
+-rw-rw-rw-   0        0        0    14615 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/jquery-ui/AUTHORS.txt
+-rw-rw-rw-   0        0        0     1860 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/jquery-ui/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.828693 iinfer-0.7.4/iinfer/web/assets/jquery-ui/images/
+-rw-rw-rw-   0        0        0     7142 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png
+-rw-rw-rw-   0        0        0     7126 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png
+-rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png
+-rw-rw-rw-   0        0        0     7163 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png
+-rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png
+-rw-rw-rw-   0        0        0     6539 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png
+-rw-rw-rw-   0        0        0    32136 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/jquery-ui/jquery-ui.min.css
+-rw-rw-rw-   0        0        0   255089 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/jquery-ui/jquery-ui.min.js
+-rw-rw-rw-   0        0        0    15564 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css
+-rw-rw-rw-   0        0        0    13895 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css
+-rw-rw-rw-   0        0        0     1886 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/jquery-ui/package.json
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.099121 iinfer-0.7.4/iinfer/web/assets/lightbox2/
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.830693 iinfer-0.7.4/iinfer/web/assets/lightbox2/css/
+-rw-rw-rw-   0        0        0     2532 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/lightbox2/css/lightbox.min.css
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.844690 iinfer-0.7.4/iinfer/web/assets/lightbox2/images/
+-rw-rw-rw-   0        0        0      280 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/lightbox2/images/close.png
+-rw-rw-rw-   0        0        0     8476 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/lightbox2/images/loading.gif
+-rw-rw-rw-   0        0        0     1350 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/lightbox2/images/next.png
+-rw-rw-rw-   0        0        0     1360 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/lightbox2/images/prev.png
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.846690 iinfer-0.7.4/iinfer/web/assets/lightbox2/js/
+-rw-rw-rw-   0        0        0     9768 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/lightbox2/js/lightbox.min.js
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.104131 iinfer-0.7.4/iinfer/web/assets/tree-menu/
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.849691 iinfer-0.7.4/iinfer/web/assets/tree-menu/css/
+-rw-rw-rw-   0        0        0     1101 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/tree-menu/css/tree-menu.css
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.860690 iinfer-0.7.4/iinfer/web/assets/tree-menu/image/
+-rw-rw-rw-   0        0        0      248 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/tree-menu/image/file.png
+-rw-rw-rw-   0        0        0      284 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/tree-menu/image/folder-close.png
+-rw-rw-rw-   0        0        0      301 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/tree-menu/image/folder-open.png
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.862693 iinfer-0.7.4/iinfer/web/assets/tree-menu/js/
+-rw-rw-rw-   0        0        0     1029 2024-02-15 15:34:05.000000 iinfer-0.7.4/iinfer/web/assets/tree-menu/js/tree-menu.js
+-rw-rw-rw-   0        0        0    31077 2024-05-06 05:48:36.000000 iinfer-0.7.4/iinfer/web/gui.html
+drwxrwxrwx   0        0        0        0 2024-05-18 12:21:49.189692 iinfer-0.7.4/iinfer.egg-info/
+-rw-rw-rw-   0        0        0     5553 2024-05-18 12:21:48.000000 iinfer-0.7.4/iinfer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8719 2024-05-18 12:21:49.000000 iinfer-0.7.4/iinfer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 12:21:48.000000 iinfer-0.7.4/iinfer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-18 12:21:48.000000 iinfer-0.7.4/iinfer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2024-05-18 12:21:48.000000 iinfer-0.7.4/iinfer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-18 12:21:48.000000 iinfer-0.7.4/iinfer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 12:21:49.865690 iinfer-0.7.4/setup.cfg
+-rw-rw-rw-   0        0        0     2198 2024-05-12 01:49:05.000000 iinfer-0.7.4/setup.py
```

### Comparing `iinfer-0.7.3/LICENSE` & `iinfer-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/PKG-INFO` & `iinfer-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iinfer
-Version: 0.7.3
+Version: 0.7.4
 Summary: iinfer: An application that executes AI model files in onnx or mmlab format.
 Home-page: https://github.com/hamacom2004jp/iinfer
 Author: hamacom2004jp
 Author-email: hamacom2004jp@gmail.com
 Maintainer: hamacom2004jp
 Maintainer-email: hamacom2004jp@gmail.com
 License: MIT
```

### Comparing `iinfer-0.7.3/README.md` & `iinfer-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/client.py` & `iinfer-0.7.4/iinfer/app/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -210,22 +210,25 @@
         if not ret: return label_file_b64
         ret, color_file_b64 = _conf_b64("color_file", color_file)
         if not ret: return color_file_b64
         ret, before_injection_conf_b64 = _conf_b64("before_injection_conf", before_injection_conf)
         if not ret: return before_injection_conf_b64
         ret, after_injection_conf_b64 = _conf_b64("after_injection_conf", after_injection_conf)
         if not ret: return after_injection_conf_b64
-        if model_file is not None and not model_file.startswith("http"):
-            model_file = Path(model_file)
-            if model_file.exists():
-                with open(model_file, "rb") as mf:
-                    model_bytes_b64 = base64.b64encode(mf.read()).decode('utf-8')
+        if model_file is not None and not model_file.startswith("http://") and not model_file.startswith("https://"):
+            if common.BASE_MODELS[predict_type]['required_model_weight']:
+                model_file = Path(model_file)
+                if model_file.exists():
+                    with open(model_file, "rb") as mf:
+                        model_bytes_b64 = base64.b64encode(mf.read()).decode('utf-8')
+                else:
+                    self.logger.error(f"model_file {model_file} does not exist")
+                    return {"error": f"model_file {model_file} does not exist"}
             else:
-                self.logger.error(f"model_file {model_file} does not exist")
-                return {"error": f"model_file {model_file} does not exist"}
+                model_bytes_b64 = None
         else:
             model_bytes_b64 = None
         def _name_b64(aname:str, files:List[Path]):
             if files is not None:
                 b64s = []
                 names = []
                 for p in files:
@@ -331,24 +334,24 @@
         return res_json
 
 
     def stop_server(self, timeout:int = 60):
         res_json = self._proc(self.svname, 'stop_server', [], timeout=timeout)
         return res_json
 
-    def predict(self, name:str, image = None, image_file = None, image_file_enable:bool=True, image_type:str = 'jpeg', output_image_file:str = None, output_preview:bool=False, nodraw:bool=False, timeout:int = 60):
+    def predict(self, name:str, image = None, image_file = None, image_file_enable:bool=True, pred_input_type:str = 'jpeg', output_image_file:str = None, output_preview:bool=False, nodraw:bool=False, timeout:int = 60):
         """
         画像をRedisサーバーに送信し、推論結果を取得する
 
         Args:
             name (str): モデル名
             image (np.ndarray | bytes, optional): 画像データ. Defaults to None. np.ndarray型の場合はデコードしない(RGBであること).
             image_file (str|file-like object, optional): 画像ファイルのパス. Defaults to None.
             image_file_enable (bool, optional): 画像ファイルを使用するかどうか. Defaults to True. image_fileがNoneでなく、このパラメーターがTrueの場合はimage_fileを使用する.
-            image_type (str, optional): 画像の形式. Defaults to 'jpeg'.
+            pred_input_type (str, optional): 画像の形式. Defaults to 'jpeg'.
             output_image_file (str, optional): 予測結果の画像ファイルのパス. Defaults to None.
             output_preview (bool, optional): 予測結果の画像をプレビューするかどうか. Defaults to False.
             nodraw (bool, optional): 描画フラグ. Defaults to False.
             timeout (int, optional): タイムアウト時間. Defaults to 60.
 
         Returns:
             dict: Redisサーバーからの応答
@@ -366,50 +369,51 @@
         npy_b64 = None
         simgloadtime = time.perf_counter()
         if image_file is not None and image_file_enable:
             if type(image_file) == str:
                 if not Path(image_file).exists():
                     self.logger.error(f"Not found image_file. {image_file}.")
                     return {"error": f"Not found image_file. {image_file}."}
-            if image_type == 'jpeg' or image_type == 'png' or image_type == 'bmp':
+            if pred_input_type == 'jpeg' or pred_input_type == 'png' or pred_input_type == 'bmp':
                 f = None
                 try:
                     f = image_file if type(image_file) is not str else open(image_file, "rb")
                     img_npy = convert.imgfile2npy(f)
                 finally:
                     if f is not None: f.close()
-            elif image_type == 'capture':
+            elif pred_input_type == 'capture':
                 f = None
                 try:
                     f = image_file if type(image_file) is not str else open(image_file, "r", encoding='utf-8')
                     res_list = []
                     for line in f:
                         if type(line) is bytes:
-                            line = line.decode('utf-8').strip()
-                        capture_data = line.split(',')
+                            line = line.decode('utf-8')
+                        capture_data = line.strip().split(',')
                         t = capture_data[0]
                         img = capture_data[1]
                         h = int(capture_data[2])
                         w = int(capture_data[3])
                         c = int(capture_data[4])
                         fn = Path(capture_data[5].strip())
                         if t == 'capture':
                             img_npy = convert.b64str2npy(img, shape=(h, w, c) if c > 0 else (h, w))
                         else:
                             img_npy = convert.imgbytes2npy(convert.b64str2bytes(img))
-                        res_json = self.predict(name, image=img_npy, image_file=fn, image_file_enable=False, output_image_file=output_image_file, output_preview=output_preview, nodraw=nodraw, timeout=timeout)
+                        res_json = self.predict(name, image=img_npy, image_file=fn, image_file_enable=False,
+                                                output_image_file=output_image_file, output_preview=output_preview, nodraw=nodraw, timeout=timeout)
                         res_list.append(res_json)
                     if len(res_list) <= 0:
                         return {"warn": f"capture file is no data."}
                     elif len(res_list) == 1:
                         return res_list[0]
                     return res_list
                 finally:
                     if f is not None: f.close()
-            elif image_type == 'output_json':
+            elif pred_input_type == 'output_json':
                 f = None
                 try:
                     f = image_file if type(image_file) is not str else open(image_file, "r", encoding='utf-8')
                     res_list = []
                     for line in f:
                         res_json = json.loads(line)
                         if not ("output_image" in res_json and "output_image_shape" in res_json and "output_image_name" in res_json):
@@ -422,62 +426,88 @@
                     if len(res_list) <= 0:
                         return {"warn": f"output_json file is no data."}
                     elif len(res_list) == 1:
                         return res_list[0]
                     return res_list
                 finally:
                     if f is not None: f.close()
+            elif pred_input_type == 'prompt':
+                f = None
+                try:
+                    f = image_file if type(image_file) is not str else open(image_file, "r", encoding='utf-8')
+                    res_list = []
+                    for line in f:
+                        if type(line) is bytes:
+                            line = line.decode('utf-8')
+                        prompt_data = line.strip().split(',')
+                        fn = Path(prompt_data[2].strip())
+                        res_json = self.predict(name, image=line, image_file=fn, image_file_enable=False, pred_input_type='prompt',
+                                                output_image_file=output_image_file, output_preview=output_preview, nodraw=nodraw, timeout=timeout)
+                        res_list.append(res_json)
+                    if len(res_list) <= 0:
+                        return {"warn": f"prompt file is no data."}
+                    elif len(res_list) == 1:
+                        return res_list[0]
+                    return res_list
+                finally:
+                    if f is not None: f.close()
             else:
-                self.logger.error(f"image_type is invalid. {image_type}.")
-                return {"error": f"image_type is invalid. {image_type}."}
+                self.logger.error(f"pred_input_type is invalid. {pred_input_type}.")
+                return {"error": f"pred_input_type is invalid. {pred_input_type}."}
         else:
             if type(image) == np.ndarray:
                 img_npy = image
                 if image_file is None: image_file = f'{datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")}.capture'
                 image_file_enable = False
-            elif image_type == 'capture':
+            elif pred_input_type == 'capture':
                 capture_data = image.split(',')
                 #self.logger.info(f"capture_data={capture_data[1:]}")
                 t = capture_data[0]
                 img = capture_data[1]
                 h = int(capture_data[2])
                 w = int(capture_data[3])
                 c = int(capture_data[4])
                 if image_file is None: image_file = capture_data[5]
                 image_file_enable = False
                 if t == 'capture':
                     img_npy = convert.b64str2npy(img, shape=(h, w, c) if c > 0 else (h, w))
                 else:
                     img_npy = convert.imgbytes2npy(convert.b64str2bytes(img))
-            elif image_type == 'output_json':
+            elif pred_input_type == 'prompt':
+                prompt_data = image.split(',')
+                t = prompt_data[0]
+                prompt_b64 = prompt_data[1]
+                if image_file is None: image_file = prompt_data[2]
+            elif pred_input_type == 'output_json':
                 res_json = json.loads(image)
                 if not ("output_image" in res_json and "output_image_shape" in res_json and "output_image_name" in res_json):
                     self.logger.error(f"image_file data is invalid. Not found output_image or output_image_shape or output_image_name key.")
                     return {"error": f"image_file data is invalid. Not found output_image or output_image_shape or output_image_name key."}
                 img_npy = convert.b64str2npy(res_json["output_image"], shape=res_json["output_image_shape"])
                 if image_file is None: image_file = res_json["output_image_name"]
                 image_file_enable = False
-            elif image_type == 'jpeg' or image_type == 'png' or image_type == 'bmp':
+            elif pred_input_type == 'jpeg' or pred_input_type == 'png' or pred_input_type == 'bmp':
                 img_npy = convert.imgbytes2npy(image)
-                if image_file is None: image_file = f'{datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")}.{image_type}'
+                if image_file is None: image_file = f'{datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")}.{pred_input_type}'
                 image_file_enable = False
             else:
-                self.logger.error(f"image_type is invalid. {image_type}.")
-                return {"error": f"image_type is invalid. {image_type}."}
+                self.logger.error(f"pred_input_type is invalid. {pred_input_type}.")
+                return {"error": f"pred_input_type is invalid. {pred_input_type}."}
 
-        npy_b64 = convert.npy2b64str(img_npy)
-        #img_npy2 = np.frombuffer(base64.b64decode(npy_b64), dtype='uint8').reshape(img_npy.shape)
         eimgloadtime = time.perf_counter()
-        res_json = self._proc(self.svname, 'predict',
-                              [name, npy_b64, str(nodraw), str(img_npy.shape[0]), str(img_npy.shape[1]),
-                               str(img_npy.shape[2] if len(img_npy.shape) > 2 else '-1'), image_file], timeout=timeout)
+        if pred_input_type == 'prompt':
+            res_json = self._proc(self.svname, 'predict',
+                                  [name, prompt_b64, str(nodraw), str(-1), str(-1), str(-1), image_file], timeout=timeout)
+        else:
+            npy_b64 = convert.npy2b64str(img_npy)
+            res_json = self._proc(self.svname, 'predict',
+                                  [name, npy_b64, str(nodraw), str(img_npy.shape[0]), str(img_npy.shape[1]),
+                                  str(img_npy.shape[2] if len(img_npy.shape) > 2 else '-1'), image_file], timeout=timeout)
         soutputtime = time.perf_counter()
         if "output_image" in res_json and "output_image_shape" in res_json:
-            #byteio = BytesIO(base64.b64decode(res_json["output_image"]))
-            #img_npy = np.load(byteio)
             img_npy = convert.b64str2npy(res_json["output_image"], res_json["output_image_shape"])
             if output_image_file is not None:
                 exp = Path(output_image_file).suffix
                 exp = exp[1:] if exp[0] == '.' else exp
                 convert.npy2imgfile(img_npy, output_image_file=output_image_file, image_type=exp)
             if output_preview:
                 # RGB画像をBGR画像に変換
@@ -659,7 +689,24 @@
                 if interval - (end - start) > 0:
                     time.sleep(interval - (end - start))
 
         except KeyboardInterrupt:
             self.logger.info("KeyboardInterrupt", exc_info=True)
         finally:
             cap.release()
+
+    def prompt(self, prompt_format='{prompt}', prompt_form:bool=False):
+        try:
+            self.is_running = True
+            while self.is_running:
+                if not prompt_form:
+                    prompt = prompt_format.format(input('Enter the prompt > '))
+                else:
+                    prompt = common.show_input(common.APP_ID, 'Enter the prompt')
+                    prompt = prompt_format.format(prompt=prompt) if prompt is not None else ''
+                output_name = datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")
+                output_name = f"{output_name}.txt"
+                yield 'prompt', convert.str2b64str(prompt), output_name
+        except KeyboardInterrupt:
+            self.logger.info("KeyboardInterrupt", exc_info=True)
+        finally:
+            pass
```

### Comparing `iinfer-0.7.3/iinfer/app/common.py` & `iinfer-0.7.4/iinfer/app/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import cv2
 import datetime
 import logging
 import logging.config
 import json
 import numpy as np
 import os
-import platform
+import multiprocessing
 import random
 import shutil
 import string
 import re
 import requests
 import subprocess
 import tempfile
@@ -112,15 +112,15 @@
     """
     if preval is not None:
         v = preval
         if isinstance(preval, dict):
             v = preval.get(key, None)
         if (v is None or not v) and key in opt:
             v = opt[key]
-        elif v is None or not v:
+        elif (v is None or not v) and v != 0:
             v = defval
         if withset:
             opt[key] = v
         return v
     if key in opt:
         return opt[key]
     else:
@@ -287,17 +287,17 @@
     output = None
     while proc.returncode is None:
         out = proc.stdout.readline()
         if out == b'' and proc.poll() is not None:
             break
         for enc in ['utf-8', 'cp932', 'utf-16', 'utf-16-le', 'utf-16-be']:
             try:
-                output = out.decode(enc)
-                if platform.system() == 'Windows' or strip:
-                    output = output.rstrip()
+                output = out.decode(enc).rstrip()
+                #if platform.system() == 'Windows' or strip:
+                #    output = output.rstrip()
                 logger.debug(f"output:{output}")
                 break
             except UnicodeDecodeError:
                 pass
 
     return proc.returncode, output
 
@@ -377,8 +377,35 @@
 
     return image, output_labels
 
 def make_color(idstr:str) -> Tuple[int]:
     if len(idstr) < 3:
         idstr = idstr.zfill(3)
     return tuple([ord(c) * ord(c) % 256 for c in idstr[:3]])
-    
+
+def show_input(title:str, message:str) -> str:
+    """
+    ダイアログで入力を求めます。
+
+    Args:
+        title (str): タイトル
+        message (str): メッセージ
+
+    Returns:
+        str: 入力された文字列
+    """
+    manager = multiprocessing.Manager()
+    result = manager.dict()
+    proc = multiprocessing.Process(target=_show_input_daialog, args=(title, message, result))
+    proc.start()
+    proc.join()
+    return result['input_text']
+
+def _show_input_daialog(title:str, message:str, result) -> str:
+    import wx
+    app = wx.App()
+    dlg = wx.TextEntryDialog(None, message, title)
+    dlg.ShowModal()
+    dlg.Destroy()
+    input_text = dlg.GetValue()
+    app.Destroy()
+    result['input_text'] = input_text
```

### Comparing `iinfer-0.7.3/iinfer/app/commons/convert.py` & `iinfer-0.7.4/iinfer/app/commons/convert.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/commons/module.py` & `iinfer-0.7.4/iinfer/app/commons/module.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from iinfer.app import common, predict, injection
 from pathlib import Path
-from typing import List, Dict, Any
+from typing import List, Dict, Any, Tuple
 import importlib.util
 import inspect
 import iinfer
 import logging
 import pkgutil
-
-import iinfer.app
-import iinfer.app.predict
+import iinfer
 
 
 def load_custom_predict(custom_predict_py:Path, logger:logging.Logger) -> predict.Predict:
     """
     カスタム予測オブジェクトを読み込みます。
 
     Args:
@@ -29,14 +27,28 @@
     module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(module)
     for name, obj in inspect.getmembers(module):
         if inspect.isclass(obj) and issubclass(obj, predict.Predict):
             return obj(logger)
     raise BaseException(f"Predict class not found.({custom_predict_py})")
 
+def build_predict(predict_type:str, custom_predict_file:str, logger:logging.Logger) -> Tuple[bool, predict.Predict]:
+    if predict_type == 'Custom':
+        custom_predict_py = Path(custom_predict_file) if custom_predict_file is not None else None
+        if custom_predict_py is None:
+            logger.warn(f"predict_type is Custom but custom_predict_py is None.")
+            return False, {"warn": f"predict_type is Custom but custom_predict_py is None."}
+        if not custom_predict_py.exists():
+            logger.warn(f"custom_predict_py path {str(custom_predict_py)} does not exist")
+            return False, {"warn": f"custom_predict_py path {str(custom_predict_py)} does not exist"}
+        predict_obj = load_custom_predict(custom_predict_py, logger)
+    else:
+        predict_obj = load_predict(predict_type, logger)
+    return True, predict_obj
+
 def load_predict(predict_type:str, logger:logging.Logger) -> predict.Predict:
     """
     指定された予測オブジェクトを読み込みます。
 
     Args:
         predict_type (str): 予測オブジェクトのモジュール名
         logger (logging.Logger): ロガー
```

### Comparing `iinfer-0.7.3/iinfer/app/gui.py` & `iinfer-0.7.4/iinfer/app/gui.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/injection.py` & `iinfer-0.7.4/iinfer/app/injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/injections/after_cls_jadge_injection.py` & `iinfer-0.7.4/iinfer/app/injections/after_cls_jadge_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/injections/after_csv_injection.py` & `iinfer-0.7.4/iinfer/app/injections/after_csv_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/injections/after_det_filter_injection.py` & `iinfer-0.7.4/iinfer/app/injections/after_det_filter_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/injections/after_det_jadge_injection.py` & `iinfer-0.7.4/iinfer/app/injections/after_det_jadge_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/injections/after_http_injection.py` & `iinfer-0.7.4/iinfer/app/injections/after_http_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/injections/after_seg_bbox_injection.py` & `iinfer-0.7.4/iinfer/app/injections/after_seg_bbox_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/injections/after_seg_filter_injection.py` & `iinfer-0.7.4/iinfer/app/injections/after_seg_filter_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/injections/before_grayimg_injection.py` & `iinfer-0.7.4/iinfer/app/injections/before_grayimg_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/install.py` & `iinfer-0.7.4/iinfer/app/install.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             return {"success": f"Success to install redis-server."}
 
         else:
             return {"warn":f"Unsupported platform."}
 
     def server(self, data:Path, install_iinfer:str='iinfer', install_onnx:bool=True,
                install_mmdet:bool=True, install_mmseg:bool=True, install_mmcls:bool=False, install_mmpretrain:bool=True,
-               install_insightface=False, install_diffusers=True,
+               install_insightface=False, install_diffusers=True, install_llamaindex=True,
                install_tag:str=None, install_use_gpu:bool=False):
         if platform.system() == 'Windows':
             return {"warn": f"Build server command is Unsupported in windows platform."}
         from importlib.resources import read_text
         user = getpass.getuser()
         install_tag = f"_{install_tag}" if install_tag is not None else ''
         with open('Dockerfile', 'w', encoding='utf-8') as fp:
@@ -52,26 +52,31 @@
             if wheel.exists() and wheel.suffix == '.whl':
                 shutil.copy(wheel, Path('.').resolve() / wheel.name)
                 install_iinfer = f'/home/{user}/{wheel.name}'
                 text = text.replace('#{COPY_IINFER}', f'COPY {wheel.name} {install_iinfer}')
             else:
                 text = text.replace('#{COPY_IINFER}', '')
             install_use_gpu = '--install_use_gpu' if install_use_gpu else ''
-            text = text.replace('#{FROM}', f'FROM nvidia/cuda:11.8.0-cudnn8-runtime-ubuntu20.04' if install_use_gpu else f'FROM python:3.8.18-slim')
+            base_image = 'python:3.11.9-slim' #'python:3.8.18-slim'
+            if install_use_gpu:
+                base_image = 'nvidia/cuda:12.4.1-cudnn-runtime-ubuntu22.04' if install_llamaindex else 'nvidia/cuda:11.8.0-cudnn8-runtime-ubuntu22.04'
+            text = text.replace('#{FROM}', f'FROM {base_image}')
             text = text.replace('${MKUSER}', user)
-            text = text.replace('#{INSTALL_PYTHON}', f'RUN apt-get update && apt-get install -y python3.8 python3.8-distutils python3-pip python-is-python3' if install_use_gpu else '')
+            #text = text.replace('#{INSTALL_PYTHON}', f'RUN apt-get update && apt-get install -y python3.8 python3.8-distutils python3-pip python-is-python3' if install_use_gpu else '')
+            text = text.replace('#{INSTALL_PYTHON}', f'RUN apt-get update && apt-get install -y python3.11 python3.11-distutils python3-pip python-is-python3' if install_use_gpu else '')
             text = text.replace('#{INSTALL_TAG}', install_tag)
             text = text.replace('#{INSTALL_IINFER}', install_iinfer)
             text = text.replace('#{INSTALL_ONNX}', f'RUN iinfer -m install -c onnx --data /home/{user}/.iinfer {install_use_gpu}' if install_onnx else '')
             text = text.replace('#{INSTALL_MMDET}', f'RUN iinfer -m install -c mmdet --data /home/{user}/.iinfer {install_use_gpu}' if install_mmdet else '')
             text = text.replace('#{INSTALL_MMSEG}', f'RUN iinfer -m install -c mmseg --data /home/{user}/.iinfer {install_use_gpu}' if install_mmseg else '')
             text = text.replace('#{INSTALL_MMCLS}', f'RUN iinfer -m install -c mmcls --data /home/{user}/.iinfer {install_use_gpu}' if install_mmcls else '')
             text = text.replace('#{INSTALL_MMPRETRAIN}', f'RUN iinfer -m install -c mmpretrain --data /home/{user}/.iinfer {install_use_gpu}' if install_mmpretrain else '')
             text = text.replace('#{INSTALL_INSIGHTFACE}', f'RUN iinfer -m install -c insightface --data /home/{user}/.iinfer {install_use_gpu}' if install_insightface else '')
             text = text.replace('#{INSTALL_DIFFUSERS}', f'RUN iinfer -m install -c diffusers --data /home/{user}/.iinfer {install_use_gpu}' if install_diffusers else '')
+            text = text.replace('#{INSTALL_LLAMAINDEX}', f'RUN iinfer -m install -c llamaindex --data /home/{user}/.iinfer {install_use_gpu}' if install_llamaindex else '')
             fp.write(text)
         docker_compose_path = Path('docker-compose.yml')
         if not docker_compose_path.exists():
             with open(docker_compose_path, 'w', encoding='utf-8') as fp:
                 text = read_text(f'{common.APP_ID}.docker', 'docker-compose.yml')
                 fp.write(text)
         with open(f'docker-compose.yml', 'r+', encoding='utf-8') as fp:
@@ -106,15 +111,15 @@
             )
             fp.seek(0)
             yaml.dump(comp, fp)
         cmd = f'docker build -t hamacom/iinfer:{version.__version__}{install_tag} -f Dockerfile .'
 
         if platform.system() == 'Linux':
             returncode, _ = common.cmd(f"{cmd}", self.logger, True)
-            os.remove('Dockerfile')
+            #os.remove('Dockerfile')
             if returncode != 0:
                 self.logger.error(f"Failed to install iinfer-server.")
                 return {"error": f"Failed to install iinfer-server."}
             return {"success": f"Success to install iinfer-server. and docker-compose.yml is copied."}
 
         else:
             return {"warn":f"Unsupported platform."}
@@ -146,21 +151,21 @@
         if returncode != 0:
             self.logger.error(f"Failed to install insightface.")
             return {"error": f"Failed to install insightface."}
         return {"success": f"Success to install insightface."}
 
     def _torch(self, install_use_gpu:bool=False):
         if install_use_gpu:
-            returncode, _ = common.cmd('pip install torch==2.1.0 torchvision --index-url https://download.pytorch.org/whl/cu118', logger=self.logger)
+            returncode, _ = common.cmd('pip install torch==2.1.0 torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118', logger=self.logger)
         else:
-            returncode, _ = common.cmd('pip install torch==2.1.0 torchvision', logger=self.logger)
+            returncode, _ = common.cmd('pip install torch==2.1.0 torchvision torchaudio', logger=self.logger)
         if returncode != 0:
-            self.logger.error(f"Failed to install torch.")
-            return {"error": f"Failed to install torch."}
-        return {"success": f"Success to install torch."}
+            self.logger.error(f"Failed to install torch torchvision torchaudio.")
+            return {"error": f"Failed to install torch torchvision torchaudio."}
+        return {"success": f"Success to install torch torchvision torchaudio."}
 
     def _openmin(self, install_use_gpu:bool=False):
         returncode, _ = common.cmd('pip install openmim', logger=self.logger)
         if returncode != 0:
             self.logger.error(f"Failed to install openmim.")
             return {"error": f"Failed to install openmim."}
         return {"success": f"Success to install openmim."}
@@ -175,19 +180,19 @@
             returncode, _ = common.cmd('mim install mmcv>=2.0.0', logger=self.logger)
         if returncode != 0:
             self.logger.error(f"Failed to install mmcv.")
             return {"error": f"Failed to install mmcv."}
         return {"success": f"Success to install mmcv."}
 
     def _transformers(self, install_use_gpu:bool=False):
-        returncode, _ = common.cmd('pip install accelerate transformers', logger=self.logger)
+        returncode, _ = common.cmd('pip install accelerate transformers bitsandbytes sentence-transformers', logger=self.logger)
         if returncode != 0:
-            self.logger.error(f"Failed to install accelerate transformers.")
-            return {"error": f"Failed to install accelerate transformers."}
-        return {"success": f"Success to install accelerate transformers."}
+            self.logger.error(f"Failed to install accelerate transformers bitsandbytes sentence-transformers.")
+            return {"error": f"Failed to install accelerate transformers bitsandbytes sentence-transformers."}
+        return {"success": f"Success to install accelerate transformers bitsandbytes sentence-transformers."}
 
     def mmdet(self, data_dir:Path, install_use_gpu:bool=False):
         returncode, _ = common.cmd(f'git clone https://github.com/open-mmlab/mmdetection.git', logger=self.logger)
         if returncode != 0:
             self.logger.error(f"Failed to git clone mmdetection.")
             return {"error": f"Failed to git clone mmdetection."}
         srcdir = Path('.') / 'mmdetection'
@@ -294,7 +299,25 @@
 
         ret, _ = common.cmd('pip install diffusers', logger=self.logger)
         if ret != 0:
             self.logger.error(f"Failed to install diffusers.")
             return {"error": f"Failed to install diffusers."}
 
         return {"success": f"Success to install diffusers."}
+
+    def llamaindex(self, data_dir:Path, install_use_gpu:bool=False):
+        ret = self._torch(install_use_gpu)
+        if "error" in ret: return ret
+        ret = self._transformers(install_use_gpu)
+        if "error" in ret: return ret
+
+        if install_use_gpu and platform.system() == 'Linux':
+            returncode, _ = common.cmd('apt-get install -y nvidia-cuda-toolkit', logger=self.logger)
+            returncode, _ = common.cmd('rm -rf /usr/lib/x86_64-linux-gnu/libnvidia-ml.so.1 /usr/lib/x86_64-linux-gnu/libcuda.so.1 /usr/lib/x86_64-linux-gnu/libcudadebugger.so.1', logger=self.logger)
+            returncode, _ = common.cmd('pip install llama_index llama-index-llms-huggingface llama-index-embeddings-huggingface', logger=self.logger)
+        else:
+            # llama-cpp-python
+            returncode, _ = common.cmd('pip install llama_index llama-index-llms-huggingface llama-index-embeddings-huggingface', logger=self.logger)
+        if returncode != 0:
+            self.logger.error(f"Failed to install llama_index llama-index-llms-huggingface llama-index-embeddings-huggingface.")
+            return {"error": f"Failed to install llama_index llama-index-llms-huggingface llama-index-embeddings-huggingface."}
+        return {"success": f"Success to install llama_index llama-index-llms-huggingface llama-index-embeddings-huggingface."}
```

### Comparing `iinfer-0.7.3/iinfer/app/options.py` & `iinfer-0.7.4/iinfer/app/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 from iinfer.app import common
+from iinfer.app.commons import module
+import argparse
+import os
 
 
 class Options:
     def __init__(self):
         self._options = dict()
         self.init_options()
 
@@ -20,36 +23,83 @@
     def get_opt_opt(self, mode, cmd):
         if mode not in self._options["cmd"]:
             return [f'Unknown mode. ({mode})']
         if cmd is None or cmd == "" or cmd not in self._options["cmd"][mode]:
             return []
         return self._options["cmd"][mode][cmd]["choise"]
 
+    def list_options(self):
+        def _list(ret, key, val):
+            if type(val) == dict:
+                opt = dict()
+                if val['type'] == 'int':
+                    opt['type'] = int
+                    opt['action'] = 'append' if val['multi'] else None
+                elif val['type'] == 'float':
+                    opt['type'] = float
+                    opt['action'] = 'append' if val['multi'] else None
+                elif val['type'] == 'bool':
+                    opt['type'] = None
+                    opt['action'] = 'store_true'
+                else:
+                    opt['type'] = str
+                    opt['action'] = 'append' if val['multi'] else None
+                o = [f'-{val["short"]}'] if "short" in val else []
+                o += [f'--{key}']
+                opt['help'] = val['discription_en']
+                opt['default'] = val['default']
+                opt['opts'] = o
+                if val['choise'] is not None:
+                    opt['choices'] = []
+                    for c in val['choise']:
+                        if type(c) == dict:
+                            opt['choices'] += [c['opt']]
+                        elif c is not None and c != "":
+                            opt['choices'] += [c]
+                else:
+                    opt['choices'] = None
+                ret[key] = opt
+        ret = dict()
+        for k, v in self._options.items():
+            _list(ret, k, v)
+        for mode in self._options["mode"]['choise']:
+            for c, cmd in mode.items():
+                if type(cmd) is not dict:
+                    continue
+                for opt in cmd["choise"]:
+                    if type(opt) is not dict:
+                        continue
+                    _list(ret, opt['opt'], opt)
+        return ret
+
     def init_options(self):
+        default_host = os.environ.get('REDIS_HOST', 'localhost')
+        default_port = int(os.environ.get('REDIS_PORT', '6379'))
+        default_pass = os.environ.get('REDIS_PASSWORD', 'password')
         self._options = dict()
+        self._options["version"] = dict(
+            short="v", type="bool", default=None, required=False, multi=False, hide=True,
+            discription_ja="バージョン表示",
+            discription_en="Display version",
+            choise=None)
         self._options["useopt"] = dict(
             short="u", type="str", default=None, required=False, multi=False, hide=True,
             discription_ja="オプションを保存しているファイルを使用します。",
             discription_en="Use the file that saves the options.",
             choise=None)
         self._options["saveopt"] = dict(
-            short="s", type="str", default=None, required=False, multi=False, hide=True,
+            short="s", type="bool", default=None, required=False, multi=False, hide=True,
             discription_ja="指定しているオプションを `-u` で指定したファイルに保存します。",
             discription_en="Save the specified options to the file specified by `-u`.",
-            choise=None)
+            choise=[True, False])
         self._options["format"] = dict(
-            short="f", type="str", default=None, required=False, multi=False, hide=True,
+            short="f", type="bool", default=None, required=False, multi=False, hide=True,
             discription_ja="処理結果を見やすい形式で出力します。指定しない場合json形式で出力します。",
             discription_en="Output the processing result in an easy-to-read format. If not specified, output in json format.",
             choise=None)
-        self._options["version"] = dict(
-            short="v", type="bool", default=None, required=False, multi=False, hide=True,
-            discription_ja="バージョン表示",
-            discription_en="Display version",
-            choise=None)
         self._options["mode"] = dict(
             short="m", type="str", default=None, required=True, multi=False, hide=True,
             discription_ja="起動モードを指定します。",
             discription_en="Specify the startup mode.",
             choise=[])
         self._options["cmd"] = dict(
             short="c", type="str", default=None, required=True, multi=False, hide=True,
@@ -60,21 +110,21 @@
                 discription_ja="クライアントモード",
                 discription_en="Client mode",
                 deploy=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="AIモデルをサーバーに配備します。",
                     discription_en="Deploy AI model to server.",
                     choise=[
-                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="host", type="str", default=default_host, required=True, multi=False, hide=True, choise=None,
                             discription_ja="Redisサーバーのサービスホストを指定します。",
                             discription_en="Specify the service host of the Redis server."),
-                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None,
+                        dict(opt="port", type="int", default=default_port, required=True, multi=False, hide=True, choise=None,
                             discription_ja="Redisサーバーのサービスポートを指定します。",
                             discription_en="Specify the service port of the Redis server."),
-                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="password", type="str", default=default_pass, required=True, multi=False, hide=True, choise=None,
                             discription_ja="Redisサーバーのアクセスパスワード(任意)を指定します。省略時は `password` を使用します。",
                             discription_en="Specify the access password of the Redis server (optional). If omitted, `password` is used."),
                         dict(opt="svname", type="str", default="server", required=True, multi=False, hide=True, choise=None,
                             discription_ja="推論サーバーのサービス名を指定します。省略時は `server` を使用します。",
                             discription_en="Specify the service name of the inference server. If omitted, `server` is used."),
                         dict(short="n", opt="name", type="str", default="", required=True, multi=False, hide=False, choise=None,
                             discription_ja="AIモデルの登録名を指定します。",
@@ -88,15 +138,15 @@
                         dict(opt="model_img_width", type="int", default="", required=False, multi=False, hide=True, choise=None,
                             discription_ja="AIモデルのINPUTサイズ(横px)を指定します。",
                             discription_en="Specify the INPUT size (width px) of the AI model."),
                         dict(opt="model_img_height", type="int", default="", required=False, multi=False, hide=True, choise=None,
                             discription_ja="AIモデルのINPUTサイズ(縦px)を指定します。",
                             discription_en="Specify the INPUT size (height px) of the AI model."),
                         dict(opt="predict_type", type="str", default="", required=False, multi=False, hide=False,
-                            choise=['']+[key for key in common.BASE_MODELS.keys()],
+                            choise=['','Custom']+[key for key in common.BASE_MODELS.keys()],
                             discription_ja="AIモデルの推論タイプを指定します。",
                             discription_en="Specify the inference type of the AI model."),
                         dict(opt="custom_predict_py", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="in",
                             discription_ja="独自の推論タイプを作成するときに指定。この時は `--predict_type Custom` を指定。",
                             discription_en="Specify when creating a custom inference type. In this case, specify `--predict_type Custom`."),
                         dict(opt="label_file", type="file", default="", required=False, multi=False, hide=False, choise=None, fileio="in",
                             discription_ja="推論結果のクラスラベルファイルを指定。改行区切りでラベル名(行indexがクラスと一致する)を指定したファイル。",
@@ -143,33 +193,33 @@
                     ]
                 ),
                 deploy_list=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="サーバーに配備されているAIモデル一覧を取得します。",
                     discription_en="Get a list of AI models deployed on the server.",
                     choise=[
-                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="host", type="str", default=default_host, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスホストを指定します。",
                              discription_en="Specify the service host of the Redis server."),
-                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None,
+                        dict(opt="port", type="int", default=default_port, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスポートを指定します。",
                              discription_en="Specify the service port of the Redis server."),
-                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="password", type="str", default=default_pass, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのアクセスパスワード(任意)を指定します。省略時は `password` を使用します。",
                             discription_en="Specify the access password of the Redis server (optional). If omitted, `password` is used."),
                         dict(opt="svname", type="str", default="server", required=True, multi=False, hide=True, choise=None,
                              discription_ja="推論サーバーのサービス名を指定します。省略時は `server` を使用します。",
                              discription_en="Specify the service name of the inference server. If omitted, `server` is used."),
                         dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None,
                              discription_ja="サーバーの応答が返ってくるまでの最大待ち時間を指定。",
                              discription_en="Specify the maximum waiting time until the server responds."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o" , type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a" , type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -177,36 +227,36 @@
                     ]
                 ),
                 undeploy=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="サーバーに配備されているAIモデルを削除します。",
                     discription_en="Delete AI models deployed on the server.",
                     choise=[
-                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="host", type="str", default=default_host, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスホストを指定します。",
                              discription_en="Specify the service host of the Redis server."),
-                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None,
+                        dict(opt="port", type="int", default=default_port, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスポートを指定します。",
                              discription_en="Specify the service port of the Redis server."),
-                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="password", type="str", default=default_pass, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのアクセスパスワード(任意)を指定します。省略時は `password` を使用します。",
                              discription_en="Specify the access password of the Redis server (optional). If omitted, `password` is used."),
                         dict(opt="svname", type="str", default="server", required=True, multi=False, hide=True, choise=None,
                              discription_ja="推論サーバーのサービス名を指定します。省略時は `server` を使用します。",
                              discription_en="Specify the service name of the inference server. If omitted, `server` is used."),
                         dict(short="n", opt="name", type="str", default="", required=True, multi=False, hide=False, choise=None,
                              discription_ja="削除するAIモデルの登録名を指定します。",
                              discription_en="Specify the registration name of the AI model to be deleted."),
                         dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None,
                              discription_ja="サーバーの応答が返ってくるまでの最大待ち時間を指定。",
                              discription_en="Specify the maximum waiting time until the server responds."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o" , type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a" , type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -214,46 +264,46 @@
                     ]
                 ),
                 start=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="AIモデルを指定して推論サーバーを起動します。",
                     discription_en="Start the inference server by specifying the AI model.",
                     choise=[
-                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="host", type="str", default=default_host, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスホストを指定します。",
                              discription_en="Specify the service host of the Redis server."),
-                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None,
+                        dict(opt="port", type="int", default=default_port, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスポートを指定します。",
                              discription_en="Specify the service port of the Redis server."),
-                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="password", type="str", default=default_pass, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのアクセスパスワード(任意)を指定します。省略時は `password` を使用します。",
                              discription_en="Specify the access password of the Redis server (optional). If omitted, `password` is used."),
                         dict(opt="svname", type="str", default="server", required=True, multi=False, hide=True, choise=None,
                              discription_ja="推論サーバーのサービス名を指定します。省略時は `server` を使用します。",
                              discription_en="Specify the service name of the inference server. If omitted, `server` is used."),
                         dict(short="n", opt="name", type="str", default="", required=True, multi=False, hide=False, choise=None,
                              discription_ja="削除するAIモデルの登録名を指定します。",
                              discription_en="Specify the registration name of the AI model to be deleted."),
                         dict(opt="model_provider", type="str", default="CPUExecutionProvider", required=False, multi=False, hide=True,
                              choise=['CPUExecutionProvider', 'CUDAExecutionProvider', 'TensorrtExecutionProvider'],
                              discription_ja="ONNX形式のモデルファイルの場合に指定可能。",
                              discription_en="Specify when the model file is in ONNX format."),
-                        dict(opt="use_track", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False],
+                        dict(short="T", opt="use_track", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False],
                              discription_ja="ObjectDetectionタスクの場合に指定可能。motpyを使ってトラッキングID付与を行う。",
                              discription_en="Specify when the task is ObjectDetection. Assign a tracking ID using motpy."),
                         dict(opt="gpuid", type="str", default="", required=False, multi=False, hide=False, choise=None,
                              discription_ja="GPUのディバイスIDを指定します。",
                              discription_en="Specify the device ID of the GPU."),
                         dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None,
                              discription_ja="サーバーの応答が返ってくるまでの最大待ち時間を指定。",
                              discription_en="Specify the maximum waiting time until the server responds."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o" , type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a" , type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -261,18 +311,18 @@
                     ]
                 ),
                 predict_type_list=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="推論タイプ一覧を取得します。",
                     discription_en="Get a list of inference types.",
                     choise=[
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o" , type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a" , type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -280,36 +330,36 @@
                     ]
                 ),
                 stop=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="AIモデルを指定して推論サーバーを停止します。",
                     discription_en="Stop the inference server by specifying the AI model.",
                     choise=[
-                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="host", type="str", default=default_host, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスホストを指定します。",
                              discription_en="Specify the service host of the Redis server."),
-                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None,
+                        dict(opt="port", type="int", default=default_port, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスポートを指定します。",
                              discription_en="Specify the service port of the Redis server."),
-                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="password", type="str", default=default_pass, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのアクセスパスワード(任意)を指定します。省略時は `password` を使用します。",
                              discription_en="Specify the access password of the Redis server (optional). If omitted, `password` is used."),
                         dict(opt="svname", type="str", default="server", required=True, multi=False, hide=True, choise=None,
                              discription_ja="推論サーバーのサービス名を指定します。省略時は `server` を使用します。",
                              discription_en="Specify the service name of the inference server. If omitted, `server` is used."),
                         dict(short="n", opt="name", type="str", default="", required=True, multi=False, hide=False, choise=None,
                              discription_ja="削除するAIモデルの登録名を指定します。",
                              discription_en="Specify the registration name of the AI model to be deleted."),
                         dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None,
                              discription_ja="サーバーの応答が返ってくるまでの最大待ち時間を指定。",
                              discription_en="Specify the maximum waiting time until the server responds."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o" , type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a" , type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -317,21 +367,21 @@
                     ]
                 ),
                 predict=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="AIモデルを指定して推論を実行します。",
                     discription_en="Perform inference by specifying the AI model.",
                     choise=[
-                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="host", type="str", default=default_host, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスホストを指定します。",
                              discription_en="Specify the service host of the Redis server."),
-                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None,
+                        dict(opt="port", type="int", default=default_port, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスポートを指定します。",
                              discription_en="Specify the service port of the Redis server."),
-                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="password", type="str", default=default_pass, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのアクセスパスワード(任意)を指定します。省略時は `password` を使用します。",
                              discription_en="Specify the access password of the Redis server (optional). If omitted, `password` is used."),
                         dict(opt="svname", type="str", default="server", required=True, multi=False, hide=True, choise=None,
                              discription_ja="推論サーバーのサービス名を指定します。省略時は `server` を使用します。",
                              discription_en="Specify the service name of the inference server. If omitted, `server` is used."),
                         dict(short="n", opt="name", type="str", default="", required=True, multi=False, hide=False, choise=None,
                              discription_ja="削除するAIモデルの登録名を指定します。",
@@ -341,31 +391,31 @@
                              discription_en="Specify the image to be inferred by file."),
                         dict(opt="stdin", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False],
                              discription_ja="推論させる画像を標準入力から読み込む。",
                              discription_en="Read the image to be inferred from standard input."),
                         dict(opt="nodraw", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False],
                              discription_ja="推論結果画像にbbox等の描き込みを行わない。",
                              discription_en="Do not draw bboxes etc. on the inference result image."),
-                        dict(opt="image_type", type="str", default="jpeg", required=True, multi=False, hide=False,
-                             choise=['bmp', 'png', 'jpeg', 'capture', 'output_json'],
-                             discription_ja="推論させる画像のタイプを指定します。",
-                             discription_en="Specify the type of image to be inferred."),
+                        dict(opt="pred_input_type", type="str", default="jpeg", required=True, multi=False, hide=False,
+                             choise=['bmp', 'png', 'jpeg', 'capture', 'output_json', 'prompt'],
+                             discription_ja="推論させる入力タイプを指定します。",
+                             discription_en="Specifies the input type to be inferred."),
                         dict(opt="output_image", type="file", default="", required=False, multi=False, hide=False, choise=None, fileio="out",
                              discription_ja="推論結果画像の保存先ファイルを指定します。",
                              discription_en="Specify the destination file for saving the inference result image."),
                         dict(short="P", opt="output_preview", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False],
                              discription_ja="推論結果画像を `cv2.imshow` で表示します。",
                              discription_en="Display the inference result image with `cv2.imshow`."),
                         dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None,
                              discription_ja="サーバーの応答が返ってくるまでの最大待ち時間を指定。",
                              discription_en="Specify the maximum waiting time until the server responds."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o" , type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a" , type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -373,19 +423,19 @@
                     ]
                 ),
                 capture=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="クライアント側でキャプチャー画像を取得します。",
                     discription_en="Get a capture image on the client side.",
                     choise=[
-                        dict(opt="capture_device", type="str", default="0", required=True, multi=False, hide=True, choise=None,
+                        dict(short="d", opt="capture_device", type="str", default="0", required=True, multi=False, hide=True, choise=None,
                              discription_ja="キャプチャーディバイスを指定します。 `cv2.VideoCapture` の第一引数に渡される値。",
                              discription_en="Specify the capture device. The value passed to the first argument of `cv2.VideoCapture`."),
                         dict(opt="image_type", type="str", default="capture", required=True, multi=False, hide=False, choise=['bmp', 'png', 'jpeg', 'capture'],
-                             discription_ja="キ出力する画像のタイプを指定します。",
+                             discription_ja="出力する画像のタイプを指定します。",
                              discription_en="Specify the type of image to output."),
                         dict(opt="capture_frame_width", type="int", default=640, required=False, multi=False, hide=True, choise=None,
                              discription_ja="キャプチャーする画像の横px。 `cv2.VideoCapture` オブジェクトの `cv2.CAP_PROP_FRAME_WIDTH` オプションに指定する値。",
                              discription_en="Width px of the image to be captured. The value to be specified in the `cv2.CAP_PROP_FRAME_WIDTH` option of the `cv2.VideoCapture` object."),
                         dict(opt="capture_frame_height", type="int", default=480, required=False, multi=False, hide=True, choise=None,
                              discription_ja="キャプチャーする画像の縦px。 `cv2.VideoCapture` オブジェクトの `cv2.CAP_PROP_FRAME_HEIGHT` オプションに指定する値。",
                              discription_en="Height px of the image to be captured. The value to be specified in the `cv2.CAP_PROP_FRAME_HEIGHT` option of the `cv2.VideoCapture` object."),
@@ -395,51 +445,76 @@
                         dict(opt="capture_count", type="int", default=5, required=False, multi=False, hide=False, choise=None,
                              discription_ja="キャプチャーする回数。",
                              discription_en="Number of captures."),
                         dict(opt="output_preview", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False],
                              discription_ja="推論結果画像を `cv2.imshow` で表示します。",
                              discription_en="Display the inference result image with `cv2.imshow`."),
                         dict(opt="output_csv", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
-                             discription_ja="キャプチャーした内容をcsvで保存します。これを指定した場合、標準出力は行いません。",
-                             discription_en="Save the captured content in csv. If this is specified, no standard output will be performed."),
+                             discription_ja="入力した内容をcsvで保存します。これを指定した場合、標準出力は行いません。",
+                             discription_en="Saves the input as a csv file. If this is specified, no standard output is performed."),
+                        dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
+                             discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
+                             discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
+                        dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
+                             discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
+                             discription_en="Available only in GUI mode. Captures standard output during command execution and displays it on the execution result screen."),
+                    ]
+                ),
+                prompt=dict(
+                    type="str", default=None, required=False, multi=False, hide=False,
+                    discription_ja="LLM向けに単にキー入力したものを標準出力します。",
+                    discription_en="Standard output of simply keyed input for LLM.",
+                    choise=[
+                        dict(opt="prompt_format", type="str", default="{prompt}", required=False, multi=False, hide=False, choise=None,
+                             discription_ja="入力をフォーマットするときの書式を指定します。",
+                             discription_en="Specifies the format in which the input is formatted."),
+                        dict(opt="prompt_count", type="int", default=1, required=False, multi=False, hide=False, choise=None,
+                             discription_ja="プロンプトでキー入力する回数。",
+                             discription_en="Number of keystrokes at the prompt."),
+                        dict(opt="prompt_form", type="bool", default=True, required=False, multi=False, hide=False, choise=[True, False],
+                             discription_ja="プロンプト入力フォームを表示します。",
+                             discription_en="Displays prompt input form."),
+                        dict(opt="output_csv", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                             discription_ja="入力した内容をcsvで保存します。これを指定した場合、標準出力は行いません。",
+                             discription_en="Saves the input as a csv file. If this is specified, no standard output is performed."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
                              discription_en="Available only in GUI mode. Captures standard output during command execution and displays it on the execution result screen."),
                     ]
                 ),
                 file_list=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="サーバー側のデータフォルダ配下のファイルリストを取得します。",
                     discription_en="Get a list of files under the data folder on the server.",
                     choise=[
-                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="host", type="str", default=default_host, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスホストを指定します。",
                              discription_en="Specify the service host of the Redis server."),
-                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None,
+                        dict(opt="port", type="int", default=default_port, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスポートを指定します。",
                              discription_en="Specify the service port of the Redis server."),
-                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="password", type="str", default=default_pass, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのアクセスパスワード(任意)を指定します。省略時は `password` を使用します。",
                              discription_en="Specify the access password of the Redis server (optional). If omitted, `password` is used."),
                         dict(opt="svname", type="str", default="server", required=True, multi=False, hide=True, choise=None,
                              discription_ja="推論サーバーのサービス名を指定します。省略時は `server` を使用します。",
                              discription_en="Specify the service name of the inference server. If omitted, `server` is used."),
                         dict(opt="svpath", type="str", default="/", required=True, multi=False, hide=False, choise=None,
                              discription_ja="推論サーバーのデータフォルダ以下のパスを指定します。省略時は `/` を使用します。",
                              discription_en="Specify the directory path to get the list of files."),
                         dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None,
                              discription_ja="サーバーの応答が返ってくるまでの最大待ち時間を指定。",
                              discription_en="Specify the maximum waiting time until the server responds."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -447,36 +522,36 @@
                     ]
                 ),
                 file_mkdir=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="サーバー側のデータフォルダ配下に新しいフォルダを作成します。",
                     discription_en="Create a new folder under the data folder on the server.",
                     choise=[
-                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="host", type="str", default=default_host, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスホストを指定します。",
                              discription_en="Specify the service host of the Redis server."),
-                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None,
+                        dict(opt="port", type="int", default=default_port, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスポートを指定します。",
                              discription_en="Specify the service port of the Redis server."),
-                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="password", type="str", default=default_pass, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのアクセスパスワード(任意)を指定します。省略時は `password` を使用します。",
                              discription_en="Specify the access password of the Redis server (optional). If omitted, `password` is used."),
                         dict(opt="svname", type="str", default="server", required=True, multi=False, hide=True, choise=None,
                              discription_ja="推論サーバーのサービス名を指定します。省略時は `server` を使用します。",
                              discription_en="Specify the service name of the inference server. If omitted, `server` is used."),
                         dict(opt="svpath", type="str", default="/", required=True, multi=False, hide=False, choise=None,
                              discription_ja="推論サーバーのデータフォルダ以下のパスを指定します。省略時は `/` を使用します。",
                              discription_en="Specify the directory path to get the list of files."),
                         dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None,
                              discription_ja="サーバーの応答が返ってくるまでの最大待ち時間を指定。",
                              discription_en="Specify the maximum waiting time until the server responds."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -484,36 +559,36 @@
                     ]
                 ),
                 file_rmdir=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="サーバー側のデータフォルダ配下のフォルダを削除します。",
                     discription_en="Delete a folder under the data folder on the server.",
                     choise=[
-                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="host", type="str", default=default_host, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスホストを指定します。",
                              discription_en="Specify the service host of the Redis server."),
-                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None,
+                        dict(opt="port", type="int", default=default_port, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスポートを指定します。",
                              discription_en="Specify the service port of the Redis server."),
-                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="password", type="str", default=default_pass, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのアクセスパスワード(任意)を指定します。省略時は `password` を使用します。",
                              discription_en="Specify the access password of the Redis server (optional). If omitted, `password` is used."),
                         dict(opt="svname", type="str", default="server", required=True, multi=False, hide=True, choise=None,
                              discription_ja="推論サーバーのサービス名を指定します。省略時は `server` を使用します。",
                              discription_en="Specify the service name of the inference server. If omitted, `server` is used."),
                         dict(opt="svpath", type="str", default="/", required=True, multi=False, hide=False, choise=None,
                              discription_ja="推論サーバーのデータフォルダ以下のパスを指定します。",
                              discription_en="Specify the directory path to get the list of files."),
                         dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None,
                              discription_ja="サーバーの応答が返ってくるまでの最大待ち時間を指定。",
                              discription_en="Specify the maximum waiting time until the server responds."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -521,39 +596,39 @@
                     ]
                 ),
                 file_download=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="サーバー側のデータフォルダ配下のファイルをダウンロードします。",
                     discription_en="Download a file under the data folder on the server.",
                     choise=[
-                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="host", type="str", default=default_host, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスホストを指定します。",
                              discription_en="Specify the service host of the Redis server."),
-                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None,
+                        dict(opt="port", type="int", default=default_port, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスポートを指定します。",
                              discription_en="Specify the service port of the Redis server."),
-                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="password", type="str", default=default_pass, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのアクセスパスワード(任意)を指定します。省略時は `password` を使用します。",
                              discription_en="Specify the access password of the Redis server (optional). If omitted, `password` is used."),
                         dict(opt="svname", type="str", default="server", required=True, multi=False, hide=True, choise=None,
                              discription_ja="推論サーバーのサービス名を指定します。省略時は `server` を使用します。",
                              discription_en="Specify the service name of the inference server. If omitted, `server` is used."),
                         dict(opt="svpath", type="str", default="/", required=True, multi=False, hide=False, choise=None,
                              discription_ja="推論サーバーのデータフォルダ以下のパスを指定します。",
                              discription_en="Specify the directory path to get the list of files."),
                         dict(opt="download_file", type="file", default="", required=False, multi=False, hide=False, choise=None, fileio="out",
                              discription_ja="クライアントの保存先パスを指定します。",
                              discription_en="Specify the destination path of the client."),
                         dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None,
                              discription_ja="サーバーの応答が返ってくるまでの最大待ち時間を指定。",
                              discription_en="Specify the maximum waiting time until the server responds."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -561,39 +636,39 @@
                     ]
                 ),
                 file_upload=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="サーバー側のデータフォルダ配下にファイルをアップロードします。",
                     discription_en="Upload a file under the data folder on the server.",
                     choise=[
-                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="host", type="str", default=default_host, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスホストを指定します。",
                              discription_en="Specify the service host of the Redis server."),
-                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None,
+                        dict(opt="port", type="int", default=default_port, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスポートを指定します。",
                              discription_en="Specify the service port of the Redis server."),
-                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="password", type="str", default=default_pass, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのアクセスパスワード(任意)を指定します。省略時は `password` を使用します。",
                              discription_en="Specify the access password of the Redis server (optional). If omitted, `password` is used."),
                         dict(opt="svname", type="str", default="server", required=True, multi=False, hide=True, choise=None,
                              discription_ja="推論サーバーのサービス名を指定します。省略時は `server` を使用します。",
                              discription_en="Specify the service name of the inference server. If omitted, `server` is used."),
                         dict(opt="svpath", type="str", default="/", required=True, multi=False, hide=False, choise=None,
                              discription_ja="推論サーバーのデータフォルダ以下のパスを指定します。",
                              discription_en="Specify the directory path to get the list of files."),
                         dict(opt="upload_file", type="file", default="", required=False, multi=False, hide=False, choise=None, fileio="out",
                              discription_ja="クライアントのアップロード元パスを指定します。",
                              discription_en="Specify the source path of the client."),
                         dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None,
                              discription_ja="サーバーの応答が返ってくるまでの最大待ち時間を指定。",
                              discription_en="Specify the maximum waiting time until the server responds."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -601,36 +676,36 @@
                     ]
                 ),
                 file_remove=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="サーバー側のデータフォルダ配下のファイルを削除します。",
                     discription_en="Delete a file under the data folder on the server.",
                     choise=[
-                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="host", type="str", default=default_host, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスホストを指定します。",
                              discription_en="Specify the service host of the Redis server."),
-                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None,
+                        dict(opt="port", type="int", default=default_port, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスポートを指定します。",
                              discription_en="Specify the service port of the Redis server."),
-                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="password", type="str", default=default_pass, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのアクセスパスワード(任意)を指定します。省略時は `password` を使用します。",
                              discription_en="Specify the access password of the Redis server (optional). If omitted, `password` is used."),
                         dict(opt="svname", type="str", default="server", required=True, multi=False, hide=True, choise=None,
                              discription_ja="推論サーバーのサービス名を指定します。省略時は `server` を使用します。",
                              discription_en="Specify the service name of the inference server. If omitted, `server` is used."),
                         dict(opt="svpath", type="str", default="/", required=True, multi=False, hide=False, choise=None,
                              discription_ja="推論サーバーのデータフォルダ以下のパスを指定します。",
                              discription_en="Specify the directory path to get the list of files."),
                         dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None,
                              discription_ja="サーバーの応答が返ってくるまでの最大待ち時間を指定。",
                              discription_en="Specify the maximum waiting time until the server responds."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -684,18 +759,18 @@
                              discription_en="Do not draw bboxes, etc. on the inference result image."),
                         dict(short="P", opt="output_preview", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False],
                              discription_ja="判定結果画像を`cv2.imshow`で表示します。",
                              discription_en="Display the judgment result image with `cv2.imshow`."),
                         dict(opt="output_image", type="file", default="", required=False, multi=False, hide=False, choise=None, fileio="out",
                              discription_ja="後処理結果画像の保存先ファイルを指定します。",
                              discription_en="Specify the destination file for saving the post-processing result image."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -817,18 +892,18 @@
                              discription_en="Do not draw bboxes, etc. on the inference result image."),
                         dict(short="P", opt="output_preview", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False],
                              discription_ja="判定結果画像を`cv2.imshow`で表示します。",
                              discription_en="Display the judgment result image with `cv2.imshow`."),
                         dict(opt="output_image", type="file", default="", required=False, multi=False, hide=False, choise=None, fileio="out",
                              discription_ja="後処理結果画像の保存先ファイルを指定します。",
                              discription_en="Specify the destination file for saving the post-processing result image."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -878,18 +953,18 @@
                              discription_en="Do not draw bboxes, etc. on the inference result image."),
                         dict(short="P", opt="output_preview", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False],
                              discription_ja="判定結果画像を`cv2.imshow`で表示します。",
                              discription_en="Display the judgment result image with `cv2.imshow`."),
                         dict(opt="output_image", type="file", default="", required=False, multi=False, hide=False, choise=None, fileio="out",
                              discription_ja="後処理結果画像の保存先ファイルを指定します。",
                              discription_en="Specify the destination file for saving the post-processing result image."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -909,14 +984,17 @@
                              discription_en="Read the inference result to be post-processed from standard input."),
                         dict(opt="json_connectstr", type="str", default="", required=True, multi=False, hide=False, choise=None,
                              discription_ja="推論結果のJSONのPOST先URLを指定します。",
                              discription_en="Specify the POST destination URL of the JSON of the inference result."),
                         dict(opt="img_connectstr", type="str", default="", required=False, multi=False, hide=False, choise=None,
                              discription_ja="推論結果の画像のPOST先URLを指定します。",
                              discription_en="Specify the POST destination URL of the image of the inference result."),
+                        dict(opt="text_connectstr", type="str", default="", required=False, multi=False, hide=False, choise=None,
+                             discription_ja="推論結果のテキストのPOST先URLを指定します。",
+                             discription_en="Specify the POST destination URL of the text of the inference result."),
                         dict(opt="fileup_name", type="str", default="file", required=True, multi=False, hide=False, choise=None,
                              discription_ja="推論結果の画像をPOSTするときのパラメータ名を指定します。省略すると `file` が使用されます。",
                              discription_en="Specify the parameter name when posting the image of the inference result. If omitted, `file` is used."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
@@ -949,18 +1027,18 @@
                              discription_en="Do not draw rotated bboxes on the inference result image."),
                         dict(short="P", opt="output_preview", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False],
                              discription_ja="判定結果画像を`cv2.imshow`で表示します。",
                              discription_en="Display the judgment result image with `cv2.imshow`."),
                         dict(opt="output_image", type="file", default="", required=False, multi=False, hide=False, choise=None, fileio="out",
                              discription_ja="後処理結果画像の保存先ファイルを指定します。",
                              discription_en="Specify the destination file for saving the post-processing result image."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -998,18 +1076,18 @@
                              discription_en="Remove the segmentation score from the result. This reduces the result capacity."),
                         dict(short="P", opt="output_preview", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False],
                              discription_ja="判定結果画像を`cv2.imshow`で表示します。",
                              discription_en="Display the judgment result image with `cv2.imshow`."),
                         dict(opt="output_image", type="file", default="", required=False, multi=False, hide=False, choise=None, fileio="out",
                              discription_ja="後処理結果画像の保存先ファイルを指定します。",
                              discription_en="Specify the destination file for saving the post-processing result image."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -1021,33 +1099,33 @@
                 discription_ja="サーバーモード",
                 discription_en="Server mode",
                 start=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="推論サーバーを起動します。installモードで `iinfer -m install -c server` を実行している場合は、 `docker-compose up -d` を使用してください。",
                     discription_en="Start the inference server. If you are running `iinfer -m install -c server` in install mode, use `docker-compose up -d`.",
                     choise=[
-                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="host", type="str", default=default_host, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスホストを指定します。",
                              discription_en="Specify the service host of the Redis server."),
-                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None,
+                        dict(opt="port", type="int", default=default_port, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスポートを指定します。",
                              discription_en="Specify the service port of the Redis server."),
-                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="password", type="str", default=default_pass, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのアクセスパスワード(任意)を指定します。省略時は `password` を使用します。",
                              discription_en="Specify the access password of the Redis server (optional). If omitted, `password` is used."),
                         dict(opt="svname", type="str", default="server", required=True, multi=False, hide=True, choise=None,
                              discription_ja="推論サーバーのサービス名を指定します。省略時は `server` を使用します。",
                              discription_en="Specify the service name of the inference server. If omitted, `server` is used."),
-                        dict(opt="data", type="file", default=None, required=False, multi=False, hide=False, choise=None,
+                        dict(opt="data", type="file", default=common.HOME_DIR / '.iinfer', required=False, multi=False, hide=False, choise=None,
                              discription_ja="省略した時は `$HONE/.iinfer` を使用します。",
                              discription_en="When omitted, `$HONE/.iinfer` is used."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -1055,33 +1133,33 @@
                     ]
                 ),
                 stop=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="推論サーバーを停止します。installモードで `iinfer -m install -c server` を実行している場合は、 `docker-compose down` を使用してください。",
                     discription_en="Stop the inference server. If you are running `iinfer -m install -c server` in install mode, use `docker-compose down`.",
                     choise=[
-                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="host", type="str", default=default_host, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスホストを指定します。",
                              discription_en="Specify the service host of the Redis server."),
-                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None,
+                        dict(opt="port", type="int", default=default_port, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスポートを指定します。",
                              discription_en="Specify the service port of the Redis server."),
-                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="password", type="str", default=default_pass, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのアクセスパスワード(任意)を指定します。省略時は `password` を使用します。",
                              discription_en="Specify the access password of the Redis server (optional). If omitted, `password` is used."),
                         dict(opt="svname", type="str", default="server", required=True, multi=False, hide=True, choise=None,
                              discription_ja="推論サーバーのサービス名を指定します。省略時は `server` を使用します。",
                              discription_en="Specify the service name of the inference server. If omitted, `server` is used."),
                         dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None,
                              discription_ja="サーバーの応答が返ってくるまでの最大待ち時間を指定。",
                              discription_en="Specify the maximum waiting time until the server responds."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -1089,30 +1167,30 @@
                     ]
                 ),
                 list=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="起動中の推論サーバーの一覧を表示します。クライアント環境からの利用も可能です。",
                     discription_en="Displays a list of running inference servers. Can also be used from the client environment.",
                     choise=[
-                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="host", type="str", default=default_host, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスホストを指定します。",
                              discription_en="Specify the service host of the Redis server."),
-                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None,
+                        dict(opt="port", type="int", default=default_port, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスポートを指定します。",
                              discription_en="Specify the service port of the Redis server."),
-                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="password", type="str", default=default_pass, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのアクセスパスワード(任意)を指定します。省略時は `password` を使用します。",
                              discription_en="Specify the access password of the Redis server (optional). If omitted, `password` is used."),
                         dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None,
                              discription_ja="サーバーの応答が返ってくるまでの最大待ち時間を指定。",
                              discription_en="Specify the maximum waiting time until the server responds."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -1124,30 +1202,30 @@
                 discription_ja="Redisモード",
                 discription_en="Redis mode",
                 docker_run=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="installモードで `iinfer -m install -c server` を実行している場合は、 `docker-compose up -d` を使用してください。",
                     discription_en="If you are running `iinfer -m install -c server` in install mode, use `docker-compose up -d`.",
                     choise=[
-                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None,
+                        dict(opt="port", type="int", default=default_port, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスポートを指定します。",
                              discription_en="Specify the service port of the Redis server."),
-                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None,
+                        dict(opt="password", type="str", default=default_pass, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのアクセスパスワードを指定します。省略時は`password`を使用します。",
                              discription_en="Specify the access password of the Redis server. If omitted, `password` is used."),
                         dict(opt="wsl_name", type="str", default="", required=False, multi=False, hide=True, choise=None,
                              discription_ja="Windowsの場合はWSLのディストリビューションの名前を指定します。",
                              discription_en="For Windows, specify the name of the WSL distribution."),
                         dict(opt="wsl_user", type="str", default="ubuntu", required=False, multi=False, hide=True, choise=None,
                              discription_ja="Windowsの場合はWSL内のユーザー名を指定します。",
                              discription_en="For Windows, specify the user name in WSL."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -1161,18 +1239,18 @@
                     choise=[
                         dict(opt="wsl_name", type="str", default="", required=False, multi=False, hide=True, choise=None,
                              discription_ja="Windowsの場合はWSLのディストリビューションの名前を指定します。",
                              discription_en="For Windows, specify the name of the WSL distribution."),
                         dict(opt="wsl_user", type="str", default="ubuntu", required=False, multi=False, hide=True, choise=None,
                              discription_ja="Windowsの場合はWSL内のユーザー名を指定します。",
                              discription_en="For Windows, specify the user name in WSL."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -1184,18 +1262,18 @@
                 discription_ja="インストールモード",
                 discription_en="Install mode",
                 onnx=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="`onnxruntime` をインストールします。",
                     discription_en="Install `onnxruntime`.",
                     choise=[
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -1206,18 +1284,18 @@
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="`mmdetection` をインストールします。",
                     discription_en="Install `mmdetection`.",
                     choise=[
                         dict(opt="install_use_gpu", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False],
                              discription_ja="GPUを使用するモジュール構成でインストールします。",
                              discription_en="Install with a module configuration that uses the GPU."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -1228,18 +1306,18 @@
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="`mmsegmentation` をインストールします。",
                     discription_en="Install `mmsegmentation`.",
                     choise=[
                         dict(opt="install_use_gpu", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False],
                              discription_ja="GPUを使用するモジュール構成でインストールします。",
                              discription_en="Install with a module configuration that uses the GPU."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -1250,18 +1328,18 @@
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="`mmcls` をインストールします。",
                     discription_en="Install `mmcls`.",
                     choise=[
                         dict(opt="install_use_gpu", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False],
                              discription_ja="GPUを使用するモジュール構成でインストールします。",
                              discription_en="Install with a module configuration that uses the GPU."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -1272,18 +1350,84 @@
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="`mmpretrain` をインストールします。",
                     discription_en="Install `mmpretrain`.",
                     choise=[
                         dict(opt="install_use_gpu", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False],
                              discription_ja="GPUを使用するモジュール構成でインストールします。",
                              discription_en="Install with a module configuration that uses the GPU."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                             discription_ja="処理結果jsonファイルを追記保存します。",
+                             discription_en="Save the processing result json file by appending."),
+                        dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
+                             discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
+                             discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
+                        dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
+                             discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
+                             discription_en="Available only in GUI mode. Captures standard output during command execution and displays it on the execution result screen."),
+                    ]
+                ),
+                insightface=dict(
+                    type="str", default=None, required=False, multi=False, hide=False,
+                    discription_ja="`insightface` をインストールします。",
+                    discription_en="Install `insightface`.",
+                    choise=[
+                        dict(opt="install_use_gpu", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False],
+                             discription_ja="GPUを使用するモジュール構成でインストールします。",
+                             discription_en="Install with a module configuration that uses the GPU."),
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                             discription_ja="処理結果jsonの保存先ファイルを指定。",
+                             discription_en="Specify the destination file for saving the processing result json."),
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                             discription_ja="処理結果jsonファイルを追記保存します。",
+                             discription_en="Save the processing result json file by appending."),
+                        dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
+                             discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
+                             discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
+                        dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
+                             discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
+                             discription_en="Available only in GUI mode. Captures standard output during command execution and displays it on the execution result screen."),
+                    ]
+                ),
+                diffusers=dict(
+                    type="str", default=None, required=False, multi=False, hide=False,
+                    discription_ja="`diffusers` をインストールします。",
+                    discription_en="Install `diffusers`.",
+                    choise=[
+                        dict(opt="install_use_gpu", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False],
+                             discription_ja="GPUを使用するモジュール構成でインストールします。",
+                             discription_en="Install with a module configuration that uses the GPU."),
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                             discription_ja="処理結果jsonの保存先ファイルを指定。",
+                             discription_en="Specify the destination file for saving the processing result json."),
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                             discription_ja="処理結果jsonファイルを追記保存します。",
+                             discription_en="Save the processing result json file by appending."),
+                        dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
+                             discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
+                             discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
+                        dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
+                             discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
+                             discription_en="Available only in GUI mode. Captures standard output during command execution and displays it on the execution result screen."),
+                    ]
+                ),
+                llamaindex=dict(
+                    type="str", default=None, required=False, multi=False, hide=False,
+                    discription_ja="`llamaindex` をインストールします。",
+                    discription_en="Install `llamaindex`.",
+                    choise=[
+                        dict(opt="install_use_gpu", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False],
+                             discription_ja="GPUを使用するモジュール構成でインストールします。",
+                             discription_en="Install with a module configuration that uses the GPU."),
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                             discription_ja="処理結果jsonの保存先ファイルを指定。",
+                             discription_en="Specify the destination file for saving the processing result json."),
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -1297,18 +1441,18 @@
                     choise=[
                         dict(opt="wsl_name", type="str", default="", required=False, multi=False, hide=True, choise=None,
                              discription_ja="Windowsの場合はWSLのディストリビューションの名前を指定します。",
                              discription_en="For Windows, specify the name of the WSL distribution."),
                         dict(opt="wsl_user", type="str", default="ubuntu", required=False, multi=False, hide=True, choise=None,
                              discription_ja="Windowsの場合はWSL内のユーザー名を指定します。",
                              discription_en="For Windows, specify the user name in WSL."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -1316,48 +1460,54 @@
                     ]
                 ),
                 server=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="`推論サーバー` のdockerイメージを `build` します。`build` が成功すると、実行時ディレクトリに `docker-compose.yml` ファイルが生成されます。",
                     discription_en="`Build` the docker image of the `inference server`. If the `build` is successful, a `docker-compose.yml` file is generated in the execution directory.",
                     choise=[
-                        dict(opt="data", type="file", default=None, required=False, multi=False, hide=False, choise=None,
+                        dict(opt="data", type="file", default=common.HOME_DIR / '.iinfer', required=False, multi=False, hide=False, choise=None,
                              discription_ja="省略した時は `$HONE/.iinfer` を使用します。",
                              discription_en="When omitted, `$HONE/.iinfer` is used."),
                         dict(opt="install_iinfer", type="str", default='iinfer', required=False, multi=False, hide=True, choise=None,
                              discription_ja="省略した時は `iinfer` を使用します。 `iinfer==0.7.2` といった指定も可能です。",
                              discription_en="When omitted, `iinfer` is used. You can also specify `iinfer==0.7.2`."),
-                        dict(opt="install_onnx", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="install_onnx", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="dockerイメージ内に `onnxruntime` をインストールします。",
                              discription_en="Install `onnxruntime` in the docker image."),
-                        dict(opt="install_mmdet", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="install_mmdet", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="dockerイメージ内に `mmdetection` をインストールします。",
                              discription_en="Install `mmdetection` in the docker image."),
-                        dict(opt="install_mmseg", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="install_mmseg", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="dockerイメージ内に `mmsegmentation` をインストールします。",
                              discription_en="Install `mmsegmentation` in the docker image."),
-                        dict(opt="install_mmcls", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="install_mmcls", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="dockerイメージ内に `mmclassification` をインストールします。",
                              discription_en="Install `mmclassification` in the docker image."),
-                        dict(opt="install_mmpretrain", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="install_mmpretrain", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="dockerイメージ内に `mmpretrain` をインストールします。",
                              discription_en="Install `mmpretrain` in the docker image."),
-                        dict(opt="install_insightface", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="install_insightface", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="dockerイメージ内に `insightface` をインストールします。",
                              discription_en="Install `insightface` in the docker image."),
-                        dict(opt="install_tag", type="str", default=False, required=False, multi=False, hide=False, choise=None,
+                        dict(opt="install_diffusers", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                             discription_ja="dockerイメージ内に `diffusers` をインストールします。",
+                             discription_en="Install `diffusers` in the docker image."),
+                        dict(opt="install_llamaindex", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                             discription_ja="dockerイメージ内に `llamaindex` をインストールします。",
+                             discription_en="Install `llamaindex` in the docker image."),
+                        dict(opt="install_tag", type="str", default="", required=False, multi=False, hide=False, choise=None,
                              discription_ja="指定すると作成するdockerイメージのタグ名に追記出来ます。",
                              discription_en="If specified, you can add to the tag name of the docker image to create."),
                         dict(opt="install_use_gpu", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False],
                              discription_ja="GPUを使用するモジュール構成でインストールします。",
                              discription_en="Install with a module configuration that uses the GPU."),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
+                        dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
                              discription_en="Specify the destination file for saving the processing result json."),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
+                        dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="処理結果jsonファイルを追記保存します。",
                              discription_en="Save the processing result json file by appending."),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をConsole logに出力します。",
                              discription_en="Available only in GUI mode. Outputs standard output during command execution to Console log."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
@@ -1369,15 +1519,15 @@
                 discription_ja="Webモード",
                 discription_en="Web mode",
                 start=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="Webモードを起動します。",
                     discription_en="Start Web mode.",
                     choise=[
-                        dict(opt="data", type="file", default=None, required=False, multi=False, hide=False, choise=None,
+                        dict(opt="data", type="file", default=common.HOME_DIR / '.iinfer', required=False, multi=False, hide=False, choise=None,
                              discription_ja="省略した時は `$HONE/.iinfer` を使用します。",
                              discription_en="When omitted, `$HONE/.iinfer` is used."),
                         dict(opt="allow_host", type="str", default="0.0.0.0", required=False, multi=False, hide=False, choise=None,
                              discription_ja="省略した時は `0.0.0.0` を使用します。",
                              discription_en="If omitted, `0.0.0.0` is used."),
                         dict(opt="listen_port", type="int", default="8081", required=False, multi=False, hide=False, choise=None,
                              discription_ja="省略した時は `8081` を使用します。",
@@ -1388,24 +1538,43 @@
                     ]
                 ),
                 stop=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="Webモードを停止します。",
                     discription_en="Stop Web mode.",
                     choise=[
-                        dict(opt="data", type="file", default=None, required=False, multi=False, hide=False, choise=None,
+                        dict(opt="data", type="file", default=common.HOME_DIR / '.iinfer', required=False, multi=False, hide=False, choise=None,
                              discription_ja="省略した時は `$HONE/.iinfer` を使用します。",
                              discription_en="When omitted, `$HONE/.iinfer` is used."),
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
                              discription_en="Available only in GUI mode. Captures standard output during command execution and displays it on the execution result screen."),
                     ]
                 ),
+            ),
+            gui=dict(
+                discription_ja="GUIモード",
+                discription_en="GUI mode",
+                start=dict(
+                    type="str", default=None, required=False, multi=False, hide=False,
+                    discription_ja="GUIモードを起動します。",
+                    discription_en="Start GUI mode.",
+                    choise=[
+                        dict(opt="data", type="file", default=common.HOME_DIR / '.iinfer', required=False, multi=False, hide=False, choise=None,
+                             discription_ja="省略した時は `$HONE/.iinfer` を使用します。",
+                             discription_en="When omitted, `$HONE/.iinfer` is used."),
+                    ]
+                ),
             )
         )
         for key, mode in self._options["cmd"].items():
             if type(mode) is not dict:
                 continue
-            self._options["cmd"]["choise"] += [cmd for cmd in mode.keys()]
+            mode['opt'] = key
+            for k, c in mode.items():
+                if type(c) is not dict:
+                    continue
+                c["opt"] = k
+                self._options["cmd"]["choise"] += [c]
             self._options["mode"][key] = mode
             self._options["mode"]["choise"] += [mode]
```

### Comparing `iinfer-0.7.3/iinfer/app/postprocess.py` & `iinfer-0.7.4/iinfer/app/postprocess.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/postprocesses/cls_jadge.py` & `iinfer-0.7.4/iinfer/app/postprocesses/cls_jadge.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/postprocesses/csv.py` & `iinfer-0.7.4/iinfer/app/postprocesses/csv.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/postprocesses/det_clip.py` & `iinfer-0.7.4/iinfer/app/postprocesses/det_clip.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/postprocesses/det_face_store.py` & `iinfer-0.7.4/iinfer/app/postprocesses/det_face_store.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/postprocesses/det_filter.py` & `iinfer-0.7.4/iinfer/app/postprocesses/det_filter.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/postprocesses/det_jadge.py` & `iinfer-0.7.4/iinfer/app/postprocesses/det_jadge.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/postprocesses/httpreq.py` & `iinfer-0.7.4/iinfer/app/postprocesses/httpreq.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/postprocesses/seg_bbox.py` & `iinfer-0.7.4/iinfer/app/postprocesses/seg_bbox.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/postprocesses/seg_filter.py` & `iinfer-0.7.4/iinfer/app/postprocesses/seg_filter.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/predict.py` & `iinfer-0.7.4/iinfer/app/predict.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 from PIL import Image
-from typing import List, Tuple, Dict, Any
+from typing import List, Tuple, Dict, Any, Union
 import logging
 
 
 class Predict(object):
     def __init__(self, logger:logging.Logger) -> None:
         """
         このクラスのインスタンスを初期化します。
@@ -24,24 +24,36 @@
         Args:
             gpu_id (int, optional): GPU ID. Defaults to None.
         Returns:
             bool: GPUが利用可能かどうか
         """
         raise NotImplementedError()
 
-    def create_session(self, logger:logging.Logger, model_path:Path, model_conf_path:Path, model_provider:str, gpu_id:int=None) -> Any:
+    def post_deploy(self, deploy_dir:Path, conf:dict) -> None:
+        """
+        デプロイ後の処理を行う関数です。
+        deployコマンド実行時に呼び出されます。
+        この関数内でデプロイ後の処理を実装してください。
+        
+        Args:
+            deploy_dir (Path): デプロイディレクトリのパス
+            conf (dict): デプロイ設定
+        """
+        pass
+
+    def create_session(self, deploy_dir:Path, model_path:Union[Path|Any], model_conf_path:Path, model_provider:str, gpu_id:int=None) -> Any:
         """
         推論セッションを作成する関数です。
         startコマンド実行時に呼び出されます。
         この関数内でAIモデルのロードを行い、推論準備を完了するようにしてください。
         戻り値の推論セッションの型は問いません。
 
         Args:
-            logger (logging.Logger): ロガー
-            model_path (Path): モデルファイルのパス
+            deploy_dir (Path): デプロイディレクトリのパス
+            model_path (Path|Any): モデルファイルのパス
             model_conf_path (Path): モデル設定ファイルのパス
             gpu_id (int, optional): GPU ID. Defaults to None.
 
         Returns:
             推論セッション
         """
         raise NotImplementedError()
@@ -78,22 +90,22 @@
         継承時は、このコンストラクタを呼び出すようにしてください。
             super().__init__(logger)
         Args:
             logger (logging.Logger): ロガー
         """
         super().__init__(logger)
 
-    def is_gpu_available(self, model_path:Path, model_conf_path:Path, gpu_id:int=None) -> bool:
+    def is_gpu_available(self, model_path:Union[Path|Any], model_conf_path:Path, gpu_id:int=None) -> bool:
         """
         GPUが利用可能かどうかを返す関数です。
         戻り値がTrueの場合、GPUが利用可能です。
         戻り値がFalseの場合、GPUが利用不可です。
 
         Args:
-            model_path (Path): モデルファイルのパス
+            model_path (Path|Any): モデルファイルのパス
             model_conf_path (Path): モデル設定ファイルのパス
             gpu_id (int, optional): GPU ID. Defaults to None.
         Returns:
             bool: GPUが利用可能かどうか
         """
         try:
             import onnxruntime as rt
@@ -111,22 +123,22 @@
         継承時は、このコンストラクタを呼び出すようにしてください。
             super().__init__(logger)
         Args:
             logger (logging.Logger): ロガー
         """
         super().__init__(logger)
 
-    def is_gpu_available(self, model_path:Path, model_conf_path:Path, gpu_id:int=None) -> bool:
+    def is_gpu_available(self, model_path:Union[Path|Any], model_conf_path:Path, gpu_id:int=None) -> bool:
         """
         GPUが利用可能かどうかを返す関数です。
         戻り値がTrueの場合、GPUが利用可能です。
         戻り値がFalseの場合、GPUが利用不可です。
 
         Args:
-            model_path (Path): モデルファイルのパス
+            model_path (Path|Any): モデルファイルのパス
             model_conf_path (Path): モデル設定ファイルのパス
             gpu_id (int, optional): GPU ID. Defaults to None.
         Returns:
             bool: GPUが利用可能かどうか
         """
         try:
             import torch
```

### Comparing `iinfer-0.7.3/iinfer/app/predicts/diffusers_stablediffusion_txt2img.py` & `iinfer-0.7.4/iinfer/app/predicts/diffusers_stablediffusionpipeline_txt2img.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 from pathlib import Path
 from PIL import Image
 from iinfer.app import common, predict
 from iinfer.app.commons import convert
-from typing import List, Tuple
+from typing import List, Tuple, Union, Any
 import logging
 
 
 SITE = 'https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion/text2img'
 IMAGE_WIDTH = 640
 IMAGE_HEIGHT = 640
 REQUIREd_MODEL_CONF = False
 REQUIREd_MODEL_WEIGHT = False
 
-class Diffusers_StableDiffusion_Txt2Img(predict.TorchPredict):
+class Diffusers_StableDiffusionPipeline_Txt2Img(predict.TorchPredict):
     def __init__(self, logger:logging.Logger) -> None:
         super().__init__(logger)
 
-    def create_session(self, model_path:Path, model_conf_path:Path, model_provider:str, gpu_id:int=None):
+    def create_session(self, deploy_dir:Path, model_path:Union[Path|Any], model_conf_path:Path, model_provider:str, gpu_id:int=None):
         """
         推論セッションを作成する関数です。
         startコマンド実行時に呼び出されます。
         この関数内でAIモデルのロードを行い、推論準備を完了するようにしてください。
         戻り値の推論セッションの型は問いません。
 
         Args:
-            model_path (Path): モデルファイルのパス
+            deploy_dir (Path): デプロイディレクトリのパス
+            model_path (Path|Any): モデルファイルのパス
             model_conf_path (Path): モデル設定ファイルのパス
             gpu_id (int, optional): GPU ID. Defaults to None.
 
         Returns:
             推論セッション
         """
         from diffusers import StableDiffusionPipeline, DPMSolverMultistepScheduler
 
-        model_id = "KBlueLeaf/kohaku-v2.1"
-        pipeline = StableDiffusionPipeline.from_pretrained(model_id, cache_dir=model_conf_path.parent)
+        opt = common.loadopt(model_conf_path) if model_conf_path is not None else dict()
+        self.num_inference_steps = common.getopt(opt, 'num_inference_steps', preval=10, withset=False)
+
+        # KBlueLeaf/kohaku-v2.1
+        # SimianLuo/LCM_Dreamshaper_v7
+        pipeline = StableDiffusionPipeline.from_pretrained(model_path, cache_dir=deploy_dir)
         pipeline.scheduler = DPMSolverMultistepScheduler.from_config(pipeline.scheduler.config)
-        if gpu_id is not None:
+        if gpu_id is not None and self.is_gpu_available(model_path, model_conf_path, gpu_id):
             pipeline.to("cuda")
         return pipeline
 
-    def predict(self, model, img_width:int, img_height:int, image:Image.Image, labels:List[str]=None, colors:List[Tuple[int]]=None, nodraw:bool=False):
+    def predict(self, model, img_width:int, img_height:int, input_data:Union[Image.Image, str], labels:List[str]=None, colors:List[Tuple[int]]=None, nodraw:bool=False):
         """
         予測を行う関数です。
         predictコマンドやcaptureコマンド実行時に呼び出されます。
-        引数のimageはRGBですので、戻り値の出力画像もRGBにしてください。
+        引数のinput_dataが画像の場合RGBですので、戻り値の出力画像もRGBにしてください。
         戻り値の推論結果のdictは、通常推論結果項目ごとに値(list)を設定します。
-        例）Image Classification（EfficientNet_Lite4）の場合
-        return dict(output_scores=output_scores, output_classes=output_classes), image_obj
-        例）Object Detection（YoloX）の場合
-        return dict(output_boxes=final_boxes, output_scores=final_scores, output_classes=final_cls_inds), output_image
 
         Args:
             model: 推論セッション
-            img_width (int): モデルのINPUTサイズ（画像の幅）
-            img_height (int): モデルのINPUTサイズ（画像の高さ）
-            image (Image): 入力画像（RGB配列であること）
+            img_width (int): モデルのINPUTサイズ（input_dataが画像の場合は、画像の幅）
+            img_height (int): モデルのINPUTサイズ（input_dataが画像の場合は、画像の高さ）
+            input_data (Image | str): 推論するデータ（画像の場合RGB配列であること）
             labels (List[str], optional): クラスラベルのリスト. Defaults to None.
             colors (List[Tuple[int]], optional): ボックスの色のリスト. Defaults to None.
             nodraw (bool, optional): 描画フラグ. Defaults to False.
 
         Returns:
             Tuple[Dict[str, Any], Image]: 予測結果と出力画像(RGB)のタプル
         """
         import torch
-        prompt = "A Japanese woman is taking a shower while eating pizza."
-        output_images = model(prompt, height=img_height, width=img_width, num_inference_steps=5, output_type='pil',
+        output_images = model(input_data, height=img_height, width=img_width, num_inference_steps=self.num_inference_steps, output_type='pil',
                               torch_dtype=torch.float16).images
 
-        return dict(prompt=prompt), output_images[0]
+        return dict(prompt=input_data), output_images[0]
```

### Comparing `iinfer-0.7.3/iinfer/app/predicts/insightface_det.py` & `iinfer-0.7.4/iinfer/app/predicts/insightface_det.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from PIL import Image
 from iinfer.app import common, predict
 from iinfer.app.commons import convert
-from typing import List, Tuple
+from typing import List, Tuple, Union, Any
 import json
 import logging
 import numpy as np
 import shutil
 
 
 SITE = 'https://github.com/deepinsight/insightface/tree/master/python-package'
@@ -15,31 +15,33 @@
 REQUIREd_MODEL_CONF = False
 REQUIREd_MODEL_WEIGHT = True
 
 class InsightfaceDet(predict.OnnxPredict):
     def __init__(self, logger:logging.Logger) -> None:
         super().__init__(logger)
 
-    def create_session(self, model_path:Path, model_conf_path:Path, model_provider:str, gpu_id:int=None):
+    def create_session(self, deploy_dir:Path, model_path:Union[Path|Any], model_conf_path:Path, model_provider:str, gpu_id:int=None):
         """
         推論セッションを作成する関数です。
         startコマンド実行時に呼び出されます。
         この関数内でAIモデルのロードを行い、推論準備を完了するようにしてください。
         戻り値の推論セッションの型は問いません。
 
         Args:
-            model_path (Path): モデルファイルのパス
+            deploy_dir (Path): デプロイディレクトリのパス
+            model_path (Path|Any): モデルファイルのパス
             model_conf_path (Path): モデル設定ファイルのパス
             gpu_id (int, optional): GPU ID. Defaults to None.
 
         Returns:
             推論セッション
         """
         from insightface.app import FaceAnalysis
-        model_dir = model_path.parent / 'models'
+        model_path = Path(model_path)
+        model_dir = deploy_dir / 'models'
         if not model_dir.exists():
             common.mkdirs(model_dir)
             shutil.unpack_archive(model_path, model_dir)
         fa = FaceAnalysis(name=model_path.stem, root=model_path.parent, providers=[model_provider])
         self.input_width = IMAGE_WIDTH
         self.input_height = IMAGE_HEIGHT
         fa.prepare(ctx_id=0, det_size=(self.input_height, self.input_width))
@@ -61,44 +63,40 @@
                             raise Exception('Invalid outputs. line[\'success\'][i][\'face_embedding_shape\'] must be set.')
 
                         face_store.append(dict(face_label=data['face_label'],
                                                face_embedding=convert.b64str2npy(data['face_embedding'], shape=data['face_embedding_shape'], dtype=data['face_embedding_dtype'])))
 
         return dict(fa=fa, face_store=face_store, face_threshold=0.0)
 
-    def predict(self, model, img_width:int, img_height:int, image:Image.Image, labels:List[str]=None, colors:List[Tuple[int]]=None, nodraw:bool=False):
+    def predict(self, model, img_width:int, img_height:int, input_data:Union[Image.Image, str], labels:List[str]=None, colors:List[Tuple[int]]=None, nodraw:bool=False):
         """
         予測を行う関数です。
         predictコマンドやcaptureコマンド実行時に呼び出されます。
-        引数のimageはRGBですので、戻り値の出力画像もRGBにしてください。
+        引数のinput_dataが画像の場合RGBですので、戻り値の出力画像もRGBにしてください。
         戻り値の推論結果のdictは、通常推論結果項目ごとに値(list)を設定します。
-        例）Image Classification（EfficientNet_Lite4）の場合
-        return dict(output_scores=output_scores, output_classes=output_classes), image_obj
-        例）Object Detection（YoloX）の場合
-        return dict(output_boxes=final_boxes, output_scores=final_scores, output_classes=final_cls_inds), output_image
 
         Args:
             model: 推論セッション
-            img_width (int): モデルのINPUTサイズ（画像の幅）
-            img_height (int): モデルのINPUTサイズ（画像の高さ）
-            image (Image): 入力画像（RGB配列であること）
+            img_width (int): モデルのINPUTサイズ（input_dataが画像の場合は、画像の幅）
+            img_height (int): モデルのINPUTサイズ（input_dataが画像の場合は、画像の高さ）
+            input_data (Image | str): 推論するデータ（画像の場合RGB配列であること）
             labels (List[str], optional): クラスラベルのリスト. Defaults to None.
             colors (List[Tuple[int]], optional): ボックスの色のリスト. Defaults to None.
             nodraw (bool, optional): 描画フラグ. Defaults to False.
 
         Returns:
             Tuple[Dict[str, Any], Image]: 予測結果と出力画像(RGB)のタプル
         """
         if img_width != self.input_width or img_height != self.input_height:
             self.input_width = img_width
             self.input_height = img_height
             model['fa'].prepare(ctx_id=0, det_size=(self.input_height, self.input_width))
 
         # RGB画像をBGR画像に変換
-        img_npy = convert.img2npy(image)
+        img_npy = convert.img2npy(input_data)
         img_npy = convert.bgr2rgb(img_npy)
 
         # 顔検知
         face_store = model['face_store']
         face_threshold = model['face_threshold']
         faces = model['fa'].get(img_npy)
         boxes = []
@@ -119,15 +117,15 @@
             scores.append(score)
             ids.append(i)
             clses.append(0)
             if store_index >= 0:
                 labels.append(face_store[store_index]['face_label'])
             else:
                 labels.append(None)
-        output_image, output_labels = common.draw_boxes(image, boxes, scores, clses, ids=ids, labels=labels, colors=colors, nodraw=nodraw)
+        output_image, output_labels = common.draw_boxes(input_data, boxes, scores, clses, ids=ids, labels=labels, colors=colors, nodraw=nodraw)
 
         return dict(output_ids=ids, output_scores=scores, output_classes=clses, output_labels=output_labels, output_boxes=boxes,
                     output_embeddings=embeddings, output_embedding_dtypes=embedding_dtypes, output_embedding_shapes=embedding_shapes), output_image
 
     def search_face(self, store:list, face_embedding:np.array, th:float):
         last_score = -1
         index = -1
```

### Comparing `iinfer-0.7.3/iinfer/app/predicts/mmdet_det_YoloX.py` & `iinfer-0.7.4/iinfer/app/predicts/mmdet_det_YoloX.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,77 @@
 from pathlib import Path
 from PIL import Image
 from iinfer.app import common, predict
 from iinfer.app.commons import convert
-from typing import List, Tuple
+from typing import List, Tuple, Union, Any
 import logging
 
 
 SITE = 'https://github.com/open-mmlab/mmdetection/tree/main/configs/yolox'
 IMAGE_WIDTH = 640
 IMAGE_HEIGHT = 640
 REQUIREd_MODEL_CONF = True
 REQUIREd_MODEL_WEIGHT = False
 
 class MMDetYoloX(predict.TorchPredict):
     def __init__(self, logger:logging.Logger) -> None:
         super().__init__(logger)
 
-    def create_session(self, model_path:Path, model_conf_path:Path, model_provider:str, gpu_id:int=None):
+    def create_session(self, deploy_dir:Path, model_path:Union[Path|Any], model_conf_path:Path, model_provider:str, gpu_id:int=None):
         """
         推論セッションを作成する関数です。
         startコマンド実行時に呼び出されます。
         この関数内でAIモデルのロードを行い、推論準備を完了するようにしてください。
         戻り値の推論セッションの型は問いません。
 
         Args:
-            model_path (Path): モデルファイルのパス
+            deploy_dir (Path): デプロイディレクトリのパス
+            model_path (Path|Any): モデルファイルのパス
             model_conf_path (Path): モデル設定ファイルのパス
             gpu_id (int, optional): GPU ID. Defaults to None.
 
         Returns:
             推論セッション
         """
         from mmdet.apis import init_detector
         import torch
         gpu = f'cuda:{gpu_id}' if gpu_id is not None else 'cuda'
         device = torch.device(gpu if self.is_gpu_available(model_path, model_conf_path, gpu_id) else 'cpu')
         model = init_detector(model_conf_path, str(model_path), device=device) # , cfg_options = {'show': True}
         return model
 
-    def predict(self, model, img_width:int, img_height:int, image:Image.Image, labels:List[str]=None, colors:List[Tuple[int]]=None, nodraw:bool=False):
+    def predict(self, model, img_width:int, img_height:int, input_data:Union[Image.Image, str], labels:List[str]=None, colors:List[Tuple[int]]=None, nodraw:bool=False):
         """
         予測を行う関数です。
         predictコマンドやcaptureコマンド実行時に呼び出されます。
-        引数のimageはRGBですので、戻り値の出力画像もRGBにしてください。
+        引数のinput_dataが画像の場合RGBですので、戻り値の出力画像もRGBにしてください。
         戻り値の推論結果のdictは、通常推論結果項目ごとに値(list)を設定します。
-        例）Image Classification（EfficientNet_Lite4）の場合
-        return dict(output_scores=output_scores, output_classes=output_classes), image_obj
-        例）Object Detection（YoloX）の場合
-        return dict(output_boxes=final_boxes, output_scores=final_scores, output_classes=final_cls_inds), output_image
 
         Args:
             model: 推論セッション
-            img_width (int): モデルのINPUTサイズ（画像の幅）
-            img_height (int): モデルのINPUTサイズ（画像の高さ）
-            image (Image): 入力画像（RGB配列であること）
+            img_width (int): モデルのINPUTサイズ（input_dataが画像の場合は、画像の幅）
+            img_height (int): モデルのINPUTサイズ（input_dataが画像の場合は、画像の高さ）
+            input_data (Image | str): 推論するデータ（画像の場合RGB配列であること）
             labels (List[str], optional): クラスラベルのリスト. Defaults to None.
             colors (List[Tuple[int]], optional): ボックスの色のリスト. Defaults to None.
             nodraw (bool, optional): 描画フラグ. Defaults to False.
 
         Returns:
             Tuple[Dict[str, Any], Image]: 予測結果と出力画像(RGB)のタプル
         """
         # RGB画像をBGR画像に変換
-        img_npy = convert.img2npy(image)
+        img_npy = convert.img2npy(input_data)
         img_npy = convert.bgr2rgb(img_npy)
 
         #input_shape = (img_width, img_height)
         #img, ratio = self.preprocess(img_npy, input_shape)
 
         #output = session.run(None, {session.get_inputs()[0].name: img[None, :, :, :]})
         from mmdet.apis import inference_detector
         result = inference_detector(model, img_npy)
         boxes = result.pred_instances.bboxes.cpu().numpy().tolist()
         boxes = [[row[1],row[0],row[3],row[2]] for row in boxes]
         ids = [i for i in range(len(boxes))]
         scores = result.pred_instances.scores.cpu().numpy().tolist()
         clses = result.pred_instances.labels.cpu().numpy().tolist()
-        output_image, output_labels = common.draw_boxes(image, boxes, scores, clses, ids=ids, labels=labels, colors=colors, nodraw=nodraw)
+        output_image, output_labels = common.draw_boxes(input_data, boxes, scores, clses, ids=ids, labels=labels, colors=colors, nodraw=nodraw)
         return dict(output_ids=ids, output_scores=scores, output_classes=clses, output_labels=output_labels, output_boxes=boxes), output_image
```

### Comparing `iinfer-0.7.3/iinfer/app/predicts/mmpretrain_cls_swin.py` & `iinfer-0.7.4/iinfer/app/predicts/mmpretrain_cls_swin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,81 +1,78 @@
 from iinfer.app import predict
 from iinfer.app.commons import convert
 from pathlib import Path
 from PIL import Image
-from typing import List, Tuple
+from typing import List, Tuple, Any, Union
 import logging
 import numpy as np
 
 SITE = 'https://github.com/open-mmlab/mmpretrain/tree/master/configs/swin_transformer'
 IMAGE_WIDTH = 384
 IMAGE_HEIGHT = 384
 REQUIREd_MODEL_CONF = True
 REQUIREd_MODEL_WEIGHT = False
 
 class MMPretrainClsSwin(predict.TorchPredict):
     def __init__(self, logger:logging.Logger) -> None:
         super().__init__(logger)
 
-    def create_session(self, model_path:Path, model_conf_path:Path, model_provider:str, gpu_id:int=None):
+    def create_session(self, deploy_dir:Path, model_path:Union[Path|Any], model_conf_path:Path, model_provider:str, gpu_id:int=None):
         """
         推論セッションを作成する関数です。
         startコマンド実行時に呼び出されます。
         この関数内でAIモデルのロードを行い、推論準備を完了するようにしてください。
         戻り値の推論セッションの型は問いません。
 
         Args:
-            model_path (Path): モデルファイルのパス
+            deploy_dir (Path): デプロイディレクトリのパス
+            model_path (Path|Any): モデルファイルのパス
             model_conf_path (Path): モデル設定ファイルのパス
             gpu_id (int, optional): GPU ID. Defaults to None.
 
         Returns:
             推論セッション
         """
-        self.deploy_dir = model_path.parent
+        self.deploy_dir = deploy_dir
         import torch
         import mmpretrain
         gpu = f'cuda:{gpu_id}' if gpu_id is not None else 'cuda'
         device = torch.device(gpu if self.is_gpu_available(model_path, model_conf_path, gpu_id) else 'cpu')
         session = mmpretrain.ImageClassificationInferencer(str(model_conf_path), pretrained=str(model_path), device=device)
         return session
 
-    def predict(self, session, img_width:int, img_height:int, image:Image.Image, labels:List[str]=None, colors:List[Tuple[int]]=None, nodraw:bool=False):
+    def predict(self, model, img_width:int, img_height:int, input_data:Union[Image.Image, str], labels:List[str]=None, colors:List[Tuple[int]]=None, nodraw:bool=False):
         """
         予測を行う関数です。
         predictコマンドやcaptureコマンド実行時に呼び出されます。
-        引数のimageはRGBですので、戻り値の出力画像もRGBにしてください。
+        引数のinput_dataが画像の場合RGBですので、戻り値の出力画像もRGBにしてください。
         戻り値の推論結果のdictは、通常推論結果項目ごとに値(list)を設定します。
-        例）Image Classification（EfficientNet_Lite4）の場合
-        return dict(output_scores=output_scores, output_classes=output_classes), image_obj
-        例）Object Detection（YoloX）の場合
-        return dict(output_boxes=final_boxes, output_scores=final_scores, output_classes=final_cls_inds), output_image
 
         Args:
-            session: 推論セッション
-            img_width (int): モデルのINPUTサイズ（画像の幅）
-            img_height (int): モデルのINPUTサイズ（画像の高さ）
-            image (Image): 入力画像（RGB配列であること）
+            model: 推論セッション
+            img_width (int): モデルのINPUTサイズ（input_dataが画像の場合は、画像の幅）
+            img_height (int): モデルのINPUTサイズ（input_dataが画像の場合は、画像の高さ）
+            input_data (Image | str): 推論するデータ（画像の場合RGB配列であること）
             labels (List[str], optional): クラスラベルのリスト. Defaults to None.
             colors (List[Tuple[int]], optional): ボックスの色のリスト. Defaults to None.
             nodraw (bool, optional): 描画フラグ. Defaults to False.
 
         Returns:
             Tuple[Dict[str, Any], Image]: 予測結果と出力画像(RGB)のタプル
         """
         import mmpretrain
         # RGB画像をBGR画像に変換
-        img_npy = convert.img2npy(image)
+        img_npy = convert.img2npy(input_data)
         img_npy = convert.bgr2rgb(img_npy)
 
-        image_data, _, image_obj = self.preprocess_img(image, img_width, img_height)
+        image_data, _, image_obj = self.preprocess_img(input_data, img_width, img_height)
 
         with open(self.deploy_dir / 'tmp.png', 'wb') as fp:
             fp.write(convert.img2byte(image_obj,format='PNG'))
-            result = session(self.deploy_dir / 'tmp.png')[0]
+            result = model(self.deploy_dir / 'tmp.png')[0]
 
         output_scores = result["pred_scores"]
         output_classes = result["pred_class"]
 
         return dict(output_scores=output_scores, output_classes=output_classes), image_obj
 
     def resize_img(self, image:Image.Image, to_w, to_h):
```

### Comparing `iinfer-0.7.3/iinfer/app/predicts/mmrotate_det_ReDet.py` & `iinfer-0.7.4/iinfer/app/predicts/onnx_det_YoloX.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,109 +1,96 @@
 from pathlib import Path
 from PIL import Image
 from iinfer.app import common, predict
 from iinfer.app.commons import convert
-from typing import List, Tuple
+from typing import List, Tuple, Union
 import cv2
 import logging
 import numpy as np
 
 
-SITE = 'https://github.com/open-mmlab/mmrotate/tree/main/configs/redet'
-IMAGE_WIDTH = 1024
-IMAGE_HEIGHT = 1024
-REQUIREd_MODEL_CONF = True
-REQUIREd_MODEL_WEIGHT = False
+SITE = 'https://github.com/Megvii-BaseDetection/YOLOX/'
+IMAGE_WIDTH = 640
+IMAGE_HEIGHT = 640
+REQUIREd_MODEL_CONF = False
+REQUIREd_MODEL_WEIGHT = True
 
-class MMRotateReDet(predict.TorchPredict):
+class OnnxDetYoloX(predict.OnnxPredict):
     def __init__(self, logger:logging.Logger) -> None:
         super().__init__(logger)
 
-    def create_session(self, model_path:Path, model_conf_path:Path, model_provider:str, gpu_id:int=None):
+    def create_session(self, deploy_dir:Path, model_path:Path, model_conf_path:Path, model_provider:str, gpu_id:int=None):
         """
         推論セッションを作成する関数です。
         startコマンド実行時に呼び出されます。
         この関数内でAIモデルのロードを行い、推論準備を完了するようにしてください。
         戻り値の推論セッションの型は問いません。
 
         Args:
+            deploy_dir (Path): デプロイディレクトリのパス
             model_path (Path): モデルファイルのパス
             model_conf_path (Path): モデル設定ファイルのパス
             gpu_id (int, optional): GPU ID. Defaults to None.
 
         Returns:
             推論セッション
         """
-        from mmdet.apis import init_detector
-        import mmrotate
-        import torch
-        gpu = f'cuda:{gpu_id}' if gpu_id is not None else 'gpu'
-        device = torch.device(gpu if self.is_gpu_available(model_path, model_conf_path, gpu_id) else 'cpu')
-        model = init_detector(model_conf_path, str(model_path), device=device) # , cfg_options = {'show': True}
-        return model
+        import onnxruntime as rt
+        if self.is_gpu_available(model_path, model_conf_path, gpu_id):
+            session = rt.InferenceSession(model_path, providers=[model_provider])
+        else:
+            session = rt.InferenceSession(model_path, providers=[model_provider], providers_options=[{'device_id': str(gpu_id)}])
+        return session
 
-    def predict(self, model, img_width:int, img_height:int, image:Image.Image, labels:List[str]=None, colors:List[Tuple[int]]=None, nodraw:bool=False):
+    def predict(self, model, img_width:int, img_height:int, input_data:Union[Image.Image, str], labels:List[str]=None, colors:List[Tuple[int]]=None, nodraw:bool=False):
         """
         予測を行う関数です。
         predictコマンドやcaptureコマンド実行時に呼び出されます。
-        引数のimageはRGBですので、戻り値の出力画像もRGBにしてください。
+        引数のinput_dataが画像の場合RGBですので、戻り値の出力画像もRGBにしてください。
         戻り値の推論結果のdictは、通常推論結果項目ごとに値(list)を設定します。
-        例）Image Classification（EfficientNet_Lite4）の場合
-        return dict(output_scores=output_scores, output_classes=output_classes), image_obj
-        例）Object Detection（YoloX）の場合
-        return dict(output_boxes=final_boxes, output_scores=final_scores, output_classes=final_cls_inds), output_image
 
         Args:
             model: 推論セッション
-            img_width (int): モデルのINPUTサイズ（画像の幅）
-            img_height (int): モデルのINPUTサイズ（画像の高さ）
-            image (Image): 入力画像（RGB配列であること）
+            img_width (int): モデルのINPUTサイズ（input_dataが画像の場合は、画像の幅）
+            img_height (int): モデルのINPUTサイズ（input_dataが画像の場合は、画像の高さ）
+            input_data (Image | str): 推論するデータ（画像の場合RGB配列であること）
             labels (List[str], optional): クラスラベルのリスト. Defaults to None.
             colors (List[Tuple[int]], optional): ボックスの色のリスト. Defaults to None.
             nodraw (bool, optional): 描画フラグ. Defaults to False.
 
         Returns:
             Tuple[Dict[str, Any], Image]: 予測結果と出力画像(RGB)のタプル
         """
         # RGB画像をBGR画像に変換
-        img_npy = convert.img2npy(image)
+        img_npy = convert.img2npy(input_data)
         img_npy = convert.bgr2rgb(img_npy)
 
-        #input_shape = (img_width, img_height)
-        #img, ratio = self.preprocess(img_npy, input_shape)
+        input_shape = (img_width, img_height)
+        img, ratio = self.preprocess(img_npy, input_shape)
 
-        #output = session.run(None, {session.get_inputs()[0].name: img[None, :, :, :]})
-        from mmdet.apis import inference_detector
-        result = inference_detector(model, img_npy)
-        boxes = result.pred_instances.bboxes.numpy().tolist()
-        boxes = [[row[1],row[0],row[3],row[2]] for row in boxes]
-        ids = [i for i in range(len(boxes))]
-        scores = result.pred_instances.scores.numpy().tolist()
-        clses = result.pred_instances.labels.numpy().tolist()
-        output_image, output_labels = common.draw_boxes(image, boxes, scores, clses, ids=ids, labels=labels, colors=colors, nodraw=nodraw)
-        return dict(output_ids=ids, output_boxes=boxes, output_scores=scores, output_classes=clses, output_labels=output_labels), output_image
-        """
+        output = model.run(None, {model.get_inputs()[0].name: img[None, :, :, :]})
         predictions = self.postprocess(output[0], input_shape)[0]
         boxes = predictions[:, :4]
         scores = predictions[:, 4:5] * predictions[:, 5:]
         boxes_xyxy = np.ones_like(boxes)
         boxes_xyxy[:, 0] = boxes[:, 0] - boxes[:, 2]/2.
         boxes_xyxy[:, 1] = boxes[:, 1] - boxes[:, 3]/2.
         boxes_xyxy[:, 2] = boxes[:, 0] + boxes[:, 2]/2.
         boxes_xyxy[:, 3] = boxes[:, 1] + boxes[:, 3]/2.
         boxes_xyxy /= ratio
 
         dets = self.multiclass_nms(boxes_xyxy, scores, nms_thr=0.45, score_thr=0.1)
         if dets is not None:
             final_boxes, final_scores, final_cls_inds = dets[:, :4], dets[:, 4], dets[:, 5]
             final_boxes = [[row[1],row[0],row[3],row[2]] for row in final_boxes]
-            output_image = common.draw_boxes(image, final_boxes, final_scores, final_cls_inds, labels=labels, colors=colors)
+            ids = [i for i in range(len(final_boxes))]
+            output_image, output_labels = common.draw_boxes(input_data, final_boxes, final_scores, final_cls_inds, ids=ids, labels=labels, colors=colors, nodraw=nodraw)
 
-            return dict(output_boxes=final_boxes, output_scores=final_scores, output_classes=final_cls_inds), output_image
-        """
+            return dict(output_ids=ids, output_scores=final_scores, output_classes=final_cls_inds, output_labels=output_labels, output_boxes=final_boxes), output_image
+        return dict(output_ids=[], output_scores=[], output_classes=[], output_labels=[], output_boxes=[]), input_data
 
     def preprocess(self, img, input_size, swap=(2, 0, 1)):
         """
         画像を前処理する関数です。
 
         Args:
             img (numpy.ndarray): 入力画像（BGR）
```

### Comparing `iinfer-0.7.3/iinfer/app/predicts/mmseg_seg_PSPNet.py` & `iinfer-0.7.4/iinfer/app/predicts/mmseg_seg_PSPNet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,73 +1,70 @@
 from pathlib import Path
 from PIL import Image
 from iinfer.app import common, predict
 from iinfer.app.commons import convert
-from typing import List, Tuple
+from typing import List, Tuple, Union, Any
 import logging
 import numpy as np
 
 
 SITE = 'https://github.com/open-mmlab/mmsegmentation/tree/main/configs/pspnet'
 IMAGE_WIDTH = 1024
 IMAGE_HEIGHT = 512
 REQUIREd_MODEL_CONF = True
 REQUIREd_MODEL_WEIGHT = False
 
 class MMSegPSPNet(predict.TorchPredict):
     def __init__(self, logger:logging.Logger) -> None:
         super().__init__(logger)
 
-    def create_session(self, model_path:Path, model_conf_path:Path, model_provider:str, gpu_id:int=None):
+    def create_session(self, deploy_dir:Path, model_path:Union[Path|Any], model_conf_path:Path, model_provider:str, gpu_id:int=None):
         """
         推論セッションを作成する関数です。
         startコマンド実行時に呼び出されます。
         この関数内でAIモデルのロードを行い、推論準備を完了するようにしてください。
         戻り値の推論セッションの型は問いません。
 
         Args:
-            model_path (Path): モデルファイルのパス
+            deploy_dir (Path): デプロイディレクトリのパス
+            model_path (Path|Any): モデルファイルのパス
             model_conf_path (Path): モデル設定ファイルのパス
             gpu_id (int, optional): GPU ID. Defaults to None.
 
         Returns:
             推論セッション
         """
         from mmseg.apis import init_model
         import torch
         gpu = f'cuda:{gpu_id}' if gpu_id is not None else 'cuda'
         device = torch.device(gpu if self.is_gpu_available(model_path, model_conf_path, gpu_id) else 'cpu')
         model = init_model(model_conf_path, str(model_path), device=device) # , cfg_options = {'show': True}
         return model
 
-    def predict(self, model, img_width:int, img_height:int, image:Image.Image, labels:List[str]=None, colors:List[Tuple[int]]=None, nodraw:bool=False):
+    def predict(self, model, img_width:int, img_height:int, input_data:Union[Image.Image, str], labels:List[str]=None, colors:List[Tuple[int]]=None, nodraw:bool=False):
         """
         予測を行う関数です。
         predictコマンドやcaptureコマンド実行時に呼び出されます。
-        引数のimageはRGBですので、戻り値の出力画像もRGBにしてください。
+        引数のinput_dataが画像の場合RGBですので、戻り値の出力画像もRGBにしてください。
         戻り値の推論結果のdictは、通常推論結果項目ごとに値(list)を設定します。
-        例）Image Classification（EfficientNet_Lite4）の場合
-        return dict(output_scores=output_scores, output_classes=output_classes), image_obj
-        例）Object Detection（YoloX）の場合
-        return dict(output_boxes=final_boxes, output_scores=final_scores, output_classes=final_cls_inds), output_image
 
         Args:
             model: 推論セッション
-            img_width (int): モデルのINPUTサイズ（画像の幅）
-            img_height (int): モデルのINPUTサイズ（画像の高さ）
-            image (Image): 入力画像（RGB配列であること）
+            img_width (int): モデルのINPUTサイズ（input_dataが画像の場合は、画像の幅）
+            img_height (int): モデルのINPUTサイズ（input_dataが画像の場合は、画像の高さ）
+            input_data (Image | str): 推論するデータ（画像の場合RGB配列であること）
             labels (List[str], optional): クラスラベルのリスト. Defaults to None.
             colors (List[Tuple[int]], optional): ボックスの色のリスト. Defaults to None.
             nodraw (bool, optional): 描画フラグ. Defaults to False.
 
         Returns:
             Tuple[Dict[str, Any], Image]: 予測結果と出力画像(RGB)のタプル
         """
         # RGB画像をBGR画像に変換
-        img_npy = convert.img2npy(image)
+        img_npy = convert.img2npy(input_data)
 
         from mmseg.apis import inference_model
         from mmseg.structures import SegDataSample
 
         result:SegDataSample = inference_model(model, img_npy)
         if hasattr(model, 'module'):
             model = model.module
@@ -88,15 +85,15 @@
         if not nodraw:
             img = self.draw_mask(img_npy, result,
                                  labels if labels is not None else output_catalog,
                                  colors if colors is not None else model.dataset_meta['palette'])
             output_image = convert.npy2img(img)
 
         else:
-            output_image = image
+            output_image = input_data
 
         return dict(output_catalog=output_catalog,
                     output_palette=output_palette,
                     output_classes=output_classes,
                     output_labels=output_labels,
                     output_sem_seg=output_sem_seg,
                     output_sem_seg_shape=output_sem_seg_shape,
```

### Comparing `iinfer-0.7.3/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py` & `iinfer-0.7.4/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,78 +1,75 @@
 from iinfer.app import predict
 from iinfer.app.commons import convert
 from pathlib import Path
 from PIL import Image
-from typing import List, Tuple
+from typing import List, Tuple, Union, Any
 import logging
 import numpy as np
 
 
 SITE = 'https://github.com/onnx/models/tree/main/vision/classification/efficientnet-lite4'
 IMAGE_WIDTH = 224
 IMAGE_HEIGHT = 224
 REQUIREd_MODEL_CONF = False
 REQUIREd_MODEL_WEIGHT = True
 
 class OnnxClsEfficientNetLite4(predict.OnnxPredict):
     def __init__(self, logger:logging.Logger) -> None:
         super().__init__(logger)
 
-    def create_session(self, model_path:Path, model_conf_path:Path, model_provider:str, gpu_id:int=None):
+    def create_session(self, deploy_dir:Path, model_path:Union[Path|Any], model_conf_path:Path, model_provider:str, gpu_id:int=None):
         """
         推論セッションを作成する関数です。
         startコマンド実行時に呼び出されます。
         この関数内でAIモデルのロードを行い、推論準備を完了するようにしてください。
         戻り値の推論セッションの型は問いません。
 
         Args:
-            model_path (Path): モデルファイルのパス
+            deploy_dir (Path): デプロイディレクトリのパス
+            model_path (Path|Any): モデルファイルのパス
             model_conf_path (Path): モデル設定ファイルのパス
             gpu_id (int, optional): GPU ID. Defaults to None.
 
         Returns:
             推論セッション
         """
         import onnxruntime as rt
         if self.is_gpu_available(model_path, model_conf_path, gpu_id):
             session = rt.InferenceSession(model_path, providers=[model_provider])
         else:
             session = rt.InferenceSession(model_path, providers=[model_provider], providers_options=[{'device_id': str(gpu_id)}])
         return session
 
-    def predict(self, session, img_width:int, img_height:int, image:Image.Image, labels:List[str]=None, colors:List[Tuple[int]]=None, nodraw:bool=False):
+    def predict(self, model, img_width:int, img_height:int, input_data:Union[Image.Image, str], labels:List[str]=None, colors:List[Tuple[int]]=None, nodraw:bool=False):
         """
         予測を行う関数です。
         predictコマンドやcaptureコマンド実行時に呼び出されます。
-        引数のimageはRGBですので、戻り値の出力画像もRGBにしてください。
+        引数のinput_dataが画像の場合RGBですので、戻り値の出力画像もRGBにしてください。
         戻り値の推論結果のdictは、通常推論結果項目ごとに値(list)を設定します。
-        例）Image Classification（EfficientNet_Lite4）の場合
-        return dict(output_scores=output_scores, output_classes=output_classes), image_obj
-        例）Object Detection（YoloX）の場合
-        return dict(output_boxes=final_boxes, output_scores=final_scores, output_classes=final_cls_inds), output_image
 
         Args:
-            session: 推論セッション
-            img_width (int): モデルのINPUTサイズ（画像の幅）
-            img_height (int): モデルのINPUTサイズ（画像の高さ）
-            image (Image): 入力画像（RGB配列であること）
+            model: 推論セッション
+            img_width (int): モデルのINPUTサイズ（input_dataが画像の場合は、画像の幅）
+            img_height (int): モデルのINPUTサイズ（input_dataが画像の場合は、画像の高さ）
+            input_data (Image | str): 推論するデータ（画像の場合RGB配列であること）
             labels (List[str], optional): クラスラベルのリスト. Defaults to None.
             colors (List[Tuple[int]], optional): ボックスの色のリスト. Defaults to None.
             nodraw (bool, optional): 描画フラグ. Defaults to False.
 
         Returns:
             Tuple[Dict[str, Any], Image]: 予測結果と出力画像(RGB)のタプル
         """
         # RGB画像をBGR画像に変換
-        img_npy = convert.img2npy(image)
+        img_npy = convert.img2npy(input_data)
         img_npy = convert.bgr2rgb(img_npy)
 
-        image_data, _, image_obj = self.preprocess_img(image, img_width, img_height)
+        image_data, _, image_obj = self.preprocess_img(input_data, img_width, img_height)
 
-        results = session.run(["Softmax:0"], {"images:0": image_data})[0]
+        results = model.run(["Softmax:0"], {"images:0": image_data})[0]
 
         output_scores, output_classes = [], []
         result = reversed(results[0].argsort()[-5:])
         for r in result:
             output_classes.append(r)
             output_scores.append(results[0][r])
```

### Comparing `iinfer-0.7.3/iinfer/app/predicts/onnx_det_TinyYoloV3.py` & `iinfer-0.7.4/iinfer/app/predicts/onnx_det_YoloV3.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,84 @@
 from pathlib import Path
 from PIL import Image
-from typing import List, Tuple
 from iinfer.app import common, predict
-from iinfer.app.predicts import onnx_det_YoloV3
+from typing import List, Tuple, Union, Any
 import logging
 import numpy as np
 
 
-SITE = 'https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/tiny-yolov3'
+SITE = 'https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/yolov3'
 IMAGE_WIDTH = 416
 IMAGE_HEIGHT = 416
 REQUIREd_MODEL_CONF = False
 REQUIREd_MODEL_WEIGHT = True
 
-class OnnxDetTinyYoloV3(predict.OnnxPredict):
+class OnnxDetYoloV3(predict.OnnxPredict):
     def __init__(self, logger:logging.Logger) -> None:
         super().__init__(logger)
 
-    def create_session(self, model_path:Path, model_conf_path:Path, model_provider:str, gpu_id:int=None):
+    def create_session(self, deploy_dir:Path, model_path:Union[Path|Any], model_conf_path:Path, model_provider:str, gpu_id:int=None):
         """
         推論セッションを作成する関数です。
         startコマンド実行時に呼び出されます。
         この関数内でAIモデルのロードを行い、推論準備を完了するようにしてください。
         戻り値の推論セッションの型は問いません。
 
         Args:
+            deploy_dir (Path): デプロイディレクトリのパス
             model_path (Path): モデルファイルのパス
             model_conf_path (Path): モデル設定ファイルのパス
             gpu_id (int, optional): GPU ID. Defaults to None.
 
         Returns:
             推論セッション
         """
-        return onnx_det_YoloV3.create_session(model_path, model_conf_path, model_provider, gpu_id)
+        import onnxruntime as rt
+        if self.is_gpu_available(model_path, model_conf_path, gpu_id):
+            session = rt.InferenceSession(model_path, providers=[model_provider])
+        else:
+            session = rt.InferenceSession(model_path, providers=[model_provider], providers_options=[{'device_id': str(gpu_id)}])
+        return session
 
-    def predict(self, session, img_width:int, img_height:int, image:Image.Image, labels:List[str]=None, colors:List[Tuple[int]]=None, nodraw:bool=False):
+    def predict(self, model, img_width:int, img_height:int, input_data:Union[Image.Image, str], labels:List[str]=None, colors:List[Tuple[int]]=None, nodraw:bool=False):
         """
         予測を行う関数です。
         predictコマンドやcaptureコマンド実行時に呼び出されます。
-        引数のimageはRGBですので、戻り値の出力画像もRGBにしてください。
+        引数のinput_dataが画像の場合RGBですので、戻り値の出力画像もRGBにしてください。
         戻り値の推論結果のdictは、通常推論結果項目ごとに値(list)を設定します。
-        例）Image Classification（EfficientNet_Lite4）の場合
-        return dict(output_scores=output_scores, output_classes=output_classes), image_obj
-        例）Object Detection（YoloX）の場合
-        return dict(output_boxes=final_boxes, output_scores=final_scores, output_classes=final_cls_inds), output_image
 
         Args:
-            session: 推論セッション
-            img_width (int): モデルのINPUTサイズ（画像の幅）
-            img_height (int): モデルのINPUTサイズ（画像の高さ）
-            image (Image): 入力画像（RGB配列であること）
+            model: 推論セッション
+            img_width (int): モデルのINPUTサイズ（input_dataが画像の場合は、画像の幅）
+            img_height (int): モデルのINPUTサイズ（input_dataが画像の場合は、画像の高さ）
+            input_data (Image | str): 推論するデータ（画像の場合RGB配列であること）
             labels (List[str], optional): クラスラベルのリスト. Defaults to None.
             colors (List[Tuple[int]], optional): ボックスの色のリスト. Defaults to None.
             nodraw (bool, optional): 描画フラグ. Defaults to False.
 
         Returns:
             Tuple[Dict[str, Any], Image]: 予測結果と出力画像(RGB)のタプル
         """
-        image_data, image_size, image_obj = self.preprocess_img(image, img_width, img_height)
+        image_data, image_size, image_obj = self.preprocess_img(input_data, img_width, img_height)
 
-        input_name = session.get_inputs()[0].name           # 'image'
-        input_name_img_shape = session.get_inputs()[1].name # 'image_shape'
-        output_name_boxes = session.get_outputs()[0].name   # 'boxes'
-        output_name_scores = session.get_outputs()[1].name  # 'scores'
-        output_name_indices = session.get_outputs()[2].name # 'indices'
+        input_name = model.get_inputs()[0].name           # 'image'
+        input_name_img_shape = model.get_inputs()[1].name # 'image_shape'
+        output_name_boxes = model.get_outputs()[0].name   # 'boxes'
+        output_name_scores = model.get_outputs()[1].name  # 'scores'
+        output_name_indices = model.get_outputs()[2].name # 'indices'
 
-        outputs_index = session.run([output_name_boxes, output_name_scores, output_name_indices],
-                                    {input_name: image_data, input_name_img_shape: image_size})
+        outputs_index = model.run([output_name_boxes, output_name_scores, output_name_indices],
+                                  {input_name: image_data, input_name_img_shape: image_size})
 
         output_boxes = outputs_index[0]
         output_scores = outputs_index[1]
         output_indices = outputs_index[2]
 
         out_boxes, out_scores, out_classes = [], [], []
-        for idx_ in output_indices[0]:
+        for idx_ in output_indices:
             out_classes.append(idx_[1])
             out_scores.append(output_scores[tuple(idx_)])
             idx_1 = (idx_[0], idx_[2])
             out_boxes.append(output_boxes[idx_1])
 
         ids = [i for i in range(len(out_boxes))]
         output_image, output_labels = common.draw_boxes(image_obj, out_boxes, out_scores, out_classes, ids=ids, labels=labels, colors=colors, nodraw=nodraw)
@@ -91,15 +92,15 @@
         nw = int(iw*scale)
         nh = int(ih*scale)
         image = image.resize((nw,nh), Image.BICUBIC)
         new_image = Image.new('RGB', (to_w, to_h), (128,128,128))
         new_image.paste(image, ((to_w-nw)//2, (to_h-nh)//2))
         return new_image
 
-    def preprocess_img(self, image:Image, model_img_width:int, model_img_height:int):
+    def preprocess_img(self, image:Image.Image, model_img_width:int, model_img_height:int):
         boxed_image = self.resize_img(image, model_img_width, model_img_height)
         image_data = np.array(boxed_image, dtype='float32')
         image_data /= 255.
         image_data = np.transpose(image_data, [2, 0, 1])
         image_data = np.expand_dims(image_data, 0)
         image_size = np.array([image.size[1], image.size[0]], dtype=np.float32).reshape(1, 2)
         return image_data, image_size, image
```

### Comparing `iinfer-0.7.3/iinfer/app/redis.py` & `iinfer-0.7.4/iinfer/app/redis.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/app/server.py` & `iinfer-0.7.4/iinfer/app/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from motpy import Detection, MultiObjectTracker
 from pathlib import Path
 from PIL import Image
 from iinfer.app import common, predict, injection
 from iinfer.app.commons import convert, module
-from typing import List, Dict, Any, Tuple
+from typing import List, Dict, Any, Tuple, Union
 import base64
 import datetime
 import logging
 import json
 import numpy as np
 import redis
 import shutil
@@ -212,23 +212,24 @@
                 elif msg[0] == 'undeploy':
                     st = self.undeploy(msg[1], msg[2])
                 elif msg[0] == 'start':
                     st = self.start(msg[1], msg[2], msg[3], (True if msg[4]=='True' else False), (None if msg[5]=='None' else msg[5]))
                 elif msg[0] == 'stop':
                     st = self.stop(msg[1], msg[2])
                 elif msg[0] == 'predict':
-                    #byteio = BytesIO(base64.b64decode(msg[3]))
-                    #img_npy = np.load(byteio)
                     nodraw = True if msg[4] == 'True' else False
                     shape = [int(msg[5]), int(msg[6])]
                     if int(msg[7]) > 0: shape.append(int(msg[7]))
                     output_image_name = msg[8]
-                    img_npy = convert.b64str2npy(msg[3], shape)
-                    image = convert.npy2img(img_npy)
-                    st = self.predict(msg[1], msg[2], image, output_image_name, nodraw)
+                    if shape[0] >0 and shape[1] > 0:
+                        img_npy = convert.b64str2npy(msg[3], shape)
+                        image = convert.npy2img(img_npy)
+                        st = self.predict(msg[1], msg[2], image, output_image_name, nodraw)
+                    else:
+                        st = self.predict(msg[1], msg[2], convert.b64str2str(msg[3]), output_image_name, nodraw)
                 elif msg[0] == 'stop_server':
                     self.is_running = False
                     self.responce(msg[1], {"success": f"Successful stop server. svname={self.svname}"})
                     break
                 elif msg[0] == 'file_list':
                     svpath = convert.b64str2str(msg[2])
                     st = self.file_list(msg[1], svpath)
@@ -363,34 +364,35 @@
             return self.RESP_WARN
         if common.BASE_MODELS[predict_type]['required_model_conf']==True and model_conf_file is None:
             self.logger.warn(f"model_conf_file is None.")
             self.responce(reskey, {"warn": f"model_conf_file is None."})
             return self.RESP_WARN
 
         common.mkdirs(deploy_dir)
-        def _save_s(file:str, data:bytes):
+        def _save_s(file:str, data:bytes, ret_fn:bool=False):
             if file is None or data is None:
-                return False, None
+                return False, file if ret_fn else None
             file = deploy_dir / file
             with open(file, "wb") as f:
                 f.write(data)
                 self.logger.info(f"Save {file} to {str(deploy_dir)}")
-            return True, file
+            return True, file if ret_fn else None
 
-        if model_file.startswith("http") and (model_bin is None or model_bin == ''):
-            model_path = deploy_dir / urllib.parse.urlparse(model_file).path.split('/')[-1]
-            if not model_path.exists():
-                self.logger.info(f"Downloading. {model_file}")
-                urllib.request.urlretrieve(model_file, model_path)
-                self.logger.info(f"Save {model_path}")
+        if common.BASE_MODELS[predict_type]['required_model_weight']:
+            if model_file.startswith("http") and (model_bin is None or model_bin == ''):
+                model_path = deploy_dir / urllib.parse.urlparse(model_file).path.split('/')[-1]
+                if not model_path.exists():
+                    self.logger.info(f"Downloading. {model_file}")
+                    urllib.request.urlretrieve(model_file, model_path)
+                    self.logger.info(f"Save {model_path}")
+                else:
+                    self.logger.info(f"Already exists. {model_path}")
+                model_file = model_path
             else:
-                self.logger.info(f"Already exists. {model_path}")
-            model_file = model_path
-        else:
-            ret, model_file = _save_s(model_file, model_bin)
+                ret, model_file = _save_s(model_file, model_bin, ret_fn=True)
 
         ret, before_injection_conf = _save_s("before_injection_conf.json", before_injection_conf)
         ret, after_injection_conf = _save_s("after_injection_conf.json", after_injection_conf)
 
         def _save_m(name:str, files:List[str], datas:List[bytes]):
             if files is not None and datas is None:
                 self.logger.warn(f"{name}_file is not None but {name}_bin is None.")
@@ -466,14 +468,25 @@
                 if returncode != 0:
                     self.logger.error(f"Failed to git clone mmsegmentation.")
                     self.responce(reskey, {"error": f"Failed to git clone mmsegmentation."})
                     return self.RESP_ERROR
             shutil.copytree(self.data_dir / "mmsegmentation" / "configs", deploy_dir / "configs", dirs_exist_ok=True)
             self.logger.info(f"Copy mmsegmentation configs to {str(deploy_dir / 'configs')}")
 
+        try:
+            ret, predict_obj = module.build_predict(conf["predict_type"], conf["custom_predict_file"], self.logger)
+            if not ret:
+                self.responce(reskey, predict_obj)
+                return self.RESP_WARN
+            predict_obj.post_deploy(deploy_dir, conf)
+        except Exception as e:
+            self.logger.warn(f"Failed to load Predict: {e}", exc_info=True)
+            self.responce(reskey, {"warn": f"Failed to load Predict: {e}"})
+            return self.RESP_WARN
+
         self.responce(reskey, {"success": f"Save conf.json to {str(deploy_dir)}"})
         return self.RESP_SCCESS
 
     def deploy_list(self, reskey:str):
         """
         デプロイされたモデルのリストを取得する
 
@@ -573,15 +586,18 @@
         conf_path = deploy_dir / "conf.json"
         if not conf_path.exists():
             self.logger.warn(f"Conf path {str(conf_path)} does not exist")
             self.responce(reskey, {"warn": f"Conf path {str(conf_path)} does not exist"})
             return self.RESP_WARN
         with open(conf_path, "r") as cf:
             conf = json.load(cf)
-            model_path = Path(conf["model_file"])
+            if conf['predict_type'] != 'Custom' and common.BASE_MODELS[conf['predict_type']]['required_model_weight']:
+                model_path = Path(conf["model_file"])
+            else:
+                model_path = conf["model_file"]
             if "model_conf_file" in conf and conf["model_conf_file"] is not None and len(conf["model_conf_file"]) > 0:
                 model_conf_path = Path(conf["model_conf_file"][0])
             else:
                 model_conf_path = None
             try:
                 if "before_injection_conf" in conf and conf["before_injection_conf"] is not None:
                     before_injection_conf = dict()
@@ -614,36 +630,27 @@
                     after_injections = module.load_after_injection_type(types, after_injection_conf, self.logger)
                 else:
                     after_injections = None
                 if "after_injection_py" in conf and conf["after_injection_py"] is not None and len(conf["after_injection_py"]) > 0:
                     paths = [Path(p) for p in conf["after_injection_py"]]
                     after_injections = [] if after_injections is None else after_injections
                     after_injections = module.load_after_injections(paths, after_injection_conf, self.logger)
-                if not model_path.exists():
+                if type(model_path) is Path and not model_path.exists():
                     self.logger.warn(f"Model path {str(model_path)} does not exist")
                     self.responce(reskey, {"warn": f"Model path {str(model_path)} does not exist"})
                     return self.RESP_WARN
             except Exception as e:
                 self.logger.warn(f"Failed to load after_injection: {e}", exc_info=True)
                 self.responce(reskey, {"warn": f"Failed to load after_injection: {e}"})
                 return self.RESP_WARN
             try:
-                if conf["predict_type"] == 'Custom':
-                    custom_predict_py = Path(conf["custom_predict_file"]) if conf["custom_predict_file"] is not None else None
-                    if custom_predict_py is None:
-                        self.logger.warn(f"predict_type is Custom but custom_predict_py is None.")
-                        self.responce(reskey, {"warn": f"predict_type is Custom but custom_predict_py is None."})
-                        return self.RESP_WARN
-                    if not custom_predict_py.exists():
-                        self.logger.warn(f"custom_predict_py path {str(custom_predict_py)} does not exist")
-                        self.responce(reskey, {"warn": f"custom_predict_py path {str(custom_predict_py)} does not exist"})
-                        return self.RESP_WARN
-                    predict_obj = module.load_custom_predict(custom_predict_py, self.logger)
-                else:
-                    predict_obj = module.load_predict(conf["predict_type"], self.logger)
+                ret, predict_obj = module.build_predict(conf["predict_type"], conf["custom_predict_file"], self.logger)
+                if not ret:
+                    self.responce(reskey, predict_obj)
+                    return self.RESP_WARN
             except Exception as e:
                 self.logger.warn(f"Failed to load Predict: {e}", exc_info=True)
                 self.responce(reskey, {"warn": f"Failed to load Predict: {e}"})
                 return self.RESP_WARN
             if "label_file" in conf and conf["label_file"] is not None:
                 label_file = Path(conf["label_file"])
                 if not label_file.exists():
@@ -661,15 +668,15 @@
                     self.responce(reskey, {"warn": f"color_file path {str(color_file)} does not exist"})
                     return self.RESP_WARN
                 with open(color_file, "r") as f:
                     colors = f.read().splitlines()
             else:
                 colors = None
             try:
-                session = predict_obj.create_session(model_path, model_conf_path, model_provider, gpu_id=gpuid)
+                session = predict_obj.create_session(deploy_dir, model_path, model_conf_path, model_provider, gpu_id=gpuid)
                 self.sessions[name] = dict(
                     session=session,
                     model_img_width=conf["model_img_width"],
                     model_img_height=conf["model_img_height"],
                     predict_obj=predict_obj,
                     labels=labels,
                     colors=colors,
@@ -703,62 +710,62 @@
             return self.RESP_WARN
         #self.sessions[name]['session'].close()
         del self.sessions[name]
         self.logger.info(f"Successful stop of {name} session.")
         self.responce(reskey, {"success": f"Successful stop of {name} session."})
         return self.RESP_SCCESS
 
-    def predict(self, reskey:str, name:str, image:Image.Image, output_image_name:str, nodraw:bool):
+    def predict(self, reskey:str, name:str, input_data:Union[Image.Image, str], output_image_name:str, nodraw:bool):
         """
         クライアントから送られてきた画像の推論を行う。
 
         Args:
             reskey (str): レスポンスキー
             name (dict): モデル名
-            image (Image.Image): 推論する画像データ
+            input_data (Image.Image | str): 推論するデータ
             output_image_name (str): 出力画像のファイル名
             nodraw (bool): 描画フラグ
         """
         if name is None or name == "":
             self.logger.warn(f"Name is empty.")
             self.responce(reskey, {"warn": f"Name is empty."})
             return self.RESP_WARN
-        if image is None:
-            self.logger.warn(f"img_npy is empty.")
-            self.responce(reskey, {"warn": f"img_npy is empty."})
+        if input_data is None:
+            self.logger.warn(f"input_data is empty.")
+            self.responce(reskey, {"warn": f"input_data is empty."})
             return self.RESP_WARN
         if name not in self.sessions:
             self.logger.warn(f"{name} has not yet started a session.")
             self.responce(reskey, {"warn": f"{name} has not yet started a session."})
             return self.RESP_WARN
         if nodraw is None:
             nodraw = False
         session = self.sessions[name]
         try:
             predict_process_start = time.perf_counter()
             # 前処理を実行
             if session['before_injections'] is not None:
                 injections:List[injection.BeforeInjection] = session['before_injections']
                 for inject in injections:
-                    image = inject.action(reskey, name, image, session)
+                    input_data = inject.action(reskey, name, input_data, session)
             before_injections_end = time.perf_counter()
             # 推論を実行
             predict_obj:predict.Predict = session['predict_obj']
-            outputs, output_image = predict_obj.predict(session['session'], session['model_img_width'], session['model_img_height'], image,
+            outputs, output_image = predict_obj.predict(session['session'], session['model_img_width'], session['model_img_height'], input_data,
                                                         labels=session['labels'], colors=session['colors'], nodraw=nodraw)
             outputs['image_name'] = output_image_name
             predict_end = time.perf_counter()
             if session['tracker'] is not None:
                 if 'output_boxes' in outputs and 'output_scores' in outputs and 'output_classes' in outputs:
                     detections = [Detection(box, score, cls) for box, score, cls in zip(outputs['output_boxes'], outputs['output_scores'], outputs['output_classes'])]
                     session['tracker'].step(detections=detections)
                     tracks = session['tracker'].active_tracks()
                     outputs['output_tracks'] = [t.id for t in tracks]
-                    if image is not None and not nodraw:
-                        image = common.draw_boxes(image, outputs['output_boxes'], outputs['output_scores'], outputs['output_classes'], ids=outputs['output_tracks'])
+                    if output_image is not None and not nodraw:
+                        output_image, _ = common.draw_boxes(output_image, outputs['output_boxes'], outputs['output_scores'], outputs['output_classes'], ids=outputs['output_tracks'])
             tracker_end = time.perf_counter()
 
             def _after_injection(reskey:str, name:str, output:dict, output_image:Image.Image, session:dict):
                 if session['after_injections'] is not None:
                     injections:List[injection.AfterInjection] = session['after_injections']
                     for inject in injections:
                         output, output_image = inject.action(reskey, name, output, output_image, session)
```

### Comparing `iinfer-0.7.3/iinfer/app/web.py` & `iinfer-0.7.4/iinfer/app/web.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,18 +82,24 @@
                     opt_list.append(f"--{key}")
                 continue
             if type(val) == list:
                 for v in val:
                     if v is None or v == '':
                         continue
                     opt_list.append(f"--{key}")
-                    opt_list.append(str(v))
+                    if str(v).find(' ') >= 0:
+                        opt_list.append(f'"{v}"')
+                    else:
+                        opt_list.append(str(v))
             elif val is not None and val != '':
                 opt_list.append(f"--{key}")
-                opt_list.append(str(val))
+                if str(val).find(' ') >= 0:
+                    opt_list.append(f'"{val}"')
+                else:
+                    opt_list.append(str(val))
             if 'fileio' in schema and schema[0]['fileio'] == 'in' and type(val) != str:
                 file_dict[key] = val
         return opt_list, file_dict
 
     def bbforce_cmd(self):
         self.logger.info(f"bbforce_cmd")
         try:
@@ -282,19 +288,28 @@
                 #chk_input_file = len([ref for ref in cmd_ref if ref['opt'] == 'input_file']) > 0
                 if 'capture_stdout' in cmd_opt:
                     capture_stdout = cmd_opt['capture_stdout']
                 else:
                     capture_stdout = True
                 if 'output_csv' in cmd_opt and cmd_opt['output_csv'] != '':
                     output = dict(warn=f'The "output_csv" option is not supported in pipe. ({cmd_title})')
-                    if nothread: return output
                     self.callback_return_pipe_exec_func(title, output)
                     return
-
-            cmdline = self.raw_pipe(title, opt)[0]['raw']
+            cmdline = None
+            has_warn = False
+            for cl in self.raw_pipe(title, opt):
+                if cl['type'] == 'cmdline':
+                    cmdline = cl['raw']
+                if cl['type'] == 'warn':
+                    self.callback_return_pipe_exec_func(title, cl)
+                    has_warn = True
+            if cmdline is None:
+                self.callback_return_pipe_exec_func(title, dict(warn='No command to execute.'))
+                has_warn = True
+            if has_warn: return
             try:
                 container['pipe_proc'] = subprocess.Popen(cmdline, shell=True, text=True, encoding='utf-8', 
                                                         stdout=(subprocess.PIPE if capture_stdout else None),
                                                         stderr=(subprocess.STDOUT if capture_stdout else None))
                 output = ""
                 output_size = 0
                 while container['pipe_proc'].poll() is None:
@@ -307,15 +322,15 @@
                             if len(o) < self.output_size_th:
                                 o = to_json(o)
                                 self.callback_return_stream_log_func(o)
                             else:
                                 o = [dict(warn=f'The captured stdout was discarded because its size was larger than {self.output_size_th} bytes.')]
                                 self.callback_return_stream_log_func(o)
                         except:
-                            o = [dict(warn=f'<pre>{html.escape(traceback.format_exc())}</pre>')]
+                            o = [dict(warn=f'<pre>{html.escape(o)}</pre><br><pre>{html.escape(traceback.format_exc())}</pre>')]
                             self.callback_return_stream_log_func(o)
                 if capture_stdout:
                     container['pipe_proc'].stdout.read() # 最後のストリームは読み捨て
                 else:
                     output = [dict(warn='capture_stdout is off.')]
             except Exception as e:
                 output = [dict(warn=f'<pre>{html.escape(traceback.format_exc())}</pre>')]
@@ -357,14 +372,16 @@
             chk_stdin = len([ref for ref in cmd_ref if ref['opt'] == 'stdin']) > 0
 
             if 'output_csv' in cmd_opt and cmd_opt['output_csv'] != '':
                 errormsg.append(f'The "output_csv" option is not supported in pipe. ({cmd_title})')
             if i>0:
                 if chk_stdin and ('stdin' not in cmd_opt or not cmd_opt['stdin']):
                     errormsg.append(f'The "stdin" option should be specified for the second and subsequent commands. ({cmd_title})')
+                if chk_stdin and 'pred_input_type' in cmd_opt and cmd_opt['pred_input_type'] not in ['capture', 'prompt']:
+                    errormsg.append(f'When using the "stdin" option, "pred_input_type" cannot be other than "capture" or "prompt". ({cmd_title})')
                 for ref in cmd_ref:
                     if 'fileio' in ref and ref['fileio'] == 'in' and ref['opt'] in cmd_opt and cmd_opt[ref['opt']] != '' and len([v for v in cmd_opt[ref['opt']] if v != '']) > 0:
                         errormsg.append(f'The "{ref["opt"]}" option should not be specified in a second or subsequent command. ({cmd_title})')
             if i==0:
                 if 'request_files' in opt and len(opt['request_files']) > 0:
                     for fn in opt['request_files']:
                         if fn in cmd_opt:
```

### Comparing `iinfer-0.7.3/iinfer/docker/Dockerfile` & `iinfer-0.7.4/iinfer/docker/Dockerfile`

 * *Files 21% similar despite different names*

```diff
@@ -7,23 +7,25 @@
     useradd -m -g ${MKUSER} -s /usr/bin/bash ${MKUSER}
 ENV DEBIAN_FRONTEND=noninteractive
 ENV TZ=Asia/Tokyo
 #{INSTALL_PYTHON}
 RUN apt-get update && \
     apt-get install -y libgl1-mesa-dev libglib2.0-0 git build-essential
 RUN pip install --upgrade pip && \
-    pip install #{INSTALL_IINFER}
+    pip install #{INSTALL_IINFER} && \
+    iinfer --version
 
 #{INSTALL_ONNX}
 #{INSTALL_MMDET}
 #{INSTALL_MMSEG}
 #{INSTALL_MMCLS}
 #{INSTALL_MMPRETRAIN}
 #{INSTALL_INSIGHTFACE}
 #{INSTALL_DIFFUSERS}
+#{INSTALL_LLAMAINDEX}
 RUN mkdir -p /home/${MKUSER}/.iinfer && chown -R ${MKUSER}:${MKUSER} /home/${MKUSER}/.iinfer
 
 ENV REDIS_HOST=redis
 ENV REDIS_PORT=6379
 ENV REDIS_PASSWORD=password
 ENV SVNAME=server#{INSTALL_TAG}
```

### Comparing `iinfer-0.7.3/iinfer/extensions/configs/mmdet/yolox_s_8xb8-300e_coco.py` & `iinfer-0.7.4/iinfer/extensions/configs/mmdet/yolox_s_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/extensions/configs/mmdet/yolox_tiny_8xb8-300e_coco.py` & `iinfer-0.7.4/iinfer/extensions/configs/mmdet/yolox_tiny_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/extensions/configs/mmdet/yolox_tta.py` & `iinfer-0.7.4/iinfer/extensions/configs/mmdet/yolox_tta.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/extensions/configs/mmseg/san-vit-b16_coco-stuff164k-640x640.py` & `iinfer-0.7.4/iinfer/extensions/configs/mmseg/san-vit-b16_coco-stuff164k-640x640.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/extensions/configs/mmseg/san-vit-l14_coco-stuff164k-640x640.py` & `iinfer-0.7.4/iinfer/extensions/configs/mmseg/san-vit-l14_coco-stuff164k-640x640.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py` & `iinfer-0.7.4/iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/extensions/configs/mmseg/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py` & `iinfer-0.7.4/iinfer/extensions/configs/mmseg/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/extensions/label_coco.txt` & `iinfer-0.7.4/iinfer/extensions/label_coco.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt` & `iinfer-0.7.4/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/licenses/files.txt` & `iinfer-0.7.4/iinfer/licenses/files.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/logconf_client.yml` & `iinfer-0.7.4/iinfer/logconf_client.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/logconf_gui.yml` & `iinfer-0.7.4/iinfer/logconf_gui.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/logconf_install.yml` & `iinfer-0.7.4/iinfer/logconf_install.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/logconf_postprocess.yml` & `iinfer-0.7.4/iinfer/logconf_postprocess.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/logconf_redis.yml` & `iinfer-0.7.4/iinfer/logconf_redis.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/logconf_server.yml` & `iinfer-0.7.4/iinfer/logconf_server.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/logconf_web.yml` & `iinfer-0.7.4/iinfer/logconf_web.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/version.py` & `iinfer-0.7.4/iinfer/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 
 
-dt_now = datetime.datetime(2024, 5, 6)
+dt_now = datetime.datetime(2024, 5, 18)
 __title__ = 'iinfer (Image Inference Application)'
-__version__ = '0.7.3'
+__version__ = '0.7.4'
 __copyright__ = f'Copyright © 2023-{dt_now.strftime("%Y")} hamacom2004jp'
 __pypiurl__ = 'https://pypi.org/project/iinfer/'
 __srcurl__ = 'https://github.com/hamacom2004jp/iinfer'
 __docurl__ = 'https://hamacom2004jp.github.io/iinfer/index.html'
 __description__ = f'{__title__} {__version__}\n' + \
                   f'{__copyright__}\n' + \
                   f'Web Site: PyPi <{__pypiurl__}>\n' + \
```

### Comparing `iinfer-0.7.3/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js` & `iinfer-0.7.4/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js` & `iinfer-0.7.4/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css` & `iinfer-0.7.4/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css` & `iinfer-0.7.4/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/iinfer/filer_modal.js` & `iinfer-0.7.4/iinfer/web/assets/iinfer/filer_modal.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/iinfer/list_cmd.js` & `iinfer-0.7.4/iinfer/web/assets/iinfer/list_cmd.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -109,15 +109,19 @@
                     btn_a.append('<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-plus" viewBox="0 0 16 16">' +
                         '<path d="M8 4a.5.5 0 0 1 .5.5v3h3a.5.5 0 0 1 0 1h-3v3a.5.5 0 0 1-1 0v-3h-3a.5.5 0 0 1 0-1h3v-3A.5.5 0 0 1 8 4z"/>' +
                         '</svg>');
                     input_elem.parent().append(btn_a);
                     let mk_func = (row, next_elem) => {
                         // row, next_elemの値を残すためにクロージャーにする
                         return () => {
-                            add_form_func(0, row, next_elem);
+                            r = {
+                                ...row
+                            };
+                            r.hide = false;
+                            add_form_func(0, r, next_elem);
                         }
                     }
                     btn_a.click(mk_func(row, input_elem.parent().parent()));
                     // 2個目以降は削除ボタンを追加
                     if (cmd_modal.find(`[name="${target_name}"]`).length > 1) {
                         mk_func = (del_elem, row) => {
                             // del_elemの値を残すためにクロージャーにする
```

### Comparing `iinfer-0.7.3/iinfer/web/assets/iinfer/list_pipe.js` & `iinfer-0.7.4/iinfer/web/assets/iinfer/list_pipe.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/iinfer/main.js` & `iinfer-0.7.4/iinfer/web/assets/iinfer/main.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/iinfer/svfiler.js` & `iinfer-0.7.4/iinfer/web/assets/iinfer/svfiler.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/iinfer/view_raw.js` & `iinfer-0.7.4/iinfer/web/assets/iinfer/view_raw.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/iinfer/view_result.js` & `iinfer-0.7.4/iinfer/web/assets/iinfer/view_result.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/jquery/jquery.min.3.2.0.js` & `iinfer-0.7.4/iinfer/web/assets/jquery/jquery.min.3.2.0.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js` & `iinfer-0.7.4/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/jquery-ui/AUTHORS.txt` & `iinfer-0.7.4/iinfer/web/assets/jquery-ui/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/jquery-ui/LICENSE.txt` & `iinfer-0.7.4/iinfer/web/assets/jquery-ui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png` & `iinfer-0.7.4/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png` & `iinfer-0.7.4/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png` & `iinfer-0.7.4/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png` & `iinfer-0.7.4/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png` & `iinfer-0.7.4/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png` & `iinfer-0.7.4/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/jquery-ui/jquery-ui.min.css` & `iinfer-0.7.4/iinfer/web/assets/jquery-ui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/jquery-ui/jquery-ui.min.js` & `iinfer-0.7.4/iinfer/web/assets/jquery-ui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css` & `iinfer-0.7.4/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css` & `iinfer-0.7.4/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/jquery-ui/package.json` & `iinfer-0.7.4/iinfer/web/assets/jquery-ui/package.json`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/lightbox2/css/lightbox.min.css` & `iinfer-0.7.4/iinfer/web/assets/lightbox2/css/lightbox.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/lightbox2/images/loading.gif` & `iinfer-0.7.4/iinfer/web/assets/lightbox2/images/loading.gif`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/lightbox2/images/next.png` & `iinfer-0.7.4/iinfer/web/assets/lightbox2/images/next.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/lightbox2/images/prev.png` & `iinfer-0.7.4/iinfer/web/assets/lightbox2/images/prev.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/lightbox2/js/lightbox.min.js` & `iinfer-0.7.4/iinfer/web/assets/lightbox2/js/lightbox.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/tree-menu/css/tree-menu.css` & `iinfer-0.7.4/iinfer/web/assets/tree-menu/css/tree-menu.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/assets/tree-menu/js/tree-menu.js` & `iinfer-0.7.4/iinfer/web/assets/tree-menu/js/tree-menu.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer/web/gui.html` & `iinfer-0.7.4/iinfer/web/gui.html`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.3/iinfer.egg-info/PKG-INFO` & `iinfer-0.7.4/iinfer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iinfer
-Version: 0.7.3
+Version: 0.7.4
 Summary: iinfer: An application that executes AI model files in onnx or mmlab format.
 Home-page: https://github.com/hamacom2004jp/iinfer
 Author: hamacom2004jp
 Author-email: hamacom2004jp@gmail.com
 Maintainer: hamacom2004jp
 Maintainer-email: hamacom2004jp@gmail.com
 License: MIT
```

### Comparing `iinfer-0.7.3/iinfer.egg-info/SOURCES.txt` & `iinfer-0.7.4/iinfer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,21 +47,21 @@
 iinfer/app/postprocesses/det_face_store.py
 iinfer/app/postprocesses/det_filter.py
 iinfer/app/postprocesses/det_jadge.py
 iinfer/app/postprocesses/httpreq.py
 iinfer/app/postprocesses/seg_bbox.py
 iinfer/app/postprocesses/seg_filter.py
 iinfer/app/predicts/__init__.py
-iinfer/app/predicts/diffusers_stablediffusion_txt2img.py
+iinfer/app/predicts/diffusers_stablediffusionpipeline_txt2img.py
 iinfer/app/predicts/insightface_det.py
+iinfer/app/predicts/llamaindex_elyza_search.py
 iinfer/app/predicts/mmdet_det_YoloX.py
 iinfer/app/predicts/mmdet_det_YoloX_Lite.py
 iinfer/app/predicts/mmpretrain_cls_swin.py
 iinfer/app/predicts/mmpretrain_cls_swin_Lite.py
-iinfer/app/predicts/mmrotate_det_ReDet.py
 iinfer/app/predicts/mmseg_seg_PSPNet.py
 iinfer/app/predicts/mmseg_seg_San.py
 iinfer/app/predicts/mmseg_seg_SwinUpernet.py
 iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py
 iinfer/app/predicts/onnx_det_TinyYoloV3.py
 iinfer/app/predicts/onnx_det_YoloV3.py
 iinfer/app/predicts/onnx_det_YoloX.py
```

### Comparing `iinfer-0.7.3/setup.py` & `iinfer-0.7.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     'opencv-python',
     'Pillow',
     'pyyaml',
     'redis',
     'requests',
     'tabulate',
     'urllib3',
-    'wheel'
+    'wheel',
+    'wxPython'
 ]
 PACKAGES = [
     'iinfer',
     'iinfer.app',
     'iinfer.app.commons',
     'iinfer.app.injections',
     'iinfer.app.postprocesses',
```

