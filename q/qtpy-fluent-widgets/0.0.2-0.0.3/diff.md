# Comparing `tmp/QtPy-Fluent-Widgets-0.0.2.tar.gz` & `tmp/QtPy-Fluent-Widgets-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QtPy-Fluent-Widgets-0.0.2.tar", last modified: Mon Apr 10 12:09:21 2023, max compression
+gzip compressed data, was "QtPy-Fluent-Widgets-0.0.3.tar", last modified: Wed Apr 12 15:21:13 2023, max compression
```

## Comparing `QtPy-Fluent-Widgets-0.0.2.tar` & `QtPy-Fluent-Widgets-0.0.3.tar`

### file list

```diff
@@ -1,284 +1,284 @@
--rw-r--r--   0        0        0    35823 2023-04-10 08:38:48.343855 QtPy-Fluent-Widgets-0.0.2/LICENSE
--rw-r--r--   0        0        0     1198 2023-04-10 12:08:40.135836 QtPy-Fluent-Widgets-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      493 2023-04-10 10:35:11.915022 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 08:43:27.190572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/__init__.py
--rw-r--r--   0        0        0   271829 2023-04-10 08:43:27.192574 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/acrylic/noise.png
--rw-r--r--   0        0        0      611 2023-04-10 08:43:27.192574 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/check_box/Accept_black.svg
--rw-r--r--   0        0        0      611 2023-04-10 08:43:27.193572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/check_box/Accept_white.svg
--rw-r--r--   0        0        0      546 2023-04-10 08:43:27.193572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/check_box/PartialAccept_black.svg
--rw-r--r--   0        0        0      546 2023-04-10 08:43:27.194584 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/check_box/PartialAccept_white.svg
--rw-r--r--   0        0        0     1018 2023-04-10 08:43:27.194584 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/color_dialog/Clear_black.svg
--rw-r--r--   0        0        0     1018 2023-04-10 08:43:27.195572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/color_dialog/Clear_white.svg
--rw-r--r--   0        0        0    18226 2023-04-10 08:43:27.195572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/color_dialog/HuePanel.png
--rw-r--r--   0        0        0      136 2023-04-10 08:43:27.195572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/folder_list_dialog/Add_black.png
--rw-r--r--   0        0        0      132 2023-04-10 08:43:27.195572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/folder_list_dialog/Add_white.png
--rw-r--r--   0        0        0      324 2023-04-10 08:43:27.196572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/folder_list_dialog/Close_black.png
--rw-r--r--   0        0        0      341 2023-04-10 08:43:27.196572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/folder_list_dialog/Close_white.png
--rw-r--r--   0        0        0     1637 2023-04-10 08:43:27.196572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Add_black.svg
--rw-r--r--   0        0        0     1637 2023-04-10 08:43:27.196572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Add_white.svg
--rw-r--r--   0        0        0     2549 2023-04-10 08:43:27.197573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Album_black.svg
--rw-r--r--   0        0        0     2549 2023-04-10 08:43:27.197573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Album_white.svg
--rw-r--r--   0        0        0     2152 2023-04-10 08:43:27.197573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Alignment_black.svg
--rw-r--r--   0        0        0     2152 2023-04-10 08:43:27.198579 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Alignment_white.svg
--rw-r--r--   0        0        0     4140 2023-04-10 08:43:27.198579 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/BackgroundColor_black.svg
--rw-r--r--   0        0        0     4140 2023-04-10 08:43:27.198579 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/BackgroundColor_white.svg
--rw-r--r--   0        0        0     1920 2023-04-10 08:43:27.198579 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/BookShelf_black.svg
--rw-r--r--   0        0        0     1920 2023-04-10 08:43:27.199573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/BookShelf_white.svg
--rw-r--r--   0        0        0     3724 2023-04-10 08:43:27.199573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Brush_black.svg
--rw-r--r--   0        0        0     3724 2023-04-10 08:43:27.199573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Brush_white.svg
--rw-r--r--   0        0        0     1961 2023-04-10 08:43:27.200572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Camera_black.svg
--rw-r--r--   0        0        0     1961 2023-04-10 08:43:27.200572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Camera_white.svg
--rw-r--r--   0        0        0     3528 2023-04-10 08:43:27.200572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Cancel_black.svg
--rw-r--r--   0        0        0     3528 2023-04-10 08:43:27.201575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Cancel_white.svg
--rw-r--r--   0        0        0     2827 2023-04-10 08:43:27.201575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Chat_black.svg
--rw-r--r--   0        0        0     2827 2023-04-10 08:43:27.201575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Chat_white.svg
--rw-r--r--   0        0        0     1171 2023-04-10 08:43:27.201575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/CheckBox_black.svg
--rw-r--r--   0        0        0     1171 2023-04-10 08:43:27.202572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/CheckBox_white.svg
--rw-r--r--   0        0        0     1077 2023-04-10 08:43:27.202572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/ChevronDown_black.svg
--rw-r--r--   0        0        0     1058 2023-04-10 08:43:27.202572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/ChevronDown_white.svg
--rw-r--r--   0        0        0      769 2023-04-10 08:43:27.202572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/ChevronRight_black.svg
--rw-r--r--   0        0        0      769 2023-04-10 08:43:27.203572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/ChevronRight_white.svg
--rw-r--r--   0        0        0     1022 2023-04-10 08:43:27.203572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Close_black.svg
--rw-r--r--   0        0        0     1022 2023-04-10 08:43:27.203572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Close_white.svg
--rw-r--r--   0        0        0     1759 2023-04-10 08:43:27.203572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Code_black.svg
--rw-r--r--   0        0        0     1759 2023-04-10 08:43:27.203572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Code_white.svg
--rw-r--r--   0        0        0     4323 2023-04-10 08:43:27.204573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Completed_black.svg
--rw-r--r--   0        0        0     4325 2023-04-10 08:43:27.204573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Completed_white.svg
--rw-r--r--   0        0        0     1968 2023-04-10 08:43:27.204573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Constract_black.svg
--rw-r--r--   0        0        0     1968 2023-04-10 08:43:27.204573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Constract_white.svg
--rw-r--r--   0        0        0     4091 2023-04-10 08:43:27.205573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Copy_black.svg
--rw-r--r--   0        0        0     4091 2023-04-10 08:43:27.205573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Copy_white.svg
--rw-r--r--   0        0        0     5785 2023-04-10 08:43:27.205573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Cut_black.svg
--rw-r--r--   0        0        0     5785 2023-04-10 08:43:27.206575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Cut_white.svg
--rw-r--r--   0        0        0     1458 2023-04-10 08:43:27.206575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Delete_black.svg
--rw-r--r--   0        0        0     1458 2023-04-10 08:43:27.206575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Delete_white.svg
--rw-r--r--   0        0        0     1104 2023-04-10 08:43:27.206575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Document_black.svg
--rw-r--r--   0        0        0     1104 2023-04-10 08:43:27.207579 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Document_white.svg
--rw-r--r--   0        0        0     2948 2023-04-10 08:43:27.207579 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Download_black.svg
--rw-r--r--   0        0        0     2948 2023-04-10 08:43:27.207579 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Download_white.svg
--rw-r--r--   0        0        0     1218 2023-04-10 08:43:27.207579 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Edit_black.svg
--rw-r--r--   0        0        0     1218 2023-04-10 08:43:27.208575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Edit_white.svg
--rw-r--r--   0        0        0     2809 2023-04-10 08:43:27.208575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Embed_black.svg
--rw-r--r--   0        0        0     2809 2023-04-10 08:43:27.208575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Embed_white.svg
--rw-r--r--   0        0        0     6962 2023-04-10 08:43:27.208575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Feedback_black.svg
--rw-r--r--   0        0        0     6962 2023-04-10 08:43:27.209572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Feedback_white.svg
--rw-r--r--   0        0        0     1675 2023-04-10 08:43:27.210572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Folder_black.svg
--rw-r--r--   0        0        0     1675 2023-04-10 08:43:27.210572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Folder_white.svg
--rw-r--r--   0        0        0     5168 2023-04-10 08:43:27.209572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/FolderAdd_black.svg
--rw-r--r--   0        0        0     5168 2023-04-10 08:43:27.209572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/FolderAdd_white.svg
--rw-r--r--   0        0        0     4627 2023-04-10 08:43:27.211573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Font_black.svg
--rw-r--r--   0        0        0     4627 2023-04-10 08:43:27.211573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Font_white.svg
--rw-r--r--   0        0        0      963 2023-04-10 08:43:27.211573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/GitHub_black.svg
--rw-r--r--   0        0        0      960 2023-04-10 08:43:27.212542 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/GitHub_white.svg
--rw-r--r--   0        0        0     6603 2023-04-10 08:43:27.212542 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Globe_black.svg
--rw-r--r--   0        0        0     6603 2023-04-10 08:43:27.212542 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Globe_white.svg
--rw-r--r--   0        0        0     1246 2023-04-10 08:43:27.212542 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Heart_black.svg
--rw-r--r--   0        0        0     1246 2023-04-10 08:43:27.213574 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Heart_white.svg
--rw-r--r--   0        0        0     7474 2023-04-10 08:43:27.213574 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Help_black.svg
--rw-r--r--   0        0        0     7474 2023-04-10 08:43:27.213574 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Help_white.svg
--rw-r--r--   0        0        0     1992 2023-04-10 08:43:27.213574 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Hide_black.svg
--rw-r--r--   0        0        0     1992 2023-04-10 08:43:27.214572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Hide_white.svg
--rw-r--r--   0        0        0     3197 2023-04-10 08:43:27.214572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Highlight_black.svg
--rw-r--r--   0        0        0     3197 2023-04-10 08:43:27.214572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Highlight_white.svg
--rw-r--r--   0        0        0     2288 2023-04-10 08:43:27.214572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/History_black.svg
--rw-r--r--   0        0        0     2288 2023-04-10 08:43:27.215572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/History_white.svg
--rw-r--r--   0        0        0     1653 2023-04-10 08:43:27.215572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Home_black.svg
--rw-r--r--   0        0        0     1653 2023-04-10 08:43:27.215572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Home_white.svg
--rw-r--r--   0        0        0     5845 2023-04-10 08:43:27.216573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Info_black.svg
--rw-r--r--   0        0        0     5845 2023-04-10 08:43:27.216573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Info_white.svg
--rw-r--r--   0        0        0     7159 2023-04-10 08:43:27.216573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Language_black.svg
--rw-r--r--   0        0        0     7159 2023-04-10 08:43:27.216573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Language_white.svg
--rw-r--r--   0        0        0     1439 2023-04-10 08:43:27.217575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Layout_black.svg
--rw-r--r--   0        0        0     1439 2023-04-10 08:43:27.217575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Layout_white.svg
--rw-r--r--   0        0        0     4311 2023-04-10 08:43:27.218544 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Link_black.svg
--rw-r--r--   0        0        0     4311 2023-04-10 08:43:27.218544 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Link_white.svg
--rw-r--r--   0        0        0     1078 2023-04-10 08:43:27.218544 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Mail_black.svg
--rw-r--r--   0        0        0     1078 2023-04-10 08:43:27.219572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Mail_white.svg
--rw-r--r--   0        0        0     2947 2023-04-10 08:43:27.219572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Media_black.svg
--rw-r--r--   0        0        0     2947 2023-04-10 08:43:27.219572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Media_white.svg
--rw-r--r--   0        0        0     2518 2023-04-10 08:43:27.219572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Menu_black copy.svg
--rw-r--r--   0        0        0     1228 2023-04-10 08:43:27.220573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Menu_black.svg
--rw-r--r--   0        0        0     2518 2023-04-10 08:43:27.220573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Menu_white copy.svg
--rw-r--r--   0        0        0     1228 2023-04-10 08:43:27.220573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Menu_white.svg
--rw-r--r--   0        0        0     1863 2023-04-10 08:43:27.221552 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Message_black.svg
--rw-r--r--   0        0        0     1863 2023-04-10 08:43:27.221552 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Message_white.svg
--rw-r--r--   0        0        0     1529 2023-04-10 08:43:27.222575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Microphone_black.svg
--rw-r--r--   0        0        0     1529 2023-04-10 08:43:27.222575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Microphone_white.svg
--rw-r--r--   0        0        0     4953 2023-04-10 08:43:27.222575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Minimize_black.svg
--rw-r--r--   0        0        0     4953 2023-04-10 08:43:27.223573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Minimize_white.svg
--rw-r--r--   0        0        0     1594 2023-04-10 08:43:27.223573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/More_black.svg
--rw-r--r--   0        0        0     1594 2023-04-10 08:43:27.223573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/More_white.svg
--rw-r--r--   0        0        0     3871 2023-04-10 08:43:27.223573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Movie_black.svg
--rw-r--r--   0        0        0     3871 2023-04-10 08:43:27.224573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Movie_white.svg
--rw-r--r--   0        0        0     4478 2023-04-10 08:43:27.224573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Music_black.svg
--rw-r--r--   0        0        0     4478 2023-04-10 08:43:27.225581 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Music_white.svg
--rw-r--r--   0        0        0     4087 2023-04-10 08:43:27.224573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/MusicFolder_black.svg
--rw-r--r--   0        0        0     4087 2023-04-10 08:43:27.224573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/MusicFolder_white.svg
--rw-r--r--   0        0        0     8283 2023-04-10 08:43:27.225581 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Palette_black.svg
--rw-r--r--   0        0        0     8283 2023-04-10 08:43:27.225581 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Palette_white.svg
--rw-r--r--   0        0        0     2365 2023-04-10 08:43:27.226573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Paste_black.svg
--rw-r--r--   0        0        0     2365 2023-04-10 08:43:27.226573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Paste_white.svg
--rw-r--r--   0        0        0     5500 2023-04-10 08:43:27.226573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/PencilInk_black.svg
--rw-r--r--   0        0        0     5500 2023-04-10 08:43:27.227580 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/PencilInk_white.svg
--rw-r--r--   0        0        0     1948 2023-04-10 08:43:27.227580 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Phone_black.svg
--rw-r--r--   0        0        0     1948 2023-04-10 08:43:27.227580 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Phone_white.svg
--rw-r--r--   0        0        0     2023 2023-04-10 08:43:27.227580 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Photo_black.svg
--rw-r--r--   0        0        0     2023 2023-04-10 08:43:27.228572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Photo_white.svg
--rw-r--r--   0        0        0     1261 2023-04-10 08:43:27.228572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Pin_black.svg
--rw-r--r--   0        0        0     1261 2023-04-10 08:43:27.228572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Pin_white.svg
--rw-r--r--   0        0        0     1626 2023-04-10 08:43:27.228572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Print_black.svg
--rw-r--r--   0        0        0     1626 2023-04-10 08:43:27.229573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Print_white.svg
--rw-r--r--   0        0        0     3631 2023-04-10 08:43:27.229573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Question_black.svg
--rw-r--r--   0        0        0     3631 2023-04-10 08:43:27.229573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Question_white.svg
--rw-r--r--   0        0        0      638 2023-04-10 08:43:27.229573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Return_black.svg
--rw-r--r--   0        0        0      638 2023-04-10 08:43:27.230573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Return_white.svg
--rw-r--r--   0        0        0     2230 2023-04-10 08:43:27.230573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Ringer_black.svg
--rw-r--r--   0        0        0     2230 2023-04-10 08:43:27.230573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Ringer_white.svg
--rw-r--r--   0        0        0     1897 2023-04-10 08:43:27.231577 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Save_black.svg
--rw-r--r--   0        0        0     1897 2023-04-10 08:43:27.232572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Save_white.svg
--rw-r--r--   0        0        0     2498 2023-04-10 08:43:27.230573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/SaveAs_black.svg
--rw-r--r--   0        0        0     2498 2023-04-10 08:43:27.231577 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/SaveAs_white.svg
--rw-r--r--   0        0        0      933 2023-04-10 08:43:27.232572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Scroll_black.svg
--rw-r--r--   0        0        0      933 2023-04-10 08:43:27.232572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Scroll_white.svg
--rw-r--r--   0        0        0     3967 2023-04-10 08:43:27.233573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Search_black.svg
--rw-r--r--   0        0        0     3967 2023-04-10 08:43:27.233573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Search_white.svg
--rw-r--r--   0        0        0      683 2023-04-10 08:43:27.234573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Send_black.svg
--rw-r--r--   0        0        0      683 2023-04-10 08:43:27.234573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Send_white.svg
--rw-r--r--   0        0        0      701 2023-04-10 08:43:27.233573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/SendFill_black.svg
--rw-r--r--   0        0        0      701 2023-04-10 08:43:27.233573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/SendFill_white.svg
--rw-r--r--   0        0        0    10042 2023-04-10 08:43:27.234573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Setting_black.svg
--rw-r--r--   0        0        0    10042 2023-04-10 08:43:27.235544 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Setting_white.svg
--rw-r--r--   0        0        0     2237 2023-04-10 08:43:27.235544 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Share_black.svg
--rw-r--r--   0        0        0     2237 2023-04-10 08:43:27.235544 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Share_white.svg
--rw-r--r--   0        0        0     3508 2023-04-10 08:43:27.235544 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Sync_black.svg
--rw-r--r--   0        0        0     3510 2023-04-10 08:43:27.236574 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Sync_white.svg
--rw-r--r--   0        0        0     1579 2023-04-10 08:43:27.236574 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Tag_black.svg
--rw-r--r--   0        0        0     1579 2023-04-10 08:43:27.236574 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Tag_white.svg
--rw-r--r--   0        0        0     8499 2023-04-10 08:43:27.237573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Transparent_black.svg
--rw-r--r--   0        0        0     8499 2023-04-10 08:43:27.237573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Transparent_white.svg
--rw-r--r--   0        0        0     1388 2023-04-10 08:43:27.237573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Unpin_black.svg
--rw-r--r--   0        0        0     1388 2023-04-10 08:43:27.237573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Unpin_white.svg
--rw-r--r--   0        0        0     8989 2023-04-10 08:43:27.238572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Update_black.svg
--rw-r--r--   0        0        0     8989 2023-04-10 08:43:27.238572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Update_white.svg
--rw-r--r--   0        0        0     6996 2023-04-10 08:43:27.239573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Video_black.svg
--rw-r--r--   0        0        0     6996 2023-04-10 08:43:27.239573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Video_white.svg
--rw-r--r--   0        0        0     2312 2023-04-10 08:43:27.240573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/View_black.svg
--rw-r--r--   0        0        0     2312 2023-04-10 08:43:27.240573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/View_white.svg
--rw-r--r--   0        0        0     2120 2023-04-10 08:43:27.240573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/ZipFolder_black.svg
--rw-r--r--   0        0        0     2120 2023-04-10 08:43:27.240573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/ZipFolder_white.svg
--rw-r--r--   0        0        0     5993 2023-04-10 08:43:27.242543 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Zoom_black.svg
--rw-r--r--   0        0        0     5993 2023-04-10 08:43:27.242543 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Zoom_white.svg
--rw-r--r--   0        0        0     1911 2023-04-10 08:43:27.241572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/ZoomIn_black.svg
--rw-r--r--   0        0        0     1911 2023-04-10 08:43:27.241572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/ZoomIn_white.svg
--rw-r--r--   0        0        0     1721 2023-04-10 08:43:27.242543 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/ZoomOut_black.svg
--rw-r--r--   0        0        0     1721 2023-04-10 08:43:27.242543 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/ZoomOut_white.svg
--rw-r--r--   0        0        0     1585 2023-04-10 08:43:27.243573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/info_bar/Error_dark.svg
--rw-r--r--   0        0        0     1588 2023-04-10 08:43:27.243573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/info_bar/Error_light.svg
--rw-r--r--   0        0        0     1393 2023-04-10 08:43:27.243573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/info_bar/Info_dark.svg
--rw-r--r--   0        0        0     1396 2023-04-10 08:43:27.243573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/info_bar/Info_light.svg
--rw-r--r--   0        0        0     1351 2023-04-10 08:43:27.244573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/info_bar/Success_dark.svg
--rw-r--r--   0        0        0     1356 2023-04-10 08:43:27.244573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/info_bar/Success_light.svg
--rw-r--r--   0        0        0     1397 2023-04-10 08:43:27.244573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/info_bar/Warning_dark.svg
--rw-r--r--   0        0        0     1400 2023-04-10 08:43:27.244573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/info_bar/Warning_light.svg
--rw-r--r--   0        0        0      583 2023-04-10 08:43:27.245581 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/spin_box/Down_black.svg
--rw-r--r--   0        0        0      669 2023-04-10 08:43:27.245581 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/spin_box/Down_white.svg
--rw-r--r--   0        0        0      579 2023-04-10 08:43:27.245581 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/spin_box/Up_black.svg
--rw-r--r--   0        0        0      665 2023-04-10 08:43:27.246543 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/spin_box/Up_white.svg
--rw-r--r--   0        0        0      646 2023-04-10 11:42:11.353289 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/tree_view/TreeViewClose_black.svg
--rw-r--r--   0        0        0      646 2023-04-10 11:42:11.353289 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/tree_view/TreeViewClose_white.svg
--rw-r--r--   0        0        0      763 2023-04-10 11:42:11.353289 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/tree_view/TreeViewOpen_black.svg
--rw-r--r--   0        0        0      763 2023-04-10 11:42:11.353289 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/tree_view/TreeViewOpen_white.svg
--rw-r--r--   0        0        0     3937 2023-04-10 08:43:27.246543 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/button.qss
--rw-r--r--   0        0        0     1623 2023-04-10 08:43:27.246543 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/check_box.qss
--rw-r--r--   0        0        0     3016 2023-04-10 08:43:27.247576 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/color_dialog.qss
--rw-r--r--   0        0        0     1481 2023-04-10 08:43:27.247576 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/combo_box.qss
--rw-r--r--   0        0        0     1504 2023-04-10 08:43:27.247576 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/dialog.qss
--rw-r--r--   0        0        0     2162 2023-04-10 08:43:27.248572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/expand_setting_card.qss
--rw-r--r--   0        0        0     1569 2023-04-10 08:43:27.248572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/folder_list_dialog.qss
--rw-r--r--   0        0        0      848 2023-04-10 08:43:27.248572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/info_bar.qss
--rw-r--r--   0        0        0     2184 2023-04-10 08:43:27.249575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/line_edit.qss
--rw-r--r--   0        0        0     1605 2023-04-10 08:43:27.249575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/menu.qss
--rw-r--r--   0        0        0      813 2023-04-10 08:43:27.249575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/message_dialog.qss
--rw-r--r--   0        0        0      524 2023-04-10 08:43:27.249575 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/navigation_interface.qss
--rw-r--r--   0        0        0     1670 2023-04-10 09:33:25.271948 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/setting_card.qss
--rw-r--r--   0        0        0      212 2023-04-10 08:43:27.251573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/setting_card_group.qss
--rw-r--r--   0        0        0     2543 2023-04-10 08:43:27.251573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/slider.qss
--rw-r--r--   0        0        0     1420 2023-04-10 08:43:27.251573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/spin_box.qss
--rw-r--r--   0        0        0      355 2023-04-10 08:43:27.251573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/state_tool_tip.qss
--rw-r--r--   0        0        0     1403 2023-04-10 08:43:27.252573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/switch_button.qss
--rw-r--r--   0        0        0      309 2023-04-10 08:43:27.252573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/tool_tip.qss
--rw-r--r--   0        0        0     2761 2023-04-10 11:42:11.354289 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/tree_view.qss
--rw-r--r--   0        0        0     3985 2023-04-10 08:43:27.252573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/button.qss
--rw-r--r--   0        0        0     1634 2023-04-10 08:43:27.253572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/check_box.qss
--rw-r--r--   0        0        0     3027 2023-04-10 08:43:27.253572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/color_dialog.qss
--rw-r--r--   0        0        0     1423 2023-04-10 08:43:27.253572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/combo_box.qss
--rw-r--r--   0        0        0     1518 2023-04-10 08:43:27.253572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/dialog.qss
--rw-r--r--   0        0        0     2167 2023-04-10 08:43:27.253572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/expand_setting_card.qss
--rw-r--r--   0        0        0     1435 2023-04-10 08:43:27.254573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/folder_list_dialog.qss
--rw-r--r--   0        0        0      854 2023-04-10 08:43:27.254573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/info_bar.qss
--rw-r--r--   0        0        0     2196 2023-04-10 08:43:27.254573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/line_edit.qss
--rw-r--r--   0        0        0     1521 2023-04-10 08:43:27.255573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/menu.qss
--rw-r--r--   0        0        0      802 2023-04-10 08:43:27.255573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/message_dialog.qss
--rw-r--r--   0        0        0      532 2023-04-10 08:43:27.255573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/navigation_interface.qss
--rw-r--r--   0        0        0     1658 2023-04-10 08:43:27.255573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/setting_card.qss
--rw-r--r--   0        0        0      210 2023-04-10 08:43:27.255573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/setting_card_group.qss
--rw-r--r--   0        0        0     2931 2023-04-10 08:43:27.256574 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/slider.qss
--rw-r--r--   0        0        0     1416 2023-04-10 08:43:27.256574 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/spin_box.qss
--rw-r--r--   0        0        0      354 2023-04-10 08:43:27.256574 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/state_tool_tip.qss
--rw-r--r--   0        0        0     1414 2023-04-10 08:43:27.256574 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/switch_button.qss
--rw-r--r--   0        0        0      318 2023-04-10 08:43:27.257581 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/tool_tip.qss
--rw-r--r--   0        0        0     2772 2023-04-10 11:42:11.354289 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/tree_view.qss
--rw-r--r--   0        0        0  3473858 2023-04-10 11:48:57.559462 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/resource.py
--rw-r--r--   0        0        0    11723 2023-04-10 11:42:11.398294 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/resource.qrc
--rw-r--r--   0        0        0  1637139 2023-04-10 11:50:59.545473 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/resource_rc.py
--rw-r--r--   0        0        0      390 2023-04-10 08:43:27.273573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/common/__init__.py
--rw-r--r--   0        0        0     3193 2023-04-10 08:43:27.273573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/common/auto_wrap.py
--rw-r--r--   0        0        0    10560 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/common/config.py
--rw-r--r--   0        0        0      675 2023-04-10 08:43:27.274572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/common/exception_handler.py
--rw-r--r--   0        0        0     7211 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/common/icon.py
--rw-r--r--   0        0        0     4782 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/common/image_utils.py
--rw-r--r--   0        0        0     4796 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/common/smooth_scroll.py
--rw-r--r--   0        0        0     6990 2023-04-10 11:44:26.750465 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/common/style_sheet.py
--rw-r--r--   0        0        0      124 2023-04-10 11:41:52.425867 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/__init__.py
--rw-r--r--   0        0        0      170 2023-04-10 08:43:27.276573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/dialog_box/__init__.py
--rw-r--r--   0        0        0    11987 2023-04-10 10:39:04.022260 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/dialog_box/color_dialog.py
--rw-r--r--   0        0        0     5250 2023-04-10 11:09:38.442297 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/dialog_box/dialog.py
--rw-r--r--   0        0        0    11235 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/dialog_box/folder_list_dialog.py
--rw-r--r--   0        0        0     3196 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/dialog_box/mask_dialog_base.py
--rw-r--r--   0        0        0     2486 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/dialog_box/message_dialog.py
--rw-r--r--   0        0        0      114 2023-04-10 08:43:27.278573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/layout/__init__.py
--rw-r--r--   0        0        0     2649 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/layout/expand_layout.py
--rw-r--r--   0        0        0     5431 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/layout/flow_layout.py
--rw-r--r--   0        0        0     1299 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/layout/v_box_layout.py
--rw-r--r--   0        0        0      260 2023-04-10 08:43:27.280572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/navigation/__init__.py
--rw-r--r--   0        0        0     4245 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/navigation/navigation_interface.py
--rw-r--r--   0        0        0    14424 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/navigation/navigation_panel.py
--rw-r--r--   0        0        0     4864 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/navigation/navigation_widget.py
--rw-r--r--   0        0        0      550 2023-04-10 08:43:27.281572 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/settings/__init__.py
--rw-r--r--   0        0        0     5186 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/settings/custom_color_setting_card.py
--rw-r--r--   0        0        0     8017 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/settings/expand_setting_card.py
--rw-r--r--   0        0        0     6019 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/settings/folder_list_setting_card.py
--rw-r--r--   0        0        0     2829 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/settings/options_setting_card.py
--rw-r--r--   0        0        0    12810 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/settings/setting_card.py
--rw-r--r--   0        0        0     1510 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/settings/setting_card_group.py
--rw-r--r--   0        0        0      915 2023-04-10 11:42:22.643239 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/__init__.py
--rw-r--r--   0        0        0     4587 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/acrylic_label.py
--rw-r--r--   0        0        0     4641 2023-04-10 10:35:11.922022 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/button.py
--rw-r--r--   0        0        0      303 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/check_box.py
--rw-r--r--   0        0        0    13473 2023-04-10 10:35:11.922022 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/combo_box.py
--rw-r--r--   0        0        0      701 2023-04-10 12:02:57.033746 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/icon_widget.py
--rw-r--r--   0        0        0    18826 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/info_bar.py
--rw-r--r--   0        0        0      855 2023-04-10 10:35:11.964022 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/label.py
--rw-r--r--   0        0        0     5747 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/line_edit.py
--rw-r--r--   0        0        0    23261 2023-04-10 10:47:10.716030 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/menu.py
--rw-r--r--   0        0        0     4505 2023-04-10 10:35:11.967022 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/scroll_area.py
--rw-r--r--   0        0        0     5047 2023-04-10 11:33:41.269573 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/slider.py
--rw-r--r--   0        0        0     4389 2023-04-10 10:35:11.985023 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/spin_box.py
--rw-r--r--   0        0        0     6308 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/stacked_widget.py
--rw-r--r--   0        0        0     5786 2023-04-10 10:35:11.985023 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/state_tool_tip.py
--rw-r--r--   0        0        0     6568 2023-04-10 10:35:11.985023 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/switch_button.py
--rw-r--r--   0        0        0     1651 2023-04-10 10:35:11.985023 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/three_state_button.py
--rw-r--r--   0        0        0     5166 2023-04-10 10:35:11.985023 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/tool_tip.py
--rw-r--r--   0        0        0     2826 2023-04-10 08:41:41.422117 QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/tree_view.py
--rw-r--r--   0        0        0     3022 2023-04-10 09:12:49.197878 QtPy-Fluent-Widgets-0.0.2/README.md
--rw-r--r--   0        0        0     3771 1970-01-01 00:00:00.000000 QtPy-Fluent-Widgets-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-04-10 08:38:48.343855 QtPy-Fluent-Widgets-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1064 2023-04-12 15:20:30.126134 QtPy-Fluent-Widgets-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      493 2023-04-10 10:35:11.915022 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 08:43:27.190572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/__init__.py
+-rw-r--r--   0        0        0   271829 2023-04-10 08:43:27.192574 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/acrylic/noise.png
+-rw-r--r--   0        0        0      611 2023-04-10 08:43:27.192574 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/check_box/Accept_black.svg
+-rw-r--r--   0        0        0      611 2023-04-10 08:43:27.193572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/check_box/Accept_white.svg
+-rw-r--r--   0        0        0      546 2023-04-10 08:43:27.193572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/check_box/PartialAccept_black.svg
+-rw-r--r--   0        0        0      546 2023-04-10 08:43:27.194584 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/check_box/PartialAccept_white.svg
+-rw-r--r--   0        0        0     1018 2023-04-10 08:43:27.194584 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/color_dialog/Clear_black.svg
+-rw-r--r--   0        0        0     1018 2023-04-10 08:43:27.195572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/color_dialog/Clear_white.svg
+-rw-r--r--   0        0        0    18226 2023-04-10 08:43:27.195572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/color_dialog/HuePanel.png
+-rw-r--r--   0        0        0      136 2023-04-10 08:43:27.195572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/folder_list_dialog/Add_black.png
+-rw-r--r--   0        0        0      132 2023-04-10 08:43:27.195572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/folder_list_dialog/Add_white.png
+-rw-r--r--   0        0        0      324 2023-04-10 08:43:27.196572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/folder_list_dialog/Close_black.png
+-rw-r--r--   0        0        0      341 2023-04-10 08:43:27.196572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/folder_list_dialog/Close_white.png
+-rw-r--r--   0        0        0     1637 2023-04-10 08:43:27.196572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Add_black.svg
+-rw-r--r--   0        0        0     1637 2023-04-10 08:43:27.196572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Add_white.svg
+-rw-r--r--   0        0        0     2549 2023-04-10 08:43:27.197573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Album_black.svg
+-rw-r--r--   0        0        0     2549 2023-04-10 08:43:27.197573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Album_white.svg
+-rw-r--r--   0        0        0     2152 2023-04-10 08:43:27.197573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Alignment_black.svg
+-rw-r--r--   0        0        0     2152 2023-04-10 08:43:27.198579 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Alignment_white.svg
+-rw-r--r--   0        0        0     4140 2023-04-10 08:43:27.198579 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/BackgroundColor_black.svg
+-rw-r--r--   0        0        0     4140 2023-04-10 08:43:27.198579 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/BackgroundColor_white.svg
+-rw-r--r--   0        0        0     1920 2023-04-10 08:43:27.198579 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/BookShelf_black.svg
+-rw-r--r--   0        0        0     1920 2023-04-10 08:43:27.199573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/BookShelf_white.svg
+-rw-r--r--   0        0        0     3724 2023-04-10 08:43:27.199573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Brush_black.svg
+-rw-r--r--   0        0        0     3724 2023-04-10 08:43:27.199573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Brush_white.svg
+-rw-r--r--   0        0        0     1961 2023-04-10 08:43:27.200572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Camera_black.svg
+-rw-r--r--   0        0        0     1961 2023-04-10 08:43:27.200572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Camera_white.svg
+-rw-r--r--   0        0        0     3528 2023-04-10 08:43:27.200572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Cancel_black.svg
+-rw-r--r--   0        0        0     3528 2023-04-10 08:43:27.201575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Cancel_white.svg
+-rw-r--r--   0        0        0     2827 2023-04-10 08:43:27.201575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Chat_black.svg
+-rw-r--r--   0        0        0     2827 2023-04-10 08:43:27.201575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Chat_white.svg
+-rw-r--r--   0        0        0     1171 2023-04-10 08:43:27.201575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/CheckBox_black.svg
+-rw-r--r--   0        0        0     1171 2023-04-10 08:43:27.202572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/CheckBox_white.svg
+-rw-r--r--   0        0        0     1077 2023-04-10 08:43:27.202572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/ChevronDown_black.svg
+-rw-r--r--   0        0        0     1058 2023-04-10 08:43:27.202572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/ChevronDown_white.svg
+-rw-r--r--   0        0        0      769 2023-04-10 08:43:27.202572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/ChevronRight_black.svg
+-rw-r--r--   0        0        0      769 2023-04-10 08:43:27.203572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/ChevronRight_white.svg
+-rw-r--r--   0        0        0     1022 2023-04-10 08:43:27.203572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Close_black.svg
+-rw-r--r--   0        0        0     1022 2023-04-10 08:43:27.203572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Close_white.svg
+-rw-r--r--   0        0        0     1759 2023-04-10 08:43:27.203572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Code_black.svg
+-rw-r--r--   0        0        0     1759 2023-04-10 08:43:27.203572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Code_white.svg
+-rw-r--r--   0        0        0     4323 2023-04-10 08:43:27.204573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Completed_black.svg
+-rw-r--r--   0        0        0     4325 2023-04-10 08:43:27.204573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Completed_white.svg
+-rw-r--r--   0        0        0     1968 2023-04-10 08:43:27.204573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Constract_black.svg
+-rw-r--r--   0        0        0     1968 2023-04-10 08:43:27.204573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Constract_white.svg
+-rw-r--r--   0        0        0     4091 2023-04-10 08:43:27.205573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Copy_black.svg
+-rw-r--r--   0        0        0     4091 2023-04-10 08:43:27.205573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Copy_white.svg
+-rw-r--r--   0        0        0     5785 2023-04-10 08:43:27.205573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Cut_black.svg
+-rw-r--r--   0        0        0     5785 2023-04-10 08:43:27.206575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Cut_white.svg
+-rw-r--r--   0        0        0     1458 2023-04-10 08:43:27.206575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Delete_black.svg
+-rw-r--r--   0        0        0     1458 2023-04-10 08:43:27.206575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Delete_white.svg
+-rw-r--r--   0        0        0     1104 2023-04-10 08:43:27.206575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Document_black.svg
+-rw-r--r--   0        0        0     1104 2023-04-10 08:43:27.207579 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Document_white.svg
+-rw-r--r--   0        0        0     2948 2023-04-10 08:43:27.207579 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Download_black.svg
+-rw-r--r--   0        0        0     2948 2023-04-10 08:43:27.207579 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Download_white.svg
+-rw-r--r--   0        0        0     1218 2023-04-10 08:43:27.207579 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Edit_black.svg
+-rw-r--r--   0        0        0     1218 2023-04-10 08:43:27.208575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Edit_white.svg
+-rw-r--r--   0        0        0     2809 2023-04-10 08:43:27.208575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Embed_black.svg
+-rw-r--r--   0        0        0     2809 2023-04-10 08:43:27.208575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Embed_white.svg
+-rw-r--r--   0        0        0     6962 2023-04-10 08:43:27.208575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Feedback_black.svg
+-rw-r--r--   0        0        0     6962 2023-04-10 08:43:27.209572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Feedback_white.svg
+-rw-r--r--   0        0        0     1675 2023-04-10 08:43:27.210572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Folder_black.svg
+-rw-r--r--   0        0        0     1675 2023-04-10 08:43:27.210572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Folder_white.svg
+-rw-r--r--   0        0        0     5168 2023-04-10 08:43:27.209572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/FolderAdd_black.svg
+-rw-r--r--   0        0        0     5168 2023-04-10 08:43:27.209572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/FolderAdd_white.svg
+-rw-r--r--   0        0        0     4627 2023-04-10 08:43:27.211573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Font_black.svg
+-rw-r--r--   0        0        0     4627 2023-04-10 08:43:27.211573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Font_white.svg
+-rw-r--r--   0        0        0      963 2023-04-10 08:43:27.211573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/GitHub_black.svg
+-rw-r--r--   0        0        0      960 2023-04-10 08:43:27.212542 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/GitHub_white.svg
+-rw-r--r--   0        0        0     6603 2023-04-10 08:43:27.212542 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Globe_black.svg
+-rw-r--r--   0        0        0     6603 2023-04-10 08:43:27.212542 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Globe_white.svg
+-rw-r--r--   0        0        0     1246 2023-04-10 08:43:27.212542 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Heart_black.svg
+-rw-r--r--   0        0        0     1246 2023-04-10 08:43:27.213574 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Heart_white.svg
+-rw-r--r--   0        0        0     7474 2023-04-10 08:43:27.213574 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Help_black.svg
+-rw-r--r--   0        0        0     7474 2023-04-10 08:43:27.213574 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Help_white.svg
+-rw-r--r--   0        0        0     1992 2023-04-10 08:43:27.213574 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Hide_black.svg
+-rw-r--r--   0        0        0     1992 2023-04-10 08:43:27.214572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Hide_white.svg
+-rw-r--r--   0        0        0     3197 2023-04-10 08:43:27.214572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Highlight_black.svg
+-rw-r--r--   0        0        0     3197 2023-04-10 08:43:27.214572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Highlight_white.svg
+-rw-r--r--   0        0        0     2288 2023-04-10 08:43:27.214572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/History_black.svg
+-rw-r--r--   0        0        0     2288 2023-04-10 08:43:27.215572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/History_white.svg
+-rw-r--r--   0        0        0     1653 2023-04-10 08:43:27.215572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Home_black.svg
+-rw-r--r--   0        0        0     1653 2023-04-10 08:43:27.215572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Home_white.svg
+-rw-r--r--   0        0        0     5845 2023-04-10 08:43:27.216573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Info_black.svg
+-rw-r--r--   0        0        0     5845 2023-04-10 08:43:27.216573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Info_white.svg
+-rw-r--r--   0        0        0     7159 2023-04-10 08:43:27.216573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Language_black.svg
+-rw-r--r--   0        0        0     7159 2023-04-10 08:43:27.216573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Language_white.svg
+-rw-r--r--   0        0        0     1439 2023-04-10 08:43:27.217575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Layout_black.svg
+-rw-r--r--   0        0        0     1439 2023-04-10 08:43:27.217575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Layout_white.svg
+-rw-r--r--   0        0        0     4311 2023-04-10 08:43:27.218544 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Link_black.svg
+-rw-r--r--   0        0        0     4311 2023-04-10 08:43:27.218544 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Link_white.svg
+-rw-r--r--   0        0        0     1078 2023-04-10 08:43:27.218544 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Mail_black.svg
+-rw-r--r--   0        0        0     1078 2023-04-10 08:43:27.219572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Mail_white.svg
+-rw-r--r--   0        0        0     2947 2023-04-10 08:43:27.219572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Media_black.svg
+-rw-r--r--   0        0        0     2947 2023-04-10 08:43:27.219572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Media_white.svg
+-rw-r--r--   0        0        0     2518 2023-04-10 08:43:27.219572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Menu_black copy.svg
+-rw-r--r--   0        0        0     1228 2023-04-10 08:43:27.220573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Menu_black.svg
+-rw-r--r--   0        0        0     2518 2023-04-10 08:43:27.220573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Menu_white copy.svg
+-rw-r--r--   0        0        0     1228 2023-04-10 08:43:27.220573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Menu_white.svg
+-rw-r--r--   0        0        0     1863 2023-04-10 08:43:27.221552 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Message_black.svg
+-rw-r--r--   0        0        0     1863 2023-04-10 08:43:27.221552 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Message_white.svg
+-rw-r--r--   0        0        0     1529 2023-04-10 08:43:27.222575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Microphone_black.svg
+-rw-r--r--   0        0        0     1529 2023-04-10 08:43:27.222575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Microphone_white.svg
+-rw-r--r--   0        0        0     4953 2023-04-10 08:43:27.222575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Minimize_black.svg
+-rw-r--r--   0        0        0     4953 2023-04-10 08:43:27.223573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Minimize_white.svg
+-rw-r--r--   0        0        0     1594 2023-04-10 08:43:27.223573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/More_black.svg
+-rw-r--r--   0        0        0     1594 2023-04-10 08:43:27.223573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/More_white.svg
+-rw-r--r--   0        0        0     3871 2023-04-10 08:43:27.223573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Movie_black.svg
+-rw-r--r--   0        0        0     3871 2023-04-10 08:43:27.224573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Movie_white.svg
+-rw-r--r--   0        0        0     4478 2023-04-10 08:43:27.224573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Music_black.svg
+-rw-r--r--   0        0        0     4478 2023-04-10 08:43:27.225581 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Music_white.svg
+-rw-r--r--   0        0        0     4087 2023-04-10 08:43:27.224573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/MusicFolder_black.svg
+-rw-r--r--   0        0        0     4087 2023-04-10 08:43:27.224573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/MusicFolder_white.svg
+-rw-r--r--   0        0        0     8283 2023-04-10 08:43:27.225581 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Palette_black.svg
+-rw-r--r--   0        0        0     8283 2023-04-10 08:43:27.225581 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Palette_white.svg
+-rw-r--r--   0        0        0     2365 2023-04-10 08:43:27.226573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Paste_black.svg
+-rw-r--r--   0        0        0     2365 2023-04-10 08:43:27.226573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Paste_white.svg
+-rw-r--r--   0        0        0     5500 2023-04-10 08:43:27.226573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/PencilInk_black.svg
+-rw-r--r--   0        0        0     5500 2023-04-10 08:43:27.227580 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/PencilInk_white.svg
+-rw-r--r--   0        0        0     1948 2023-04-10 08:43:27.227580 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Phone_black.svg
+-rw-r--r--   0        0        0     1948 2023-04-10 08:43:27.227580 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Phone_white.svg
+-rw-r--r--   0        0        0     2023 2023-04-10 08:43:27.227580 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Photo_black.svg
+-rw-r--r--   0        0        0     2023 2023-04-10 08:43:27.228572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Photo_white.svg
+-rw-r--r--   0        0        0     1261 2023-04-10 08:43:27.228572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Pin_black.svg
+-rw-r--r--   0        0        0     1261 2023-04-10 08:43:27.228572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Pin_white.svg
+-rw-r--r--   0        0        0     1626 2023-04-10 08:43:27.228572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Print_black.svg
+-rw-r--r--   0        0        0     1626 2023-04-10 08:43:27.229573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Print_white.svg
+-rw-r--r--   0        0        0     3631 2023-04-10 08:43:27.229573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Question_black.svg
+-rw-r--r--   0        0        0     3631 2023-04-10 08:43:27.229573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Question_white.svg
+-rw-r--r--   0        0        0      638 2023-04-10 08:43:27.229573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Return_black.svg
+-rw-r--r--   0        0        0      638 2023-04-10 08:43:27.230573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Return_white.svg
+-rw-r--r--   0        0        0     2230 2023-04-10 08:43:27.230573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Ringer_black.svg
+-rw-r--r--   0        0        0     2230 2023-04-10 08:43:27.230573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Ringer_white.svg
+-rw-r--r--   0        0        0     1897 2023-04-10 08:43:27.231577 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Save_black.svg
+-rw-r--r--   0        0        0     1897 2023-04-10 08:43:27.232572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Save_white.svg
+-rw-r--r--   0        0        0     2498 2023-04-10 08:43:27.230573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/SaveAs_black.svg
+-rw-r--r--   0        0        0     2498 2023-04-10 08:43:27.231577 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/SaveAs_white.svg
+-rw-r--r--   0        0        0      933 2023-04-10 08:43:27.232572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Scroll_black.svg
+-rw-r--r--   0        0        0      933 2023-04-10 08:43:27.232572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Scroll_white.svg
+-rw-r--r--   0        0        0     3967 2023-04-10 08:43:27.233573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Search_black.svg
+-rw-r--r--   0        0        0     3967 2023-04-10 08:43:27.233573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Search_white.svg
+-rw-r--r--   0        0        0      683 2023-04-10 08:43:27.234573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Send_black.svg
+-rw-r--r--   0        0        0      683 2023-04-10 08:43:27.234573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Send_white.svg
+-rw-r--r--   0        0        0      701 2023-04-10 08:43:27.233573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/SendFill_black.svg
+-rw-r--r--   0        0        0      701 2023-04-10 08:43:27.233573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/SendFill_white.svg
+-rw-r--r--   0        0        0    10042 2023-04-10 08:43:27.234573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Setting_black.svg
+-rw-r--r--   0        0        0    10042 2023-04-10 08:43:27.235544 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Setting_white.svg
+-rw-r--r--   0        0        0     2237 2023-04-10 08:43:27.235544 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Share_black.svg
+-rw-r--r--   0        0        0     2237 2023-04-10 08:43:27.235544 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Share_white.svg
+-rw-r--r--   0        0        0     3508 2023-04-10 08:43:27.235544 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Sync_black.svg
+-rw-r--r--   0        0        0     3510 2023-04-10 08:43:27.236574 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Sync_white.svg
+-rw-r--r--   0        0        0     1579 2023-04-10 08:43:27.236574 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Tag_black.svg
+-rw-r--r--   0        0        0     1579 2023-04-10 08:43:27.236574 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Tag_white.svg
+-rw-r--r--   0        0        0     8499 2023-04-10 08:43:27.237573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Transparent_black.svg
+-rw-r--r--   0        0        0     8499 2023-04-10 08:43:27.237573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Transparent_white.svg
+-rw-r--r--   0        0        0     1388 2023-04-10 08:43:27.237573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Unpin_black.svg
+-rw-r--r--   0        0        0     1388 2023-04-10 08:43:27.237573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Unpin_white.svg
+-rw-r--r--   0        0        0     8989 2023-04-10 08:43:27.238572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Update_black.svg
+-rw-r--r--   0        0        0     8989 2023-04-10 08:43:27.238572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Update_white.svg
+-rw-r--r--   0        0        0     6996 2023-04-10 08:43:27.239573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Video_black.svg
+-rw-r--r--   0        0        0     6996 2023-04-10 08:43:27.239573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Video_white.svg
+-rw-r--r--   0        0        0     2312 2023-04-10 08:43:27.240573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/View_black.svg
+-rw-r--r--   0        0        0     2312 2023-04-10 08:43:27.240573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/View_white.svg
+-rw-r--r--   0        0        0     2120 2023-04-10 08:43:27.240573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/ZipFolder_black.svg
+-rw-r--r--   0        0        0     2120 2023-04-10 08:43:27.240573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/ZipFolder_white.svg
+-rw-r--r--   0        0        0     5993 2023-04-10 08:43:27.242543 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Zoom_black.svg
+-rw-r--r--   0        0        0     5993 2023-04-10 08:43:27.242543 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Zoom_white.svg
+-rw-r--r--   0        0        0     1911 2023-04-10 08:43:27.241572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/ZoomIn_black.svg
+-rw-r--r--   0        0        0     1911 2023-04-10 08:43:27.241572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/ZoomIn_white.svg
+-rw-r--r--   0        0        0     1721 2023-04-10 08:43:27.242543 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/ZoomOut_black.svg
+-rw-r--r--   0        0        0     1721 2023-04-10 08:43:27.242543 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/ZoomOut_white.svg
+-rw-r--r--   0        0        0     1585 2023-04-10 08:43:27.243573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/info_bar/Error_dark.svg
+-rw-r--r--   0        0        0     1588 2023-04-10 08:43:27.243573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/info_bar/Error_light.svg
+-rw-r--r--   0        0        0     1393 2023-04-10 08:43:27.243573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/info_bar/Info_dark.svg
+-rw-r--r--   0        0        0     1396 2023-04-10 08:43:27.243573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/info_bar/Info_light.svg
+-rw-r--r--   0        0        0     1351 2023-04-10 08:43:27.244573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/info_bar/Success_dark.svg
+-rw-r--r--   0        0        0     1356 2023-04-10 08:43:27.244573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/info_bar/Success_light.svg
+-rw-r--r--   0        0        0     1397 2023-04-10 08:43:27.244573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/info_bar/Warning_dark.svg
+-rw-r--r--   0        0        0     1400 2023-04-10 08:43:27.244573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/info_bar/Warning_light.svg
+-rw-r--r--   0        0        0      583 2023-04-10 08:43:27.245581 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/spin_box/Down_black.svg
+-rw-r--r--   0        0        0      669 2023-04-10 08:43:27.245581 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/spin_box/Down_white.svg
+-rw-r--r--   0        0        0      579 2023-04-10 08:43:27.245581 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/spin_box/Up_black.svg
+-rw-r--r--   0        0        0      665 2023-04-10 08:43:27.246543 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/spin_box/Up_white.svg
+-rw-r--r--   0        0        0      646 2023-04-10 11:42:11.353289 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/tree_view/TreeViewClose_black.svg
+-rw-r--r--   0        0        0      646 2023-04-10 11:42:11.353289 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/tree_view/TreeViewClose_white.svg
+-rw-r--r--   0        0        0      763 2023-04-10 11:42:11.353289 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/tree_view/TreeViewOpen_black.svg
+-rw-r--r--   0        0        0      763 2023-04-10 11:42:11.353289 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/tree_view/TreeViewOpen_white.svg
+-rw-r--r--   0        0        0     3937 2023-04-10 08:43:27.246543 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/button.qss
+-rw-r--r--   0        0        0     1623 2023-04-10 08:43:27.246543 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/check_box.qss
+-rw-r--r--   0        0        0     3016 2023-04-10 08:43:27.247576 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/color_dialog.qss
+-rw-r--r--   0        0        0     1481 2023-04-10 08:43:27.247576 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/combo_box.qss
+-rw-r--r--   0        0        0     1504 2023-04-10 08:43:27.247576 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/dialog.qss
+-rw-r--r--   0        0        0     2162 2023-04-10 08:43:27.248572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/expand_setting_card.qss
+-rw-r--r--   0        0        0     1569 2023-04-10 08:43:27.248572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/folder_list_dialog.qss
+-rw-r--r--   0        0        0      848 2023-04-10 08:43:27.248572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/info_bar.qss
+-rw-r--r--   0        0        0     2184 2023-04-10 08:43:27.249575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/line_edit.qss
+-rw-r--r--   0        0        0     1605 2023-04-10 08:43:27.249575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/menu.qss
+-rw-r--r--   0        0        0      813 2023-04-10 08:43:27.249575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/message_dialog.qss
+-rw-r--r--   0        0        0      524 2023-04-10 08:43:27.249575 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/navigation_interface.qss
+-rw-r--r--   0        0        0     1670 2023-04-10 09:33:25.271948 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/setting_card.qss
+-rw-r--r--   0        0        0      212 2023-04-10 08:43:27.251573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/setting_card_group.qss
+-rw-r--r--   0        0        0     2543 2023-04-10 08:43:27.251573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/slider.qss
+-rw-r--r--   0        0        0     1420 2023-04-10 08:43:27.251573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/spin_box.qss
+-rw-r--r--   0        0        0      355 2023-04-10 08:43:27.251573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/state_tool_tip.qss
+-rw-r--r--   0        0        0     1403 2023-04-10 08:43:27.252573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/switch_button.qss
+-rw-r--r--   0        0        0      309 2023-04-10 08:43:27.252573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/tool_tip.qss
+-rw-r--r--   0        0        0     2761 2023-04-10 11:42:11.354289 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/tree_view.qss
+-rw-r--r--   0        0        0     3985 2023-04-10 08:43:27.252573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/button.qss
+-rw-r--r--   0        0        0     1634 2023-04-10 08:43:27.253572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/check_box.qss
+-rw-r--r--   0        0        0     3027 2023-04-10 08:43:27.253572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/color_dialog.qss
+-rw-r--r--   0        0        0     1423 2023-04-10 08:43:27.253572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/combo_box.qss
+-rw-r--r--   0        0        0     1518 2023-04-10 08:43:27.253572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/dialog.qss
+-rw-r--r--   0        0        0     2167 2023-04-10 08:43:27.253572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/expand_setting_card.qss
+-rw-r--r--   0        0        0     1435 2023-04-10 08:43:27.254573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/folder_list_dialog.qss
+-rw-r--r--   0        0        0      854 2023-04-10 08:43:27.254573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/info_bar.qss
+-rw-r--r--   0        0        0     2196 2023-04-10 08:43:27.254573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/line_edit.qss
+-rw-r--r--   0        0        0     1521 2023-04-10 08:43:27.255573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/menu.qss
+-rw-r--r--   0        0        0      802 2023-04-10 08:43:27.255573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/message_dialog.qss
+-rw-r--r--   0        0        0      532 2023-04-10 08:43:27.255573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/navigation_interface.qss
+-rw-r--r--   0        0        0     1658 2023-04-10 08:43:27.255573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/setting_card.qss
+-rw-r--r--   0        0        0      210 2023-04-10 08:43:27.255573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/setting_card_group.qss
+-rw-r--r--   0        0        0     2931 2023-04-10 08:43:27.256574 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/slider.qss
+-rw-r--r--   0        0        0     1416 2023-04-10 08:43:27.256574 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/spin_box.qss
+-rw-r--r--   0        0        0      354 2023-04-10 08:43:27.256574 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/state_tool_tip.qss
+-rw-r--r--   0        0        0     1414 2023-04-10 08:43:27.256574 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/switch_button.qss
+-rw-r--r--   0        0        0      318 2023-04-10 08:43:27.257581 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/tool_tip.qss
+-rw-r--r--   0        0        0     2772 2023-04-10 11:42:11.354289 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/tree_view.qss
+-rw-r--r--   0        0        0  1637136 2023-04-12 06:51:06.630968 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/resource.py
+-rw-r--r--   0        0        0    11723 2023-04-10 11:42:11.398294 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/resource.qrc
+-rw-r--r--   0        0        0  1637139 2023-04-12 14:57:04.333322 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/resource_rc.py
+-rw-r--r--   0        0        0      390 2023-04-10 08:43:27.273573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/common/__init__.py
+-rw-r--r--   0        0        0     3193 2023-04-10 08:43:27.273573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/common/auto_wrap.py
+-rw-r--r--   0        0        0    10560 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/common/config.py
+-rw-r--r--   0        0        0      675 2023-04-10 08:43:27.274572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/common/exception_handler.py
+-rw-r--r--   0        0        0     7211 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/common/icon.py
+-rw-r--r--   0        0        0     4782 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/common/image_utils.py
+-rw-r--r--   0        0        0     4796 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/common/smooth_scroll.py
+-rw-r--r--   0        0        0     6990 2023-04-10 11:44:26.750465 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/common/style_sheet.py
+-rw-r--r--   0        0        0      124 2023-04-10 11:41:52.425867 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/__init__.py
+-rw-r--r--   0        0        0      170 2023-04-10 08:43:27.276573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/dialog_box/__init__.py
+-rw-r--r--   0        0        0    11987 2023-04-10 10:39:04.022260 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/dialog_box/color_dialog.py
+-rw-r--r--   0        0        0     5250 2023-04-10 11:09:38.442297 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/dialog_box/dialog.py
+-rw-r--r--   0        0        0    11235 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/dialog_box/folder_list_dialog.py
+-rw-r--r--   0        0        0     3196 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/dialog_box/mask_dialog_base.py
+-rw-r--r--   0        0        0     2486 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/dialog_box/message_dialog.py
+-rw-r--r--   0        0        0      114 2023-04-10 08:43:27.278573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/layout/__init__.py
+-rw-r--r--   0        0        0     2649 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/layout/expand_layout.py
+-rw-r--r--   0        0        0     5431 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/layout/flow_layout.py
+-rw-r--r--   0        0        0     1299 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/layout/v_box_layout.py
+-rw-r--r--   0        0        0      260 2023-04-10 08:43:27.280572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/navigation/__init__.py
+-rw-r--r--   0        0        0     4245 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/navigation/navigation_interface.py
+-rw-r--r--   0        0        0    14424 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/navigation/navigation_panel.py
+-rw-r--r--   0        0        0     4864 2023-04-10 10:35:11.987021 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/navigation/navigation_widget.py
+-rw-r--r--   0        0        0      550 2023-04-10 08:43:27.281572 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/settings/__init__.py
+-rw-r--r--   0        0        0     5186 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/settings/custom_color_setting_card.py
+-rw-r--r--   0        0        0     8017 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/settings/expand_setting_card.py
+-rw-r--r--   0        0        0     6019 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/settings/folder_list_setting_card.py
+-rw-r--r--   0        0        0     2829 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/settings/options_setting_card.py
+-rw-r--r--   0        0        0    12810 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/settings/setting_card.py
+-rw-r--r--   0        0        0     1510 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/settings/setting_card_group.py
+-rw-r--r--   0        0        0      915 2023-04-10 11:42:22.643239 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/__init__.py
+-rw-r--r--   0        0        0     4587 2023-04-12 15:20:30.138105 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/acrylic_label.py
+-rw-r--r--   0        0        0     4641 2023-04-10 10:35:11.922022 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/button.py
+-rw-r--r--   0        0        0      303 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/check_box.py
+-rw-r--r--   0        0        0    13473 2023-04-10 10:35:11.922022 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/combo_box.py
+-rw-r--r--   0        0        0      701 2023-04-10 12:02:57.033746 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/icon_widget.py
+-rw-r--r--   0        0        0    18826 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/info_bar.py
+-rw-r--r--   0        0        0      855 2023-04-10 10:35:11.964022 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/label.py
+-rw-r--r--   0        0        0     5747 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/line_edit.py
+-rw-r--r--   0        0        0    23261 2023-04-10 10:47:10.716030 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/menu.py
+-rw-r--r--   0        0        0     4505 2023-04-10 10:35:11.967022 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/scroll_area.py
+-rw-r--r--   0        0        0     5047 2023-04-10 11:33:41.269573 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/slider.py
+-rw-r--r--   0        0        0     4389 2023-04-10 10:35:11.985023 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/spin_box.py
+-rw-r--r--   0        0        0     6308 2023-04-10 10:35:11.986024 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/stacked_widget.py
+-rw-r--r--   0        0        0     5786 2023-04-10 10:35:11.985023 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/state_tool_tip.py
+-rw-r--r--   0        0        0     6568 2023-04-10 10:35:11.985023 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/switch_button.py
+-rw-r--r--   0        0        0     1651 2023-04-10 10:35:11.985023 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/three_state_button.py
+-rw-r--r--   0        0        0     5166 2023-04-10 10:35:11.985023 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/tool_tip.py
+-rw-r--r--   0        0        0     2826 2023-04-10 08:41:41.422117 QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/tree_view.py
+-rw-r--r--   0        0        0     1551 2023-04-12 06:41:26.816247 QtPy-Fluent-Widgets-0.0.3/README.md
+-rw-r--r--   0        0        0     2175 1970-01-01 00:00:00.000000 QtPy-Fluent-Widgets-0.0.3/PKG-INFO
```

### Comparing `QtPy-Fluent-Widgets-0.0.2/LICENSE` & `QtPy-Fluent-Widgets-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/pyproject.toml` & `QtPy-Fluent-Widgets-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -18,24 +18,22 @@
 description = "A fluent design widgets library based on QtPy"
 keywords = [
     "qtpy fluent widgets",
 ]
 name = "QtPy-Fluent-Widgets"
 readme = "README.md"
 requires-python = ">=3.7,<3.10"
-version = "0.0.2"
+version = "0.0.3"
 
 [project.license]
 text = "GPLv3"
 
 [project.urls]
-"Bug Tracker" = "https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues"
 Documentation = "https://pyqt-fluent-widgets.readthedocs.io/"
-Homepage = "https://github.com/zhiyiYo/PyQt-Fluent-Widgets"
-"Source Code" = "https://github.com/zhiyiYo/PyQt-Fluent-Widgets"
+Homepage = "https://github.com/TaoChenyue/QtPy-Fluent-Widgets"
 
 [project.optional-dependencies]
 full = [
     "colorthief",
     "pillow",
     "scipy",
 ]
```

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/acrylic/noise.png` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/acrylic/noise.png`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/check_box/Accept_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/check_box/Accept_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/check_box/Accept_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/check_box/Accept_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/check_box/PartialAccept_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/check_box/PartialAccept_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/check_box/PartialAccept_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/check_box/PartialAccept_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/color_dialog/Clear_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/color_dialog/Clear_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/color_dialog/Clear_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/color_dialog/Clear_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/color_dialog/HuePanel.png` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/color_dialog/HuePanel.png`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Add_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Add_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Add_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Add_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Album_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Album_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Album_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Album_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Alignment_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Alignment_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Alignment_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Alignment_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/BackgroundColor_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/BackgroundColor_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/BackgroundColor_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/BackgroundColor_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/BookShelf_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/BookShelf_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/BookShelf_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/BookShelf_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Brush_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Brush_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Brush_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Brush_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Camera_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Camera_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Camera_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Camera_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Cancel_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Cancel_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Cancel_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Cancel_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Chat_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Chat_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Chat_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Chat_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/CheckBox_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/CheckBox_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/CheckBox_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/CheckBox_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/ChevronDown_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/ChevronDown_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/ChevronDown_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/ChevronDown_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/ChevronRight_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/ChevronRight_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/ChevronRight_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/ChevronRight_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Close_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Close_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Close_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Close_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Code_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Code_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Code_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Code_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Completed_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Completed_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Completed_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Completed_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Constract_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Constract_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Constract_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Constract_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Copy_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Copy_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Copy_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Copy_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Cut_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Cut_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Cut_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Cut_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Delete_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Delete_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Delete_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Delete_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Document_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Document_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Document_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Document_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Download_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Download_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Download_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Download_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Edit_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Edit_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Edit_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Edit_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Embed_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Embed_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Embed_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Embed_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Feedback_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Feedback_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Feedback_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Feedback_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Folder_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Folder_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Folder_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Folder_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/FolderAdd_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/FolderAdd_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/FolderAdd_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/FolderAdd_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Font_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Font_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Font_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Font_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/GitHub_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/GitHub_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/GitHub_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/GitHub_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Globe_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Globe_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Globe_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Globe_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Heart_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Heart_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Heart_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Heart_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Help_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Help_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Help_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Help_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Hide_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Hide_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Hide_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Hide_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Highlight_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Highlight_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Highlight_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Highlight_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/History_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/History_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/History_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/History_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Home_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Home_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Home_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Home_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Info_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Info_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Info_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Info_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Language_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Language_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Language_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Language_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Layout_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Layout_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Layout_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Layout_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Link_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Link_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Link_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Link_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Mail_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Mail_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Mail_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Mail_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Media_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Media_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Media_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Media_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Menu_black copy.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Menu_black copy.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Menu_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Menu_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Menu_white copy.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Menu_white copy.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Menu_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Menu_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Message_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Message_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Message_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Message_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Microphone_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Microphone_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Microphone_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Microphone_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Minimize_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Minimize_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Minimize_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Minimize_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/More_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/More_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/More_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/More_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Movie_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Movie_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Movie_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Movie_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Music_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Music_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Music_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Music_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/MusicFolder_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/MusicFolder_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/MusicFolder_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/MusicFolder_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Palette_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Palette_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Palette_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Palette_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Paste_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Paste_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Paste_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Paste_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/PencilInk_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/PencilInk_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/PencilInk_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/PencilInk_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Phone_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Phone_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Phone_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Phone_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Photo_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Photo_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Photo_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Photo_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Pin_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Pin_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Pin_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Pin_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Print_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Print_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Print_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Print_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Question_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Question_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Question_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Question_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Return_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Return_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Return_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Return_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Ringer_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Ringer_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Ringer_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Ringer_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Save_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Save_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Save_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Save_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/SaveAs_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/SaveAs_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/SaveAs_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/SaveAs_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Scroll_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Scroll_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Scroll_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Scroll_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Search_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Search_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Search_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Search_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Send_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Send_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Send_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Send_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/SendFill_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/SendFill_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/SendFill_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/SendFill_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Setting_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Setting_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Setting_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Setting_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Share_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Share_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Share_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Share_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Sync_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Sync_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Sync_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Sync_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Tag_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Tag_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Tag_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Tag_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Transparent_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Transparent_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Transparent_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Transparent_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Unpin_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Unpin_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Unpin_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Unpin_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Update_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Update_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Update_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Update_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Video_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Video_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Video_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Video_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/View_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/View_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/View_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/View_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/ZipFolder_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/ZipFolder_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/ZipFolder_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/ZipFolder_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Zoom_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Zoom_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/Zoom_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/Zoom_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/ZoomIn_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/ZoomIn_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/ZoomIn_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/ZoomIn_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/ZoomOut_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/ZoomOut_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/icons/ZoomOut_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/icons/ZoomOut_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/info_bar/Error_dark.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/info_bar/Error_dark.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/info_bar/Error_light.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/info_bar/Error_light.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/info_bar/Info_dark.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/info_bar/Info_dark.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/info_bar/Info_light.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/info_bar/Info_light.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/info_bar/Success_dark.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/info_bar/Success_dark.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/info_bar/Success_light.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/info_bar/Success_light.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/info_bar/Warning_dark.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/info_bar/Warning_dark.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/info_bar/Warning_light.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/info_bar/Warning_light.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/spin_box/Down_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/spin_box/Down_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/spin_box/Down_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/spin_box/Down_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/spin_box/Up_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/spin_box/Up_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/spin_box/Up_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/spin_box/Up_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/tree_view/TreeViewClose_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/tree_view/TreeViewClose_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/tree_view/TreeViewClose_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/tree_view/TreeViewClose_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/tree_view/TreeViewOpen_black.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/tree_view/TreeViewOpen_black.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/images/tree_view/TreeViewOpen_white.svg` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/images/tree_view/TreeViewOpen_white.svg`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/button.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/button.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/check_box.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/check_box.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/color_dialog.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/color_dialog.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/combo_box.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/combo_box.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/dialog.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/dialog.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/expand_setting_card.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/expand_setting_card.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/folder_list_dialog.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/folder_list_dialog.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/info_bar.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/info_bar.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/line_edit.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/line_edit.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/menu.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/menu.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/message_dialog.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/message_dialog.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/navigation_interface.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/navigation_interface.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/setting_card.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/setting_card.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/slider.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/slider.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/spin_box.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/spin_box.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/switch_button.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/switch_button.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/dark/tree_view.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/dark/tree_view.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/button.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/button.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/check_box.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/check_box.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/color_dialog.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/color_dialog.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/combo_box.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/combo_box.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/dialog.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/dialog.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/expand_setting_card.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/expand_setting_card.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/folder_list_dialog.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/folder_list_dialog.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/info_bar.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/info_bar.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/line_edit.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/line_edit.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/menu.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/menu.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/message_dialog.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/message_dialog.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/navigation_interface.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/navigation_interface.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/setting_card.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/setting_card.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/slider.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/slider.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/spin_box.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/spin_box.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/switch_button.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/switch_button.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/qss/light/tree_view.qss` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/qss/light/tree_view.qss`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/resource.qrc` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/resource.qrc`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/_rc/resource_rc.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/_rc/resource_rc.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/common/auto_wrap.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/common/auto_wrap.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/common/config.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/common/config.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/common/exception_handler.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/common/icon.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/common/image_utils.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/common/smooth_scroll.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/common/style_sheet.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/common/style_sheet.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/dialog_box/color_dialog.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/dialog_box/color_dialog.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/dialog_box/dialog.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/dialog_box/dialog.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/dialog_box/folder_list_dialog.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/dialog_box/folder_list_dialog.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/dialog_box/mask_dialog_base.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/dialog_box/message_dialog.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/dialog_box/message_dialog.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/layout/expand_layout.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/layout/flow_layout.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/layout/flow_layout.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/layout/v_box_layout.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/layout/v_box_layout.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/navigation/navigation_interface.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/navigation/navigation_interface.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/navigation/navigation_panel.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/navigation/navigation_panel.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/navigation/navigation_widget.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/navigation/navigation_widget.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/settings/__init__.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/settings/custom_color_setting_card.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/settings/custom_color_setting_card.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/settings/expand_setting_card.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/settings/expand_setting_card.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/settings/folder_list_setting_card.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/settings/folder_list_setting_card.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/settings/options_setting_card.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/settings/options_setting_card.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/settings/setting_card.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/settings/setting_card.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/settings/setting_card_group.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/settings/setting_card_group.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/__init__.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/acrylic_label.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/acrylic_label.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from qtpy.QtGui import QBrush, QColor, QImage, QPainter, QPixmap
 from qtpy.QtWidgets import QLabel
 
 try:
     from ...common.image_utils import gaussianBlur
 except ImportError as e:
     warnings.warn(
-        '`AcrylicLabel` is not supported in current qfluentwidgets, use `pip install PyQt-Fluent-Widgets[full]` to enable it.')
+        '`AcrylicLabel` is not supported in current qfluentwidgets, use `pip install QtPy-Fluent-Widgets[full]` to enable it.')
 
     def gaussianBlur(imagePath, blurRadius=18, brightFactor=1, blurPicSize=None):
         return QPixmap(imagePath)
 
 
 class BlurCoverThread(QThread):
     """ Blur album cover thread """
```

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/button.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/button.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/combo_box.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/icon_widget.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/info_bar.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/info_bar.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/label.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/line_edit.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/menu.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/scroll_area.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/slider.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/spin_box.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/stacked_widget.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/state_tool_tip.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/state_tool_tip.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/switch_button.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/three_state_button.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/three_state_button.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/tool_tip.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `QtPy-Fluent-Widgets-0.0.2/qtfluentwidgets/components/widgets/tree_view.py` & `QtPy-Fluent-Widgets-0.0.3/qtfluentwidgets/components/widgets/tree_view.py`

 * *Files identical despite different names*

