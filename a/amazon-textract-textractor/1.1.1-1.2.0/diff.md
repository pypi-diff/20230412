# Comparing `tmp/amazon-textract-textractor-1.1.1.tar.gz` & `tmp/amazon-textract-textractor-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-textract-textractor-1.1.1.tar", last modified: Thu Mar  2 20:19:21 2023, max compression
+gzip compressed data, was "amazon-textract-textractor-1.2.0.tar", last modified: Wed Apr 12 15:25:42 2023, max compression
```

## Comparing `amazon-textract-textractor-1.1.1.tar` & `amazon-textract-textractor-1.2.0.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:19:21.418984 amazon-textract-textractor-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-03-02 20:19:21.418984 amazon-textract-textractor-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:19:21.414984 amazon-textract-textractor-1.1.1/amazon_textract_textractor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-03-02 20:19:21.000000 amazon-textract-textractor-1.1.1/amazon_textract_textractor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-02 20:19:21.000000 amazon-textract-textractor-1.1.1/amazon_textract_textractor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 20:19:21.000000 amazon-textract-textractor-1.1.1/amazon_textract_textractor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-02 20:19:21.000000 amazon-textract-textractor-1.1.1/amazon_textract_textractor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-02 20:19:21.000000 amazon-textract-textractor-1.1.1/amazon_textract_textractor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-02 20:19:21.000000 amazon-textract-textractor-1.1.1/amazon_textract_textractor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:19:21.414984 amazon-textract-textractor-1.1.1/extras/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/extras/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/extras/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/extras/pandas.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/extras/pdf.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/extras/torch.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-02 20:19:21.418984 amazon-textract-textractor-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:19:21.414984 amazon-textract-textractor-1.1.1/textractor/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:19:21.414984 amazon-textract-textractor-1.1.1/textractor/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:19:21.414984 amazon-textract-textractor-1.1.1/textractor/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/data/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:19:21.414984 amazon-textract-textractor-1.1.1/textractor/entities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/entities/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    30720 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/entities/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/entities/document_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/entities/expense_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/entities/expense_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/entities/identity_document.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/entities/identity_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/entities/key_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/entities/lazy_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/entities/line.py
--rw-r--r--   0 runner    (1001) docker     (123)    34524 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/entities/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/entities/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/entities/query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/entities/selection_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/entities/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    21708 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/entities/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/entities/table_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/entities/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/entities/word.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:19:21.414984 amazon-textract-textractor-1.1.1/textractor/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32593 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/parsers/response_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    37674 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/textractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:19:21.414984 amazon-textract-textractor-1.1.1/textractor/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/utils/geometry_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/utils/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/utils/search_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:19:21.414984 amazon-textract-textractor-1.1.1/textractor/validate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/validate/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:19:21.418984 amazon-textract-textractor-1.1.1/textractor/visualizers/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/visualizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   367112 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/visualizers/arial.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    39992 2023-03-02 20:19:12.000000 amazon-textract-textractor-1.1.1/textractor/visualizers/entitylist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.682259 amazon-textract-textractor-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-12 15:25:25.000000 amazon-textract-textractor-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-12 15:25:25.000000 amazon-textract-textractor-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-12 15:25:25.000000 amazon-textract-textractor-1.2.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-04-12 15:25:42.682259 amazon-textract-textractor-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-04-12 15:25:25.000000 amazon-textract-textractor-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.670259 amazon-textract-textractor-1.2.0/amazon_textract_textractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-04-12 15:25:42.000000 amazon-textract-textractor-1.2.0/amazon_textract_textractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-12 15:25:42.000000 amazon-textract-textractor-1.2.0/amazon_textract_textractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:25:42.000000 amazon-textract-textractor-1.2.0/amazon_textract_textractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 15:25:42.000000 amazon-textract-textractor-1.2.0/amazon_textract_textractor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-12 15:25:42.000000 amazon-textract-textractor-1.2.0/amazon_textract_textractor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 15:25:42.000000 amazon-textract-textractor-1.2.0/amazon_textract_textractor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.674259 amazon-textract-textractor-1.2.0/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/extras/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/extras/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/extras/pandas.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/extras/pdf.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/extras/torch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-12 15:25:42.682259 amazon-textract-textractor-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.674259 amazon-textract-textractor-1.2.0/textractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.674259 amazon-textract-textractor-1.2.0/textractor/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15145 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.674259 amazon-textract-textractor-1.2.0/textractor/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/data/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.678259 amazon-textract-textractor-1.2.0/textractor/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30720 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/document_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/expense_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/expense_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/identity_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/identity_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/key_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/lazy_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34524 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/selection_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23273 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/table_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/table_footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/table_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/word.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.678259 amazon-textract-textractor-1.2.0/textractor/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35493 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/parsers/response_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37612 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/textractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.682259 amazon-textract-textractor-1.2.0/textractor/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/utils/geometry_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/utils/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/utils/search_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.682259 amazon-textract-textractor-1.2.0/textractor/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/validate/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.682259 amazon-textract-textractor-1.2.0/textractor/visualizers/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/visualizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   367112 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/visualizers/arial.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    42343 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/visualizers/entitylist.py
```

### Comparing `amazon-textract-textractor-1.1.1/LICENSE` & `amazon-textract-textractor-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/PKG-INFO` & `amazon-textract-textractor-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-textract-textractor
-Version: 1.1.1
+Version: 1.2.0
 Summary: A package to use AWS Textract services.
 Home-page: https://github.com/aws-samples/amazon-textract-textractor
 License: Apache 2.0
 Keywords: amazon textract aws ocr document
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `amazon-textract-textractor-1.1.1/README.md` & `amazon-textract-textractor-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/amazon_textract_textractor.egg-info/PKG-INFO` & `amazon-textract-textractor-1.2.0/amazon_textract_textractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-textract-textractor
-Version: 1.1.1
+Version: 1.2.0
 Summary: A package to use AWS Textract services.
 Home-page: https://github.com/aws-samples/amazon-textract-textractor
 License: Apache 2.0
 Keywords: amazon textract aws ocr document
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `amazon-textract-textractor-1.1.1/amazon_textract_textractor.egg-info/SOURCES.txt` & `amazon-textract-textractor-1.2.0/amazon_textract_textractor.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 textractor/entities/page.py
 textractor/entities/query.py
 textractor/entities/query_result.py
 textractor/entities/selection_element.py
 textractor/entities/signature.py
 textractor/entities/table.py
 textractor/entities/table_cell.py
+textractor/entities/table_footer.py
+textractor/entities/table_title.py
 textractor/entities/value.py
 textractor/entities/word.py
 textractor/parsers/__init__.py
 textractor/parsers/response_parser.py
 textractor/utils/__init__.py
 textractor/utils/geometry_util.py
 textractor/utils/s3_utils.py
```

### Comparing `amazon-textract-textractor-1.1.1/amazon_textract_textractor.egg-info/requires.txt` & `amazon-textract-textractor-1.2.0/amazon_textract_textractor.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Pillow
 XlsxWriter==3.0.*
 amazon-textract-caller<0.1.0,>=0.0.27
+amazon-textract-pipeline-pagedimensions
 amazon-textract-response-parser<0.2.0,>=0.1.37
 editdistance==0.6.2
 jsonschema
 tabulate==0.9.*
 
 [dev]
 jsonschema
```

### Comparing `amazon-textract-textractor-1.1.1/setup.py` & `amazon-textract-textractor-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         requirements = [line for line in f.readlines()]
     return requirements
 
 
 setup(
     # include data files
     name="amazon-textract-textractor",
-    version="1.1.1",
+    version="1.2.0",
     license="Apache 2.0",
     description="A package to use AWS Textract services.",
     url="https://github.com/aws-samples/amazon-textract-textractor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `amazon-textract-textractor-1.1.1/textractor/cli/cli.py` & `amazon-textract-textractor-1.2.0/textractor/cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,28 +308,31 @@
                 "--s3-upload-path is required if file_source is not an S3 path"
             )
         if args.subcommand == "start-document-text-detection":
             out = extractor.start_document_text_detection(
                 args.file_source,
                 s3_output_path=args.s3_output_path,
                 s3_upload_path=args.s3_upload_path,
+                save_image=False,
             )
         elif args.subcommand == "start-document-analysis":
             out = extractor.start_document_analysis(
                 args.file_source,
                 features=[TextractFeatures[feat] for feat in args.features],
                 queries=args.queries,
                 s3_output_path=args.s3_output_path,
                 s3_upload_path=args.s3_upload_path,
+                save_image=False,
             )
         elif args.subcommand == "start-expense-analysis":
             out = extractor.start_expense_analysis(
                 args.file_source,
                 s3_output_path=args.s3_output_path,
                 s3_upload_path=args.s3_upload_path,
+                save_image=False,
             )
         print(out.job_id)
     # SYNC
     else:
         if args.subcommand == "detect-document-text":
             out = extractor.detect_document_text(
                 args.file_source,
```

### Comparing `amazon-textract-textractor-1.1.1/textractor/data/constants.py` & `amazon-textract-textractor-1.2.0/textractor/data/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,21 @@
 from textractor.exceptions import InputError
 
 WORD = "WORD"
 LINE = "LINE"
 KEY_VALUE_SET = "KEY_VALUE_SET"
 SELECTION_ELEMENT = "SELECTION_ELEMENT"
 TABLE = "TABLE"
+TABLE_TITLE = "TABLE_TITLE"
+TABLE_FOOTER = "TABLE_FOOTER"
+TABLE_SUMMARY = "TABLE_SUMMARY"
+TABLE_SECTION_TITLE = "TABLE_SECTION_TITLE"
+TABLE_COLUMN_HEADER = "COLUMN_HEADER"
+TABLE_STRUCTURED = "STRUCTURED"
+TABLE_SEMI_STRUCTURED = "SEMI_STRUCTURED"
 CELL = "CELL"
 PAGE = "PAGE"
 MERGED_CELL = "MERGED_CELL"
 QUERY = "QUERY"
 QUERY_RESULT = "QUERY_RESULT"
 SIGNATURE = "SIGNATURE"
 
@@ -26,14 +33,20 @@
 IS_FOOTER_CELL = "isFooterCell"
 IS_MERGED_CELL = "isMergedCell"
 
 # Text Types
 HANDWRITING = "HANDWRITING"
 PRINTED = "PRINTED"
 
+class TableTypes(Enum):
+    """Types of tables recognized by Textract APIs."""
+
+    UNKNOWN = 0
+    STRUCTURED = 1
+    SEMI_STRUCTURED = 2
 
 class Direction(Enum):
     """Directions available for search using DirectionalFinder"""
 
     ABOVE = 0
     BELOW = 1
     RIGHT = 2
```

### Comparing `amazon-textract-textractor-1.1.1/textractor/entities/bbox.py` & `amazon-textract-textractor-1.2.0/textractor/entities/bbox.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/entities/document.py` & `amazon-textract-textractor-1.2.0/textractor/entities/document.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/entities/document_entity.py` & `amazon-textract-textractor-1.2.0/textractor/entities/document_entity.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/entities/expense_document.py` & `amazon-textract-textractor-1.2.0/textractor/entities/expense_document.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/entities/expense_field.py` & `amazon-textract-textractor-1.2.0/textractor/entities/expense_field.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/entities/identity_document.py` & `amazon-textract-textractor-1.2.0/textractor/entities/identity_document.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/entities/key_value.py` & `amazon-textract-textractor-1.2.0/textractor/entities/key_value.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/entities/lazy_document.py` & `amazon-textract-textractor-1.2.0/textractor/entities/lazy_document.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/entities/line.py` & `amazon-textract-textractor-1.2.0/textractor/entities/line.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/entities/page.py` & `amazon-textract-textractor-1.2.0/textractor/entities/page.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/entities/query.py` & `amazon-textract-textractor-1.2.0/textractor/entities/query.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/entities/query_result.py` & `amazon-textract-textractor-1.2.0/textractor/entities/query_result.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/entities/selection_element.py` & `amazon-textract-textractor-1.2.0/textractor/entities/selection_element.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/entities/signature.py` & `amazon-textract-textractor-1.2.0/textractor/entities/signature.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/entities/table.py` & `amazon-textract-textractor-1.2.0/textractor/entities/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 
 from textractor.exceptions import InputError
 from textractor.entities.bbox import BoundingBox
 from textractor.entities.table_cell import TableCell
 from textractor.visualizers.entitylist import EntityList
 from textractor.entities.document_entity import DocumentEntity
 from textractor.entities.selection_element import SelectionElement
+from textractor.entities.table_title import TableTitle
+from textractor.entities.table_footer import TableFooter
 from textractor.utils.geometry_util import get_indices
-from textractor.data.constants import SimilarityMetric, TextTypes, CellTypes
+from textractor.data.constants import SimilarityMetric, TextTypes, CellTypes, TableTypes
 from textractor.data.constants import (
     IS_COLUMN_HEAD,
     IS_MERGED_CELL,
 )
 from textractor.utils.search_utils import SearchUtils, get_metadata_attr_name
 
 
@@ -37,14 +39,17 @@
     :param bbox:                Bounding box of the table.
     """
 
     def __init__(self, entity_id, bbox: BoundingBox):
         super().__init__(entity_id, bbox)
         self.table_cells: List[TableCell] = []
         self.column_headers: Dict[str, List[TableCell]] = {}
+        self._title: TableTitle = None
+        self._footers: TableFooter = []
+        self._table_type: TableTypes = TableTypes.UNKNOWN
         self._page = None
         self._page_id = None
 
     @property
     def words(self):
         """
         Returns all the :class:`Word` objects present in the :class:`Table`.
@@ -77,14 +82,74 @@
         :param page_num: Page number where the Table entity exists.
         :type page_num: int
         """
 
         self._page = page_num
 
     @property
+    def table_type(self):
+        """
+        :return: Returns the table type.
+        :rtype: TableTypes
+        """
+
+        return self._table_type
+
+    @table_type.setter
+    def table_type(self, table_type: TableTypes):
+        """
+        Sets the table type attribute of the Table entity.
+
+        :param title: Type of the Table entity.
+        :type title: TableTypes
+        """
+
+        self._table_type = table_type
+
+    @property
+    def title(self):
+        """
+        :return: Returns the table title.
+        :rtype: TableTitle
+        """
+
+        return self._title
+
+    @title.setter
+    def title(self, title: TableTitle):
+        """
+        Sets the table title attribute of the Table entity.
+
+        :param title: Title of the Table entity.
+        :type title: TableTitle
+        """
+
+        self._title = title
+
+    @property
+    def footers(self):
+        """
+        :return: Returns the table footers.
+        :rtype: List[TableFooter]
+        """
+
+        return self._footers
+
+    @footers.setter
+    def footers(self, footers: List[TableFooter]):
+        """
+        Sets the footers attribute of the Table entity.
+
+        :param footers: Footers of the Table entity.
+        :type footers: List[TableFooter]
+        """
+
+        self._footers = footers
+
+    @property
     def page_id(self) -> str:
         """
         :return: Returns the Page ID attribute of the page which the entity belongs to.
         :rtype: str
         """
 
         return self._page_id
```

### Comparing `amazon-textract-textractor-1.1.1/textractor/entities/table_cell.py` & `amazon-textract-textractor-1.2.0/textractor/entities/table_cell.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,51 +34,80 @@
     To create a new TableCell object we need the following:
 
     :param entity_id: Unique id of the TableCell object
     :param bbox: Bounding box of the entity
     :param row_index: Row index of position of cell within the table
     :param col_index: Column index of position of cell within the table
     :param row_span: How many merged cells does the cell spans horizontally (1 means no merged cells)
-    :param col_span: How mant merged cells does the cell spand vertically (1 means no merged cells)
+    :param col_span: How many merged cells does the cell spand vertically (1 means no merged cells)
     :param confidence: Confidence out of 100 with which the Cell was detected.
+    :param is_column_header: Indicates if the cell is a column header
+    :param is_title: Indicates if the cell is a table title
+    :param is_footer: Indicates if the cell is a table footer
+    :param is_summary: Indicates if the cell is a summary cell
+    :param is_section_title: Indicates if the cell is a section title
     """
 
     def __init__(
         self,
         entity_id: str,
         bbox: BoundingBox,
         row_index: int,
         col_index: int,
         row_span: int,
         col_span: int,
         confidence: float = 0,
-        is_column_header: bool = False
+        is_column_header: bool = False,
+        is_title: bool = False,
+        is_footer: bool = False,
+        is_summary: bool = False,
+        is_section_title: bool = False
     ):
 
         super().__init__(entity_id, bbox)
         self._row_index: int = int(row_index)
         self._col_index: int = int(col_index)
         self._row_span: int = int(row_span)
         self._col_span: int = int(col_span)
         self._words: List[Word] = []
         self.confidence = confidence / 100
         self._page = None
         self._page_id = None
         self._is_column_header = is_column_header
+        self._is_title = is_title
+        self._is_footer = is_footer
+        self._is_summary = is_summary
+        self._is_section_title = is_section_title
         # this gets populated when cells are added to a table using the `add_cells` method
         # or when cells are attributed to a table with table.cells = [TableCell]
         self._parent_table_id = None
         self.parent_cell_id = None
         self.siblings: List[TableCell] = []
 
     @property
     def is_column_header(self):
         return self._is_column_header
 
     @property
+    def is_title(self):
+        return self._is_title
+    
+    @property
+    def is_footer(self):
+        return self._is_footer
+    
+    @property
+    def is_summary(self):
+        return self._is_summary
+    
+    @property
+    def is_section_title(self):
+        return self._is_section_title
+
+    @property
     def page(self):
         """
         :return: Returns the page number of the page the :class:`TableCell` entity is present in.
         :rtype: int
         """
         return self._page
```

### Comparing `amazon-textract-textractor-1.1.1/textractor/entities/value.py` & `amazon-textract-textractor-1.2.0/textractor/entities/value.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/entities/word.py` & `amazon-textract-textractor-1.2.0/textractor/entities/word.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/exceptions.py` & `amazon-textract-textractor-1.2.0/textractor/exceptions.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/parsers/response_parser.py` & `amazon-textract-textractor-1.2.0/textractor/parsers/response_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,25 +20,33 @@
 from textractor.entities.line import Line
 from textractor.entities.value import Value
 from textractor.entities.table import Table
 from textractor.entities.bbox import BoundingBox
 from textractor.entities.document import Document
 from textractor.entities.key_value import KeyValue
 from textractor.entities.table_cell import TableCell
+from textractor.entities.table_title import TableTitle
+from textractor.entities.table_footer import TableFooter
 from textractor.entities.query import Query
 from textractor.validate.validation import validate_entity_schema
 from textractor.entities.document_entity import DocumentEntity
 from textractor.entities.selection_element import SelectionElement
 from textractor.data.constants import (
+    TABLE_FOOTER,
+    TABLE_TITLE,
+    COLUMN_HEADER,
+    TABLE_SUMMARY,
+    TABLE_SECTION_TITLE,
+    TABLE_STRUCTURED,
+    TABLE_SEMI_STRUCTURED,
     SelectionStatus,
     TextTypes,
+    TableTypes,
     HANDWRITING,
     PRINTED,
-)
-from textractor.data.constants import (
     WORD,
     LINE,
     KEY_VALUE_SET,
     CELL,
     TABLE,
     SELECTION_ELEMENT,
     PAGE,
@@ -585,15 +593,19 @@
                 elem["Geometry"]["BoundingBox"], spatial_object=page
             ),
             row_index=elem["RowIndex"],
             col_index=elem["ColumnIndex"],
             row_span=elem["RowSpan"],
             col_span=elem["ColumnSpan"],
             confidence=elem["Confidence"],
-            is_column_header="COLUMN_HEADER" in elem.get("EntityTypes", [])
+            is_column_header=COLUMN_HEADER in elem.get("EntityTypes", []),
+            is_title=TABLE_TITLE in elem.get("EntityTypes", []),
+            is_footer=TABLE_FOOTER in elem.get("EntityTypes", []),
+            is_summary=TABLE_SUMMARY in elem.get("EntityTypes", []),
+            is_section_title=TABLE_SECTION_TITLE in elem.get("EntityTypes", []),
         )
         table_cells[elem_id].raw_object = elem
 
     for cell in table_cells.values():
         cell.page = page.page_num
         cell.page_id = page.id
     return table_cells, all_table_cells_info
@@ -636,14 +648,22 @@
     for val in page_tables:
         tables[val["Id"]] = Table(
             entity_id=val["Id"],
             bbox=BoundingBox.from_normalized_dict(
                 val["Geometry"]["BoundingBox"], spatial_object=page
             ),
         )
+        # Setting table type based on the entity types present in the table
+        if TABLE_STRUCTURED in val.get("EntityTypes", []):
+            tables[val["Id"]].table_type = TableTypes.STRUCTURED
+        elif TABLE_SEMI_STRUCTURED in val.get("EntityTypes", []):
+            tables[val["Id"]].table_type = TableTypes.SEMI_STRUCTURED
+        else:
+            tables[val["Id"]].table_type = TableTypes.UNKNOWN
+        # Setting raw JSON in the resulting object
         tables[val["Id"]].raw_object = val
 
     # Create Table Cells
     table_cells, all_table_cells_info = _create_table_cell_objects(
         page_tables, id_entity_map, id_json_map, page
     )
 
@@ -692,23 +712,66 @@
         for child_id in child_cells:
             if child_id in table_cells.keys():
                 table_cells[child_id].parent_cell_id = merge_id
                 table_cells[child_id].siblings = [
                     table_cells[cid] for cid in child_cells
                 ]  # CHECK IF IDS ARE BETTER THAN INSTANCES
 
+    # Create table title (if exists)
+    for table in page_tables:
+        children = _get_relationship_ids(table, relationship="TABLE_TITLE")
+        for child_id in children:
+            tables[table["Id"]].title = TableTitle(
+                entity_id=child_id,
+                bbox=BoundingBox.from_normalized_dict(id_json_map[child_id]["Geometry"]["BoundingBox"])
+            )
+            children = _get_relationship_ids(id_json_map[child_id], relationship="CHILD")
+            tables[table["Id"]].title.words = _create_word_objects(
+                [child_id for child_id in children if id_entity_map[child_id] == WORD],
+                id_json_map,
+                page
+            )
+
+    # Create table footer (if exists)
+    for table in page_tables:
+        children = _get_relationship_ids(table, relationship="TABLE_FOOTER")
+        for child_id in children:
+            tables[table["Id"]].footers.append(
+                TableFooter(
+                    entity_id=child_id,
+                    bbox=BoundingBox.from_normalized_dict(id_json_map[child_id]["Geometry"]["BoundingBox"])
+                )
+            )
+            children = _get_relationship_ids(id_json_map[child_id], relationship="CHILD")
+            tables[table["Id"]].footers[-1].words = _create_word_objects(
+                [child_id for child_id in children if id_entity_map[child_id] == WORD],
+                id_json_map,
+                page
+            )
+
     # Associate Children with Tables
     for table in page_tables:
         children = _get_relationship_ids(table, relationship="CHILD")
         children_cells = []
         for child_id in children:
             children_cells.append(table_cells[child_id])
+            if table_cells[child_id].is_title:
+                tables[table["Id"]].title.is_floating = False
+        # FIXME: This will be slow and there should be a better way to do it.
+        words = set([w.id for child_id in children for w in table_cells[child_id].words])
+        for footer in tables[table["Id"]].footers:
+            for w in footer.words:
+                if w.id in words:
+                    footer.is_floating = False
+                    break
 
         tables[table["Id"]].add_cells(children_cells)
 
+    
+
     tables = list(tables.values())
     for table in tables:
         table.page = page.page_num
         table.page_id = page.id
     return tables, table_words
```

### Comparing `amazon-textract-textractor-1.1.1/textractor/textractor.py` & `amazon-textract-textractor-1.2.0/textractor/textractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,32 +438,31 @@
         document = response_parser.parse(response)
         document.response = response
         if save_image:
             for page in document.pages:
                 page.image = images[document.pages.index(page)]
         return document
 
-    # FIXME: This should not be synchronous
     def start_document_analysis(
         self,
         file_source: Union[str, bytes, Image.Image],
         features,
         s3_output_path: str = "",
         s3_upload_path: str = "",
         queries: Union[QueriesConfig, List[Query], List[str]] = None,
         client_request_token: str = "",
         job_tag: str = "",
         save_image: bool = True,
     ) -> LazyDocument:
         """
         Make a call to the ASYNC StartDocumentAnalysis API, implicitly parses the response and produces a :class:`Document` object.
-        This function is ideal for multipage PDFs or list of images.
+        This function is ideal for multipage PDFs or an image.
 
-        :param file_source: Path to a file stored locally, on an S3 bucket or list of PIL Images
-        :type file_source: str or List[PIL.Image], required
+        :param file_source: Path to a file stored locally, on an S3 bucket or a PIL Image
+        :type file_source: Union[str, bytes, Image.Image], required
         :param features: List of TextractFeatures to be extracted from the Document by the TextractAPI
         :type features: list, required
         :param s3_output_path: Path to store the output on the S3 bucket (passed as param to Textractor).
         :type s3_output_path: str
         :param s3_upload_path: If given, will automatically upload the document to the given S3 prefix before calling Textract. Files are uploaded
                                under a uuid. If not given the data is expected to be already in s3
         :type s3_upload_path: str, optional
@@ -720,17 +719,17 @@
         s3_output_path: str = "",
         s3_upload_path: str = "",
         client_request_token: str = "",
         job_tag: str = "",
         save_image: bool = True,
     ) -> LazyDocument:
         """Make a call to the ASYNC StartExpenseAnalysis API, implicitly parses the response and produces a :class:`Document` object.
-        This function is ideal for multipage PDFs or list of images.
+        This function is ideal for multipage PDFs or an image.
 
-        :param file_source: Path to a file stored locally, on an S3 bucket or list of PIL Images
+        :param file_source: Path to a file stored locally, on an S3 bucket or a PIL Image
         :type file_source: Union[str, bytes, Image.Image]
         :param s3_output_path: Path to store the output on the S3 bucket (passed as param to Textractor).
         :type s3_output_path: str
         :param s3_upload_path: If given, will automatically upload the document to the given S3 prefix before calling Textract. Files are uploaded
                                under a uuid. If not given the data is expected to be already in s3
         :type s3_upload_path: str, optional
         :param client_request_token: The idempotent token that's used to identify the start request. If you use the same. token
```

### Comparing `amazon-textract-textractor-1.1.1/textractor/utils/geometry_util.py` & `amazon-textract-textractor-1.2.0/textractor/utils/geometry_util.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/utils/s3_utils.py` & `amazon-textract-textractor-1.2.0/textractor/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/utils/search_utils.py` & `amazon-textract-textractor-1.2.0/textractor/utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/validate/validation.py` & `amazon-textract-textractor-1.2.0/textractor/validate/validation.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/visualizers/arial.ttf` & `amazon-textract-textractor-1.2.0/textractor/visualizers/arial.ttf`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.1.1/textractor/visualizers/entitylist.py` & `amazon-textract-textractor-1.2.0/textractor/visualizers/entitylist.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,15 @@
             entities_pagewise[obj.page].append(obj)
             try:
                 if with_words:
                     entities_pagewise[obj.page].extend(obj.words)
             # FIXME: There should be a way to recurse through all entities
             except AttributeError:
                 pass
+
         for page in list(entities_pagewise.keys()):
             # Deduplication
             entities_pagewise[page] = list(set(entities_pagewise[page]))
 
         for page in entities_pagewise.keys():
             visualized_images[page] = _draw_bbox(
                 entities_pagewise[page],
@@ -600,22 +601,48 @@
     image = entities[0].bbox.spatial_object.image
     image = image.convert("RGBA")
     overlay = Image.new("RGBA", image.size, (255, 255, 255, 0))
     drw = ImageDraw.Draw(overlay, "RGBA")
 
     text_locations = {}
 
-    # First drawing, bounding boxes
+    # First drawing tables
     for entity in entities:
         width, height = image.size
         if entity.__class__.__name__ == "Table":
             overlayer_data = _get_overlayer_data(entity, width, height)
             drw.rectangle(
                 xy=overlayer_data["coords"], outline=overlayer_data["color"], width=2
             )
+            if entity.title:
+                drw.rectangle(
+                    (
+                        int(entity.title.bbox.x * width),
+                        int(entity.title.bbox.y * height),
+                        int((entity.title.bbox.x + entity.title.bbox.width) * width),
+                        int((entity.title.bbox.y + entity.title.bbox.height) * height),
+                    ),
+                    outline=overlayer_data["color"],
+                    fill=ImageColor.getrgb("red") + (120,),
+                    width=2,
+                )
+
+            for footer in entity.footers:
+                drw.rectangle(
+                    (
+                        int(footer.bbox.x * width),
+                        int(footer.bbox.y * height),
+                        int((footer.bbox.x + footer.bbox.width) * width),
+                        int((footer.bbox.y + footer.bbox.height) * height),
+                    ),
+                    outline=overlayer_data["color"],
+                    fill=ImageColor.getrgb("cyan") + (120,),
+                    width=2,
+                )
+
             processed_cells = set()
             for cell in entity.table_cells:
                 if cell.id in processed_cells:
                     continue
                 if cell.siblings:
                     for c in cell.siblings:
                         processed_cells.add(c.id)
@@ -646,14 +673,22 @@
                         cell.bbox.x + cell.bbox.width,
                         cell.bbox.y + cell.bbox.height,
                     )
 
                 fill_color=None
                 if cell.is_column_header:
                     fill_color = ImageColor.getrgb("blue") + (120,)
+                if cell.is_title:
+                    fill_color = ImageColor.getrgb("red") + (120,)
+                if cell.is_footer:
+                    fill_color = ImageColor.getrgb("cyan") + (120,)
+                if cell.is_summary:
+                    fill_color = ImageColor.getrgb("yellow") + (120,)
+                if cell.is_section_title:
+                    fill_color = ImageColor.getrgb("green") + (120,)
 
                 drw.rectangle(
                     (
                         int(min_x * width),
                         int(min_y * height),
                         int(max_x * width),
                         int(max_y * height),
@@ -666,15 +701,27 @@
                     drw.rectangle(
                         (int(checkbox.bbox.x * width),
                         int(checkbox.bbox.y * height),
                         int((checkbox.bbox.x + checkbox.bbox.width) * width),
                         int((checkbox.bbox.y + checkbox.bbox.height) * height)),
                         outline=ImageColor.getrgb("lightgreen") if checkbox.is_selected() else ImageColor.getrgb("indianred")
                     )
-        elif entity.__class__.__name__ == "Query":
+    # Second drawing bounding boxes
+    for entity in entities:
+        if entity.__class__.__name__ == "Query":
+            overlayer_data = _get_overlayer_data(entity.result, width, height)
+            drw.rectangle(
+                xy=overlayer_data["coords"], outline=overlayer_data["color"], width=2
+            )
+        elif entity.__class__.__name__ == "TableTitle":
+            overlayer_data = _get_overlayer_data(entity.result, width, height)
+            drw.rectangle(
+                xy=overlayer_data["coords"], outline=overlayer_data["color"], width=2
+            )
+        elif entity.__class__.__name__ == "TableFooter":
             overlayer_data = _get_overlayer_data(entity.result, width, height)
             drw.rectangle(
                 xy=overlayer_data["coords"], outline=overlayer_data["color"], width=2
             )
         elif entity.__class__.__name__ == "ExpenseField":
             overlayer_data = _get_overlayer_data(entity, width, height)
             drw.rectangle(
@@ -921,14 +968,20 @@
             value_bbox.height * height + 2,
         )
         data["value_bbox"] = [x, y, x + w, y + h]
 
     elif entity.__class__.__name__ == "Table":
         data["color"] = ImageColor.getrgb("green")
         data["text"] = ""
+    elif entity.__class__.__name__ == "TableTitle":
+        data["color"] = ImageColor.getrgb("green")
+        data["text"] = ""
+    elif entity.__class__.__name__ == "TableFooter":
+        data["color"] = ImageColor.getrgb("green")
+        data["text"] = ""
 
     elif entity.__class__.__name__ == "TableCell":
         data["color"] = ImageColor.getrgb("skyblue")
         data["text"] = entity.__repr__().split(">")[-1][1:]
 
     elif entity.__class__.__name__ == "QueryResult":
         data["color"] = ImageColor.getrgb("mediumturquoise")
```

