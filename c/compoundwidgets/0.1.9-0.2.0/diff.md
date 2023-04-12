# Comparing `tmp/compoundwidgets-0.1.9.tar.gz` & `tmp/compoundwidgets-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compoundwidgets-0.1.9.tar", last modified: Mon Jul 18 15:43:25 2022, max compression
+gzip compressed data, was "compoundwidgets-0.2.0.tar", last modified: Wed Apr 12 14:10:19 2023, max compression
```

## Comparing `compoundwidgets-0.1.9.tar` & `compoundwidgets-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,1002 @@
-drwxrwxrwx   0        0        0        0 2022-07-18 15:43:25.460876 compoundwidgets-0.1.9/
--rw-rw-rw-   0        0        0     1058 2022-06-17 11:09:41.000000 compoundwidgets-0.1.9/LICENSE.txt
--rw-rw-rw-   0        0        0      432 2022-07-18 13:44:59.000000 compoundwidgets-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0      332 2022-07-18 15:43:25.460876 compoundwidgets-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      160 2022-06-17 11:09:41.000000 compoundwidgets-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2022-07-18 15:43:25.329394 compoundwidgets-0.1.9/compoundwidgets/
--rw-rw-rw-   0        0        0    36487 2022-07-18 15:40:34.000000 compoundwidgets-0.1.9/compoundwidgets/COMPOUND_WIDGETS.py
--rw-rw-rw-   0        0        0     5774 2022-07-18 12:52:05.000000 compoundwidgets-0.1.9/compoundwidgets/CUSTOM_BUTTONS.py
--rw-rw-rw-   0        0        0     9353 2022-06-17 11:09:41.000000 compoundwidgets-0.1.9/compoundwidgets/CUSTOM_FRAMES.py
-drwxrwxrwx   0        0        0        0 2022-07-18 15:43:25.398386 compoundwidgets-0.1.9/compoundwidgets/IMAGES/
--rw-rw-rw-   0        0        0        0 2022-07-18 13:42:01.000000 compoundwidgets-0.1.9/compoundwidgets/IMAGES/__init__.py
--rw-rw-rw-   0        0        0     7038 2022-06-17 11:09:41.000000 compoundwidgets-0.1.9/compoundwidgets/IMAGES/add_to_form.png
--rw-rw-rw-   0        0        0    56482 2022-06-17 11:09:41.000000 compoundwidgets-0.1.9/compoundwidgets/IMAGES/back.png
--rw-rw-rw-   0        0        0    14398 2022-06-17 11:09:41.000000 compoundwidgets-0.1.9/compoundwidgets/IMAGES/calculate.png
--rw-rw-rw-   0        0        0     7680 2022-06-17 11:09:41.000000 compoundwidgets-0.1.9/compoundwidgets/IMAGES/clear.png
--rw-rw-rw-   0        0        0     4075 2022-06-17 11:09:41.000000 compoundwidgets-0.1.9/compoundwidgets/IMAGES/edit_form.png
--rw-rw-rw-   0        0        0    17569 2022-06-17 11:09:41.000000 compoundwidgets-0.1.9/compoundwidgets/IMAGES/help.png
--rw-rw-rw-   0        0        0    20256 2022-06-17 11:09:41.000000 compoundwidgets-0.1.9/compoundwidgets/IMAGES/no.png
--rw-rw-rw-   0        0        0     6569 2022-06-17 11:09:41.000000 compoundwidgets-0.1.9/compoundwidgets/IMAGES/remove_from_form.png
--rw-rw-rw-   0        0        0     4873 2022-06-17 11:09:41.000000 compoundwidgets-0.1.9/compoundwidgets/IMAGES/save.png
--rw-rw-rw-   0        0        0     5766 2022-06-17 11:09:41.000000 compoundwidgets-0.1.9/compoundwidgets/IMAGES/yes.png
--rw-rw-rw-   0        0        0    11691 2022-06-17 11:09:41.000000 compoundwidgets-0.1.9/compoundwidgets/MESSAGE_BOX_WIDGETS.py
--rw-rw-rw-   0        0        0     1272 2022-07-18 15:43:17.000000 compoundwidgets-0.1.9/compoundwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-18 15:43:25.376258 compoundwidgets-0.1.9/compoundwidgets.egg-info/
--rw-rw-rw-   0        0        0      332 2022-07-18 15:43:24.000000 compoundwidgets-0.1.9/compoundwidgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      959 2022-07-18 15:43:25.000000 compoundwidgets-0.1.9/compoundwidgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-18 15:43:24.000000 compoundwidgets-0.1.9/compoundwidgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2022-07-18 15:43:24.000000 compoundwidgets-0.1.9/compoundwidgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-07-18 15:43:25.000000 compoundwidgets-0.1.9/compoundwidgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-18 15:43:25.460876 compoundwidgets-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      575 2022-07-18 15:43:17.000000 compoundwidgets-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-18 15:43:25.460876 compoundwidgets-0.1.9/test/
--rw-rw-rw-   0        0        0     6284 2022-07-18 15:29:34.000000 compoundwidgets-0.1.9/test/test_all_compound_widgets.py
--rw-rw-rw-   0        0        0     1803 2022-06-17 11:09:41.000000 compoundwidgets-0.1.9/test/test_collapsable_frame.py
--rw-rw-rw-   0        0        0      570 2022-06-17 11:09:41.000000 compoundwidgets-0.1.9/test/test_custom_buttons.py
--rw-rw-rw-   0        0        0     2066 2022-06-17 11:09:41.000000 compoundwidgets-0.1.9/test/test_message_boxes.py
--rw-rw-rw-   0        0        0      983 2022-06-17 11:09:41.000000 compoundwidgets-0.1.9/test/test_scrollable_frame.py
--rw-rw-rw-   0        0        0      996 2022-07-11 17:32:32.000000 compoundwidgets-0.1.9/test/test_spinbox.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:19.164003 compoundwidgets-0.2.0/
+-rw-rw-rw-   0        0        0     1062 2023-04-12 10:28:05.000000 compoundwidgets-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      538 2023-03-10 20:29:07.000000 compoundwidgets-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      332 2023-04-12 14:10:19.164003 compoundwidgets-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:10.419089 compoundwidgets-0.2.0/compoundwidgets/
+-rw-rw-rw-   0        0        0     7179 2023-04-12 10:28:05.000000 compoundwidgets-0.2.0/compoundwidgets/AUTOCOMPLETE_WIDGETS.py
+-rw-rw-rw-   0        0        0    51971 2023-04-12 10:28:05.000000 compoundwidgets-0.2.0/compoundwidgets/COMPOUND_WIDGETS.py
+-rw-rw-rw-   0        0        0     7766 2023-04-12 10:28:05.000000 compoundwidgets-0.2.0/compoundwidgets/CUSTOM_BUTTONS.py
+-rw-rw-rw-   0        0        0    16269 2023-04-07 22:03:31.000000 compoundwidgets-0.2.0/compoundwidgets/CUSTOM_FRAMES.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:10.498763 compoundwidgets-0.2.0/compoundwidgets/IMAGES/
+-rw-rw-rw-   0        0        0        0 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/__init__.py
+-rw-rw-rw-   0        0        0     3203 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/add_new.png
+-rw-rw-rw-   0        0        0     7038 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/add_to_form.png
+-rw-rw-rw-   0        0        0    56482 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/back.png
+-rw-rw-rw-   0        0        0    14398 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/calculate.png
+-rw-rw-rw-   0        0        0     7680 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/clear.png
+-rw-rw-rw-   0        0        0     4075 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/edit_form.png
+-rw-rw-rw-   0        0        0    17569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/help.png
+-rw-rw-rw-   0        0        0    20256 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/no.png
+-rw-rw-rw-   0        0        0    13946 2023-03-06 16:15:17.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/quit.png
+-rw-rw-rw-   0        0        0     6569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/remove_from_form.png
+-rw-rw-rw-   0        0        0     4873 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/save.png
+-rw-rw-rw-   0        0        0     8180 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/trash_can.png
+-rw-rw-rw-   0        0        0     5433 2023-04-07 20:00:14.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/yes.png
+-rw-rw-rw-   0        0        0    15883 2023-04-12 10:10:39.000000 compoundwidgets-0.2.0/compoundwidgets/LED_BUTTONS.py
+-rw-rw-rw-   0        0        0    15192 2023-04-12 13:54:57.000000 compoundwidgets-0.2.0/compoundwidgets/MESSAGE_BOX_WIDGETS.py
+-rw-rw-rw-   0        0        0     2272 2023-04-12 10:28:05.000000 compoundwidgets-0.2.0/compoundwidgets/SCRIPTS.py
+-rw-rw-rw-   0        0        0     1843 2023-04-12 10:28:05.000000 compoundwidgets-0.2.0/compoundwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:10.451516 compoundwidgets-0.2.0/compoundwidgets.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-04-12 14:10:09.000000 compoundwidgets-0.2.0/compoundwidgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    49571 2023-04-12 14:10:10.000000 compoundwidgets-0.2.0/compoundwidgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 14:10:09.000000 compoundwidgets-0.2.0/compoundwidgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-12 14:10:09.000000 compoundwidgets-0.2.0/compoundwidgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-12 14:10:09.000000 compoundwidgets-0.2.0/compoundwidgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 14:10:19.164003 compoundwidgets-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      576 2023-04-05 20:13:41.000000 compoundwidgets-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:10.578957 compoundwidgets-0.2.0/test/
+-rw-rw-rw-   0        0        0     2815 2023-04-07 11:49:55.000000 compoundwidgets-0.2.0/test/autocomplete_widget_test.py
+-rw-rw-rw-   0        0        0    10106 2023-04-07 11:48:52.000000 compoundwidgets-0.2.0/test/compound_widgets_test_1.py
+-rw-rw-rw-   0        0        0     7285 2023-04-07 19:05:00.000000 compoundwidgets-0.2.0/test/compound_widgets_test_2.py
+-rw-rw-rw-   0        0        0      981 2023-04-07 20:22:34.000000 compoundwidgets-0.2.0/test/custom_buttons_test.py
+-rw-rw-rw-   0        0        0     2517 2023-04-07 21:26:04.000000 compoundwidgets-0.2.0/test/custom_frames_test_1.py
+-rw-rw-rw-   0        0        0     2495 2023-04-07 21:32:27.000000 compoundwidgets-0.2.0/test/custom_frames_test_2.py
+-rw-rw-rw-   0        0        0      888 2023-04-07 22:03:48.000000 compoundwidgets-0.2.0/test/custom_frames_test_3.py
+-rw-rw-rw-   0        0        0     4541 2023-04-12 10:11:28.000000 compoundwidgets-0.2.0/test/led_buttons_test.py
+-rw-rw-rw-   0        0        0     3937 2023-04-12 13:58:27.000000 compoundwidgets-0.2.0/test/message_box_test.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:10.344025 compoundwidgets-0.2.0/venv/
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:10.271765 compoundwidgets-0.2.0/venv/Lib/
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:10.593930 compoundwidgets-0.2.0/venv/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:11.609021 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/
+-rw-rw-rw-   0        0        0     3359 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/BdfFontFile.py
+-rw-rw-rw-   0        0        0    16483 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/BlpImagePlugin.py
+-rw-rw-rw-   0        0        0    18138 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/BmpImagePlugin.py
+-rw-rw-rw-   0        0        0     1629 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/BufrStubImagePlugin.py
+-rw-rw-rw-   0        0        0     3003 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ContainerIO.py
+-rw-rw-rw-   0        0        0     1796 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/CurImagePlugin.py
+-rw-rw-rw-   0        0        0     2037 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/DcxImagePlugin.py
+-rw-rw-rw-   0        0        0     9637 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/DdsImagePlugin.py
+-rw-rw-rw-   0        0        0    15413 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/EpsImagePlugin.py
+-rw-rw-rw-   0        0        0    10098 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ExifTags.py
+-rw-rw-rw-   0        0        0     2132 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/FitsImagePlugin.py
+-rw-rw-rw-   0        0        0     1749 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/FitsStubImagePlugin.py
+-rw-rw-rw-   0        0        0     4614 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/FliImagePlugin.py
+-rw-rw-rw-   0        0        0     2874 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/FontFile.py
+-rw-rw-rw-   0        0        0     7214 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/FpxImagePlugin.py
+-rw-rw-rw-   0        0        0     3980 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/FtexImagePlugin.py
+-rw-rw-rw-   0        0        0     3010 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/GbrImagePlugin.py
+-rw-rw-rw-   0        0        0     2704 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/GdImageFile.py
+-rw-rw-rw-   0        0        0    36797 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/GifImagePlugin.py
+-rw-rw-rw-   0        0        0     3533 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/GimpGradientFile.py
+-rw-rw-rw-   0        0        0     1401 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/GimpPaletteFile.py
+-rw-rw-rw-   0        0        0     1623 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/GribStubImagePlugin.py
+-rw-rw-rw-   0        0        0     1626 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/Hdf5StubImagePlugin.py
+-rw-rw-rw-   0        0        0    12329 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/IcnsImagePlugin.py
+-rw-rw-rw-   0        0        0    11980 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/IcoImagePlugin.py
+-rw-rw-rw-   0        0        0    11238 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImImagePlugin.py
+-rw-rw-rw-   0        0        0   137510 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/Image.py
+-rw-rw-rw-   0        0        0     7306 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageChops.py
+-rw-rw-rw-   0        0        0    38772 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageCms.py
+-rw-rw-rw-   0        0        0     9097 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageColor.py
+-rw-rw-rw-   0        0        0    39813 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageDraw.py
+-rw-rw-rw-   0        0        0     6210 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageDraw2.py
+-rw-rw-rw-   0        0        0     3293 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageEnhance.py
+-rw-rw-rw-   0        0        0    24312 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageFile.py
+-rw-rw-rw-   0        0        0    17019 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageFilter.py
+-rw-rw-rw-   0        0        0    51659 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageFont.py
+-rw-rw-rw-   0        0        0     4834 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageGrab.py
+-rw-rw-rw-   0        0        0     7620 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageMath.py
+-rw-rw-rw-   0        0        0     3004 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageMode.py
+-rw-rw-rw-   0        0        0     8231 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageMorph.py
+-rw-rw-rw-   0        0        0    21590 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageOps.py
+-rw-rw-rw-   0        0        0     8421 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImagePalette.py
+-rw-rw-rw-   0        0        0      355 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImagePath.py
+-rw-rw-rw-   0        0        0     7119 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageQt.py
+-rw-rw-rw-   0        0        0     1948 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageSequence.py
+-rw-rw-rw-   0        0        0    11813 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageShow.py
+-rw-rw-rw-   0        0        0     4072 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageStat.py
+-rw-rw-rw-   0        0        0     8988 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageTk.py
+-rw-rw-rw-   0        0        0     2985 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageTransform.py
+-rw-rw-rw-   0        0        0     7421 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageWin.py
+-rw-rw-rw-   0        0        0     2680 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImtImagePlugin.py
+-rw-rw-rw-   0        0        0     6007 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/IptcImagePlugin.py
+-rw-rw-rw-   0        0        0    11982 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/Jpeg2KImagePlugin.py
+-rw-rw-rw-   0        0        0    30012 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/JpegImagePlugin.py
+-rw-rw-rw-   0        0        0    12583 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/JpegPresets.py
+-rw-rw-rw-   0        0        0     1871 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/McIdasImagePlugin.py
+-rw-rw-rw-   0        0        0     2699 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/MicImagePlugin.py
+-rw-rw-rw-   0        0        0     1905 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/MpegImagePlugin.py
+-rw-rw-rw-   0        0        0     6486 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/MpoImagePlugin.py
+-rw-rw-rw-   0        0        0     5806 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/MspImagePlugin.py
+-rw-rw-rw-   0        0        0     6754 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PSDraw.py
+-rw-rw-rw-   0        0        0     1179 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PaletteFile.py
+-rw-rw-rw-   0        0        0     9369 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PalmImagePlugin.py
+-rw-rw-rw-   0        0        0     1558 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PcdImagePlugin.py
+-rw-rw-rw-   0        0        0     7013 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PcfFontFile.py
+-rw-rw-rw-   0        0        0     6242 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PcxImagePlugin.py
+-rw-rw-rw-   0        0        0     9264 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PdfImagePlugin.py
+-rw-rw-rw-   0        0        0    35563 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PdfParser.py
+-rw-rw-rw-   0        0        0     1720 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PixarImagePlugin.py
+-rw-rw-rw-   0        0        0    48199 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PngImagePlugin.py
+-rw-rw-rw-   0        0        0    11746 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PpmImagePlugin.py
+-rw-rw-rw-   0        0        0     7838 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PsdImagePlugin.py
+-rw-rw-rw-   0        0        0    10189 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PyAccess.py
+-rw-rw-rw-   0        0        0     3722 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/QoiImagePlugin.py
+-rw-rw-rw-   0        0        0     6409 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/SgiImagePlugin.py
+-rw-rw-rw-   0        0        0     9792 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/SpiderImagePlugin.py
+-rw-rw-rw-   0        0        0     4537 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/SunImagePlugin.py
+-rw-rw-rw-   0        0        0     1557 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/TarIO.py
+-rw-rw-rw-   0        0        0     6830 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/TgaImagePlugin.py
+-rw-rw-rw-   0        0        0    79211 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/TiffImagePlugin.py
+-rw-rw-rw-   0        0        0    17374 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/TiffTags.py
+-rw-rw-rw-   0        0        0     5642 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/WalImageFile.py
+-rw-rw-rw-   0        0        0    11732 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/WebPImagePlugin.py
+-rw-rw-rw-   0        0        0     4867 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/WmfImagePlugin.py
+-rw-rw-rw-   0        0        0     2064 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/XVThumbImagePlugin.py
+-rw-rw-rw-   0        0        0     2581 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/XbmImagePlugin.py
+-rw-rw-rw-   0        0        0     3312 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/XpmImagePlugin.py
+-rw-rw-rw-   0        0        0     2091 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/__main__.py
+-rw-rw-rw-   0        0        0     2145 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/_binary.py
+-rw-rw-rw-   0        0        0     2071 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/_deprecate.py
+-rw-rw-rw-   0        0        0      691 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/_tkinter_finder.py
+-rw-rw-rw-   0        0        0      388 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/_util.py
+-rw-rw-rw-   0        0        0       52 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/_version.py
+-rw-rw-rw-   0        0        0     9949 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/features.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:11.625652 compoundwidgets-0.2.0/venv/Lib/site-packages/_distutils_hack/
+-rw-rw-rw-   0        0        0     6128 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/_distutils_hack/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/_distutils_hack/override.py
+-rw-rw-rw-   0        0        0     5770 2023-04-07 11:44:14.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/_virtualenv.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:11.673007 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/
+-rw-rw-rw-   0        0        0      357 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/__main__.py
+-rw-rw-rw-   0        0        0     1444 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/__pip-runner__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:11.755008 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/
+-rw-rw-rw-   0        0        0      573 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/__init__.py
+-rw-rw-rw-   0        0        0    10243 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/build_env.py
+-rw-rw-rw-   0        0        0    10734 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cache.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:11.880531 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/
+-rw-rw-rw-   0        0        0      132 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/__init__.py
+-rw-rw-rw-   0        0        0     6676 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
+-rw-rw-rw-   0        0        0     7842 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/base_command.py
+-rw-rw-rw-   0        0        0    29497 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-rw-rw-   0        0        0      774 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/command_context.py
+-rw-rw-rw-   0        0        0     2472 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/main.py
+-rw-rw-rw-   0        0        0     4338 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/main_parser.py
+-rw-rw-rw-   0        0        0    10817 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/parser.py
+-rw-rw-rw-   0        0        0     1968 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
+-rw-rw-rw-   0        0        0    18172 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/req_command.py
+-rw-rw-rw-   0        0        0     5118 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/spinners.py
+-rw-rw-rw-   0        0        0      116 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/status_codes.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.070182 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/
+-rw-rw-rw-   0        0        0     3882 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/__init__.py
+-rw-rw-rw-   0        0        0     7582 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/cache.py
+-rw-rw-rw-   0        0        0     1685 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/check.py
+-rw-rw-rw-   0        0        0     4129 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/completion.py
+-rw-rw-rw-   0        0        0     9815 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/configuration.py
+-rw-rw-rw-   0        0        0     6591 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/debug.py
+-rw-rw-rw-   0        0        0     5289 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/download.py
+-rw-rw-rw-   0        0        0     2951 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/freeze.py
+-rw-rw-rw-   0        0        0     1703 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/hash.py
+-rw-rw-rw-   0        0        0     1132 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/help.py
+-rw-rw-rw-   0        0        0     4793 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/index.py
+-rw-rw-rw-   0        0        0     3188 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/inspect.py
+-rw-rw-rw-   0        0        0    32389 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/install.py
+-rw-rw-rw-   0        0        0    12343 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/list.py
+-rw-rw-rw-   0        0        0     5697 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/search.py
+-rw-rw-rw-   0        0        0     6419 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/show.py
+-rw-rw-rw-   0        0        0     3886 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/uninstall.py
+-rw-rw-rw-   0        0        0     7396 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/wheel.py
+-rw-rw-rw-   0        0        0    13529 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/configuration.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.117629 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/distributions/
+-rw-rw-rw-   0        0        0      858 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/distributions/__init__.py
+-rw-rw-rw-   0        0        0     1221 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/distributions/base.py
+-rw-rw-rw-   0        0        0      729 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/distributions/installed.py
+-rw-rw-rw-   0        0        0     6494 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/distributions/sdist.py
+-rw-rw-rw-   0        0        0     1164 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/distributions/wheel.py
+-rw-rw-rw-   0        0        0    24244 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.149931 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/index/
+-rw-rw-rw-   0        0        0       30 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/index/__init__.py
+-rw-rw-rw-   0        0        0    16504 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/index/collector.py
+-rw-rw-rw-   0        0        0    37873 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/index/package_finder.py
+-rw-rw-rw-   0        0        0     6557 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/index/sources.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.197270 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/locations/
+-rw-rw-rw-   0        0        0    15365 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/locations/__init__.py
+-rw-rw-rw-   0        0        0     6100 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/locations/_distutils.py
+-rw-rw-rw-   0        0        0     7680 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-rw-rw-   0        0        0     2556 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/locations/base.py
+-rw-rw-rw-   0        0        0      340 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/main.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.247967 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/
+-rw-rw-rw-   0        0        0     4280 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/__init__.py
+-rw-rw-rw-   0        0        0     2595 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/_json.py
+-rw-rw-rw-   0        0        0    25277 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/base.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.295480 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/
+-rw-rw-rw-   0        0        0      107 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-rw-rw-   0        0        0     1882 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-rw-rw-   0        0        0     8181 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-rw-rw-   0        0        0     7457 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-rw-rw-   0        0        0     9773 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.410268 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/
+-rw-rw-rw-   0        0        0       63 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/__init__.py
+-rw-rw-rw-   0        0        0      990 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/candidate.py
+-rw-rw-rw-   0        0        0     6626 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/direct_url.py
+-rw-rw-rw-   0        0        0     2520 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/format_control.py
+-rw-rw-rw-   0        0        0     1030 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/index.py
+-rw-rw-rw-   0        0        0     2617 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/installation_report.py
+-rw-rw-rw-   0        0        0    18602 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/link.py
+-rw-rw-rw-   0        0        0      738 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/scheme.py
+-rw-rw-rw-   0        0        0     4644 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/search_scope.py
+-rw-rw-rw-   0        0        0     1907 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
+-rw-rw-rw-   0        0        0     3858 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/target_python.py
+-rw-rw-rw-   0        0        0     3600 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/wheel.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.490791 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/
+-rw-rw-rw-   0        0        0       50 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/__init__.py
+-rw-rw-rw-   0        0        0    16507 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/auth.py
+-rw-rw-rw-   0        0        0     2145 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/cache.py
+-rw-rw-rw-   0        0        0     6096 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/download.py
+-rw-rw-rw-   0        0        0     7638 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-rw-rw-   0        0        0    18443 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/session.py
+-rw-rw-rw-   0        0        0     4073 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/utils.py
+-rw-rw-rw-   0        0        0     1791 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.522600 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.599169 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/__init__.py
+-rw-rw-rw-   0        0        0     4133 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-rw-rw-   0        0        0     1422 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py
+-rw-rw-rw-   0        0        0     1474 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-rw-rw-   0        0        0     2198 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-rw-rw-   0        0        0     1075 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py
+-rw-rw-rw-   0        0        0     1417 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-rw-rw-   0        0        0     3064 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-rw-rw-   0        0        0     5122 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/check.py
+-rw-rw-rw-   0        0        0     9784 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/freeze.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.630510 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/install/
+-rw-rw-rw-   0        0        0       51 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
+-rw-rw-rw-   0        0        0     1354 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-rw-rw-   0        0        0     4105 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py
+-rw-rw-rw-   0        0        0    27407 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
+-rw-rw-rw-   0        0        0    25091 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/prepare.py
+-rw-rw-rw-   0        0        0     6987 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/pyproject.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.708947 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/req/
+-rw-rw-rw-   0        0        0     2807 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/req/__init__.py
+-rw-rw-rw-   0        0        0    16611 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/req/constructors.py
+-rw-rw-rw-   0        0        0    17646 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/req/req_file.py
+-rw-rw-rw-   0        0        0    35763 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/req/req_install.py
+-rw-rw-rw-   0        0        0     2858 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/req/req_set.py
+-rw-rw-rw-   0        0        0    24045 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.724575 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/base.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.724575 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-rw-rw-   0        0        0    24129 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.823294 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-rw-rw-   0        0        0     5220 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-rw-rw-   0        0        0    18963 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-rw-rw-   0        0        0    27878 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-rw-rw-   0        0        0     5705 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-rw-rw-   0        0        0     9914 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-rw-rw-   0        0        0     2526 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-rw-rw-   0        0        0     5455 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-rw-rw-   0        0        0    11533 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-rw-rw-   0        0        0     8167 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/self_outdated_check.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.106217 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/__init__.py
+-rw-rw-rw-   0        0        0     1015 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/_log.py
+-rw-rw-rw-   0        0        0     1665 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/appdirs.py
+-rw-rw-rw-   0        0        0     1884 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/compat.py
+-rw-rw-rw-   0        0        0     5377 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-rw-rw-   0        0        0      242 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/datetime.py
+-rw-rw-rw-   0        0        0     5764 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/deprecation.py
+-rw-rw-rw-   0        0        0     3206 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-rw-rw-   0        0        0     1115 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py
+-rw-rw-rw-   0        0        0     2118 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/egg_link.py
+-rw-rw-rw-   0        0        0     1169 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/encoding.py
+-rw-rw-rw-   0        0        0     3064 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
+-rw-rw-rw-   0        0        0     5122 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/filesystem.py
+-rw-rw-rw-   0        0        0      716 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/filetypes.py
+-rw-rw-rw-   0        0        0     3110 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/glibc.py
+-rw-rw-rw-   0        0        0     4831 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/hashes.py
+-rw-rw-rw-   0        0        0      795 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-rw-rw-   0        0        0    11632 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/logging.py
+-rw-rw-rw-   0        0        0    22253 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/misc.py
+-rw-rw-rw-   0        0        0     1193 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/models.py
+-rw-rw-rw-   0        0        0     2108 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/packaging.py
+-rw-rw-rw-   0        0        0     5662 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-rw-rw-   0        0        0     9200 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/subprocess.py
+-rw-rw-rw-   0        0        0     7702 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
+-rw-rw-rw-   0        0        0     8821 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/unpacking.py
+-rw-rw-rw-   0        0        0     1759 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/urls.py
+-rw-rw-rw-   0        0        0     3456 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
+-rw-rw-rw-   0        0        0     4549 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/wheel.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.169236 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/vcs/
+-rw-rw-rw-   0        0        0      596 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/vcs/__init__.py
+-rw-rw-rw-   0        0        0     3519 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
+-rw-rw-rw-   0        0        0    18116 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/vcs/git.py
+-rw-rw-rw-   0        0        0     5238 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
+-rw-rw-rw-   0        0        0    11729 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/vcs/subversion.py
+-rw-rw-rw-   0        0        0    22811 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-rw-rw-   0        0        0    13079 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/wheel_builder.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.202489 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/
+-rw-rw-rw-   0        0        0     4966 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.315895 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/
+-rw-rw-rw-   0        0        0      465 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-rw-rw-   0        0        0     1379 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-rw-rw-   0        0        0     5033 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-rw-rw-   0        0        0     1535 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.348855 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/
+-rw-rw-rw-   0        0        0      242 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-rw-rw-   0        0        0     5271 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-rw-rw-   0        0        0     1033 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-rw-rw-   0        0        0      778 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-rw-rw-   0        0        0    16416 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-rw-rw-   0        0        0     3946 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-rw-rw-   0        0        0     4154 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-rw-rw-   0        0        0     7105 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-rw-rw-   0        0        0      774 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.377966 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/certifi/
+-rw-rw-rw-   0        0        0       94 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
+-rw-rw-rw-   0        0        0      255 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
+-rw-rw-rw-   0        0        0     4279 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/certifi/core.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.821486 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/
+-rw-rw-rw-   0        0        0     4797 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
+-rw-rw-rw-   0        0        0    31274 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-rw-rw-   0        0        0     1763 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-rw-rw-   0        0        0    10032 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-rw-rw-   0        0        0     3915 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-rw-rw-   0        0        0     5420 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.837614 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-rw-rw-   0        0        0     3242 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-rw-rw-   0        0        0     3732 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-rw-rw-   0        0        0      542 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-rw-rw-   0        0        0     1860 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-rw-rw-   0        0        0     1683 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/enums.py
+-rw-rw-rw-   0        0        0     4006 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
+-rw-rw-rw-   0        0        0    12176 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
+-rw-rw-rw-   0        0        0     3934 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-rw-rw-   0        0        0    13566 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-rw-rw-   0        0        0     1753 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-rw-rw-   0        0        0    36913 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-rw-rw-   0        0        0     1753 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-rw-rw-   0        0        0    20735 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-rw-rw-   0        0        0     1759 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-rw-rw-   0        0        0    14537 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-rw-rw-   0        0        0    25796 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-rw-rw-   0        0        0    42498 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-rw-rw-   0        0        0     1752 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-rw-rw-   0        0        0    27055 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-rw-rw-   0        0        0   104562 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-rw-rw-   0        0        0    98484 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-rw-rw-   0        0        0    98196 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-rw-rw-   0        0        0   101363 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-rw-rw-   0        0        0   128035 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-rw-rw-   0        0        0   102774 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-rw-rw-   0        0        0    95372 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-rw-rw-   0        0        0     5380 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-rw-rw-   0        0        0     6077 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-rw-rw-   0        0        0     3715 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-rw-rw-   0        0        0     2131 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-rw-rw-   0        0        0    30391 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.849574 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-rw-rw-   0        0        0    13560 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-rw-rw-   0        0        0      402 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-rw-rw-   0        0        0     6400 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-rw-rw-   0        0        0     4137 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-rw-rw-   0        0        0     4007 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-rw-rw-   0        0        0    14848 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-rw-rw-   0        0        0     8505 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-rw-rw-   0        0        0     2812 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-rw-rw-   0        0        0      244 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/version.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.900821 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/
+-rw-rw-rw-   0        0        0      266 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
+-rw-rw-rw-   0        0        0    11128 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-rw-rw-   0        0        0     3325 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.964020 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/
+-rw-rw-rw-   0        0        0       75 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-rw-rw-   0        0        0     2839 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-rw-rw-   0        0        0    10678 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-rw-rw-   0        0        0     6741 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-rw-rw-   0        0        0     1866 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-rw-rw-   0        0        0     1079 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-rw-rw-   0        0        0     3709 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-rw-rw-   0        0        0     6181 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/win32.py
+-rw-rw-rw-   0        0        0     7134 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.120653 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/
+-rw-rw-rw-   0        0        0      581 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
+-rw-rw-rw-   0        0        0    41259 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/compat.py
+-rw-rw-rw-   0        0        0    51697 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/database.py
+-rw-rw-rw-   0        0        0    20834 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/index.py
+-rw-rw-rw-   0        0        0    51991 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/locators.py
+-rw-rw-rw-   0        0        0    14811 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
+-rw-rw-rw-   0        0        0     5058 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/markers.py
+-rw-rw-rw-   0        0        0    39801 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
+-rw-rw-rw-   0        0        0    10820 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/resources.py
+-rw-rw-rw-   0        0        0    18102 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
+-rw-rw-rw-   0        0        0    66262 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/util.py
+-rw-rw-rw-   0        0        0    23513 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/version.py
+-rw-rw-rw-   0        0        0    43898 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.152296 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distro/
+-rw-rw-rw-   0        0        0      981 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distro/__init__.py
+-rw-rw-rw-   0        0        0       64 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distro/__main__.py
+-rw-rw-rw-   0        0        0    49330 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distro/distro.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.249930 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/
+-rw-rw-rw-   0        0        0      849 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/__init__.py
+-rw-rw-rw-   0        0        0     3374 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/codec.py
+-rw-rw-rw-   0        0        0      321 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/compat.py
+-rw-rw-rw-   0        0        0    12950 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/core.py
+-rw-rw-rw-   0        0        0    44375 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
+-rw-rw-rw-   0        0        0     1881 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/intranges.py
+-rw-rw-rw-   0        0        0       21 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/package_data.py
+-rw-rw-rw-   0        0        0   206539 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.282126 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/msgpack/
+-rw-rw-rw-   0        0        0     1132 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-rw-rw-   0        0        0     1081 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-rw-rw-   0        0        0     6080 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
+-rw-rw-rw-   0        0        0    34557 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.396538 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1431 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8487 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4676 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30110 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15699 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.427996 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/
+-rw-rw-rw-   0        0        0   108287 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-rw-rw-   0        0        0      562 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.523467 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/
+-rw-rw-rw-   0        0        0    12936 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-rw-rw-   0        0        0     1176 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-rw-rw-   0        0        0     4068 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
+-rw-rw-rw-   0        0        0     4910 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
+-rw-rw-rw-   0        0        0     2655 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-rw-rw-   0        0        0     6911 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-rw-rw-   0        0        0      160 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
+-rw-rw-rw-   0        0        0     6596 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.697254 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/
+-rw-rw-rw-   0        0        0     2999 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
+-rw-rw-rw-   0        0        0      353 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
+-rw-rw-rw-   0        0        0    23685 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-rw-rw-   0        0        0     1697 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/console.py
+-rw-rw-rw-   0        0        0     1938 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/filter.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.697254 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/filters/
+-rw-rw-rw-   0        0        0    40386 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-rw-rw-   0        0        0     2917 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.850582 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/
+-rw-rw-rw-   0        0        0     4810 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-rw-rw-   0        0        0     4104 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-rw-rw-   0        0        0     3314 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-rw-rw-   0        0        0     5086 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-rw-rw-   0        0        0    35441 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-rw-rw-   0        0        0    21938 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-rw-rw-   0        0        0     5871 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-rw-rw-   0        0        0    19351 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-rw-rw-   0        0        0     5073 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-rw-rw-   0        0        0     2212 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-rw-rw-   0        0        0     5014 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-rw-rw-   0        0        0     7335 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-rw-rw-   0        0        0     4674 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-rw-rw-   0        0        0    11753 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-rw-rw-   0        0        0    32005 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.888897 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/
+-rw-rw-rw-   0        0        0    11174 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-rw-rw-   0        0        0    70232 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-rw-rw-   0        0        0    53376 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-rw-rw-   0        0        0      986 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
+-rw-rw-rw-   0        0        0     2591 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
+-rw-rw-rw-   0        0        0     3072 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-rw-rw-   0        0        0     3092 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
+-rw-rw-rw-   0        0        0     4630 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-rw-rw-   0        0        0     6257 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/style.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.888897 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/styles/
+-rw-rw-rw-   0        0        0     3419 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-rw-rw-   0        0        0     6184 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/token.py
+-rw-rw-rw-   0        0        0    63187 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
+-rw-rw-rw-   0        0        0     9110 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/util.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:15.015125 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/
+-rw-rw-rw-   0        0        0     9171 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-rw-rw-   0        0        0     6426 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-rw-rw-   0        0        0    12936 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
+-rw-rw-rw-   0        0        0   213344 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:15.030673 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/
+-rw-rw-rw-   0        0        0    23685 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-rw-   0        0        0     9023 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-rw-rw-   0        0        0    39129 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-rw-rw-   0        0        0    25341 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
+-rw-rw-rw-   0        0        0    13402 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-rw-rw-   0        0        0    10787 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-rw-rw-   0        0        0     6805 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:15.051041 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/
+-rw-rw-rw-   0        0        0      491 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-rw-rw-   0        0        0      138 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-rw-rw-   0        0        0    11920 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:15.062621 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/
+-rw-rw-rw-   0        0        0      546 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-rw-rw-   0        0        0    10927 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:15.251459 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/
+-rw-rw-rw-   0        0        0     5178 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/__version__.py
+-rw-rw-rw-   0        0        0     1397 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-rw-rw-   0        0        0    21443 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/adapters.py
+-rw-rw-rw-   0        0        0     6377 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/api.py
+-rw-rw-rw-   0        0        0    10187 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/auth.py
+-rw-rw-rw-   0        0        0      575 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/certs.py
+-rw-rw-rw-   0        0        0     1286 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/compat.py
+-rw-rw-rw-   0        0        0    18560 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/cookies.py
+-rw-rw-rw-   0        0        0     3823 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
+-rw-rw-rw-   0        0        0     3879 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/help.py
+-rw-rw-rw-   0        0        0      733 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/hooks.py
+-rw-rw-rw-   0        0        0    35288 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/models.py
+-rw-rw-rw-   0        0        0      695 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/packages.py
+-rw-rw-rw-   0        0        0    30180 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/sessions.py
+-rw-rw-rw-   0        0        0     4235 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
+-rw-rw-rw-   0        0        0     2912 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/structures.py
+-rw-rw-rw-   0        0        0    33240 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:15.282668 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/
+-rw-rw-rw-   0        0        0      537 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:15.301380 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-rw-rw-   0        0        0     5872 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-rw-rw-   0        0        0     1583 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-rw-rw-   0        0        0    17592 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-rw-rw-   0        0        0     4794 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.052673 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/
+-rw-rw-rw-   0        0        0     6090 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/__init__.py
+-rw-rw-rw-   0        0        0     8478 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/__main__.py
+-rw-rw-rw-   0        0        0    10096 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-rw-rw-   0        0        0   140235 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-rw-rw-   0        0        0     1064 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-rw-rw-   0        0        0     2114 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
+-rw-rw-rw-   0        0        0      265 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_extension.py
+-rw-rw-rw-   0        0        0     9695 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
+-rw-rw-rw-   0        0        0     3225 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
+-rw-rw-rw-   0        0        0     1236 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_loop.py
+-rw-rw-rw-   0        0        0     1643 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_null_file.py
+-rw-rw-rw-   0        0        0     7063 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
+-rw-rw-rw-   0        0        0      423 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_pick.py
+-rw-rw-rw-   0        0        0     5472 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
+-rw-rw-rw-   0        0        0    19919 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
+-rw-rw-rw-   0        0        0      351 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_stack.py
+-rw-rw-rw-   0        0        0      417 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_timer.py
+-rw-rw-rw-   0        0        0    22820 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-rw-rw-   0        0        0     1926 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_windows.py
+-rw-rw-rw-   0        0        0     2783 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-rw-rw-   0        0        0     1840 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
+-rw-rw-rw-   0        0        0      890 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/abc.py
+-rw-rw-rw-   0        0        0    10368 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/align.py
+-rw-rw-rw-   0        0        0     6819 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/ansi.py
+-rw-rw-rw-   0        0        0     3264 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/bar.py
+-rw-rw-rw-   0        0        0     9842 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/box.py
+-rw-rw-rw-   0        0        0     4503 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/cells.py
+-rw-rw-rw-   0        0        0    18015 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/color.py
+-rw-rw-rw-   0        0        0     1054 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-rw-rw-   0        0        0     7131 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/columns.py
+-rw-rw-rw-   0        0        0    97992 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/console.py
+-rw-rw-rw-   0        0        0     1288 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/constrain.py
+-rw-rw-rw-   0        0        0     5497 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/containers.py
+-rw-rw-rw-   0        0        0     6630 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/control.py
+-rw-rw-rw-   0        0        0     7954 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
+-rw-rw-rw-   0        0        0      972 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
+-rw-rw-rw-   0        0        0     2501 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/emoji.py
+-rw-rw-rw-   0        0        0      642 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/errors.py
+-rw-rw-rw-   0        0        0     1616 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-rw-rw-   0        0        0     2508 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/filesize.py
+-rw-rw-rw-   0        0        0     9585 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
+-rw-rw-rw-   0        0        0     5053 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/json.py
+-rw-rw-rw-   0        0        0     3252 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
+-rw-rw-rw-   0        0        0    14007 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/layout.py
+-rw-rw-rw-   0        0        0    14172 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/live.py
+-rw-rw-rw-   0        0        0     3667 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/live_render.py
+-rw-rw-rw-   0        0        0    11903 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/logging.py
+-rw-rw-rw-   0        0        0     8198 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/markup.py
+-rw-rw-rw-   0        0        0     5305 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/measure.py
+-rw-rw-rw-   0        0        0     4970 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/padding.py
+-rw-rw-rw-   0        0        0      828 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/pager.py
+-rw-rw-rw-   0        0        0     3396 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/palette.py
+-rw-rw-rw-   0        0        0    10574 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/panel.py
+-rw-rw-rw-   0        0        0    37414 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/pretty.py
+-rw-rw-rw-   0        0        0    59836 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/progress.py
+-rw-rw-rw-   0        0        0     8165 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-rw-rw-   0        0        0    11303 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/prompt.py
+-rw-rw-rw-   0        0        0     1391 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/protocol.py
+-rw-rw-rw-   0        0        0      166 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/region.py
+-rw-rw-rw-   0        0        0     4436 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/repr.py
+-rw-rw-rw-   0        0        0     4773 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/rule.py
+-rw-rw-rw-   0        0        0     2843 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/scope.py
+-rw-rw-rw-   0        0        0     1591 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/screen.py
+-rw-rw-rw-   0        0        0    24224 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/segment.py
+-rw-rw-rw-   0        0        0     4374 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/spinner.py
+-rw-rw-rw-   0        0        0     4425 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/status.py
+-rw-rw-rw-   0        0        0    26332 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/style.py
+-rw-rw-rw-   0        0        0     1258 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/styled.py
+-rw-rw-rw-   0        0        0    34995 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/syntax.py
+-rw-rw-rw-   0        0        0    39684 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/table.py
+-rw-rw-rw-   0        0        0     3370 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-rw-rw-   0        0        0    45686 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/text.py
+-rw-rw-rw-   0        0        0     3627 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/theme.py
+-rw-rw-rw-   0        0        0      102 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/themes.py
+-rw-rw-rw-   0        0        0    26070 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/traceback.py
+-rw-rw-rw-   0        0        0     9169 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/tree.py
+-rw-rw-rw-   0        0        0    34549 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/six.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.138889 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/
+-rw-rw-rw-   0        0        0    18364 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-rw-rw-   0        0        0     3314 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-rw-rw-   0        0        0     1944 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-rw-rw-   0        0        0     1496 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/after.py
+-rw-rw-rw-   0        0        0     1376 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/before.py
+-rw-rw-rw-   0        0        0     1908 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-rw-rw-   0        0        0     1383 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
+-rw-rw-rw-   0        0        0     7550 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
+-rw-rw-rw-   0        0        0     2790 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
+-rw-rw-rw-   0        0        0     2145 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-rw-rw-   0        0        0     8011 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.170688 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tomli/
+-rw-rw-rw-   0        0        0      396 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
+-rw-rw-rw-   0        0        0    22633 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
+-rw-rw-rw-   0        0        0     2943 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tomli/_re.py
+-rw-rw-rw-   0        0        0      254 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tomli/_types.py
+-rw-rw-rw-   0        0        0    80114 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/typing_extensions.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.281865 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/
+-rw-rw-rw-   0        0        0     3333 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-rw-rw-   0        0        0    10811 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-rw-rw-   0        0        0       64 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
+-rw-rw-rw-   0        0        0    20070 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
+-rw-rw-rw-   0        0        0    39095 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.331805 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-rw-rw-   0        0        0      957 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.364259 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-rw-rw-   0        0        0    17632 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-rw-rw-   0        0        0    13922 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-rw-rw-   0        0        0    11036 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-rw-rw-   0        0        0     4528 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-rw-rw-   0        0        0    17081 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-rw-rw-   0        0        0    34448 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-rw-rw-   0        0        0     7097 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-rw-rw-   0        0        0     8217 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-rw-rw-   0        0        0     8579 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
+-rw-rw-rw-   0        0        0     2440 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.383790 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.383790 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-rw-rw-   0        0        0     1417 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-rw-rw-   0        0        0    34665 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-rw-rw-   0        0        0    19786 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-rw-rw-   0        0        0     5985 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/request.py
+-rw-rw-rw-   0        0        0    30641 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/response.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.525568 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/
+-rw-rw-rw-   0        0        0     1155 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-rw-rw-   0        0        0     4901 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-rw-rw-   0        0        0     1605 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-rw-rw-   0        0        0      498 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-rw-rw-   0        0        0     3997 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-rw-rw-   0        0        0     3510 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-rw-rw-   0        0        0    22003 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-rw-rw-   0        0        0    17177 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-rw-rw-   0        0        0     5758 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-rw-rw-   0        0        0     6895 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-rw-rw-   0        0        0    10003 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-rw-rw-   0        0        0    14298 2023-04-07 11:44:47.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-rw-rw-   0        0        0     5403 2023-04-07 11:44:47.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.588990 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/webencodings/
+-rw-rw-rw-   0        0        0    10579 2023-04-07 11:44:47.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-rw-rw-   0        0        0     8979 2023-04-07 11:44:47.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
+-rw-rw-rw-   0        0        0     1305 2023-04-07 11:44:47.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-rw-rw-   0        0        0     6563 2023-04-07 11:44:47.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
+-rw-rw-rw-   0        0        0     4307 2023-04-07 11:44:47.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.605334 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/
+-rw-rw-rw-   0        0        0   109315 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.620338 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.715142 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-rw-rw-   0        0        0      506 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-rw-rw-   0        0        0     4504 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-rw-rw-   0        0        0     5457 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-rw-rw-   0        0        0     2925 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-rw-rw-   0        0        0      884 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-rw-rw-   0        0        0     3481 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-rw-rw-   0        0        0     5140 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-rw-rw-   0        0        0     3581 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-rw-rw-   0        0        0     2576 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.762660 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-rw-rw-   0        0        0     7460 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py
+-rw-rw-rw-   0        0        0    13515 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.778300 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/
+-rw-rw-rw-   0        0        0    15526 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.828811 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-rw-rw-   0        0        0      148 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-rw-rw-   0        0        0   133344 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-rw-rw-   0        0        0    22975 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.955254 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/
+-rw-rw-rw-   0        0        0      501 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0     3266 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_elffile.py
+-rw-rw-rw-   0        0        0     8813 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     2524 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     9399 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_parser.py
+-rw-rw-rw-   0        0        0     1431 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     5148 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py
+-rw-rw-rw-   0        0        0     8161 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     3264 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    39046 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    18065 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4355 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    16295 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.986632 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/
+-rw-rw-rw-   0        0        0    12806 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/__init__.py
+-rw-rw-rw-   0        0        0     1164 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/__main__.py
+-rw-rw-rw-   0        0        0     4068 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/android.py
+-rw-rw-rw-   0        0        0     4910 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/api.py
+-rw-rw-rw-   0        0        0     2655 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/macos.py
+-rw-rw-rw-   0        0        0     6911 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/unix.py
+-rw-rw-rw-   0        0        0      160 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/version.py
+-rw-rw-rw-   0        0        0     6596 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/windows.py
+-rw-rw-rw-   0        0        0    80078 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/typing_extensions.py
+-rw-rw-rw-   0        0        0     8425 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:17.002940 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/extern/
+-rw-rw-rw-   0        0        0     2442 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/extern/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:17.301892 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/
+-rw-rw-rw-   0        0        0     9170 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/__init__.py
+-rw-rw-rw-   0        0        0      218 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_deprecation_warning.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:17.655795 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/
+-rw-rw-rw-   0        0        0      359 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/__init__.py
+-rw-rw-rw-   0        0        0     5300 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/_collections.py
+-rw-rw-rw-   0        0        0      411 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/_functools.py
+-rw-rw-rw-   0        0        0       43 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/_log.py
+-rw-rw-rw-   0        0        0      239 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-rw-rw-   0        0        0    19616 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-rw-rw-   0        0        0     8572 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/archive_util.py
+-rw-rw-rw-   0        0        0    14721 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-rw-rw-   0        0        0    48643 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
+-rw-rw-rw-   0        0        0    17861 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/cmd.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:17.920236 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/
+-rw-rw-rw-   0        0        0      430 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
+-rw-rw-rw-   0        0        0     1614 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-rw-rw-   0        0        0     5408 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
+-rw-rw-rw-   0        0        0     4665 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-rw-rw-   0        0        0    22013 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-rw-rw-   0        0        0     5584 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/build.py
+-rw-rw-rw-   0        0        0     7684 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-rw-rw-   0        0        0    31503 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-rw-rw-   0        0        0    16537 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
+-rw-rw-rw-   0        0        0     5604 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-rw-rw-   0        0        0     4872 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/check.py
+-rw-rw-rw-   0        0        0     2594 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/clean.py
+-rw-rw-rw-   0        0        0    13077 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/config.py
+-rw-rw-rw-   0        0        0    30153 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/install.py
+-rw-rw-rw-   0        0        0     2762 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
+-rw-rw-rw-   0        0        0     2788 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-rw-rw-   0        0        0     1180 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-rw-rw-   0        0        0     8409 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-rw-rw-   0        0        0     1932 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-rw-rw-   0        0        0      672 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-rw-rw-   0        0        0    11817 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/register.py
+-rw-rw-rw-   0        0        0    19232 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
+-rw-rw-rw-   0        0        0     7491 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/upload.py
+-rw-rw-rw-   0        0        0     4911 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/config.py
+-rw-rw-rw-   0        0        0     9397 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/core.py
+-rw-rw-rw-   0        0        0    11924 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-rw-rw-   0        0        0      139 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/debug.py
+-rw-rw-rw-   0        0        0     3414 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/dep_util.py
+-rw-rw-rw-   0        0        0     8072 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/dir_util.py
+-rw-rw-rw-   0        0        0    50174 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/dist.py
+-rw-rw-rw-   0        0        0     3589 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/errors.py
+-rw-rw-rw-   0        0        0    10270 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/extension.py
+-rw-rw-rw-   0        0        0    17899 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-rw-rw-   0        0        0     8212 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/file_util.py
+-rw-rw-rw-   0        0        0    13715 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/filelist.py
+-rw-rw-rw-   0        0        0     1201 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/log.py
+-rw-rw-rw-   0        0        0    30188 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-rw-rw-   0        0        0    23577 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-rw-rw-   0        0        0      217 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/py38compat.py
+-rw-rw-rw-   0        0        0      639 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/py39compat.py
+-rw-rw-rw-   0        0        0     3495 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/spawn.py
+-rw-rw-rw-   0        0        0    18928 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
+-rw-rw-rw-   0        0        0    12085 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/text_file.py
+-rw-rw-rw-   0        0        0    15601 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-rw-rw-   0        0        0    18099 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/util.py
+-rw-rw-rw-   0        0        0    12951 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/version.py
+-rw-rw-rw-   0        0        0     5205 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-rw-rw-   0        0        0     2282 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_entry_points.py
+-rw-rw-rw-   0        0        0     2392 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_imp.py
+-rw-rw-rw-   0        0        0     1311 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_importlib.py
+-rw-rw-rw-   0        0        0      675 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_itertools.py
+-rw-rw-rw-   0        0        0     3722 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_normalization.py
+-rw-rw-rw-   0        0        0     1056 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_path.py
+-rw-rw-rw-   0        0        0      882 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_reqs.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:17.956185 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.046759 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-rw-rw-   0        0        0    26498 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-rw-rw-   0        0        0     2454 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-rw-rw-   0        0        0      743 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-rw-rw-   0        0        0     1859 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-rw-rw-   0        0        0     2895 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-rw-rw-   0        0        0     2068 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-rw-rw-   0        0        0     1165 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-rw-rw-   0        0        0     1098 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py
+-rw-rw-rw-   0        0        0     2166 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.093020 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/
+-rw-rw-rw-   0        0        0      506 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-rw-rw-   0        0        0     4504 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-rw-rw-   0        0        0     5457 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-rw-rw-   0        0        0     2925 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-rw-rw-   0        0        0      884 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-rw-rw-   0        0        0     3481 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-rw-rw-   0        0        0     5140 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-rw-rw-   0        0        0     3581 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-rw-rw-   0        0        0     2576 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.108775 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-rw-rw-   0        0        0     7460 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py
+-rw-rw-rw-   0        0        0    13512 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.124312 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/
+-rw-rw-rw-   0        0        0    15517 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.156522 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/
+-rw-rw-rw-   0        0        0       82 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-rw-rw-   0        0        0   117959 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-rw-rw-   0        0        0    16256 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-rw-rw-   0        0        0    15130 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.234813 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/
+-rw-rw-rw-   0        0        0      501 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0     3266 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_elffile.py
+-rw-rw-rw-   0        0        0     8813 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     2524 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     9399 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_parser.py
+-rw-rw-rw-   0        0        0     1431 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     5148 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_tokenizer.py
+-rw-rw-rw-   0        0        0     8161 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     3264 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    39046 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    18065 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4355 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    16295 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.259929 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/tomli/
+-rw-rw-rw-   0        0        0      396 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-rw-rw-   0        0        0    22633 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-rw-rw-   0        0        0     2943 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-rw-rw-   0        0        0      254 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-rw-rw-   0        0        0    87149 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-rw-rw-   0        0        0     8425 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/zipp.py
+-rw-rw-rw-   0        0        0     7346 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/archive_util.py
+-rw-rw-rw-   0        0        0    19612 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/build_meta.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.527830 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/
+-rw-rw-rw-   0        0        0      396 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/__init__.py
+-rw-rw-rw-   0        0        0     2381 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/alias.py
+-rw-rw-rw-   0        0        0    16596 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/bdist_egg.py
+-rw-rw-rw-   0        0        0     1182 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/bdist_rpm.py
+-rw-rw-rw-   0        0        0     6589 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/build.py
+-rw-rw-rw-   0        0        0     4423 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/build_clib.py
+-rw-rw-rw-   0        0        0    15821 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/build_ext.py
+-rw-rw-rw-   0        0        0    14115 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/build_py.py
+-rw-rw-rw-   0        0        0     6963 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/develop.py
+-rw-rw-rw-   0        0        0     4074 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/dist_info.py
+-rw-rw-rw-   0        0        0    85662 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/easy_install.py
+-rw-rw-rw-   0        0        0    31903 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/editable_wheel.py
+-rw-rw-rw-   0        0        0    28176 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/egg_info.py
+-rw-rw-rw-   0        0        0     5163 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/install.py
+-rw-rw-rw-   0        0        0     2123 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/install_egg_info.py
+-rw-rw-rw-   0        0        0     3875 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/install_lib.py
+-rw-rw-rw-   0        0        0     2714 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/install_scripts.py
+-rw-rw-rw-   0        0        0     4946 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/py36compat.py
+-rw-rw-rw-   0        0        0      468 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/register.py
+-rw-rw-rw-   0        0        0     2128 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/rotate.py
+-rw-rw-rw-   0        0        0      658 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/saveopts.py
+-rw-rw-rw-   0        0        0     7071 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/sdist.py
+-rw-rw-rw-   0        0        0     5086 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/setopt.py
+-rw-rw-rw-   0        0        0     8102 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/test.py
+-rw-rw-rw-   0        0        0      462 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/upload.py
+-rw-rw-rw-   0        0        0     7470 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/upload_docs.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.575295 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/
+-rw-rw-rw-   0        0        0     1121 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/__init__.py
+-rw-rw-rw-   0        0        0    13816 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.657358 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/
+-rw-rw-rw-   0        0        0     1038 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-rw-rw-   0        0        0    11266 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-rw-rw-   0        0        0     1153 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-rw-rw-   0        0        0     1612 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-rw-rw-   0        0        0   274907 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-rw-rw-   0        0        0     9161 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-rw-rw-   0        0        0    16319 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/expand.py
+-rw-rw-rw-   0        0        0    19598 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py
+-rw-rw-rw-   0        0        0    25431 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/setupcfg.py
+-rw-rw-rw-   0        0        0      949 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/dep_util.py
+-rw-rw-rw-   0        0        0     5499 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/depends.py
+-rw-rw-rw-   0        0        0    21087 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/discovery.py
+-rw-rw-rw-   0        0        0    45710 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/dist.py
+-rw-rw-rw-   0        0        0     2464 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/errors.py
+-rw-rw-rw-   0        0        0     5591 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/extension.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.670677 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/extern/
+-rw-rw-rw-   0        0        0     2527 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/extern/__init__.py
+-rw-rw-rw-   0        0        0     4873 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/glob.py
+-rw-rw-rw-   0        0        0     5063 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/installer.py
+-rw-rw-rw-   0        0        0      812 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/launch.py
+-rw-rw-rw-   0        0        0     1232 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/logging.py
+-rw-rw-rw-   0        0        0     4697 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/monkey.py
+-rw-rw-rw-   0        0        0    47115 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/msvc.py
+-rw-rw-rw-   0        0        0     3093 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/namespaces.py
+-rw-rw-rw-   0        0        0    39682 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/package_index.py
+-rw-rw-rw-   0        0        0      245 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/py34compat.py
+-rw-rw-rw-   0        0        0    14348 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/sandbox.py
+-rw-rw-rw-   0        0        0      941 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/unicode_utils.py
+-rw-rw-rw-   0        0        0      134 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/version.py
+-rw-rw-rw-   0        0        0     8608 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/wheel.py
+-rw-rw-rw-   0        0        0      718 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/windows_support.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.843071 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/
+-rw-rw-rw-   0        0        0      396 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/__init__.py
+-rw-rw-rw-   0        0        0     8926 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/__main__.py
+-rw-rw-rw-   0        0        0     5255 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/colorutils.py
+-rw-rw-rw-   0        0        0      775 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.894710 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/dialogs/
+-rw-rw-rw-   0        0        0       42 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/dialogs/__init__.py
+-rw-rw-rw-   0        0        0    22700 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/dialogs/colorchooser.py
+-rw-rw-rw-   0        0        0     6885 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/dialogs/colordropper.py
+-rw-rw-rw-   0        0        0    64245 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/dialogs/dialogs.py
+-rw-rw-rw-   0        0        0   118811 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/icons.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.925957 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/localization/
+-rw-rw-rw-   0        0        0      675 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/localization/__init__.py
+-rw-rw-rw-   0        0        0     5594 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/localization/msgcat.py
+-rw-rw-rw-   0        0        0    15106 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/localization/msgs.py
+-rw-rw-rw-   0        0        0     2879 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/publisher.py
+-rw-rw-rw-   0        0        0    15839 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/scrolled.py
+-rw-rw-rw-   0        0        0   172335 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/style.py
+-rw-rw-rw-   0        0        0    92575 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/tableview.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.942245 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/themes/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/themes/__init__.py
+-rw-rw-rw-   0        0        0    11286 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/themes/standard.py
+-rw-rw-rw-   0        0        0       14 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/themes/user.py
+-rw-rw-rw-   0        0        0     8389 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/toast.py
+-rw-rw-rw-   0        0        0     5139 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/tooltip.py
+-rw-rw-rw-   0        0        0     3555 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/utility.py
+-rw-rw-rw-   0        0        0    10200 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/validation.py
+-rw-rw-rw-   0        0        0    40690 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/widgets.py
+-rw-rw-rw-   0        0        0    18186 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/window.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.957748 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkcreator/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkcreator/__init__.py
+-rw-rw-rw-   0        0        0    17276 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkcreator/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:19.020532 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/
+-rw-rw-rw-   0        0        0       59 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/__init__.py
+-rw-rw-rw-   0        0        0      455 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/__main__.py
+-rw-rw-rw-   0        0        0      746 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/_setuptools_logging.py
+-rw-rw-rw-   0        0        0    19868 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/bdist_wheel.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:19.084426 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/cli/
+-rw-rw-rw-   0        0        0     3932 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/cli/__init__.py
+-rw-rw-rw-   0        0        0     9427 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/cli/convert.py
+-rw-rw-rw-   0        0        0     4338 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/cli/pack.py
+-rw-rw-rw-   0        0        0     5124 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/cli/tags.py
+-rw-rw-rw-   0        0        0     1021 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/cli/unpack.py
+-rw-rw-rw-   0        0        0    16143 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/macosx_libfile.py
+-rw-rw-rw-   0        0        0     5889 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/metadata.py
+-rw-rw-rw-   0        0        0      621 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/util.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:19.084426 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:19.158208 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/__init__.py
+-rw-rw-rw-   0        0        0     3266 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/_elffile.py
+-rw-rw-rw-   0        0        0     8813 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     2524 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     9399 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/_parser.py
+-rw-rw-rw-   0        0        0     1431 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/_structures.py
+-rw-rw-rw-   0        0        0     5148 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/_tokenizer.py
+-rw-rw-rw-   0        0        0     8161 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/markers.py
+-rw-rw-rw-   0        0        0     3264 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/requirements.py
+-rw-rw-rw-   0        0        0    39047 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    18065 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/tags.py
+-rw-rw-rw-   0        0        0     4355 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/utils.py
+-rw-rw-rw-   0        0        0    16295 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/version.py
+-rw-rw-rw-   0        0        0     7674 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/wheelfile.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:10:19.164003 compoundwidgets-0.2.0/venv/Scripts/
+-rw-rw-rw-   0        0        0     1169 2023-04-07 11:44:20.000000 compoundwidgets-0.2.0/venv/Scripts/activate_this.py
```

### Comparing `compoundwidgets-0.1.9/LICENSE.txt` & `compoundwidgets-0.2.0/LICENSE.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 Copyright 2022 Andre Mariano
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, but not to sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `compoundwidgets-0.1.9/compoundwidgets/COMPOUND_WIDGETS.py` & `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PdfParser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,993 +1,999 @@
-import tkinter as tk
-import tkinter.ttk as ttk
-
-
-def float_only(action, value, text, max_length=None):
-    """ Checks that only float related characters are accepted as input """
-
-    permitted = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9', '.', '-']
-    if action == '1':
-        if str(max_length) != 'None':
-            if len(value) > int(max_length):
-                return False
-        if value == '.' and text == '.':
-            return False
-        elif value == '-' and text == '-':
-            return True
-        elif text in permitted:
-            try:
-                float(value)
-                return True
-            except ValueError:
-                return False
-        else:
-            return False
+import calendar
+import codecs
+import collections
+import mmap
+import os
+import re
+import time
+import zlib
+
+
+# see 7.9.2.2 Text String Type on page 86 and D.3 PDFDocEncoding Character Set
+# on page 656
+def encode_text(s):
+    return codecs.BOM_UTF16_BE + s.encode("utf_16_be")
+
+
+PDFDocEncoding = {
+    0x16: "\u0017",
+    0x18: "\u02D8",
+    0x19: "\u02C7",
+    0x1A: "\u02C6",
+    0x1B: "\u02D9",
+    0x1C: "\u02DD",
+    0x1D: "\u02DB",
+    0x1E: "\u02DA",
+    0x1F: "\u02DC",
+    0x80: "\u2022",
+    0x81: "\u2020",
+    0x82: "\u2021",
+    0x83: "\u2026",
+    0x84: "\u2014",
+    0x85: "\u2013",
+    0x86: "\u0192",
+    0x87: "\u2044",
+    0x88: "\u2039",
+    0x89: "\u203A",
+    0x8A: "\u2212",
+    0x8B: "\u2030",
+    0x8C: "\u201E",
+    0x8D: "\u201C",
+    0x8E: "\u201D",
+    0x8F: "\u2018",
+    0x90: "\u2019",
+    0x91: "\u201A",
+    0x92: "\u2122",
+    0x93: "\uFB01",
+    0x94: "\uFB02",
+    0x95: "\u0141",
+    0x96: "\u0152",
+    0x97: "\u0160",
+    0x98: "\u0178",
+    0x99: "\u017D",
+    0x9A: "\u0131",
+    0x9B: "\u0142",
+    0x9C: "\u0153",
+    0x9D: "\u0161",
+    0x9E: "\u017E",
+    0xA0: "\u20AC",
+}
+
+
+def decode_text(b):
+    if b[: len(codecs.BOM_UTF16_BE)] == codecs.BOM_UTF16_BE:
+        return b[len(codecs.BOM_UTF16_BE) :].decode("utf_16_be")
     else:
-        return True
+        return "".join(PDFDocEncoding.get(byte, chr(byte)) for byte in b)
 
 
-def max_chars(action, value, max_length):
-    """ Checks for the maximum number of characters """
-    if action == '1':
-        if len(value) > int(max_length):
-            return False
-    return True
+class PdfFormatError(RuntimeError):
+    """An error that probably indicates a syntactic or semantic error in the
+    PDF file structure"""
 
+    pass
 
-class LedButton (ttk.Frame):
-    """
-    Create a compound widget, with a color canvas (left) and a label (right).
-    The master (application top level) shall have a ttkbootstrap Style defined.
-    Input:
-        parent: container in which the widgets will be created
-        label_text: string to be shown on the label
-        label_width: width of the label im characters
-        label_method: method to bind to the label
-    Methods:
-        enable method:
-            enables the widgets (state='normal')
-        disable method:
-            disables the widgets (state='disabled')
-        select method:
-            changes the color of the canvas to the selected one
-        deselect method:
-            changes the color of the canvas to the deselected one
-    """
 
-    def __init__(self, parent, label_text='Label', label_width=10, label_method=None):
+def check_format_condition(condition, error_message):
+    if not condition:
+        raise PdfFormatError(error_message)
 
-        # Parent class initialization
-        super().__init__(parent)
-        self.label_method = label_method
-
-        # Gets the current style from the top level container
-        style = parent.winfo_toplevel().style
-
-        # Gets the active/inactive colors from the style
-        if True:
-            self.selected_color = style.colors.info
-            self.deselected_color = style.colors.fg
-            self.disable_color = style.colors.light
-
-        # Frame configuration
-        if True:
-            self.rowconfigure(0, weight=1)
-            self.columnconfigure(0, weight=0)
-            self.columnconfigure(1, weight=1)
-
-        # Canvas
-        if True:
-            self.color_canvas = tk.Canvas(self, bd=0, width=10, height=0, highlightthickness=0)
-            self.color_canvas.grid(row=0, column=0, sticky='nsew')
-            self.color_canvas.configure(background=self.deselected_color)
-
-        # Label
-        if True:
-            self.label = ttk.Label(self, text=label_text, anchor='w', style='secondary.TButton', padding=2,
-                                   width=label_width)
-            self.label.grid(row=0, column=1, sticky='nsew')
-
-        # Bind mouse button click event
-        self.color_canvas.bind('<Button-1>', self.select)
-        self.label.bind('<Button-1>', self.select)
-        self.color_canvas.bind('<ButtonRelease-1>', self.check_hover)
-        self.label.bind('<ButtonRelease-1>', self.check_hover)
 
-    def check_hover(self, event):
-        """ Checks whether the mouse is still over the widget before calling the assigned method """
+class IndirectReference(
+    collections.namedtuple("IndirectReferenceTuple", ["object_id", "generation"])
+):
+    def __str__(self):
+        return "%s %s R" % self
 
-        if str(self.label.cget('state')) == 'disabled':
-            return
+    def __bytes__(self):
+        return self.__str__().encode("us-ascii")
 
-        self.deselect()
-        current_widget = event.widget.winfo_containing(event.x_root, event.y_root)
-        if current_widget == event.widget:
-            self.label_method(event)
-
-    def enable(self):
-        self.color_canvas.config(bg=self.deselected_color)
-        self.label.config(state='normal')
-
-    def disable(self):
-        self.color_canvas.config(bg=self.disable_color)
-        self.label.config(state='disabled')
+    def __eq__(self, other):
+        return (
+            other.__class__ is self.__class__
+            and other.object_id == self.object_id
+            and other.generation == self.generation
+        )
 
-    def select(self, event=None):
-        if str(self.label.cget('state')) == 'disabled':
-            return
-        self.color_canvas.config(bg=self.selected_color)
-        self.label.config(style='primary.TButton')
+    def __ne__(self, other):
+        return not (self == other)
 
-    def deselect(self, event=None):
-        if str(self.label.cget('state')) == 'disabled':
-            return
-        self.color_canvas.config(bg=self.deselected_color)
-        self.label.config(style='secondary.TButton')
-
-
-class CheckLedButton (ttk.Frame):
-    """
-    Create a compound widget, with a color canvas (left) and a label (right).
-    The master (application top level) shall have a ttkbootstrap Style defined.
-    This button remains ON until once again selected
-    Input:
-        parent: container in which the widgets will be created
-        label_text: string to be shown on the label
-        label_width: width of the label im characters
-        label_method: method to bind to the label
-    Methods:
-        enable method:
-            enables the widgets (state='normal')
-        disable method:
-            disables the widgets (state='disabled')
-        select method:
-            changes the color of the canvas to the selected one
-        deselect method:
-            changes the color of the canvas to the deselected one
-        is_selected:
-            checks whether the button is currently selected
-    """
-
-    def __init__(self, parent, label_text='Label', label_width=10, label_method=None):
-
-        # Parent class initialization
-        super().__init__(parent)
-        self.label_method = label_method
-
-        # Gets the current style from the top level container
-        style = parent.winfo_toplevel().style
-
-        # Gets the active/inactive colors from the style
-        if True:
-            self.selected_color = style.colors.info
-            self.deselected_color = style.colors.fg
-            self.disable_color = style.colors.light
-            self.bg_color = style.colors.secondary
-
-        # Frame configuration
-        if True:
-            self.rowconfigure(0, weight=1)
-            self.columnconfigure(0, weight=0)
-            self.columnconfigure(1, weight=0)
-            self.columnconfigure(2, weight=1)
-
-        # Canvas
-        if True:
-            self.color_canvas_1 = tk.Canvas(self, bd=0, width=10, height=0, highlightthickness=0)
-            self.color_canvas_1.grid(row=0, column=0, sticky='nsew', padx=(1, 0))
-            self.color_canvas_1.configure(background=self.deselected_color)
-
-            self.color_canvas_2 = tk.Canvas(self, bd=0, width=10, height=0, highlightthickness=0)
-            self.color_canvas_2.grid(row=0, column=1, sticky='nsew', padx=(0, 1))
-            self.color_canvas_2.configure(background=self.bg_color)
-
-        # Label
-        if True:
-            self.label = ttk.Label(self, text=label_text, anchor='w', style='secondary.TButton', padding=2,
-                                   width=label_width)
-            self.label.grid(row=0, column=2, sticky='nsew')
-
-        # Bind method
-        self.color_canvas_1.bind('<ButtonRelease-1>', self.check_hover)
-        self.color_canvas_2.bind('<ButtonRelease-1>', self.check_hover)
-        self.label.bind('<ButtonRelease-1>', self.check_hover)
-
-    def check_hover(self, event):
-        """ Checks whether the mouse is still over the widget before releasing the assigned method """
-
-        if str(self.label.cget('state')) == 'disabled':
-            return
+    def __hash__(self):
+        return hash((self.object_id, self.generation))
 
-        widget_under_cursor = event.widget.winfo_containing(event.x_root, event.y_root)
 
-        if widget_under_cursor in (self.color_canvas_1, self.color_canvas_2, self.label):
-            if self.is_selected():
-                self.deselect()
-            else:
-                self.select()
-                self.label_method(event)
+class IndirectObjectDef(IndirectReference):
+    def __str__(self):
+        return "%s %s obj" % self
 
-    def enable(self):
-        self.color_canvas_1.config(bg=self.deselected_color)
-        self.color_canvas_2.config(bg=self.bg_color)
-        self.label.config(state='normal')
-
-    def disable(self):
-        self.color_canvas_1.config(bg=self.disable_color)
-        self.color_canvas_2.config(bg=self.bg_color)
-        self.label.config(state='disabled')
 
-    def select(self):
-        if str(self.label.cget('state')) == 'disabled':
-            return
-        self.color_canvas_1.config(bg=self.bg_color)
-        self.color_canvas_2.config(bg=self.selected_color)
-        self.label.config(style='primary.TButton')
+class XrefTable:
+    def __init__(self):
+        self.existing_entries = {}  # object ID => (offset, generation)
+        self.new_entries = {}  # object ID => (offset, generation)
+        self.deleted_entries = {0: 65536}  # object ID => generation
+        self.reading_finished = False
 
-    def deselect(self):
-        if str(self.label.cget('state')) == 'disabled':
-            return
-        self.color_canvas_1.config(bg=self.deselected_color)
-        self.color_canvas_2.config(bg=self.bg_color)
-        self.label.config(style='secondary.TButton')
-
-    def is_selected(self):
-        if self.color_canvas_2.cget('bg') == self.selected_color:
-            return True
+    def __setitem__(self, key, value):
+        if self.reading_finished:
+            self.new_entries[key] = value
         else:
-            return False
-
-
-class RadioLedButton(ttk.Frame):
-    """
-    Create a compound widget, with a color canvas and a label.
-    The set of instance with the same control variable will work as radio buttons.
-    Input:
-        parent: container in which the widgets will be created
-        label_text: string to be shown on the label
-        label_width: width of the label im characters
-        label_method: method to bind to the label
-        control_variable: variable that will group the buttons for "radio button" like operation
-    Methods:
-        enable method:
-            enables the widgets (state='normal')
-        disable method:
-            disables the widgets (state='disabled')
-        select method:
-            changes the color of the canvas to the selected one
-        deselect method:
-            changes the color of the canvas to the deselected one
-        is_selected:
-            checks whether the button is currently selected
-    """
-
-    control_variable_dict = {}
-
-    def __init__(self, parent, label_text='Label', label_width=10, label_method=None, control_variable=None):
-
-        super().__init__(parent)
-        self.label_method = label_method
-        self.control_variable = control_variable
-
-        if control_variable in RadioLedButton.control_variable_dict:
-            RadioLedButton.control_variable_dict[control_variable].append(self)
+            self.existing_entries[key] = value
+        if key in self.deleted_entries:
+            del self.deleted_entries[key]
+
+    def __getitem__(self, key):
+        try:
+            return self.new_entries[key]
+        except KeyError:
+            return self.existing_entries[key]
+
+    def __delitem__(self, key):
+        if key in self.new_entries:
+            generation = self.new_entries[key][1] + 1
+            del self.new_entries[key]
+            self.deleted_entries[key] = generation
+        elif key in self.existing_entries:
+            generation = self.existing_entries[key][1] + 1
+            self.deleted_entries[key] = generation
+        elif key in self.deleted_entries:
+            generation = self.deleted_entries[key]
         else:
-            RadioLedButton.control_variable_dict[control_variable] = [self]
-
-        # Gets the current style from the top level container
-        style = parent.winfo_toplevel().style
-
-        # Gets the active/inactive colors from the style
-        if True:
-            self.selected_color = style.colors.info
-            self.deselected_color = style.colors.fg
-            self.disabled_color = style.colors.light
-
-        # Frame configuration
-        if True:
-            self.rowconfigure(0, weight=1)
-            self.columnconfigure(0, weight=0)
-            self.columnconfigure(1, weight=1)
-
-        # Canvas
-        if True:
-            self.color_canvas = tk.Canvas(self, bd=0, width=10, height=0, highlightthickness=0)
-            self.color_canvas.grid(row=0, column=0, sticky='nsew')
-            self.color_canvas.configure(background=self.deselected_color)
-
-        # Label
-        if True:
-            self.label = ttk.Label(self, text=label_text, anchor='w', justify='left', style='secondary.TButton',
-                                   padding=1, width=label_width)
-            self.label.grid(row=0, column=1, sticky='nsew')
-
-        self.color_canvas.bind('<ButtonRelease-1>', self.check_hover)
-        self.label.bind('<ButtonRelease-1>', self.check_hover)
-
-    def check_hover(self, event):
-        if str(self.label.cget('state')) == 'disabled':
-            return
-
-        widget_under_cursor = event.widget.winfo_containing(event.x_root, event.y_root)
-        if widget_under_cursor not in (self.color_canvas, self.label):
-            return
-
-        for widget in list(self.control_variable_dict[self.control_variable]):
-            if str(widget) == str(event.widget.winfo_parent()):
-                widget.select()
-                self.label_method(event)
+            msg = (
+                "object ID " + str(key) + " cannot be deleted because it doesn't exist"
+            )
+            raise IndexError(msg)
+
+    def __contains__(self, key):
+        return key in self.existing_entries or key in self.new_entries
+
+    def __len__(self):
+        return len(
+            set(self.existing_entries.keys())
+            | set(self.new_entries.keys())
+            | set(self.deleted_entries.keys())
+        )
+
+    def keys(self):
+        return (
+            set(self.existing_entries.keys()) - set(self.deleted_entries.keys())
+        ) | set(self.new_entries.keys())
+
+    def write(self, f):
+        keys = sorted(set(self.new_entries.keys()) | set(self.deleted_entries.keys()))
+        deleted_keys = sorted(set(self.deleted_entries.keys()))
+        startxref = f.tell()
+        f.write(b"xref\n")
+        while keys:
+            # find a contiguous sequence of object IDs
+            prev = None
+            for index, key in enumerate(keys):
+                if prev is None or prev + 1 == key:
+                    prev = key
+                else:
+                    contiguous_keys = keys[:index]
+                    keys = keys[index:]
+                    break
             else:
-                widget.deselect()
-
-    def select(self):
-        self.color_canvas.config(bg=self.selected_color)
-        self.label.config(style='primary.TButton')
-
-    def deselect(self):
-        self.color_canvas.config(bg=self.deselected_color)
-        self.label.config(style='secondary.TButton')
-
-    def enable(self):
-        self.color_canvas.config(bg=self.deselected_color)
-        self.label.config(state='normal')
-
-    def disable(self):
-        self.color_canvas.config(bg=self.disabled_color)
-        self.label.config(state='disabled')
-
-    def is_selected(self):
-        if self.color_canvas.cget('bg') == self.selected_color:
-            return True
-        return False
-
-
-class LabelEntryUnit (ttk.Frame):
-    """
-    Creates a compound widget, with a label, an entry field, and a combobox with applicable units (metric and imperial).
-    Input:
-        parent: container in which the widgets will be created
-        label_text: string to be shown on the label
-        label_anchor: position of the text within the label
-        label_width: width of the label in characters
-        entry_value: initial value to show at the entry (if any)
-        entry_numeric: whether the entry accepts only numbers
-        entry_width: entry width in number of characters
-        entry_method: method to associate when the entry events
-        entry_max_char: maximum number of characters in the entry field
-        combobox_unit: unit system for the entry
-        combobox_unit_width: width of the combobox in characters
-    Methods:
-        enable method:
-            enables the widgets (state='normal')
-        disable method:
-            disables the widgets (state='disabled')
-        read_only method:
-            disabled edition of the entry widget (state='readonly')
-        get_entry method:
-            gets the value from the entry widget
-        set_entry method:
-            sets the value to the entry widget
-        get_unit method:
-            gets the value from the unit widget
-        set_unit method:
-            sets the value from the unit widget
-        get_metric_value:
-            gets the value from the entry widget already converted for the metric (SI) unit
-    """
-
-    class TemperatureCombo(ttk.Combobox):
-        def __init__(self, parent, width):
-            super().__init__(parent)
-
-            self.values = ('°C', '°F')
-            self.variable = tk.StringVar(value=self.values[0])
-            self.configure(textvariable=self.variable, justify='center', width=width, values=self.values,
-                           state='readonly')
-
-        def get(self):
-            return self.variable.get()
-
-        def set(self, value):
-            if value in self.values:
-                self.variable.set(value)
-
-    class LengthCombo(ttk.Combobox):
-        def __init__(self, parent, width):
-            super().__init__(parent)
-
-            self.values = ('mm', 'in')
-            self.conversion_values = (1, 25.4)
-
-            self.variable = tk.StringVar(value=self.values[0])
-            self.configure(textvariable=self.variable, justify='center', width=width, values=self.values,
-                           state='readonly')
-
-        def get(self):
-            return self.variable.get()
-
-        def set(self, value):
-            self.variable.set(value)
-
-    class PressureCombo(ttk.Combobox):
-        def __init__(self, parent, width):
-            super().__init__(parent)
-
-            self.values = ('MPa', 'kgf/cm²', 'psi', 'bar', 'kPa', 'ksi')
-            self.conversion_values = (1, 0.0980665, 0.006894757, 0.1, 0.001, 6.894757)
-            self.variable = tk.StringVar(value=self.values[0])
-            self.configure(textvariable=self.variable, justify='center', width=width, values=self.values,
-                           state='readonly')
-
-        def get(self):
-            return self.variable.get()
-
-        def set(self, value):
-            if value in self.values:
-                self.variable.set(value)
-
-    class StressCombo(ttk.Combobox):
-        def __init__(self, parent, width):
-            super().__init__(parent)
-
-            self.values = ('MPa', 'GPa', 'psi', 'ksi')
-            self.conversion_values = (1, 1000, 0.006894757, 6.894757)
-            self.variable = tk.StringVar(value=self.values[0])
-            self.configure(textvariable=self.variable, justify='center', width=width, values=self.values,
-                           state='readonly')
-
-        def get(self):
-            return self.variable.get()
-
-        def set(self, value):
-            self.variable.set(value)
-
-    class ForceCombo(ttk.Combobox):
-        def __init__(self, parent, width):
-            super().__init__(parent)
-
-            self.values = ('N', 'kgf', 'lbf')
-            self.conversion_values = (1, 9.80665, 4.448222)
-            self.variable = tk.StringVar(value=self.values[0])
-            self.configure(textvariable=self.variable, justify='center', width=width, values=self.values,
-                           state='readonly')
-
-        def get(self):
-            return self.variable.get()
-
-        def set(self, value):
-            self.variable.set(value)
-
-    class MomentCombo(ttk.Combobox):
-        def __init__(self, parent, width):
-            super().__init__(parent)
-
-            self.values = ('N.m', 'kgf.m', 'lbf.ft')
-            self.conversion_values = (1, 9.80665, 1.35582)
-            self.variable = tk.StringVar(value=self.values[0])
-            self.configure(textvariable=self.variable, justify='center', width=width, values=self.values,
-                           state='readonly')
-
-    class NoUnitCombo(ttk.Combobox):
-        def __init__(self, parent, width):
-            super().__init__(parent)
-
-            self.values = ('-',)
-            self.variable = tk.StringVar(value='-')
-            self.configure(textvariable=self.variable, justify='center', width=width, values=self.values,
-                           state='readonly')
-
-        def get(self):
-            return self.variable.get()
-
-        def set(self, value):
-            self.variable.set(value)
-
-    unit_dict = {
-        'temperature': TemperatureCombo,
-        'length': LengthCombo,
-        'pressure': PressureCombo,
-        'stress': StressCombo,
-        'force': ForceCombo,
-        'moment': MomentCombo,
-        'none': NoUnitCombo
-    }
-
-    def __init__(self, parent,
-                 label_text='Label:',
-                 label_anchor='e',
-                 label_width=30,
-                 entry_value='',
-                 entry_numeric=False,
-                 entry_width=10,
-                 entry_max_char=None,
-                 entry_method=None,
-                 combobox_unit=None,
-                 combobox_unit_width=8
-                 ):
-
-        # Parent class initialization
-        super().__init__(parent)
-
-        # Entry validation for numbers
-        validate_numbers = self.register(float_only)
-
-        # Frame configuration
-        if True:
-            self.rowconfigure(0, weight=1)
-            self.columnconfigure(0, weight=1)
-            self.columnconfigure(1, weight=0)
-            self.columnconfigure(2, weight=0)
-
-        # Label
-        if True:
-            self.label = ttk.Label(self, text=label_text, anchor=label_anchor, width=label_width)
-            self.label.grid(row=0, column=0, sticky='ew', padx=2)
-
-        # Entry
-        if True:
-            self.variable = tk.StringVar(value=entry_value)
-            self.entry = ttk.Entry(self, textvariable=self.variable, justify='center', width=entry_width)
-            self.entry.grid(row=0, column=1, sticky='ew', padx=2)
-
-        # Restrict numeric values
-        if entry_numeric:
-            self.entry.config(validate='all', validatecommand=(validate_numbers, '%d', '%P', '%S'))
-
-        # Restrict maximum number of characters
-        if entry_max_char:
-            self.entry_max_char = entry_max_char
-            self.entry.bind('<Key>', self.check_length)
-
-        # Unit Combobox
-        if True:
-            if not combobox_unit:
-                combobox_unit = 'none'
-
-            local_class = LabelEntryUnit.unit_dict.get(combobox_unit.lower(), None)
-            if not local_class:
-                raise Exception('Unit not found in current units dictionary.')
-
-            self.unit_combo = local_class(self, combobox_unit_width)
-            self.unit_combo.grid(row=0, column=2, sticky='ew', padx=2)
-
-        # Bind method
-        if True:
-            self.entry.bind("<Return>", entry_method)
-            self.entry.bind("<FocusOut>", entry_method)
-            self.unit_combo.bind("<<ComboboxSelected>>", entry_method)
-
-    def enable(self):
-        self.label.config(style='TLabel')
-        self.entry.config(state='normal')
-        self.unit_combo.config(state='readonly', values=self.unit_combo.values)
-
-    def disable(self):
-        self.label.config(style='secondary.TLabel')
-        self.entry.config(state='disabled')
-        self.unit_combo.config(state='disabled')
-
-    def readonly(self):
-        self.label.config(style='TLabel')
-        self.entry.config(state='readonly')
-        self.unit_combo.config(state='readonly', values=[])
-
-    def get_entry(self):
-        return self.variable.get() or 0
-
-    def set_entry(self, value):
-        self.variable.set(value)
-
-    def get_unit(self):
-        return self.unit_combo.get()
-
-    def set_unit(self, value):
-        self.unit_combo.set(value)
-
-    def get(self):
-        return self.get_entry(), self.get_unit()
-
-    def set(self, value, unit):
-        self.variable.set(value)
-        if unit in list(self.unit_combo.values):
-            self.set_entry(value)
-            self.set_unit(unit)
+                contiguous_keys = keys
+                keys = None
+            f.write(b"%d %d\n" % (contiguous_keys[0], len(contiguous_keys)))
+            for object_id in contiguous_keys:
+                if object_id in self.new_entries:
+                    f.write(b"%010d %05d n \n" % self.new_entries[object_id])
+                else:
+                    this_deleted_object_id = deleted_keys.pop(0)
+                    check_format_condition(
+                        object_id == this_deleted_object_id,
+                        f"expected the next deleted object ID to be {object_id}, "
+                        f"instead found {this_deleted_object_id}",
+                    )
+                    try:
+                        next_in_linked_list = deleted_keys[0]
+                    except IndexError:
+                        next_in_linked_list = 0
+                    f.write(
+                        b"%010d %05d f \n"
+                        % (next_in_linked_list, self.deleted_entries[object_id])
+                    )
+        return startxref
+
+
+class PdfName:
+    def __init__(self, name):
+        if isinstance(name, PdfName):
+            self.name = name.name
+        elif isinstance(name, bytes):
+            self.name = name
         else:
-            raise Exception('Unit not found in current units dictionary.')
-
-    def get_metric_value(self):
+            self.name = name.encode("us-ascii")
 
-        if isinstance(self.unit_combo, LabelEntryUnit.NoUnitCombo):
-            return self.get_entry(), '-'
+    def name_as_str(self):
+        return self.name.decode("us-ascii")
 
-        if isinstance(self.unit_combo, LabelEntryUnit.TemperatureCombo):
-            if str(self.unit_combo.get()) == '°F':
-                return 5 * (float(self.get_entry()) - 32) / 9, self.unit_combo.values[0]
-            return self.get_entry(), self.unit_combo.values[0]
+    def __eq__(self, other):
+        return (
+            isinstance(other, PdfName) and other.name == self.name
+        ) or other == self.name
 
-        index = self.unit_combo.values.index(self.get_unit())
-        return float(self.get_entry()) * self.unit_combo.conversion_values[index], self.unit_combo.values[0]
+    def __hash__(self):
+        return hash(self.name)
 
-    def check_length(self, event):
-        current = self.get_entry()
-        if len(current) >= self.entry_max_char:
-            self.set_entry(current[:int(self.entry_max_char)])
+    def __repr__(self):
+        return f"PdfName({repr(self.name)})"
 
+    @classmethod
+    def from_pdf_stream(cls, data):
+        return cls(PdfParser.interpret_name(data))
 
-class LabelCombo (ttk.Frame):
-    """
-    Create a compound widget, with a label and a combo box within a ttk Frame.
-    Input:
-        parent - container in which the widgets will be created
-        label_text - string to be shown on the label
-        label_anchor - position of the text within the label
-        label_width: label width in number of characters
-        combo_value - initial value to show at the combo box (if any)
-        combo_list - list of values to be shown at the combo box
-        combo_width: combo box width in number of characters
-        combo_method: method to associate when combo box is selected
-    Methods:
-        enable method:
-            enables the widgets (state='normal')
-        disable method:
-            disables the widgets (state='disabled')
-        get method:
-            gets the value from the combo box widget
-        set method:
-            sets the value to the combo box widget
-    """
+    allowed_chars = set(range(33, 127)) - {ord(c) for c in "#%/()<>[]{}"}
 
-    def __init__(self, parent,
-                 label_text='Label:',
-                 label_anchor='e',
-                 label_width=10,
-                 combo_value='',
-                 combo_list=('No values informed',),
-                 combo_width=20,
-                 combo_method=None):
-
-        # Parent class initialization
-        super().__init__(parent)
-
-        # Frame configuration
-        if True:
-            self.rowconfigure(0, weight=1)
-            self.columnconfigure(0, weight=1)
-            self.columnconfigure(1, weight=0)
-
-        # Label configuration
-        if True:
-            self.label = ttk.Label(self, text=label_text, anchor=label_anchor, width=label_width)
-            self.label.grid(row=0, column=0, sticky='ew', padx=2)
-
-        # Combo box configuration
-        if True:
-            self.combo_list = combo_list
-            self.variable = tk.StringVar(value=combo_value)
-            self.combobox = ttk.Combobox(self, textvariable=self.variable, justify='center', width=combo_width,
-                                         values=combo_list, state='readonly')
-            self.combobox.grid(row=0, column=1, sticky='ew', padx=2)
-
-        # Bind method
-        if True:
-            self.combobox.bind('<<ComboboxSelected>>', combo_method)
-
-    def enable(self):
-        self.label.config(style='TLabel')
-        self.combobox.config(state='readonly', values=self.combo_list)
-
-    def disable(self):
-        self.label.config(style='secondary.TLabel')
-        self.combobox.config(state='disabled')
-
-    def readonly(self):
-        self.label.config(style='TLabel')
-        self.combobox.config(state='readonly', values=[])
-
-    def get(self):
-        return self.variable.get()
+    def __bytes__(self):
+        result = bytearray(b"/")
+        for b in self.name:
+            if b in self.allowed_chars:
+                result.append(b)
+            else:
+                result.extend(b"#%02X" % b)
+        return bytes(result)
 
-    def set(self, value):
-        self.variable.set(value)
 
+class PdfArray(list):
+    def __bytes__(self):
+        return b"[ " + b" ".join(pdf_repr(x) for x in self) + b" ]"
 
-class LabelEntry (ttk.Frame):
-    """
-    Create a compound widget, with a label and an entry field.
-    Input:
-        parent: container in which the widgets will be created
-        label_text: string to be shown on the label
-        label_anchor - position of the text within the label
-        label_width: label width in number of characters
-        entry_value: initial value to show at the entry (if any)
-        entry_numeric: whether the entry accepts only numbers
-        entry_width: entry width in number of characters
-        entry_method: method to associate when the entry events
-        entry_max_char: maximum number of characters in the entry field
-    Methods:
-        enable method:
-            enables the widgets (state='normal')
-        disable method:
-            disables the widgets (state='disabled')
-        read_only method:
-            disabled edition of the entry widget (state='readonly')
-        get method:
-            gets the value from the entry widget
-        set method:
-            sets the value to the entry widget
-    """
 
-    def __init__(self, parent,
-                 label_text='label:',
-                 label_anchor='e',
-                 entry_value='',
-                 label_width=10,
-                 entry_numeric=False,
-                 entry_width=20,
-                 entry_max_char=None,
-                 entry_method=None):
-
-        # Parent class initialization
-        super().__init__(parent)
-
-        # Entry validation for numbers
-        validate_numbers = self.register(float_only)
-        validate_chars = self.register(max_chars)
-
-        # Frame configuration
-        if True:
-            self.rowconfigure(0, weight=1)
-            self.columnconfigure(0, weight=1)
-            self.columnconfigure(1, weight=0)
-
-        # Label
-        if True:
-            self.label = ttk.Label(self, text=label_text, anchor=label_anchor, width=label_width)
-            self.label.grid(row=0, column=0, sticky='ew', padx=2)
-
-        # Entry
-        if True:
-            self.variable = tk.StringVar(value=entry_value)
-            self.entry = ttk.Entry(self, textvariable=self.variable, justify='center', width=entry_width)
-            self.entry.grid(row=0, column=1, sticky='ew', padx=2)
-
-        # Restrict numeric values
-        if entry_numeric:
-            self.entry.config(validate='all', validatecommand=(validate_numbers, '%d', '%P', '%S', entry_max_char))
-
-        # Restrict max characters
-        elif entry_max_char:
-            self.entry.config(validate='all', validatecommand=(validate_chars, '%d', '%P', entry_max_char))
-
-        # Bind method
-        if True:
-            self.entry.bind("<Return>", entry_method)
-            self.entry.bind("<FocusOut>", entry_method)
-
-    def enable(self):
-        self.label.config(style='TLabel')
-        self.entry.config(state='normal')
-
-    def disable(self):
-        self.label.config(style='secondary.TLabel')
-        self.entry.config(state='disabled')
-
-    def readonly(self):
-        self.label.config(style='TLabel')
-        self.entry.config(state='readonly')
-
-    def get(self):
-        return self.variable.get()
+class PdfDict(collections.UserDict):
+    def __setattr__(self, key, value):
+        if key == "data":
+            collections.UserDict.__setattr__(self, key, value)
+        else:
+            self[key.encode("us-ascii")] = value
 
-    def set(self, value):
-        self.variable.set(value)
+    def __getattr__(self, key):
+        try:
+            value = self[key.encode("us-ascii")]
+        except KeyError as e:
+            raise AttributeError(key) from e
+        if isinstance(value, bytes):
+            value = decode_text(value)
+        if key.endswith("Date"):
+            if value.startswith("D:"):
+                value = value[2:]
+
+            relationship = "Z"
+            if len(value) > 17:
+                relationship = value[14]
+                offset = int(value[15:17]) * 60
+                if len(value) > 20:
+                    offset += int(value[18:20])
+
+            format = "%Y%m%d%H%M%S"[: len(value) - 2]
+            value = time.strptime(value[: len(format) + 2], format)
+            if relationship in ["+", "-"]:
+                offset *= 60
+                if relationship == "+":
+                    offset *= -1
+                value = time.gmtime(calendar.timegm(value) + offset)
+        return value
+
+    def __bytes__(self):
+        out = bytearray(b"<<")
+        for key, value in self.items():
+            if value is None:
+                continue
+            value = pdf_repr(value)
+            out.extend(b"\n")
+            out.extend(bytes(PdfName(key)))
+            out.extend(b" ")
+            out.extend(value)
+        out.extend(b"\n>>")
+        return bytes(out)
+
+
+class PdfBinary:
+    def __init__(self, data):
+        self.data = data
+
+    def __bytes__(self):
+        return b"<%s>" % b"".join(b"%02X" % b for b in self.data)
+
+
+class PdfStream:
+    def __init__(self, dictionary, buf):
+        self.dictionary = dictionary
+        self.buf = buf
+
+    def decode(self):
+        try:
+            filter = self.dictionary.Filter
+        except AttributeError:
+            return self.buf
+        if filter == b"FlateDecode":
+            try:
+                expected_length = self.dictionary.DL
+            except AttributeError:
+                expected_length = self.dictionary.Length
+            return zlib.decompress(self.buf, bufsize=int(expected_length))
+        else:
+            msg = f"stream filter {repr(self.dictionary.Filter)} unknown/unsupported"
+            raise NotImplementedError(msg)
 
 
-class LabelText (ttk.Frame):
-    """
-    Create a compound widget, with a label and a text field.
-    Input:
-        parent: container in which the widgets will be created
-        label_text: string to be shown on the label
-        label_width: label width in number of characters
-        label_anchor: position of the text within the label
-        text_value: initial value to show at the text (if any)
-        text_width: text width in number of characters
-        text_method: method to associate when the text events
-    Methods:
-        enable method:
-            enables the widgets (state='normal')
-        disable method:
-            disables the widgets (state='disabled')
-        get method:
-            gets the value from the entry widget
-        set method:
-            sets the value to the entry widget
-    """
+def pdf_repr(x):
+    if x is True:
+        return b"true"
+    elif x is False:
+        return b"false"
+    elif x is None:
+        return b"null"
+    elif isinstance(x, (PdfName, PdfDict, PdfArray, PdfBinary)):
+        return bytes(x)
+    elif isinstance(x, (int, float)):
+        return str(x).encode("us-ascii")
+    elif isinstance(x, time.struct_time):
+        return b"(D:" + time.strftime("%Y%m%d%H%M%SZ", x).encode("us-ascii") + b")"
+    elif isinstance(x, dict):
+        return bytes(PdfDict(x))
+    elif isinstance(x, list):
+        return bytes(PdfArray(x))
+    elif isinstance(x, str):
+        return pdf_repr(encode_text(x))
+    elif isinstance(x, bytes):
+        # XXX escape more chars? handle binary garbage
+        x = x.replace(b"\\", b"\\\\")
+        x = x.replace(b"(", b"\\(")
+        x = x.replace(b")", b"\\)")
+        return b"(" + x + b")"
+    else:
+        return bytes(x)
 
-    def __init__(self, parent,
-                 label_text='label:',
-                 label_anchor='e',
-                 label_width=20,
-                 text_value='',
-                 text_width=20,
-                 text_height=3,
-                 text_method=None):
-
-        # Parent class initialization
-        super().__init__(parent)
-
-        # Frame configuration
-        if True:
-            self.rowconfigure(0, weight=1)
-            self.columnconfigure(0, weight=0)
-            self.columnconfigure(1, weight=1)
-            self.columnconfigure(2, weight=0)
-
-        # Label
-        if True:
-            self.label = ttk.Label(self, text=label_text, anchor=label_anchor, width=label_width)
-            self.label.grid(row=0, column=0, sticky='ne', padx=2, pady=2)
-
-        # Text
-        if True:
-            self.text = tk.Text(self, width=text_width, height=text_height, wrap=tk.WORD)
-            self.disabled_color = parent.winfo_toplevel().style.colors.secondary
-            self.enabled_color = self.text.cget('fg')
-            self.text.grid(row=0, column=1, sticky='nsew', padx=2, pady=2)
-            self.set(text_value)
-
-        # Scroll bar
-        if True:
-            y_scroll = ttk.Scrollbar(self, orient='vertical', command=self.text.yview)
-            y_scroll.grid(row=0, column=2, sticky='ns')
-            self.text.configure(yscrollcommand=y_scroll.set)
-            self.text.bind('<MouseWheel>', self.on_mouse_wheel)
-            y_scroll.bind('<MouseWheel>', self.on_mouse_wheel)
-
-        # Bind method
-        if True:
-            self.text.bind("<Return>", text_method)
-            self.text.bind("<FocusOut>", text_method)
-
-    def on_mouse_wheel(self, event):
-        self.text.yview_scroll(int(-1 * event.delta / 120), 'units')
-
-    def enable(self):
-        self.label.config(style='TLabel')
-        self.text.config(state='normal')
-        self.text.config(fg=self.enabled_color)
-
-    def disable(self):
-        self.label.config(style='secondary.TLabel')
-        self.text.config(state='disabled')
-        self.text.config(fg=self.disabled_color)
-
-    def readonly(self):
-        self.label.config(style='TLabel')
-        self.text.config(state='disabled')
-        self.text.config(fg=self.enabled_color)
-
-    def get(self):
-        return str(self.text.get('1.0', tk.END)).rstrip('\n')
-
-    def set(self, value):
-        state = self.text.cget('state')
-        self.text.config(state='normal')
-        self.text.delete('1.0', tk.END)
-        self.text.insert('1.0', value)
-        self.text.config(state=state)
 
+class PdfParser:
+    """Based on
+    https://www.adobe.com/content/dam/acom/en/devnet/acrobat/pdfs/PDF32000_2008.pdf
+    Supports PDF up to 1.4
+    """
+
+    def __init__(self, filename=None, f=None, buf=None, start_offset=0, mode="rb"):
+        if buf and f:
+            msg = "specify buf or f or filename, but not both buf and f"
+            raise RuntimeError(msg)
+        self.filename = filename
+        self.buf = buf
+        self.f = f
+        self.start_offset = start_offset
+        self.should_close_buf = False
+        self.should_close_file = False
+        if filename is not None and f is None:
+            self.f = f = open(filename, mode)
+            self.should_close_file = True
+        if f is not None:
+            self.buf = buf = self.get_buf_from_file(f)
+            self.should_close_buf = True
+            if not filename and hasattr(f, "name"):
+                self.filename = f.name
+        self.cached_objects = {}
+        if buf:
+            self.read_pdf_info()
+        else:
+            self.file_size_total = self.file_size_this = 0
+            self.root = PdfDict()
+            self.root_ref = None
+            self.info = PdfDict()
+            self.info_ref = None
+            self.page_tree_root = {}
+            self.pages = []
+            self.orig_pages = []
+            self.pages_ref = None
+            self.last_xref_section_offset = None
+            self.trailer_dict = {}
+            self.xref_table = XrefTable()
+        self.xref_table.reading_finished = True
+        if f:
+            self.seek_end()
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.close()
+        return False  # do not suppress exceptions
+
+    def start_writing(self):
+        self.close_buf()
+        self.seek_end()
+
+    def close_buf(self):
+        try:
+            self.buf.close()
+        except AttributeError:
+            pass
+        self.buf = None
+
+    def close(self):
+        if self.should_close_buf:
+            self.close_buf()
+        if self.f is not None and self.should_close_file:
+            self.f.close()
+            self.f = None
+
+    def seek_end(self):
+        self.f.seek(0, os.SEEK_END)
+
+    def write_header(self):
+        self.f.write(b"%PDF-1.4\n")
+
+    def write_comment(self, s):
+        self.f.write(f"% {s}\n".encode())
+
+    def write_catalog(self):
+        self.del_root()
+        self.root_ref = self.next_object_id(self.f.tell())
+        self.pages_ref = self.next_object_id(0)
+        self.rewrite_pages()
+        self.write_obj(self.root_ref, Type=PdfName(b"Catalog"), Pages=self.pages_ref)
+        self.write_obj(
+            self.pages_ref,
+            Type=PdfName(b"Pages"),
+            Count=len(self.pages),
+            Kids=self.pages,
+        )
+        return self.root_ref
+
+    def rewrite_pages(self):
+        pages_tree_nodes_to_delete = []
+        for i, page_ref in enumerate(self.orig_pages):
+            page_info = self.cached_objects[page_ref]
+            del self.xref_table[page_ref.object_id]
+            pages_tree_nodes_to_delete.append(page_info[PdfName(b"Parent")])
+            if page_ref not in self.pages:
+                # the page has been deleted
+                continue
+            # make dict keys into strings for passing to write_page
+            stringified_page_info = {}
+            for key, value in page_info.items():
+                # key should be a PdfName
+                stringified_page_info[key.name_as_str()] = value
+            stringified_page_info["Parent"] = self.pages_ref
+            new_page_ref = self.write_page(None, **stringified_page_info)
+            for j, cur_page_ref in enumerate(self.pages):
+                if cur_page_ref == page_ref:
+                    # replace the page reference with the new one
+                    self.pages[j] = new_page_ref
+        # delete redundant Pages tree nodes from xref table
+        for pages_tree_node_ref in pages_tree_nodes_to_delete:
+            while pages_tree_node_ref:
+                pages_tree_node = self.cached_objects[pages_tree_node_ref]
+                if pages_tree_node_ref.object_id in self.xref_table:
+                    del self.xref_table[pages_tree_node_ref.object_id]
+                pages_tree_node_ref = pages_tree_node.get(b"Parent", None)
+        self.orig_pages = []
+
+    def write_xref_and_trailer(self, new_root_ref=None):
+        if new_root_ref:
+            self.del_root()
+            self.root_ref = new_root_ref
+        if self.info:
+            self.info_ref = self.write_obj(None, self.info)
+        start_xref = self.xref_table.write(self.f)
+        num_entries = len(self.xref_table)
+        trailer_dict = {b"Root": self.root_ref, b"Size": num_entries}
+        if self.last_xref_section_offset is not None:
+            trailer_dict[b"Prev"] = self.last_xref_section_offset
+        if self.info:
+            trailer_dict[b"Info"] = self.info_ref
+        self.last_xref_section_offset = start_xref
+        self.f.write(
+            b"trailer\n"
+            + bytes(PdfDict(trailer_dict))
+            + b"\nstartxref\n%d\n%%%%EOF" % start_xref
+        )
+
+    def write_page(self, ref, *objs, **dict_obj):
+        if isinstance(ref, int):
+            ref = self.pages[ref]
+        if "Type" not in dict_obj:
+            dict_obj["Type"] = PdfName(b"Page")
+        if "Parent" not in dict_obj:
+            dict_obj["Parent"] = self.pages_ref
+        return self.write_obj(ref, *objs, **dict_obj)
+
+    def write_obj(self, ref, *objs, **dict_obj):
+        f = self.f
+        if ref is None:
+            ref = self.next_object_id(f.tell())
+        else:
+            self.xref_table[ref.object_id] = (f.tell(), ref.generation)
+        f.write(bytes(IndirectObjectDef(*ref)))
+        stream = dict_obj.pop("stream", None)
+        if stream is not None:
+            dict_obj["Length"] = len(stream)
+        if dict_obj:
+            f.write(pdf_repr(dict_obj))
+        for obj in objs:
+            f.write(pdf_repr(obj))
+        if stream is not None:
+            f.write(b"stream\n")
+            f.write(stream)
+            f.write(b"\nendstream\n")
+        f.write(b"endobj\n")
+        return ref
 
-class LabelSpinbox(ttk.Frame):
-    """
-        Create a compound widget, with a label and a Spinbox.
-        Input:
-            parent: container in which the widgets will be created
-            label_text: string to be shown on the label
-            label_anchor - position of the text within the label
-            label_width: label width in number of characters
-            entry_width: entry width in number of characters
-            entry_method: method to associate when the entry events
-            spin_start: initial value
-            spin_end: end_value
-            spin_increment: increment
-        Methods:
-            enable method:
-                enables the widgets (state='normal')
-            disable method:
-                disables the widgets (state='disabled')
-            read_only method:
-                disabled edition of the entry widget (state='readonly')
-            get method:
-                gets the value from the entry widget
-            set method:
-                sets the value to the entry widget
-        """
-
-    def __init__(self, parent,
-                 label_text='label:',
-                 label_anchor='e',
-                 label_width=10,
-                 entry_width=5,
-                 entry_method=None,
-                 spin_start=0,
-                 spin_end=10,
-                 spin_increment=1,
-                 spin_precision=1
-                 ):
-
-        # Parent class initialization
-        super().__init__(parent)
-        self.increment = spin_increment
-        self.start = spin_start
-        self.end = spin_end
-        self.precision = spin_precision
-
-        # Frame configuration
-        if True:
-            self.rowconfigure(0, weight=1)
-            self.columnconfigure(0, weight=1)
-            self.columnconfigure(1, weight=0)
-
-        # Label
-        if True:
-            self.label = ttk.Label(self, text=label_text, anchor=label_anchor, width=label_width)
-            self.label.grid(row=0, column=0, sticky='ew', padx=2)
-
-        # Spinbox
-        if True:
-            self.variable = tk.DoubleVar(value=spin_start)
-            self.spin = ttk.Spinbox(self, textvariable=self.variable, justify='center', width=entry_width,
-                                    from_=spin_start, to=spin_end, increment=spin_increment)
-            self.spin.grid(row=0, column=1, sticky='ew', padx=2)
-
-        # Bind method
-        if True:
-            self.spin.bind("<Return>", entry_method)
-            self.spin.bind("<FocusOut>", entry_method)
-            self.spin.bind("<<Increment>>", self._do_on_increment)
-            self.spin.bind("<<Decrement>>", self._do_on_decrement)
-
-    def enable(self):
-        self.label.config(style='TLabel')
-        self.spin.config(state='normal')
-
-    def disable(self):
-        self.label.config(style='secondary.TLabel')
-        self.spin.config(state='disabled')
-
-    def readonly(self):
-        self.label.config(style='TLabel')
-        self.spin.config(state='readonly')
-
-    def _do_on_increment(self, *args, **kwargs):
-        self.do_upon_clicking_arrows("up")
-        return "break"
-
-    def _do_on_decrement(self, *args, **kwargs):
-        self.do_upon_clicking_arrows("down")
-        return "break"
-
-    def do_upon_clicking_arrows(self, direction):
-
-        if direction == 'up':
-            sign = 1
-            if self.get() >= self.end:
-                self.set(self.end)
+    def del_root(self):
+        if self.root_ref is None:
+            return
+        del self.xref_table[self.root_ref.object_id]
+        del self.xref_table[self.root[b"Pages"].object_id]
 
+    @staticmethod
+    def get_buf_from_file(f):
+        if hasattr(f, "getbuffer"):
+            return f.getbuffer()
+        elif hasattr(f, "getvalue"):
+            return f.getvalue()
+        else:
+            try:
+                return mmap.mmap(f.fileno(), 0, access=mmap.ACCESS_READ)
+            except ValueError:  # cannot mmap an empty file
+                return b""
+
+    def read_pdf_info(self):
+        self.file_size_total = len(self.buf)
+        self.file_size_this = self.file_size_total - self.start_offset
+        self.read_trailer()
+        self.root_ref = self.trailer_dict[b"Root"]
+        self.info_ref = self.trailer_dict.get(b"Info", None)
+        self.root = PdfDict(self.read_indirect(self.root_ref))
+        if self.info_ref is None:
+            self.info = PdfDict()
+        else:
+            self.info = PdfDict(self.read_indirect(self.info_ref))
+        check_format_condition(b"Type" in self.root, "/Type missing in Root")
+        check_format_condition(
+            self.root[b"Type"] == b"Catalog", "/Type in Root is not /Catalog"
+        )
+        check_format_condition(b"Pages" in self.root, "/Pages missing in Root")
+        check_format_condition(
+            isinstance(self.root[b"Pages"], IndirectReference),
+            "/Pages in Root is not an indirect reference",
+        )
+        self.pages_ref = self.root[b"Pages"]
+        self.page_tree_root = self.read_indirect(self.pages_ref)
+        self.pages = self.linearize_page_tree(self.page_tree_root)
+        # save the original list of page references
+        # in case the user modifies, adds or deletes some pages
+        # and we need to rewrite the pages and their list
+        self.orig_pages = self.pages[:]
+
+    def next_object_id(self, offset=None):
+        try:
+            # TODO: support reuse of deleted objects
+            reference = IndirectReference(max(self.xref_table.keys()) + 1, 0)
+        except ValueError:
+            reference = IndirectReference(1, 0)
+        if offset is not None:
+            self.xref_table[reference.object_id] = (offset, 0)
+        return reference
+
+    delimiter = rb"[][()<>{}/%]"
+    delimiter_or_ws = rb"[][()<>{}/%\000\011\012\014\015\040]"
+    whitespace = rb"[\000\011\012\014\015\040]"
+    whitespace_or_hex = rb"[\000\011\012\014\015\0400-9a-fA-F]"
+    whitespace_optional = whitespace + b"*"
+    whitespace_mandatory = whitespace + b"+"
+    # No "\012" aka "\n" or "\015" aka "\r":
+    whitespace_optional_no_nl = rb"[\000\011\014\040]*"
+    newline_only = rb"[\r\n]+"
+    newline = whitespace_optional_no_nl + newline_only + whitespace_optional_no_nl
+    re_trailer_end = re.compile(
+        whitespace_mandatory
+        + rb"trailer"
+        + whitespace_optional
+        + rb"<<(.*>>)"
+        + newline
+        + rb"startxref"
+        + newline
+        + rb"([0-9]+)"
+        + newline
+        + rb"%%EOF"
+        + whitespace_optional
+        + rb"$",
+        re.DOTALL,
+    )
+    re_trailer_prev = re.compile(
+        whitespace_optional
+        + rb"trailer"
+        + whitespace_optional
+        + rb"<<(.*?>>)"
+        + newline
+        + rb"startxref"
+        + newline
+        + rb"([0-9]+)"
+        + newline
+        + rb"%%EOF"
+        + whitespace_optional,
+        re.DOTALL,
+    )
+
+    def read_trailer(self):
+        search_start_offset = len(self.buf) - 16384
+        if search_start_offset < self.start_offset:
+            search_start_offset = self.start_offset
+        m = self.re_trailer_end.search(self.buf, search_start_offset)
+        check_format_condition(m, "trailer end not found")
+        # make sure we found the LAST trailer
+        last_match = m
+        while m:
+            last_match = m
+            m = self.re_trailer_end.search(self.buf, m.start() + 16)
+        if not m:
+            m = last_match
+        trailer_data = m.group(1)
+        self.last_xref_section_offset = int(m.group(2))
+        self.trailer_dict = self.interpret_trailer(trailer_data)
+        self.xref_table = XrefTable()
+        self.read_xref_table(xref_section_offset=self.last_xref_section_offset)
+        if b"Prev" in self.trailer_dict:
+            self.read_prev_trailer(self.trailer_dict[b"Prev"])
+
+    def read_prev_trailer(self, xref_section_offset):
+        trailer_offset = self.read_xref_table(xref_section_offset=xref_section_offset)
+        m = self.re_trailer_prev.search(
+            self.buf[trailer_offset : trailer_offset + 16384]
+        )
+        check_format_condition(m, "previous trailer not found")
+        trailer_data = m.group(1)
+        check_format_condition(
+            int(m.group(2)) == xref_section_offset,
+            "xref section offset in previous trailer doesn't match what was expected",
+        )
+        trailer_dict = self.interpret_trailer(trailer_data)
+        if b"Prev" in trailer_dict:
+            self.read_prev_trailer(trailer_dict[b"Prev"])
+
+    re_whitespace_optional = re.compile(whitespace_optional)
+    re_name = re.compile(
+        whitespace_optional
+        + rb"/([!-$&'*-.0-;=?-Z\\^-z|~]+)(?="
+        + delimiter_or_ws
+        + rb")"
+    )
+    re_dict_start = re.compile(whitespace_optional + rb"<<")
+    re_dict_end = re.compile(whitespace_optional + rb">>" + whitespace_optional)
+
+    @classmethod
+    def interpret_trailer(cls, trailer_data):
+        trailer = {}
+        offset = 0
+        while True:
+            m = cls.re_name.match(trailer_data, offset)
+            if not m:
+                m = cls.re_dict_end.match(trailer_data, offset)
+                check_format_condition(
+                    m and m.end() == len(trailer_data),
+                    "name not found in trailer, remaining data: "
+                    + repr(trailer_data[offset:]),
+                )
+                break
+            key = cls.interpret_name(m.group(1))
+            value, offset = cls.get_value(trailer_data, m.end())
+            trailer[key] = value
+        check_format_condition(
+            b"Size" in trailer and isinstance(trailer[b"Size"], int),
+            "/Size not in trailer or not an integer",
+        )
+        check_format_condition(
+            b"Root" in trailer and isinstance(trailer[b"Root"], IndirectReference),
+            "/Root not in trailer or not an indirect reference",
+        )
+        return trailer
+
+    re_hashes_in_name = re.compile(rb"([^#]*)(#([0-9a-fA-F]{2}))?")
+
+    @classmethod
+    def interpret_name(cls, raw, as_text=False):
+        name = b""
+        for m in cls.re_hashes_in_name.finditer(raw):
+            if m.group(3):
+                name += m.group(1) + bytearray.fromhex(m.group(3).decode("us-ascii"))
             else:
-                self.set(self.get() + sign * self.increment)
+                name += m.group(1)
+        if as_text:
+            return name.decode("utf-8")
         else:
-            sign = -1
-            if self.get() <= self.start:
-                self.set(self.start)
+            return bytes(name)
 
+    re_null = re.compile(whitespace_optional + rb"null(?=" + delimiter_or_ws + rb")")
+    re_true = re.compile(whitespace_optional + rb"true(?=" + delimiter_or_ws + rb")")
+    re_false = re.compile(whitespace_optional + rb"false(?=" + delimiter_or_ws + rb")")
+    re_int = re.compile(
+        whitespace_optional + rb"([-+]?[0-9]+)(?=" + delimiter_or_ws + rb")"
+    )
+    re_real = re.compile(
+        whitespace_optional
+        + rb"([-+]?([0-9]+\.[0-9]*|[0-9]*\.[0-9]+))(?="
+        + delimiter_or_ws
+        + rb")"
+    )
+    re_array_start = re.compile(whitespace_optional + rb"\[")
+    re_array_end = re.compile(whitespace_optional + rb"]")
+    re_string_hex = re.compile(
+        whitespace_optional + rb"<(" + whitespace_or_hex + rb"*)>"
+    )
+    re_string_lit = re.compile(whitespace_optional + rb"\(")
+    re_indirect_reference = re.compile(
+        whitespace_optional
+        + rb"([-+]?[0-9]+)"
+        + whitespace_mandatory
+        + rb"([-+]?[0-9]+)"
+        + whitespace_mandatory
+        + rb"R(?="
+        + delimiter_or_ws
+        + rb")"
+    )
+    re_indirect_def_start = re.compile(
+        whitespace_optional
+        + rb"([-+]?[0-9]+)"
+        + whitespace_mandatory
+        + rb"([-+]?[0-9]+)"
+        + whitespace_mandatory
+        + rb"obj(?="
+        + delimiter_or_ws
+        + rb")"
+    )
+    re_indirect_def_end = re.compile(
+        whitespace_optional + rb"endobj(?=" + delimiter_or_ws + rb")"
+    )
+    re_comment = re.compile(
+        rb"(" + whitespace_optional + rb"%[^\r\n]*" + newline + rb")*"
+    )
+    re_stream_start = re.compile(whitespace_optional + rb"stream\r?\n")
+    re_stream_end = re.compile(
+        whitespace_optional + rb"endstream(?=" + delimiter_or_ws + rb")"
+    )
+
+    @classmethod
+    def get_value(cls, data, offset, expect_indirect=None, max_nesting=-1):
+        if max_nesting == 0:
+            return None, None
+        m = cls.re_comment.match(data, offset)
+        if m:
+            offset = m.end()
+        m = cls.re_indirect_def_start.match(data, offset)
+        if m:
+            check_format_condition(
+                int(m.group(1)) > 0,
+                "indirect object definition: object ID must be greater than 0",
+            )
+            check_format_condition(
+                int(m.group(2)) >= 0,
+                "indirect object definition: generation must be non-negative",
+            )
+            check_format_condition(
+                expect_indirect is None
+                or expect_indirect
+                == IndirectReference(int(m.group(1)), int(m.group(2))),
+                "indirect object definition different than expected",
+            )
+            object, offset = cls.get_value(data, m.end(), max_nesting=max_nesting - 1)
+            if offset is None:
+                return object, None
+            m = cls.re_indirect_def_end.match(data, offset)
+            check_format_condition(m, "indirect object definition end not found")
+            return object, m.end()
+        check_format_condition(
+            not expect_indirect, "indirect object definition not found"
+        )
+        m = cls.re_indirect_reference.match(data, offset)
+        if m:
+            check_format_condition(
+                int(m.group(1)) > 0,
+                "indirect object reference: object ID must be greater than 0",
+            )
+            check_format_condition(
+                int(m.group(2)) >= 0,
+                "indirect object reference: generation must be non-negative",
+            )
+            return IndirectReference(int(m.group(1)), int(m.group(2))), m.end()
+        m = cls.re_dict_start.match(data, offset)
+        if m:
+            offset = m.end()
+            result = {}
+            m = cls.re_dict_end.match(data, offset)
+            while not m:
+                key, offset = cls.get_value(data, offset, max_nesting=max_nesting - 1)
+                if offset is None:
+                    return result, None
+                value, offset = cls.get_value(data, offset, max_nesting=max_nesting - 1)
+                result[key] = value
+                if offset is None:
+                    return result, None
+                m = cls.re_dict_end.match(data, offset)
+            offset = m.end()
+            m = cls.re_stream_start.match(data, offset)
+            if m:
+                try:
+                    stream_len = int(result[b"Length"])
+                except (TypeError, KeyError, ValueError) as e:
+                    msg = "bad or missing Length in stream dict (%r)" % result.get(
+                        b"Length", None
+                    )
+                    raise PdfFormatError(msg) from e
+                stream_data = data[m.end() : m.end() + stream_len]
+                m = cls.re_stream_end.match(data, m.end() + stream_len)
+                check_format_condition(m, "stream end not found")
+                offset = m.end()
+                result = PdfStream(PdfDict(result), stream_data)
             else:
-                self.set(self.get() + sign * self.increment)
-
-    def get(self):
-        return self.variable.get()
-
-    def set(self, value):
-        self.variable.set(round(value, self.precision))
+                result = PdfDict(result)
+            return result, offset
+        m = cls.re_array_start.match(data, offset)
+        if m:
+            offset = m.end()
+            result = []
+            m = cls.re_array_end.match(data, offset)
+            while not m:
+                value, offset = cls.get_value(data, offset, max_nesting=max_nesting - 1)
+                result.append(value)
+                if offset is None:
+                    return result, None
+                m = cls.re_array_end.match(data, offset)
+            return result, m.end()
+        m = cls.re_null.match(data, offset)
+        if m:
+            return None, m.end()
+        m = cls.re_true.match(data, offset)
+        if m:
+            return True, m.end()
+        m = cls.re_false.match(data, offset)
+        if m:
+            return False, m.end()
+        m = cls.re_name.match(data, offset)
+        if m:
+            return PdfName(cls.interpret_name(m.group(1))), m.end()
+        m = cls.re_int.match(data, offset)
+        if m:
+            return int(m.group(1)), m.end()
+        m = cls.re_real.match(data, offset)
+        if m:
+            # XXX Decimal instead of float???
+            return float(m.group(1)), m.end()
+        m = cls.re_string_hex.match(data, offset)
+        if m:
+            # filter out whitespace
+            hex_string = bytearray(
+                b for b in m.group(1) if b in b"0123456789abcdefABCDEF"
+            )
+            if len(hex_string) % 2 == 1:
+                # append a 0 if the length is not even - yes, at the end
+                hex_string.append(ord(b"0"))
+            return bytearray.fromhex(hex_string.decode("us-ascii")), m.end()
+        m = cls.re_string_lit.match(data, offset)
+        if m:
+            return cls.get_literal_string(data, m.end())
+        # return None, offset  # fallback (only for debugging)
+        msg = "unrecognized object: " + repr(data[offset : offset + 32])
+        raise PdfFormatError(msg)
+
+    re_lit_str_token = re.compile(
+        rb"(\\[nrtbf()\\])|(\\[0-9]{1,3})|(\\(\r\n|\r|\n))|(\r\n|\r|\n)|(\()|(\))"
+    )
+    escaped_chars = {
+        b"n": b"\n",
+        b"r": b"\r",
+        b"t": b"\t",
+        b"b": b"\b",
+        b"f": b"\f",
+        b"(": b"(",
+        b")": b")",
+        b"\\": b"\\",
+        ord(b"n"): b"\n",
+        ord(b"r"): b"\r",
+        ord(b"t"): b"\t",
+        ord(b"b"): b"\b",
+        ord(b"f"): b"\f",
+        ord(b"("): b"(",
+        ord(b")"): b")",
+        ord(b"\\"): b"\\",
+    }
 
+    @classmethod
+    def get_literal_string(cls, data, offset):
+        nesting_depth = 0
+        result = bytearray()
+        for m in cls.re_lit_str_token.finditer(data, offset):
+            result.extend(data[offset : m.start()])
+            if m.group(1):
+                result.extend(cls.escaped_chars[m.group(1)[1]])
+            elif m.group(2):
+                result.append(int(m.group(2)[1:], 8))
+            elif m.group(3):
+                pass
+            elif m.group(5):
+                result.extend(b"\n")
+            elif m.group(6):
+                result.extend(b"(")
+                nesting_depth += 1
+            elif m.group(7):
+                if nesting_depth == 0:
+                    return bytes(result), m.end()
+                result.extend(b")")
+                nesting_depth -= 1
+            offset = m.end()
+        msg = "unfinished literal string"
+        raise PdfFormatError(msg)
+
+    re_xref_section_start = re.compile(whitespace_optional + rb"xref" + newline)
+    re_xref_subsection_start = re.compile(
+        whitespace_optional
+        + rb"([0-9]+)"
+        + whitespace_mandatory
+        + rb"([0-9]+)"
+        + whitespace_optional
+        + newline_only
+    )
+    re_xref_entry = re.compile(rb"([0-9]{10}) ([0-9]{5}) ([fn])( \r| \n|\r\n)")
+
+    def read_xref_table(self, xref_section_offset):
+        subsection_found = False
+        m = self.re_xref_section_start.match(
+            self.buf, xref_section_offset + self.start_offset
+        )
+        check_format_condition(m, "xref section start not found")
+        offset = m.end()
+        while True:
+            m = self.re_xref_subsection_start.match(self.buf, offset)
+            if not m:
+                check_format_condition(
+                    subsection_found, "xref subsection start not found"
+                )
+                break
+            subsection_found = True
+            offset = m.end()
+            first_object = int(m.group(1))
+            num_objects = int(m.group(2))
+            for i in range(first_object, first_object + num_objects):
+                m = self.re_xref_entry.match(self.buf, offset)
+                check_format_condition(m, "xref entry not found")
+                offset = m.end()
+                is_free = m.group(3) == b"f"
+                generation = int(m.group(2))
+                if not is_free:
+                    new_entry = (int(m.group(1)), generation)
+                    check_format_condition(
+                        i not in self.xref_table or self.xref_table[i] == new_entry,
+                        "xref entry duplicated (and not identical)",
+                    )
+                    self.xref_table[i] = new_entry
+        return offset
+
+    def read_indirect(self, ref, max_nesting=-1):
+        offset, generation = self.xref_table[ref[0]]
+        check_format_condition(
+            generation == ref[1],
+            f"expected to find generation {ref[1]} for object ID {ref[0]} in xref "
+            f"table, instead found generation {generation} at offset {offset}",
+        )
+        value = self.get_value(
+            self.buf,
+            offset + self.start_offset,
+            expect_indirect=IndirectReference(*ref),
+            max_nesting=max_nesting,
+        )[0]
+        self.cached_objects[ref] = value
+        return value
+
+    def linearize_page_tree(self, node=None):
+        if node is None:
+            node = self.page_tree_root
+        check_format_condition(
+            node[b"Type"] == b"Pages", "/Type of page tree node is not /Pages"
+        )
+        pages = []
+        for kid in node[b"Kids"]:
+            kid_object = self.read_indirect(kid)
+            if kid_object[b"Type"] == b"Page":
+                pages.append(kid)
+            else:
+                pages.extend(self.linearize_page_tree(node=kid_object))
+        return pages
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `compoundwidgets-0.1.9/compoundwidgets/CUSTOM_BUTTONS.py` & `compoundwidgets-0.2.0/compoundwidgets/CUSTOM_BUTTONS.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,144 +1,210 @@
-import tkinter.ttk as ttk
-from PIL import Image, ImageTk
+import ttkbootstrap as ttk
+from .SCRIPTS import *
 import os
 
 ROOT_DIR = os.path.realpath(os.path.join(os.path.dirname(__file__), 'IMAGES'))
 
 
-def open_image(file_name: str, size_x: int, size_y: int, maximize: bool = False) -> ImageTk:
-    """
-    Function to open an image file and to adjust its dimensions as specified
-    Input:  file_name - full path to the image
-            size_x - final horizontal size of the image
-            size_y - final vertical size of the image
-            maximize -  if True enlarges the image to fit the dimensions,
-                        else if reduces the image to fit the dimensions
-    Return: tk_image - ImageTK to be inserted on a widget
-    """
-    image_final_width = size_x
-    image_final_height = size_y
-    pil_image = Image.open(file_name)
-    w, h = pil_image.size
-    if maximize:
-        final_scale = min(h / image_final_height, w / image_final_width)
-    else:
-        final_scale = max(h / image_final_height, w / image_final_width)
-    width_final = int(w / final_scale)
-    height_final = int(h / final_scale)
-    final_pil_image = pil_image.resize((width_final, height_final), Image.ANTIALIAS)
-    final_pil_image = final_pil_image.convert('RGBA')
-    tk_image = ImageTk.PhotoImage(final_pil_image)
-    return tk_image
+class YesButton(ttk.Button):
+    def __init__(self, *args, language='en', style='success', width=10, **kwargs):
+        super().__init__(*args, **kwargs)
+        image_path = os.path.join(ROOT_DIR, 'yes.png')
+        tk_image = open_image(file_name=image_path, size_x=20, size_y=20, maximize=True)
 
+        if language == 'br':
+            text = 'SIM\t'
+        else:
+            text = 'YES\t'
 
-class ClearButton(ttk.Button):
-    def __init__(self, *args, **kwargs):
+        self.configure(text=text, bootstyle=style, width=width, image=tk_image, compound='right')
+        self.image = tk_image
+
+
+class NoButton(ttk.Button):
+    def __init__(self, *args, language='en', style='danger', width=10, **kwargs):
         super().__init__(*args, **kwargs)
-        image_path = os.path.join(ROOT_DIR, 'clear.png')
+        image_path = os.path.join(ROOT_DIR, 'no.png')
         tk_image = open_image(file_name=image_path, size_x=20, size_y=20)
 
-        self.configure(text='LIMPAR\t\t', style='warning.TButton', width=15, image=tk_image, compound='right')
+        if language == 'br':
+            text = 'NÃO\t'
+        else:
+            text = 'NO\t'
+
+        self.configure(text=text, bootstyle=style, width=width, image=tk_image, compound='right')
         self.image = tk_image
 
 
-class SaveButton(ttk.Button):
-    def __init__(self, *args, **kwargs):
+class OKButton(ttk.Button):
+    def __init__(self, *args, language='en', style='success', width=10, **kwargs):
         super().__init__(*args, **kwargs)
-        image_path = os.path.join(ROOT_DIR, 'save.png')
-        tk_image = open_image(file_name=image_path, size_x=20, size_y=20)
+        image_path = os.path.join(ROOT_DIR, 'yes.png')
+        tk_image = open_image(file_name=image_path, size_x=20, size_y=20, maximize=True)
 
-        self.configure(text='SALVAR\t\t', style='success.TButton', width=15, image=tk_image, compound='right')
+        self.configure(text='OK\t', bootstyle=style, width=width, image=tk_image, compound='right')
         self.image = tk_image
 
 
 class CancelButton(ttk.Button):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, language='en', style='danger', width=10,  **kwargs):
         super().__init__(*args, **kwargs)
         image_path = os.path.join(ROOT_DIR, 'no.png')
         tk_image = open_image(file_name=image_path, size_x=20, size_y=20)
 
-        self.configure(text='CANCELAR\t', style='danger.TButton', width=15, image=tk_image, compound='right')
+        if language == 'br':
+            text = 'CANCELAR\t'
+        else:
+            text = 'CANCEL\t'
+
+        self.configure(text=text, bootstyle=style, width=width, image=tk_image, compound='right')
         self.image = tk_image
 
 
-class YesButton(ttk.Button):
-    def __init__(self, *args, **kwargs):
+class ClearButton(ttk.Button):
+    def __init__(self, *args, language='en', style='warning', width=10, **kwargs):
         super().__init__(*args, **kwargs)
-        image_path = os.path.join(ROOT_DIR, 'yes.png')
-        tk_image = open_image(file_name=image_path, size_x=20, size_y=20)
+        image_path = os.path.join(ROOT_DIR, 'clear.png')
+        tk_image = open_image(file_name=image_path, size_x=20, size_y=20, maximize=True)
 
-        self.configure(text='SIM\t\t', style='success.TButton', width=15, image=tk_image, compound='right')
+        if language == 'br':
+            text = 'LIMPAR\t'
+        else:
+            text = 'CLEAR\t'
+
+        self.configure(text=text, bootstyle=style, width=width, image=tk_image, compound='right')
         self.image = tk_image
 
 
-class NoButton(ttk.Button):
-    def __init__(self, *args, **kwargs):
+class SaveButton(ttk.Button):
+    def __init__(self, *args, language='en', style='success', width=10, **kwargs):
         super().__init__(*args, **kwargs)
-        image_path = os.path.join(ROOT_DIR, 'no.png')
+        image_path = os.path.join(ROOT_DIR, 'save.png')
         tk_image = open_image(file_name=image_path, size_x=20, size_y=20)
 
-        self.configure(text='NÃO\t\t', style='danger.TButton', width=15, image=tk_image, compound='right')
+        if language == 'br':
+            text = 'SALVAR\t'
+        else:
+            text = 'SAVE\t'
+
+        self.configure(text=text, bootstyle=style, width=width, image=tk_image, compound='right')
         self.image = tk_image
 
 
 class CalculateButton(ttk.Button):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, language='en', style='primary', width=15, **kwargs):
         super().__init__(*args, **kwargs)
         image_path = os.path.join(ROOT_DIR, 'calculate.png')
         tk_image = open_image(file_name=image_path, size_x=20, size_y=20)
 
-        self.configure(text='CALCULAR\t', style='primary.TButton', width=15, image=tk_image, compound='right')
+        if language == 'br':
+            text = 'CALCULAR\t'
+        else:
+            text = 'CALCULATE\t'
+
+        self.configure(text=text, bootstyle=style, width=width, image=tk_image, compound='right')
         self.image = tk_image
 
 
 class HelpButton(ttk.Button):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, language='en', style='secondary', width=10,  **kwargs):
         super().__init__(*args, **kwargs)
         image_path = os.path.join(ROOT_DIR, 'help.png')
         tk_image = open_image(file_name=image_path, size_x=30, size_y=20)
 
-        self.configure(style='secondary.TButton', image=tk_image)
+        self.configure(bootstyle=style, width=width,  image=tk_image)
         self.image = tk_image
 
 
 class BackButton(ttk.Button):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, language='en', style='primary', width=15, **kwargs):
         super().__init__(*args, **kwargs)
         image_path = os.path.join(ROOT_DIR, 'back.png')
         tk_image = open_image(file_name=image_path, size_x=30, size_y=20)
 
-        self.configure(text='VOLTAR\t\t', style='primary.TButton', width=15, image=tk_image, compound='right')
+        if language == 'br':
+            text = 'VOLTAR\t\t'
+        else:
+            text = 'BACK\t\t'
+
+        self.configure(text=text, bootstyle=style, width=width, image=tk_image, compound='right')
         self.image = tk_image
 
 
 class AddToReport(ttk.Button):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, language='en', style='success', width=15,  **kwargs):
         super().__init__(*args, **kwargs)
         image_path = os.path.join(ROOT_DIR, 'add_to_form.png')
-        tk_image = open_image(file_name=image_path, size_x=16, size_y=16)
+        tk_image = open_image(file_name=image_path, size_x=30, size_y=20)
+
+        if language == 'br':
+            text = 'ADICIONAR\t'
+        else:
+            text = 'ADD\t\t'
 
-        self.configure(text='ADICIONAR\t', style='success.TButton', width=13, image=tk_image, compound='right',
-                       padding=4)
+        self.configure(text=text, bootstyle=style, width=width,  image=tk_image, compound='right')
         self.image = tk_image
 
 
 class EditReport(ttk.Button):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, language='en', style='primary', width=15, **kwargs):
         super().__init__(*args, **kwargs)
         image_path = os.path.join(ROOT_DIR, 'edit_form.png')
-        tk_image = open_image(file_name=image_path, size_x=16, size_y=16)
+        tk_image = open_image(file_name=image_path, size_x=30, size_y=20)
+
+        if language == 'br':
+            text = 'EDITAR\t\t'
+        else:
+            text = 'EDIT\t\t'
 
-        self.configure(text='EDITAR\t\t', style='primary.TButton', width=13, image=tk_image, compound='right',
-                       padding=4)
+        self.configure(text=text, bootstyle=style, width=width, image=tk_image, compound='right')
         self.image = tk_image
 
 
 class RemoveFromReport(ttk.Button):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, language='en', style='danger', width=15, **kwargs):
         super().__init__(*args, **kwargs)
         image_path = os.path.join(ROOT_DIR, 'remove_from_form.png')
-        tk_image = open_image(file_name=image_path, size_x=16, size_y=16)
+        tk_image = open_image(file_name=image_path, size_x=30, size_y=20)
+
+        if language == 'br':
+            text = 'EXCLUIR\t\t'
+        else:
+            text = 'DELETE\t\t'
+
+        self.configure(text=text, bootstyle=style, width=width, image=tk_image, compound='right')
+        self.image = tk_image
+
+
+class AddNewButton(ttk.Button):
+    def __init__(self, *args, language='en', style='primary', width=15, **kwargs):
+        super().__init__(*args, **kwargs)
+        image_path = os.path.join(ROOT_DIR, 'add_new.png')
+        tk_image = open_image(file_name=image_path, size_x=30, size_y=20)
+
+        self.configure(bootstyle=style, width=width, image=tk_image, padding=2)
+        self.image = tk_image
+
+
+class EraseButton(ttk.Button):
+    def __init__(self, *args, language='en', style='danger', width=15, **kwargs):
+        super().__init__(*args, **kwargs)
+        image_path = os.path.join(ROOT_DIR, 'trash_can.png')
+        tk_image = open_image(file_name=image_path, size_x=30, size_y=20)
+
+        self.configure(bootstyle=style, width=width, image=tk_image, padding=2)
+        self.image = tk_image
+
+
+class QuitButton(ttk.Button):
+    def __init__(self, *args, language='en', style='danger', width=15, **kwargs):
+        super().__init__(*args, **kwargs)
+        image_path = os.path.join(ROOT_DIR, 'quit.png')
+        tk_image = open_image(file_name=image_path, size_x=30, size_y=20)
+
+        if language == 'br':
+            text = 'SAIR\t\t'
+        else:
+            text = 'EXIT\t\t'
 
-        self.configure(text='EXCLUIR\t\t', style='danger.TButton', width=13, image=tk_image, compound='right',
-                       padding=4)
+        self.configure(text=text, bootstyle=style, width=width, image=tk_image, compound='right')
         self.image = tk_image
```

### Comparing `compoundwidgets-0.1.9/compoundwidgets/IMAGES/add_to_form.png` & `compoundwidgets-0.2.0/compoundwidgets/IMAGES/add_to_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.1.9/compoundwidgets/IMAGES/back.png` & `compoundwidgets-0.2.0/compoundwidgets/IMAGES/back.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.1.9/compoundwidgets/IMAGES/calculate.png` & `compoundwidgets-0.2.0/compoundwidgets/IMAGES/calculate.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.1.9/compoundwidgets/IMAGES/clear.png` & `compoundwidgets-0.2.0/compoundwidgets/IMAGES/clear.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.1.9/compoundwidgets/IMAGES/edit_form.png` & `compoundwidgets-0.2.0/compoundwidgets/IMAGES/edit_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.1.9/compoundwidgets/IMAGES/help.png` & `compoundwidgets-0.2.0/compoundwidgets/IMAGES/help.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.1.9/compoundwidgets/IMAGES/no.png` & `compoundwidgets-0.2.0/compoundwidgets/IMAGES/no.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.1.9/compoundwidgets/IMAGES/remove_from_form.png` & `compoundwidgets-0.2.0/compoundwidgets/IMAGES/remove_from_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.1.9/compoundwidgets/IMAGES/save.png` & `compoundwidgets-0.2.0/compoundwidgets/IMAGES/save.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.1.9/compoundwidgets/MESSAGE_BOX_WIDGETS.py` & `compoundwidgets-0.2.0/compoundwidgets/MESSAGE_BOX_WIDGETS.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 import tkinter as tk
-import tkinter.ttk as ttk
+import ttkbootstrap as ttk
 
 
-class OkCancelBox(tk.Toplevel):
+class BaseTopLevelWidget(tk.Toplevel):
     """
-    Creates a OK/CANCEL message box with the same style as the main application
+    Basic TopLevel Widget for Message Boxes
     Input:
         parent: widget over which the progress bar will be positioned
+        icon_path: path to the icon for the widget
+        title: title message for the widget
         message = text to be shown as an alert to the user
     """
 
-    def __init__(self, parent, message):
+    def __init__(self, parent, icon_path, title, message):
 
         # Configuration
         if True:
             super().__init__(parent)
-            self.minsize(350, 150)
+            self.iconbitmap(icon_path)
+            self.title(title)
+            self.minsize(250, 120)
             self.columnconfigure(0, weight=1)
-            self.columnconfigure(1, weight=1)
+            self.columnconfigure(1, weight=0)
+            self.columnconfigure(2, weight=0)
             self.rowconfigure(0, weight=1)
             self.rowconfigure(1, weight=0)
-            self.overrideredirect(True)
-            self.config(padx=10, pady=10, bd=1, relief='raised')
+            self.rowconfigure(2, weight=0)
             self.lift()
 
-        # Widgets
+        # Label configuration
         if True:
-            self.control_var = tk.IntVar(value=0)
-            label = ttk.Label(self, text=message, anchor='center', justify='center', padding=10, wraplength=300)
-            label.grid(row=0, column=0, columnspan=2, sticky='nsew')
-
-            cancel_button = ttk.Button(self, text="Cancel", command=lambda: self.adjust_var(0), width=10,
-                                       style='danger.TButton')
-            cancel_button.grid(row=1, column=0, sticky='nsew', padx=30, pady=(0, 10))
-
-            ok_button = ttk.Button(self, text="OK", command=lambda: self.adjust_var(1), width=10,
-                                   style='success.TButton')
-            ok_button.grid(row=1, column=1, sticky='nsew', padx=30, pady=(0, 10))
+            self.label = ttk.Label(self, text=message, justify='left', padding=5)
+            self.label.grid(row=0, column=0, columnspan=3, sticky='nsew')
+            if self.label.winfo_reqwidth() > self.minsize()[0]:
+                self.minsize(self.label.winfo_reqwidth() + 20, 120)
+                self.update()
+
+        # Separator configuration
+            separator = ttk.Separator(self, orient='horizontal', style='secondary.Horizontal.TSeparator')
+            separator.grid(row=1, column=0, columnspan=3, sticky='nsew')
 
         # Determine relative position
         if True:
             position_x = parent.winfo_x()
             position_y = parent.winfo_y()
             height = parent.winfo_height()
             width = parent.winfo_width()
@@ -48,84 +50,123 @@
             local_height = self.minsize()[1]
             local_width = self.minsize()[0]
 
             final_position = (position_x + width / 2 - local_width / 2, position_y + height / 2 - local_height / 2)
             self.geometry('%dx%d+%d+%d' % (local_width, local_height, final_position[0], final_position[1]))
             self.grab_set()
 
+        # Control variable
+        self.control_var = tk.IntVar(value=0)
+
     def adjust_var(self, option):
         self.control_var.set(option)
         self.destroy()
 
     def show(self):
         self.deiconify()
         self.wait_window()
         value = self.control_var.get()
         return value
 
 
-class YesNoBox(tk.Toplevel):
+class OkCancelBox(BaseTopLevelWidget):
+    """
+    Creates a OK/CANCEL message box with the same style as the main application
+    Input:
+        parent: widget over which the progress bar will be positioned
+        icon_path: path to the icon for the widget
+        title: title message for the widget
+        message: text to be shown as an alert to the user
+        language: language for the buttons text
+    """
+
+    def __init__(self, parent, icon_path, title, message, language='en'):
+
+        super().__init__(parent, icon_path, title, message)
+
+        if language == 'br':
+            cancel_text, ok_text = 'CANCELAR', 'OK'
+        else:
+            cancel_text, ok_text = 'CANCEL', 'OK'
+
+        cancel_button = ttk.Button(self, text=cancel_text, command=lambda: self.adjust_var(0), width=8,
+                                   style='secondary.TButton')
+        cancel_button.grid(row=2, column=1, sticky='nsew', pady=5)
+
+        ok_button = ttk.Button(self, text=ok_text, command=lambda: self.adjust_var(1), width=8,
+                               style='primary.TButton')
+        ok_button.grid(row=2, column=2, sticky='nsew', padx=5, pady=5)
+
+
+class YesNoBox(BaseTopLevelWidget):
     """
     Creates a Yes/No message box with the same style as the main application
     Input:
         parent: widget over which the progress bar will be positioned
-        message = text to be shown as a question to the user
+        icon_path: path to the icon for the widget
+        title: title message for the widget
+        message: text to be shown as an alert to the user
+        language: language for the buttons text
     """
 
-    def __init__(self, parent, message):
+    def __init__(self, parent, icon_path, title, message, language='en'):
 
-        # Configuration
-        if True:
-            super().__init__(parent)
-            self.minsize(350, 150)
-            self.columnconfigure(0, weight=1)
-            self.columnconfigure(1, weight=1)
-            self.rowconfigure(0, weight=1)
-            self.rowconfigure(1, weight=0)
-            self.overrideredirect(True)
-            self.config(padx=10, pady=10, bd=1, relief='raised')
-            self.lift()
+        super().__init__(parent, icon_path, title, message)
 
-        # Widgets
-        if True:
-            self.control_var = tk.IntVar(value=0)
-            label = ttk.Label(self, text=message, anchor='center', justify='center', padding=10, wraplength=300)
-            label.grid(row=0, column=0, columnspan=2, sticky='nsew')
-
-            no_button = ttk.Button(self, text="NO", command=lambda: self.adjust_var(0), width=10,
-                                   style='danger.TButton')
-            no_button.grid(row=1, column=0, sticky='nsew', padx=30, pady=(0, 10))
-
-            yes_button = ttk.Button(self, text="YES", command=lambda: self.adjust_var(1), width=10,
-                                    style='success.TButton')
-            yes_button.grid(row=1, column=1, sticky='nsew', padx=30, pady=(0, 10))
+        if language == 'br':
+            no_text, yes_text = 'NÃO', 'SIM'
+        else:
+            no_text, yes_text = 'NO', 'YES'
 
-        # Determine relative position
-        if True:
-            position_x = parent.winfo_x()
-            position_y = parent.winfo_y()
-            height = parent.winfo_height()
-            width = parent.winfo_width()
+        no_button = ttk.Button(self, text=no_text, command=lambda: self.adjust_var(0), width=8,
+                               style='secondary.TButton')
+        no_button.grid(row=2, column=1, sticky='nsew', pady=5)
+        yes_button = ttk.Button(self, text=yes_text, command=lambda: self.adjust_var(1), width=8,
+                                style='primary.TButton')
+        yes_button.grid(row=2, column=2, sticky='nsew', padx=5, pady=5)
 
-            local_height = self.minsize()[1]
-            local_width = self.minsize()[0]
 
-            final_position = (position_x + width / 2 - local_width / 2, position_y + height / 2 - local_height / 2)
-            self.geometry('%dx%d+%d+%d' % (local_width, local_height, final_position[0], final_position[1]))
-            self.grab_set()
+class WarningBox(BaseTopLevelWidget):
+    """
+    Creates a message box with the same style as the main application
+    Input:
+        parent: widget over which the progress bar will be positioned
+        icon_path: path to the icon for the widget
+        title: title message for the widget
+        message: text to be shown as an alert to the user
+        language: language for the buttons text
+    """
 
-    def adjust_var(self, option):
-        self.control_var.set(option)
-        self.destroy()
+    def __init__(self, parent, icon_path, title, message, language='en'):
 
-    def show(self):
-        self.deiconify()
-        self.wait_window()
-        value = self.control_var.get()
-        return value
+        super().__init__(parent, icon_path, title, message)
+
+        self.label.config(style='danger.TLabel')
+        ok_button = ttk.Button(self, text="OK", command=lambda: self.destroy(), width=8,
+                               style='danger.TButton')
+        ok_button.grid(row=2, column=2, sticky='nsew', padx=5, pady=5)
+
+
+class SuccessBox(BaseTopLevelWidget):
+    """
+    Creates a message box with the same style as the main application
+    Input:
+        parent: widget over which the progress bar will be positioned
+        icon_path: path to the icon for the widget
+        title: title message for the widget
+        message: text to be shown as an alert to the user
+        language: language for the buttons text
+    """
+
+    def __init__(self, parent, icon_path, title, message, language='en'):
+
+        super().__init__(parent, icon_path, title, message)
+        ok_button = ttk.Button(self, text="OK", command=lambda: self.destroy(), width=8,
+                               style='primary.TButton')
+        ok_button.grid(row=2, column=2, sticky='nsew', padx=5, pady=5)
 
 
 class ProgressBar(tk.Toplevel):
     """
     Creates a progress bar to follow the program tasks
     Input:
         parent: widget over which the progress bar will be positioned
@@ -144,18 +185,21 @@
             self.columnconfigure(0, weight=1)
             self.rowconfigure(0, weight=1)
             self.rowconfigure(1, weight=0)
             self.overrideredirect(True)
             self.config(padx=10, pady=10, bd=1, relief='raised')
             self.lift()
 
-        # Message
+        # Label configuration
         if True:
-            label = ttk.Label(self, text=message, padding=10, wraplength=300)
-            label.grid(row=0, column=0, sticky='nsew')
+            self.label = ttk.Label(self, text=message, justify='left', padding=10)
+            self.label.grid(row=0, column=0, sticky='nsew')
+            if self.label.winfo_reqwidth() > self.minsize()[0]:
+                self.minsize(self.label.winfo_reqwidth() + 20, 100)
+                self.update()
 
         # Progress bar
         if True:
             local_frame = ttk.Frame(self)
             local_frame.grid(row=1, column=0, sticky='nsew')
             local_frame.columnconfigure(0, weight=1)
             local_frame.rowconfigure(0, weight=1)
@@ -183,59 +227,14 @@
             self.grab_set()
 
     def update_bar(self, value):
         self.progress_var.set(value/self.final_value)
         self.update_idletasks()
 
 
-class WarningBox(tk.Toplevel):
-    """ Creates a message box with the same style as the main application """
-
-    def __init__(self, parent, message):
-
-        # Configuration
-        if True:
-            super().__init__(parent)
-            self.minsize(350, 150)
-            self.columnconfigure(0, weight=1)
-            self.rowconfigure(0, weight=1)
-            self.rowconfigure(1, weight=0)
-            self.overrideredirect(True)
-            self.config(padx=10, pady=10, bd=1, relief='raised')
-            self.lift()
-
-        # Widgets
-        if True:
-            label = ttk.Label(self, text=message, anchor='center', justify='center', padding=10, wraplength=300)
-            label.grid(row=0, column=0, sticky='nsew')
-
-            ok_button = ttk.Button(self, text="OK", command=lambda: self.destroy(), width=10,
-                                   style='danger.TButton')
-            ok_button.grid(row=1, column=0, sticky='nsew', padx=30, pady=(0, 10))
-
-        # Determine relative position
-        if True:
-            position_x = parent.winfo_x()
-            position_y = parent.winfo_y()
-            height = parent.winfo_height()
-            width = parent.winfo_width()
-
-            local_height = self.minsize()[1]
-            local_width = self.minsize()[0]
-
-            final_position = (position_x + width / 2 - local_width / 2, position_y + height / 2 - local_height / 2)
-            self.geometry('%dx%d+%d+%d' % (local_width, local_height, final_position[0], final_position[1]))
-            self.grab_set()
-
-    def show(self):
-        self.deiconify()
-        self.wait_window()
-        return
-
-
 class Tooltip:
     """ It creates a tooltip for a given widget as the mouse goes on it. """
 
     def __init__(self, widget, text='widget info', bg='#FFFF8B', fg='black', wait_time=500, wrap_length=250):
 
         self.style = widget.winfo_toplevel().style
         self.style.configure('custom.TLabel', background=bg, foreground=fg)
@@ -311,7 +310,90 @@
 
         self.top_level.geometry(f'+{x}+{y}')
 
     def hide(self):
         if self.top_level:
             self.top_level.destroy()
         self.top_level = None
+
+
+class TimedBox(tk.Toplevel):
+    """
+    TopLevel widget for timed message boxes.
+    Input:
+        parent = widget over which the progress bar will be positioned
+        message = text to be shown as an alert to the user
+        time = time in seconds for the pop-up window display
+        style = color scheme for the window
+    """
+
+    def __init__(self, parent, message, time=1, style=None):
+
+        # Configuration
+        if True:
+            super().__init__(parent)
+            self.overrideredirect(True)
+            self.total_time_ms = 1000 * time
+            self.minsize(250, 120)
+            self.columnconfigure(0, weight=1)
+            self.columnconfigure(1, weight=0)
+            self.rowconfigure(0, weight=1)
+            self.rowconfigure(1, weight=0)
+            self.rowconfigure(2, weight=0)
+            self.lift()
+            style_dict = {
+                'danger': ('danger.TLabel','danger.TButton', 'danger.Horizontal.TProgressbar'),
+                'warning': ('warning.TLabel', 'warning.TButton', 'warning.Horizontal.TProgressbar'),
+                'info': ('info.TLabel', 'info.TButton', 'info.Horizontal.TProgressbar'),
+            }
+
+        # Widgets
+        if True:
+            label_style, button_style, progress_bar_style = \
+                style_dict.get(style, ('TLabel', 'TButton', 'TProgressbar'))
+            label = ttk.Label(self, text=message, justify='left', style=label_style)
+            label.grid(row=0, column=0, columnspan=2, sticky='nsew', padx=10, pady=10)
+
+            self.progressbar_var = tk.DoubleVar(value=0)
+            self.progressbar = ttk.Progressbar(self, maximum=self.total_time_ms, orient='horizontal',
+                                               mode='determinate', style=progress_bar_style,
+                                               variable=self.progressbar_var)
+            self.progressbar.grid(row=1, column=0, columnspan=2, sticky='nsew', padx=10)
+
+            button = ttk.Button(self, text='CLOSE', style=button_style, command= lambda: self.destroy())
+            button.grid(row=2, column=1, sticky='nsew', pady=10, padx=10)
+
+            if label.winfo_reqwidth() > self.minsize()[0]:
+                self.minsize(label.winfo_reqwidth() + 40, 120)
+                self.update()
+
+        # Determine relative position
+        if True:
+            position_x = parent.winfo_x()
+            position_y = parent.winfo_y()
+            height = parent.winfo_height()
+            width = parent.winfo_width()
+
+            local_height = self.minsize()[1]
+            local_width = self.minsize()[0]
+
+            final_position = (position_x + width / 2 - local_width / 2, position_y + height / 2 - local_height / 2)
+            self.geometry('%dx%d+%d+%d' % (local_width, local_height, final_position[0], final_position[1]))
+            self.grab_set()
+
+    def update_progress_bar(self):
+
+        step_number = 50
+        step = int(self.total_time_ms / step_number)
+
+        for i in range(step_number):
+            self.after(step)
+            self.progressbar_var.set((i + 1) * step)
+            self.progressbar.update()
+        self.destroy()
+
+
+    def show(self):
+        self.update()
+        self.deiconify()
+        self.update_progress_bar()
+        return
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `compoundwidgets-0.1.9/compoundwidgets/__init__.py` & `compoundwidgets-0.2.0/compoundwidgets/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,53 @@
-__version__ = "0.1.9"
+__version__ = "0.2.00"
 __author__ = 'Andre Mariano'
-__all__ = ['COMPOUND_WIDGETS', 'CUSTOM_BUTTONS', 'CUSTOM_FRAMES', 'MESSAGE_BOX_WIDGETS', 'IMAGES']
+__all__ = ['AUTOCOMPLETE_WIDGETS',
+           'COMPOUND_WIDGETS',
+           'CUSTOM_BUTTONS',
+           'CUSTOM_FRAMES',
+           'MESSAGE_BOX_WIDGETS',
+           'IMAGES',
+           'SCRIPTS']
+
+from .AUTOCOMPLETE_WIDGETS import AutocompleteEntryList
 
-from .COMPOUND_WIDGETS import CheckLedButton
 from .COMPOUND_WIDGETS import LabelCombo
+from .COMPOUND_WIDGETS import LabelComboButton
 from .COMPOUND_WIDGETS import LabelEntry
+from .COMPOUND_WIDGETS import LabelEntryButton
 from .COMPOUND_WIDGETS import LabelEntryUnit
-from .COMPOUND_WIDGETS import LabelText
-from .COMPOUND_WIDGETS import LedButton
-from .COMPOUND_WIDGETS import RadioLedButton
 from .COMPOUND_WIDGETS import LabelSpinbox
+from .COMPOUND_WIDGETS import LabelText
 
+from .CUSTOM_BUTTONS import AddNewButton
 from .CUSTOM_BUTTONS import AddToReport
 from .CUSTOM_BUTTONS import BackButton
 from .CUSTOM_BUTTONS import CalculateButton
 from .CUSTOM_BUTTONS import CancelButton
 from .CUSTOM_BUTTONS import ClearButton
 from .CUSTOM_BUTTONS import EditReport
+from .CUSTOM_BUTTONS import EraseButton
 from .CUSTOM_BUTTONS import HelpButton
 from .CUSTOM_BUTTONS import NoButton
+from .CUSTOM_BUTTONS import OKButton
+from .CUSTOM_BUTTONS import QuitButton
 from .CUSTOM_BUTTONS import RemoveFromReport
 from .CUSTOM_BUTTONS import SaveButton
 from .CUSTOM_BUTTONS import YesButton
 
 from .CUSTOM_FRAMES import CollapsableFrame
 from .CUSTOM_FRAMES import ScrollableFrame
+from .CUSTOM_FRAMES import VCollapsableFrame
+
+from .LED_BUTTONS import CheckLedButton
+from .LED_BUTTONS import LedButton
+from .LED_BUTTONS import RadioLedButton
 
 from .MESSAGE_BOX_WIDGETS import OkCancelBox
 from .MESSAGE_BOX_WIDGETS import ProgressBar
+from .MESSAGE_BOX_WIDGETS import SuccessBox
+from .MESSAGE_BOX_WIDGETS import TimedBox
 from .MESSAGE_BOX_WIDGETS import Tooltip
 from .MESSAGE_BOX_WIDGETS import WarningBox
 from .MESSAGE_BOX_WIDGETS import YesNoBox
+
+from .SCRIPTS import *
```

### Comparing `compoundwidgets-0.1.9/setup.py` & `compoundwidgets-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='compoundwidgets',
-    version='0.1.9',
+    version='0.2.00',
     author='Andre Mariano',
     license="MIT",
     url='https://github.com/AndreMariano100/CompoundWidgets.git',
     description='Compound TTK Widgets with ttkbootstrap',
     author_email='andremariano100@gmail.com',
     packages=['compoundwidgets', 'compoundwidgets.IMAGES'],
     install_requires=['ttkbootstrap', 'Pillow'],
```

### Comparing `compoundwidgets-0.1.9/test/test_scrollable_frame.py` & `compoundwidgets-0.2.0/test/custom_frames_test_3.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 import tkinter as tk
-import tkinter.ttk as ttk
+import ttkbootstrap as ttk
 from ttkbootstrap import Style
 import compoundwidgets as cw
 
 root = tk.Tk()
 root.columnconfigure(0, weight=1)
 
 root.geometry(f'600x300+200+50')
 root.title('Scrollable frame test')
-
-# All compound widgets use ttkboostrap Style
 root.style = Style(theme='darkly')
 
 root.columnconfigure(0, weight=1)
 root.rowconfigure(0, weight=1)
 
 # Create frame instance
 frame = cw.ScrollableFrame(root)
 frame.grid(row=0, column=0, sticky='nsew', padx=10, pady=10)
-# The scroll is not active while all widgets fit in the frame
 
 # To add widgets to the frame, they shall be children of its 'widgets_frame' as follows
-frame.widgets_frame.columnconfigure(0, weight=1)
-for i in range(20):
-    label = ttk.Label(frame.widgets_frame, text=f'This is label {i}')
-    label.grid(row=i, column=0, sticky='nsew', pady=5)
+frame.columnconfigure(0, weight=1)
+for i in range(10):
+    label = ttk.Label(frame, text=f'This is label {i}', style='secondary.Inverse.TLabel')
+    label.grid(row=i, column=0, sticky='nsew', pady=5, padx=20)
 
-# the srollable frame does not behave apropriatelly if you use two of the on the same container
+# the scrollable frame does not behave apropriately if you use two of the on the same container
 
 root.mainloop()
```

