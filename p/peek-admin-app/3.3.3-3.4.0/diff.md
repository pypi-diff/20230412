# Comparing `tmp/peek-admin-app-3.3.3.tar.gz` & `tmp/peek-admin-app-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-admin-app-3.3.3.tar", last modified: Mon Nov 14 05:35:12 2022, max compression
+gzip compressed data, was "peek-admin-app-3.4.0.tar", last modified: Wed Apr 12 11:04:00 2023, max compression
```

## Comparing `peek-admin-app-3.3.3.tar` & `peek-admin-app-3.4.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:12.377577 peek-admin-app-3.3.3/
--rw-r--r--   0 root         (0) root         (0)      376 2022-11-14 05:35:12.376577 peek-admin-app-3.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1015 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:12.374577 peek-admin-app-3.3.3/peek_admin_app/
--rw-r--r--   0 root         (0) root         (0)      487 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/.browserslistrc
--rw-r--r--   0 root         (0) root         (0)       69 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/.gitignore
--rw-r--r--   0 root         (0) root         (0)      460 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)     1084 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/README.md
--rw-r--r--   0 root         (0) root         (0)       22 2022-11-14 05:35:12.000000 peek-admin-app-3.3.3/peek_admin_app/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6385 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/angular.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:12.374577 peek-admin-app-3.3.3/peek_admin_app/e2e/
--rw-r--r--   0 root         (0) root         (0)      332 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/e2e/app.e2e-spec.ts
--rw-r--r--   0 root         (0) root         (0)      229 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/e2e/app.po.ts
--rw-r--r--   0 root         (0) root         (0)      367 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/e2e/tsconfig.e2e.json
--rw-r--r--   0 root         (0) root         (0)     1341 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/karma.conf.js
--rw-r--r--   0 root         (0) root         (0)   675654 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/package-lock.json
--rw-r--r--   0 root         (0) root         (0)     2900 2022-11-14 05:35:12.000000 peek-admin-app-3.3.3/peek_admin_app/package.json
--rw-r--r--   0 root         (0) root         (0)      868 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/protractor.conf.js
--rw-r--r--   0 root         (0) root         (0)      641 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/proxy.conf.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:12.375577 peek-admin-app-3.3.3/peek_admin_app/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:12.375577 peek-admin-app-3.3.3/peek_admin_app/src/app/
--rw-r--r--   0 root         (0) root         (0)      999 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app/app-routing.module.ts
--rw-r--r--   0 root         (0) root         (0)      174 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app/app.component.html
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app/app.component.scss
--rw-r--r--   0 root         (0) root         (0)     1080 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app/app.component.spec.ts
--rw-r--r--   0 root         (0) root         (0)     1101 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app/app.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:12.375577 peek-admin-app-3.3.3/peek_admin_app/src/app/dashboard/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:12.376577 peek-admin-app-3.3.3/peek_admin_app/src/app/dashboard/dashboard-stats/
--rw-r--r--   0 root         (0) root         (0)      598 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app/dashboard/dashboard-stats/dashboard-stats.component.html
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app/dashboard/dashboard-stats/dashboard-stats.component.scss
--rw-r--r--   0 root         (0) root         (0)      765 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app/dashboard/dashboard-stats/dashboard-stats.component.spec.ts
--rw-r--r--   0 root         (0) root         (0)     1303 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app/dashboard/dashboard-stats/dashboard-stats.component.ts
--rw-r--r--   0 root         (0) root         (0)      208 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app/dashboard/dashboard.component.html
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app/dashboard/dashboard.component.scss
--rw-r--r--   0 root         (0) root         (0)      729 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app/dashboard/dashboard.component.spec.ts
--rw-r--r--   0 root         (0) root         (0)      220 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app/dashboard/dashboard.component.ts
--rw-r--r--   0 root         (0) root         (0)      379 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app/dashboard/dashboard.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:12.376577 peek-admin-app-3.3.3/peek_admin_app/src/app/navbar/
--rw-r--r--   0 root         (0) root         (0)     5843 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app/navbar/navbar.component.html
--rw-r--r--   0 root         (0) root         (0)      127 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app/navbar/navbar.component.scss
--rw-r--r--   0 root         (0) root         (0)      708 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app/navbar/navbar.component.spec.ts
--rw-r--r--   0 root         (0) root         (0)     2529 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app/navbar/navbar.component.ts
--rw-r--r--   0 root         (0) root         (0)      489 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app/navbar/navbar.module.ts
--rw-r--r--   0 root         (0) root         (0)      222 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app/plugin-root.component.ts
--rw-r--r--   0 root         (0) root         (0)     2243 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/app.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:12.376577 peek-admin-app-3.3.3/peek_admin_app/src/assets/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/assets/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:12.376577 peek-admin-app-3.3.3/peek_admin_app/src/environments/
--rw-r--r--   0 root         (0) root         (0)       54 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/environments/environment.prod.ts
--rw-r--r--   0 root         (0) root         (0)      390 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/environments/environment.ts
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-14 05:35:12.000000 peek-admin-app-3.3.3/peek_admin_app/src/environments/peek-app-environment.ts
--rw-r--r--   0 root         (0) root         (0)     5430 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/favicon.ico
--rw-r--r--   0 root         (0) root         (0)     4931 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/index.html
--rw-r--r--   0 root         (0) root         (0)      696 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/main.ts
--rw-r--r--   0 root         (0) root         (0)     2395 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/polyfills.ts
--rw-r--r--   0 root         (0) root         (0)       90 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/styles.scss
--rw-r--r--   0 root         (0) root         (0)     1090 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/test.ts
--rw-r--r--   0 root         (0) root         (0)      521 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/tsconfig.app.json
--rw-r--r--   0 root         (0) root         (0)      242 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/tsconfig.spec.json
--rw-r--r--   0 root         (0) root         (0)      101 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/typings.d.ts
--rw-r--r--   0 root         (0) root         (0)       43 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/src/variables.scss
--rw-r--r--   0 root         (0) root         (0)      414 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/tsconfig.json
--rw-r--r--   0 root         (0) root         (0)      320 2022-11-14 05:34:26.000000 peek-admin-app-3.3.3/peek_admin_app/tsconfig.worker.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:12.374577 peek-admin-app-3.3.3/peek_admin_app.egg-info/
--rw-r--r--   0 root         (0) root         (0)      376 2022-11-14 05:35:12.000000 peek-admin-app-3.3.3/peek_admin_app.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2411 2022-11-14 05:35:12.000000 peek-admin-app-3.3.3/peek_admin_app.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:35:12.000000 peek-admin-app-3.3.3/peek_admin_app.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:35:12.000000 peek-admin-app-3.3.3/peek_admin_app.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       32 2022-11-14 05:35:12.000000 peek-admin-app-3.3.3/peek_admin_app.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-11-14 05:35:12.000000 peek-admin-app-3.3.3/peek_admin_app.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-14 05:35:12.377577 peek-admin-app-3.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3103 2022-11-14 05:35:12.000000 peek-admin-app-3.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:00.392217 peek-admin-app-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)      376 2023-04-12 11:04:00.392217 peek-admin-app-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:00.389217 peek-admin-app-3.4.0/peek_admin_app/
+-rw-r--r--   0 root         (0) root         (0)      487 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/.browserslistrc
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/README.md
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-12 11:04:00.000000 peek-admin-app-3.4.0/peek_admin_app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6385 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/angular.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:00.390217 peek-admin-app-3.4.0/peek_admin_app/e2e/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/e2e/app.e2e-spec.ts
+-rw-r--r--   0 root         (0) root         (0)      229 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/e2e/app.po.ts
+-rw-r--r--   0 root         (0) root         (0)      367 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/e2e/tsconfig.e2e.json
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/karma.conf.js
+-rw-r--r--   0 root         (0) root         (0)   675654 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/package-lock.json
+-rw-r--r--   0 root         (0) root         (0)     2900 2023-04-12 11:04:00.000000 peek-admin-app-3.4.0/peek_admin_app/package.json
+-rw-r--r--   0 root         (0) root         (0)      868 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/protractor.conf.js
+-rw-r--r--   0 root         (0) root         (0)      641 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/proxy.conf.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:00.391217 peek-admin-app-3.4.0/peek_admin_app/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:00.391217 peek-admin-app-3.4.0/peek_admin_app/src/app/
+-rw-r--r--   0 root         (0) root         (0)      999 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app/app-routing.module.ts
+-rw-r--r--   0 root         (0) root         (0)      174 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app/app.component.html
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app/app.component.scss
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app/app.component.spec.ts
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app/app.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:00.391217 peek-admin-app-3.4.0/peek_admin_app/src/app/dashboard/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:00.391217 peek-admin-app-3.4.0/peek_admin_app/src/app/dashboard/dashboard-stats/
+-rw-r--r--   0 root         (0) root         (0)      598 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app/dashboard/dashboard-stats/dashboard-stats.component.html
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app/dashboard/dashboard-stats/dashboard-stats.component.scss
+-rw-r--r--   0 root         (0) root         (0)      765 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app/dashboard/dashboard-stats/dashboard-stats.component.spec.ts
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app/dashboard/dashboard-stats/dashboard-stats.component.ts
+-rw-r--r--   0 root         (0) root         (0)      208 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app/dashboard/dashboard.component.html
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app/dashboard/dashboard.component.scss
+-rw-r--r--   0 root         (0) root         (0)      729 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app/dashboard/dashboard.component.spec.ts
+-rw-r--r--   0 root         (0) root         (0)      220 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app/dashboard/dashboard.component.ts
+-rw-r--r--   0 root         (0) root         (0)      379 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app/dashboard/dashboard.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:00.392217 peek-admin-app-3.4.0/peek_admin_app/src/app/navbar/
+-rw-r--r--   0 root         (0) root         (0)     5844 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app/navbar/navbar.component.html
+-rw-r--r--   0 root         (0) root         (0)      127 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app/navbar/navbar.component.scss
+-rw-r--r--   0 root         (0) root         (0)      708 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app/navbar/navbar.component.spec.ts
+-rw-r--r--   0 root         (0) root         (0)     2529 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app/navbar/navbar.component.ts
+-rw-r--r--   0 root         (0) root         (0)      489 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app/navbar/navbar.module.ts
+-rw-r--r--   0 root         (0) root         (0)      222 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app/plugin-root.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2243 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/app.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:00.392217 peek-admin-app-3.4.0/peek_admin_app/src/assets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/assets/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:00.392217 peek-admin-app-3.4.0/peek_admin_app/src/environments/
+-rw-r--r--   0 root         (0) root         (0)       54 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/environments/environment.prod.ts
+-rw-r--r--   0 root         (0) root         (0)      390 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/environments/environment.ts
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-12 11:04:00.000000 peek-admin-app-3.4.0/peek_admin_app/src/environments/peek-app-environment.ts
+-rw-r--r--   0 root         (0) root         (0)     5430 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)     4931 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/index.html
+-rw-r--r--   0 root         (0) root         (0)      696 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/main.ts
+-rw-r--r--   0 root         (0) root         (0)     2395 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/polyfills.ts
+-rw-r--r--   0 root         (0) root         (0)       90 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/styles.scss
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/test.ts
+-rw-r--r--   0 root         (0) root         (0)      521 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/tsconfig.app.json
+-rw-r--r--   0 root         (0) root         (0)      242 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/tsconfig.spec.json
+-rw-r--r--   0 root         (0) root         (0)      101 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/typings.d.ts
+-rw-r--r--   0 root         (0) root         (0)       43 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/src/variables.scss
+-rw-r--r--   0 root         (0) root         (0)      414 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/tsconfig.json
+-rw-r--r--   0 root         (0) root         (0)      320 2023-04-12 11:03:17.000000 peek-admin-app-3.4.0/peek_admin_app/tsconfig.worker.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:00.390217 peek-admin-app-3.4.0/peek_admin_app.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      376 2023-04-12 11:04:00.000000 peek-admin-app-3.4.0/peek_admin_app.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2411 2023-04-12 11:04:00.000000 peek-admin-app-3.4.0/peek_admin_app.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:04:00.000000 peek-admin-app-3.4.0/peek_admin_app.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:04:00.000000 peek-admin-app-3.4.0/peek_admin_app.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-12 11:04:00.000000 peek-admin-app-3.4.0/peek_admin_app.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-12 11:04:00.000000 peek-admin-app-3.4.0/peek_admin_app.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 11:04:00.392217 peek-admin-app-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3103 2023-04-12 11:04:00.000000 peek-admin-app-3.4.0/setup.py
```

### Comparing `peek-admin-app-3.3.3/README.rst` & `peek-admin-app-3.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/README.md` & `peek-admin-app-3.4.0/peek_admin_app/README.md`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/angular.json` & `peek-admin-app-3.4.0/peek_admin_app/angular.json`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/karma.conf.js` & `peek-admin-app-3.4.0/peek_admin_app/karma.conf.js`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/package-lock.json` & `peek-admin-app-3.4.0/peek_admin_app/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999852406902816%*

 * *Differences: {"'dependencies'": "{'@synerty/vortexjs': {'version': '3.3.3', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@synerty/vortexjs/-/vortexjs-3.3.3.tgz', "*

 * *                   "'integrity': "*

 * *                   "'sha512-SE4PvtrpdAVfwarFAYJkAzpiwjFyxDhdnQxS8C2y2vN1mLV5yE1J7mPExOyQIMwXFbCdO+GtUHuBgpIk+WVUDg==', "*

 * *                   "'dependencies': {'tslib': {'version': '2.5.0', 'resolved': "*

 * *                   "'https://registry.npmjs.org/tslib/-/tslib-2.5.0.tgz', 'integrity': "*

 * *                   […]*

```diff
@@ -2253,25 +2253,25 @@
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

### Comparing `peek-admin-app-3.3.3/peek_admin_app/package.json` & `peek-admin-app-3.4.0/peek_admin_app/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9225983076157293%*

 * *Differences: {"'dependencies'": "{'@synerty/vortexjs': '^3.3.3'}",*

 * * "'scripts'": "{'start': 'ng serve --host 3.4.0.0 --port 4010 --proxy-config proxy.conf.json'}",*

 * * "'version'": "'3.4.0'"}*

```diff
@@ -21,15 +21,15 @@
         "@capacitor/dialog": "^1.0.7",
         "@capacitor/geolocation": "^1.3.1",
         "@capacitor/ios": "^3.5.1",
         "@capacitor/local-notifications": "^1.1.0",
         "@capacitor/network": "^1.0.7",
         "@ionic/pwa-elements": "^3.1.1",
         "@synerty/peek-plugin-base-js": "^10.7.10",
-        "@synerty/vortexjs": "^3.2.5",
+        "@synerty/vortexjs": "^3.3.3",
         "base-64": "^0.1.0",
         "bootstrap": "^3.3.7",
         "brace": "^0.11.1",
         "cordova-plugin-nativeaudio": "^3.0.9",
         "core-js": "^3.6.5",
         "jquery": "^3.3.1",
         "json-stable-stringify": "^1.0.1",
@@ -69,12 +69,12 @@
     "private": true,
     "scripts": {
         "build": "ng build",
         "e2e": "ng e2e",
         "lint": "ng lint",
         "ng": "ng",
         "postinstall": "ngcc --properties es2015 es5 browser module main --first-only --create-ivy-entry-points",
-        "start": "ng serve --host 3.3.3.0 --port 4010 --proxy-config proxy.conf.json",
+        "start": "ng serve --host 3.4.0.0 --port 4010 --proxy-config proxy.conf.json",
         "test": "ng test"
     },
-    "version": "3.3.3"
+    "version": "3.4.0"
 }
```

### Comparing `peek-admin-app-3.3.3/peek_admin_app/protractor.conf.js` & `peek-admin-app-3.4.0/peek_admin_app/protractor.conf.js`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/proxy.conf.json` & `peek-admin-app-3.4.0/peek_admin_app/proxy.conf.json`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/src/app/app-routing.module.ts` & `peek-admin-app-3.4.0/peek_admin_app/src/app/app-routing.module.ts`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/src/app/app.component.spec.ts` & `peek-admin-app-3.4.0/peek_admin_app/src/app/app.component.spec.ts`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/src/app/app.component.ts` & `peek-admin-app-3.4.0/peek_admin_app/src/app/app.component.ts`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/src/app/dashboard/dashboard-stats/dashboard-stats.component.html` & `peek-admin-app-3.4.0/peek_admin_app/src/app/dashboard/dashboard-stats/dashboard-stats.component.html`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/src/app/dashboard/dashboard-stats/dashboard-stats.component.spec.ts` & `peek-admin-app-3.4.0/peek_admin_app/src/app/dashboard/dashboard-stats/dashboard-stats.component.spec.ts`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/src/app/dashboard/dashboard-stats/dashboard-stats.component.ts` & `peek-admin-app-3.4.0/peek_admin_app/src/app/dashboard/dashboard-stats/dashboard-stats.component.ts`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/src/app/dashboard/dashboard.component.spec.ts` & `peek-admin-app-3.4.0/peek_admin_app/src/app/dashboard/dashboard.component.spec.ts`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/src/app/navbar/navbar.component.html` & `peek-admin-app-3.4.0/peek_admin_app/src/app/navbar/navbar.component.html`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             <!-- Collect the nav links, forms, and other content for toggling -->
             <div
                 class="collapse navbar-collapse"
                 id="bs-example-navbar-collapse-1"
             >
                 <ul class="nav navbar-nav">
                     <li>
-                        <a href="/docs/index.html" target="_self">
+                        <a href="/docs/index.html" target="_blank">
                             <i
                                 nz-icon
                                 nzTheme="outline"
                                 nzType="question-circle"
                             ></i>
                         </a>
                     </li>
```

### Comparing `peek-admin-app-3.3.3/peek_admin_app/src/app/navbar/navbar.component.spec.ts` & `peek-admin-app-3.4.0/peek_admin_app/src/app/navbar/navbar.component.spec.ts`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/src/app/navbar/navbar.component.ts` & `peek-admin-app-3.4.0/peek_admin_app/src/app/navbar/navbar.component.ts`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/src/app.module.ts` & `peek-admin-app-3.4.0/peek_admin_app/src/app.module.ts`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/src/favicon.ico` & `peek-admin-app-3.4.0/peek_admin_app/src/favicon.ico`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/src/index.html` & `peek-admin-app-3.4.0/peek_admin_app/src/index.html`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/src/main.ts` & `peek-admin-app-3.4.0/peek_admin_app/src/main.ts`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/src/polyfills.ts` & `peek-admin-app-3.4.0/peek_admin_app/src/polyfills.ts`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/src/test.ts` & `peek-admin-app-3.4.0/peek_admin_app/src/test.ts`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app/src/tsconfig.app.json` & `peek-admin-app-3.4.0/peek_admin_app/src/tsconfig.app.json`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/peek_admin_app.egg-info/SOURCES.txt` & `peek-admin-app-3.4.0/peek_admin_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-admin-app-3.3.3/setup.py` & `peek-admin-app-3.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_admin_app"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.3.3"
+package_version = "3.4.0"
 description = "Peek Plugin ENAMC Email Incidents."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

