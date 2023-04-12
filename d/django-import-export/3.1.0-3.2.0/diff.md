# Comparing `tmp/django-import-export-3.1.0.tar.gz` & `tmp/django-import-export-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-import-export-3.1.0.tar", last modified: Tue Feb 21 18:59:34 2023, max compression
+gzip compressed data, was "django-import-export-3.2.0.tar", last modified: Wed Apr 12 18:04:31 2023, max compression
```

## Comparing `django-import-export-3.1.0.tar` & `django-import-export-3.2.0.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.902292 django-import-export-3.1.0/
--rw-r--r--   0 matthew    (501) staff       (20)     3418 2023-02-21 18:59:34.000000 django-import-export-3.1.0/AUTHORS
--rw-r--r--   0 matthew    (501) staff       (20)     1343 2023-02-21 18:59:34.000000 django-import-export-3.1.0/LICENSE
--rw-r--r--   0 matthew    (501) staff       (20)      177 2023-02-21 18:59:34.000000 django-import-export-3.1.0/MANIFEST.in
--rw-r--r--   0 matthew    (501) staff       (20)     3021 2023-02-21 18:59:34.902357 django-import-export-3.1.0/PKG-INFO
--rw-r--r--   0 matthew    (501) staff       (20)     1716 2023-02-21 18:59:34.000000 django-import-export-3.1.0/README.rst
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.891726 django-import-export-3.1.0/django_import_export.egg-info/
--rw-r--r--   0 matthew    (501) staff       (20)     3021 2023-02-21 18:59:34.000000 django-import-export-3.1.0/django_import_export.egg-info/PKG-INFO
--rw-r--r--   0 matthew    (501) staff       (20)     3412 2023-02-21 18:59:34.000000 django-import-export-3.1.0/django_import_export.egg-info/SOURCES.txt
--rw-r--r--   0 matthew    (501) staff       (20)        1 2023-02-21 18:59:34.000000 django-import-export-3.1.0/django_import_export.egg-info/dependency_links.txt
--rw-r--r--   0 matthew    (501) staff       (20)        1 2023-02-21 18:59:34.000000 django-import-export-3.1.0/django_import_export.egg-info/not-zip-safe
--rw-r--r--   0 matthew    (501) staff       (20)       67 2023-02-21 18:59:34.000000 django-import-export-3.1.0/django_import_export.egg-info/requires.txt
--rw-r--r--   0 matthew    (501) staff       (20)       14 2023-02-21 18:59:34.000000 django-import-export-3.1.0/django_import_export.egg-info/top_level.txt
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.894050 django-import-export-3.1.0/import_export/
--rw-r--r--   0 matthew    (501) staff       (20)       22 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/__init__.py
--rw-r--r--   0 matthew    (501) staff       (20)    34829 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/admin.py
--rw-r--r--   0 matthew    (501) staff       (20)      200 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/exceptions.py
--rw-r--r--   0 matthew    (501) staff       (20)     5455 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/fields.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.894344 django-import-export-3.1.0/import_export/formats/
--rw-r--r--   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/formats/__init__.py
--rw-r--r--   0 matthew    (501) staff       (20)     5598 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/formats/base_formats.py
--rw-r--r--   0 matthew    (501) staff       (20)     3182 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/forms.py
--rw-r--r--   0 matthew    (501) staff       (20)     2139 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/instance_loaders.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.889508 django-import-export-3.1.0/import_export/locale/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.886876 django-import-export-3.1.0/import_export/locale/ar/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.894667 django-import-export-3.1.0/import_export/locale/ar/LC_MESSAGES/
--rw-r--r--   0 matthew    (501) staff       (20)     1750 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 matthew    (501) staff       (20)     3761 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.887018 django-import-export-3.1.0/import_export/locale/bg/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.894990 django-import-export-3.1.0/import_export/locale/bg/LC_MESSAGES/
--rw-r--r--   0 matthew    (501) staff       (20)     2070 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 matthew    (501) staff       (20)     3981 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.887156 django-import-export-3.1.0/import_export/locale/ca/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.895289 django-import-export-3.1.0/import_export/locale/ca/LC_MESSAGES/
--rw-r--r--   0 matthew    (501) staff       (20)     1548 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 matthew    (501) staff       (20)     3560 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.887301 django-import-export-3.1.0/import_export/locale/cs/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.895604 django-import-export-3.1.0/import_export/locale/cs/LC_MESSAGES/
--rw-r--r--   0 matthew    (501) staff       (20)     1663 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 matthew    (501) staff       (20)     3559 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.887436 django-import-export-3.1.0/import_export/locale/de/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.895927 django-import-export-3.1.0/import_export/locale/de/LC_MESSAGES/
--rw-r--r--   0 matthew    (501) staff       (20)     2507 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 matthew    (501) staff       (20)     4009 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.887570 django-import-export-3.1.0/import_export/locale/es/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.896251 django-import-export-3.1.0/import_export/locale/es/LC_MESSAGES/
--rw-r--r--   0 matthew    (501) staff       (20)     1559 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 matthew    (501) staff       (20)     3570 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.887724 django-import-export-3.1.0/import_export/locale/es_AR/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.896624 django-import-export-3.1.0/import_export/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 matthew    (501) staff       (20)     1563 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/es_AR/LC_MESSAGES/django.mo
--rw-r--r--   0 matthew    (501) staff       (20)     3552 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/es_AR/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.887857 django-import-export-3.1.0/import_export/locale/fa/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.896986 django-import-export-3.1.0/import_export/locale/fa/LC_MESSAGES/
--rw-r--r--   0 matthew    (501) staff       (20)     2450 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 matthew    (501) staff       (20)     4088 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.887994 django-import-export-3.1.0/import_export/locale/fr/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.897313 django-import-export-3.1.0/import_export/locale/fr/LC_MESSAGES/
--rw-r--r--   0 matthew    (501) staff       (20)     1544 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 matthew    (501) staff       (20)     3552 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.888134 django-import-export-3.1.0/import_export/locale/it/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.897619 django-import-export-3.1.0/import_export/locale/it/LC_MESSAGES/
--rw-r--r--   0 matthew    (501) staff       (20)     1537 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 matthew    (501) staff       (20)     3524 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.888269 django-import-export-3.1.0/import_export/locale/ja/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.897930 django-import-export-3.1.0/import_export/locale/ja/LC_MESSAGES/
--rw-r--r--   0 matthew    (501) staff       (20)     1650 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 matthew    (501) staff       (20)     3658 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.888404 django-import-export-3.1.0/import_export/locale/ko/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.898223 django-import-export-3.1.0/import_export/locale/ko/LC_MESSAGES/
--rw-r--r--   0 matthew    (501) staff       (20)     2046 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 matthew    (501) staff       (20)     3772 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.888547 django-import-export-3.1.0/import_export/locale/kz/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.898518 django-import-export-3.1.0/import_export/locale/kz/LC_MESSAGES/
--rw-r--r--   0 matthew    (501) staff       (20)     2597 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/kz/LC_MESSAGES/django.mo
--rw-r--r--   0 matthew    (501) staff       (20)     4252 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/kz/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.888691 django-import-export-3.1.0/import_export/locale/nl/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.898790 django-import-export-3.1.0/import_export/locale/nl/LC_MESSAGES/
--rw-r--r--   0 matthew    (501) staff       (20)     2167 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 matthew    (501) staff       (20)     3837 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.888838 django-import-export-3.1.0/import_export/locale/pl/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.899070 django-import-export-3.1.0/import_export/locale/pl/LC_MESSAGES/
--rw-r--r--   0 matthew    (501) staff       (20)     1740 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 matthew    (501) staff       (20)     3649 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.888982 django-import-export-3.1.0/import_export/locale/pt_BR/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.899321 django-import-export-3.1.0/import_export/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 matthew    (501) staff       (20)     2159 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 matthew    (501) staff       (20)     3781 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.889129 django-import-export-3.1.0/import_export/locale/ru/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.899570 django-import-export-3.1.0/import_export/locale/ru/LC_MESSAGES/
--rw-r--r--   0 matthew    (501) staff       (20)     2643 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 matthew    (501) staff       (20)     4305 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.889270 django-import-export-3.1.0/import_export/locale/sk/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.899820 django-import-export-3.1.0/import_export/locale/sk/LC_MESSAGES/
--rw-r--r--   0 matthew    (501) staff       (20)     1543 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 matthew    (501) staff       (20)     3554 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.889420 django-import-export-3.1.0/import_export/locale/tr/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.900078 django-import-export-3.1.0/import_export/locale/tr/LC_MESSAGES/
--rw-r--r--   0 matthew    (501) staff       (20)     2169 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 matthew    (501) staff       (20)     3828 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.889569 django-import-export-3.1.0/import_export/locale/zh_Hans/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.900342 django-import-export-3.1.0/import_export/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 matthew    (501) staff       (20)     1977 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 matthew    (501) staff       (20)     3646 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 matthew    (501) staff       (20)     6925 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/mixins.py
--rw-r--r--   0 matthew    (501) staff       (20)    46879 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/resources.py
--rw-r--r--   0 matthew    (501) staff       (20)     4952 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/results.py
--rw-r--r--   0 matthew    (501) staff       (20)      110 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/signals.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.889722 django-import-export-3.1.0/import_export/static/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.900814 django-import-export-3.1.0/import_export/static/import_export/
--rw-r--r--   0 matthew    (501) staff       (20)      765 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/static/import_export/action_formats.js
--rw-r--r--   0 matthew    (501) staff       (20)      711 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/static/import_export/guess_format.js
--rw-r--r--   0 matthew    (501) staff       (20)     2051 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/static/import_export/import.css
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.889880 django-import-export-3.1.0/import_export/templates/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.889940 django-import-export-3.1.0/import_export/templates/admin/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.901922 django-import-export-3.1.0/import_export/templates/admin/import_export/
--rw-r--r--   0 matthew    (501) staff       (20)      789 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/templates/admin/import_export/base.html
--rw-r--r--   0 matthew    (501) staff       (20)      392 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/templates/admin/import_export/change_list.html
--rw-r--r--   0 matthew    (501) staff       (20)      187 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/templates/admin/import_export/change_list_export.html
--rw-r--r--   0 matthew    (501) staff       (20)      207 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/templates/admin/import_export/change_list_export_item.html
--rw-r--r--   0 matthew    (501) staff       (20)      187 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/templates/admin/import_export/change_list_import.html
--rw-r--r--   0 matthew    (501) staff       (20)      254 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/templates/admin/import_export/change_list_import_export.html
--rw-r--r--   0 matthew    (501) staff       (20)      184 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/templates/admin/import_export/change_list_import_item.html
--rw-r--r--   0 matthew    (501) staff       (20)      894 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/templates/admin/import_export/export.html
--rw-r--r--   0 matthew    (501) staff       (20)     6086 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/templates/admin/import_export/import.html
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.902160 django-import-export-3.1.0/import_export/templatetags/
--rw-r--r--   0 matthew    (501) staff       (20)        0 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/templatetags/__init__.py
--rw-r--r--   0 matthew    (501) staff       (20)      322 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/templatetags/import_export_tags.py
--rw-r--r--   0 matthew    (501) staff       (20)     2453 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/tmp_storages.py
--rw-r--r--   0 matthew    (501) staff       (20)      997 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/utils.py
--rw-r--r--   0 matthew    (501) staff       (20)    15578 2023-02-21 18:59:34.000000 django-import-export-3.1.0/import_export/widgets.py
--rw-r--r--   0 matthew    (501) staff       (20)      242 2023-02-21 18:59:34.902602 django-import-export-3.1.0/setup.cfg
--rw-r--r--   0 matthew    (501) staff       (20)     1818 2023-02-21 18:59:34.000000 django-import-export-3.1.0/setup.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.820093 django-import-export-3.2.0/
+-rw-r--r--   0 matthew    (501) staff       (20)     3479 2023-04-12 18:04:31.000000 django-import-export-3.2.0/AUTHORS
+-rw-r--r--   0 matthew    (501) staff       (20)     1343 2023-04-12 18:04:31.000000 django-import-export-3.2.0/LICENSE
+-rw-r--r--   0 matthew    (501) staff       (20)      177 2023-04-12 18:04:31.000000 django-import-export-3.2.0/MANIFEST.in
+-rw-r--r--   0 matthew    (501) staff       (20)     3031 2023-04-12 18:04:31.820181 django-import-export-3.2.0/PKG-INFO
+-rw-r--r--   0 matthew    (501) staff       (20)     1723 2023-04-12 18:04:31.000000 django-import-export-3.2.0/README.rst
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.809862 django-import-export-3.2.0/django_import_export.egg-info/
+-rw-r--r--   0 matthew    (501) staff       (20)     3031 2023-04-12 18:04:31.000000 django-import-export-3.2.0/django_import_export.egg-info/PKG-INFO
+-rw-r--r--   0 matthew    (501) staff       (20)     3412 2023-04-12 18:04:31.000000 django-import-export-3.2.0/django_import_export.egg-info/SOURCES.txt
+-rw-r--r--   0 matthew    (501) staff       (20)        1 2023-04-12 18:04:31.000000 django-import-export-3.2.0/django_import_export.egg-info/dependency_links.txt
+-rw-r--r--   0 matthew    (501) staff       (20)        1 2023-04-12 18:04:31.000000 django-import-export-3.2.0/django_import_export.egg-info/not-zip-safe
+-rw-r--r--   0 matthew    (501) staff       (20)       67 2023-04-12 18:04:31.000000 django-import-export-3.2.0/django_import_export.egg-info/requires.txt
+-rw-r--r--   0 matthew    (501) staff       (20)       14 2023-04-12 18:04:31.000000 django-import-export-3.2.0/django_import_export.egg-info/top_level.txt
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.811748 django-import-export-3.2.0/import_export/
+-rw-r--r--   0 matthew    (501) staff       (20)       22 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/__init__.py
+-rw-r--r--   0 matthew    (501) staff       (20)    35080 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/admin.py
+-rw-r--r--   0 matthew    (501) staff       (20)      200 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/exceptions.py
+-rw-r--r--   0 matthew    (501) staff       (20)     5455 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/fields.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.812001 django-import-export-3.2.0/import_export/formats/
+-rw-r--r--   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/formats/__init__.py
+-rw-r--r--   0 matthew    (501) staff       (20)     6423 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/formats/base_formats.py
+-rw-r--r--   0 matthew    (501) staff       (20)     3837 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/forms.py
+-rw-r--r--   0 matthew    (501) staff       (20)     2139 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/instance_loaders.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.807616 django-import-export-3.2.0/import_export/locale/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.804851 django-import-export-3.2.0/import_export/locale/ar/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.812291 django-import-export-3.2.0/import_export/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 matthew    (501) staff       (20)     1750 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthew    (501) staff       (20)     3761 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.804991 django-import-export-3.2.0/import_export/locale/bg/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.812564 django-import-export-3.2.0/import_export/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 matthew    (501) staff       (20)     2070 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthew    (501) staff       (20)     3981 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.805129 django-import-export-3.2.0/import_export/locale/ca/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.812811 django-import-export-3.2.0/import_export/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 matthew    (501) staff       (20)     1548 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthew    (501) staff       (20)     3560 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.805269 django-import-export-3.2.0/import_export/locale/cs/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.813072 django-import-export-3.2.0/import_export/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 matthew    (501) staff       (20)     1663 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthew    (501) staff       (20)     3559 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.805405 django-import-export-3.2.0/import_export/locale/de/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.813341 django-import-export-3.2.0/import_export/locale/de/LC_MESSAGES/
+-rw-r--r--   0 matthew    (501) staff       (20)     2507 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthew    (501) staff       (20)     4009 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.805545 django-import-export-3.2.0/import_export/locale/es/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.813604 django-import-export-3.2.0/import_export/locale/es/LC_MESSAGES/
+-rw-r--r--   0 matthew    (501) staff       (20)     2481 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthew    (501) staff       (20)     4089 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.805694 django-import-export-3.2.0/import_export/locale/es_AR/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.813894 django-import-export-3.2.0/import_export/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 matthew    (501) staff       (20)     2507 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/es_AR/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthew    (501) staff       (20)     4093 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/es_AR/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.805836 django-import-export-3.2.0/import_export/locale/fa/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.814224 django-import-export-3.2.0/import_export/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 matthew    (501) staff       (20)     2450 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthew    (501) staff       (20)     4088 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.805975 django-import-export-3.2.0/import_export/locale/fr/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.814502 django-import-export-3.2.0/import_export/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 matthew    (501) staff       (20)     1544 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthew    (501) staff       (20)     3552 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.806123 django-import-export-3.2.0/import_export/locale/it/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.814813 django-import-export-3.2.0/import_export/locale/it/LC_MESSAGES/
+-rw-r--r--   0 matthew    (501) staff       (20)     1537 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthew    (501) staff       (20)     3524 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.806281 django-import-export-3.2.0/import_export/locale/ja/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.815102 django-import-export-3.2.0/import_export/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 matthew    (501) staff       (20)     1650 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthew    (501) staff       (20)     3658 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.806433 django-import-export-3.2.0/import_export/locale/ko/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.815419 django-import-export-3.2.0/import_export/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 matthew    (501) staff       (20)     2046 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthew    (501) staff       (20)     3772 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.806583 django-import-export-3.2.0/import_export/locale/kz/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.815703 django-import-export-3.2.0/import_export/locale/kz/LC_MESSAGES/
+-rw-r--r--   0 matthew    (501) staff       (20)     2597 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/kz/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthew    (501) staff       (20)     4252 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/kz/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.806743 django-import-export-3.2.0/import_export/locale/nl/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.816014 django-import-export-3.2.0/import_export/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 matthew    (501) staff       (20)     2167 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthew    (501) staff       (20)     3837 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.806897 django-import-export-3.2.0/import_export/locale/pl/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.816302 django-import-export-3.2.0/import_export/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 matthew    (501) staff       (20)     1740 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthew    (501) staff       (20)     3649 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.807047 django-import-export-3.2.0/import_export/locale/pt_BR/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.816605 django-import-export-3.2.0/import_export/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 matthew    (501) staff       (20)     2159 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthew    (501) staff       (20)     3781 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.807221 django-import-export-3.2.0/import_export/locale/ru/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.816891 django-import-export-3.2.0/import_export/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 matthew    (501) staff       (20)     2643 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthew    (501) staff       (20)     4305 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.807379 django-import-export-3.2.0/import_export/locale/sk/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.817211 django-import-export-3.2.0/import_export/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 matthew    (501) staff       (20)     1543 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthew    (501) staff       (20)     3554 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.807531 django-import-export-3.2.0/import_export/locale/tr/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.817502 django-import-export-3.2.0/import_export/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 matthew    (501) staff       (20)     2169 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthew    (501) staff       (20)     3828 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.807678 django-import-export-3.2.0/import_export/locale/zh_Hans/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.817810 django-import-export-3.2.0/import_export/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 matthew    (501) staff       (20)     1977 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthew    (501) staff       (20)     3646 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 matthew    (501) staff       (20)     7853 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/mixins.py
+-rw-r--r--   0 matthew    (501) staff       (20)    47591 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/resources.py
+-rw-r--r--   0 matthew    (501) staff       (20)     4952 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/results.py
+-rw-r--r--   0 matthew    (501) staff       (20)      110 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/signals.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.807836 django-import-export-3.2.0/import_export/static/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.818264 django-import-export-3.2.0/import_export/static/import_export/
+-rw-r--r--   0 matthew    (501) staff       (20)      765 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/static/import_export/action_formats.js
+-rw-r--r--   0 matthew    (501) staff       (20)      711 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/static/import_export/guess_format.js
+-rw-r--r--   0 matthew    (501) staff       (20)     2051 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/static/import_export/import.css
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.807985 django-import-export-3.2.0/import_export/templates/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.808046 django-import-export-3.2.0/import_export/templates/admin/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.819673 django-import-export-3.2.0/import_export/templates/admin/import_export/
+-rw-r--r--   0 matthew    (501) staff       (20)      789 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/templates/admin/import_export/base.html
+-rw-r--r--   0 matthew    (501) staff       (20)      392 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/templates/admin/import_export/change_list.html
+-rw-r--r--   0 matthew    (501) staff       (20)      187 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/templates/admin/import_export/change_list_export.html
+-rw-r--r--   0 matthew    (501) staff       (20)      207 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/templates/admin/import_export/change_list_export_item.html
+-rw-r--r--   0 matthew    (501) staff       (20)      187 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/templates/admin/import_export/change_list_import.html
+-rw-r--r--   0 matthew    (501) staff       (20)      254 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/templates/admin/import_export/change_list_import_export.html
+-rw-r--r--   0 matthew    (501) staff       (20)      184 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/templates/admin/import_export/change_list_import_item.html
+-rw-r--r--   0 matthew    (501) staff       (20)      894 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/templates/admin/import_export/export.html
+-rw-r--r--   0 matthew    (501) staff       (20)     6086 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/templates/admin/import_export/import.html
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.819956 django-import-export-3.2.0/import_export/templatetags/
+-rw-r--r--   0 matthew    (501) staff       (20)        0 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/templatetags/__init__.py
+-rw-r--r--   0 matthew    (501) staff       (20)      322 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/templatetags/import_export_tags.py
+-rw-r--r--   0 matthew    (501) staff       (20)     2453 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/tmp_storages.py
+-rw-r--r--   0 matthew    (501) staff       (20)      997 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/utils.py
+-rw-r--r--   0 matthew    (501) staff       (20)    15578 2023-04-12 18:04:31.000000 django-import-export-3.2.0/import_export/widgets.py
+-rw-r--r--   0 matthew    (501) staff       (20)      242 2023-04-12 18:04:31.820466 django-import-export-3.2.0/setup.cfg
+-rw-r--r--   0 matthew    (501) staff       (20)     1821 2023-04-12 18:04:31.000000 django-import-export-3.2.0/setup.py
```

### Comparing `django-import-export-3.1.0/AUTHORS` & `django-import-export-3.2.0/AUTHORS`

 * *Files 4% similar despite different names*

```diff
@@ -134,7 +134,9 @@
 * 1gni5 (Jules Ducange)
 * mpasternak (Michał Pasternak)
 * nikatlas (Nikos Atlas)
 * cocorocho (Erkan Çoban)
 * bdnettleton (Brian Nettleton)
 * Ptosiek (Antonin)
 * samupl (Jakub Szafrański)
+* smunoz-ml (Santiago Muñoz)
+* carlosal0ns0 (Carlos Alonso)
```

### Comparing `django-import-export-3.1.0/LICENSE` & `django-import-export-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/PKG-INFO` & `django-import-export-3.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: django-import-export
-Version: 3.1.0
+Version: 3.2.0
 Summary: Django application and library for importing and exporting data with included admin integration.
 Home-page: https://github.com/django-import-export/django-import-export
-Author: Informatika Mihelac
-Author-email: bmihelac@mihelac.org
+Author: Bojan Mihelač
+Author-email: djangoimportexport@gmail.com
 License: BSD License
 Project-URL: Documentation, https://django-import-export.readthedocs.io/en/stable/
 Project-URL: Changelog, https://django-import-export.readthedocs.io/en/stable/changelog.html
 Platform: OS Independent
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
@@ -49,15 +49,15 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/django-import-export
     :alt: PyPI - Python Version
 
 .. image:: https://img.shields.io/pypi/djversions/django-import-export
     :alt: PyPI - Django Version
 
-.. image:: https://static.pepy.tech/personalized-badge/django-import-export?period=week&units=international_system&left_color=black&right_color=blue&left_text=Downloads
+.. image:: https://static.pepy.tech/personalized-badge/django-import-export?period=month&units=international_system&left_color=black&right_color=blue&left_text=Downloads/month
     :target: https://pepy.tech/project/django-import-export
 
 django-import-export is a Django application and library for importing
 and exporting data from a variety of formats.  Includes Django Admin site integration.
 
 * Documentation: https://django-import-export.readthedocs.io/en/stable/
 * GitHub: https://github.com/django-import-export/django-import-export/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-import-export-3.1.0/README.rst` & `django-import-export-3.2.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/django-import-export
     :alt: PyPI - Python Version
 
 .. image:: https://img.shields.io/pypi/djversions/django-import-export
     :alt: PyPI - Django Version
 
-.. image:: https://static.pepy.tech/personalized-badge/django-import-export?period=week&units=international_system&left_color=black&right_color=blue&left_text=Downloads
+.. image:: https://static.pepy.tech/personalized-badge/django-import-export?period=month&units=international_system&left_color=black&right_color=blue&left_text=Downloads/month
     :target: https://pepy.tech/project/django-import-export
 
 django-import-export is a Django application and library for importing
 and exporting data from a variety of formats.  Includes Django Admin site integration.
 
 * Documentation: https://django-import-export.readthedocs.io/en/stable/
 * GitHub: https://github.com/django-import-export/django-import-export/
```

### Comparing `django-import-export-3.1.0/django_import_export.egg-info/PKG-INFO` & `django-import-export-3.2.0/django_import_export.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: django-import-export
-Version: 3.1.0
+Version: 3.2.0
 Summary: Django application and library for importing and exporting data with included admin integration.
 Home-page: https://github.com/django-import-export/django-import-export
-Author: Informatika Mihelac
-Author-email: bmihelac@mihelac.org
+Author: Bojan Mihelač
+Author-email: djangoimportexport@gmail.com
 License: BSD License
 Project-URL: Documentation, https://django-import-export.readthedocs.io/en/stable/
 Project-URL: Changelog, https://django-import-export.readthedocs.io/en/stable/changelog.html
 Platform: OS Independent
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
@@ -49,15 +49,15 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/django-import-export
     :alt: PyPI - Python Version
 
 .. image:: https://img.shields.io/pypi/djversions/django-import-export
     :alt: PyPI - Django Version
 
-.. image:: https://static.pepy.tech/personalized-badge/django-import-export?period=week&units=international_system&left_color=black&right_color=blue&left_text=Downloads
+.. image:: https://static.pepy.tech/personalized-badge/django-import-export?period=month&units=international_system&left_color=black&right_color=blue&left_text=Downloads/month
     :target: https://pepy.tech/project/django-import-export
 
 django-import-export is a Django application and library for importing
 and exporting data from a variety of formats.  Includes Django Admin site integration.
 
 * Documentation: https://django-import-export.readthedocs.io/en/stable/
 * GitHub: https://github.com/django-import-export/django-import-export/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-import-export-3.1.0/django_import_export.egg-info/SOURCES.txt` & `django-import-export-3.2.0/django_import_export.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/admin.py` & `django-import-export-3.2.0/import_export/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,17 +170,17 @@
 
             tmp_storage.remove()
 
             return self.process_result(result, request)
 
     def process_dataset(self, dataset, confirm_form, request, *args, rollback_on_validation_errors=False, **kwargs):
 
-        res_kwargs = self.get_import_resource_kwargs(request, form=confirm_form, *args, **kwargs)
+        res_kwargs = self.get_import_resource_kwargs(request, *args, form=confirm_form, **kwargs)
         resource = self.choose_import_resource_class(confirm_form)(**res_kwargs)
-        imp_kwargs = self.get_import_data_kwargs(request, form=confirm_form, *args, **kwargs)
+        imp_kwargs = self.get_import_data_kwargs(request, *args, form=confirm_form, **kwargs)
 
         return resource.import_data(dataset,
                                     dry_run=False,
                                     file_name=confirm_form.cleaned_data.get('original_file_name'),
                                     user=request.user,
                                     rollback_on_validation_errors=True,
                                     **imp_kwargs)
@@ -295,15 +295,15 @@
         if not issubclass(form_class, ImportExportFormBase):
             warnings.warn(
                 "The ImportForm class must inherit from ImportExportFormBase, "
                 "this is needed for multiple resource classes to work properly. ",
                 category=DeprecationWarning
             )
             return form_class(formats, **kwargs)
-        return form_class(formats, self.get_import_resource_classes(), **kwargs)
+        return form_class(formats, resources=self.get_import_resource_classes(), **kwargs)
 
     def get_import_form_class(self, request):
         """
         .. versionadded:: 3.0
 
         Return the form class to use for the 'import' step. If you only have
         a single custom form class, you can set the ``import_form_class``
@@ -476,17 +476,17 @@
         else:
             form_class = self.get_import_form_class(request)
             form_kwargs = self.get_form_kwargs(form_class, *args, **kwargs)
 
             if issubclass(form_class, ImportExportFormBase):
                 import_form = form_class(
                     import_formats,
-                    self.get_import_resource_classes(),
                     request.POST or None,
                     request.FILES or None,
+                    resources=self.get_import_resource_classes(),
                     **form_kwargs
                 )
             else:
                 warnings.warn(
                     "The ImportForm class must inherit from ImportExportFormBase, "
                     "this is needed for multiple resource classes to work properly. ",
                     category=DeprecationWarning
@@ -540,20 +540,20 @@
                     data = tmp_storage.read()
                     dataset = input_format.create_dataset(data)
                 except Exception as e:
                     self.add_data_read_fail_error_to_form(import_form, e)
 
                 if not import_form.errors:
                     # prepare kwargs for import data, if needed
-                    res_kwargs = self.get_import_resource_kwargs(request, form=import_form, *args, **kwargs)
+                    res_kwargs = self.get_import_resource_kwargs(request, *args, form=import_form, **kwargs)
                     resource = self.choose_import_resource_class(import_form)(**res_kwargs)
                     resources = [resource]
 
                     # prepare additional kwargs for import_data, if needed
-                    imp_kwargs = self.get_import_data_kwargs(request, form=import_form, *args, **kwargs)
+                    imp_kwargs = self.get_import_data_kwargs(request, *args, form=import_form, **kwargs)
                     result = resource.import_data(dataset, dry_run=True,
                                                   raise_errors=False,
                                                   file_name=import_file.name,
                                                   user=request.user,
                                                   **imp_kwargs)
 
                     context['result'] = result
@@ -567,15 +567,15 @@
                         else:
                             confirm_form_class = self.get_confirm_form_class(request)
                             initial = self.get_confirm_form_initial(request, import_form)
                             context["confirm_form"] = confirm_form_class(
                                 initial=self.get_form_kwargs(form=import_form, **initial)
                             )
         else:
-            res_kwargs = self.get_import_resource_kwargs(request, form=import_form, *args, **kwargs)
+            res_kwargs = self.get_import_resource_kwargs(request, *args, form=import_form, **kwargs)
             resource_classes = self.get_import_resource_classes()
             resources = [resource_class(**res_kwargs) for resource_class in resource_classes]
 
         context.update(self.admin_site.each_context(request))
 
         context['title'] = _("Import")
         context['form'] = import_form
@@ -675,15 +675,18 @@
         Returns file_format representation for given queryset.
         """
         request = kwargs.pop("request")
         if not self.has_export_permission(request):
             raise PermissionDenied
 
         data = self.get_data_for_export(request, queryset, *args, **kwargs)
-        export_data = file_format.export_data(data, escape_output=self.should_escape_output)
+        export_data = file_format.export_data(data,
+                                              escape_output=self.should_escape_output,
+                                              escape_html=self.should_escape_html,
+                                              escape_formulae=self.should_escape_formulae)
         encoding = kwargs.get("encoding")
         if not file_format.is_binary() and encoding:
             export_data = export_data.encode(encoding)
         return export_data
 
     def get_export_context_data(self, **kwargs):
         return self.get_context_data(**kwargs)
@@ -719,15 +722,15 @@
             raise PermissionDenied
 
         if getattr(self.get_export_form, 'is_original', False):
             form_type = self.get_export_form_class()
         else:
             form_type = self.get_export_form()
         formats = self.get_export_formats()
-        form = form_type(formats, self.get_export_resource_classes(), request.POST or None)
+        form = form_type(formats,  request.POST or None, resources=self.get_export_resource_classes())
         if form.is_valid():
             file_format = formats[
                 int(form.cleaned_data['file_format'])
             ]()
 
             queryset = self.get_export_queryset(request)
             export_data = self.get_export_data(
```

### Comparing `django-import-export-3.1.0/import_export/fields.py` & `django-import-export-3.2.0/import_export/fields.py`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/formats/base_formats.py` & `django-import-export-3.2.0/import_export/formats/base_formats.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import html
+import warnings
 
 import tablib
 from tablib.formats import registry
 
 
 class Format:
     def get_title(self):
@@ -78,31 +79,52 @@
             return False
         return True
 
     def get_title(self):
         return self.get_format().title
 
     def create_dataset(self, in_stream, **kwargs):
-        return tablib.import_set(in_stream, format=self.get_title())
+        return tablib.import_set(in_stream, format=self.get_title(), **kwargs)
 
-    def export_data(self, dataset, escape_output=False, **kwargs):
+    def export_data(self, dataset, **kwargs):
+        # remove the deprecated `escape_output` param if present
+        kwargs.pop("escape_output", None)
+        if kwargs.pop("escape_html", None):
+            self._escape_html(dataset)
+        if kwargs.pop("escape_formulae", None):
+            self._escape_formulae(dataset)
         return dataset.export(self.get_title(), **kwargs)
 
     def get_extension(self):
         return self.get_format().extensions[0]
 
     def get_content_type(self):
         return self.CONTENT_TYPE
 
     def can_import(self):
         return hasattr(self.get_format(), 'import_set')
 
     def can_export(self):
         return hasattr(self.get_format(), 'export_set')
 
+    def _escape_html(self, dataset):
+        for _ in dataset:
+            row = dataset.lpop()
+            row = [html.escape(str(cell)) for cell in row]
+            dataset.append(row)
+
+    def _escape_formulae(self, dataset):
+        def _do_escape(s):
+            return s.replace("=", "", 1) if s.startswith("=") else s
+
+        for _ in dataset:
+            row = dataset.lpop()
+            row = [_do_escape(str(cell)) for cell in row]
+            dataset.append(row)
+
 
 class TextFormat(TablibFormat):
 
     def create_dataset(self, in_stream, **kwargs):
         if isinstance(in_stream, bytes) and self.encoding:
             in_stream = in_stream.decode(self.encoding)
         return super().create_dataset(in_stream, **kwargs)
@@ -145,19 +167,21 @@
 
 class HTML(TextFormat):
     TABLIB_MODULE = 'tablib.formats._html'
     CONTENT_TYPE = 'text/html'
 
     def export_data(self, dataset, escape_output=False, **kwargs):
         if escape_output:
-            for _ in dataset:
-                row = dataset.lpop()
-                row = [html.escape(str(cell)) for cell in row]
-                dataset.append(row)
-        return dataset.export(self.get_title(), **kwargs)
+            warnings.warn(
+                "escape_output flag now deprecated - "
+                "this will be removed in a future release",
+                DeprecationWarning,
+            )
+            super()._escape_html(dataset)
+        return super().export_data(dataset, **kwargs)
 
 
 class XLS(TablibFormat):
     TABLIB_MODULE = 'tablib.formats._xls'
     CONTENT_TYPE = 'application/vnd.ms-excel'
 
     def create_dataset(self, in_stream):
@@ -198,15 +222,14 @@
         dataset.headers = [cell.value for cell in next(rows)]
 
         for row in rows:
             row_values = [cell.value for cell in row]
             dataset.append(row_values)
         return dataset
 
-
 #: These are the default formats for import and export. Whether they can be
 #: used or not is depending on their implementation in the tablib library.
 DEFAULT_FORMATS = [fmt for fmt in (
     CSV,
     XLS,
     XLSX,
     TSV,
```

### Comparing `django-import-export-3.1.0/import_export/forms.py` & `django-import-export-3.2.0/import_export/forms.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 import os.path
+import warnings
 
 from django import forms
 from django.conf import settings
 from django.contrib.admin.helpers import ActionForm
 from django.utils.translation import gettext_lazy as _
 
 
 class ImportExportFormBase(forms.Form):
     resource = forms.ChoiceField(
         label=_('Resource'),
         choices=(),
         required=False,
     )
 
-    def __init__(self, resources=None, *args, **kwargs):
+    def __init__(self,  *args, resources=None, **kwargs):
         super().__init__(*args, **kwargs)
+        if len(args) == 1 and resources is None:
+            # issue 1565: definition of __init__() was incorrect
+            # this logic included to aid backwards compatibility,
+            # for cases where users are calling with the original form.
+            # this check can be removed in a future release
+            warnings.warn(
+                "'resources' must be supplied as a named parameter",
+                category=DeprecationWarning
+            )
+            resources = args
+
         if resources and len(resources) > 1:
             resource_choices = []
             for i, resource in enumerate(resources):
                 resource_choices.append((i, resource.get_display_name()))
             self.fields['resource'].choices = resource_choices
         else:
             del self.fields['resource']
@@ -30,15 +42,16 @@
     )
     input_format = forms.ChoiceField(
         label=_('Format'),
         choices=(),
     )
 
     def __init__(self, import_formats, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+        resources = kwargs.pop("resources", None)
+        super().__init__(*args, resources=resources, **kwargs)
         choices = [
             (str(i), f().get_title())
             for i, f in enumerate(import_formats)
         ]
         if len(import_formats) > 1:
             choices.insert(0, ('', '---'))
             self.fields['import_file'].widget.attrs['class'] = 'guess_format'
@@ -73,15 +86,16 @@
 class ExportForm(ImportExportFormBase):
     file_format = forms.ChoiceField(
         label=_('Format'),
         choices=(),
         )
 
     def __init__(self, formats, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+        resources = kwargs.pop("resources", None)
+        super().__init__(*args, resources=resources, **kwargs)
         choices = []
         for i, f in enumerate(formats):
             choices.append((str(i), f().get_title(),))
         if len(formats) > 1:
             choices.insert(0, ('', '---'))
 
         self.fields['file_format'].choices = choices
```

### Comparing `django-import-export-3.1.0/import_export/instance_loaders.py` & `django-import-export-3.2.0/import_export/instance_loaders.py`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/locale/ar/LC_MESSAGES/django.mo` & `django-import-export-3.2.0/import_export/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/locale/ar/LC_MESSAGES/django.po` & `django-import-export-3.2.0/import_export/locale/ar/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-21 18:05+0000\n"
+"POT-Creation-Date: 2023-04-12 18:40+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -35,37 +35,37 @@
 msgstr ""
 
 #: admin.py:580 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
 msgstr "إستبراد"
 
-#: admin.py:749 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:752 templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
 msgstr "تصدير"
 
-#: admin.py:812
+#: admin.py:815
 msgid "You must select an export format."
 msgstr "يجب تحديد تنسيق التصدير."
 
-#: admin.py:835
+#: admin.py:838
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
 msgstr "تصدير %(verbose_name_plural)s المحددة"
 
-#: forms.py:11
+#: forms.py:12
 msgid "Resource"
 msgstr ""
 
-#: forms.py:29
+#: forms.py:41
 msgid "File to import"
 msgstr "ملف للإستيراد"
 
-#: forms.py:32 forms.py:75 forms.py:100
+#: forms.py:44 forms.py:88 forms.py:114
 msgid "Format"
 msgstr "تنسيق"
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
 msgstr "الرئيسية"
```

### Comparing `django-import-export-3.1.0/import_export/locale/bg/LC_MESSAGES/django.mo` & `django-import-export-3.2.0/import_export/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/locale/bg/LC_MESSAGES/django.po` & `django-import-export-3.2.0/import_export/locale/bg/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Hristo Gatsinski <gatsinski@gmail.com>, 2017.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-21 18:05+0000\n"
+"POT-Creation-Date: 2023-04-12 18:40+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Hristo Gatsinski <gatsinski@gmail.com>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: Bulgarian\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -34,37 +34,37 @@
 msgstr ""
 
 #: admin.py:580 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
 msgstr "Импортиране"
 
-#: admin.py:749 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:752 templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
 msgstr "Експортиране"
 
-#: admin.py:812
+#: admin.py:815
 msgid "You must select an export format."
 msgstr "Трябва да изберете формат за експортиране."
 
-#: admin.py:835
+#: admin.py:838
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
 msgstr "Експортиране на избраните %(verbose_name_plural)s"
 
-#: forms.py:11
+#: forms.py:12
 msgid "Resource"
 msgstr ""
 
-#: forms.py:29
+#: forms.py:41
 msgid "File to import"
 msgstr "Файл за импортиране"
 
-#: forms.py:32 forms.py:75 forms.py:100
+#: forms.py:44 forms.py:88 forms.py:114
 msgid "Format"
 msgstr "Формат"
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
 msgstr "Начало"
```

### Comparing `django-import-export-3.1.0/import_export/locale/ca/LC_MESSAGES/django.mo` & `django-import-export-3.2.0/import_export/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/locale/ca/LC_MESSAGES/django.po` & `django-import-export-3.2.0/import_export/locale/ca/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Manel Clos <manelclos@gmail.com>, 2016.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-21 18:05+0000\n"
+"POT-Creation-Date: 2023-04-12 18:40+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -34,37 +34,37 @@
 msgstr ""
 
 #: admin.py:580 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
 msgstr "Importar"
 
-#: admin.py:749 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:752 templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
 msgstr "Exportar"
 
-#: admin.py:812
+#: admin.py:815
 msgid "You must select an export format."
 msgstr "Heu de seleccionar un format d'exportació"
 
-#: admin.py:835
+#: admin.py:838
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
 msgstr "Exportar %(verbose_name_plural)s seleccionats"
 
-#: forms.py:11
+#: forms.py:12
 msgid "Resource"
 msgstr ""
 
-#: forms.py:29
+#: forms.py:41
 msgid "File to import"
 msgstr "Arxiu a importar"
 
-#: forms.py:32 forms.py:75 forms.py:100
+#: forms.py:44 forms.py:88 forms.py:114
 msgid "Format"
 msgstr "Format"
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
 msgstr "Inici"
```

### Comparing `django-import-export-3.1.0/import_export/locale/cs/LC_MESSAGES/django.mo` & `django-import-export-3.2.0/import_export/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/locale/cs/LC_MESSAGES/django.po` & `django-import-export-3.2.0/import_export/locale/cs/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-21 18:05+0000\n"
+"POT-Creation-Date: 2023-04-12 18:40+0100\n"
 "PO-Revision-Date: 2017-05-02 19:17+0200\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -34,37 +34,37 @@
 msgstr ""
 
 #: admin.py:580 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
 msgstr "Import"
 
-#: admin.py:749 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:752 templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
 msgstr "Export"
 
-#: admin.py:812
+#: admin.py:815
 msgid "You must select an export format."
 msgstr "Musíte vybrat formát pro export."
 
-#: admin.py:835
+#: admin.py:838
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
 msgstr "Vybrán export %(verbose_name_plural)s"
 
-#: forms.py:11
+#: forms.py:12
 msgid "Resource"
 msgstr ""
 
-#: forms.py:29
+#: forms.py:41
 msgid "File to import"
 msgstr "Soubor k importu"
 
-#: forms.py:32 forms.py:75 forms.py:100
+#: forms.py:44 forms.py:88 forms.py:114
 msgid "Format"
 msgstr "Formát"
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
 msgstr "Domů"
```

### Comparing `django-import-export-3.1.0/import_export/locale/de/LC_MESSAGES/django.mo` & `django-import-export-3.2.0/import_export/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/locale/de/LC_MESSAGES/django.po` & `django-import-export-3.2.0/import_export/locale/de/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-21 18:05+0000\n"
+"POT-Creation-Date: 2023-04-12 18:40+0100\n"
 "PO-Revision-Date: 2022-10-17 17:42+0200\n"
 "Last-Translator: Jannes Blobel <jannes.blobel@inlang.com>\n"
 "Language-Team: \n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -36,37 +36,37 @@
 "Stellen Sie sicher, dass du  das richtige Format für deine Datei gewählt hast"
 
 #: admin.py:580 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
 msgstr "Importieren"
 
-#: admin.py:749 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:752 templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
 msgstr "Exportieren"
 
-#: admin.py:812
+#: admin.py:815
 msgid "You must select an export format."
 msgstr "Es muss ein Exportformat ausgewählt werden."
 
-#: admin.py:835
+#: admin.py:838
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
 msgstr "Ausgewählte %(verbose_name_plural)s exportieren"
 
-#: forms.py:11
+#: forms.py:12
 msgid "Resource"
 msgstr "Ressource"
 
-#: forms.py:29
+#: forms.py:41
 msgid "File to import"
 msgstr "Zu importierende Datei"
 
-#: forms.py:32 forms.py:75 forms.py:100
+#: forms.py:44 forms.py:88 forms.py:114
 msgid "Format"
 msgstr "Dateiformat"
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
 msgstr "Start"
```

### Comparing `django-import-export-3.1.0/import_export/locale/es/LC_MESSAGES/django.mo` & `django-import-export-3.2.0/import_export/locale/sk/LC_MESSAGES/django.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -5,66 +5,66 @@
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
 
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
 msgstr ""
-"A continuación se muestra una vista previa de los datos a importar. Si estás "
-"satisfecho con los resultados, haz clic en 'Confirmar importación'"
+"Nižšie je zobrazený náhľad importovaných dát. Ak je všetko v poriadku, "
+"kliknite na tlačidlo 'Potvrdiť import'"
 
 msgid "Confirm import"
-msgstr "Confirmar importación"
+msgstr "Potvrdiť import"
 
 msgid "Delete"
-msgstr "Borrar"
+msgstr "Vymazaný"
 
 msgid "Errors"
-msgstr "Errores"
+msgstr "Chyby"
 
 msgid "Export"
-msgstr "Exportar"
+msgstr "Exportovať"
 
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "Exportar %(verbose_name_plural)s seleccionados"
+msgstr "Exportovať vybrané %(verbose_name_plural)s"
 
 msgid "File to import"
-msgstr "Fichero a importar"
+msgstr "Importovať súbor"
 
 msgid "Format"
-msgstr "Formato"
+msgstr "Formát"
 
 msgid "Home"
-msgstr "Inicio"
+msgstr "Domov"
 
 msgid "Import"
-msgstr "Importar"
+msgstr "Importovať"
 
 msgid "Line number"
-msgstr "Número de línea"
+msgstr "Číslo riadku"
 
 msgid "New"
-msgstr "Nuevo"
+msgstr "Nový"
 
 msgid "Preview"
-msgstr "Vista previa"
+msgstr "Náhľad"
 
 msgid "Skipped"
-msgstr "Omitido"
+msgstr "Preskočený"
 
 msgid "Submit"
-msgstr "Enviar"
+msgstr "Odoslať"
 
 msgid "This importer will import the following fields: "
-msgstr "Este importador importará los siguientes campos:"
+msgstr "Budú importované nasledujúce polia: "
 
 msgid "Update"
-msgstr "Actualizar"
+msgstr "Aktualizovaný"
 
 msgid "You must select an export format."
-msgstr "Debes seleccionar un formato de exportación."
+msgstr "Je potrebné vybrať formát exportu."
```

### Comparing `django-import-export-3.1.0/import_export/locale/es/LC_MESSAGES/django.po` & `django-import-export-3.2.0/import_export/locale/it/LC_MESSAGES/django.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-# SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# David Díaz <d.diazp@gmail.com>, 2015.
 #
-#, fuzzy
+# Christian Galeffi <chri@gallochri.com>, 2015.
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
+"Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-21 18:05+0000\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2023-04-12 18:40+0100\n"
+"PO-Revision-Date: 2015-08-30 20:32+0100\n"
+"Last-Translator: Christian Galeffi <chri@gallochri.com>\n"
+"Language-Team: Italian <kde-i18n-it@kde.org>\n"
+"Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"X-Generator: Poedit 1.5.4\n"
 
 #: admin.py:214
 #, python-format
 msgid "%s through import_export"
 msgstr ""
 
 #: admin.py:220
@@ -32,75 +31,75 @@
 "'{type(e).__name__}' encountered while trying to read file. Ensure you have "
 "chosen the correct format for the file. "
 msgstr ""
 
 #: admin.py:580 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
-msgstr "Importar"
+msgstr "Importare"
 
-#: admin.py:749 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:752 templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
-msgstr "Exportar"
+msgstr "Esportare"
 
-#: admin.py:812
+#: admin.py:815
 msgid "You must select an export format."
-msgstr "Debes seleccionar un formato de exportación."
+msgstr "Devi selezionare un formato di esportazione."
 
-#: admin.py:835
+#: admin.py:838
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "Exportar %(verbose_name_plural)s seleccionados"
+msgstr "Esporta selezionati %(verbose_name_plural)s"
 
-#: forms.py:11
+#: forms.py:12
 msgid "Resource"
 msgstr ""
 
-#: forms.py:29
+#: forms.py:41
 msgid "File to import"
-msgstr "Fichero a importar"
+msgstr "File da importare"
 
-#: forms.py:32 forms.py:75 forms.py:100
+#: forms.py:44 forms.py:88 forms.py:114
 msgid "Format"
 msgstr "Formato"
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
-msgstr "Inicio"
+msgstr "Home"
 
 #: templates/admin/import_export/export.html:36
 #: templates/admin/import_export/import.html:73
 msgid "Submit"
-msgstr "Enviar"
+msgstr "Inviare"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
 msgstr ""
-"A continuación se muestra una vista previa de los datos a importar. Si estás "
-"satisfecho con los resultados, haz clic en 'Confirmar importación'"
+"Questa è un'anteprima dei dati che saranno importati. Se il risultato è "
+"soddisfacente, premi 'Conferma importazione'"
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
-msgstr "Confirmar importación"
+msgstr "Conferma importazione"
 
 #: templates/admin/import_export/import.html:43
 msgid "This importer will import the following fields: "
-msgstr "Este importador importará los siguientes campos:"
+msgstr "Verranno importati i seguenti campi:"
 
 #: templates/admin/import_export/import.html:83
 #: templates/admin/import_export/import.html:114
 msgid "Errors"
-msgstr "Errores"
+msgstr "Errori"
 
 #: templates/admin/import_export/import.html:94
 msgid "Line number"
-msgstr "Número de línea"
+msgstr "Numero linea"
 
 #: templates/admin/import_export/import.html:106
 msgid "Some rows failed to validate"
 msgstr ""
 
 #: templates/admin/import_export/import.html:108
 msgid ""
@@ -114,24 +113,24 @@
 
 #: templates/admin/import_export/import.html:140
 msgid "Non field specific"
 msgstr ""
 
 #: templates/admin/import_export/import.html:163
 msgid "Preview"
-msgstr "Vista previa"
+msgstr "Anteprima"
 
 #: templates/admin/import_export/import.html:178
 msgid "New"
-msgstr "Nuevo"
+msgstr "Nuovo"
 
 #: templates/admin/import_export/import.html:180
 msgid "Skipped"
-msgstr "Omitido"
+msgstr "Salta"
 
 #: templates/admin/import_export/import.html:182
 msgid "Delete"
-msgstr "Borrar"
+msgstr "Cancella"
 
 #: templates/admin/import_export/import.html:184
 msgid "Update"
-msgstr "Actualizar"
+msgstr "Aggiorna"
```

### Comparing `django-import-export-3.1.0/import_export/locale/es_AR/LC_MESSAGES/django.mo` & `django-import-export-3.2.0/import_export/locale/pl/LC_MESSAGES/django.mo`

 * *Files 27% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,71 +1,77 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: \n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2015-10-11 18:49-0300\n"
-"Last-Translator: Gonzalo Bustos\n"
-"Language-Team: Spanish (Argentina)\n"
-"Language: es_AR\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Poedit 1.6.10\n"
+"Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
+"|| n%100>=20) ? 1 : 2);\n"
+
+msgid "%s through import_export"
+msgstr "%s przez import_export"
 
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
 msgstr ""
-"A continuación se muestra una vista previa de los datos a importar. Si está "
-"satisfecho con los resultados, haga clic en 'Confirmar importación'"
+"Poniżej znajdują się przykładowe dane do zaimportowania. Jeśli "
+"satysfakcjonuje Cię wynik, kliknij 'Potwierdź import'"
 
 msgid "Confirm import"
-msgstr "Confirmar importación"
+msgstr "Potwierdź import"
 
 msgid "Delete"
-msgstr "Borrar"
+msgstr "Usuń"
 
 msgid "Errors"
-msgstr "Errores"
+msgstr "Błędy"
 
 msgid "Export"
-msgstr "Exportar"
+msgstr "Eksport"
 
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "Exportar %(verbose_name_plural)s seleccionados"
+msgstr "Eksportuj wybrane %(verbose_name_plural)s"
 
 msgid "File to import"
-msgstr "Archivo a importar"
+msgstr "Plik do importu"
 
 msgid "Format"
-msgstr "Formato"
+msgstr "Format"
 
 msgid "Home"
-msgstr "Inicio"
+msgstr "Powrót"
 
 msgid "Import"
-msgstr "Importar"
+msgstr "Import"
+
+msgid "Import finished, with {} new and {} updated {}."
+msgstr "Import zakończony, z {} nowymi i {} zaktualizowanymi {}."
 
 msgid "Line number"
-msgstr "Número de línea"
+msgstr "Numer linii"
 
 msgid "New"
-msgstr "Nuevo"
+msgstr "Nowy"
 
 msgid "Preview"
-msgstr "Vista previa"
+msgstr "Podgląd"
 
 msgid "Skipped"
-msgstr "Omitido"
+msgstr "Pominięty"
 
 msgid "Submit"
-msgstr "Enviar"
+msgstr "Wyślij"
 
 msgid "This importer will import the following fields: "
-msgstr "Este importador importará los siguientes campos:"
+msgstr "Zostaną zaimportowane następujące pola: "
 
 msgid "Update"
-msgstr "Actualizar"
+msgstr "Zaktualizowany"
 
 msgid "You must select an export format."
-msgstr "Debe seleccionar un formato de exportación."
+msgstr "Musisz wybrać format eksportu."
```

### Comparing `django-import-export-3.1.0/import_export/locale/es_AR/LC_MESSAGES/django.po` & `django-import-export-3.2.0/import_export/locale/nl/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,137 +1,139 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Gonzalo Bustos, 2015.
+# Bram Janssen <zakelijk@bram-janssen.nl>, 2019.
 #
+#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: \n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-21 18:05+0000\n"
-"PO-Revision-Date: 2015-10-11 18:49-0300\n"
-"Last-Translator: Gonzalo Bustos\n"
-"Language-Team: Spanish (Argentina)\n"
-"Language: es_AR\n"
+"POT-Creation-Date: 2023-04-12 18:40+0100\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Poedit 1.6.10\n"
 
 #: admin.py:214
 #, python-format
 msgid "%s through import_export"
-msgstr ""
+msgstr "%s door import_export"
 
 #: admin.py:220
 msgid "Import finished, with {} new and {} updated {}."
-msgstr ""
+msgstr "Import is klaar met {} nieuwe en {} geupdate {}."
 
 #: admin.py:456
 msgid ""
 "'{type(e).__name__}' encountered while trying to read file. Ensure you have "
 "chosen the correct format for the file. "
 msgstr ""
 
 #: admin.py:580 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
-msgstr "Importar"
+msgstr "Importeren"
 
-#: admin.py:749 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:752 templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
-msgstr "Exportar"
+msgstr "Exporteren"
 
-#: admin.py:812
+#: admin.py:815
 msgid "You must select an export format."
-msgstr "Debe seleccionar un formato de exportación."
+msgstr "U moet een export formaat kiezen."
 
-#: admin.py:835
+#: admin.py:838
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "Exportar %(verbose_name_plural)s seleccionados"
+msgstr "Exporteer geselecteerde %(verbose_name_plural)s"
 
-#: forms.py:11
+#: forms.py:12
 msgid "Resource"
 msgstr ""
 
-#: forms.py:29
+#: forms.py:41
 msgid "File to import"
-msgstr "Archivo a importar"
+msgstr "Bestand om te importeren"
 
-#: forms.py:32 forms.py:75 forms.py:100
+#: forms.py:44 forms.py:88 forms.py:114
 msgid "Format"
-msgstr "Formato"
+msgstr "Formaat"
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
-msgstr "Inicio"
+msgstr "Terug"
 
 #: templates/admin/import_export/export.html:36
 #: templates/admin/import_export/import.html:73
 msgid "Submit"
-msgstr "Enviar"
+msgstr "Indienen"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
 msgstr ""
-"A continuación se muestra una vista previa de los datos a importar. Si está "
-"satisfecho con los resultados, haga clic en 'Confirmar importación'"
+"Hieronder is een voorvertoning van de data die geïmporteerd zal worden. Als "
+"u tevreden bent met het resultaat, klik dan op 'Accepteer de import'."
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
-msgstr "Confirmar importación"
+msgstr "Accepteer de import"
 
 #: templates/admin/import_export/import.html:43
 msgid "This importer will import the following fields: "
-msgstr "Este importador importará los siguientes campos:"
+msgstr "Deze import zal de volgende velden toevoegen"
 
 #: templates/admin/import_export/import.html:83
 #: templates/admin/import_export/import.html:114
 msgid "Errors"
-msgstr "Errores"
+msgstr "Fouten"
 
 #: templates/admin/import_export/import.html:94
 msgid "Line number"
-msgstr "Número de línea"
+msgstr "Regel nummer"
 
 #: templates/admin/import_export/import.html:106
 msgid "Some rows failed to validate"
-msgstr ""
+msgstr "Sommige regels zijn niet goedgekeurd"
 
 #: templates/admin/import_export/import.html:108
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
 msgstr ""
+"Verander alstublieft de volgende fouten in uw data waar mogelijk. Upload het "
+"bestand daarna nogmaals met het veld hierboven."
 
 #: templates/admin/import_export/import.html:113
 msgid "Row"
-msgstr ""
+msgstr "Regel"
 
 #: templates/admin/import_export/import.html:140
 msgid "Non field specific"
-msgstr ""
+msgstr "Niet veld specifiek"
 
 #: templates/admin/import_export/import.html:163
 msgid "Preview"
-msgstr "Vista previa"
+msgstr "Voorbeeldweergave"
 
 #: templates/admin/import_export/import.html:178
 msgid "New"
-msgstr "Nuevo"
+msgstr "Nieuw"
 
 #: templates/admin/import_export/import.html:180
 msgid "Skipped"
-msgstr "Omitido"
+msgstr "Overgeslagen"
 
 #: templates/admin/import_export/import.html:182
 msgid "Delete"
-msgstr "Borrar"
+msgstr "Verwijderen"
 
 #: templates/admin/import_export/import.html:184
 msgid "Update"
-msgstr "Actualizar"
+msgstr "Bijwerken"
```

### Comparing `django-import-export-3.1.0/import_export/locale/fa/LC_MESSAGES/django.mo` & `django-import-export-3.2.0/import_export/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/locale/fa/LC_MESSAGES/django.po` & `django-import-export-3.2.0/import_export/locale/fa/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is distributed under the same license as the django-import-export package.
 #
 # Yazdan Ranjbar <Yazdan_ra@icloud.com>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: 0.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-21 18:05+0000\n"
+"POT-Creation-Date: 2023-04-12 18:40+0100\n"
 "PO-Revision-Date: 2021-03-09 00:29+0030\n"
 "Last-Translator: Yazdan Ranjbar <Yazdan_ra@icloud.com>\n"
 "Language-Team: Persain/Farsi <kde-i18n-it@kde.org>\n"
 "Language: Farsi/Persian\n"
 "MIME-Version: 0.1\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -33,37 +33,37 @@
 msgstr ""
 
 #: admin.py:580 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
 msgstr "بارگذاری"
 
-#: admin.py:749 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:752 templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
 msgstr "خروجی"
 
-#: admin.py:812
+#: admin.py:815
 msgid "You must select an export format."
 msgstr "شما باید یک فرمت خروجی انتخاب کنید"
 
-#: admin.py:835
+#: admin.py:838
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
 msgstr "خروجی %(verbose_name_plural)s انتخاب شده"
 
-#: forms.py:11
+#: forms.py:12
 msgid "Resource"
 msgstr ""
 
-#: forms.py:29
+#: forms.py:41
 msgid "File to import"
 msgstr "قایل برای بارگذاری"
 
-#: forms.py:32 forms.py:75 forms.py:100
+#: forms.py:44 forms.py:88 forms.py:114
 msgid "Format"
 msgstr "فرمت"
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
 msgstr "خانه"
```

### Comparing `django-import-export-3.1.0/import_export/locale/fr/LC_MESSAGES/django.mo` & `django-import-export-3.2.0/import_export/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/locale/fr/LC_MESSAGES/django.po` & `django-import-export-3.2.0/import_export/locale/fr/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-21 18:05+0000\n"
+"POT-Creation-Date: 2023-04-12 18:40+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -34,37 +34,37 @@
 msgstr ""
 
 #: admin.py:580 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
 msgstr "Importer"
 
-#: admin.py:749 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:752 templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
 msgstr "Exporter"
 
-#: admin.py:812
+#: admin.py:815
 msgid "You must select an export format."
 msgstr "Vous devez sélectionner un format d'exportation."
 
-#: admin.py:835
+#: admin.py:838
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
 msgstr "Exporter %(verbose_name_plural)s selectionnés"
 
-#: forms.py:11
+#: forms.py:12
 msgid "Resource"
 msgstr ""
 
-#: forms.py:29
+#: forms.py:41
 msgid "File to import"
 msgstr "Fichier à importer"
 
-#: forms.py:32 forms.py:75 forms.py:100
+#: forms.py:44 forms.py:88 forms.py:114
 msgid "Format"
 msgstr "Format"
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
 msgstr "Accueil"
```

### Comparing `django-import-export-3.1.0/import_export/locale/it/LC_MESSAGES/django.mo` & `django-import-export-3.2.0/import_export/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/locale/it/LC_MESSAGES/django.po` & `django-import-export-3.2.0/import_export/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,136 +1,138 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 #
-# Christian Galeffi <chri@gallochri.com>, 2015.
+# Dan <pluthd@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-21 18:05+0000\n"
-"PO-Revision-Date: 2015-08-30 20:32+0100\n"
-"Last-Translator: Christian Galeffi <chri@gallochri.com>\n"
-"Language-Team: Italian <kde-i18n-it@kde.org>\n"
-"Language: it\n"
+"POT-Creation-Date: 2023-04-12 18:40+0100\n"
+"PO-Revision-Date: 2020-06-06 10:30-0500\n"
+"Last-Translator: Daniel Pluth <pluthd@gmail.com>\n"
+"Language-Team: \n"
+"Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Poedit 1.5.4\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"X-Generator: Lokalize 20.04.1\n"
 
 #: admin.py:214
 #, python-format
 msgid "%s through import_export"
-msgstr ""
+msgstr "%s através import_export "
 
 #: admin.py:220
 msgid "Import finished, with {} new and {} updated {}."
-msgstr ""
+msgstr "A importação foi completada com {} novas e {} atualizadas {}"
 
 #: admin.py:456
 msgid ""
 "'{type(e).__name__}' encountered while trying to read file. Ensure you have "
 "chosen the correct format for the file. "
 msgstr ""
 
 #: admin.py:580 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
-msgstr "Importare"
+msgstr "Importar"
 
-#: admin.py:749 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:752 templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
-msgstr "Esportare"
+msgstr "Exportar"
 
-#: admin.py:812
+#: admin.py:815
 msgid "You must select an export format."
-msgstr "Devi selezionare un formato di esportazione."
+msgstr "Você tem que selecionar um formato de exportação."
 
-#: admin.py:835
+#: admin.py:838
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "Esporta selezionati %(verbose_name_plural)s"
+msgstr "Exportar %(verbose_name_plural)s selecionados"
 
-#: forms.py:11
+#: forms.py:12
 msgid "Resource"
 msgstr ""
 
-#: forms.py:29
+#: forms.py:41
 msgid "File to import"
-msgstr "File da importare"
+msgstr "Arquivo a ser importado"
 
-#: forms.py:32 forms.py:75 forms.py:100
+#: forms.py:44 forms.py:88 forms.py:114
 msgid "Format"
 msgstr "Formato"
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
-msgstr "Home"
+msgstr "Início"
 
 #: templates/admin/import_export/export.html:36
 #: templates/admin/import_export/import.html:73
 msgid "Submit"
-msgstr "Inviare"
+msgstr "Enviar"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
 msgstr ""
-"Questa è un'anteprima dei dati che saranno importati. Se il risultato è "
-"soddisfacente, premi 'Conferma importazione'"
+"Ver abaixo uma prévia dos dados a serem importados. Se você esta satisfeito "
+"com os resultados, clique em 'Confirmar importação'"
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
-msgstr "Conferma importazione"
+msgstr "Confirmar importação"
 
 #: templates/admin/import_export/import.html:43
 msgid "This importer will import the following fields: "
-msgstr "Verranno importati i seguenti campi:"
+msgstr "Este importador vai importar os seguintes campos:"
 
 #: templates/admin/import_export/import.html:83
 #: templates/admin/import_export/import.html:114
 msgid "Errors"
-msgstr "Errori"
+msgstr "Erros"
 
 #: templates/admin/import_export/import.html:94
 msgid "Line number"
-msgstr "Numero linea"
+msgstr "Número da linha"
 
 #: templates/admin/import_export/import.html:106
 msgid "Some rows failed to validate"
-msgstr ""
+msgstr "Algumas linhas não foram validadas"
 
 #: templates/admin/import_export/import.html:108
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
 msgstr ""
+"Por favor corrigir os erros nos dados onde possível e recarregar os dados "
+"com o formato acima."
 
 #: templates/admin/import_export/import.html:113
 msgid "Row"
-msgstr ""
+msgstr "Linha"
 
 #: templates/admin/import_export/import.html:140
 msgid "Non field specific"
-msgstr ""
+msgstr "Campo não é específico"
 
 #: templates/admin/import_export/import.html:163
 msgid "Preview"
-msgstr "Anteprima"
+msgstr "Prévia"
 
 #: templates/admin/import_export/import.html:178
 msgid "New"
-msgstr "Nuovo"
+msgstr "Novo"
 
 #: templates/admin/import_export/import.html:180
 msgid "Skipped"
-msgstr "Salta"
+msgstr "Não usados"
 
 #: templates/admin/import_export/import.html:182
 msgid "Delete"
-msgstr "Cancella"
+msgstr "Remover"
 
 #: templates/admin/import_export/import.html:184
 msgid "Update"
-msgstr "Aggiorna"
+msgstr "Atualizar"
```

### Comparing `django-import-export-3.1.0/import_export/locale/ja/LC_MESSAGES/django.mo` & `django-import-export-3.2.0/import_export/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/locale/ja/LC_MESSAGES/django.po` & `django-import-export-3.2.0/import_export/locale/ja/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-21 18:05+0000\n"
+"POT-Creation-Date: 2023-04-12 18:40+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -34,37 +34,37 @@
 msgstr ""
 
 #: admin.py:580 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
 msgstr "インポート"
 
-#: admin.py:749 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:752 templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
 msgstr "エクスポート"
 
-#: admin.py:812
+#: admin.py:815
 msgid "You must select an export format."
 msgstr "エクスポートフォーマットを選択してください。"
 
-#: admin.py:835
+#: admin.py:838
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
 msgstr "選択した %(verbose_name_plural)s をエクスポート"
 
-#: forms.py:11
+#: forms.py:12
 msgid "Resource"
 msgstr ""
 
-#: forms.py:29
+#: forms.py:41
 msgid "File to import"
 msgstr "インポートするファイル"
 
-#: forms.py:32 forms.py:75 forms.py:100
+#: forms.py:44 forms.py:88 forms.py:114
 msgid "Format"
 msgstr "フォーマット"
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
 msgstr "ホーム"
```

### Comparing `django-import-export-3.1.0/import_export/locale/ko/LC_MESSAGES/django.mo` & `django-import-export-3.2.0/import_export/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/locale/ko/LC_MESSAGES/django.po` & `django-import-export-3.2.0/import_export/locale/ko/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Jinmyeong Cho <britzegs@gmail.com>, 2020.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-21 18:05+0000\n"
+"POT-Creation-Date: 2023-04-12 18:40+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Yeongkwang Yang <immutable000@gmail.com>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -34,37 +34,37 @@
 msgstr ""
 
 #: admin.py:580 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
 msgstr "가져오기"
 
-#: admin.py:749 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:752 templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
 msgstr "내보내기"
 
-#: admin.py:812
+#: admin.py:815
 msgid "You must select an export format."
 msgstr "내보낼 형식을 선택해주세요."
 
-#: admin.py:835
+#: admin.py:838
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
 msgstr "선택한 %(verbose_name_plural)s 내보내기"
 
-#: forms.py:11
+#: forms.py:12
 msgid "Resource"
 msgstr ""
 
-#: forms.py:29
+#: forms.py:41
 msgid "File to import"
 msgstr "파일"
 
-#: forms.py:32 forms.py:75 forms.py:100
+#: forms.py:44 forms.py:88 forms.py:114
 msgid "Format"
 msgstr "형식"
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
 msgstr ""
```

### Comparing `django-import-export-3.1.0/import_export/locale/kz/LC_MESSAGES/django.mo` & `django-import-export-3.2.0/import_export/locale/kz/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/locale/kz/LC_MESSAGES/django.po` & `django-import-export-3.2.0/import_export/locale/kz/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-21 18:05+0000\n"
+"POT-Creation-Date: 2023-04-12 18:40+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Muslim Beibytuly <muslimbeibytuly@gmail.com>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: Kazakh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -33,37 +33,37 @@
 msgstr ""
 
 #: admin.py:580 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
 msgstr "Импорт"
 
-#: admin.py:749 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:752 templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
 msgstr "Экспорт"
 
-#: admin.py:812
+#: admin.py:815
 msgid "You must select an export format."
 msgstr "Сіз экспорт форматын таңдауыңыз керек."
 
-#: admin.py:835
+#: admin.py:838
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
 msgstr "Таңдалған %(verbose_name_plural)s экспорттаңыз"
 
-#: forms.py:11
+#: forms.py:12
 msgid "Resource"
 msgstr ""
 
-#: forms.py:29
+#: forms.py:41
 msgid "File to import"
 msgstr "Импорттауға арналған файл"
 
-#: forms.py:32 forms.py:75 forms.py:100
+#: forms.py:44 forms.py:88 forms.py:114
 msgid "Format"
 msgstr "Формат"
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
 msgstr "Басты бет"
```

### Comparing `django-import-export-3.1.0/import_export/locale/nl/LC_MESSAGES/django.mo` & `django-import-export-3.2.0/import_export/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/locale/nl/LC_MESSAGES/django.po` & `django-import-export-3.2.0/import_export/locale/es/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,139 +1,143 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Bram Janssen <zakelijk@bram-janssen.nl>, 2019.
+# David Díaz <d.diazp@gmail.com>, 2015.
+# Santiago Muñoz <smunoz@mythologylabs.com.uy>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-21 18:05+0000\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2023-04-12 18:40+0100\n"
+"PO-Revision-Date: 2023-02-22 10:44-0300\n"
+"Last-Translator: Santiago Muñoz <smunoz@mythologylabs.com.uy>\n"
+"Language-Team: Spanish\n"
+"Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin.py:214
 #, python-format
 msgid "%s through import_export"
-msgstr "%s door import_export"
+msgstr ""
 
 #: admin.py:220
 msgid "Import finished, with {} new and {} updated {}."
-msgstr "Import is klaar met {} nieuwe en {} geupdate {}."
+msgstr "Proceso de importación finalizado, con {} nuevos y {} actualizados"
 
 #: admin.py:456
 msgid ""
 "'{type(e).__name__}' encountered while trying to read file. Ensure you have "
 "chosen the correct format for the file. "
 msgstr ""
+"Se encontró '{type(e).__name__}' mientras se intentaba leer el archivo."
+"Asegúrese que seleccionó el formato correcto para el archivo."
 
 #: admin.py:580 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
-msgstr "Importeren"
+msgstr "Importar"
 
-#: admin.py:749 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:752 templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
-msgstr "Exporteren"
+msgstr "Exportar"
 
-#: admin.py:812
+#: admin.py:815
 msgid "You must select an export format."
-msgstr "U moet een export formaat kiezen."
+msgstr "Debes seleccionar un formato de exportación."
 
-#: admin.py:835
+#: admin.py:838
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "Exporteer geselecteerde %(verbose_name_plural)s"
+msgstr "Exportar %(verbose_name_plural)s seleccionados"
 
-#: forms.py:11
+#: forms.py:12
 msgid "Resource"
-msgstr ""
+msgstr "Recurso"
 
-#: forms.py:29
+#: forms.py:41
 msgid "File to import"
-msgstr "Bestand om te importeren"
+msgstr "Fichero a importar"
 
-#: forms.py:32 forms.py:75 forms.py:100
+#: forms.py:44 forms.py:88 forms.py:114
 msgid "Format"
-msgstr "Formaat"
+msgstr "Formato"
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
-msgstr "Terug"
+msgstr "Inicio"
 
 #: templates/admin/import_export/export.html:36
 #: templates/admin/import_export/import.html:73
 msgid "Submit"
-msgstr "Indienen"
+msgstr "Enviar"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
 msgstr ""
-"Hieronder is een voorvertoning van de data die geïmporteerd zal worden. Als "
-"u tevreden bent met het resultaat, klik dan op 'Accepteer de import'."
+"A continuación se muestra una vista previa de los datos a importar. Si estás "
+"satisfecho con los resultados, haz clic en 'Confirmar importación'"
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
-msgstr "Accepteer de import"
+msgstr "Confirmar importación"
 
 #: templates/admin/import_export/import.html:43
 msgid "This importer will import the following fields: "
-msgstr "Deze import zal de volgende velden toevoegen"
+msgstr "Este importador importará los siguientes campos:"
 
 #: templates/admin/import_export/import.html:83
 #: templates/admin/import_export/import.html:114
 msgid "Errors"
-msgstr "Fouten"
+msgstr "Errores"
 
 #: templates/admin/import_export/import.html:94
 msgid "Line number"
-msgstr "Regel nummer"
+msgstr "Número de línea"
 
 #: templates/admin/import_export/import.html:106
 msgid "Some rows failed to validate"
-msgstr "Sommige regels zijn niet goedgekeurd"
+msgstr "Falló la validación de algunas filas"
 
 #: templates/admin/import_export/import.html:108
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
 msgstr ""
-"Verander alstublieft de volgende fouten in uw data waar mogelijk. Upload het "
-"bestand daarna nogmaals met het veld hierboven."
+"Por favor corrija los siguientes errores en la información ingresada "
+"dondesea posible, luego vuelva a subir el archivo utilizando el formulario "
+"de laparte superior."
 
 #: templates/admin/import_export/import.html:113
 msgid "Row"
-msgstr "Regel"
+msgstr "Fila"
 
 #: templates/admin/import_export/import.html:140
 msgid "Non field specific"
-msgstr "Niet veld specifiek"
+msgstr "No específico del campo"
 
 #: templates/admin/import_export/import.html:163
 msgid "Preview"
-msgstr "Voorbeeldweergave"
+msgstr "Vista previa"
 
 #: templates/admin/import_export/import.html:178
 msgid "New"
-msgstr "Nieuw"
+msgstr "Nuevo"
 
 #: templates/admin/import_export/import.html:180
 msgid "Skipped"
-msgstr "Overgeslagen"
+msgstr "Omitido"
 
 #: templates/admin/import_export/import.html:182
 msgid "Delete"
-msgstr "Verwijderen"
+msgstr "Borrar"
 
 #: templates/admin/import_export/import.html:184
 msgid "Update"
-msgstr "Bijwerken"
+msgstr "Actualizar"
```

### Comparing `django-import-export-3.1.0/import_export/locale/pl/LC_MESSAGES/django.mo` & `django-import-export-3.2.0/import_export/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files 25% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,77 +1,85 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Last-Translator: hao wang <173300430@qq.com>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
-"|| n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "%s through import_export"
-msgstr "%s przez import_export"
+msgstr "%s 通过 django-import-export导入"
 
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
-msgstr ""
-"Poniżej znajdują się przykładowe dane do zaimportowania. Jeśli "
-"satysfakcjonuje Cię wynik, kliknij 'Potwierdź import'"
+msgstr "以下是导入数据的预览。如果确认结果没有问题，可以点击 “确认导入”"
 
 msgid "Confirm import"
-msgstr "Potwierdź import"
+msgstr "确认导入"
 
 msgid "Delete"
-msgstr "Usuń"
+msgstr "删除"
 
 msgid "Errors"
-msgstr "Błędy"
+msgstr "错误"
 
 msgid "Export"
-msgstr "Eksport"
+msgstr "导出"
 
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "Eksportuj wybrane %(verbose_name_plural)s"
+msgstr "导出选中的 %(verbose_name_plural)s"
 
 msgid "File to import"
-msgstr "Plik do importu"
+msgstr "导入文件"
 
 msgid "Format"
-msgstr "Format"
-
-msgid "Home"
-msgstr "Powrót"
+msgstr "格式"
 
 msgid "Import"
-msgstr "Import"
+msgstr "导入"
 
 msgid "Import finished, with {} new and {} updated {}."
-msgstr "Import zakończony, z {} nowymi i {} zaktualizowanymi {}."
+msgstr "导入成功，新增{}条记录，更新{}条记录。"
 
 msgid "Line number"
-msgstr "Numer linii"
+msgstr "行号"
 
 msgid "New"
-msgstr "Nowy"
+msgstr "新增"
+
+msgid "Non field specific"
+msgstr "没有指定的字段"
+
+msgid ""
+"Please correct these errors in your data where possible, then reupload it "
+"using the form above."
+msgstr "请使用上面的表单，纠正这些提示有错误的数据，并重新上传"
 
 msgid "Preview"
-msgstr "Podgląd"
+msgstr "预览"
+
+msgid "Row"
+msgstr "行"
 
 msgid "Skipped"
-msgstr "Pominięty"
+msgstr "忽略"
+
+msgid "Some rows failed to validate"
+msgstr "某些行验数据证失败"
 
 msgid "Submit"
-msgstr "Wyślij"
+msgstr "提交"
 
 msgid "This importer will import the following fields: "
-msgstr "Zostaną zaimportowane następujące pola: "
+msgstr "此次将导入以下字段："
 
 msgid "Update"
-msgstr "Zaktualizowany"
+msgstr "更新"
 
 msgid "You must select an export format."
-msgstr "Musisz wybrać format eksportu."
+msgstr "您必须选择一个导出格式。"
```

### Comparing `django-import-export-3.1.0/import_export/locale/pl/LC_MESSAGES/django.po` & `django-import-export-3.2.0/import_export/locale/es_AR/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,138 +1,143 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Ludwik Trammer <ludwik@gmail.com>, 2015.
+# Gonzalo Bustos, 2015.
+# Santiago Muñoz <smunoz@mythologylabs.com.uy>, 2023.
 #
-#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
+"Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-21 18:05+0000\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2023-04-12 18:40+0100\n"
+"PO-Revision-Date: 2023-02-22 10:44-0300\n"
+"Last-Translator: Santiago Muñoz <smunoz@mythologylabs.com.uy>\n"
+"Language-Team: Spanish (Argentina)\n"
+"Language: es_AR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
-"|| n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"X-Generator: Poedit 1.6.10\n"
 
 #: admin.py:214
 #, python-format
 msgid "%s through import_export"
-msgstr "%s przez import_export"
+msgstr ""
 
 #: admin.py:220
 msgid "Import finished, with {} new and {} updated {}."
-msgstr "Import zakończony, z {} nowymi i {} zaktualizowanymi {}."
+msgstr "Proceso de importación finalizado, con {} nuevos y {} actualizados"
 
 #: admin.py:456
 msgid ""
 "'{type(e).__name__}' encountered while trying to read file. Ensure you have "
 "chosen the correct format for the file. "
 msgstr ""
+"Se encontró '{type(e).__name__}' mientras se intentaba leer el archivo."
+"Asegúrese que seleccionó el formato correcto para el archivo."
 
 #: admin.py:580 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
-msgstr "Import"
+msgstr "Importar"
 
-#: admin.py:749 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:752 templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
-msgstr "Eksport"
+msgstr "Exportar"
 
-#: admin.py:812
+#: admin.py:815
 msgid "You must select an export format."
-msgstr "Musisz wybrać format eksportu."
+msgstr "Debe seleccionar un formato de exportación."
 
-#: admin.py:835
+#: admin.py:838
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "Eksportuj wybrane %(verbose_name_plural)s"
+msgstr "Exportar %(verbose_name_plural)s seleccionados"
 
-#: forms.py:11
+#: forms.py:12
 msgid "Resource"
-msgstr ""
+msgstr "Recurso"
 
-#: forms.py:29
+#: forms.py:41
 msgid "File to import"
-msgstr "Plik do importu"
+msgstr "Archivo a importar"
 
-#: forms.py:32 forms.py:75 forms.py:100
+#: forms.py:44 forms.py:88 forms.py:114
 msgid "Format"
-msgstr "Format"
+msgstr "Formato"
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
-msgstr "Powrót"
+msgstr "Inicio"
 
 #: templates/admin/import_export/export.html:36
 #: templates/admin/import_export/import.html:73
 msgid "Submit"
-msgstr "Wyślij"
+msgstr "Enviar"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
 msgstr ""
-"Poniżej znajdują się przykładowe dane do zaimportowania. Jeśli "
-"satysfakcjonuje Cię wynik, kliknij 'Potwierdź import'"
+"A continuación se muestra una vista previa de los datos a importar. Si está "
+"satisfecho con los resultados, haga clic en 'Confirmar importación'"
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
-msgstr "Potwierdź import"
+msgstr "Confirmar importación"
 
 #: templates/admin/import_export/import.html:43
 msgid "This importer will import the following fields: "
-msgstr "Zostaną zaimportowane następujące pola: "
+msgstr "Este importador importará los siguientes campos:"
 
 #: templates/admin/import_export/import.html:83
 #: templates/admin/import_export/import.html:114
 msgid "Errors"
-msgstr "Błędy"
+msgstr "Errores"
 
 #: templates/admin/import_export/import.html:94
 msgid "Line number"
-msgstr "Numer linii"
+msgstr "Número de línea"
 
 #: templates/admin/import_export/import.html:106
 msgid "Some rows failed to validate"
-msgstr ""
+msgstr "Falló la validación de algunas filas"
 
 #: templates/admin/import_export/import.html:108
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
 msgstr ""
+"Por favor corrija los siguientes errores en la información ingresada "
+"dondesea posible, luego vuelva a subir el archivo utilizando el formulario "
+"de laparte superior."
 
 #: templates/admin/import_export/import.html:113
 msgid "Row"
-msgstr ""
+msgstr "Fila"
 
 #: templates/admin/import_export/import.html:140
 msgid "Non field specific"
-msgstr ""
+msgstr "No específico del campo"
 
 #: templates/admin/import_export/import.html:163
 msgid "Preview"
-msgstr "Podgląd"
+msgstr "Vista previa"
 
 #: templates/admin/import_export/import.html:178
 msgid "New"
-msgstr "Nowy"
+msgstr "Nuevo"
 
 #: templates/admin/import_export/import.html:180
 msgid "Skipped"
-msgstr "Pominięty"
+msgstr "Omitido"
 
 #: templates/admin/import_export/import.html:182
 msgid "Delete"
-msgstr "Usuń"
+msgstr "Borrar"
 
 #: templates/admin/import_export/import.html:184
 msgid "Update"
-msgstr "Zaktualizowany"
+msgstr "Actualizar"
```

### Comparing `django-import-export-3.1.0/import_export/locale/pt_BR/LC_MESSAGES/django.mo` & `django-import-export-3.2.0/import_export/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/locale/pt_BR/LC_MESSAGES/django.po` & `django-import-export-3.2.0/import_export/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,138 +1,135 @@
+# SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
-# Dan <pluthd@gmail.com>, 2020.
+#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: \n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-21 18:05+0000\n"
-"PO-Revision-Date: 2020-06-06 10:30-0500\n"
-"Last-Translator: Daniel Pluth <pluthd@gmail.com>\n"
-"Language-Team: \n"
-"Language: pt_BR\n"
+"POT-Creation-Date: 2023-04-12 18:40+0100\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: hao wang <173300430@qq.com>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
-"X-Generator: Lokalize 20.04.1\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: admin.py:214
 #, python-format
 msgid "%s through import_export"
-msgstr "%s através import_export "
+msgstr "%s 通过 django-import-export导入"
 
 #: admin.py:220
 msgid "Import finished, with {} new and {} updated {}."
-msgstr "A importação foi completada com {} novas e {} atualizadas {}"
+msgstr "导入成功，新增{}条记录，更新{}条记录。"
 
 #: admin.py:456
 msgid ""
 "'{type(e).__name__}' encountered while trying to read file. Ensure you have "
 "chosen the correct format for the file. "
 msgstr ""
 
 #: admin.py:580 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
-msgstr "Importar"
+msgstr "导入"
 
-#: admin.py:749 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:752 templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
-msgstr "Exportar"
+msgstr "导出"
 
-#: admin.py:812
+#: admin.py:815
 msgid "You must select an export format."
-msgstr "Você tem que selecionar um formato de exportação."
+msgstr "您必须选择一个导出格式。"
 
-#: admin.py:835
+#: admin.py:838
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "Exportar %(verbose_name_plural)s selecionados"
+msgstr "导出选中的 %(verbose_name_plural)s"
 
-#: forms.py:11
+#: forms.py:12
 msgid "Resource"
 msgstr ""
 
-#: forms.py:29
+#: forms.py:41
 msgid "File to import"
-msgstr "Arquivo a ser importado"
+msgstr "导入文件"
 
-#: forms.py:32 forms.py:75 forms.py:100
+#: forms.py:44 forms.py:88 forms.py:114
 msgid "Format"
-msgstr "Formato"
+msgstr "格式"
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
-msgstr "Início"
+msgstr ""
 
 #: templates/admin/import_export/export.html:36
 #: templates/admin/import_export/import.html:73
 msgid "Submit"
-msgstr "Enviar"
+msgstr "提交"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
-msgstr ""
-"Ver abaixo uma prévia dos dados a serem importados. Se você esta satisfeito "
-"com os resultados, clique em 'Confirmar importação'"
+msgstr "以下是导入数据的预览。如果确认结果没有问题，可以点击 “确认导入”"
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
-msgstr "Confirmar importação"
+msgstr "确认导入"
 
 #: templates/admin/import_export/import.html:43
 msgid "This importer will import the following fields: "
-msgstr "Este importador vai importar os seguintes campos:"
+msgstr "此次将导入以下字段："
 
 #: templates/admin/import_export/import.html:83
 #: templates/admin/import_export/import.html:114
 msgid "Errors"
-msgstr "Erros"
+msgstr "错误"
 
 #: templates/admin/import_export/import.html:94
 msgid "Line number"
-msgstr "Número da linha"
+msgstr "行号"
 
 #: templates/admin/import_export/import.html:106
 msgid "Some rows failed to validate"
-msgstr "Algumas linhas não foram validadas"
+msgstr "某些行验数据证失败"
 
 #: templates/admin/import_export/import.html:108
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
-msgstr ""
-"Por favor corrigir os erros nos dados onde possível e recarregar os dados "
-"com o formato acima."
+msgstr "请使用上面的表单，纠正这些提示有错误的数据，并重新上传"
 
 #: templates/admin/import_export/import.html:113
 msgid "Row"
-msgstr "Linha"
+msgstr "行"
 
 #: templates/admin/import_export/import.html:140
 msgid "Non field specific"
-msgstr "Campo não é específico"
+msgstr "没有指定的字段"
 
 #: templates/admin/import_export/import.html:163
 msgid "Preview"
-msgstr "Prévia"
+msgstr "预览"
 
 #: templates/admin/import_export/import.html:178
 msgid "New"
-msgstr "Novo"
+msgstr "新增"
 
 #: templates/admin/import_export/import.html:180
 msgid "Skipped"
-msgstr "Não usados"
+msgstr "忽略"
 
 #: templates/admin/import_export/import.html:182
 msgid "Delete"
-msgstr "Remover"
+msgstr "删除"
 
 #: templates/admin/import_export/import.html:184
 msgid "Update"
-msgstr "Atualizar"
+msgstr "更新"
```

### Comparing `django-import-export-3.1.0/import_export/locale/ru/LC_MESSAGES/django.mo` & `django-import-export-3.2.0/import_export/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/locale/ru/LC_MESSAGES/django.po` & `django-import-export-3.2.0/import_export/locale/ru/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-21 18:05+0000\n"
+"POT-Creation-Date: 2023-04-12 18:40+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -35,37 +35,37 @@
 msgstr ""
 
 #: admin.py:580 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
 msgstr "Импорт"
 
-#: admin.py:749 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:752 templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
 msgstr "Экспорт"
 
-#: admin.py:812
+#: admin.py:815
 msgid "You must select an export format."
 msgstr "Необходимо выбрать формат экспорта"
 
-#: admin.py:835
+#: admin.py:838
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
 msgstr "Экспортировать выбранные %(verbose_name_plural)s"
 
-#: forms.py:11
+#: forms.py:12
 msgid "Resource"
 msgstr ""
 
-#: forms.py:29
+#: forms.py:41
 msgid "File to import"
 msgstr "Файл для импорта"
 
-#: forms.py:32 forms.py:75 forms.py:100
+#: forms.py:44 forms.py:88 forms.py:114
 msgid "Format"
 msgstr "Формат"
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
 msgstr "Главная"
```

### Comparing `django-import-export-3.1.0/import_export/locale/sk/LC_MESSAGES/django.po` & `django-import-export-3.2.0/import_export/locale/sk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Juraj Bubniak <contact@jbub.eu>, 2015.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-21 18:05+0000\n"
+"POT-Creation-Date: 2023-04-12 18:40+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -34,37 +34,37 @@
 msgstr ""
 
 #: admin.py:580 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
 msgstr "Importovať"
 
-#: admin.py:749 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:752 templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
 msgstr "Exportovať"
 
-#: admin.py:812
+#: admin.py:815
 msgid "You must select an export format."
 msgstr "Je potrebné vybrať formát exportu."
 
-#: admin.py:835
+#: admin.py:838
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
 msgstr "Exportovať vybrané %(verbose_name_plural)s"
 
-#: forms.py:11
+#: forms.py:12
 msgid "Resource"
 msgstr ""
 
-#: forms.py:29
+#: forms.py:41
 msgid "File to import"
 msgstr "Importovať súbor"
 
-#: forms.py:32 forms.py:75 forms.py:100
+#: forms.py:44 forms.py:88 forms.py:114
 msgid "Format"
 msgstr "Formát"
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
 msgstr "Domov"
```

### Comparing `django-import-export-3.1.0/import_export/locale/tr/LC_MESSAGES/django.mo` & `django-import-export-3.2.0/import_export/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/locale/tr/LC_MESSAGES/django.po` & `django-import-export-3.2.0/import_export/locale/tr/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-21 18:05+0000\n"
+"POT-Creation-Date: 2023-04-12 18:40+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -34,37 +34,37 @@
 msgstr ""
 
 #: admin.py:580 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
 msgstr "İçe aktar"
 
-#: admin.py:749 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:752 templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
 msgstr "Dışa aktar"
 
-#: admin.py:812
+#: admin.py:815
 msgid "You must select an export format."
 msgstr "Bir dosya biçimi seçmelisiniz"
 
-#: admin.py:835
+#: admin.py:838
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
 msgstr "Seçililenleri dışa aktar %(verbose_name_plural)s"
 
-#: forms.py:11
+#: forms.py:12
 msgid "Resource"
 msgstr ""
 
-#: forms.py:29
+#: forms.py:41
 msgid "File to import"
 msgstr "İçe alınacak dosya"
 
-#: forms.py:32 forms.py:75 forms.py:100
+#: forms.py:44 forms.py:88 forms.py:114
 msgid "Format"
 msgstr "Dosya biçimi"
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
 msgstr "Ana sayfa"
```

### Comparing `django-import-export-3.1.0/import_export/locale/zh_Hans/LC_MESSAGES/django.po` & `django-import-export-3.2.0/import_export/locale/pl/LC_MESSAGES/django.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,135 +1,138 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+# Ludwik Trammer <ludwik@gmail.com>, 2015.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-21 18:05+0000\n"
+"POT-Creation-Date: 2023-04-12 18:40+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: hao wang <173300430@qq.com>\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
+"|| n%100>=20) ? 1 : 2);\n"
 
 #: admin.py:214
 #, python-format
 msgid "%s through import_export"
-msgstr "%s 通过 django-import-export导入"
+msgstr "%s przez import_export"
 
 #: admin.py:220
 msgid "Import finished, with {} new and {} updated {}."
-msgstr "导入成功，新增{}条记录，更新{}条记录。"
+msgstr "Import zakończony, z {} nowymi i {} zaktualizowanymi {}."
 
 #: admin.py:456
 msgid ""
 "'{type(e).__name__}' encountered while trying to read file. Ensure you have "
 "chosen the correct format for the file. "
 msgstr ""
 
 #: admin.py:580 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
-msgstr "导入"
+msgstr "Import"
 
-#: admin.py:749 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:752 templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
-msgstr "导出"
+msgstr "Eksport"
 
-#: admin.py:812
+#: admin.py:815
 msgid "You must select an export format."
-msgstr "您必须选择一个导出格式。"
+msgstr "Musisz wybrać format eksportu."
 
-#: admin.py:835
+#: admin.py:838
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "导出选中的 %(verbose_name_plural)s"
+msgstr "Eksportuj wybrane %(verbose_name_plural)s"
 
-#: forms.py:11
+#: forms.py:12
 msgid "Resource"
 msgstr ""
 
-#: forms.py:29
+#: forms.py:41
 msgid "File to import"
-msgstr "导入文件"
+msgstr "Plik do importu"
 
-#: forms.py:32 forms.py:75 forms.py:100
+#: forms.py:44 forms.py:88 forms.py:114
 msgid "Format"
-msgstr "格式"
+msgstr "Format"
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
-msgstr ""
+msgstr "Powrót"
 
 #: templates/admin/import_export/export.html:36
 #: templates/admin/import_export/import.html:73
 msgid "Submit"
-msgstr "提交"
+msgstr "Wyślij"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
-msgstr "以下是导入数据的预览。如果确认结果没有问题，可以点击 “确认导入”"
+msgstr ""
+"Poniżej znajdują się przykładowe dane do zaimportowania. Jeśli "
+"satysfakcjonuje Cię wynik, kliknij 'Potwierdź import'"
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
-msgstr "确认导入"
+msgstr "Potwierdź import"
 
 #: templates/admin/import_export/import.html:43
 msgid "This importer will import the following fields: "
-msgstr "此次将导入以下字段："
+msgstr "Zostaną zaimportowane następujące pola: "
 
 #: templates/admin/import_export/import.html:83
 #: templates/admin/import_export/import.html:114
 msgid "Errors"
-msgstr "错误"
+msgstr "Błędy"
 
 #: templates/admin/import_export/import.html:94
 msgid "Line number"
-msgstr "行号"
+msgstr "Numer linii"
 
 #: templates/admin/import_export/import.html:106
 msgid "Some rows failed to validate"
-msgstr "某些行验数据证失败"
+msgstr ""
 
 #: templates/admin/import_export/import.html:108
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
-msgstr "请使用上面的表单，纠正这些提示有错误的数据，并重新上传"
+msgstr ""
 
 #: templates/admin/import_export/import.html:113
 msgid "Row"
-msgstr "行"
+msgstr ""
 
 #: templates/admin/import_export/import.html:140
 msgid "Non field specific"
-msgstr "没有指定的字段"
+msgstr ""
 
 #: templates/admin/import_export/import.html:163
 msgid "Preview"
-msgstr "预览"
+msgstr "Podgląd"
 
 #: templates/admin/import_export/import.html:178
 msgid "New"
-msgstr "新增"
+msgstr "Nowy"
 
 #: templates/admin/import_export/import.html:180
 msgid "Skipped"
-msgstr "忽略"
+msgstr "Pominięty"
 
 #: templates/admin/import_export/import.html:182
 msgid "Delete"
-msgstr "删除"
+msgstr "Usuń"
 
 #: templates/admin/import_export/import.html:184
 msgid "Update"
-msgstr "更新"
+msgstr "Zaktualizowany"
```

### Comparing `django-import-export-3.1.0/import_export/mixins.py` & `django-import-export-3.2.0/import_export/mixins.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import logging
 import warnings
 
 from django.conf import settings
 from django.http import HttpResponse
 from django.utils.timezone import now
 from django.views.generic.edit import FormView
 
 from .formats import base_formats
 from .forms import ExportForm
 from .resources import modelresource_factory
 from .signals import post_export
 
+logger = logging.getLogger(__name__)
+
 
 class BaseImportExportMixin:
     formats = base_formats.DEFAULT_FORMATS
     resource_class = None
     resource_classes = []
 
     def check_resource_classes(self, resource_classes):
@@ -87,19 +90,41 @@
         resource_index = self.get_resource_index(form)
         return self.get_import_resource_classes()[resource_index]
 
 
 class BaseExportMixin(BaseImportExportMixin):
     model = None
     escape_exported_data = False
+    escape_html = False
+    escape_formulae = False
 
     @property
     def should_escape_output(self):
+        if hasattr(settings, 'IMPORT_EXPORT_ESCAPE_OUTPUT_ON_EXPORT'):
+            warnings.warn(
+                "IMPORT_EXPORT_ESCAPE_OUTPUT_ON_EXPORT will be deprecated in a future release. "
+                "Refer to docs for new attributes.",
+                DeprecationWarning,
+            )
         return getattr(settings, 'IMPORT_EXPORT_ESCAPE_OUTPUT_ON_EXPORT', self.escape_exported_data)
 
+    @property
+    def should_escape_html(self):
+        v = getattr(settings, 'IMPORT_EXPORT_ESCAPE_HTML_ON_EXPORT', self.escape_html)
+        if v is True:
+            logger.debug('IMPORT_EXPORT_ESCAPE_HTML_ON_EXPORT is enabled')
+        return v
+
+    @property
+    def should_escape_formulae(self):
+        v = getattr(settings, 'IMPORT_EXPORT_ESCAPE_FORMULAE_ON_EXPORT', self.escape_formulae)
+        if v is True:
+            logger.debug('IMPORT_EXPORT_ESCAPE_FORMULAE_ON_EXPORT is enabled')
+        return v
+
     def get_export_formats(self):
         """
         Returns available export formats.
         """
         return [f for f in self.formats if f().can_export()]
 
     def get_export_resource_classes(self):
@@ -125,15 +150,15 @@
     def get_export_resource_kwargs(self, request, *args, **kwargs):
         return self.get_resource_kwargs(request, *args, **kwargs)
 
     def get_data_for_export(self, request, queryset, *args, **kwargs):
         export_form = kwargs.pop('export_form', None)
         return self.choose_export_resource_class(export_form)\
             (**self.get_export_resource_kwargs(request, *args, **kwargs))\
-            .export(queryset, *args, **kwargs)
+            .export(*args, queryset=queryset, **kwargs)
 
     def get_export_filename(self, file_format):
         date_str = now().strftime('%Y-%m-%d')
         filename = "%s-%s.%s" % (self.model.__name__,
                                  date_str,
                                  file_format.get_extension())
         return filename
```

### Comparing `django-import-export-3.1.0/import_export/resources.py` & `django-import-export-3.2.0/import_export/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -623,15 +623,15 @@
             if isinstance(field.widget, widgets.ManyToManyWidget):
                 # #1437 - handle m2m field not present in import file
                 if field.column_name not in row.keys():
                     continue
                 # m2m instance values are taken from the 'row' because they
                 # have not been written to the 'instance' at this point
                 instance_values = list(field.clean(row))
-                original_values = list(field.get_value(original).all())
+                original_values = list() if original.pk is None else list(field.get_value(original).all())
                 if len(instance_values) != len(original_values):
                     return False
 
                 if sorted(v.pk for v in instance_values) != sorted(v.pk for v in original_values):
                     return False
             else:
                 if field.get_value(instance) != field.get_value(original):
@@ -962,18 +962,30 @@
                 queryset = queryset.order_by('pk')
             paginator = Paginator(queryset, self.get_chunk_size())
             for index in range(paginator.num_pages):
                 yield from paginator.get_page(index + 1)
         else:
             yield from queryset.iterator(chunk_size=self.get_chunk_size())
 
-    def export(self, queryset=None, *args, **kwargs):
+    def export(self, *args, queryset=None, **kwargs):
         """
         Exports a resource.
+        :returns: Dataset object.
         """
+        if len(args) == 1 and (isinstance(args[0], QuerySet) or isinstance(args[0], list)):
+            # issue 1565: definition of export() was incorrect
+            # if queryset is being passed, it must be as the first arg or named parameter
+            # this logic is included for backwards compatibility:
+            # if the method is being called without a named parameter, add a warning
+            # this check should be removed in a future release
+            warnings.warn(
+                "'queryset' must be supplied as a named parameter",
+                category=DeprecationWarning
+            )
+            queryset = args[0]
 
         self.before_export(queryset, *args, **kwargs)
 
         if queryset is None:
             queryset = self.get_queryset()
         headers = self.get_export_headers()
         data = tablib.Dataset(headers=headers)
```

### Comparing `django-import-export-3.1.0/import_export/results.py` & `django-import-export-3.2.0/import_export/results.py`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/static/import_export/action_formats.js` & `django-import-export-3.2.0/import_export/static/import_export/action_formats.js`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/static/import_export/guess_format.js` & `django-import-export-3.2.0/import_export/static/import_export/guess_format.js`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/static/import_export/import.css` & `django-import-export-3.2.0/import_export/static/import_export/import.css`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/templates/admin/import_export/base.html` & `django-import-export-3.2.0/import_export/templates/admin/import_export/base.html`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/templates/admin/import_export/export.html` & `django-import-export-3.2.0/import_export/templates/admin/import_export/export.html`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/templates/admin/import_export/import.html` & `django-import-export-3.2.0/import_export/templates/admin/import_export/import.html`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/tmp_storages.py` & `django-import-export-3.2.0/import_export/tmp_storages.py`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/utils.py` & `django-import-export-3.2.0/import_export/utils.py`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/import_export/widgets.py` & `django-import-export-3.2.0/import_export/widgets.py`

 * *Files identical despite different names*

### Comparing `django-import-export-3.1.0/setup.py` & `django-import-export-3.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,30 +22,30 @@
     'Programming Language :: Python :: 3 :: Only',
     'Topic :: Software Development',
 ]
 
 install_requires = [
     'diff-match-patch',
     'Django>=3.2',
-    'tablib[html,ods,xls,xlsx,yaml]>=3.2.1',
+    'tablib[html,ods,xls,xlsx,yaml]>=3.4.0',
 ]
 
 
 with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as f:
     readme = f.read()
 
 
 setup(
     name="django-import-export",
     description="Django application and library for importing and exporting"
                 " data with included admin integration.",
     long_description=readme,
     version=VERSION,
-    author="Informatika Mihelac",
-    author_email="bmihelac@mihelac.org",
+    author="Bojan Mihelač",
+    author_email="djangoimportexport@gmail.com",
     license='BSD License',
     platforms=['OS Independent'],
     url="https://github.com/django-import-export/django-import-export",
     project_urls={
         "Documentation": "https://django-import-export.readthedocs.io/en/stable/",
         "Changelog": "https://django-import-export.readthedocs.io/en/stable/changelog.html",
     },
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

