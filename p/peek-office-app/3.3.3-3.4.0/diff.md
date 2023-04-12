# Comparing `tmp/peek-office-app-3.3.3.tar.gz` & `tmp/peek-office-app-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-office-app-3.3.3.tar", last modified: Mon Nov 14 05:36:23 2022, max compression
+gzip compressed data, was "peek-office-app-3.4.0.tar", last modified: Wed Apr 12 11:05:09 2023, max compression
```

## Comparing `peek-office-app-3.3.3.tar` & `peek-office-app-3.4.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.884107 peek-office-app-3.3.3/
--rw-r--r--   0 root         (0) root         (0)      364 2022-11-14 05:36:23.883107 peek-office-app-3.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1052 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.878107 peek-office-app-3.3.3/peek_office_app/
--rw-r--r--   0 root         (0) root         (0)      487 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/.browserslistrc
--rw-r--r--   0 root         (0) root         (0)       69 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/.gitignore
--rw-r--r--   0 root         (0) root         (0)      460 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)     1082 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/README.md
--rw-r--r--   0 root         (0) root         (0)       22 2022-11-14 05:36:23.000000 peek-office-app-3.3.3/peek_office_app/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6615 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/angular.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.879107 peek-office-app-3.3.3/peek_office_app/e2e/
--rw-r--r--   0 root         (0) root         (0)      326 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/e2e/app.e2e-spec.ts
--rw-r--r--   0 root         (0) root         (0)      227 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/e2e/app.po.ts
--rw-r--r--   0 root         (0) root         (0)      367 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/e2e/tsconfig.e2e.json
--rw-r--r--   0 root         (0) root         (0)     1341 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/karma.conf.js
--rw-r--r--   0 root         (0) root         (0)   678663 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/package-lock.json
--rw-r--r--   0 root         (0) root         (0)     2837 2022-11-14 05:36:23.000000 peek-office-app-3.3.3/peek_office_app/package.json
--rw-r--r--   0 root         (0) root         (0)      868 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/protractor.conf.js
--rw-r--r--   0 root         (0) root         (0)      279 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/proxy.conf.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.880107 peek-office-app-3.3.3/peek_office_app/src/
--rw-r--r--   0 root         (0) root         (0)     1151 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/_components.scss
--rw-r--r--   0 root         (0) root         (0)      994 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/_variables.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.880107 peek-office-app-3.3.3/peek_office_app/src/app/
--rw-r--r--   0 root         (0) root         (0)     2400 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/app.module.ts
--rw-r--r--   0 root         (0) root         (0)     1110 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/app.routes.ts
--rw-r--r--   0 root         (0) root         (0)      897 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/app.services.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.880107 peek-office-app-3.3.3/peek_office_app/src/app/core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.880107 peek-office-app-3.3.3/peek_office_app/src/app/core/components/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.880107 peek-office-app-3.3.3/peek_office_app/src/app/core/components/app/
--rw-r--r--   0 root         (0) root         (0)      746 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/core/components/app/app.component.html
--rw-r--r--   0 root         (0) root         (0)      899 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/core/components/app/app.component.scss
--rw-r--r--   0 root         (0) root         (0)     1391 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/core/components/app/app.component.ts
--rw-r--r--   0 root         (0) root         (0)       33 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/core/components/app/index.ts
--rw-r--r--   0 root         (0) root         (0)     1012 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/core/components/components.module.ts
--rw-r--r--   0 root         (0) root         (0)       37 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/core/components/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.880107 peek-office-app-3.3.3/peek_office_app/src/app/core/components/sidebar/
--rw-r--r--   0 root         (0) root         (0)       37 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/core/components/sidebar/index.ts
--rw-r--r--   0 root         (0) root         (0)     3416 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/core/components/sidebar/sidebar.component.html
--rw-r--r--   0 root         (0) root         (0)     1457 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/core/components/sidebar/sidebar.component.scss
--rw-r--r--   0 root         (0) root         (0)     2935 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/core/components/sidebar/sidebar.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.881107 peek-office-app-3.3.3/peek_office_app/src/app/core/components/status/
--rw-r--r--   0 root         (0) root         (0)       36 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/core/components/status/index.ts
--rw-r--r--   0 root         (0) root         (0)      861 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/core/components/status/status.component.html
--rw-r--r--   0 root         (0) root         (0)      505 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/core/components/status/status.component.scss
--rw-r--r--   0 root         (0) root         (0)     1585 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/core/components/status/status.component.ts
--rw-r--r--   0 root         (0) root         (0)       30 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/core/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.881107 peek-office-app-3.3.3/peek_office_app/src/app/pages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.881107 peek-office-app-3.3.3/peek_office_app/src/app/pages/config/
--rw-r--r--   0 root         (0) root         (0)      948 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/pages/config/config.page.html
--rw-r--r--   0 root         (0) root         (0)     1373 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/pages/config/config.page.scss
--rw-r--r--   0 root         (0) root         (0)      723 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/pages/config/config.page.ts
--rw-r--r--   0 root         (0) root         (0)       44 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/pages/config/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.881107 peek-office-app-3.3.3/peek_office_app/src/app/pages/home/
--rw-r--r--   0 root         (0) root         (0)      113 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/pages/home/home.page.html
--rw-r--r--   0 root         (0) root         (0)      333 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/pages/home/home.page.scss
--rw-r--r--   0 root         (0) root         (0)      597 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/pages/home/home.page.ts
--rw-r--r--   0 root         (0) root         (0)       40 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/pages/home/index.ts
--rw-r--r--   0 root         (0) root         (0)      126 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/pages/index.ts
--rw-r--r--   0 root         (0) root         (0)      800 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/pages/pages.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.882107 peek-office-app-3.3.3/peek_office_app/src/app/pages/unknown-route/
--rw-r--r--   0 root         (0) root         (0)       57 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/pages/unknown-route/index.ts
--rw-r--r--   0 root         (0) root         (0)    19057 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/pages/unknown-route/unknown-route.page.html
--rw-r--r--   0 root         (0) root         (0)     1101 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/pages/unknown-route/unknown-route.page.scss
--rw-r--r--   0 root         (0) root         (0)      513 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/pages/unknown-route/unknown-route.page.ts
--rw-r--r--   0 root         (0) root         (0)      222 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/app/plugin-root.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.883107 peek-office-app-3.3.3/peek_office_app/src/assets/
--rw-r--r--   0 root         (0) root         (0)   156480 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/assets/Poppins-Medium.ttf
--rw-r--r--   0 root         (0) root         (0)   158192 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/assets/Poppins-Regular.ttf
--rw-r--r--   0 root         (0) root         (0)   155192 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/assets/Poppins-SemiBold.ttf
--rw-r--r--   0 root         (0) root         (0)   715281 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/assets/home-background.png
--rw-r--r--   0 root         (0) root         (0)    66513 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/assets/home-center.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.883107 peek-office-app-3.3.3/peek_office_app/src/assets/peek_core_docdb/
--rw-r--r--   0 root         (0) root         (0)    12054 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/assets/peek_core_docdb/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.883107 peek-office-app-3.3.3/peek_office_app/src/assets/peek_core_search/
--rw-r--r--   0 root         (0) root         (0)    12730 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/assets/peek_core_search/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.883107 peek-office-app-3.3.3/peek_office_app/src/assets/peek_core_user/
--rw-r--r--   0 root         (0) root         (0)     5572 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/assets/peek_core_user/plugin_icon.png
--rw-r--r--   0 root         (0) root         (0)   161189 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/assets/sidebar_background.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.883107 peek-office-app-3.3.3/peek_office_app/src/environments/
--rw-r--r--   0 root         (0) root         (0)       54 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/environments/environment.prod.ts
--rw-r--r--   0 root         (0) root         (0)      390 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/environments/environment.ts
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-14 05:36:23.000000 peek-office-app-3.3.3/peek_office_app/src/environments/peek-app-environment.ts
--rw-r--r--   0 root         (0) root         (0)    39980 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/favicon.ico
--rw-r--r--   0 root         (0) root         (0)     4988 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/index.html
--rw-r--r--   0 root         (0) root         (0)      737 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/main.ts
--rw-r--r--   0 root         (0) root         (0)     2395 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/polyfills.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.883107 peek-office-app-3.3.3/peek_office_app/src/styles/
--rw-r--r--   0 root         (0) root         (0)     5595 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/styles/shared.scss
--rw-r--r--   0 root         (0) root         (0)    33066 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/styles/theme.less
--rw-r--r--   0 root         (0) root         (0)     3384 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/styles.scss
--rw-r--r--   0 root         (0) root         (0)     1090 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/test.ts
--rw-r--r--   0 root         (0) root         (0)      521 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/tsconfig.app.json
--rw-r--r--   0 root         (0) root         (0)      242 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/tsconfig.spec.json
--rw-r--r--   0 root         (0) root         (0)      101 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/src/typings.d.ts
--rw-r--r--   0 root         (0) root         (0)      414 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/tsconfig.json
--rw-r--r--   0 root         (0) root         (0)      320 2022-11-14 05:34:28.000000 peek-office-app-3.3.3/peek_office_app/tsconfig.worker.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:23.879107 peek-office-app-3.3.3/peek_office_app.egg-info/
--rw-r--r--   0 root         (0) root         (0)      364 2022-11-14 05:36:23.000000 peek-office-app-3.3.3/peek_office_app.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3632 2022-11-14 05:36:23.000000 peek-office-app-3.3.3/peek_office_app.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:36:23.000000 peek-office-app-3.3.3/peek_office_app.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:36:23.000000 peek-office-app-3.3.3/peek_office_app.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       32 2022-11-14 05:36:23.000000 peek-office-app-3.3.3/peek_office_app.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-11-14 05:36:23.000000 peek-office-app-3.3.3/peek_office_app.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-14 05:36:23.884107 peek-office-app-3.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3089 2022-11-14 05:36:23.000000 peek-office-app-3.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.477208 peek-office-app-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-04-12 11:05:09.477208 peek-office-app-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.473208 peek-office-app-3.4.0/peek_office_app/
+-rw-r--r--   0 root         (0) root         (0)      487 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/.browserslistrc
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/README.md
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-12 11:05:09.000000 peek-office-app-3.4.0/peek_office_app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6615 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/angular.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.474208 peek-office-app-3.4.0/peek_office_app/e2e/
+-rw-r--r--   0 root         (0) root         (0)      326 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/e2e/app.e2e-spec.ts
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/e2e/app.po.ts
+-rw-r--r--   0 root         (0) root         (0)      367 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/e2e/tsconfig.e2e.json
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/karma.conf.js
+-rw-r--r--   0 root         (0) root         (0)   680107 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/package-lock.json
+-rw-r--r--   0 root         (0) root         (0)     3021 2023-04-12 11:05:09.000000 peek-office-app-3.4.0/peek_office_app/package.json
+-rw-r--r--   0 root         (0) root         (0)      868 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/protractor.conf.js
+-rw-r--r--   0 root         (0) root         (0)      279 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/proxy.conf.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.474208 peek-office-app-3.4.0/peek_office_app/src/
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/_components.scss
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/_variables.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.474208 peek-office-app-3.4.0/peek_office_app/src/app/
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/app.module.ts
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/app.routes.ts
+-rw-r--r--   0 root         (0) root         (0)      897 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/app.services.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.474208 peek-office-app-3.4.0/peek_office_app/src/app/core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.475208 peek-office-app-3.4.0/peek_office_app/src/app/core/components/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.475208 peek-office-app-3.4.0/peek_office_app/src/app/core/components/app/
+-rw-r--r--   0 root         (0) root         (0)      746 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/core/components/app/app.component.html
+-rw-r--r--   0 root         (0) root         (0)      899 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/core/components/app/app.component.scss
+-rw-r--r--   0 root         (0) root         (0)     1391 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/core/components/app/app.component.ts
+-rw-r--r--   0 root         (0) root         (0)       33 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/core/components/app/index.ts
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/core/components/components.module.ts
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/core/components/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.475208 peek-office-app-3.4.0/peek_office_app/src/app/core/components/sidebar/
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/core/components/sidebar/index.ts
+-rw-r--r--   0 root         (0) root         (0)     3805 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/core/components/sidebar/sidebar.component.html
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/core/components/sidebar/sidebar.component.scss
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/core/components/sidebar/sidebar.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.475208 peek-office-app-3.4.0/peek_office_app/src/app/core/components/status/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/core/components/status/index.ts
+-rw-r--r--   0 root         (0) root         (0)      861 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/core/components/status/status.component.html
+-rw-r--r--   0 root         (0) root         (0)      505 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/core/components/status/status.component.scss
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/core/components/status/status.component.ts
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/core/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.475208 peek-office-app-3.4.0/peek_office_app/src/app/pages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.475208 peek-office-app-3.4.0/peek_office_app/src/app/pages/config/
+-rw-r--r--   0 root         (0) root         (0)      948 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/pages/config/config.page.html
+-rw-r--r--   0 root         (0) root         (0)     1373 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/pages/config/config.page.scss
+-rw-r--r--   0 root         (0) root         (0)      723 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/pages/config/config.page.ts
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/pages/config/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.476208 peek-office-app-3.4.0/peek_office_app/src/app/pages/home/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/pages/home/home.page.html
+-rw-r--r--   0 root         (0) root         (0)      333 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/pages/home/home.page.scss
+-rw-r--r--   0 root         (0) root         (0)      597 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/pages/home/home.page.ts
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/pages/home/index.ts
+-rw-r--r--   0 root         (0) root         (0)      126 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/pages/index.ts
+-rw-r--r--   0 root         (0) root         (0)      800 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/pages/pages.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.476208 peek-office-app-3.4.0/peek_office_app/src/app/pages/unknown-route/
+-rw-r--r--   0 root         (0) root         (0)       57 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/pages/unknown-route/index.ts
+-rw-r--r--   0 root         (0) root         (0)    19057 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/pages/unknown-route/unknown-route.page.html
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/pages/unknown-route/unknown-route.page.scss
+-rw-r--r--   0 root         (0) root         (0)      513 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/pages/unknown-route/unknown-route.page.ts
+-rw-r--r--   0 root         (0) root         (0)      222 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/app/plugin-root.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.477208 peek-office-app-3.4.0/peek_office_app/src/assets/
+-rw-r--r--   0 root         (0) root         (0)   156480 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/assets/Poppins-Medium.ttf
+-rw-r--r--   0 root         (0) root         (0)   158192 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/assets/Poppins-Regular.ttf
+-rw-r--r--   0 root         (0) root         (0)   155192 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/assets/Poppins-SemiBold.ttf
+-rw-r--r--   0 root         (0) root         (0)   715281 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/assets/home-background.png
+-rw-r--r--   0 root         (0) root         (0)    66513 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/assets/home-center.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.477208 peek-office-app-3.4.0/peek_office_app/src/assets/peek_core_docdb/
+-rw-r--r--   0 root         (0) root         (0)    12054 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/assets/peek_core_docdb/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.477208 peek-office-app-3.4.0/peek_office_app/src/assets/peek_core_search/
+-rw-r--r--   0 root         (0) root         (0)    12730 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/assets/peek_core_search/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.477208 peek-office-app-3.4.0/peek_office_app/src/assets/peek_core_user/
+-rw-r--r--   0 root         (0) root         (0)     5572 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/assets/peek_core_user/plugin_icon.png
+-rw-r--r--   0 root         (0) root         (0)   161189 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/assets/sidebar_background.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.477208 peek-office-app-3.4.0/peek_office_app/src/environments/
+-rw-r--r--   0 root         (0) root         (0)       54 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/environments/environment.prod.ts
+-rw-r--r--   0 root         (0) root         (0)      390 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/environments/environment.ts
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-12 11:05:09.000000 peek-office-app-3.4.0/peek_office_app/src/environments/peek-app-environment.ts
+-rw-r--r--   0 root         (0) root         (0)    39980 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)     4988 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/index.html
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/main.ts
+-rw-r--r--   0 root         (0) root         (0)     2395 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/polyfills.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.477208 peek-office-app-3.4.0/peek_office_app/src/styles/
+-rw-r--r--   0 root         (0) root         (0)     5595 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/styles/shared.scss
+-rw-r--r--   0 root         (0) root         (0)    33066 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/styles/theme.less
+-rw-r--r--   0 root         (0) root         (0)     3384 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/styles.scss
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/test.ts
+-rw-r--r--   0 root         (0) root         (0)      521 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/tsconfig.app.json
+-rw-r--r--   0 root         (0) root         (0)      242 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/tsconfig.spec.json
+-rw-r--r--   0 root         (0) root         (0)      101 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/src/typings.d.ts
+-rw-r--r--   0 root         (0) root         (0)      414 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/tsconfig.json
+-rw-r--r--   0 root         (0) root         (0)      320 2023-04-12 11:03:19.000000 peek-office-app-3.4.0/peek_office_app/tsconfig.worker.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:09.473208 peek-office-app-3.4.0/peek_office_app.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-04-12 11:05:09.000000 peek-office-app-3.4.0/peek_office_app.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3632 2023-04-12 11:05:09.000000 peek-office-app-3.4.0/peek_office_app.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:05:09.000000 peek-office-app-3.4.0/peek_office_app.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:05:09.000000 peek-office-app-3.4.0/peek_office_app.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-12 11:05:09.000000 peek-office-app-3.4.0/peek_office_app.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-12 11:05:09.000000 peek-office-app-3.4.0/peek_office_app.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 11:05:09.477208 peek-office-app-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3089 2023-04-12 11:05:09.000000 peek-office-app-3.4.0/setup.py
```

### Comparing `peek-office-app-3.3.3/README.rst` & `peek-office-app-3.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/README.md` & `peek-office-app-3.4.0/peek_office_app/README.md`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/angular.json` & `peek-office-app-3.4.0/peek_office_app/angular.json`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/karma.conf.js` & `peek-office-app-3.4.0/peek_office_app/karma.conf.js`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/package-lock.json` & `peek-office-app-3.4.0/peek_office_app/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999621246587807%*

 * *Differences: {"'dependencies'": "{'@synerty/vortexjs': {'version': '3.3.3', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@synerty/vortexjs/-/vortexjs-3.3.3.tgz', "*

 * *                   "'integrity': "*

 * *                   "'sha512-SE4PvtrpdAVfwarFAYJkAzpiwjFyxDhdnQxS8C2y2vN1mLV5yE1J7mPExOyQIMwXFbCdO+GtUHuBgpIk+WVUDg==', "*

 * *                   "'dependencies': {'tslib': {'version': '2.5.0', 'resolved': "*

 * *                   "'https://registry.npmjs.org/tslib/-/tslib-2.5.0.tgz', 'integrity': "*

 * *                   […]*

```diff
@@ -1721,14 +1721,30 @@
             "version": "7.12.1"
         },
         "@capacitor-community/background-geolocation": {
             "integrity": "sha512-2dbTAjcSibf1OYl66KqH3Yhh9cBqhvppJlcV5Z6BMgPqccPcPTipPCoQpWdTIc8fZfKjSUD5DVDZjPMbRV3cTw==",
             "resolved": "https://registry.npmjs.org/@capacitor-community/background-geolocation/-/background-geolocation-1.2.1.tgz",
             "version": "1.2.1"
         },
+        "@capacitor-community/file-opener": {
+            "integrity": "sha512-tNxt6HeyPYW5Q0ZarEIG2uBbWEtLYpUnEyyxWXobWccXqJegT19KXwX53/vbzPBy56Z8pEQR8RavRnJOSha1Eg==",
+            "resolved": "https://registry.npmjs.org/@capacitor-community/file-opener/-/file-opener-1.0.4.tgz",
+            "version": "1.0.4"
+        },
+        "@capacitor-community/http": {
+            "integrity": "sha512-+pCkBXrwfm97UfjOgjV950H/qZ8SE36Mrcb46BlL1ps3VIsGuIO+AulL8GqTC6LewheRVtGJpRspNtneXQotNA==",
+            "requires": {
+                "@capacitor/android": "^3.0.0",
+                "@capacitor/core": "^3.0.0",
+                "@capacitor/filesystem": "^1.0.0",
+                "@capacitor/ios": "^3.0.0"
+            },
+            "resolved": "https://registry.npmjs.org/@capacitor-community/http/-/http-1.4.1.tgz",
+            "version": "1.4.1"
+        },
         "@capacitor-community/sqlite": {
             "integrity": "sha512-51ZW+CQoXnuW8HXgVsUfXS+rvUQaVp3LthLKEj0o+1n2sC5A3hJm6w6+nL/1tgvyJi00Pj8uB9IKKqE6E+qIeg==",
             "requires": {
                 "jeep-sqlite": "^1.5.2"
             },
             "resolved": "https://registry.npmjs.org/@capacitor-community/sqlite/-/sqlite-3.5.1-1.tgz",
             "version": "3.5.1-1"
@@ -1739,14 +1755,19 @@
             "version": "3.5.1"
         },
         "@capacitor/app": {
             "integrity": "sha512-8ADkldHnoE1xkWvPUsGlERVGm6/Zvcxy6hCI80AxydIKyaCG7kbDAvUclebbnw/eFRxj2zBoVatGLjmJNvTbYw==",
             "resolved": "https://registry.npmjs.org/@capacitor/app/-/app-1.1.1.tgz",
             "version": "1.1.1"
         },
+        "@capacitor/browser": {
+            "integrity": "sha512-ni8IjsPyFUYqQ2JxBwzI7VpJUZHPr7QiRds5hQWM/1cpfH0+DWvjWHwzxQXuSbW0h+QGXGSJ/vwqjRns7NzLfQ==",
+            "resolved": "https://registry.npmjs.org/@capacitor/browser/-/browser-1.0.7.tgz",
+            "version": "1.0.7"
+        },
         "@capacitor/cli": {
             "dependencies": {
                 "commander": {
                     "integrity": "sha512-U7VdrJFnJgo4xjrHpTzu0yrHPGImdsmD95ZlgYSEajAn2JKzDhDTPG9kBTefmObL2w/ngeZnilk+OV9CG3d7UA==",
                     "resolved": "https://registry.npmjs.org/commander/-/commander-6.2.1.tgz",
                     "version": "6.2.1"
                 },
@@ -1834,14 +1855,19 @@
             "version": "1.1.2"
         },
         "@capacitor/dialog": {
             "integrity": "sha512-+B6lKlqlpZk9uDrHEYk2rj+b3DF1kxCqV+vGtKwNMr2tFvNppZVkYdZU+L503yAoFFejqgQ27n0A4vXg+BTcBQ==",
             "resolved": "https://registry.npmjs.org/@capacitor/dialog/-/dialog-1.0.7.tgz",
             "version": "1.0.7"
         },
+        "@capacitor/filesystem": {
+            "integrity": "sha512-8O3UuvL8HNUEJvZnmn8yUmvgB1evtXfcF0oxIo3YbSlylqywJwS3JTiuhKmsvSxCdpbTy8IaTsutVh3gZgWbKg==",
+            "resolved": "https://registry.npmjs.org/@capacitor/filesystem/-/filesystem-1.1.0.tgz",
+            "version": "1.1.0"
+        },
         "@capacitor/geolocation": {
             "integrity": "sha512-3u9Hu4E0VBMa6r0d2t9MENDIR+bv5Tf144uPmb2Bl7XLQeFwvu4BSp2neNq39x58PvcROPMNX1BOTSGpQep+1Q==",
             "resolved": "https://registry.npmjs.org/@capacitor/geolocation/-/geolocation-1.3.1.tgz",
             "version": "1.3.1"
         },
         "@capacitor/ios": {
             "integrity": "sha512-295L9dHe/QaejUpGI8Pxwb1i2yVgick1ExIDK26xk+tk1km3B1HVjsIS8qkf2SOp7tuwP9+W5T5p7rLMNN4v5g==",
@@ -2253,25 +2279,25 @@
             },
             "resolved": "https://registry.npmjs.org/@synerty/peek-plugin-base-js/-/peek-plugin-base-js-10.7.10.tgz",
             "version": "10.7.10"
         },
         "@synerty/vortexjs": {
             "dependencies": {
                 "tslib": {
-                    "integrity": "sha512-d6xOpEDfsi2CZVlPQzGeux8XMwLT9hssAsaPYExaQMuYskwb+x1x7J371tWlbBdWHroy99KnVB6qIkUbs5X3UQ==",
-                    "resolved": "https://registry.npmjs.org/tslib/-/tslib-2.4.0.tgz",
-                    "version": "2.4.0"
+                    "integrity": "sha512-336iVw3rtn2BUK7ORdIAHTyxHGRIHVReokCR3XjbckJMK7ms8FysBfhLR8IXnAgy7T0PTPNBWKiH514FOW/WSg==",
+                    "resolved": "https://registry.npmjs.org/tslib/-/tslib-2.5.0.tgz",
+                    "version": "2.5.0"
                 }
             },
-            "integrity": "sha512-mH7pbrJfx8C16cHCdPFbzMpSGq9An2BKZjUwzzMfnemHksujYO+xXtOTbKHrY/tu/xXaSYUEzgbzr8aTqqOs1Q==",
+            "integrity": "sha512-SE4PvtrpdAVfwarFAYJkAzpiwjFyxDhdnQxS8C2y2vN1mLV5yE1J7mPExOyQIMwXFbCdO+GtUHuBgpIk+WVUDg==",
             "requires": {
                 "tslib": "^2.0.0"
             },
-            "resolved": "https://registry.npmjs.org/@synerty/vortexjs/-/vortexjs-3.2.5.tgz",
-            "version": "3.2.5"
+            "resolved": "https://registry.npmjs.org/@synerty/vortexjs/-/vortexjs-3.3.3.tgz",
+            "version": "3.3.3"
         },
         "@types/cordova": {
             "integrity": "sha512-rkiiTuf/z2wTd4RxFOb+clE7PF4AEJU0hsczbUdkHHBtkUmpWQpEddynNfJYKYtZFJKbq4F+brfekt1kx85IZA==",
             "resolved": "https://registry.npmjs.org/@types/cordova/-/cordova-0.0.34.tgz",
             "version": "0.0.34"
         },
         "@types/emscripten": {
```

### Comparing `peek-office-app-3.3.3/peek_office_app/package.json` & `peek-office-app-3.4.0/peek_office_app/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9159943046986238%*

 * *Differences: {"'dependencies'": "{'@synerty/vortexjs': '^3.3.3', '@capacitor-community/file-opener': '^1.0.4', "*

 * *                   "'@capacitor-community/http': '^1.4.1', '@capacitor/browser': '^1.0.7', "*

 * *                   "'@capacitor/filesystem': '^1.1.0'}",*

 * * "'scripts'": "{'start': 'ng serve --disableHostCheck --host 3.4.0.0 --port 4002 --proxy-config "*

 * *              "proxy.conf.json'}",*

 * * "'version'": "'3.4.0'"}*

```diff
@@ -8,28 +8,32 @@
         "@angular/forms": "^10.2.0",
         "@angular/platform-browser": "^10.2.0",
         "@angular/platform-browser-dynamic": "^10.2.0",
         "@angular/router": "^10.2.0",
         "@awesome-cordova-plugins/core": "^5.41.0",
         "@awesome-cordova-plugins/native-audio": "^5.41.0",
         "@capacitor-community/background-geolocation": "^1.2.1",
+        "@capacitor-community/file-opener": "^1.0.4",
+        "@capacitor-community/http": "^1.4.1",
         "@capacitor-community/sqlite": "^3.5.1-1",
         "@capacitor/android": "^3.5.1",
         "@capacitor/app": "^1.1.1",
+        "@capacitor/browser": "^1.0.7",
         "@capacitor/cli": "^3.5.1",
         "@capacitor/core": "^3.5.1",
         "@capacitor/device": "^1.1.2",
         "@capacitor/dialog": "^1.0.7",
+        "@capacitor/filesystem": "^1.1.0",
         "@capacitor/geolocation": "^1.3.1",
         "@capacitor/ios": "^3.5.1",
         "@capacitor/local-notifications": "^1.1.0",
         "@capacitor/network": "^1.0.7",
         "@ionic/pwa-elements": "^3.1.1",
         "@synerty/peek-plugin-base-js": "^10.7.10",
-        "@synerty/vortexjs": "^3.2.5",
+        "@synerty/vortexjs": "^3.3.3",
         "assert": "^1.5.0",
         "base-64": "^0.1.0",
         "bootstrap": "^3.4.1",
         "cordova-plugin-nativeaudio": "^3.0.9",
         "core-js": "^3.6.5",
         "jquery": "^3.4.1",
         "json-stable-stringify": "^1.0.1",
@@ -67,12 +71,12 @@
     "private": true,
     "scripts": {
         "build": "ng build",
         "e2e": "ng e2e",
         "lint": "ng lint",
         "ng": "ng",
         "postinstall": "ngcc --properties es2015 es5 browser module main --first-only --create-ivy-entry-points",
-        "start": "ng serve --disableHostCheck --host 3.3.3.0 --port 4002 --proxy-config proxy.conf.json",
+        "start": "ng serve --disableHostCheck --host 3.4.0.0 --port 4002 --proxy-config proxy.conf.json",
         "test": "ng test"
     },
-    "version": "3.3.3"
+    "version": "3.4.0"
 }
```

### Comparing `peek-office-app-3.3.3/peek_office_app/protractor.conf.js` & `peek-office-app-3.4.0/peek_office_app/protractor.conf.js`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/_components.scss` & `peek-office-app-3.4.0/peek_office_app/src/_components.scss`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/_variables.scss` & `peek-office-app-3.4.0/peek_office_app/src/_variables.scss`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/app/app.module.ts` & `peek-office-app-3.4.0/peek_office_app/src/app/app.module.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/app/app.routes.ts` & `peek-office-app-3.4.0/peek_office_app/src/app/app.routes.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/app/app.services.ts` & `peek-office-app-3.4.0/peek_office_app/src/app/app.services.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/app/core/components/app/app.component.html` & `peek-office-app-3.4.0/peek_office_app/src/app/core/components/app/app.component.html`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/app/core/components/app/app.component.scss` & `peek-office-app-3.4.0/peek_office_app/src/app/core/components/app/app.component.scss`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/app/core/components/app/app.component.ts` & `peek-office-app-3.4.0/peek_office_app/src/app/core/components/app/app.component.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/app/core/components/components.module.ts` & `peek-office-app-3.4.0/peek_office_app/src/app/core/components/components.module.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/app/core/components/sidebar/sidebar.component.html` & `peek-office-app-3.4.0/peek_office_app/src/app/core/components/sidebar/sidebar.component.html`

 * *Files 2% similar despite different names*

```diff
@@ -180,35 +180,59 @@
 00000b30: 2020 3e0a 2020 2020 2020 2020 2020 2020    >.            
 00000b40: 2020 2020 3c69 206e 7a2d 6963 6f6e 206e      <i nz-icon n
 00000b50: 7a54 6865 6d65 3d22 6f75 746c 696e 6522  zTheme="outline"
 00000b60: 206e 7a54 7970 653d 2273 6574 7469 6e67   nzType="setting
 00000b70: 223e 3c2f 693e 0a20 2020 2020 2020 2020  "></i>.         
 00000b80: 2020 203c 2f62 7574 746f 6e3e 0a20 2020     </button>.   
 00000b90: 2020 2020 203c 2f64 6976 3e0a 0a20 2020       </div>..   
-00000ba0: 2020 2020 203c 6469 760a 2020 2020 2020       <div.      
-00000bb0: 2020 2020 2020 5b6e 7a54 6f6f 6c74 6970        [nzTooltip
-00000bc0: 5469 746c 655d 3d22 706f 7765 7265 6442  Title]="poweredB
-00000bd0: 7954 656d 706c 6174 6522 0a20 2020 2020  yTemplate".     
-00000be0: 2020 2020 2020 205b 726f 7574 6572 4c69         [routerLi
-00000bf0: 6e6b 5d3d 225b 272f 275d 220a 2020 2020  nk]="['/']".    
-00000c00: 2020 2020 2020 2020 6e7a 2d74 6f6f 6c74          nz-toolt
-00000c10: 6970 0a20 2020 2020 2020 2020 2020 205b  ip.            [
-00000c20: 6e7a 546f 6f6c 7469 704d 6f75 7365 456e  nzTooltipMouseEn
-00000c30: 7465 7244 656c 6179 5d3d 2231 2e30 220a  terDelay]="1.0".
-00000c40: 2020 2020 2020 2020 2020 2020 6e7a 546f              nzTo
-00000c50: 6f6c 7469 7050 6c61 6365 6d65 6e74 3d22  oltipPlacement="
-00000c60: 7269 6768 7454 6f70 220a 2020 2020 2020  rightTop".      
-00000c70: 2020 3e0a 2020 2020 2020 2020 2020 2020    >.            
-00000c80: 3c69 6d67 2063 6c61 7373 3d22 7369 6465  <img class="side
-00000c90: 6261 722d 706f 7765 7265 642d 6279 2220  bar-powered-by" 
-00000ca0: 7372 633d 222f 6173 7365 7473 2f68 6f6d  src="/assets/hom
-00000cb0: 652d 6365 6e74 6572 2e70 6e67 2220 2f3e  e-center.png" />
-00000cc0: 0a20 2020 2020 2020 203c 2f64 6976 3e0a  .        </div>.
-00000cd0: 2020 2020 3c2f 6469 763e 0a3c 2f64 6976      </div>.</div
-00000ce0: 3e0a 0a3c 6e67 2d74 656d 706c 6174 6520  >..<ng-template 
-00000cf0: 2370 6f77 6572 6564 4279 5465 6d70 6c61  #poweredByTempla
-00000d00: 7465 3e0a 2020 2020 3c69 6d67 2063 6c61  te>.    <img cla
-00000d10: 7373 3d22 706f 7765 7265 642d 6279 2d74  ss="powered-by-t
-00000d20: 6f6f 6c74 6970 2220 7372 633d 222f 6173  ooltip" src="/as
-00000d30: 7365 7473 2f68 6f6d 652d 6365 6e74 6572  sets/home-center
-00000d40: 2e70 6e67 2220 2f3e 0a3c 2f6e 672d 7465  .png" />.</ng-te
-00000d50: 6d70 6c61 7465 3e0a                      mplate>.
+00000ba0: 2020 2020 203c 6469 763e 0a20 2020 2020       <div>.     
+00000bb0: 2020 2020 2020 203c 6120 6872 6566 3d22         <a href="
+00000bc0: 2f64 6f63 732f 696e 6465 782e 6874 6d6c  /docs/index.html
+00000bd0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000be0: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
+00000bf0: 6275 7474 6f6e 0a20 2020 2020 2020 2020  button.         
+00000c00: 2020 2020 2020 2063 6c61 7373 3d22 7369         class="si
+00000c10: 6465 6261 722d 6275 7474 6f6e 220a 2020  debar-button".  
+00000c20: 2020 2020 2020 2020 2020 2020 2020 6e7a                nz
+00000c30: 2d74 6f6f 6c74 6970 0a20 2020 2020 2020  -tooltip.       
+00000c40: 2020 2020 2020 2020 206e 7a54 6f6f 6c74           nzToolt
+00000c50: 6970 506c 6163 656d 656e 743d 2272 6967  ipPlacement="rig
+00000c60: 6874 220a 2020 2020 2020 2020 2020 2020  ht".            
+00000c70: 2020 2020 6e7a 546f 6f6c 7469 7054 6974      nzTooltipTit
+00000c80: 6c65 3d22 4865 6c70 220a 2020 2020 2020  le="Help".      
+00000c90: 2020 2020 2020 3e0a 2020 2020 2020 2020        >.        
+00000ca0: 2020 2020 2020 2020 3c69 206e 7a2d 6963          <i nz-ic
+00000cb0: 6f6e 206e 7a54 6865 6d65 3d22 6f75 746c  on nzTheme="outl
+00000cc0: 696e 6522 206e 7a54 7970 653d 2271 7565  ine" nzType="que
+00000cd0: 7374 696f 6e2d 6369 7263 6c65 223e 3c2f  stion-circle"></
+00000ce0: 693e 0a20 2020 2020 2020 2020 2020 203c  i>.            <
+00000cf0: 2f62 7574 746f 6e3e 0a20 2020 2020 2020  /button>.       
+00000d00: 2020 2020 203c 2f61 3e0a 2020 2020 2020       </a>.      
+00000d10: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00000d20: 200a 2020 2020 2020 2020 3c64 6976 0a20   .        <div. 
+00000d30: 2020 2020 2020 2020 2020 205b 6e7a 546f             [nzTo
+00000d40: 6f6c 7469 7054 6974 6c65 5d3d 2270 6f77  oltipTitle]="pow
+00000d50: 6572 6564 4279 5465 6d70 6c61 7465 220a  eredByTemplate".
+00000d60: 2020 2020 2020 2020 2020 2020 5b72 6f75              [rou
+00000d70: 7465 724c 696e 6b5d 3d22 5b27 2f27 5d22  terLink]="['/']"
+00000d80: 0a20 2020 2020 2020 2020 2020 206e 7a2d  .            nz-
+00000d90: 746f 6f6c 7469 700a 2020 2020 2020 2020  tooltip.        
+00000da0: 2020 2020 5b6e 7a54 6f6f 6c74 6970 4d6f      [nzTooltipMo
+00000db0: 7573 6545 6e74 6572 4465 6c61 795d 3d22  useEnterDelay]="
+00000dc0: 312e 3022 0a20 2020 2020 2020 2020 2020  1.0".           
+00000dd0: 206e 7a54 6f6f 6c74 6970 506c 6163 656d   nzTooltipPlacem
+00000de0: 656e 743d 2272 6967 6874 546f 7022 0a20  ent="rightTop". 
+00000df0: 2020 2020 2020 203e 0a20 2020 2020 2020         >.       
+00000e00: 2020 2020 203c 696d 6720 636c 6173 733d       <img class=
+00000e10: 2273 6964 6562 6172 2d70 6f77 6572 6564  "sidebar-powered
+00000e20: 2d62 7922 2073 7263 3d22 2f61 7373 6574  -by" src="/asset
+00000e30: 732f 686f 6d65 2d63 656e 7465 722e 706e  s/home-center.pn
+00000e40: 6722 202f 3e0a 2020 2020 2020 2020 3c2f  g" />.        </
+00000e50: 6469 763e 0a20 2020 203c 2f64 6976 3e0a  div>.    </div>.
+00000e60: 3c2f 6469 763e 0a0a 3c6e 672d 7465 6d70  </div>..<ng-temp
+00000e70: 6c61 7465 2023 706f 7765 7265 6442 7954  late #poweredByT
+00000e80: 656d 706c 6174 653e 0a20 2020 203c 696d  emplate>.    <im
+00000e90: 6720 636c 6173 733d 2270 6f77 6572 6564  g class="powered
+00000ea0: 2d62 792d 746f 6f6c 7469 7022 2073 7263  -by-tooltip" src
+00000eb0: 3d22 2f61 7373 6574 732f 686f 6d65 2d63  ="/assets/home-c
+00000ec0: 656e 7465 722e 706e 6722 202f 3e0a 3c2f  enter.png" />.</
+00000ed0: 6e67 2d74 656d 706c 6174 653e 0a         ng-template>.
```

### Comparing `peek-office-app-3.3.3/peek_office_app/src/app/core/components/sidebar/sidebar.component.scss` & `peek-office-app-3.4.0/peek_office_app/src/app/core/components/sidebar/sidebar.component.scss`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/app/core/components/sidebar/sidebar.component.ts` & `peek-office-app-3.4.0/peek_office_app/src/app/core/components/sidebar/sidebar.component.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/app/core/components/status/status.component.html` & `peek-office-app-3.4.0/peek_office_app/src/app/core/components/status/status.component.html`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/app/core/components/status/status.component.ts` & `peek-office-app-3.4.0/peek_office_app/src/app/core/components/status/status.component.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/app/pages/config/config.page.html` & `peek-office-app-3.4.0/peek_office_app/src/app/pages/config/config.page.html`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/app/pages/config/config.page.scss` & `peek-office-app-3.4.0/peek_office_app/src/app/pages/config/config.page.scss`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/app/pages/config/config.page.ts` & `peek-office-app-3.4.0/peek_office_app/src/app/pages/config/config.page.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/app/pages/home/home.page.ts` & `peek-office-app-3.4.0/peek_office_app/src/app/pages/home/home.page.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/app/pages/pages.module.ts` & `peek-office-app-3.4.0/peek_office_app/src/app/pages/pages.module.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/app/pages/unknown-route/unknown-route.page.html` & `peek-office-app-3.4.0/peek_office_app/src/app/pages/unknown-route/unknown-route.page.html`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/app/pages/unknown-route/unknown-route.page.scss` & `peek-office-app-3.4.0/peek_office_app/src/app/pages/unknown-route/unknown-route.page.scss`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/app/pages/unknown-route/unknown-route.page.ts` & `peek-office-app-3.4.0/peek_office_app/src/app/pages/unknown-route/unknown-route.page.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/assets/Poppins-Medium.ttf` & `peek-office-app-3.4.0/peek_office_app/src/assets/Poppins-Medium.ttf`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/assets/Poppins-Regular.ttf` & `peek-office-app-3.4.0/peek_office_app/src/assets/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/assets/Poppins-SemiBold.ttf` & `peek-office-app-3.4.0/peek_office_app/src/assets/Poppins-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/assets/home-background.png` & `peek-office-app-3.4.0/peek_office_app/src/assets/home-background.png`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/assets/home-center.png` & `peek-office-app-3.4.0/peek_office_app/src/assets/home-center.png`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/assets/peek_core_docdb/icon.png` & `peek-office-app-3.4.0/peek_office_app/src/assets/peek_core_docdb/icon.png`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/assets/peek_core_search/icon.png` & `peek-office-app-3.4.0/peek_office_app/src/assets/peek_core_search/icon.png`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/assets/peek_core_user/plugin_icon.png` & `peek-office-app-3.4.0/peek_office_app/src/assets/peek_core_user/plugin_icon.png`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/assets/sidebar_background.png` & `peek-office-app-3.4.0/peek_office_app/src/assets/sidebar_background.png`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/favicon.ico` & `peek-office-app-3.4.0/peek_office_app/src/favicon.ico`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/index.html` & `peek-office-app-3.4.0/peek_office_app/src/index.html`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/main.ts` & `peek-office-app-3.4.0/peek_office_app/src/main.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/polyfills.ts` & `peek-office-app-3.4.0/peek_office_app/src/polyfills.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/styles/shared.scss` & `peek-office-app-3.4.0/peek_office_app/src/styles/shared.scss`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/styles/theme.less` & `peek-office-app-3.4.0/peek_office_app/src/styles/theme.less`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/styles.scss` & `peek-office-app-3.4.0/peek_office_app/src/styles.scss`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/test.ts` & `peek-office-app-3.4.0/peek_office_app/src/test.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app/src/tsconfig.app.json` & `peek-office-app-3.4.0/peek_office_app/src/tsconfig.app.json`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/peek_office_app.egg-info/SOURCES.txt` & `peek-office-app-3.4.0/peek_office_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.3.3/setup.py` & `peek-office-app-3.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_office_app"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.3.3"
+package_version = "3.4.0"
 description = "Peek Office UI App."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

