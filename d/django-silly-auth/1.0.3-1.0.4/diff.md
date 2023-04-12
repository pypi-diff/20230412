# Comparing `tmp/django-silly-auth-1.0.3.tar.gz` & `tmp/django-silly-auth-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-silly-auth-1.0.3.tar", last modified: Tue Apr 11 19:05:34 2023, max compression
+gzip compressed data, was "django-silly-auth-1.0.4.tar", last modified: Wed Apr 12 17:32:44 2023, max compression
```

## Comparing `django-silly-auth-1.0.3.tar` & `django-silly-auth-1.0.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.828432 django-silly-auth-1.0.3/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-auth-1.0.3/LICENSE.md
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1591 2023-04-11 19:05:34.828432 django-silly-auth-1.0.3/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      981 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/README.md
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.820432 django-silly-auth-1.0.3/django_silly_auth/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       51 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4732 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/config.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     6302 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/forms.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.820432 django-silly-auth-1.0.3/django_silly_auth/locale/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    10296 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/locale/django.pot
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.816431 django-silly-auth-1.0.3/django_silly_auth/locale/en/
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.820432 django-silly-auth-1.0.3/django_silly_auth/locale/en/LC_MESSAGES/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      337 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    10310 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.816431 django-silly-auth-1.0.3/django_silly_auth/locale/fr/
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.824432 django-silly-auth-1.0.3/django_silly_auth/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     9766 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    15445 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2473 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/mixins.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     5326 2023-04-11 18:50:34.000000 django-silly-auth-1.0.3/django_silly_auth/serializers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.824432 django-silly-auth-1.0.3/django_silly_auth/templates/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      141 2023-04-10 01:52:00.000000 django-silly-auth-1.0.3/django_silly_auth/templates/__init__.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.824432 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      152 2023-04-10 01:52:00.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      512 2023-04-04 22:34:28.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/_base.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.824432 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/_test/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/_test/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4497 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/_test/_base.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      193 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/_test/_test.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      276 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/_test/_users.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.824432 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      161 2023-04-10 01:52:00.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      621 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/account.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      598 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/change_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      613 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/change_username.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      388 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/index.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1156 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/login.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      570 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/request_password_reset.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      583 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      870 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/reset_password.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1147 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/signup.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.828432 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/emails/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/emails/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      300 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/emails/confirm_email.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      311 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/emails/request_password_reset.txt
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.828432 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/silly/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:52:00.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/silly/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      497 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/silly/silly_confirm_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4565 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/urls.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3256 2023-04-11 18:51:15.000000 django-silly-auth-1.0.3/django_silly_auth/utils.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.828432 django-silly-auth-1.0.3/django_silly_auth/views/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      137 2023-04-10 01:52:00.000000 django-silly-auth-1.0.3/django_silly_auth/views/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3066 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/views/api_custom_login.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      325 2023-04-10 01:52:00.000000 django-silly-auth-1.0.3/django_silly_auth/views/api_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     5459 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/views/api_views_if_drf.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    13685 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/views/classics.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1775 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/views/silly_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      985 2023-04-10 01:52:00.000000 django-silly-auth-1.0.3/django_silly_auth/views/test_views.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.820432 django-silly-auth-1.0.3/django_silly_auth.egg-info/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1591 2023-04-11 19:05:34.000000 django-silly-auth-1.0.3/django_silly_auth.egg-info/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2294 2023-04-11 19:05:34.000000 django-silly-auth-1.0.3/django_silly_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-11 19:05:34.000000 django-silly-auth-1.0.3/django_silly_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       13 2023-04-11 19:05:34.000000 django-silly-auth-1.0.3/django_silly_auth.egg-info/requires.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       18 2023-04-11 19:05:34.000000 django-silly-auth-1.0.3/django_silly_auth.egg-info/top_level.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-11 19:05:34.828432 django-silly-auth-1.0.3/setup.cfg
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2193 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/setup.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.881113 django-silly-auth-1.0.4/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-auth-1.0.4/LICENSE.md
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1591 2023-04-12 17:32:44.881113 django-silly-auth-1.0.4/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      981 2023-04-11 19:05:08.000000 django-silly-auth-1.0.4/README.md
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.869113 django-silly-auth-1.0.4/django_silly_auth/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       51 2023-04-12 17:32:02.000000 django-silly-auth-1.0.4/django_silly_auth/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4859 2023-04-12 17:32:02.000000 django-silly-auth-1.0.4/django_silly_auth/config.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     6302 2023-04-11 19:05:08.000000 django-silly-auth-1.0.4/django_silly_auth/forms.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.873113 django-silly-auth-1.0.4/django_silly_auth/locale/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    10584 2023-04-12 17:32:02.000000 django-silly-auth-1.0.4/django_silly_auth/locale/django.pot
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.861112 django-silly-auth-1.0.4/django_silly_auth/locale/en/
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.873113 django-silly-auth-1.0.4/django_silly_auth/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      337 2023-04-11 19:05:08.000000 django-silly-auth-1.0.4/django_silly_auth/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    10598 2023-04-12 17:32:02.000000 django-silly-auth-1.0.4/django_silly_auth/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.861112 django-silly-auth-1.0.4/django_silly_auth/locale/fr/
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.873113 django-silly-auth-1.0.4/django_silly_auth/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    10108 2023-04-12 17:32:02.000000 django-silly-auth-1.0.4/django_silly_auth/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    15877 2023-04-12 17:32:02.000000 django-silly-auth-1.0.4/django_silly_auth/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2473 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/mixins.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5953 2023-04-12 17:32:02.000000 django-silly-auth-1.0.4/django_silly_auth/serializers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.873113 django-silly-auth-1.0.4/django_silly_auth/templates/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      141 2023-04-10 01:52:00.000000 django-silly-auth-1.0.4/django_silly_auth/templates/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.873113 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      152 2023-04-10 01:52:00.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      512 2023-04-04 22:34:28.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/_base.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.873113 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/_test/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/_test/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4497 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/_test/_base.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      193 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/_test/_test.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      276 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/_test/_users.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.877113 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      161 2023-04-10 01:52:00.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      621 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/account.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      598 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/change_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      613 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/change_username.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      388 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/index.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1156 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/login.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      570 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/request_password_reset.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      583 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      870 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/reset_password.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1147 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/signup.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.877113 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/emails/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/emails/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      300 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/emails/confirm_email.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      311 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/emails/request_password_reset.txt
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.877113 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/silly/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:52:00.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/silly/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      497 2023-04-11 19:05:08.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/silly/silly_confirm_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5003 2023-04-12 17:32:02.000000 django-silly-auth-1.0.4/django_silly_auth/urls.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3256 2023-04-11 18:51:15.000000 django-silly-auth-1.0.4/django_silly_auth/utils.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.881113 django-silly-auth-1.0.4/django_silly_auth/views/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      137 2023-04-10 01:52:00.000000 django-silly-auth-1.0.4/django_silly_auth/views/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3066 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/views/api_custom_login.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      325 2023-04-10 01:52:00.000000 django-silly-auth-1.0.4/django_silly_auth/views/api_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     6476 2023-04-12 17:32:02.000000 django-silly-auth-1.0.4/django_silly_auth/views/api_views_if_drf.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    13685 2023-04-11 19:05:08.000000 django-silly-auth-1.0.4/django_silly_auth/views/classics.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1775 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/views/silly_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      985 2023-04-10 01:52:00.000000 django-silly-auth-1.0.4/django_silly_auth/views/test_views.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.873113 django-silly-auth-1.0.4/django_silly_auth.egg-info/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1591 2023-04-12 17:32:44.000000 django-silly-auth-1.0.4/django_silly_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2294 2023-04-12 17:32:44.000000 django-silly-auth-1.0.4/django_silly_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-12 17:32:44.000000 django-silly-auth-1.0.4/django_silly_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       13 2023-04-12 17:32:44.000000 django-silly-auth-1.0.4/django_silly_auth.egg-info/requires.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       18 2023-04-12 17:32:44.000000 django-silly-auth-1.0.4/django_silly_auth.egg-info/top_level.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-12 17:32:44.881113 django-silly-auth-1.0.4/setup.cfg
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2193 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/setup.py
```

### Comparing `django-silly-auth-1.0.3/LICENSE.md` & `django-silly-auth-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.3/PKG-INFO` & `django-silly-auth-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silly-auth
-Version: 1.0.3
+Version: 1.0.4
 Summary: Authentication package for Django and DRF
 Home-page: https://github.com/byoso/django_silly_auth
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: django auth drf jwt
 Platform: UNKNOWN
```

### Comparing `django-silly-auth-1.0.3/README.md` & `django-silly-auth-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.3/django_silly_auth/config.py` & `django-silly-auth-1.0.4/django_silly_auth/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     "CLASSIC_RESET_PASSWORD": "silly_auth/classic/reset_password.html",
     "CLASSIC_REQUEST_RESEND_ACCOUNT_CONFIRMATION_EMAIL": "silly_auth/classic/request_resend_account_confirmation_email.html",
 
     # DRF settings
     "USE_DRF": False,  # False for only classic django views
     "CONFIRMATION_METHOD": 'GET',  # 'GET' or 'POST'
     "ALLOW_CREATE_USER_ENDPOINT": True,  # activate this endpoint
+    "ALLOW_MY_INFOS_ENDPOINT": True,  # activate this endpoint
+    "ALLOW_DELETE_ME_ENDPOINT": True,  # activate this endpoint
 
     # pure SPA only:
     "SPA_EMAIL_LOGIN_LINK": "http://your spa adress/",  # + <jwt_token>",
 
 
     # Silly settings
     "USE_SILLY": False,
```

### Comparing `django-silly-auth-1.0.3/django_silly_auth/forms.py` & `django-silly-auth-1.0.4/django_silly_auth/forms.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.3/django_silly_auth/locale/django.pot` & `django-silly-auth-1.0.4/django_silly_auth/locale/django.pot`

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
-"POT-Creation-Date: 2023-04-11 21:00+0200\n"
+"POT-Creation-Date: 2023-04-12 19:04+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -43,15 +43,15 @@
 msgid "Confirm password"
 msgstr ""
 
 #: forms.py:88
 msgid "different than password"
 msgstr ""
 
-#: forms.py:94 forms.py:181 mixins.py:76 serializers.py:44
+#: forms.py:94 forms.py:181 mixins.py:76 serializers.py:44 serializers.py:183
 msgid "A username cannot include the symbol '@'."
 msgstr ""
 
 #: forms.py:99 forms.py:186
 #, python-format
 msgid "'%(username)s' is already taken by someone else."
 msgstr ""
@@ -123,14 +123,18 @@
 msgid "The given token does not match the user"
 msgstr ""
 
 #: serializers.py:163
 msgid "jwt token invalid or expired"
 msgstr ""
 
+#: serializers.py:180
+msgid "This username is already associated with an existing account."
+msgstr ""
+
 #: templates/silly_auth/_test/_base.html:29
 #: templates/silly_auth/classic/index.html:9
 msgid "Home"
 msgstr ""
 
 #: templates/silly_auth/_test/_base.html:34
 #: templates/silly_auth/classic/account.html:9
@@ -343,59 +347,67 @@
 
 #: views/api_custom_login.py:72
 msgid ""
 "You've been logged in via email confirmation, please change your password if "
 "necessary."
 msgstr ""
 
-#: views/api_views_if_drf.py:39
+#: views/api_views_if_drf.py:40
 msgid "no credential provided"
 msgstr ""
 
-#: views/api_views_if_drf.py:47 views/classics.py:362
+#: views/api_views_if_drf.py:48 views/classics.py:362
 msgid "Your account is already confirmed."
 msgstr ""
 
-#: views/api_views_if_drf.py:51 views/api_views_if_drf.py:81
+#: views/api_views_if_drf.py:52 views/api_views_if_drf.py:82
 msgid "Email sent for password reset"
 msgstr ""
 
-#: views/api_views_if_drf.py:63
+#: views/api_views_if_drf.py:64
 msgid "Logged out."
 msgstr ""
 
-#: views/api_views_if_drf.py:73
+#: views/api_views_if_drf.py:74
 msgid "No credentials were provided"
 msgstr ""
 
-#: views/api_views_if_drf.py:82
+#: views/api_views_if_drf.py:83
 msgid "Invalid credential"
 msgstr ""
 
-#: views/api_views_if_drf.py:99
+#: views/api_views_if_drf.py:100
 #, python-format
 msgid "Please check your inbox at '%(email)s' to confirm your account. "
 msgstr ""
 
-#: views/api_views_if_drf.py:103
+#: views/api_views_if_drf.py:104
 #, python-format
 msgid ""
 "If you do not confirm your account within the next %(hours)s hours, it will "
 "be deleted."
 msgstr ""
 
-#: views/api_views_if_drf.py:136
+#: views/api_views_if_drf.py:137
 msgid "Password successfully changed."
 msgstr ""
 
-#: views/api_views_if_drf.py:155
+#: views/api_views_if_drf.py:156
 #, python-format
 msgid "New email saved, check your inbox at '%(new_email)s' to activate it."
 msgstr ""
 
+#: views/api_views_if_drf.py:176
+msgid "Username successfully changed."
+msgstr ""
+
+#: views/api_views_if_drf.py:194
+msgid "Account successfully deleted."
+msgstr ""
+
 #: views/classics.py:58
 msgid "Incorrect credentials or unconfirmed account."
 msgstr ""
 
 #: views/classics.py:107
 #, python-format
 msgid "Please check your inbox at '%(email)s' to confirm your account."
```

### Comparing `django-silly-auth-1.0.3/django_silly_auth/locale/en/LC_MESSAGES/django.po` & `django-silly-auth-1.0.4/django_silly_auth/locale/en/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Vincent Fabre <peigne.plume@gmail.com>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-11 21:00+0200\n"
+"POT-Creation-Date: 2023-04-12 19:04+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -43,15 +43,15 @@
 msgid "Confirm password"
 msgstr ""
 
 #: forms.py:88
 msgid "different than password"
 msgstr ""
 
-#: forms.py:94 forms.py:181 mixins.py:76 serializers.py:44
+#: forms.py:94 forms.py:181 mixins.py:76 serializers.py:44 serializers.py:183
 msgid "A username cannot include the symbol '@'."
 msgstr ""
 
 #: forms.py:99 forms.py:186
 #, python-format
 msgid "'%(username)s' is already taken by someone else."
 msgstr ""
@@ -123,14 +123,18 @@
 msgid "The given token does not match the user"
 msgstr ""
 
 #: serializers.py:163
 msgid "jwt token invalid or expired"
 msgstr ""
 
+#: serializers.py:180
+msgid "This username is already associated with an existing account."
+msgstr ""
+
 #: templates/silly_auth/_test/_base.html:29
 #: templates/silly_auth/classic/index.html:9
 msgid "Home"
 msgstr ""
 
 #: templates/silly_auth/_test/_base.html:34
 #: templates/silly_auth/classic/account.html:9
@@ -343,59 +347,67 @@
 
 #: views/api_custom_login.py:72
 msgid ""
 "You've been logged in via email confirmation, please change your password if "
 "necessary."
 msgstr ""
 
-#: views/api_views_if_drf.py:39
+#: views/api_views_if_drf.py:40
 msgid "no credential provided"
 msgstr ""
 
-#: views/api_views_if_drf.py:47 views/classics.py:362
+#: views/api_views_if_drf.py:48 views/classics.py:362
 msgid "Your account is already confirmed."
 msgstr ""
 
-#: views/api_views_if_drf.py:51 views/api_views_if_drf.py:81
+#: views/api_views_if_drf.py:52 views/api_views_if_drf.py:82
 msgid "Email sent for password reset"
 msgstr ""
 
-#: views/api_views_if_drf.py:63
+#: views/api_views_if_drf.py:64
 msgid "Logged out."
 msgstr ""
 
-#: views/api_views_if_drf.py:73
+#: views/api_views_if_drf.py:74
 msgid "No credentials were provided"
 msgstr ""
 
-#: views/api_views_if_drf.py:82
+#: views/api_views_if_drf.py:83
 msgid "Invalid credential"
 msgstr ""
 
-#: views/api_views_if_drf.py:99
+#: views/api_views_if_drf.py:100
 #, python-format
 msgid "Please check your inbox at '%(email)s' to confirm your account. "
 msgstr ""
 
-#: views/api_views_if_drf.py:103
+#: views/api_views_if_drf.py:104
 #, python-format
 msgid ""
 "If you do not confirm your account within the next %(hours)s hours, it will "
 "be deleted."
 msgstr ""
 
-#: views/api_views_if_drf.py:136
+#: views/api_views_if_drf.py:137
 msgid "Password successfully changed."
 msgstr ""
 
-#: views/api_views_if_drf.py:155
+#: views/api_views_if_drf.py:156
 #, python-format
 msgid "New email saved, check your inbox at '%(new_email)s' to activate it."
 msgstr ""
 
+#: views/api_views_if_drf.py:176
+msgid "Username successfully changed."
+msgstr ""
+
+#: views/api_views_if_drf.py:194
+msgid "Account successfully deleted."
+msgstr ""
+
 #: views/classics.py:58
 msgid "Incorrect credentials or unconfirmed account."
 msgstr ""
 
 #: views/classics.py:107
 #, python-format
 msgid "Please check your inbox at '%(email)s' to confirm your account."
```

### Comparing `django-silly-auth-1.0.3/django_silly_auth/locale/fr/LC_MESSAGES/django.mo` & `django-silly-auth-1.0.4/django_silly_auth/locale/fr/LC_MESSAGES/django.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-04-11 21:01+0200\n"
+"PO-Revision-Date: 2023-04-12 19:06+0200\n"
 "Last-Translator: Vincent Fabre <peigne.plume@gmail.com>\n"
 "Language-Team: \n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
@@ -107,14 +107,17 @@
 
 msgid "Account"
 msgstr "Compte"
 
 msgid "Account Confirmation"
 msgstr "Confirmation du compte"
 
+msgid "Account successfully deleted."
+msgstr "Compte utilisateur supprimé avec succès."
+
 msgid "Buy me a coffee"
 msgstr "Offrez-moi un café"
 
 msgid "Change Email"
 msgstr "Changer d'email"
 
 msgid "Change Username"
@@ -280,14 +283,17 @@
 
 msgid "The passwords you entered do not match."
 msgstr "Les mots de passe saisis ne correspondent pas."
 
 msgid "This email is already associated with an existing account."
 msgstr "Cet email est déjà associé à un compte existant."
 
+msgid "This username is already associated with an existing account."
+msgstr "Ce nom d'utilisateur est déjà associé à un compte existant."
+
 msgid "Token invalid or expired"
 msgstr "Token invalide ou expiré"
 
 msgid "User '%(credential)s' unknown or unconfirmed"
 msgstr "Utilisateur '%(credential)s' inconnu ou non confirmé"
 
 msgid "User not found"
@@ -302,14 +308,17 @@
 msgid "Username must contain only letters, digits and ./+/-/_ characters."
 msgstr ""
 "Un nom d'utilisateur ne doit contenir que des lettres, nombres, ou +/-/_/."
 
 msgid "Username or email"
 msgstr "Nom d'utilisateur ou email"
 
+msgid "Username successfully changed."
+msgstr "Nom d'utilisateur changé avec succès."
+
 msgid ""
 "You have been logged in via email confirmation. Please reset your password."
 msgstr ""
 "Vous avez été connecté via un email de confirmation. Réinitialisez votre mot "
 "de passe si besoin."
 
 msgid ""
```

### Comparing `django-silly-auth-1.0.3/django_silly_auth/locale/fr/LC_MESSAGES/django.po` & `django-silly-auth-1.0.4/django_silly_auth/locale/fr/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # This file is distributed under the same license as the django-silly-auth package.
 # Vincent Fabre <peigne.plume@gmail.com>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-11 21:00+0200\n"
-"PO-Revision-Date: 2023-04-11 21:01+0200\n"
+"POT-Creation-Date: 2023-04-12 19:04+0200\n"
+"PO-Revision-Date: 2023-04-12 19:06+0200\n"
 "Last-Translator: Vincent Fabre <peigne.plume@gmail.com>\n"
 "Language-Team: \n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
@@ -44,15 +44,15 @@
 msgid "Confirm password"
 msgstr "Confirmez le mot de passe"
 
 #: forms.py:88
 msgid "different than password"
 msgstr "mots de passe différents"
 
-#: forms.py:94 forms.py:181 mixins.py:76 serializers.py:44
+#: forms.py:94 forms.py:181 mixins.py:76 serializers.py:44 serializers.py:183
 msgid "A username cannot include the symbol '@'."
 msgstr "Un nom d'utilisateur ne peut pas inclure '@'."
 
 #: forms.py:99 forms.py:186
 #, python-format
 msgid "'%(username)s' is already taken by someone else."
 msgstr "'%(username)s' est déjà utilisé par quelqu'un."
@@ -125,14 +125,18 @@
 msgid "The given token does not match the user"
 msgstr "Le token fourni ne correspond pas à l'utilisateur"
 
 #: serializers.py:163
 msgid "jwt token invalid or expired"
 msgstr "le token jwt est invalide ou expiré"
 
+#: serializers.py:180
+msgid "This username is already associated with an existing account."
+msgstr "Ce nom d'utilisateur est déjà associé à un compte existant."
+
 #: templates/silly_auth/_test/_base.html:29
 #: templates/silly_auth/classic/index.html:9
 msgid "Home"
 msgstr "Accueil"
 
 #: templates/silly_auth/_test/_base.html:34
 #: templates/silly_auth/classic/account.html:9
@@ -378,65 +382,73 @@
 #: views/api_custom_login.py:72
 msgid ""
 "You've been logged in via email confirmation, please change your password if "
 "necessary."
 msgstr ""
 "Connexion par email de confirmation, changez votre mot de passe si besoin."
 
-#: views/api_views_if_drf.py:39
+#: views/api_views_if_drf.py:40
 msgid "no credential provided"
 msgstr "aucun identifiant fourni"
 
-#: views/api_views_if_drf.py:47 views/classics.py:362
+#: views/api_views_if_drf.py:48 views/classics.py:362
 msgid "Your account is already confirmed."
 msgstr "Votre compte est déjà confirmé."
 
-#: views/api_views_if_drf.py:51 views/api_views_if_drf.py:81
+#: views/api_views_if_drf.py:52 views/api_views_if_drf.py:82
 msgid "Email sent for password reset"
 msgstr "Email envoyé pour réinitialisation du mot de passe"
 
-#: views/api_views_if_drf.py:63
+#: views/api_views_if_drf.py:64
 msgid "Logged out."
 msgstr "Déconnexion."
 
-#: views/api_views_if_drf.py:73
+#: views/api_views_if_drf.py:74
 msgid "No credentials were provided"
 msgstr "Aucun identifiant fourni"
 
-#: views/api_views_if_drf.py:82
+#: views/api_views_if_drf.py:83
 msgid "Invalid credential"
 msgstr "Identifiant non valide"
 
-#: views/api_views_if_drf.py:99
+#: views/api_views_if_drf.py:100
 #, python-format
 msgid "Please check your inbox at '%(email)s' to confirm your account. "
 msgstr ""
 "Veuillez consulter votre boite mail à '%(email)s' pour confirmer votre "
 "compte. "
 
-#: views/api_views_if_drf.py:103
+#: views/api_views_if_drf.py:104
 #, python-format
 msgid ""
 "If you do not confirm your account within the next %(hours)s hours, it will "
 "be deleted."
 msgstr ""
 "Si vous ne confirmez pas votre compte dans les %(hours)s heures, il sera "
 "supprimé."
 
-#: views/api_views_if_drf.py:136
+#: views/api_views_if_drf.py:137
 msgid "Password successfully changed."
 msgstr "Mot de passe changé avec succès."
 
-#: views/api_views_if_drf.py:155
+#: views/api_views_if_drf.py:156
 #, python-format
 msgid "New email saved, check your inbox at '%(new_email)s' to activate it."
 msgstr ""
 "Nouvel email enregistré, veuillez vérifier votre boite de réception à "
 "'%(new_email)s' pour l'activer."
 
+#: views/api_views_if_drf.py:176
+msgid "Username successfully changed."
+msgstr "Nom d'utilisateur changé avec succès."
+
+#: views/api_views_if_drf.py:194
+msgid "Account successfully deleted."
+msgstr "Compte utilisateur supprimé avec succès."
+
 #: views/classics.py:58
 msgid "Incorrect credentials or unconfirmed account."
 msgstr "Identifiants incorrects ou compte non confirmé."
 
 #: views/classics.py:107
 #, python-format
 msgid "Please check your inbox at '%(email)s' to confirm your account."
```

### Comparing `django-silly-auth-1.0.3/django_silly_auth/mixins.py` & `django-silly-auth-1.0.4/django_silly_auth/mixins.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.3/django_silly_auth/serializers.py` & `django-silly-auth-1.0.4/django_silly_auth/serializers.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 User = get_user_model()
 
 
 class GetAllUsersSerializer(serializers.ModelSerializer):
     class Meta:
         model = User
-        fields = ('id', 'username', 'email')
+        fields = '__all__'
 
 
 class CreateUserSerializer(serializers.ModelSerializer):
     class Meta:
         model = User
         fields = ('id', 'username', 'email', 'password')
 
@@ -162,7 +162,27 @@
         if User.verify_jwt_token(jwt_token) is None:
             jwt_errors += [_("jwt token invalid or expired")]
         if jwt_errors:
             errors['jwt_token'] = jwt_errors
         if errors:
             raise serializers.ValidationError(errors)
         return data
+
+
+class UsernameSerializer(serializers.Serializer):
+    username = serializers.CharField()
+
+    def validate(self, data):
+        username = data.get('username')
+        errors = dict()
+        username_errors = list()
+
+        if User.objects.filter(username=username).exists():
+            username_errors += [_("This username is already associated with an existing account."), ]
+
+        if "@" in username:
+            username_errors += [_("A username cannot include the symbol '@'."), ]
+
+        if username_errors:
+            errors['username'] = username_errors
+            raise serializers.ValidationError(errors)
+        return data
```

### Comparing `django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/_base.html` & `django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/_base.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/_test/_base.html` & `django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/_test/_base.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/account.html` & `django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/account.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/change_email.html` & `django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/change_email.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/change_username.html` & `django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/change_username.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/login.html` & `django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/login.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/request_password_reset.html` & `django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/request_password_reset.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html` & `django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/reset_password.html` & `django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/reset_password.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/signup.html` & `django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/signup.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.3/django_silly_auth/urls.py` & `django-silly-auth-1.0.4/django_silly_auth/urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,23 +53,35 @@
         ),
         path(
             f'{prefix}password/change/',
             api_views.change_password,
             name='change_password'
         ),
         path(
+            f'{prefix}username/change/',
+            api_views.change_username,
+            name='change_username'
+        ),
+        path(
             f'{prefix}email/request_change/',
             api_views.change_email_request,
             name='change_email_request'
         ),
         ]
 
+    if conf["ALLOW_DELETE_ME_ENDPOINT"]:
+        urlpatterns += [
+            path(f'{prefix}users/delete_me/', api_views.delete_me, name='delete_me'),
+        ]
+
     if conf["ALLOW_CREATE_USER_ENDPOINT"]:
         urlpatterns += [path(f'{prefix}users/', api_views.UserView.as_view(), name="users")]
 
+    if conf['ALLOW_MY_INFOS_ENDPOINT']:
+        urlpatterns += [path(f'{prefix}users/my_infos/', api_views.my_infos, name="my_infos")]
 
 # Classic routes
 
 if conf["USE_CLASSIC"]:
     urlpatterns += [
         path(f'{prefix}classic_login/', classics.login_view, name='classic_login'),
         path(f'{prefix}classic_logout/', classics.logout_view, name='classic_logout'),
```

### Comparing `django-silly-auth-1.0.3/django_silly_auth/utils.py` & `django-silly-auth-1.0.4/django_silly_auth/utils.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.3/django_silly_auth/views/api_custom_login.py` & `django-silly-auth-1.0.4/django_silly_auth/views/api_custom_login.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.3/django_silly_auth/views/api_views_if_drf.py` & `django-silly-auth-1.0.4/django_silly_auth/views/api_views_if_drf.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     )
 
 from django_silly_auth.serializers import (
     GetAllUsersSerializer,
     CreateUserSerializer,
     PasswordsSerializer,
     EmailSerializer,
+    UsernameSerializer,
     )
 from django_silly_auth.config import SILLY_AUTH_SETTINGS as conf
 from django_silly_auth.utils import (
     send_password_reset_email,
     send_confirm_email,
     delete_unconfirmed
 )
@@ -154,7 +155,40 @@
             {'success': _(
                 "New email saved, check your inbox at '%(new_email)s' "
                 "to activate it."
             ) % {'new_email': new_email}}
         )
     msg = serializer.errors
     raise ValidationError({"error": msg}, code='authorization')
+
+
+
+@transaction.atomic
+@api_view(['POST'])
+@permission_classes([IsAuthenticated])
+def change_username(request):
+    """Changes the user's username"""
+    serializer = UsernameSerializer(data=request.data)
+    if serializer.is_valid():
+        user = request.user
+        username = request.data.get('username')
+        user.username = username
+        user.save()
+        return Response({'success': _('Username successfully changed.')})
+    msg = serializer.errors
+    raise ValidationError({"error": msg}, code='authorization')
+
+
+@api_view(['GET'])
+@permission_classes([IsAuthenticated])
+def my_infos(request):
+    """Returns the user's infos"""
+    serializer = GetAllUsersSerializer(request.user)
+    return Response(serializer.data)
+
+@api_view(['DELETE'])
+@permission_classes([IsAuthenticated])
+def delete_me(request):
+    """Deletes the user's account"""
+    request.user.auth_token.delete()
+    request.user.delete()
+    return Response({'success': _('Account successfully deleted.')})
```

### Comparing `django-silly-auth-1.0.3/django_silly_auth/views/classics.py` & `django-silly-auth-1.0.4/django_silly_auth/views/classics.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.3/django_silly_auth/views/silly_views.py` & `django-silly-auth-1.0.4/django_silly_auth/views/silly_views.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.3/django_silly_auth/views/test_views.py` & `django-silly-auth-1.0.4/django_silly_auth/views/test_views.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.3/django_silly_auth.egg-info/PKG-INFO` & `django-silly-auth-1.0.4/django_silly_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silly-auth
-Version: 1.0.3
+Version: 1.0.4
 Summary: Authentication package for Django and DRF
 Home-page: https://github.com/byoso/django_silly_auth
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: django auth drf jwt
 Platform: UNKNOWN
```

### Comparing `django-silly-auth-1.0.3/django_silly_auth.egg-info/SOURCES.txt` & `django-silly-auth-1.0.4/django_silly_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.3/setup.py` & `django-silly-auth-1.0.4/setup.py`

 * *Files identical despite different names*

