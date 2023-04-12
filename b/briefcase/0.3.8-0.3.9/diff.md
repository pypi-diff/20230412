# Comparing `tmp/briefcase-0.3.8.tar.gz` & `tmp/briefcase-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "briefcase-0.3.8.tar", last modified: Mon Jun 27 03:23:25 2022, max compression
+gzip compressed data, was "briefcase-0.3.9.tar", last modified: Wed Aug 17 00:59:19 2022, max compression
```

## Comparing `briefcase-0.3.8.tar` & `briefcase-0.3.9.tar`

### file list

```diff
@@ -1,443 +1,493 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.996881 briefcase-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-06-27 03:22:32.000000 briefcase-0.3.8/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-06-27 03:22:32.000000 briefcase-0.3.8/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (121)      898 2022-06-27 03:22:32.000000 briefcase-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-06-27 03:22:32.000000 briefcase-0.3.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-06-27 03:22:32.000000 briefcase-0.3.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-06-27 03:22:32.000000 briefcase-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-06-27 03:22:32.000000 briefcase-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3913 2022-06-27 03:23:24.996881 briefcase-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2541 2022-06-27 03:22:32.000000 briefcase-0.3.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.936880 briefcase-0.3.8/changes/
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-27 03:22:32.000000 briefcase-0.3.8/changes/template.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.940880 briefcase-0.3.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.928880 briefcase-0.3.8/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.940880 briefcase-0.3.8/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (121)     7219 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/_static/images/briefcase.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.940880 briefcase-0.3.8/docs/background/
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/background/community.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1468 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/background/faq.rst
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/background/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12455 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/background/releases.rst
--rw-r--r--   0 runner    (1001) docker     (121)      543 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/background/success.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9787 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.940880 briefcase-0.3.8/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (121)  1055014 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/PyStackTraceOnXCode.png
--rw-r--r--   0 runner    (1001) docker     (121)     2767 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/access-packaging-metadata.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.944880 briefcase-0.3.8/docs/how-to/code-signing/
--rw-r--r--   0 runner    (1001) docker     (121)     3548 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/code-signing/android.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.948880 briefcase-0.3.8/docs/how-to/code-signing/images/
--rw-r--r--   0 runner    (1001) docker     (121)   143459 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/code-signing/images/AppleID.png
--rw-r--r--   0 runner    (1001) docker     (121)   368909 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/code-signing/images/Certificates_Identifiers_Profiles.png
--rw-r--r--   0 runner    (1001) docker     (121)   282602 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/code-signing/images/Choose_developerID_application.png
--rw-r--r--   0 runner    (1001) docker     (121)    37523 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/code-signing/images/Create_certificate.png
--rw-r--r--   0 runner    (1001) docker     (121)   119858 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/code-signing/images/Download_certificate.png
--rw-r--r--   0 runner    (1001) docker     (121)   199526 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/code-signing/images/Keychain_request1.png
--rw-r--r--   0 runner    (1001) docker     (121)   449585 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/code-signing/images/Keychain_request2.png
--rw-r--r--   0 runner    (1001) docker     (121)   295363 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/code-signing/images/Upload_certificate_request.png
--rw-r--r--   0 runner    (1001) docker     (121)    77619 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/code-signing/images/Valid_certificate.png
--rw-r--r--   0 runner    (1001) docker     (121)    88374 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/code-signing/images/WWDR_certificate.png
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/code-signing/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7278 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/code-signing/macOS.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12707 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/contribute-code.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/contribute-docs.rst
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.948880 briefcase-0.3.8/docs/how-to/internal/
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/internal/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3027 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/internal/release.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.948880 briefcase-0.3.8/docs/how-to/publishing/
--rw-r--r--   0 runner    (1001) docker     (121)    11214 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/publishing/android.rst
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/publishing/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/see_errors_on_ios.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8289 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/how-to/upgrade-from-v0.2.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      932 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.948880 briefcase-0.3.8/docs/reference/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.948880 briefcase-0.3.8/docs/reference/commands/
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/commands/build.rst
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/commands/create.rst
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/commands/dev.rst
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/commands/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/commands/new.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1619 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/commands/package.rst
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/commands/publish.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/commands/run.rst
--rw-r--r--   0 runner    (1001) docker     (121)      998 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/commands/update.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/commands/upgrade.rst
--rw-r--r--   0 runner    (1001) docker     (121)    14381 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.948880 briefcase-0.3.8/docs/reference/platforms/
--rw-r--r--   0 runner    (1001) docker     (121)     3238 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/platforms/android.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/platforms/iOS.rst
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/platforms/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.948880 briefcase-0.3.8/docs/reference/platforms/linux/
--rw-r--r--   0 runner    (1001) docker     (121)     8204 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/platforms/linux/appimage.rst
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/platforms/linux/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.948880 briefcase-0.3.8/docs/reference/platforms/macOS/
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/platforms/macOS/app.rst
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/platforms/macOS/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/platforms/macOS/xcode.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.952880 briefcase-0.3.8/docs/reference/platforms/windows/
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/platforms/windows/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2787 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/reference/platforms/windows/msi.rst
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/spelling_wordlist
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.952880 briefcase-0.3.8/docs/tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-06-27 03:22:32.000000 briefcase-0.3.8/docs/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-06-27 03:22:32.000000 briefcase-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-27 03:22:32.000000 briefcase-0.3.8/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-27 03:22:32.000000 briefcase-0.3.8/requirements.test.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2810 2022-06-27 03:23:24.996881 briefcase-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-06-27 03:22:32.000000 briefcase-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.932880 briefcase-0.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.952880 briefcase-0.3.8/src/briefcase/
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5874 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/cmdline.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.952880 briefcase-0.3.8/src/briefcase/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22107 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (121)    25160 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (121)     5245 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/commands/dev.py
--rw-r--r--   0 runner    (1001) docker     (121)    19215 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/commands/new.py
--rw-r--r--   0 runner    (1001) docker     (121)     3573 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/commands/package.py
--rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/commands/publish.py
--rw-r--r--   0 runner    (1001) docker     (121)     2229 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     2681 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (121)     3703 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/commands/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (121)    16225 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    18960 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/console.py
--rw-r--r--   0 runner    (1001) docker     (121)     3568 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.956880 briefcase-0.3.8/src/briefcase/integrations/
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    47438 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/integrations/android_sdk.py
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/integrations/cookiecutter.py
--rw-r--r--   0 runner    (1001) docker     (121)    10338 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/integrations/docker.py
--rw-r--r--   0 runner    (1001) docker     (121)     2157 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/integrations/git.py
--rw-r--r--   0 runner    (1001) docker     (121)     9957 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/integrations/java.py
--rw-r--r--   0 runner    (1001) docker     (121)     4865 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/integrations/linuxdeploy.py
--rw-r--r--   0 runner    (1001) docker     (121)    19835 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/integrations/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)     5392 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/integrations/wix.py
--rw-r--r--   0 runner    (1001) docker     (121)    18297 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/integrations/xcode.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.956880 briefcase-0.3.8/src/briefcase/platforms/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.956880 briefcase-0.3.8/src/briefcase/platforms/android/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/android/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9809 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/android/gradle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.956880 briefcase-0.3.8/src/briefcase/platforms/django/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/django/app.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/django/project.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.956880 briefcase-0.3.8/src/briefcase/platforms/iOS/
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/iOS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15673 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/iOS/xcode.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.960880 briefcase-0.3.8/src/briefcase/platforms/linux/
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8500 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/linux/appimage.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/linux/deb.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/linux/flatpak.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/linux/rpm.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/linux/snap.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.960880 briefcase-0.3.8/src/briefcase/platforms/macOS/
--rw-r--r--   0 runner    (1001) docker     (121)    23333 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/macOS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3189 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/macOS/app.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/macOS/homebrew.py
--rw-r--r--   0 runner    (1001) docker     (121)     3758 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/macOS/xcode.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.960880 briefcase-0.3.8/src/briefcase/platforms/tvOS/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/tvOS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/tvOS/xcode.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.960880 briefcase-0.3.8/src/briefcase/platforms/watchOS/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/watchOS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/watchOS/xcode.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.960880 briefcase-0.3.8/src/briefcase/platforms/wearos/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/wearos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/wearos/gradle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.960880 briefcase-0.3.8/src/briefcase/platforms/windows/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8849 2022-06-27 03:22:32.000000 briefcase-0.3.8/src/briefcase/platforms/windows/msi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.952880 briefcase-0.3.8/src/briefcase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3913 2022-06-27 03:23:23.000000 briefcase-0.3.8/src/briefcase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15124 2022-06-27 03:23:24.000000 briefcase-0.3.8/src/briefcase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-27 03:23:24.000000 briefcase-0.3.8/src/briefcase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-06-27 03:23:24.000000 briefcase-0.3.8/src/briefcase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-27 03:22:46.000000 briefcase-0.3.8/src/briefcase.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-06-27 03:23:24.000000 briefcase-0.3.8/src/briefcase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-06-27 03:23:24.000000 briefcase-0.3.8/src/briefcase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.960880 briefcase-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.960880 briefcase-0.3.8/tests/apps/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/apps/verify-ppb.config
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/apps/verify-pyside2.config
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/apps/verify-pyside6.config
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/apps/verify-toga.config
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.960880 briefcase-0.3.8/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.964880 briefcase-0.3.8/tests/commands/base/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3299 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/base/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2504 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/base/test_app_module_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     6939 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/base/test_download_url.py
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/base/test_full_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     6934 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/base/test_parse_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/base/test_parse_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     1758 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/base/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     5813 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/base/test_update_cookiecutter_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/base/test_verify_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.964880 briefcase-0.3.8/tests/commands/build/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3320 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/build/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     5950 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/build/test_call.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.964880 briefcase-0.3.8/tests/commands/create/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/create/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5474 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/create/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2694 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/create/test_call.py
--rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/create/test_cookiecutter_cache_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     5560 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/create/test_create_app.py
--rw-r--r--   0 runner    (1001) docker     (121)    15212 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/create/test_generate_app_template.py
--rw-r--r--   0 runner    (1001) docker     (121)    10180 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/create/test_install_app_code.py
--rw-r--r--   0 runner    (1001) docker     (121)     7440 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/create/test_install_app_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)     9881 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/create/test_install_app_resources.py
--rw-r--r--   0 runner    (1001) docker     (121)    10231 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/create/test_install_app_support_package.py
--rw-r--r--   0 runner    (1001) docker     (121)    10539 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/create/test_install_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     9725 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/create/test_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.968881 briefcase-0.3.8/tests/commands/dev/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2125 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/dev/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     6790 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/dev/test_call.py
--rw-r--r--   0 runner    (1001) docker     (121)      863 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/dev/test_get_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/dev/test_install_dev_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/dev/test_run_dev_app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.968881 briefcase-0.3.8/tests/commands/new/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/new/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/new/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/new/test_build_app_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/new/test_call.py
--rw-r--r--   0 runner    (1001) docker     (121)     2136 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/new/test_input_select.py
--rw-r--r--   0 runner    (1001) docker     (121)     2651 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/new/test_input_text.py
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/new/test_make_app_name.py
--rw-r--r--   0 runner    (1001) docker     (121)      620 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/new/test_make_author_email.py
--rw-r--r--   0 runner    (1001) docker     (121)     1702 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/new/test_make_class_name.py
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/new/test_make_domain.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/new/test_make_module_name.py
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/new/test_make_project_url.py
--rw-r--r--   0 runner    (1001) docker     (121)     3610 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/new/test_new_app.py
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/new/test_titlecase.py
--rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/new/test_validate_app_name.py
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/new/test_validate_bundle.py
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/new/test_validate_email.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/new/test_validate_url.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.968881 briefcase-0.3.8/tests/commands/package/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3978 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/package/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    13200 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/package/test_call.py
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/package/test_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.972880 briefcase-0.3.8/tests/commands/publish/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3688 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/publish/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2898 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/publish/test_call.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.972880 briefcase-0.3.8/tests/commands/run/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3798 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/run/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     6035 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/run/test_call.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.972880 briefcase-0.3.8/tests/commands/update/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2816 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/update/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2947 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/update/test_call.py
--rw-r--r--   0 runner    (1001) docker     (121)     3025 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/update/test_update_app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.972880 briefcase-0.3.8/tests/commands/upgrade/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/upgrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2086 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/upgrade/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     6152 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/commands/upgrade/test_call.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.972880 briefcase-0.3.8/tests/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7561 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/config/test_AppConfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     2014 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/config/test_GlobalConfig.py
--rw-r--r--   0 runner    (1001) docker     (121)    11438 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/config/test_is_pep440_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/config/test_is_reserved_keyword.py
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/config/test_is_valid_app_name.py
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/config/test_is_valid_bundle_identifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     2097 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/config/test_merge_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    14913 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/config/test_parse_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.972880 briefcase-0.3.8/tests/console/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.976880 briefcase-0.3.8/tests/console/Console/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/console/Console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2639 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/console/Console/test_boolean_input.py
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/console/Console/test_call.py
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/console/Console/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     1921 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/console/Console/test_selection_input.py
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/console/Console/test_text_input.py
--rw-r--r--   0 runner    (1001) docker     (121)     1442 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/console/Console/test_wait_bar.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/console/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4213 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/console/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/console/test_Printer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/console/test_select_option.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.976880 briefcase-0.3.8/tests/integrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.976880 briefcase-0.3.8/tests/integrations/android_sdk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.976880 briefcase-0.3.8/tests/integrations/android_sdk/ADB/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/ADB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.976880 briefcase-0.3.8/tests/integrations/android_sdk/ADB/adb_errors/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/ADB/adb_errors/arbitrary-adb-error-unknown-command.out
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/ADB/adb_errors/arbitrary-adb-error-unknown-command.returncode
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/ADB/adb_errors/device-not-found.out
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/ADB/adb_errors/device-not-found.returncode
--rw-r--r--   0 runner    (1001) docker     (121)     2034 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/ADB/test_avd_name.py
--rw-r--r--   0 runner    (1001) docker     (121)     1542 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/ADB/test_clear_log.py
--rw-r--r--   0 runner    (1001) docker     (121)     2499 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/ADB/test_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     2024 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/ADB/test_force_stop_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     1927 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/ADB/test_has_booted.py
--rw-r--r--   0 runner    (1001) docker     (121)     1811 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/ADB/test_install_apk.py
--rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/ADB/test_logcat.py
--rw-r--r--   0 runner    (1001) docker     (121)     2302 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/ADB/test_start_app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.980881 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.980881 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/devices/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/devices/daemon_start.out
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/devices/multiple_devices.out
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/devices/no_devices.out
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/devices/one_emulator.out
--rw-r--r--   0 runner    (1001) docker     (121)     2036 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_avd_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     6782 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_create_emulator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2306 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_emulators.py
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_list_packages.py
--rw-r--r--   0 runner    (1001) docker     (121)     4330 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     9215 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_select_target_device.py
--rw-r--r--   0 runner    (1001) docker     (121)    10174 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_start_emulator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2069 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_update_emulator_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      812 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (121)    18987 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_verify.py
--rw-r--r--   0 runner    (1001) docker     (121)     5552 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_verify_avd.py
--rw-r--r--   0 runner    (1001) docker     (121)     2181 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_verify_emulator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4537 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_verify_emulator_skin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2339 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_verify_license.py
--rw-r--r--   0 runner    (1001) docker     (121)     4395 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_verify_system_image.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/android_sdk/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.980881 briefcase-0.3.8/tests/integrations/docker/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/docker/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2091 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/docker/test_Docker__prepare.py
--rw-r--r--   0 runner    (1001) docker     (121)     4177 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/docker/test_Docker__run.py
--rw-r--r--   0 runner    (1001) docker     (121)     7062 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/docker/test_verify_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.980881 briefcase-0.3.8/tests/integrations/java/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/java/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14658 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/java/test_JDK__verify.py
--rw-r--r--   0 runner    (1001) docker     (121)     8486 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/java/test_JDK_upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.984881 briefcase-0.3.8/tests/integrations/linuxdeploy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/linuxdeploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3073 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/linuxdeploy/test_LinuxDeploy__patch_elf_binary.py
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/linuxdeploy/test_LinuxDeploy__properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     2936 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/linuxdeploy/test_LinuxDeploy__upgrade.py
--rw-r--r--   0 runner    (1001) docker     (121)     3369 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/linuxdeploy/test_LinuxDeploy__verify.py
--rw-r--r--   0 runner    (1001) docker     (121)     1390 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/linuxdeploy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.984881 briefcase-0.3.8/tests/integrations/subprocess/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/subprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1468 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/subprocess/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     5386 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/subprocess/test_Subprocess__Popen.py
--rw-r--r--   0 runner    (1001) docker     (121)     6855 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/subprocess/test_Subprocess__check_output.py
--rw-r--r--   0 runner    (1001) docker     (121)      985 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/subprocess/test_Subprocess__cleanup.py
--rw-r--r--   0 runner    (1001) docker     (121)     2278 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/subprocess/test_Subprocess__final_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3491 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/subprocess/test_Subprocess__parse_output.py
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/subprocess/test_Subprocess__prepare.py
--rw-r--r--   0 runner    (1001) docker     (121)     6218 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/subprocess/test_Subprocess__run.py
--rw-r--r--   0 runner    (1001) docker     (121)     6401 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/subprocess/test_Subprocess__run_in_wait_bar.py
--rw-r--r--   0 runner    (1001) docker     (121)     3286 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/subprocess/test_Subprocess__stream_output.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/subprocess/test_creationflag_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/subprocess/test_ensure_str.py
--rw-r--r--   0 runner    (1001) docker     (121)     3672 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/subprocess/test_get_process_id_by_command.py
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/subprocess/test_is_process_dead.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/subprocess/test_json_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.984881 briefcase-0.3.8/tests/integrations/wix/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/wix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5664 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/wix/test_WiX__upgrade.py
--rw-r--r--   0 runner    (1001) docker     (121)     7829 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/wix/test_WiX__verify.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.988880 briefcase-0.3.8/tests/integrations/xcode/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.988880 briefcase-0.3.8/tests/integrations/xcode/security/
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/security/multiple-identities.out
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/security/no-identities.out
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/security/one-identity.out
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.988880 briefcase-0.3.8/tests/integrations/xcode/simctl/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/simctl/README
--rw-r--r--   0 runner    (1001) docker     (121)    43417 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/simctl/alternate-format.json
--rw-r--r--   0 runner    (1001) docker     (121)   130449 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/simctl/iOS-13.2-only.json
--rw-r--r--   0 runner    (1001) docker     (121)   129789 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/simctl/multiple-iOS-versions.json
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/simctl/no-devices.json
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/simctl/no-runtimes.json
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/simctl/single-device-booted.json
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/simctl/single-device-shutdown.json
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/simctl/single-device-shutting-down.json
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/simctl/single-device-unknown.json
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/simctl/single-device.json
--rw-r--r--   0 runner    (1001) docker     (121)     4912 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/test_confirm_xcode_license_accepted.py
--rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/test_ensure_command_line_tools_are_installed.py
--rw-r--r--   0 runner    (1001) docker     (121)    14728 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/test_ensure_xcode_is_installed.py
--rw-r--r--   0 runner    (1001) docker     (121)     3145 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/test_get_device_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     2628 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/test_get_identities.py
--rw-r--r--   0 runner    (1001) docker     (121)    11223 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/integrations/xcode/test_get_simulators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.988880 briefcase-0.3.8/tests/platforms/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.988880 briefcase-0.3.8/tests/platforms/android/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/android/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.988880 briefcase-0.3.8/tests/platforms/android/gradle/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/android/gradle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2209 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/android/gradle/test_build.py
--rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/android/gradle/test_create.py
--rw-r--r--   0 runner    (1001) docker     (121)     2463 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/android/gradle/test_package.py
--rw-r--r--   0 runner    (1001) docker     (121)     5696 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/android/gradle/test_run.py
--rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/android/gradle/test_safe_formal_name.py
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/android/gradle/test_verify_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.992881 briefcase-0.3.8/tests/platforms/iOS/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/iOS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.992881 briefcase-0.3.8/tests/platforms/iOS/xcode/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/iOS/xcode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.992881 briefcase-0.3.8/tests/platforms/iOS/xcode/mixin/
--rw-r--r--   0 runner    (1001) docker     (121)    11723 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/iOS/xcode/mixin/test_select_target_device.py
--rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/iOS/xcode/test_build.py
--rw-r--r--   0 runner    (1001) docker     (121)      770 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/iOS/xcode/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/iOS/xcode/test_package.py
--rw-r--r--   0 runner    (1001) docker     (121)    21418 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/iOS/xcode/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.992881 briefcase-0.3.8/tests/platforms/linux/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/linux/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.992881 briefcase-0.3.8/tests/platforms/linux/appimage/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/linux/appimage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8838 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/linux/appimage/test_build.py
--rw-r--r--   0 runner    (1001) docker     (121)     3261 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/linux/appimage/test_create.py
--rw-r--r--   0 runner    (1001) docker     (121)     4824 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/linux/appimage/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2204 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/linux/appimage/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.992881 briefcase-0.3.8/tests/platforms/macOS/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/macOS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.992881 briefcase-0.3.8/tests/platforms/macOS/app/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/macOS/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1872 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/macOS/app/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/macOS/app/test_build.py
--rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/macOS/app/test_create.py
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/macOS/app/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)    21918 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/macOS/app/test_package.py
--rw-r--r--   0 runner    (1001) docker     (121)    14627 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/macOS/app/test_package__notarize.py
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/macOS/app/test_package__team_id_from_identity.py
--rw-r--r--   0 runner    (1001) docker     (121)     4768 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/macOS/app/test_run.py
--rw-r--r--   0 runner    (1001) docker     (121)    13422 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/macOS/app/test_signing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.996881 briefcase-0.3.8/tests/platforms/macOS/xcode/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/macOS/xcode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/macOS/xcode/test_build.py
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/macOS/xcode/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/macOS/xcode/test_package.py
--rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/macOS/xcode/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.996881 briefcase-0.3.8/tests/platforms/windows/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/windows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:23:24.996881 briefcase-0.3.8/tests/platforms/windows/msi/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/windows/msi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3415 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/windows/msi/test_create.py
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/windows/msi/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2604 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/windows/msi/test_package.py
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/platforms/windows/msi/test_run.py
--rw-r--r--   0 runner    (1001) docker     (121)    14689 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/test_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-06-27 03:22:32.000000 briefcase-0.3.8/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1594 2022-06-27 03:22:32.000000 briefcase-0.3.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.699344 briefcase-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2022-08-17 00:58:54.000000 briefcase-0.3.9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2022-08-17 00:58:54.000000 briefcase-0.3.9/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (121)      898 2022-08-17 00:58:54.000000 briefcase-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      344 2022-08-17 00:58:54.000000 briefcase-0.3.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (121)      422 2022-08-17 00:58:54.000000 briefcase-0.3.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-08-17 00:58:54.000000 briefcase-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      732 2022-08-17 00:58:54.000000 briefcase-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3913 2022-08-17 00:59:19.699344 briefcase-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2541 2022-08-17 00:58:54.000000 briefcase-0.3.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.551342 briefcase-0.3.9/changes/
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-17 00:58:54.000000 briefcase-0.3.9/changes/template.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.555342 briefcase-0.3.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      728 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.523342 briefcase-0.3.9/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.555342 briefcase-0.3.9/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (121)     7219 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/_static/images/briefcase.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.555342 briefcase-0.3.9/docs/background/
+-rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/background/community.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1468 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/background/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/background/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    14645 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/background/releases.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      543 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/background/success.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9787 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.559342 briefcase-0.3.9/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (121)  1055014 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/PyStackTraceOnXCode.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2767 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/access-packaging-metadata.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.559342 briefcase-0.3.9/docs/how-to/code-signing/
+-rw-r--r--   0 runner    (1001) docker     (121)     4081 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/code-signing/android.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.567342 briefcase-0.3.9/docs/how-to/code-signing/images/
+-rw-r--r--   0 runner    (1001) docker     (121)   143459 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/code-signing/images/AppleID.png
+-rw-r--r--   0 runner    (1001) docker     (121)   368909 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/code-signing/images/Certificates_Identifiers_Profiles.png
+-rw-r--r--   0 runner    (1001) docker     (121)   282602 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/code-signing/images/Choose_developerID_application.png
+-rw-r--r--   0 runner    (1001) docker     (121)    37523 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/code-signing/images/Create_certificate.png
+-rw-r--r--   0 runner    (1001) docker     (121)   119858 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/code-signing/images/Download_certificate.png
+-rw-r--r--   0 runner    (1001) docker     (121)   199526 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/code-signing/images/Keychain_request1.png
+-rw-r--r--   0 runner    (1001) docker     (121)   449585 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/code-signing/images/Keychain_request2.png
+-rw-r--r--   0 runner    (1001) docker     (121)   295363 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/code-signing/images/Upload_certificate_request.png
+-rw-r--r--   0 runner    (1001) docker     (121)    77619 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/code-signing/images/Valid_certificate.png
+-rw-r--r--   0 runner    (1001) docker     (121)    88374 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/code-signing/images/WWDR_certificate.png
+-rw-r--r--   0 runner    (1001) docker     (121)      595 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/code-signing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7278 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/code-signing/macOS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12707 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/contribute-code.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/contribute-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      534 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.567342 briefcase-0.3.9/docs/how-to/internal/
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/internal/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3027 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/internal/release.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.567342 briefcase-0.3.9/docs/how-to/publishing/
+-rw-r--r--   0 runner    (1001) docker     (121)    12248 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/publishing/android.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/publishing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      602 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/see_errors_on_ios.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8289 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/how-to/upgrade-from-v0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      932 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.571342 briefcase-0.3.9/docs/reference/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.575343 briefcase-0.3.9/docs/reference/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/commands/build.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/commands/create.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      874 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/commands/dev.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/commands/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/commands/new.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1619 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/commands/package.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      937 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/commands/publish.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/commands/run.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      998 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/commands/update.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/commands/upgrade.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    14407 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1016 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/environment.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.575343 briefcase-0.3.9/docs/reference/platforms/
+-rw-r--r--   0 runner    (1001) docker     (121)     3238 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/platforms/android.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/platforms/iOS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/platforms/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.575343 briefcase-0.3.9/docs/reference/platforms/linux/
+-rw-r--r--   0 runner    (1001) docker     (121)    10247 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/platforms/linux/appimage.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4519 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/platforms/linux/flatpak.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      269 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/platforms/linux/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.579342 briefcase-0.3.9/docs/reference/platforms/macOS/
+-rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/platforms/macOS/app.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/platforms/macOS/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/platforms/macOS/xcode.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.579342 briefcase-0.3.9/docs/reference/platforms/windows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2532 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/platforms/windows/app.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/platforms/windows/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3590 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/reference/platforms/windows/visualstudio.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/spelling_wordlist
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.579342 briefcase-0.3.9/docs/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (121)      521 2022-08-17 00:58:54.000000 briefcase-0.3.9/docs/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2022-08-17 00:58:54.000000 briefcase-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-17 00:58:54.000000 briefcase-0.3.9/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-17 00:58:54.000000 briefcase-0.3.9/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-08-17 00:59:19.699344 briefcase-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-08-17 00:58:54.000000 briefcase-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.527342 briefcase-0.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.583343 briefcase-0.3.9/src/briefcase/
+-rw-r--r--   0 runner    (1001) docker     (121)      368 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5874 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/cmdline.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.587343 briefcase-0.3.9/src/briefcase/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27221 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29706 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5678 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/commands/dev.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19215 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/commands/new.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3573 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/commands/package.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/commands/publish.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2229 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2681 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4519 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/commands/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16225 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19781 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/console.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3648 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.595343 briefcase-0.3.9/src/briefcase/integrations/
+-rw-r--r--   0 runner    (1001) docker     (121)      381 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    48302 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/integrations/android_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (121)      969 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/integrations/cookiecutter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11946 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/integrations/docker.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10314 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/integrations/flatpak.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2158 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/integrations/git.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9990 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/integrations/java.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12511 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/integrations/linuxdeploy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2088 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/integrations/rcedit.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20457 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/integrations/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5773 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/integrations/visualstudio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5403 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/integrations/wix.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18297 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/integrations/xcode.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.595343 briefcase-0.3.9/src/briefcase/platforms/
+-rw-r--r--   0 runner    (1001) docker     (121)      605 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.595343 briefcase-0.3.9/src/briefcase/platforms/android/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9825 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/android/gradle.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.595343 briefcase-0.3.9/src/briefcase/platforms/django/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/django/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/django/project.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.595343 briefcase-0.3.9/src/briefcase/platforms/iOS/
+-rw-r--r--   0 runner    (1001) docker     (121)      789 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/iOS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15673 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/iOS/xcode.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.599343 briefcase-0.3.9/src/briefcase/platforms/linux/
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10572 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/linux/appimage.py
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/linux/deb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7758 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/linux/flatpak.py
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/linux/rpm.py
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/linux/snap.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.599343 briefcase-0.3.9/src/briefcase/platforms/macOS/
+-rw-r--r--   0 runner    (1001) docker     (121)    23373 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/macOS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3189 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/macOS/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/macOS/homebrew.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3758 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/macOS/xcode.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.603343 briefcase-0.3.9/src/briefcase/platforms/tvOS/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/tvOS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/tvOS/xcode.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.603343 briefcase-0.3.9/src/briefcase/platforms/watchOS/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/watchOS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/watchOS/xcode.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.603343 briefcase-0.3.9/src/briefcase/platforms/wearos/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/wearos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/wearos/gradle.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.603343 briefcase-0.3.9/src/briefcase/platforms/windows/
+-rw-r--r--   0 runner    (1001) docker     (121)     7349 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3610 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/windows/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2903 2022-08-17 00:58:54.000000 briefcase-0.3.9/src/briefcase/platforms/windows/visualstudio.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.583343 briefcase-0.3.9/src/briefcase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3913 2022-08-17 00:59:19.000000 briefcase-0.3.9/src/briefcase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    17428 2022-08-17 00:59:19.000000 briefcase-0.3.9/src/briefcase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-17 00:59:19.000000 briefcase-0.3.9/src/briefcase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      776 2022-08-17 00:59:19.000000 briefcase-0.3.9/src/briefcase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-17 00:59:00.000000 briefcase-0.3.9/src/briefcase.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2022-08-17 00:59:19.000000 briefcase-0.3.9/src/briefcase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-17 00:59:19.000000 briefcase-0.3.9/src/briefcase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.607343 briefcase-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.607343 briefcase-0.3.9/tests/apps/
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/apps/verify-ppb.config
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/apps/verify-pyside2.config
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/apps/verify-pyside6.config
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/apps/verify-toga.config
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.607343 briefcase-0.3.9/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.611343 briefcase-0.3.9/tests/commands/base/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3299 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/base/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2504 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/base/test_app_module_path.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4612 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/base/test_check_obsolete_data_dir.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6939 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/base/test_download_url.py
+-rw-r--r--   0 runner    (1001) docker     (121)      602 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/base/test_full_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6934 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/base/test_parse_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/base/test_parse_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6077 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/base/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1758 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/base/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5813 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/base/test_update_cookiecutter_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/base/test_verify_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.611343 briefcase-0.3.9/tests/commands/build/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/build/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5962 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/build/test_call.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.615343 briefcase-0.3.9/tests/commands/create/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6414 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/create/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2694 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/create/test_call.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/create/test_cookiecutter_cache_path.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5560 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/create/test_create_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15332 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/create/test_generate_app_template.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10656 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/create/test_install_app_code.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14557 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/create/test_install_app_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11493 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/create/test_install_app_resources.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13881 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/create/test_install_app_support_package.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10634 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/create/test_install_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9725 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/create/test_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.627343 briefcase-0.3.9/tests/commands/dev/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2125 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/dev/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6790 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/dev/test_call.py
+-rw-r--r--   0 runner    (1001) docker     (121)      976 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/dev/test_get_environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/dev/test_install_dev_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1385 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/dev/test_run_dev_app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.631343 briefcase-0.3.9/tests/commands/new/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/new/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      840 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/new/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/new/test_build_app_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/new/test_call.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2136 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/new/test_input_select.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2651 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/new/test_input_text.py
+-rw-r--r--   0 runner    (1001) docker     (121)      824 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/new/test_make_app_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)      620 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/new/test_make_author_email.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1702 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/new/test_make_class_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/new/test_make_domain.py
+-rw-r--r--   0 runner    (1001) docker     (121)      458 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/new/test_make_module_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)      627 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/new/test_make_project_url.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3610 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/new/test_new_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)      708 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/new/test_titlecase.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/new/test_validate_app_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)      802 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/new/test_validate_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (121)      522 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/new/test_validate_email.py
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/new/test_validate_url.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.631343 briefcase-0.3.9/tests/commands/package/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3978 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/package/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13200 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/package/test_call.py
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/package/test_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.635343 briefcase-0.3.9/tests/commands/publish/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3688 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/publish/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2898 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/publish/test_call.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.635343 briefcase-0.3.9/tests/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3798 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/run/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6035 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/run/test_call.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.635343 briefcase-0.3.9/tests/commands/update/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2816 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/update/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2947 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/update/test_call.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3025 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/update/test_update_app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.635343 briefcase-0.3.9/tests/commands/upgrade/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/upgrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3242 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/upgrade/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6618 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/commands/upgrade/test_call.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.639343 briefcase-0.3.9/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7561 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/config/test_AppConfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2014 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/config/test_GlobalConfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11438 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/config/test_is_pep440_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/config/test_is_reserved_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (121)      733 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/config/test_is_valid_app_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/config/test_is_valid_bundle_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2097 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/config/test_merge_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14913 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/config/test_parse_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.639343 briefcase-0.3.9/tests/console/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.643344 briefcase-0.3.9/tests/console/Console/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/console/Console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2639 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/console/Console/test_boolean_input.py
+-rw-r--r--   0 runner    (1001) docker     (121)      938 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/console/Console/test_call.py
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/console/Console/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1921 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/console/Console/test_selection_input.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/console/Console/test_text_input.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3577 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/console/Console/test_wait_bar.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      328 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/console/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4213 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/console/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/console/test_Printer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/console/test_select_option.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.643344 briefcase-0.3.9/tests/integrations/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.643344 briefcase-0.3.9/tests/integrations/android_sdk/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.643344 briefcase-0.3.9/tests/integrations/android_sdk/ADB/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/ADB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.647343 briefcase-0.3.9/tests/integrations/android_sdk/ADB/adb_errors/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/ADB/adb_errors/arbitrary-adb-error-unknown-command.out
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/ADB/adb_errors/arbitrary-adb-error-unknown-command.returncode
+-rw-r--r--   0 runner    (1001) docker     (121)      213 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/ADB/adb_errors/device-not-found.out
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/ADB/adb_errors/device-not-found.returncode
+-rw-r--r--   0 runner    (1001) docker     (121)     2034 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/ADB/test_avd_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2499 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/ADB/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2024 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/ADB/test_force_stop_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1927 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/ADB/test_has_booted.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1811 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/ADB/test_install_apk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1831 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/ADB/test_logcat.py
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/ADB/test_pidof.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2302 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/ADB/test_start_app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.651344 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.651344 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/devices/
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/devices/daemon_start.out
+-rw-r--r--   0 runner    (1001) docker     (121)      379 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/devices/multiple_devices.out
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/devices/no_devices.out
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/devices/one_emulator.out
+-rw-r--r--   0 runner    (1001) docker     (121)     2086 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_avd_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6908 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_create_emulator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2306 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_emulators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_list_packages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4339 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9215 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_select_target_device.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10237 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_start_emulator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2094 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_update_emulator_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      812 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19115 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_verify.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5552 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_verify_avd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2181 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_verify_emulator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4537 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_verify_emulator_skin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2339 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_verify_license.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4395 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_verify_system_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      881 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/android_sdk/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.655344 briefcase-0.3.9/tests/integrations/docker/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1642 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/docker/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/docker/test_Docker___dockerize_path.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4506 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/docker/test_Docker__check_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2129 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/docker/test_Docker__prepare.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4185 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/docker/test_Docker__run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7062 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/docker/test_verify_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.655344 briefcase-0.3.9/tests/integrations/flatpak/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/flatpak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/flatpak/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/flatpak/test_Flatpak__build.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/flatpak/test_Flatpak__bundle.py
+-rw-r--r--   0 runner    (1001) docker     (121)      856 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/flatpak/test_Flatpak__run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7178 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/flatpak/test_Flatpak__verify.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/flatpak/test_Flatpak__verify_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1428 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/flatpak/test_Flatpak__verify_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.659344 briefcase-0.3.9/tests/integrations/java/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/java/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14658 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/java/test_JDK__verify.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8486 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/java/test_JDK_upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.659344 briefcase-0.3.9/tests/integrations/linuxdeploy/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/linuxdeploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/linuxdeploy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3123 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/linuxdeploy/test_LinuxDeployBase__patch_elf_binary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3245 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/linuxdeploy/test_LinuxDeployBase__upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4937 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/linuxdeploy/test_LinuxDeployBase__verify.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/linuxdeploy/test_LinuxDeployGtkPlugin__properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/linuxdeploy/test_LinuxDeployLocalFilePlugin__properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1689 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/linuxdeploy/test_LinuxDeployLocalFilePlugin__verify.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/linuxdeploy/test_LinuxDeployQtPlugin__properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/linuxdeploy/test_LinuxDeployURLPlugin__properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1941 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/linuxdeploy/test_LinuxDeployURLPlugin__verify.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/linuxdeploy/test_LinuxDeploy__properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8469 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/linuxdeploy/test_LinuxDeploy__verify_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/linuxdeploy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.663344 briefcase-0.3.9/tests/integrations/rcedit/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/rcedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/rcedit/test_RCEdit__properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2537 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/rcedit/test_RCEdit__upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2964 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/rcedit/test_RCEdit__verify.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.667344 briefcase-0.3.9/tests/integrations/subprocess/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/subprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1653 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/subprocess/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5646 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/subprocess/test_Subprocess__Popen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7168 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/subprocess/test_Subprocess__check_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)      983 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/subprocess/test_Subprocess__cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2278 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/subprocess/test_Subprocess__final_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3491 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/subprocess/test_Subprocess__parse_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/subprocess/test_Subprocess__prepare.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6531 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/subprocess/test_Subprocess__run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6948 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/subprocess/test_Subprocess__run_in_wait_bar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4133 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/subprocess/test_Subprocess__stream_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/subprocess/test_creationflag_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)      371 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/subprocess/test_ensure_str.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3672 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/subprocess/test_get_process_id_by_command.py
+-rw-r--r--   0 runner    (1001) docker     (121)      389 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/subprocess/test_is_process_dead.py
+-rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/subprocess/test_json_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.671344 briefcase-0.3.9/tests/integrations/visualstudio/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/visualstudio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/visualstudio/test_VisualStudio__properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15363 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/visualstudio/test_VisualStudio__verify.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.671344 briefcase-0.3.9/tests/integrations/wix/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/wix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5664 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/wix/test_WiX__upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7829 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/wix/test_WiX__verify.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.671344 briefcase-0.3.9/tests/integrations/xcode/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.675344 briefcase-0.3.9/tests/integrations/xcode/security/
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/security/multiple-identities.out
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/security/no-identities.out
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/security/one-identity.out
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.679344 briefcase-0.3.9/tests/integrations/xcode/simctl/
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/simctl/README
+-rw-r--r--   0 runner    (1001) docker     (121)    43417 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/simctl/alternate-format.json
+-rw-r--r--   0 runner    (1001) docker     (121)   130449 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/simctl/iOS-13.2-only.json
+-rw-r--r--   0 runner    (1001) docker     (121)   129789 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/simctl/multiple-iOS-versions.json
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/simctl/no-devices.json
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/simctl/no-runtimes.json
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/simctl/single-device-booted.json
+-rw-r--r--   0 runner    (1001) docker     (121)      374 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/simctl/single-device-shutdown.json
+-rw-r--r--   0 runner    (1001) docker     (121)      379 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/simctl/single-device-shutting-down.json
+-rw-r--r--   0 runner    (1001) docker     (121)      373 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/simctl/single-device-unknown.json
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/simctl/single-device.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4912 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/test_confirm_xcode_license_accepted.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/test_ensure_command_line_tools_are_installed.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14728 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/test_ensure_xcode_is_installed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3145 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/test_get_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2628 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/test_get_identities.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11223 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/integrations/xcode/test_get_simulators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.679344 briefcase-0.3.9/tests/platforms/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.679344 briefcase-0.3.9/tests/platforms/android/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/android/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.683344 briefcase-0.3.9/tests/platforms/android/gradle/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/android/gradle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2199 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/android/gradle/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/android/gradle/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2453 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/android/gradle/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6354 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/android/gradle/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/android/gradle/test_safe_formal_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/android/gradle/test_verify_tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)      722 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.683344 briefcase-0.3.9/tests/platforms/iOS/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/iOS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.683344 briefcase-0.3.9/tests/platforms/iOS/xcode/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/iOS/xcode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.683344 briefcase-0.3.9/tests/platforms/iOS/xcode/mixin/
+-rw-r--r--   0 runner    (1001) docker     (121)    11723 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/iOS/xcode/mixin/test_select_target_device.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/iOS/xcode/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (121)      770 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/iOS/xcode/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/iOS/xcode/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21418 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/iOS/xcode/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.683344 briefcase-0.3.9/tests/platforms/linux/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/linux/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.687344 briefcase-0.3.9/tests/platforms/linux/appimage/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/linux/appimage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15280 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/linux/appimage/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3163 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/linux/appimage/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4824 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/linux/appimage/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2546 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/linux/appimage/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.687344 briefcase-0.3.9/tests/platforms/linux/flatpak/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/linux/flatpak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/linux/flatpak/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2221 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/linux/flatpak/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5050 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/linux/flatpak/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      950 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/linux/flatpak/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/linux/flatpak/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.687344 briefcase-0.3.9/tests/platforms/macOS/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/macOS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.691344 briefcase-0.3.9/tests/platforms/macOS/app/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/macOS/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1872 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/macOS/app/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/macOS/app/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/macOS/app/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/macOS/app/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21918 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/macOS/app/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14627 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/macOS/app/test_package__notarize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/macOS/app/test_package__team_id_from_identity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5071 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/macOS/app/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13422 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/macOS/app/test_signing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.695344 briefcase-0.3.9/tests/platforms/macOS/xcode/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/macOS/xcode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/macOS/xcode/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/macOS/xcode/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/macOS/xcode/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/macOS/xcode/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.695344 briefcase-0.3.9/tests/platforms/windows/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/windows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.695344 briefcase-0.3.9/tests/platforms/windows/app/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/windows/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2408 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/windows/app/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3734 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/windows/app/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/windows/app/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2660 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/windows/app/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/windows/app/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 00:59:19.699344 briefcase-0.3.9/tests/platforms/windows/visualstudio/
+-rw-r--r--   0 runner    (1001) docker     (121)     1867 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/windows/visualstudio/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (121)      728 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/windows/visualstudio/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3000 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/windows/visualstudio/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/platforms/windows/visualstudio/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14689 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/test_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3236 2022-08-17 00:58:54.000000 briefcase-0.3.9/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1624 2022-08-17 00:58:54.000000 briefcase-0.3.9/tox.ini
```

### Comparing `briefcase-0.3.8/.pre-commit-config.yaml` & `briefcase-0.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/LICENSE` & `briefcase-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/MANIFEST.in` & `briefcase-0.3.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/PKG-INFO` & `briefcase-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: briefcase
-Version: 0.3.8
+Version: 0.3.9
 Summary: Tools to support converting a Python project into a standalone native application.
 Home-page: http://beeware.org/briefcase
 Author: Russell Keith-Magee
 Author-email: russell@keith-magee.com
 Maintainer: Russell Keith-Magee
 Maintainer-email: russell@keith-magee.com
 License: New BSD
```

### Comparing `briefcase-0.3.8/README.rst` & `briefcase-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/changes/template.rst` & `briefcase-0.3.9/changes/template.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/Makefile` & `briefcase-0.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/_static/images/briefcase.png` & `briefcase-0.3.9/docs/_static/images/briefcase.png`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/background/community.rst` & `briefcase-0.3.9/docs/background/community.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/background/faq.rst` & `briefcase-0.3.9/docs/background/faq.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/background/releases.rst` & `briefcase-0.3.9/docs/background/releases.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,64 @@
 ===============
 Release History
 ===============
 
 .. towncrier release notes start
 
+0.3.9 (2022-08-17)
+==================
+
+Features
+--------
+
+* Linux apps can now be packaged in Flatpak format. (#359)
+* SDKs, tools, and other downloads needed to support app builds are now stored
+  in an OS-native user cache directory instead of ``~/.briefcase``. (#374)
+* Windows MSI installers can now be configured to ask the user whether they want
+  a per-user or per-machine install. (#382)
+* The console output of Windows apps is now captured and displayed during
+  ``briefcase run``. (#620)
+* Windows apps are now packaged with a stub application. This ensures that
+  Windows apps present with the name and icon of the app, rather than the
+  ``pythonw.exe`` name and icon. It also allows for improvements in logging and
+  error handling. (#629)
+* Temporary docker containers are now cleaned up after use. The wording of
+  Docker progress messages has also been improved. (#774)
+* Users can now define a ``BRIEFCASE_HOME`` environment variable. This allows
+  you to specify the location of the Briefcase tool cache, allowing the user to
+  avoid issues with spaces in paths or disk space limitations. (#789)
+* Android emulator output is now printed to the console if it fails to start
+  properly. (#799)
+* ``briefcase android run`` now shows logs from only the current process, and
+  includes all log tags except some particularly noisy and useless ones. It also
+  no longer clears the Logcat buffer. (#814)
+
+
+Bugfixes
+--------
+
+* Apps now have better isolation against the current working directory. This
+  ensures that code in the current working directory isn't inadvertently
+  included when an app runs. (#662)
+* Windows MSI installers now install in ``Program Files``, rather than ``Program
+  Files (x86)``. (#688)
+* Linuxdeploy plugiuns can now be used when building Linux AppImages; this
+  resolves many issues with GTK app deployment. (#756)
+* Collision protection has been added to custom support packages that have the
+  same name, but are served by different URLs. (#797)
+* Python 3.7 and 3.8 on Windows will no longer deadlock when CTRL+C is sent
+  during a subprocess command. (#809)
+
+
+Misc
+----
+
+* #778, #783, #784, #785, #786, #787, #794, #800, #805, #810, #813, #815
+
+
 0.3.8 (2022-06-27)
 ==================
 
 Features
 --------
 
 * macOS apps are now notarized as part of the packaging process. (#365)
```

### Comparing `briefcase-0.3.8/docs/background/success.rst` & `briefcase-0.3.9/docs/background/success.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/conf.py` & `briefcase-0.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/how-to/PyStackTraceOnXCode.png` & `briefcase-0.3.9/docs/how-to/PyStackTraceOnXCode.png`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/how-to/access-packaging-metadata.rst` & `briefcase-0.3.9/docs/how-to/access-packaging-metadata.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/how-to/code-signing/android.rst` & `briefcase-0.3.9/docs/how-to/code-signing/android.rst`

 * *Files 11% similar despite different names*

```diff
@@ -44,29 +44,36 @@
 .. tabs::
 
   .. group-tab:: macOS
 
     .. code-block:: bash
 
       $ mkdir -p ~/.android
-      $ ~/.briefcase/tools/java/Contents/Home/bin/keytool -keyalg RSA -deststoretype pkcs12 -genkey -v -storepass android -keystore ~/.android/upload-key-helloworld.jks -keysize 2048 -dname "cn=Upload Key" -alias upload-key -validity 10000
+      $ ~/Library/Caches/org.beeware.briefcase/tools/java/Contents/Home/bin/keytool -keyalg RSA -deststoretype pkcs12 -genkey -v -storepass android -keystore ~/.android/upload-key-helloworld.jks -keysize 2048 -dname "cn=Upload Key" -alias upload-key -validity 10000
 
   .. group-tab:: Linux
 
     .. code-block:: bash
 
       $ mkdir -p ~/.android
-      $ ~/.briefcase/tools/java/bin/keytool -keyalg RSA -deststoretype pkcs12 -genkey -v -storepass android -keystore ~/.android/upload-key-helloworld.jks -keysize 2048 -dname "cn=Upload Key" -alias upload-key -validity 10000
+      $ ~/.cache/briefcase/tools/java/bin/keytool -keyalg RSA -deststoretype pkcs12 -genkey -v -storepass android -keystore ~/.android/upload-key-helloworld.jks -keysize 2048 -dname "cn=Upload Key" -alias upload-key -validity 10000
 
-  .. group-tab:: Windows
+  .. group-tab:: Windows (PowerShell)
+
+    .. code-block:: powershell
+
+      C:\...>If (-Not (Test-Path "$env:HOMEPATH/.android")) { New-Item -Path "$env:HOMEPATH\.android" -ItemType Directory }
+      C:\...>& "$env:LOCALAPPDATA\BeeWare\briefcase\Cache\tools\java\bin\keytool.exe" -keyalg RSA -deststoretype pkcs12 -genkey -v -storepass android -keystore "$env:HOMEPATH\.android\upload-key-helloworld.jks" -keysize 2048 -dname "cn=Upload Key" -alias upload-key -validity 10000
+
+  .. group-tab:: Windows (cmd)
 
     .. code-block:: doscon
 
       C:\...>IF not exist %HOMEPATH%\.android mkdir %HOMEPATH%\.android
-      C:\...>%HOMEPATH%\.briefcase\tools\java\bin\keytool.exe -keyalg RSA -deststoretype pkcs12 -genkey -v -storepass android -keystore %HOMEPATH%\.android\upload-key-helloworld.jks -keysize 2048 -dname "cn=Upload Key" -alias upload-key -validity 10000
+      C:\...>%LOCALAPPDATA%\BeeWare\briefcase\Cache\tools\java\bin\keytool.exe -keyalg RSA -deststoretype pkcs12 -genkey -v -storepass android -keystore %HOMEPATH%\.android\upload-key-helloworld.jks -keysize 2048 -dname "cn=Upload Key" -alias upload-key -validity 10000
 
 
 This creates a 2048-bit key and stores it in a Java keystore located in the
 ``.android`` folder within your home folder. Since the key's purpose is to be
 used as an upload key for the Google Play store, we call the key "upload-key".
 
 We use a password of ``android``. This is the `default password for common
```

### Comparing `briefcase-0.3.8/docs/how-to/code-signing/images/AppleID.png` & `briefcase-0.3.9/docs/how-to/code-signing/images/AppleID.png`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/how-to/code-signing/images/Certificates_Identifiers_Profiles.png` & `briefcase-0.3.9/docs/how-to/code-signing/images/Certificates_Identifiers_Profiles.png`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/how-to/code-signing/images/Choose_developerID_application.png` & `briefcase-0.3.9/docs/how-to/code-signing/images/Choose_developerID_application.png`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/how-to/code-signing/images/Create_certificate.png` & `briefcase-0.3.9/docs/how-to/code-signing/images/Create_certificate.png`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/how-to/code-signing/images/Download_certificate.png` & `briefcase-0.3.9/docs/how-to/code-signing/images/Download_certificate.png`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/how-to/code-signing/images/Keychain_request1.png` & `briefcase-0.3.9/docs/how-to/code-signing/images/Keychain_request1.png`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/how-to/code-signing/images/Keychain_request2.png` & `briefcase-0.3.9/docs/how-to/code-signing/images/Keychain_request2.png`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/how-to/code-signing/images/Upload_certificate_request.png` & `briefcase-0.3.9/docs/how-to/code-signing/images/Upload_certificate_request.png`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/how-to/code-signing/images/Valid_certificate.png` & `briefcase-0.3.9/docs/how-to/code-signing/images/Valid_certificate.png`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/how-to/code-signing/images/WWDR_certificate.png` & `briefcase-0.3.9/docs/how-to/code-signing/images/WWDR_certificate.png`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/how-to/code-signing/index.rst` & `briefcase-0.3.9/docs/how-to/code-signing/index.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/how-to/code-signing/macOS.rst` & `briefcase-0.3.9/docs/how-to/code-signing/macOS.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/how-to/contribute-code.rst` & `briefcase-0.3.9/docs/how-to/contribute-code.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/how-to/contribute-docs.rst` & `briefcase-0.3.9/docs/how-to/contribute-docs.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/how-to/index.rst` & `briefcase-0.3.9/docs/how-to/index.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/how-to/internal/release.rst` & `briefcase-0.3.9/docs/how-to/internal/release.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/how-to/publishing/android.rst` & `briefcase-0.3.9/docs/how-to/publishing/android.rst`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 .. tabs::
 
   .. group-tab:: macOS
 
     .. code-block::
 
-      $ ~/.briefcase/tools/java/Contents/Home/bin/jarsigner -verbose -sigalg SHA1withRSA -digestalg SHA1 -keystore ~/.android/upload-key-helloworld.jks "android/Hello World/app/build/outputs/bundle/release/app-release.aab" upload-key -storepass android
+      $ ~/Library/Caches/org.beeware.briefcase/tools/java/Contents/Home/bin/jarsigner -verbose -sigalg SHA1withRSA -digestalg SHA1 -keystore ~/.android/upload-key-helloworld.jks "android/gradle/Hello World/app/build/outputs/bundle/release/app-release.aab" upload-key -storepass android
          adding: META-INF/MANIFEST.MF
          adding: META-INF/UPLOAD-K.SF
          adding: META-INF/UPLOAD-K.RSA
         signing: BundleConfig.pb
         signing: BUNDLE-METADATA/com.android.tools.build.libraries/dependencies.pb
         signing: base/assets/python/app/README
       ...
@@ -97,15 +97,15 @@
       Warning:
       The signer's certificate is self-signed.
 
   .. group-tab:: Linux
 
     .. code-block::
 
-      $ ~/.briefcase/tools/java/bin/jarsigner -verbose -sigalg SHA1withRSA -digestalg SHA1 -keystore ~/.android/upload-key-helloworld.jks "android/Hello World/app/build/outputs/bundle/release/app-release.aab" upload-key -storepass android
+      $ ~/.cache/briefcase/tools/java/bin/jarsigner -verbose -sigalg SHA1withRSA -digestalg SHA1 -keystore ~/.android/upload-key-helloworld.jks "android/gradle/Hello World/app/build/outputs/bundle/release/app-release.aab" upload-key -storepass android
          adding: META-INF/MANIFEST.MF
          adding: META-INF/UPLOAD-K.SF
          adding: META-INF/UPLOAD-K.RSA
         signing: BundleConfig.pb
         signing: BUNDLE-METADATA/com.android.tools.build.libraries/dependencies.pb
         signing: base/assets/python/app/README
       ...
@@ -118,19 +118,44 @@
         [trusted certificate]
 
       jar signed.
 
       Warning:
       The signer's certificate is self-signed.
 
-  .. group-tab:: Windows
+  .. group-tab:: Windows (PowerShell)
+
+    .. code-block::
+
+      C:\...>& "$env:LOCALAPPDATA\BeeWare\briefcase\Cache\tools\java\bin\jarsigner.exe" -verbose -sigalg SHA1withRSA -digestalg SHA1 -keystore "$env:HOMEPATH\.android\upload-key-helloworld.jks" "android\gradle\Hello World\app\build\outputs\bundle\release\app-release.aab" upload-key -storepass android
+         adding: META-INF/MANIFEST.MF
+         adding: META-INF/UPLOAD-K.SF
+         adding: META-INF/UPLOAD-K.RSA
+        signing: BundleConfig.pb
+        signing: BUNDLE-METADATA/com.android.tools.build.libraries/dependencies.pb
+        signing: base/assets/python/app/README
+      ...
+        signing: base/manifest/AndroidManifest.xml
+        signing: base/assets.pb
+        signing: base/native.pb
+        signing: base/resources.pb
+      >>> Signer
+        X.509, CN=Upload Key
+        [trusted certificate]
+
+      jar signed.
+
+      Warning:
+      The signer's certificate is self-signed.
+
+  .. group-tab:: Windows (cmd)
 
     .. code-block:: doscon
 
-      C:\...> %HOMEPATH%\.briefcase\tools\java\bin\jarsigner.exe -verbose -sigalg SHA1withRSA -digestalg SHA1 -keystore %HOMEPATH%\.android\upload-key-helloworld.jks "android\Hello World\app\build\outputs\bundle\release\app-release.aab" upload-key -storepass android
+      C:\...>%LOCALAPPDATA%\BeeWare\briefcase\Cache\tools\java\bin\jarsigner.exe -verbose -sigalg SHA1withRSA -digestalg SHA1 -keystore %HOMEPATH%\.android\upload-key-helloworld.jks "android\gradle\Hello World\app\build\outputs\bundle\release\app-release.aab" upload-key -storepass android
          adding: META-INF/MANIFEST.MF
          adding: META-INF/UPLOAD-K.SF
          adding: META-INF/UPLOAD-K.RSA
         signing: BundleConfig.pb
         signing: BUNDLE-METADATA/com.android.tools.build.libraries/dependencies.pb
         signing: base/assets/python/app/README
       ...
```

### Comparing `briefcase-0.3.8/docs/how-to/see_errors_on_ios.rst` & `briefcase-0.3.9/docs/how-to/see_errors_on_ios.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/how-to/upgrade-from-v0.2.rst` & `briefcase-0.3.9/docs/how-to/upgrade-from-v0.2.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/index.rst` & `briefcase-0.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/make.bat` & `briefcase-0.3.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/reference/commands/build.rst` & `briefcase-0.3.9/docs/reference/commands/build.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/reference/commands/create.rst` & `briefcase-0.3.9/docs/reference/commands/create.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/reference/commands/dev.rst` & `briefcase-0.3.9/docs/reference/commands/dev.rst`

 * *Files 10% similar despite different names*

```diff
@@ -27,7 +27,11 @@
 required if your project contains more than one application target. The app
 name specified should be the machine-readable package name for the app.
 
 ``-d`` / ``--update-dependencies``
 ----------------------------------
 
 Update application dependencies.
+
+``--no-run``
+------------
+Do not run the application and only install application dependencies.
```

### Comparing `briefcase-0.3.8/docs/reference/commands/new.rst` & `briefcase-0.3.9/docs/reference/commands/new.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/reference/commands/package.rst` & `briefcase-0.3.9/docs/reference/commands/package.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/reference/commands/publish.rst` & `briefcase-0.3.9/docs/reference/commands/publish.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/reference/commands/run.rst` & `briefcase-0.3.9/docs/reference/commands/run.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/reference/commands/update.rst` & `briefcase-0.3.9/docs/reference/commands/update.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/reference/commands/upgrade.rst` & `briefcase-0.3.9/docs/reference/commands/upgrade.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/reference/configuration.rst` & `briefcase-0.3.9/docs/reference/configuration.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-=====================
-Configuration options
-=====================
+=============================
+Project configuration options
+=============================
 
 Briefcase is a `PEP518 <https://www.python.org/dev/peps/pep-0518/>`__-compliant
 build tool. It uses a ``pyproject.toml`` file, in the root directory of your
 project, to provide build instructions for the packaged file.
 
-If you have an application called "My App", with source code in the `src/myapp`
+If you have an application called "My App", with source code in the ``src/myapp``
 directory, the simplest possible ``pyproject.toml`` Briefcase configuration
 file would be::
 
     [tool.briefcase]
     project_name = "My Project"
     bundle = "com.example"
     version = "0.1"
```

### Comparing `briefcase-0.3.8/docs/reference/platforms/android.rst` & `briefcase-0.3.9/docs/reference/platforms/android.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/reference/platforms/iOS.rst` & `briefcase-0.3.9/docs/reference/platforms/iOS.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/reference/platforms/linux/appimage.rst` & `briefcase-0.3.9/docs/reference/platforms/linux/appimage.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-==============
-Linux AppImage
-==============
+========
+AppImage
+========
 
 `AppImage <https://appimage.org>`__ provides a way for developers to provide
 "native" binaries for Linux users. It allow packaging applications for any
-common Linux based operating system, including Ubuntu, Debian, Fedora, and
-more. AppImages contain all the dependencies that cannot be assumed to
-be part of each target system, and will run on most Linux distributions
-without further modifications.
+common Linux based operating system, including Ubuntu, Debian, Fedora, and more.
+AppImages contain all the dependencies that cannot be assumed to be part of each
+target system, and will run on most Linux distributions without further
+modifications. Briefcase uses `linuxdeploy
+<https://github.com/linuxdeploy/linuxdeploy>`__ to build the AppImage in the
+correct format.
 
 Packaging binaries for Linux is complicated, because of the inconsistent
 library versions present on each distribution. An AppImage can be executed on
 *any* Linux distribution with a version of ``libc`` greater than or equal the
 version of the distribution where the AppImage was created.
 
 To simplify the packaging process, Briefcase provides a pre-compiled Python
@@ -40,15 +42,23 @@
    version of libc that is available on the distribution you use. If you build
    using Ubuntu 19.10, for example, you can expect that only people on the most
    recent versions of another distribution will be able to run your AppImage.
 
 Icon format
 ===========
 
-AppImages use ``.png`` format icons.
+AppImages uses ``.png`` format icons. An application must provide icons in
+the following sizes:
+
+  * 16px
+  * 32px
+  * 64px
+  * 128px
+  * 256px
+  * 512px
 
 Splash Image format
 ===================
 
 AppImages do not support splash screens or installer images.
 
 Additional options
@@ -88,31 +98,77 @@
 
 but the app works under ``briefcase dev``, the problem may be an incomplete
 ``system_requires`` definition. The ``briefcase build`` process generates
 a new environment that is completely isolated from your development
 environment, so if your app has any operating system dependencies, they
 *must* be listed in your ``system_requires`` definition.
 
+``linuxdeploy_plugins``
+~~~~~~~~~~~~~~~~~~~~~~~
+
+A list of `linuxdeploy plugins
+<https://docs.appimage.org/packaging-guide/from-source/linuxdeploy-user-guide.html#plugin-system>`__
+that you wish to be included when building the AppImage. This is needed for
+applications that depend on libraries that have dependencies that cannot be
+automatically discovered by linuxdeploy. GTK and Qt both have complex
+runtime resource requirements that can be difficult for linuxdeploy to
+identify automatically.
+
+The ``linuxdeploy_plugins`` declaration is a list of strings. Briefcase can take
+plugin definitions in three formats:
+
+1. The name of a plugin known by Briefcase. One of ``gtk`` or ``qt``.
+2. A URL where a plugin can be downloaded
+3. A path to a local plugin file
+
+If your plugin requires an environment variable for configuration, that
+environment variable can be provided as a prefix to the plugin declaration,
+similar to how environment variables can be defined for a shell command.
+
+For example, the ``gtk`` plugin requires the ``DEPLOY_GTK_VERSION`` environment
+variable. To set this variable with the Briefcase-managed GTK linuxdeploy plugin,
+you would define::
+
+    linuxdeploy_plugins = ["DEPLOY_GTK_VERSION=3 gtk"]
+
+Or, if you were using a plugin stored as a local file::
+
+    linuxdeploy_plugins = ["DEPLOY_GTK_VERSION=3 path/to/plugins/linuxdeploy-gtk-plugin.sh"]
+
 Runtime issues with AppImages
 =============================
 
 Packaging on Linux is a difficult problem - especially when it comes to binary
 libraries. The following are some common problems you may see, and ways that
 they can be mitigated.
 
+Undefined symbol and Namespace not available errors
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+If you get the error::
+
+    ValueError: Namespace Something not available
+
+or::
+
+    ImportError: /usr/lib/libSomething.so.0: undefined symbol: some_symbol
+
+it is likely that one or more of the libraries you are using in your app
+requires a linuxdeploy plugin. GUI libraries, or libraries that do dynamic
+module loading are particularly prone to this problem.
+
 ELF load command address/offset not properly aligned
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-The process of building an AppImage involves using a tool named ``linuxdeploy``.
-``linuxdeploy`` processes all the libraries used by an app so that they can be
-relocated into the final packaged binary. Building a ``manylinux`` binary wheel
-involves a tool called ``auditwheel`` that performs a very similar process.
-Unfortunately, processing a binary with ``linuxdeploy`` after it has been
-processed by ``auditwheel`` can result in a binary library that cannot be loaded
-at runtime.
+Briefcase uses a tool named ``linuxdeploy`` to build AppImages. ``linuxdeploy``
+processes all the libraries used by an app so that they can be relocated into
+the final packaged binary. Building a ``manylinux`` binary wheel involves a tool
+named ``auditwheel`` that performs a very similar process. Unfortunately,
+processing a binary with ``linuxdeploy`` after it has been processed by
+``auditwheel`` can result in a binary library that cannot be loaded at runtime.
 
 This is particularly common when a module installed as a binary wheel has a
 dependency on external libraries. For example, Pillow is a Python library that
 contains a binary submodule; that submodule uses ``libpng``, ``libtiff``, and
 other system libraries for image manipulation. If you install Pillow from a
 ``manylinux`` wheel, you may see an error similar to the following at runtime::
```

### Comparing `briefcase-0.3.8/docs/reference/platforms/macOS/app.rst` & `briefcase-0.3.9/docs/reference/platforms/macOS/app.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/reference/platforms/macOS/xcode.rst` & `briefcase-0.3.9/docs/reference/platforms/macOS/xcode.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/docs/reference/platforms/windows/msi.rst` & `briefcase-0.3.9/docs/reference/platforms/windows/app.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,39 @@
-=============
-MSI Installer
-=============
-
-An MSI installer is a common format used for the installation, maintenance,
-and removal of Windows software. It contains the files to be distributed, along
-with metadata supporting the files to be installed, including details such as
-registry entries. It includes a GUI installer, and automated generation of
-the uninstallation sequence.
-
-Briefcase uses the `WiX Toolset <https://wixtoolset.org/>`__ to build
-installers. WiX, in turn, requires that .NET Framework 3.5 is enabled.
-To ensure .NET Framework 3.5 is enabled:
+===========
+Windows App
+===========
+
+A Windows app is a stub binary, allow with a collection of folders taht contain
+the Python code for the app and the Python runtime libraries.
+
+Briefcase uses the `WiX Toolset <https://wixtoolset.org/>`__ to build an MSI
+installer for a Windows App. WiX, in turn, requires that .NET Framework 3.5 is
+enabled. To ensure .NET Framework 3.5 is enabled:
 
     1. Open the Windows Control Panel
     2. Traverse to Programs -> Programs and Features
     3. Select "Turn Windows features On or Off"
     4. Ensure that ".NET framework 3.5 (includes .NET 2.0 and 3.0)" is selected.
 
 Icon format
 ===========
 
-MSI installers use ``.ico`` format icons.
+Windows apps installers use multiformat ``.ico`` icons; these icons should
+contain images in the following sizes:
+
+* 16x16
+* 32x32
+* 48x48
+* 64x64
+* 256x256
 
 Splash Image format
 ===================
 
-MSI installers do not support splash screens or installer images.
+Windows Apps do not support splash screens or installer images.
 
 Application configuration
 =========================
 
 The following options can be added to the
 ``tool.briefcase.app.<appname>.windows`` section of your ``pyproject.toml``
 file.
@@ -39,15 +43,16 @@
 
 Controls whether the app will be installed as a per-user or per-machine app.
 Per-machine apps are "system" apps, and require admin permissions to run the
 installer; however, they are installed once and shared between all users on a
 computer.
 
 If ``true`` the installer will attempt to install the app as a per-machine app,
-available to all users. Defaults to a per-user install.
+available to all users. If ``false``, the installer will install as a per-user
+app. If undefined the installer will ask the user for their preference.
 
 ``version_triple``
 ------------------
 
 Python and Briefcase allow any valid `PEP440 version number
 <https://www.python.org/dev/peps/pep-0440/>`_ as a ``version`` specifier.
 However, MSI installers require a strict integer triple version number. Many
@@ -62,18 +67,7 @@
     * ``1.2b4`` becomes ``1.2.0``
     * ``1.2.3b3`` becomes ``1.2.3``
     * ``1.2.3.4`` becomes ``1.2.3``.
 
 However, if you need to override this default value, you can define
 ``version_triple`` in your app settings. If provided, this value will be used
 in the MSI configuration file instead of the auto-generated value.
-
-Features
-========
-
-Briefcase produced MSI installers do not require elevated privileges for
-installation; they default to *per-user* installs. The installer can be
-installed for all users using the CLI, with:
-
-.. code-block::
-
-    > msiexec.exe /i <msi-filename> MSIINSTALLPERUSER=""
```

### Comparing `briefcase-0.3.8/docs/tutorial/index.rst` & `briefcase-0.3.9/docs/tutorial/index.rst`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/setup.cfg` & `briefcase-0.3.9/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = briefcase
-version = attr: src.briefcase.__version__
+version = attr: briefcase.__version__
 url = http://beeware.org/briefcase
 project_urls = 
 	Funding = https://beeware.org/contributing/membership/
 	Documentation = http://briefcase.readthedocs.io/en/latest/
 	Tracker = https://github.com/beeware/briefcase/issues
 	Source = https://github.com/beeware/briefcase
 author = Russell Keith-Magee
@@ -58,14 +58,15 @@
 	cookiecutter >= 1.0
 	tomli >= 2.0.0; python_version <= "3.10"
 	requests >= 2.22.0
 	GitPython >= 3.0.8
 	dmgbuild >= 1.3.3; sys_platform == "darwin"
 	psutil >= 5.9.0
 	rich >= 12.4.1
+	platformdirs >= 2.5.2
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	briefcase = briefcase.__main__:main
@@ -77,20 +78,22 @@
 	windows = briefcase.platforms.windows
 briefcase.formats.android = 
 	gradle = briefcase.platforms.android.gradle
 briefcase.formats.ios = 
 	xcode = briefcase.platforms.iOS.xcode
 briefcase.formats.linux = 
 	appimage = briefcase.platforms.linux.appimage
+	flatpak = briefcase.platforms.linux.flatpak
 briefcase.formats.macos = 
 	app = briefcase.platforms.macOS.app
 	xcode = briefcase.platforms.macOS.xcode
 	homebrew = briefcase.platforms.macOS.homebrew
 briefcase.formats.windows = 
-	msi = briefcase.platforms.windows.msi
+	app = briefcase.platforms.windows.app
+	visualstudio = briefcase.platforms.windows.visualstudio
 
 [aliases]
 test = pytest
 
 [bdist_wheel]
 universal = 1
```

### Comparing `briefcase-0.3.8/src/briefcase/__main__.py` & `briefcase-0.3.9/src/briefcase/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 
 def main():
     log = Log()
     command = None
     try:
         command, options = parse_cmdline(sys.argv[1:])
+        command.check_obsolete_data_dir()
         command.parse_config("pyproject.toml")
         command(**options)
         result = 0
     except HelpText as e:
         log.info()
         log.info(str(e))
         result = e.error_code
```

### Comparing `briefcase-0.3.8/src/briefcase/cmdline.py` & `briefcase-0.3.9/src/briefcase/cmdline.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/src/briefcase/commands/base.py` & `briefcase-0.3.9/src/briefcase/commands/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,27 +9,29 @@
 from cgi import parse_header
 from pathlib import Path
 from urllib.parse import urlparse
 
 import requests
 from cookiecutter.main import cookiecutter
 from cookiecutter.repository import is_repo_url
+from platformdirs import PlatformDirs
 
 try:
     import tomllib
 except ModuleNotFoundError:
     import tomli as tomllib
 
 from briefcase import __version__, integrations
 from briefcase.config import AppConfig, BaseConfig, GlobalConfig, parse_config
 from briefcase.console import Console, Log
 from briefcase.exceptions import (
     BadNetworkResourceError,
     BriefcaseCommandError,
     BriefcaseConfigError,
+    InfoHelpText,
     MissingNetworkResourceError,
 )
 from briefcase.integrations.subprocess import Subprocess
 
 
 class TemplateUnsupportedVersion(BriefcaseCommandError):
     def __init__(self, python_version_tag):
@@ -108,45 +110,181 @@
 
 
 class BaseCommand(ABC):
     cmd_line = "briefcase {command} {platform} {output_format}"
     GLOBAL_CONFIG_CLASS = GlobalConfig
     APP_CONFIG_CLASS = AppConfig
 
-    def __init__(self, base_path, home_path=Path.home(), apps=None, input_enabled=True):
-        self.base_path = base_path
-        self.home_path = home_path
-        self.dot_briefcase_path = home_path / ".briefcase"
-        self.tools_path = self.dot_briefcase_path / "tools"
+    def __init__(
+        self,
+        base_path,
+        home_path=None,
+        data_path=None,
+        apps=None,
+        input_enabled=True,
+    ):
+        # Some details about the host machine
+        self.host_arch = platform.machine()
+        self.host_os = platform.system()
+
+        self.base_path = Path(base_path)
+
+        # If a home path is provided during construction, use it. This usually
+        # indicates we're under test conditions.
+        if home_path is None:
+            home_path = Path.home()
+        self.home_path = Path(home_path)
+
+        # If a data path is provided during construction, use it. This usually
+        # indicates we're under test conditions. If there's no data path
+        # provided, look for a BRIEFCASE_HOME environment variable. If that
+        # isn't defined, use a platform-specific default data path.
+        if data_path is None:
+            try:
+                briefcase_home = os.environ["BRIEFCASE_HOME"]
+                data_path = Path(briefcase_home).resolve()
+                # Path("") converts to ".", so check for that edge case.
+                if briefcase_home == "" or not data_path.exists():
+                    raise BriefcaseCommandError(
+                        "The path specified by BRIEFCASE_HOME does not exist."
+                    )
+            except KeyError:
+                if self.host_os == "Darwin":
+                    # macOS uses a bundle name, rather than just the app name
+                    app_name = "org.beeware.briefcase"
+                else:
+                    app_name = "briefcase"
+
+                data_path = PlatformDirs(
+                    appname=app_name,
+                    appauthor="BeeWare",
+                ).user_cache_path
+
+        if " " in os.fsdecode(data_path):
+            raise BriefcaseCommandError(
+                f"""
+The location Briefcase will use to store tools and support files:
+
+    {data_path}
+
+contains spaces. This will cause problems with some tools, preventing
+you from building and packaging applications.
+
+You can set the environment variable BRIEFCASE_HOME to specify
+a custom location for Briefcase's tools.
+
+"""
+            )
+
+        self.data_path = Path(data_path)
+
+        self.tools_path = self.data_path / "tools"
 
         self.global_config = None
         self.apps = {} if apps is None else apps
         self._path_index = {}
 
-        # Some details about the host machine
-        self.host_arch = platform.machine()
-        self.host_os = platform.system()
-
         # External service APIs.
         # These are abstracted to enable testing without patching.
         self.cookiecutter = cookiecutter
         self.requests = requests
         self.input = Console(enabled=input_enabled)
         self.os = os
         self.sys = sys
+        self.stdlib_platform = platform
         self.shutil = shutil
         self.subprocess = Subprocess(self)
 
         # The internal Briefcase integrations API.
         self.integrations = integrations
 
         # Initialize default logger (replaced when options are parsed).
         self.logger = Log()
         self.save_log = False
 
+    def check_obsolete_data_dir(self):
+        """Inform user if obsolete data directory exists.
+
+        TODO: Remove this check after 1 JAN 2023 since most users will have transitioned by then
+
+        Previous versions used the ~/.briefcase directory to store
+        downloads, tools, etc. This check lets users know the old
+        directory still exists and their options to migrate or clean up.
+        """
+        dot_briefcase_path = self.home_path / ".briefcase"
+
+        # If there's no .briefcase path, no need to check for migration.
+        if not dot_briefcase_path.exists():
+            return
+
+        # If the data path is user-provided, don't check for migration.
+        if "BRIEFCASE_HOME" in os.environ:
+            return
+
+        if self.data_path.exists():
+            self.logger.warning(
+                f"""\
+Briefcase is no longer using the data directory:
+
+    {dot_briefcase_path}
+
+This directory can be safely deleted.
+"""
+            )
+        else:
+            self.logger.warning(
+                f"""\
+*************************************************************************
+** NOTICE: Briefcase is changing its data directory                   **
+*************************************************************************
+
+    Briefcase is moving its data directory from:
+
+        {dot_briefcase_path}
+
+    to:
+
+        {self.data_path}
+
+    If you continue, Briefcase will re-download the tools and data it
+    uses to build and package applications.
+
+    To avoid potentially large downloads and long installations, you
+    can manually move the old data directory to the new location.
+
+    If you continue and allow Briefcase to re-download its tools, the
+    old data directory can be safely deleted.
+
+*************************************************************************
+"""
+            )
+            self.input.prompt()
+            if not self.input.boolean_input(
+                "Do you want to re-download the Briefcase support tools",
+                # Default to continuing for non-interactive runs
+                default=not self.input.enabled,
+            ):
+                raise InfoHelpText(
+                    f"""\
+Move the Briefcase data directory from:
+
+    {dot_briefcase_path}
+
+to:
+
+    {self.data_path}
+
+or delete the old data directory, and re-run Briefcase.
+
+"""
+                )
+
+            # Create data directory to prevent full notice showing again.
+            self.data_path.mkdir(parents=True, exist_ok=True)
+
     @property
     def create_command(self):
         """Factory property; return an instance of a create command for the
         same format."""
         format_module = importlib.import_module(self.__module__)
         command = format_module.create(
             base_path=self.base_path,
@@ -287,14 +425,28 @@
         # If the index file hasn't been loaded for this app, load it.
         try:
             path_index = self._path_index[app]
         except KeyError:
             path_index = self._load_path_index(app)
         return self.bundle_path(app) / path_index["support_path"]
 
+    def app_requirements_path(self, app: BaseConfig):
+        """Obtain the path into which a requirements.txt file should be
+        written.
+
+        :param app: The config object for the app
+        :return: The full path where the requirements.txt file should be written
+        """
+        # If the index file hasn't been loaded for this app, load it.
+        try:
+            path_index = self._path_index[app]
+        except KeyError:
+            path_index = self._load_path_index(app)
+        return self.bundle_path(app) / path_index["app_requirements_path"]
+
     def app_packages_path(self, app: BaseConfig):
         """Obtain the path into which dependencies should be installed.
 
         :param app: The config object for the app
         :return: The full path where application dependencies should be installed.
         """
         # If the index file hasn't been loaded for this app, load it.
@@ -455,15 +607,17 @@
                     self.apps[app_name] = create_config(
                         klass=self.APP_CONFIG_CLASS,
                         config=app_config,
                         msg=f"Configuration for '{app_name}'",
                     )
 
         except FileNotFoundError as e:
-            raise BriefcaseConfigError("configuration file not found") from e
+            raise BriefcaseConfigError(
+                f"""Configuration file not found. Did you run briefcase in the directory that contains {filename!r}?"""
+            ) from e
 
     def download_url(self, url, download_path):
         """Download a given URL, caching it. If it has already been downloaded,
         return the value that has been cached.
 
         This is a utility method used to obtain assets used by the
         install process. The cached filename will be the filename portion of
```

### Comparing `briefcase-0.3.8/src/briefcase/commands/build.py` & `briefcase-0.3.9/src/briefcase/commands/build.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/src/briefcase/commands/create.py` & `briefcase-0.3.9/src/briefcase/commands/create.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import hashlib
 import os
+import platform
 import shutil
 import subprocess
 import sys
 from datetime import date
 from pathlib import Path
 from typing import Optional
 from urllib.parse import parse_qsl, urlencode, urlsplit, urlunsplit
@@ -254,14 +256,16 @@
         )
 
         # Construct a template context from the app configuration.
         extra_context = app.__dict__.copy()
         # Augment with some extra fields.
         extra_context.update(
             {
+                # Properties of the generating environment
+                "python_version": platform.python_version(),
                 # Transformations of explicit properties into useful forms
                 "module_name": app.module_name,
                 "package_name": app.package_name,
                 # Properties that are a function of the execution
                 "year": date.today().strftime("%Y"),
                 "month": date.today().strftime("%B"),
             }
@@ -290,20 +294,45 @@
             # Either the template path is invalid,
             # or it isn't a cookiecutter template (i.e., no cookiecutter.json)
             raise InvalidTemplateRepository(app.template) from e
         except cookiecutter_exceptions.RepositoryCloneFailed as e:
             # Branch does not exist for python version
             raise TemplateUnsupportedVersion(app.template_branch) from e
 
+    def _unpack_support_package(self, support_file_path, support_path):
+        """Unpack a support package into a specific location.
+
+        :param support_file_path: The path to the support file to be unpacked.
+        :param support_path: The path where support files should unpacked.
+        """
+        try:
+            with self.input.wait_bar("Unpacking support package..."):
+                support_path.mkdir(parents=True, exist_ok=True)
+                self.shutil.unpack_archive(
+                    support_file_path,
+                    extract_dir=support_path,
+                )
+        except (shutil.ReadError, EOFError) as e:
+            raise InvalidSupportPackage(support_file_path) from e
+
     def install_app_support_package(self, app: BaseConfig):
         """Install the application support package.
 
         :param app: The config object for the app
         """
         try:
+            support_path = self.support_path(app)
+        except KeyError:
+            self.logger.info("No support package required.")
+        else:
+            support_file_path = self._download_support_package(app)
+            self._unpack_support_package(support_file_path, support_path)
+
+    def _download_support_package(self, app):
+        try:
             # Work out if the app defines a custom override for
             # the support package URL.
             try:
                 support_package_url = app.support_package
                 custom_support_package = True
                 self.logger.info(f"Using custom support package {support_package_url}")
             except AttributeError:
@@ -325,82 +354,139 @@
                     url_parts[3] = urlencode(query)
                     support_package_url = urlunsplit(url_parts)
 
                 except AttributeError:
                     # No support revision specified.
                     self.logger.info("... using most recent revision")
 
+                if custom_support_package:
+                    # If the support package is custom, cache it using a hash of
+                    # the download URL. This is needed to differentiate to support
+                    # packages with the same filename, served at different URLs.
+                    # (or a custom package that collides with an official package name)
+                    download_path = (
+                        self.data_path
+                        / "support"
+                        / hashlib.sha256(
+                            support_package_url.encode("utf-8")
+                        ).hexdigest()
+                    )
+                else:
+                    download_path = self.data_path / "support"
+
                 # Download the support file, caching the result
                 # in the user's briefcase support cache directory.
-                support_filename = self.download_url(
+                return self.download_url(
                     url=support_package_url,
-                    download_path=self.dot_briefcase_path / "support",
+                    download_path=download_path,
                 )
             else:
-                support_filename = Path(support_package_url)
+                return Path(support_package_url)
         except MissingNetworkResourceError as e:
             # If there is a custom support package, report the missing resource as-is.
             if custom_support_package:
                 raise
             else:
                 raise MissingSupportPackage(
                     python_version_tag=self.python_version_tag,
                     host_arch=self.host_arch,
                 ) from e
 
         except requests_exceptions.ConnectionError as e:
             raise NetworkFailure("downloading support package") from e
-        try:
-            with self.input.wait_bar("Unpacking support package..."):
-                support_path = self.support_path(app)
-                support_path.mkdir(parents=True, exist_ok=True)
-                # TODO: Py3.6 compatibility; os.fsdecode not required in Py3.7
-                self.shutil.unpack_archive(
-                    os.fsdecode(support_filename), extract_dir=os.fsdecode(support_path)
-                )
-        except (shutil.ReadError, EOFError) as e:
-            raise InvalidSupportPackage(support_package_url) from e
-
-    def install_app_dependencies(self, app: BaseConfig):
-        """Install the dependencies for the app.
 
-        :param app: The config object for the app
+    def _write_requirements_file(self, app: BaseConfig, requirements_path):
+        """Configure application dependencies by writing a requirements.txt
+        file.
+
+        :param app: The app configuration
+        :param requirements_path: The full path to a requirements.txt file that
+            will be written.
+        """
+        # Windows allows both / and \ as a path separator in requirements.
+        separators = [os.sep]
+        if os.altsep:
+            separators.append(os.altsep)
+
+        with self.input.wait_bar("Writing requirements file..."):
+            with (requirements_path).open("w", encoding="utf-8") as f:
+                if app.requires:
+                    for requirement in app.requires:
+                        # If the requirement is a local path, convert it to
+                        # absolute, because Flatpak moves the requirements file
+                        # to a different place before using it.
+                        if any(sep in requirement for sep in separators) and (
+                            not _has_url(requirement)
+                        ):
+                            # We use os.path.abspath() rather than Path.resolve()
+                            # because we *don't* want Path's symlink resolving behavior.
+                            requirement = os.path.abspath(self.base_path / requirement)
+                        f.write(f"{requirement}\n")
+
+    def _install_app_dependencies(self, app: BaseConfig, app_packages_path):
+        """Install dependencies for the app with pip.
+
+        :param app: The app configuration
+        :param app_packages_path: The full path of the app_packages folder into which
+            dependencies should be installed.
         """
-
-        target = self.app_packages_path(app)
-
         # Clear existing dependency directory
-        if target.is_dir():
-            self.shutil.rmtree(target)
-            self.os.mkdir(target)
+        if app_packages_path.is_dir():
+            self.shutil.rmtree(app_packages_path)
+            self.os.mkdir(app_packages_path)
 
         # Install dependencies
         if app.requires:
             with self.input.wait_bar("Installing app dependencies..."):
                 try:
                     self.subprocess.run(
                         [
                             sys.executable,
                             "-m",
                             "pip",
                             "install",
                             "--upgrade",
                             "--no-user",
-                            "--progress-bar",
-                            "off",
-                            f"--target={target}",
+                            f"--target={app_packages_path}",
                         ]
                         + app.requires,
                         check=True,
                     )
                 except subprocess.CalledProcessError as e:
                     raise DependencyInstallError() from e
         else:
             self.logger.info("No application dependencies.")
 
+    def install_app_dependencies(self, app: BaseConfig):
+        """Handle dependencies for the app.
+
+        This will result in either (in preferential order):
+         * a requirements.txt file being written at a location specified by
+           ``app_requirements_path`` in the template path index
+         * dependencies being installed with pip into the location specified
+           by the ``app_packages_path`` in the template path index.
+
+        If the path index doesn't specify either of the path index entries,
+        an error is raised.
+
+        :param app: The config object for the app
+        """
+        try:
+            path = self.app_requirements_path(app)
+            self._write_requirements_file(app, path)
+        except KeyError:
+            try:
+                path = self.app_packages_path(app)
+                self._install_app_dependencies(app, path)
+            except KeyError as e:
+                raise BriefcaseCommandError(
+                    "Application path index file does not define "
+                    "`app_requirements_path` or `app_packages_path`"
+                ) from e
+
     def install_app_code(self, app: BaseConfig):
         """Install the application code into the bundle.
 
         :param app: The config object for the app
         """
 
         # Remove existing app folder
@@ -619,7 +705,22 @@
             state = self.create_app(app, **options)
         else:
             state = None
             for app_name, app in sorted(self.apps.items()):
                 state = self.create_app(app, **full_options(state, options))
 
         return state
+
+
+# Detects any of the URL schemes supported by pip
+# (https://pip.pypa.io/en/stable/topics/vcs-support/).
+def _has_url(requirement):
+    return any(
+        f"{scheme}:" in requirement
+        for scheme in (
+            ["http", "https", "file", "ftp"]
+            + ["git+file", "git+https", "git+ssh", "git+http", "git+git", "git"]
+            + ["hg+file", "hg+http", "hg+https", "hg+ssh", "hg+static-http"]
+            + ["svn", "svn+svn", "svn+http", "svn+https", "svn+ssh"]
+            + ["bzr+http", "bzr+https", "bzr+ssh", "bzr+sftp", "bzr+ftp", "bzr+lp"]
+        )
+    )
```

### Comparing `briefcase-0.3.8/src/briefcase/commands/dev.py` & `briefcase-0.3.9/src/briefcase/commands/dev.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import subprocess
 import sys
+from pathlib import Path
 from typing import Optional
 
 from briefcase.config import BaseConfig
 from briefcase.exceptions import BriefcaseCommandError
 
 from .base import BaseCommand
 from .create import DependencyInstallError, write_dist_info
@@ -82,27 +83,40 @@
 
         :param app: The config object for the app
         :param env: environment dictionary for sub command
         """
         try:
             # Invoke the app.
             self.subprocess.run(
-                [sys.executable, "-m", app.module_name],
+                [
+                    sys.executable,
+                    "-c",
+                    (
+                        "import runpy, sys;"
+                        "sys.path.pop(0);"
+                        f'runpy.run_module("{app.module_name}", run_name="__main__", alter_sys=True)'
+                    ),
+                ],
                 env=env,
                 check=True,
+                cwd=self.home_path,
             )
         except subprocess.CalledProcessError as e:
             raise BriefcaseCommandError(
                 f"Unable to start application '{app.app_name}'"
             ) from e
 
     def get_environment(self, app):
         # Create a shell environment where PYTHONPATH points to the source
         # directories described by the app config.
-        return {"PYTHONPATH": os.pathsep.join(app.PYTHONPATH)}
+        return {
+            "PYTHONPATH": os.pathsep.join(
+                os.fsdecode(Path.cwd() / path) for path in app.PYTHONPATH
+            )
+        }
 
     def __call__(
         self,
         appname: Optional[str] = None,
         update_dependencies: Optional[bool] = False,
         run_app: Optional[bool] = True,
         **options,
```

### Comparing `briefcase-0.3.8/src/briefcase/commands/new.py` & `briefcase-0.3.9/src/briefcase/commands/new.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/src/briefcase/commands/package.py` & `briefcase-0.3.9/src/briefcase/commands/package.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/src/briefcase/commands/publish.py` & `briefcase-0.3.9/src/briefcase/commands/publish.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/src/briefcase/commands/run.py` & `briefcase-0.3.9/src/briefcase/commands/run.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/src/briefcase/commands/update.py` & `briefcase-0.3.9/src/briefcase/commands/update.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/src/briefcase/commands/upgrade.py` & `briefcase-0.3.9/src/briefcase/commands/upgrade.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 import sys
 from typing import List
 
 from briefcase.exceptions import BriefcaseCommandError
 from briefcase.integrations.android_sdk import AndroidSDK
 from briefcase.integrations.java import JDK
 from briefcase.integrations.linuxdeploy import LinuxDeploy
+from briefcase.integrations.rcedit import RCEdit
 from briefcase.integrations.wix import WiX
 
 from .base import BaseCommand
 
 
 class UpgradeCommand(BaseCommand):
     cmd_line = "briefcase upgrade"
     command = "upgrade"
     output_format = None
     description = "Upgrade briefcase-managed tools"
 
     def __init__(self, *args, **options):
         super().__init__(*args, **options)
-        self.sdks = [AndroidSDK, LinuxDeploy, JDK, WiX]
+        self.sdks = [
+            AndroidSDK,
+            LinuxDeploy,
+            JDK,
+            WiX,
+            RCEdit,
+        ]
 
     @property
     def platform(self):
         """The upgrade command always reports as the local platform."""
         return {
             "darwin": "macOS",
             "linux": "linux",
             "win32": "windows",
         }[sys.platform]
 
     def bundle_path(self, app):
         """A placeholder; Upgrade command doesn't have a bundle path."""
-        raise NotImplementedError()
+        raise NotImplementedError()  # pragma: no cover
 
     def binary_path(self, app):
         """A placeholder; Upgrade command doesn't have a binary path."""
-        raise NotImplementedError()
+        raise NotImplementedError()  # pragma: no cover
 
     def distribution_path(self, app, packaging_format):
         """A placeholder; Upgrade command doesn't have a distribution path."""
-        raise NotImplementedError()
+        raise NotImplementedError()  # pragma: no cover
 
     def add_options(self, parser):
         parser.add_argument(
             "-l",
             "--list",
             dest="list_tools",
             action="store_true",
@@ -53,26 +60,39 @@
             "tool_list",
             metavar="tool",
             nargs="*",
             help="The Briefcase-managed tool to upgrade. If no tool is named, all tools will be upgraded.",
         )
 
     def __call__(self, tool_list: List[str], list_tools=False, **options):
-        # Verify all the managed SDKs to see which are present.
+        # Verify all the managed SDKs and plugins to see which are present.
         managed_tools = {}
         non_managed_tools = set()
+
         for klass in self.sdks:
             try:
                 tool = klass.verify(self, install=False)
                 if tool.managed_install:
                     managed_tools[klass.name] = tool
+                    try:
+                        for plugin_klass in tool.plugins.values():
+                            try:
+                                plugin = plugin_klass.verify(self, install=False)
+                                # All plugins are managed
+                                managed_tools[plugin.name] = plugin
+                            except BriefcaseCommandError:
+                                # Plugin doesn't exist
+                                non_managed_tools.add(klass.name)
+                    except AttributeError:
+                        # Tool doesn't have plugins
+                        pass
                 else:
                     non_managed_tools.add(klass.name)
             except BriefcaseCommandError:
-                # Tool doesn't exist, or can't be managed
+                # Tool doesn't exist
                 non_managed_tools.add(klass.name)
 
         # If a tool list wasn't provided, use the list of installed tools
         if not tool_list:
             tool_list = sorted(managed_tools.keys())
 
         # Build a list of requested tools that are managed.
```

### Comparing `briefcase-0.3.8/src/briefcase/config.py` & `briefcase-0.3.9/src/briefcase/config.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/src/briefcase/console.py` & `briefcase-0.3.9/src/briefcase/console.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,17 @@
     highlights = [r"(?P<url>(file|https|http|ws|wss)://[-0-9a-zA-Z$_+!`(),.?/;:&=%#]*)"]
 
 
 class Printer:
     """Interface for printing and managing output to the console and/or log."""
 
     # Console to manage console output.
-    console = RichConsole(highlighter=RichConsoleHighlighter(), emoji=False)
+    console = RichConsole(
+        highlighter=RichConsoleHighlighter(), emoji=False, soft_wrap=True
+    )
 
     # Console to record all logging to a buffer while not printing anything to the console.
     # We need to be wide enough to render `sdkmanager --list_installed` output without
     # line wrapping.
     LOG_FILE_WIDTH = 180
     log = RichConsole(
         # Rich only records what's being logged if it is actually written somewhere;
@@ -269,17 +271,18 @@
 
 
 class Console:
     def __init__(self, printer=Printer(), enabled=True):
         self.print = printer
         self.input = printer.console.input
         self.enabled = enabled
+        self._wait_bar: Progress = None
         # Signal that Rich is dynamically controlling the console output.
         # Therefore, all output must be printed to the screen by Rich to
-        # prevent corruption of dynamic elements like Wait Bars.
+        # prevent corruption of dynamic elements like the Wait Bar.
         self.is_output_controlled = False
 
     def prompt(self, *values, markup=False, **kwargs):
         """Print to the screen for soliciting user interaction.
 
         :param values: strings to print as the user prompt
         :param markup: True if prompt contains Rich markup
@@ -304,49 +307,60 @@
         self,
         message="",
         done_message="done",
         *,
         transient=False,
         markup=False,
     ):
-        """Returns a wait bar as a context manager.
+        """Activates the Wait Bar as a context manager.
+
+        If the Wait Bar is already active, then its message is updated for the new
+        context. Once the new context is complete, the previous Wait Bar message
+        is restored.
 
-        :param message: text explaining what is being awaited
+        :param message: text explaining what is being awaited; should end in '...'
         :param done_message: text appended to the message after exiting
         :param transient: if True, remove bar and message from screen after exiting;
             if False (default), the message will remain on the screen without pulsing bar.
         :param markup: whether to interpret Rich styling markup in the message; if True,
             the message must already be escaped; defaults False.
         """
-        wait_bar = Progress(
-            TextColumn("    "),
-            BarColumn(bar_width=20, style="black", pulse_style="white"),
-            TextColumn(message),
-            transient=True,
-            console=self.print.console,
-        )
-        # setting start=False causes the progress bar to pulse
-        wait_bar.add_task("", start=False)
+        if self._wait_bar is None:
+            self._wait_bar = Progress(
+                TextColumn("    "),
+                BarColumn(bar_width=20, style="black", pulse_style="white"),
+                TextColumn("{task.fields[message]}"),
+                transient=True,
+                console=self.print.console,
+            )
+            # start=False causes the progress bar to "pulse"
+            # message=None is a sentinel the Wait Bar should be inactive
+            self._wait_bar.add_task("", start=False, message=None)
+
+        self.is_output_controlled = True
+        wait_bar_task = self._wait_bar.tasks[0]
+        previous_message = wait_bar_task.fields["message"]
+        self._wait_bar.update(wait_bar_task.id, message=message)
         try:
-            self.is_output_controlled = True
-            with wait_bar:
-                yield
+            self._wait_bar.start()
+            yield
         except BaseException:
             # ensure the message is left on the screen even if user sends CTRL+C
             if message and not transient:
                 self.print(message, markup=markup)
             raise
         else:
             if message and not transient:
-                self.print(
-                    f'{message}{f" {done_message}" if done_message else ""}',
-                    markup=markup,
-                )
+                self.print(f"{message} {done_message}", markup=markup)
         finally:
-            self.is_output_controlled = False
+            self._wait_bar.update(wait_bar_task.id, message=previous_message)
+            # Deactivate the Wait Bar if returning to its initial state
+            if previous_message is None:
+                self._wait_bar.stop()
+                self.is_output_controlled = False
 
     def boolean_input(self, question, default=False):
         """Get a boolean input from user, in the form of y/n.
 
         The user might press "y" for true or "n" for false.
         If input is disabled, returns default. If input is disabled and default
         is *not* defined, InputDisabled is raised.
@@ -435,14 +449,15 @@
 
     def __call__(self, prompt, *, markup=False):
         """Present input() interface."""
         if not self.enabled:
             raise InputDisabled()
         try:
             input_value = self.input(prompt, markup=markup)
+            self.print.to_log(prompt)
             self.print.to_log(f"{Log.DEBUG_PREFACE}User input: {input_value}")
             return input_value
         except EOFError:
             raise KeyboardInterrupt
 
 
 def select_option(options, input, prompt="> ", error="Invalid selection"):
```

### Comparing `briefcase-0.3.8/src/briefcase/exceptions.py` & `briefcase-0.3.9/src/briefcase/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,37 +4,42 @@
 
 
 class HelpText(BriefcaseError):
     """Exceptions that contain help text and shouldn't be displayed to users as
     an error."""
 
 
+class InfoHelpText(HelpText):
+    def __init__(self, msg):
+        super().__init__(0)
+        self.msg = msg
+
+    def __str__(self):
+        return self.msg
+
+
 class NoCommandError(HelpText):
     def __init__(self, msg):
         super().__init__(-10)
         self.msg = msg
 
     def __str__(self):
         return self.msg
 
 
-class ShowOutputFormats(HelpText):
+class ShowOutputFormats(InfoHelpText):
     def __init__(self, platform, default, choices):
-        super().__init__(0)
+        super().__init__(
+            f"Available formats for {platform}: {', '.join(sorted(choices))}\n"
+            f"Default format: {default}"
+        )
         self.platform = platform
         self.default = default
         self.choices = choices
 
-    def __str__(self):
-        choices = ", ".join(sorted(self.choices))
-        return (
-            f"Available formats for {self.platform}: {choices}\n"
-            f"Default format: {self.default}"
-        )
-
 
 class InvalidFormatError(BriefcaseError):
     def __init__(self, requested, choices):
         super().__init__(-21)
         self.requested = requested
         self.choices = choices
```

### Comparing `briefcase-0.3.8/src/briefcase/integrations/android_sdk.py` & `briefcase-0.3.9/src/briefcase/integrations/android_sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import re
 import shutil
 import subprocess
 import time
+from contextlib import suppress
 from pathlib import Path
 
 from requests import exceptions as requests_exceptions
 
 from briefcase.config import PEP508_NAME_RE
 from briefcase.console import InputDisabled, select_option
 from briefcase.exceptions import (
@@ -1000,86 +1001,94 @@
                 os.fsdecode(self.emulator_path),
                 f"@{avd}",
                 "-dns-server",
                 "8.8.8.8",
             ],
             env=self.env,
             stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
+            stderr=subprocess.STDOUT,
+            bufsize=1,
             start_new_session=True,
         )
 
         # The boot process happens in 2 phases.
         # First, the emulator appears in the device list. However, it's
         # not ready until the boot process has finished. To determine
         # the boot status, we need the device ID, and an ADB connection.
 
-        # Step 1: Wait for the device to appear so we can get an
+        # Phase 1: Wait for the device to appear so we can get an
         # ADB instance for the new device.
-        with self.command.input.wait_bar("Starting emulator..."):
-            adb = None
-            known_devices = set()
-            while adb is None:
-                if emulator_popen.poll() is not None:
-                    raise BriefcaseCommandError(
-                        f"""\
+        try:
+            with self.command.input.wait_bar("Starting emulator..."):
+                adb = None
+                known_devices = set()
+                while adb is None:
+                    if emulator_popen.poll() is not None:
+                        raise BriefcaseCommandError(
+                            f"""\
 Android emulator was unable to start!
 
 Try starting the emulator manually by running:
 
     $ {' '.join(str(arg) for arg in emulator_popen.args)}
 
 Resolve any problems you discover, then try running your app again. You may
 find this page helpful in diagnosing emulator problems.
 
     https://developer.android.com/studio/run/emulator-acceleration#accel-vm
 """
-                    )
+                        )
 
-                for device, details in sorted(self.devices().items()):
-                    # Only process authorized devices that we haven't seen.
-                    if details["authorized"] and device not in known_devices:
-                        adb = self.adb(device)
-                        device_avd = adb.avd_name()
-
-                        if device_avd == avd:
-                            # Found an active device that matches
-                            # the AVD we are starting.
-                            full_name = f"@{avd} (running emulator)"
-                            break
-                        else:
-                            # Not the one. Zathras knows.
-                            adb = None
-                            known_devices.add(device)
-
-                # Try again in 2 seconds...
-                self.sleep(2)
-
-        # Phase 2: Wait for the boot process to complete
-        if not adb.has_booted():
-            with self.command.input.wait_bar("Booting emulator..."):
-                while not adb.has_booted():
-                    if emulator_popen.poll() is not None:
-                        raise BriefcaseCommandError(
-                            f"""\
+                    for device, details in sorted(self.devices().items()):
+                        # Only process authorized devices that we haven't seen.
+                        if details["authorized"] and device not in known_devices:
+                            adb = self.adb(device)
+                            device_avd = adb.avd_name()
+
+                            if device_avd == avd:
+                                # Found an active device that matches
+                                # the AVD we are starting.
+                                full_name = f"@{avd} (running emulator)"
+                                break
+                            else:
+                                # Not the one. Zathras knows.
+                                adb = None
+                                known_devices.add(device)
+
+                    # Try again in 2 seconds...
+                    self.sleep(2)
+
+            # Phase 2: Wait for the boot process to complete
+            if not adb.has_booted():
+                with self.command.input.wait_bar("Booting emulator..."):
+                    while not adb.has_booted():
+                        if emulator_popen.poll() is not None:
+                            raise BriefcaseCommandError(
+                                f"""\
 Android emulator was unable to boot!
 
 Try starting the emulator manually by running:
 
     $ {' '.join(str(arg) for arg in emulator_popen.args)}
 
 Resolve any problems you discover, then try running your app again. You may
 find this page helpful in diagnosing emulator problems.
 
     https://developer.android.com/studio/run/emulator-acceleration#accel-vm
 """
-                        )
+                            )
 
-                    # Try again in 2 seconds...
-                    self.sleep(2)
+                        # Try again in 2 seconds...
+                        self.sleep(2)
+        except Exception:
+            # if the emulator exited, this should return its output immediately;
+            # if it is still running, this will quickly time out and print nothing.
+            with suppress(subprocess.TimeoutExpired):
+                self.command.logger.info(emulator_popen.communicate(timeout=1)[0])
+            raise
 
         # Return the device ID and full name.
         return device, full_name
 
 
 class ADB:
     def __init__(self, android_sdk, device):
@@ -1231,44 +1240,45 @@
 """
                 )
         except subprocess.CalledProcessError as e:
             raise BriefcaseCommandError(
                 f"Unable to start {package}/{activity} on {self.device}"
             ) from e
 
-    def clear_log(self):
-        """Clear the log for the device.
-
-        Returns `None` on success; raises an exception on failure.
-        """
-        try:
-            # Invoke `adb logcat -c`
-            self.run("logcat", "-c")
-        except subprocess.CalledProcessError as e:
-            raise BriefcaseCommandError(f"Unable to clear log on {self.device}") from e
-
-    def logcat(self):
+    def logcat(self, pid):
         """Start tailing the adb log for the device."""
         try:
             # stream output so it's captured in logging
             self.command.subprocess.run(
                 [
                     os.fsdecode(self.android_sdk.adb_path),
                     "-s",
                     self.device,
                     "logcat",
-                    "-s",
-                    "MainActivity:*",
-                    "stdio:*",
-                    "Python:*",
-                ],
+                    "--pid",  # This option is available since API level 24.
+                    pid,
+                ]
+                # Filter out some noisy and useless tags.
+                + [f"{tag}:S" for tag in ["EGL_emulation"]],
                 env=self.android_sdk.env,
                 check=True,
                 stream_output=True,
             )
         except subprocess.CalledProcessError as e:
             # If the user sends CTRL+C:
             #  - on Windows, adb returns 0xC000013A (STATUS_CONTROL_C_EXIT)
             #  - on Linux/macOS, adb returns -2.
             # Exit normally since the user was instructed to use CTRL+C.
             if e.returncode not in {-2, 0xC000013A}:
                 raise BriefcaseCommandError("Error starting ADB logcat.") from e
+
+    def pidof(self, package):
+        """Return the PID of the given app as a string, or None if it isn't
+        running."""
+        # The pidof command is available since API level 24. The level 23 emulator image also
+        # includes it, but it doesn't work correctly (it returns all processes).
+        try:
+            # Exit status is unreliable: some devices (e.g. Nexus 4) return 0 even when no
+            # process was found.
+            return self.run("shell", "pidof", "-s", package).strip() or None
+        except subprocess.CalledProcessError:
+            return None
```

### Comparing `briefcase-0.3.8/src/briefcase/integrations/cookiecutter.py` & `briefcase-0.3.9/src/briefcase/integrations/cookiecutter.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/src/briefcase/integrations/docker.py` & `briefcase-0.3.9/src/briefcase/integrations/docker.py`

 * *Files 14% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 """
     DOCKER_NOT_INSTALLED_ERROR = """
 Briefcase requires Docker, but it is not installed (or is not on your PATH).
 Visit:
 
     {install_url}
 
-to download and install git manually.
+to download and install Docker manually.
 {extra_content}
 If you have installed Docker recently and are still getting this error, you may
 need to restart your terminal session.
 """
     try:
         # Try to get the version of docker that is installed.
         output = command.subprocess.check_output(
@@ -195,25 +195,31 @@
 
 class Docker:
     def __init__(self, command, app):
         self.command = command
         self._subprocess = command.subprocess
         self.app = app
 
+    @property
+    def docker_data_path(self):
+        """The briefcase data directory used inside container."""
+        return "/home/brutus/.cache/briefcase"
+
     def prepare(self):
         try:
             self.command.logger.info(
-                "Building Docker container image...", prefix=self.app.app_name
+                "Building Docker container image...",
+                prefix=self.app.app_name,
             )
             try:
                 system_requires = " ".join(self.app.system_requires)
             except AttributeError:
                 system_requires = ""
 
-            with self.command.input.wait_bar("Building container..."):
+            with self.command.input.wait_bar("Building Docker image..."):
                 self._subprocess.run(
                     [
                         "docker",
                         "build",
                         "--progress",
                         "plain",
                         "--tag",
@@ -233,62 +239,89 @@
                             *self.app.sources[0].split("/")[:-1],
                         ),
                     ],
                     check=True,
                 )
         except subprocess.CalledProcessError as e:
             raise BriefcaseCommandError(
-                f"Error building Docker container for {self.app.app_name}."
+                f"Error building Docker image for {self.app.app_name}."
             ) from e
 
-    def run(self, args, env=None, **kwargs):
-        """Run a process inside the Docker container."""
-        # Set up the `docker run` invocation in interactive mode,
-        # with volume mounts for the platform and .briefcase directories.
-        # The :z suffix allows SELinux to modify the host mount; it is ignored
-        # on non-SELinux platforms.
+    def _dockerize_path(self, arg):
+        """Relocate any local path into the equivalent location on the docker
+        filesystem.
+
+        Converts:
+        * any reference to sys.executable into the python executable in the docker container
+        * any path in <platform path> into the equivalent stemming from /app
+        * any path in <data path> into the equivalent in ~/.cache/briefcase
+
+        :param arg: The string argument to convert to dockerized paths
+        :returns: A string where all convertible paths have been replaced.
+        """
+        if arg == sys.executable:
+            return f"python{self.command.python_version_tag}"
+        arg = arg.replace(os.fsdecode(self.command.platform_path), "/app")
+        arg = arg.replace(os.fsdecode(self.command.data_path), self.docker_data_path)
+
+        return arg
+
+    def _dockerize_args(self, args, env=None):
+        """Convert arguments and environment into a Docker-compatible form.
+        Convert an argument and environment specifiation into a form that can
+        be used as arguments to invoke Docker. This involves:
+
+         * Configuring the Docker invocation to reference the
+           appropriate container image, and clean up afterwards
+         * Setting volume mounts for the container instance
+         * Transforming any references to local paths into Docker path references.
+
+        :param args: The arguments for the command to be invoked
+        :param env: The environment specification for the command to be executed
+        :returns: A list of arguments that can be used to invoke the command
+            inside a docker container.
+        """
+        # The :z suffix on volument mounts allows SELinux to modify the host
+        # mount; it is ignored on non-SELinux platforms.
         docker_args = [
             "docker",
             "run",
-            "--tty",
             "--volume",
             f"{self.command.platform_path}:/app:z",
             "--volume",
-            f"{self.command.dot_briefcase_path}:/home/brutus/.briefcase:z",
+            f"{self.command.data_path}:{self.docker_data_path}:z",
+            "--rm",
         ]
 
         # If any environment variables have been defined, pass them in
         # as --env arguments to Docker.
         if env:
             for key, value in env.items():
-                docker_args.extend(["--env", f"{key}={value}"])
+                docker_args.extend(["--env", f"{key}={self._dockerize_path(value)}"])
 
-        # ... then the image name.
+        # ... then the image name to create the temporary container with
         docker_args.append(self.command.docker_image_tag(self.app))
 
-        # ... then add all the arguments
-        for arg in args:
-            arg = str(arg)
-            if arg == sys.executable:
-                docker_args.append(f"python{self.command.python_version_tag}")
-            elif os.fsdecode(self.command.platform_path) in arg:
-                docker_args.append(
-                    arg.replace(os.fsdecode(self.command.platform_path), "/app")
-                )
-            elif os.fsdecode(self.command.dot_briefcase_path) in arg:
-                docker_args.append(
-                    arg.replace(
-                        os.fsdecode(self.command.dot_briefcase_path),
-                        "/home/brutus/.briefcase",
-                    )
-                )
-            else:
-                docker_args.append(arg)
+        # ... then add the command (and its arguments) to run in the container
+        docker_args.extend([self._dockerize_path(str(arg)) for arg in args])
+
+        return docker_args
 
-        # Invoke the process.
+    def run(self, args, env=None, **kwargs):
+        """Run a process inside a Docker container."""
         # Any exceptions from running the process are *not* caught.
         # This ensures that "docker.run()" behaves as closely to
         # "subprocess.run()" as possible.
         self._subprocess.run(
-            docker_args,
+            self._dockerize_args(args, env=env),
+            **kwargs,
+        )
+
+    def check_output(self, args, env=None, **kwargs):
+        """Run a process inside a Docker container, capturing output."""
+        # Any exceptions from running the process are *not* caught.
+        # This ensures that "docker.check_output()" behaves as closely to
+        # "subprocess.check_output()" as possible.
+        return self._subprocess.check_output(
+            self._dockerize_args(args, env=env),
             **kwargs,
         )
```

### Comparing `briefcase-0.3.8/src/briefcase/integrations/git.py` & `briefcase-0.3.9/src/briefcase/integrations/git.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,17 @@
     Unfortunately, `import git` triggers a call on the operating system
     to run the git executable. On some platforms (notably macOS), the git
     binary has been instrumented such that if git *isnt'* installed,
     running git triggers a prompt to install Xcode. However, that messes
     with the UX workflow.
 
     So - we defer importing git until we actually know we need it. This
-    enables Briefcase to start us to do other Xcode checks as part of
-    macOS workflows, and ensures that "briefcase --help" works on other
-    platforms without raising an error.
+    enables Briefcase to start to do other Xcode checks as part of the macOS
+    workflows, and ensures that "briefcase --help" works on other platforms
+    without raising an error.
 
     :param command: The command that needs to perform the verification check.
     :returns: The git module, if `git` is installed and available.
     """
     # Check whether the git executable could be imported.
     try:
         import git
```

### Comparing `briefcase-0.3.8/src/briefcase/integrations/java.py` & `briefcase-0.3.9/src/briefcase/integrations/java.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         If ``JAVA_HOME`` is set, try that version. If it is a JRE, or its *not*
         a Java 8 JDK, download one.
 
         On macOS, also try invoking /usr/libexec/java_home. If that location
         points to a Java 8 JDK, use it.
 
         Otherwise, download a JDK from AdoptOpenJDK and unpack it into the
-        ``~.briefcase`` path.
+        briefcase data directory.
 
         :param command: The command that needs to perform the verification
             check.
         :param install: Should the tool be installed if it is not found?
         :returns: A valid Java JDK wrapper. If a JDK is not available, and was
             not installed, raises MissingToolError.
         """
@@ -219,16 +219,16 @@
 
     def exists(self):
         return (self.java_home / "bin").exists()
 
     @property
     def managed_install(self):
         try:
-            # Determine if java_home is relative to the .briefcase folder.
-            # If java_home isn't inside .briefcase, this will raise a ValueError,
+            # Determine if java_home is relative to the briefcase data directory.
+            # If java_home isn't inside this directory, this will raise a ValueError,
             # indicating it is a non-managed install.
             self.java_home.relative_to(self.command.tools_path)
             return True
         except ValueError:
             return False
 
     def install(self):
@@ -256,17 +256,17 @@
 
 Delete {jdk_zip_path} and run briefcase again.
 """
                 ) from e
 
             jdk_zip_path.unlink()  # Zip file no longer needed once unpacked.
 
-            # The tarball will unpack into ~.briefcase/tools/jdk8u242-b08
+            # The tarball will unpack into <briefcase data dir>/tools/jdk8u242-b08
             # (or whatever name matches the current release).
-            # We turn this into ~.briefcase/tools/java so we have a consistent name.
+            # We turn this into <briefcase data dir>/tools/java so we have a consistent name.
             java_unpack_path = (
                 self.command.tools_path / f"jdk{self.release}-{self.build}"
             )
             java_unpack_path.rename(self.command.tools_path / "java")
 
     def uninstall(self):
         """Uninstall a JDK."""
```

### Comparing `briefcase-0.3.8/src/briefcase/integrations/subprocess.py` & `briefcase-0.3.9/src/briefcase/integrations/subprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import operator
 import os
 import shlex
 import subprocess
 import sys
 import threading
 import time
+from pathlib import Path
 
 import psutil
 
 from briefcase.console import Log
 from briefcase.exceptions import CommandOutputParseError
 
 
@@ -213,14 +214,15 @@
         if stream_output or (
             self.command.input.is_output_controlled and not is_output_redirected
         ):
             return self._run_and_stream_output(args, **kwargs)
 
         # Otherwise, invoke run() normally.
         self._log_command(args)
+        self._log_cwd(kwargs.get("cwd"))
         self._log_environment(kwargs.get("env"))
 
         try:
             command_result = self._subprocess.run(
                 [str(arg) for arg in args], **self.final_kwargs(**kwargs)
             )
         except subprocess.CalledProcessError as e:
@@ -262,21 +264,24 @@
                 f"with `stream_output` or while dynamic Rich content is active."
             )
 
         # stdout must be piped so the output streamer can print it.
         kwargs["stdout"] = subprocess.PIPE
         # if stderr isn't explicitly redirected, then send it to stdout.
         kwargs.setdefault("stderr", subprocess.STDOUT)
+        # use line-buffered output by default
+        kwargs.setdefault("bufsize", 1)
 
         stderr = None
         with self.Popen(args, **kwargs) as process:
             self.stream_output(args[0], process)
             if process.stderr and kwargs["stderr"] != subprocess.STDOUT:
                 stderr = process.stderr.read()
             return_code = process.poll()
+        self._log_return_code(return_code)
 
         if check and return_code:
             raise subprocess.CalledProcessError(return_code, args, stderr=stderr)
 
         return subprocess.CompletedProcess(args, return_code, stderr=stderr)
 
     def check_output(self, args, **kwargs):
@@ -287,14 +292,15 @@
          - If the `env` is argument provided, the current system environment
            will be copied, and the contents of env overwritten into that
            environment.
          - The `text` argument is defaulted to True so all output
            is returned as strings instead of bytes.
         """
         self._log_command(args)
+        self._log_cwd(kwargs.get("cwd"))
         self._log_environment(kwargs.get("env"))
 
         try:
             cmd_output = self._subprocess.check_output(
                 [str(arg) for arg in args], **self.final_kwargs(**kwargs)
             )
         except subprocess.CalledProcessError as e:
@@ -351,21 +357,22 @@
          - If the `env` argument is provided, the current system environment
            will be copied, and the contents of env overwritten into that
            environment.
          - The `text` argument is defaulted to True so all output
            is returned as strings instead of bytes.
         """
         self._log_command(args)
+        self._log_cwd(kwargs.get("cwd"))
         self._log_environment(kwargs.get("env"))
 
         return self._subprocess.Popen(
             [str(arg) for arg in args], **self.final_kwargs(**kwargs)
         )
 
-    def stream_output(self, label, popen_process, stop_func=None):
+    def stream_output(self, label, popen_process, stop_func=lambda: False):
         """Stream the output of a Popen process until the process exits. If the
         user sends CTRL+C, the process will be terminated.
 
         This is useful for starting a process via Popen such as tailing a
         log file, then initiating a non-blocking process that populates that
         log, and finally streaming the original process's output here.
 
@@ -375,47 +382,49 @@
         :param stop_func: a Callable that returns True when output streaming
             should stop and the popen_process should be terminated.
         """
         output_streamer = threading.Thread(
             name=f"{label} output streamer",
             target=self._stream_output_thread,
             args=(popen_process,),
+            daemon=True,
         )
         try:
             output_streamer.start()
-            if stop_func:
-                while output_streamer.is_alive() and not stop_func():
-                    time.sleep(0.1)
-            else:
-                output_streamer.join()
+            # joining the thread is avoided due to demonstrated
+            # instability of thread interruption via CTRL+C (#809)
+            while not stop_func() and output_streamer.is_alive():
+                time.sleep(0.1)
         except KeyboardInterrupt:
-            pass  # allow CTRL+C to gracefully stop streaming
+            self.command.logger.info("Stopping...")
+            # allow time for CTRL+C to propagate to the child process
+            time.sleep(0.25)
         finally:
             self.cleanup(label, popen_process)
-            output_streamer.join()
+            streamer_deadline = time.time() + 3
+            while output_streamer.is_alive() and time.time() < streamer_deadline:
+                time.sleep(0.1)
+            if output_streamer.is_alive():
+                self.command.logger.error(
+                    "Log stream hasn't terminated; log output may be corrupted."
+                )
 
     def _stream_output_thread(self, popen_process):
         """Stream output for a Popen process in a Thread.
 
         :param popen_process: popen process to stream stdout
         """
         while True:
             # readline should always return at least a newline (ie \n)
             # UNLESS the underlying process is exiting/gone; then "" is returned
             output_line = ensure_str(popen_process.stdout.readline())
             if output_line:
                 self.command.logger.info(output_line)
             elif output_line == "":
-                # a return code will be available once the process returns one to the OS.
-                # by definition, that should mean the process has exited.
-                return_code = popen_process.poll()
-                # only return once all output has been read and the process has exited.
-                if return_code is not None:
-                    self._log_return_code(return_code)
-                    return
+                return
 
     def cleanup(self, label, popen_process):
         """Clean up after a Popen process, gracefully terminating if possible;
         forcibly if not.
 
         :param label: A description of the content being streamed; used for
             to provide context in logging messages.
@@ -432,14 +441,20 @@
         """Log the entire console command being executed."""
         self.command.logger.debug()
         self.command.logger.debug("Running Command:")
         self.command.logger.debug(
             f"    {' '.join(shlex.quote(str(arg)) for arg in args)}"
         )
 
+    def _log_cwd(self, cwd):
+        """Log the working directory for the  command being executed."""
+        effective_cwd = Path.cwd() if cwd is None else cwd
+        self.command.logger.debug("Working Directory:")
+        self.command.logger.debug(f"    {effective_cwd}")
+
     def _log_environment(self, overrides):
         """Log the environment variables overrides prior to command execution.
 
         :param overrides: The explicit environment passed to the subprocess call;
             can be `None` if there are no explicit environment changes.
         """
         if overrides:
```

### Comparing `briefcase-0.3.8/src/briefcase/integrations/wix.py` & `briefcase-0.3.9/src/briefcase/integrations/wix.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,16 +112,16 @@
             and self.light_exe.exists()
             and self.candle_exe.exists()
         )
 
     @property
     def managed_install(self):
         try:
-            # Determine if wix_home is relative to the .briefcase folder.
-            # If wix_home isn't inside .briefcase, this will raise a ValueError,
+            # Determine if wix_home is relative to the briefcase data directory.
+            # If wix_home isn't inside this directory, this will raise a ValueError,
             # indicating it is a non-managed install.
             self.wix_home.relative_to(self.command.tools_path)
             return True
         except ValueError:
             return False
 
     def install(self):
```

### Comparing `briefcase-0.3.8/src/briefcase/integrations/xcode.py` & `briefcase-0.3.9/src/briefcase/integrations/xcode.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/src/briefcase/platforms/__init__.py` & `briefcase-0.3.9/src/briefcase/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/src/briefcase/platforms/android/gradle.py` & `briefcase-0.3.9/src/briefcase/platforms/android/gradle.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 import subprocess
+import time
 
 from briefcase.commands import (
     BuildCommand,
     CreateCommand,
     PackageCommand,
     PublishCommand,
     RunCommand,
@@ -208,28 +209,29 @@
         with self.input.wait_bar("Stopping old versions of the app..."):
             adb.force_stop_app(package)
 
         # Install the latest APK file onto the device.
         with self.input.wait_bar("Installing new app version..."):
             adb.install_apk(self.binary_path(app))
 
-        self.logger.info("Starting app...", prefix=app.app_name)
-        with self.input.wait_bar("Clearing device log..."):
-            adb.clear_log()
-
         # To start the app, we launch `org.beeware.android.MainActivity`.
         with self.input.wait_bar("Launching app..."):
             adb.start_app(package, "org.beeware.android.MainActivity")
+            pid = None
+            while not pid:
+                pid = adb.pidof(package)
+                if not pid:
+                    time.sleep(0.5)
 
         self.logger.info(
             "Following device log output (type CTRL-C to stop log)...",
             prefix=app.app_name,
         )
         self.logger.info("=" * 75)
-        adb.logcat()
+        adb.logcat(pid)
 
 
 class GradlePackageCommand(GradleMixin, PackageCommand):
     description = "Create an Android App Bundle and APK in release mode."
 
     def package_app(self, app: BaseConfig, **kwargs):
         """Package the app for distribution.
```

### Comparing `briefcase-0.3.8/src/briefcase/platforms/iOS/__init__.py` & `briefcase-0.3.9/src/briefcase/platforms/iOS/__init__.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/src/briefcase/platforms/iOS/xcode.py` & `briefcase-0.3.9/src/briefcase/platforms/iOS/xcode.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/src/briefcase/platforms/linux/appimage.py` & `briefcase-0.3.9/src/briefcase/platforms/linux/appimage.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     BuildCommand,
     CreateCommand,
     PackageCommand,
     PublishCommand,
     RunCommand,
     UpdateCommand,
 )
-from briefcase.config import BaseConfig
+from briefcase.config import AppConfig
 from briefcase.exceptions import BriefcaseCommandError
 from briefcase.integrations.docker import verify_docker
 from briefcase.integrations.linuxdeploy import LinuxDeploy
 from briefcase.platforms.linux import LinuxMixin
 
 
 class LinuxAppImageMixin(LinuxMixin):
@@ -117,15 +117,15 @@
         """The query arguments to use in a support package query request."""
         return [
             ("platform", self.platform),
             ("version", self.python_version_tag),
             ("arch", self.host_arch),
         ]
 
-    def install_app_dependencies(self, app: BaseConfig):
+    def install_app_dependencies(self, app: AppConfig):
         """Install application dependencies.
 
         This will be containerized in Docker to ensure that the right
         binary versions are installed.
         """
         with self.dockerize(app=app) as docker:
             docker.prepare()
@@ -138,60 +138,104 @@
     description = "Update an existing Linux AppImage."
 
 
 class LinuxAppImageBuildCommand(LinuxAppImageMixin, BuildCommand):
     description = "Build a Linux AppImage."
 
     def verify_tools(self):
+        """Verify that the AppImage linuxdeploy tool and plugins exist.
+
+        :param app: The application to build
+        """
         super().verify_tools()
         self.linuxdeploy = LinuxDeploy.verify(self)
 
-    def build_app(self, app: BaseConfig, **kwargs):
+    def build_app(self, app: AppConfig, **kwargs):
         """Build an application.
 
         :param app: The application to build
         """
-        self.logger.info("Building AppImage...", prefix=app.app_name)
+        # Build a dictionary of environment definitions that are required
+        env = {}
+
+        self.logger.info("Checking for Linuxdeploy plugins...", prefix=app.app_name)
+        try:
+            plugins = self.linuxdeploy.verify_plugins(
+                app.linuxdeploy_plugins,
+                bundle_path=self.bundle_path(app),
+            )
 
+            self.logger.info("Configuring Linuxdeploy plugins...", prefix=app.app_name)
+            # We need to add the location of the linuxdeploy plugins to the PATH.
+            # However, if we arerunning inside Docker, we need to know the
+            # environment *inside* the Docker container.
+            if self.use_docker:
+                echo_cmd = ["/bin/bash", "-c", "echo $PATH"]
+                base_path = self.Docker(self, app).check_output(echo_cmd).strip()
+            else:
+                base_path = self.os.environ["PATH"]
+
+            # Add any plugin-required environment variables
+            for plugin in plugins.values():
+                env.update(plugin.env)
+
+            # Construct a path that has been prepended with the path to the plugins
+            env["PATH"] = os.pathsep.join(
+                [os.fsdecode(plugin.file_path) for plugin in plugins.values()]
+                + [base_path]
+            )
+        except AttributeError:
+            self.logger.info("No linuxdeploy plugins configured.")
+            plugins = {}
+
+        self.logger.info("Building AppImage...", prefix=app.app_name)
         with self.input.wait_bar("Building..."):
             try:
-                # Build the AppImage.
                 # For some reason, the version has to be passed in as an
-                # environment variable, *not* in the configuration...
-                env = {"VERSION": app.version}
+                # environment variable, *not* in the configuration.
+                env["VERSION"] = app.version
+                # The internals of the binary aren't inherently visible, so
+                # there's no need to package copyright files. These files
+                # appear to be missing by default in the OS dev packages anyway,
+                # so this effectively silences a bunch of warnings that can't
+                # be easily resolved by the end user.
+                env["DISABLE_COPYRIGHT_FILES_DEPLOYMENT"] = "1"
 
                 # Find all the .so files in app and app_packages,
                 # so they can be passed in to linuxdeploy to have their
                 # dependencies added to the AppImage. Looks for any .so file
                 # in the application, and make sure it is marked for deployment.
-                so_folders = set()
-                for so_file in self.appdir_path(app).glob("**/*.so"):
-                    so_folders.add(so_file.parent)
+                so_folders = {
+                    so_file.parent for so_file in self.appdir_path(app).glob("**/*.so")
+                }
 
-                deploy_deps_args = []
+                additional_args = []
                 for folder in sorted(so_folders):
-                    deploy_deps_args.extend(["--deploy-deps-only", str(folder)])
+                    additional_args.extend(["--deploy-deps-only", str(folder)])
+
+                for plugin in plugins:
+                    additional_args.extend(["--plugin", plugin])
 
                 # Build the app image. We use `--appimage-extract-and-run`
                 # because AppImages won't run natively inside Docker.
                 with self.dockerize(app) as docker:
                     docker.run(
                         [
-                            self.linuxdeploy.appimage_path,
+                            self.linuxdeploy.file_path / self.linuxdeploy.file_name,
                             "--appimage-extract-and-run",
                             f"--appdir={self.appdir_path(app)}",
                             "-d",
                             os.fsdecode(
                                 self.appdir_path(app)
                                 / f"{app.bundle}.{app.app_name}.desktop"
                             ),
                             "-o",
                             "appimage",
                         ]
-                        + deploy_deps_args,
+                        + additional_args,
                         env=env,
                         check=True,
                         cwd=self.platform_path,
                     )
 
                 # Make the binary executable.
                 self.os.chmod(self.binary_path(app), 0o755)
@@ -206,33 +250,34 @@
 
     def verify_tools(self):
         """Verify that we're on Linux."""
         super().verify_tools()
         if self.host_os != "Linux":
             raise BriefcaseCommandError("AppImages can only be executed on Linux.")
 
-    def run_app(self, app: BaseConfig, **kwargs):
+    def run_app(self, app: AppConfig, **kwargs):
         """Start the application.
 
         :param app: The config object for the app
         """
         self.logger.info("Starting app...", prefix=app.app_name)
         try:
             self.subprocess.run(
                 [
                     os.fsdecode(self.binary_path(app)),
                 ],
                 check=True,
+                cwd=self.home_path,
             )
         except subprocess.CalledProcessError as e:
             raise BriefcaseCommandError(f"Unable to start app {app.app_name}.") from e
 
 
 class LinuxAppImagePackageCommand(LinuxAppImageMixin, PackageCommand):
-    description = "Publish a Linux AppImage."
+    description = "Package a Linux AppImage."
 
 
 class LinuxAppImagePublishCommand(LinuxAppImageMixin, PublishCommand):
     description = "Publish a Linux AppImage."
 
 
 # Declare the briefcase command bindings
```

### Comparing `briefcase-0.3.8/src/briefcase/platforms/macOS/__init__.py` & `briefcase-0.3.9/src/briefcase/platforms/macOS/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,15 @@
             try:
                 self.subprocess.run(
                     [
                         "open",
                         "-n",  # Force a new app to be launched
                         os.fsdecode(self.binary_path(app)),
                     ],
+                    cwd=self.home_path,
                     check=True,
                 )
             except subprocess.CalledProcessError:
                 raise BriefcaseCommandError(f"Unable to start app {app.app_name}.")
 
             # Find the App process ID so log streaming can exit when the app exits
             app_pid = get_process_id_by_command(
```

### Comparing `briefcase-0.3.8/src/briefcase/platforms/macOS/app.py` & `briefcase-0.3.9/src/briefcase/platforms/macOS/app.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/src/briefcase/platforms/macOS/xcode.py` & `briefcase-0.3.9/src/briefcase/platforms/macOS/xcode.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/src/briefcase/platforms/windows/msi.py` & `briefcase-0.3.9/src/briefcase/platforms/windows/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,31 @@
 import os
 import struct
 import subprocess
-import sys
 import uuid
 
-from briefcase.commands import (
-    BuildCommand,
-    CreateCommand,
-    PackageCommand,
-    PublishCommand,
-    RunCommand,
-    UpdateCommand,
-)
+from briefcase.commands import CreateCommand, PackageCommand, RunCommand
 from briefcase.config import BaseConfig, parsed_version
 from briefcase.exceptions import BriefcaseCommandError
 from briefcase.integrations.wix import WiX
-from briefcase.platforms.windows import WindowsMixin
 
+DEFAULT_OUTPUT_FORMAT = "app"
 
-class WindowsMSIMixin(WindowsMixin):
-    output_format = "msi"
+
+class WindowsMixin:
+    platform = "windows"
 
     def binary_path(self, app):
-        return self.bundle_path(app)
+        return self.bundle_path(app) / self.packaging_root / f"{app.formal_name}.exe"
 
     def distribution_path(self, app, packaging_format):
         return self.platform_path / f"{app.formal_name}-{app.version}.msi"
 
-    def verify_tools(self):
-        super().verify_tools()
-        self.wix = WiX.verify(self)
-
-
-class WindowsMSICreateCommand(WindowsMSIMixin, CreateCommand):
-    description = "Create and populate a Windows app."
 
+class WindowsCreateCommand(CreateCommand):
     @property
     def support_package_url_query(self):
         """The query arguments to use in a support package query request."""
         return [
             ("platform", self.platform),
             ("version", self.python_version_tag),
             ("arch", "amd64" if (struct.calcsize("P") * 8) == 64 else "win32"),
@@ -73,90 +60,71 @@
             domain = ".".join([app.app_name] + app.bundle.split(".")[::-1])
             guid = uuid.uuid5(uuid.NAMESPACE_DNS, domain)
             self.logger.info(f"Assigning {app.app_name} an application GUID of {guid}")
 
         try:
             install_scope = "perMachine" if app.system_installer else "perUser"
         except AttributeError:
-            # system_installer not defined in config; default to perUser install.
-            install_scope = "perUser"
+            # system_installer not defined in config; default to asking the user
+            install_scope = None
 
         return {
             "version_triple": version_triple,
             "guid": str(guid),
             "install_scope": install_scope,
         }
 
-    def install_app_support_package(self, app: BaseConfig):
-        """Install, then modify the default support package."""
-        # Install the support package using the normal install logic.
-        super().install_app_support_package(app)
-
-        # We need to add a ._pth file to include app and app_packages as
-        # part of the standard PYTHONPATH. Write a _pth file directly into
-        # the support folder, overwriting the default one.
-        version_tag = f"{sys.version_info.major}{sys.version_info.minor}"
-        pth_file = self.support_path(app) / f"python{version_tag}._pth"
-        with pth_file.open("w") as f:
-            f.write(f"python{version_tag}.zip\n")
-            f.write(".\n")
-            f.write("..\\\\app\n")
-            f.write("..\\\\app_packages\n")
-
-
-class WindowsMSIUpdateCommand(WindowsMSIMixin, UpdateCommand):
-    description = "Update an existing Windows app."
-
-
-class WindowsMSIBuildCommand(WindowsMSIMixin, BuildCommand):
-    description = "Build a Windows app."
-
-
-class WindowsMSIRunCommand(WindowsMSIMixin, RunCommand):
-    description = "Run a Windows app."
 
+class WindowsRunCommand(RunCommand):
     def run_app(self, app: BaseConfig, **kwargs):
         """Start the application.
 
         :param app: The config object for the app
         """
         self.logger.info("Starting app...", prefix=app.app_name)
         try:
+            # Start streaming logs for the app.
+            self.logger.info("=" * 75)
             self.subprocess.run(
-                [
-                    os.fsdecode(
-                        self.binary_path(app) / "src" / "python" / "pythonw.exe"
-                    ),
-                    "-m",
-                    app.module_name,
-                ],
+                [os.fsdecode(self.binary_path(app))],
+                cwd=self.home_path,
                 check=True,
             )
         except subprocess.CalledProcessError as e:
             raise BriefcaseCommandError(f"Unable to start app {app.app_name}.") from e
 
 
-class WindowsMSIPackageCommand(WindowsMSIMixin, PackageCommand):
-    description = "Package an MSI for a Windows app."
+class WindowsPackageCommand(PackageCommand):
+    @property
+    def packaging_formats(self):
+        return ["msi"]
+
+    @property
+    def default_packaging_format(self):
+        return "msi"
+
+    def verify_tools(self):
+        super().verify_tools()
+        self.wix = WiX.verify(self)
 
     def package_app(self, app: BaseConfig, **kwargs):
-        """Build an application.
+        """Package an application.
 
-        :param app: The application to build
+        :param app: The application to package
         """
         self.logger.info("Building MSI...", prefix=app.app_name)
 
         try:
             self.logger.info("Compiling application manifest...")
             with self.input.wait_bar("Compiling..."):
                 self.subprocess.run(
                     [
                         self.wix.heat_exe,
                         "dir",
-                        "src",
+                        os.fsdecode(self.packaging_root),
                         "-nologo",  # Don't display startup text
                         "-gg",  # Generate GUIDs
                         "-sfrag",  # Suppress fragment generation for directories
                         "-sreg",  # Suppress registry harvesting
                         "-srd",  # Suppress harvesting the root directory
                         "-scom",  # Suppress harvesting COM components
                         "-dr",
@@ -183,15 +151,17 @@
                     [
                         self.wix.candle_exe,
                         "-nologo",  # Don't display startup text
                         "-ext",
                         "WixUtilExtension",
                         "-ext",
                         "WixUIExtension",
-                        "-dSourceDir=src",
+                        "-arch",
+                        "x64",
+                        f"-dSourceDir={self.packaging_root}",
                         f"{app.app_name}.wxs",
                         f"{app.app_name}-manifest.wxs",
                     ],
                     check=True,
                     cwd=self.bundle_path(app),
                 )
         except subprocess.CalledProcessError as e:
@@ -216,20 +186,7 @@
                         f"{app.app_name}-manifest.wixobj",
                     ],
                     check=True,
                     cwd=self.bundle_path(app),
                 )
         except subprocess.CalledProcessError as e:
             raise BriefcaseCommandError(f"Unable to link app {app.app_name}.") from e
-
-
-class WindowsMSIPublishCommand(WindowsMSIMixin, PublishCommand):
-    description = "Publish a Windows MSI."
-
-
-# Declare the briefcase command bindings
-create = WindowsMSICreateCommand  # noqa
-update = WindowsMSIUpdateCommand  # noqa
-build = WindowsMSIBuildCommand  # noqa
-run = WindowsMSIRunCommand  # noqa
-package = WindowsMSIPackageCommand  # noqa
-publish = WindowsMSIPublishCommand  # noqa
```

### Comparing `briefcase-0.3.8/src/briefcase.egg-info/PKG-INFO` & `briefcase-0.3.9/src/briefcase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: briefcase
-Version: 0.3.8
+Version: 0.3.9
 Summary: Tools to support converting a Python project into a standalone native application.
 Home-page: http://beeware.org/briefcase
 Author: Russell Keith-Magee
 Author-email: russell@keith-magee.com
 Maintainer: Russell Keith-Magee
 Maintainer-email: russell@keith-magee.com
 License: New BSD
```

### Comparing `briefcase-0.3.8/src/briefcase.egg-info/SOURCES.txt` & `briefcase-0.3.9/src/briefcase.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 docs/how-to/code-signing/images/Valid_certificate.png
 docs/how-to/code-signing/images/WWDR_certificate.png
 docs/how-to/internal/index.rst
 docs/how-to/internal/release.rst
 docs/how-to/publishing/android.rst
 docs/how-to/publishing/index.rst
 docs/reference/configuration.rst
+docs/reference/environment.rst
 docs/reference/index.rst
 docs/reference/commands/build.rst
 docs/reference/commands/create.rst
 docs/reference/commands/dev.rst
 docs/reference/commands/index.rst
 docs/reference/commands/new.rst
 docs/reference/commands/package.rst
@@ -61,20 +62,22 @@
 docs/reference/commands/run.rst
 docs/reference/commands/update.rst
 docs/reference/commands/upgrade.rst
 docs/reference/platforms/android.rst
 docs/reference/platforms/iOS.rst
 docs/reference/platforms/index.rst
 docs/reference/platforms/linux/appimage.rst
+docs/reference/platforms/linux/flatpak.rst
 docs/reference/platforms/linux/index.rst
 docs/reference/platforms/macOS/app.rst
 docs/reference/platforms/macOS/index.rst
 docs/reference/platforms/macOS/xcode.rst
+docs/reference/platforms/windows/app.rst
 docs/reference/platforms/windows/index.rst
-docs/reference/platforms/windows/msi.rst
+docs/reference/platforms/windows/visualstudio.rst
 docs/tutorial/index.rst
 src/briefcase/__init__.py
 src/briefcase/__main__.py
 src/briefcase/cmdline.py
 src/briefcase/config.py
 src/briefcase/console.py
 src/briefcase/exceptions.py
@@ -96,18 +99,21 @@
 src/briefcase/commands/run.py
 src/briefcase/commands/update.py
 src/briefcase/commands/upgrade.py
 src/briefcase/integrations/__init__.py
 src/briefcase/integrations/android_sdk.py
 src/briefcase/integrations/cookiecutter.py
 src/briefcase/integrations/docker.py
+src/briefcase/integrations/flatpak.py
 src/briefcase/integrations/git.py
 src/briefcase/integrations/java.py
 src/briefcase/integrations/linuxdeploy.py
+src/briefcase/integrations/rcedit.py
 src/briefcase/integrations/subprocess.py
+src/briefcase/integrations/visualstudio.py
 src/briefcase/integrations/wix.py
 src/briefcase/integrations/xcode.py
 src/briefcase/platforms/__init__.py
 src/briefcase/platforms/android/__init__.py
 src/briefcase/platforms/android/gradle.py
 src/briefcase/platforms/django/__init__.py
 src/briefcase/platforms/django/app.py
@@ -127,31 +133,34 @@
 src/briefcase/platforms/tvOS/__init__.py
 src/briefcase/platforms/tvOS/xcode.py
 src/briefcase/platforms/watchOS/__init__.py
 src/briefcase/platforms/watchOS/xcode.py
 src/briefcase/platforms/wearos/__init__.py
 src/briefcase/platforms/wearos/gradle.py
 src/briefcase/platforms/windows/__init__.py
-src/briefcase/platforms/windows/msi.py
+src/briefcase/platforms/windows/app.py
+src/briefcase/platforms/windows/visualstudio.py
 tests/__init__.py
 tests/conftest.py
 tests/test_cmdline.py
 tests/utils.py
 tests/apps/verify-ppb.config
 tests/apps/verify-pyside2.config
 tests/apps/verify-pyside6.config
 tests/apps/verify-toga.config
 tests/commands/__init__.py
 tests/commands/base/__init__.py
 tests/commands/base/conftest.py
 tests/commands/base/test_app_module_path.py
+tests/commands/base/test_check_obsolete_data_dir.py
 tests/commands/base/test_download_url.py
 tests/commands/base/test_full_options.py
 tests/commands/base/test_parse_config.py
 tests/commands/base/test_parse_options.py
+tests/commands/base/test_paths.py
 tests/commands/base/test_properties.py
 tests/commands/base/test_update_cookiecutter_cache.py
 tests/commands/base/test_verify_tools.py
 tests/commands/build/__init__.py
 tests/commands/build/conftest.py
 tests/commands/build/test_call.py
 tests/commands/create/__init__.py
@@ -229,20 +238,20 @@
 tests/console/Console/test_text_input.py
 tests/console/Console/test_wait_bar.py
 tests/integrations/__init__.py
 tests/integrations/android_sdk/__init__.py
 tests/integrations/android_sdk/conftest.py
 tests/integrations/android_sdk/ADB/__init__.py
 tests/integrations/android_sdk/ADB/test_avd_name.py
-tests/integrations/android_sdk/ADB/test_clear_log.py
 tests/integrations/android_sdk/ADB/test_command.py
 tests/integrations/android_sdk/ADB/test_force_stop_app.py
 tests/integrations/android_sdk/ADB/test_has_booted.py
 tests/integrations/android_sdk/ADB/test_install_apk.py
 tests/integrations/android_sdk/ADB/test_logcat.py
+tests/integrations/android_sdk/ADB/test_pidof.py
 tests/integrations/android_sdk/ADB/test_start_app.py
 tests/integrations/android_sdk/ADB/adb_errors/arbitrary-adb-error-unknown-command.out
 tests/integrations/android_sdk/ADB/adb_errors/arbitrary-adb-error-unknown-command.returncode
 tests/integrations/android_sdk/ADB/adb_errors/device-not-found.out
 tests/integrations/android_sdk/ADB/adb_errors/device-not-found.returncode
 tests/integrations/android_sdk/AndroidSDK/__init__.py
 tests/integrations/android_sdk/AndroidSDK/test_avd_config.py
@@ -263,26 +272,48 @@
 tests/integrations/android_sdk/AndroidSDK/test_verify_system_image.py
 tests/integrations/android_sdk/AndroidSDK/devices/daemon_start.out
 tests/integrations/android_sdk/AndroidSDK/devices/multiple_devices.out
 tests/integrations/android_sdk/AndroidSDK/devices/no_devices.out
 tests/integrations/android_sdk/AndroidSDK/devices/one_emulator.out
 tests/integrations/docker/__init__.py
 tests/integrations/docker/conftest.py
+tests/integrations/docker/test_Docker___dockerize_path.py
+tests/integrations/docker/test_Docker__check_output.py
 tests/integrations/docker/test_Docker__prepare.py
 tests/integrations/docker/test_Docker__run.py
 tests/integrations/docker/test_verify_docker.py
+tests/integrations/flatpak/__init__.py
+tests/integrations/flatpak/conftest.py
+tests/integrations/flatpak/test_Flatpak__build.py
+tests/integrations/flatpak/test_Flatpak__bundle.py
+tests/integrations/flatpak/test_Flatpak__run.py
+tests/integrations/flatpak/test_Flatpak__verify.py
+tests/integrations/flatpak/test_Flatpak__verify_repo.py
+tests/integrations/flatpak/test_Flatpak__verify_runtime.py
 tests/integrations/java/__init__.py
 tests/integrations/java/test_JDK__verify.py
 tests/integrations/java/test_JDK_upgrade.py
 tests/integrations/linuxdeploy/__init__.py
-tests/integrations/linuxdeploy/test_LinuxDeploy__patch_elf_binary.py
+tests/integrations/linuxdeploy/conftest.py
+tests/integrations/linuxdeploy/test_LinuxDeployBase__patch_elf_binary.py
+tests/integrations/linuxdeploy/test_LinuxDeployBase__upgrade.py
+tests/integrations/linuxdeploy/test_LinuxDeployBase__verify.py
+tests/integrations/linuxdeploy/test_LinuxDeployGtkPlugin__properties.py
+tests/integrations/linuxdeploy/test_LinuxDeployLocalFilePlugin__properties.py
+tests/integrations/linuxdeploy/test_LinuxDeployLocalFilePlugin__verify.py
+tests/integrations/linuxdeploy/test_LinuxDeployQtPlugin__properties.py
+tests/integrations/linuxdeploy/test_LinuxDeployURLPlugin__properties.py
+tests/integrations/linuxdeploy/test_LinuxDeployURLPlugin__verify.py
 tests/integrations/linuxdeploy/test_LinuxDeploy__properties.py
-tests/integrations/linuxdeploy/test_LinuxDeploy__upgrade.py
-tests/integrations/linuxdeploy/test_LinuxDeploy__verify.py
+tests/integrations/linuxdeploy/test_LinuxDeploy__verify_plugins.py
 tests/integrations/linuxdeploy/utils.py
+tests/integrations/rcedit/__init__.py
+tests/integrations/rcedit/test_RCEdit__properties.py
+tests/integrations/rcedit/test_RCEdit__upgrade.py
+tests/integrations/rcedit/test_RCEdit__verify.py
 tests/integrations/subprocess/__init__.py
 tests/integrations/subprocess/conftest.py
 tests/integrations/subprocess/test_Subprocess__Popen.py
 tests/integrations/subprocess/test_Subprocess__check_output.py
 tests/integrations/subprocess/test_Subprocess__cleanup.py
 tests/integrations/subprocess/test_Subprocess__final_kwargs.py
 tests/integrations/subprocess/test_Subprocess__parse_output.py
@@ -291,14 +322,17 @@
 tests/integrations/subprocess/test_Subprocess__run_in_wait_bar.py
 tests/integrations/subprocess/test_Subprocess__stream_output.py
 tests/integrations/subprocess/test_creationflag_constants.py
 tests/integrations/subprocess/test_ensure_str.py
 tests/integrations/subprocess/test_get_process_id_by_command.py
 tests/integrations/subprocess/test_is_process_dead.py
 tests/integrations/subprocess/test_json_parser.py
+tests/integrations/visualstudio/__init__.py
+tests/integrations/visualstudio/test_VisualStudio__properties.py
+tests/integrations/visualstudio/test_VisualStudio__verify.py
 tests/integrations/wix/__init__.py
 tests/integrations/wix/test_WiX__upgrade.py
 tests/integrations/wix/test_WiX__verify.py
 tests/integrations/xcode/__init__.py
 tests/integrations/xcode/test_confirm_xcode_license_accepted.py
 tests/integrations/xcode/test_ensure_command_line_tools_are_installed.py
 tests/integrations/xcode/test_ensure_xcode_is_installed.py
@@ -338,14 +372,20 @@
 tests/platforms/iOS/xcode/mixin/test_select_target_device.py
 tests/platforms/linux/__init__.py
 tests/platforms/linux/appimage/__init__.py
 tests/platforms/linux/appimage/test_build.py
 tests/platforms/linux/appimage/test_create.py
 tests/platforms/linux/appimage/test_mixin.py
 tests/platforms/linux/appimage/test_run.py
+tests/platforms/linux/flatpak/__init__.py
+tests/platforms/linux/flatpak/test_build.py
+tests/platforms/linux/flatpak/test_create.py
+tests/platforms/linux/flatpak/test_mixin.py
+tests/platforms/linux/flatpak/test_package.py
+tests/platforms/linux/flatpak/test_run.py
 tests/platforms/macOS/__init__.py
 tests/platforms/macOS/app/__init__.py
 tests/platforms/macOS/app/conftest.py
 tests/platforms/macOS/app/test_build.py
 tests/platforms/macOS/app/test_create.py
 tests/platforms/macOS/app/test_mixin.py
 tests/platforms/macOS/app/test_package.py
@@ -355,12 +395,17 @@
 tests/platforms/macOS/app/test_signing.py
 tests/platforms/macOS/xcode/__init__.py
 tests/platforms/macOS/xcode/test_build.py
 tests/platforms/macOS/xcode/test_mixin.py
 tests/platforms/macOS/xcode/test_package.py
 tests/platforms/macOS/xcode/test_run.py
 tests/platforms/windows/__init__.py
-tests/platforms/windows/msi/__init__.py
-tests/platforms/windows/msi/test_create.py
-tests/platforms/windows/msi/test_mixin.py
-tests/platforms/windows/msi/test_package.py
-tests/platforms/windows/msi/test_run.py
+tests/platforms/windows/app/__init__.py
+tests/platforms/windows/app/test_build.py
+tests/platforms/windows/app/test_create.py
+tests/platforms/windows/app/test_mixin.py
+tests/platforms/windows/app/test_package.py
+tests/platforms/windows/app/test_run.py
+tests/platforms/windows/visualstudio/test_build.py
+tests/platforms/windows/visualstudio/test_mixin.py
+tests/platforms/windows/visualstudio/test_package.py
+tests/platforms/windows/visualstudio/test_run.py
```

### Comparing `briefcase-0.3.8/src/briefcase.egg-info/entry_points.txt` & `briefcase-0.3.9/src/briefcase.egg-info/entry_points.txt`

 * *Files 24% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 gradle = briefcase.platforms.android.gradle
 
 [briefcase.formats.ios]
 xcode = briefcase.platforms.iOS.xcode
 
 [briefcase.formats.linux]
 appimage = briefcase.platforms.linux.appimage
+flatpak = briefcase.platforms.linux.flatpak
 
 [briefcase.formats.macos]
 app = briefcase.platforms.macOS.app
 homebrew = briefcase.platforms.macOS.homebrew
 xcode = briefcase.platforms.macOS.xcode
 
 [briefcase.formats.windows]
-msi = briefcase.platforms.windows.msi
+app = briefcase.platforms.windows.app
+visualstudio = briefcase.platforms.windows.visualstudio
 
 [briefcase.platforms]
 android = briefcase.platforms.android
 iOS = briefcase.platforms.iOS
 linux = briefcase.platforms.linux
 macOS = briefcase.platforms.macOS
 windows = briefcase.platforms.windows
```

### Comparing `briefcase-0.3.8/tests/commands/base/conftest.py` & `briefcase-0.3.9/tests/commands/base/conftest.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/base/test_app_module_path.py` & `briefcase-0.3.9/tests/commands/base/test_app_module_path.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/base/test_download_url.py` & `briefcase-0.3.9/tests/commands/base/test_download_url.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/base/test_full_options.py` & `briefcase-0.3.9/tests/commands/base/test_full_options.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/base/test_parse_config.py` & `briefcase-0.3.9/tests/commands/base/test_parse_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from briefcase.exceptions import BriefcaseConfigError
 
 
 def test_missing_config(base_command):
     """If the configuration file doesn't exit, raise an error."""
     filename = base_command.base_path / "does_not_exist.toml"
-    with pytest.raises(BriefcaseConfigError, match="configuration file not found"):
+    with pytest.raises(BriefcaseConfigError, match="Configuration file not found"):
         base_command.parse_config(filename)
 
 
 def test_incomplete_global_config(base_command):
     """If the global configuration is missing a required argument, an error is
     raised."""
     # Provide a configuration that is missing `bundle`, a required attribute
```

### Comparing `briefcase-0.3.8/tests/commands/base/test_parse_options.py` & `briefcase-0.3.9/tests/commands/base/test_parse_options.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/base/test_properties.py` & `briefcase-0.3.9/tests/commands/base/test_properties.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/base/test_update_cookiecutter_cache.py` & `briefcase-0.3.9/tests/commands/base/test_update_cookiecutter_cache.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/build/conftest.py` & `briefcase-0.3.9/tests/commands/run/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,112 +1,123 @@
 import pytest
 
-from briefcase.commands import BuildCommand
+from briefcase.commands import RunCommand
 from briefcase.commands.base import full_options
 from briefcase.config import AppConfig
 
 
-class DummyBuildCommand(BuildCommand):
-    """A dummy build command that doesn't actually do anything.
+class DummyRunCommand(RunCommand):
+    """A dummy run command that doesn't actually do anything.
 
-    It only serves to track which actions would be performend.
+    It only serves to track which actions would be performed.
     """
 
     platform = "tester"
     output_format = "dummy"
-    description = "Dummy build command"
+    description = "Dummy run command"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, apps=[], **kwargs)
 
         self.actions = []
 
     def bundle_path(self, app):
-        return self.platform_path / f"{app.app_name}.dummy"
+        return self.platform_path / app.app_name
 
     def binary_path(self, app):
-        return self.platform_path / f"{app.app_name}.dummy.bin"
+        return self.platform_path / app.app_name / f"{app.app_name}.bin"
 
     def distribution_path(self, app, packaging_format):
         return self.platform_path / f"{app.app_name}.dummy.{packaging_format}"
 
-    def verify_tools(
-        self,
-    ):
+    def verify_tools(self):
         super().verify_tools()
         self.actions.append(("verify",))
 
-    def build_app(self, app, **kwargs):
-        self.actions.append(("build", app.app_name, kwargs))
-        return full_options({"build_state": app.app_name}, kwargs)
+    def run_app(self, app, **kwargs):
+        self.actions.append(("run", app.app_name, kwargs))
+        return full_options({"run_state": app.app_name}, kwargs)
 
     # These commands override the default behavior, simply tracking that
-    # they were invoked, rather than instantiating a Create/Update command.
+    # they were invoked, rather than instantiating a Create/Update/Build command.
     # This is for testing purposes.
     def create_command(self, app, **kwargs):
         self.actions.append(("create", app.app_name, kwargs))
         return full_options({"create_state": app.app_name}, kwargs)
 
     def update_command(self, app, **kwargs):
         self.actions.append(("update", app.app_name, kwargs))
         return full_options({"update_state": app.app_name}, kwargs)
 
+    def build_command(self, app, **kwargs):
+        self.actions.append(("build", app.app_name, kwargs))
+        return full_options({"build_state": app.app_name}, kwargs)
+
 
 @pytest.fixture
-def build_command(tmp_path):
-    return DummyBuildCommand(base_path=tmp_path)
+def run_command(tmp_path):
+    return DummyRunCommand(base_path=tmp_path)
 
 
 @pytest.fixture
 def first_app_config():
     return AppConfig(
         app_name="first",
         bundle="com.example",
         version="0.0.1",
         description="The first simple app",
         sources=["src/first"],
     )
 
 
 @pytest.fixture
-def first_app_unbuilt(first_app_config, tmp_path):
+def first_app_uncompiled(first_app_config, tmp_path):
     # The same fixture as first_app_config,
     # but ensures that the bundle for the app exists
-    (tmp_path / "tester").mkdir(parents=True, exist_ok=True)
-    with (tmp_path / "tester" / "first.dummy").open("w") as f:
-        f.write("first.bundle")
+    (tmp_path / "tester" / "first").mkdir(parents=True, exist_ok=True)
+    with (tmp_path / "tester" / "first" / "first.dummy").open("w") as f:
+        f.write("first.dummy")
 
     return first_app_config
 
 
 @pytest.fixture
-def first_app(first_app_unbuilt, tmp_path):
-    # The same fixture as first_app_config,
+def first_app(first_app_uncompiled, tmp_path):
+    # The same fixture as first_app_uncompiled,
     # but ensures that the binary for the app exists
-    with (tmp_path / "tester" / "first.dummy.bin").open("w") as f:
-        f.write("first.exe")
+    with (tmp_path / "tester" / "first" / "first.bin").open("w") as f:
+        f.write("first.bin")
 
-    return first_app_unbuilt
+    return first_app_uncompiled
 
 
 @pytest.fixture
 def second_app_config():
     return AppConfig(
         app_name="second",
         bundle="com.example",
         version="0.0.2",
         description="The second simple app",
         sources=["src/second"],
     )
 
 
 @pytest.fixture
-def second_app(second_app_config, tmp_path):
+def second_app_uncompiled(second_app_config, tmp_path):
     # The same fixture as second_app_config,
+    # but ensures that the bundle for the app exists
+    (tmp_path / "tester" / "second").mkdir(parents=True, exist_ok=True)
+    with (tmp_path / "tester" / "second" / "second.dummy").open("w") as f:
+        f.write("second.dummy")
+
+    return second_app_config
+
+
+@pytest.fixture
+def second_app(second_app_uncompiled, tmp_path):
+    # The same fixture as second_app_uncompiled,
     # but ensures that the binary for the app exists
     (tmp_path / "tester").mkdir(parents=True, exist_ok=True)
-    with (tmp_path / "tester" / "second.dummy").open("w") as f:
-        f.write("second.bundle")
-    with (tmp_path / "tester" / "second.dummy.bin").open("w") as f:
-        f.write("second.exe")
+    with (tmp_path / "tester" / "second" / "second.bin").open("w") as f:
+        f.write("second.bin")
 
-    return second_app_config
+    return second_app_uncompiled
```

### Comparing `briefcase-0.3.8/tests/commands/build/test_call.py` & `briefcase-0.3.9/tests/commands/build/test_call.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
     options = build_command.parse_options(["-u"])
 
     # Run the build command
     build_command(**options)
 
     # The right sequence of things will be done
     assert build_command.actions == [
-        # Verify
+        # Tools are verified
         ("verify",),
         # First App exists, but hasn't been built; it will updated then built.
         ("update", "first", {}),
         ("build", "first", {"update_state": "first"}),
         # Second app has been built before; it will be built again.
         ("update", "second", {"update_state": "first", "build_state": "first"}),
         ("build", "second", {"update_state": "second", "build_state": "first"}),
```

### Comparing `briefcase-0.3.8/tests/commands/create/conftest.py` & `briefcase-0.3.9/tests/commands/create/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -69,17 +69,15 @@
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.actions = []
 
-    def verify_tools(
-        self,
-    ):
+    def verify_tools(self):
         super().verify_tools()
         self.actions.append(("verify",))
 
     # Override all the body methods of a CreateCommand
     # with versions that we can use to track actions performed.
     def generate_app_template(self, app):
         self.actions.append(("generate", app))
@@ -101,16 +99,17 @@
     def install_app_resources(self, app):
         self.actions.append(("resources", app))
 
 
 @pytest.fixture
 def create_command(tmp_path, mock_git):
     return DummyCreateCommand(
-        base_path=tmp_path,
-        home_path=tmp_path,
+        base_path=tmp_path / "project",
+        home_path=tmp_path / "home",
+        data_path=tmp_path / "data",
         git=mock_git,
     )
 
 
 @pytest.fixture
 def tracking_create_command(tmp_path, mock_git):
     return TrackingCreateCommand(
@@ -151,37 +150,71 @@
 
 
 @pytest.fixture
 def bundle_path(myapp, tmp_path):
     # Return the bundle path for the app; however, as a side effect,
     # ensure that the app, app_packages and support target directories
     # exist, and the briefcase index file has been created.
-    bundle_path = tmp_path / "tester" / f"{myapp.app_name}.bundle"
+    bundle_path = tmp_path / "project" / "tester" / f"{myapp.app_name}.bundle"
     (bundle_path / "path" / "to" / "app").mkdir(parents=True, exist_ok=True)
-    (bundle_path / "path" / "to" / "app_packages").mkdir(parents=True, exist_ok=True)
     (bundle_path / "path" / "to" / "support").mkdir(parents=True, exist_ok=True)
+
+    return bundle_path
+
+
+@pytest.fixture
+def app_packages_path_index(bundle_path):
+    (bundle_path / "path" / "to" / "app_packages").mkdir(parents=True, exist_ok=True)
     with (bundle_path / "briefcase.toml").open("wb") as f:
         index = {
             "paths": {
                 "app_path": "path/to/app",
                 "app_packages_path": "path/to/app_packages",
                 "support_path": "path/to/support",
             }
         }
         tomli_w.dump(index, f)
 
-    return bundle_path
+
+@pytest.fixture
+def app_requirements_path_index(bundle_path):
+    with (bundle_path / "briefcase.toml").open("wb") as f:
+        index = {
+            "paths": {
+                "app_path": "path/to/app",
+                "app_requirements_path": "path/to/requirements.txt",
+                "support_path": "path/to/support",
+            }
+        }
+        tomli_w.dump(index, f)
+
+
+@pytest.fixture
+def no_support_path_index(bundle_path):
+    with (bundle_path / "briefcase.toml").open("wb") as f:
+        index = {
+            "paths": {
+                "app_path": "path/to/app",
+                "app_requirements_path": "path/to/requirements.txt",
+            }
+        }
+        tomli_w.dump(index, f)
 
 
 @pytest.fixture
 def support_path(bundle_path):
     return bundle_path / "path" / "to" / "support"
 
 
 @pytest.fixture
+def app_requirements_path(bundle_path):
+    return bundle_path / "path" / "to" / "requirements.txt"
+
+
+@pytest.fixture
 def app_packages_path(bundle_path):
     return bundle_path / "path" / "to" / "app_packages"
 
 
 @pytest.fixture
 def app_path(bundle_path):
     return bundle_path / "path" / "to" / "app"
```

### Comparing `briefcase-0.3.8/tests/commands/create/test_call.py` & `briefcase-0.3.9/tests/commands/create/test_call.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/create/test_cookiecutter_cache_path.py` & `briefcase-0.3.9/tests/commands/create/test_cookiecutter_cache_path.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/create/test_create_app.py` & `briefcase-0.3.9/tests/commands/create/test_create_app.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/create/test_generate_app_template.py` & `briefcase-0.3.9/tests/commands/create/test_generate_app_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import platform
 import subprocess
 from datetime import date
 from pathlib import Path
 from unittest import mock
 
 import pytest
 from cookiecutter import exceptions as cookiecutter_exceptions
@@ -26,14 +27,16 @@
         "author": "First Last",
         "author_email": "first@example.com",
         "requires": None,
         "icon": None,
         "splash": None,
         "supported": True,
         "document_types": {},
+        # Properties of the generating environment
+        "python_version": platform.python_version(),
         # Fields generated from other properties
         "module_name": "my_app",
         "package_name": "com.example",
         # Date-based fields added at time of generation
         "year": date.today().strftime("%Y"),
         "month": date.today().strftime("%B"),
         # Fields added by the output format.
```

### Comparing `briefcase-0.3.8/tests/commands/create/test_install_app_code.py` & `briefcase-0.3.9/tests/commands/create/test_install_app_code.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,20 @@
 Author: First Last
 Author-email: first@example.com
 Summary: This is a simple app
 """
         )
 
 
-def test_no_code(create_command, myapp, app_path):
+def test_no_code(
+    create_command,
+    myapp,
+    app_path,
+    app_requirements_path_index,
+):
     """If an app has no code (?!), install_app_code is mostly a no-op; but
     distinfo is created."""
     # Mock shutil so we can track usage.
     create_command.shutil = mock.MagicMock()
     create_command.os = mock.MagicMock()
 
     myapp.sources = None
@@ -50,15 +55,20 @@
     create_command.shutil.copytree.assert_not_called()
     create_command.shutil.copy.assert_not_called()
 
     # Metadata has been created
     assert_dist_info(app_path)
 
 
-def test_empty_code(create_command, myapp, app_path):
+def test_empty_code(
+    create_command,
+    myapp,
+    app_path,
+    app_requirements_path_index,
+):
     """If an app has an empty sources list (?!), install_app_code is mostly a
     no-op; but distinfo is created."""
     # Mock shutil so we can track usage.
     create_command.shutil = mock.MagicMock()
     create_command.os = mock.MagicMock()
 
     myapp.sources = []
@@ -71,45 +81,58 @@
     create_command.shutil.copytree.assert_not_called()
     create_command.shutil.copy.assert_not_called()
 
     # Metadata has been created
     assert_dist_info(app_path)
 
 
-def test_source_missing(create_command, myapp, app_path):
+def test_source_missing(
+    create_command,
+    myapp,
+    app_path,
+    app_requirements_path_index,
+):
     """If an app defines sources that are missing, an error is raised."""
     # Set the app definition to point at sources that don't exsit
     myapp.sources = ["missing"]
 
     with pytest.raises(MissingAppSources):
         create_command.install_app_code(myapp)
 
     # Distinfo won't be created.
     dist_info_path = app_path / "myapp-1.2.3.dist-info"
     assert not dist_info_path.exists()
 
 
-def test_source_dir(create_command, myapp, tmp_path, app_path):
+def test_source_dir(
+    create_command,
+    myapp,
+    tmp_path,
+    app_path,
+    app_requirements_path_index,
+):
     """If an app defines directories of sources, the whole directory is
     copied."""
     # Create the mock sources
     # src /
     #   first /
     #     demo.py
     #   second /
     #     shallow.py
     #     submodule /
     #       deeper.py
-    first_src = tmp_path / "src" / "first" / "demo.py"
+    first_src = tmp_path / "project" / "src" / "first" / "demo.py"
     first_src.parent.mkdir(parents=True)
     with (first_src).open("w") as f:
         f.write("print('hello first')\n")
 
-    second_shallow_src = tmp_path / "src" / "second" / "shallow.py"
-    second_deep_src = tmp_path / "src" / "second" / "submodule" / "deeper.py"
+    second_shallow_src = tmp_path / "project" / "src" / "second" / "shallow.py"
+    second_deep_src = (
+        tmp_path / "project" / "src" / "second" / "submodule" / "deeper.py"
+    )
     second_deep_src.parent.mkdir(parents=True)
     with (second_shallow_src).open("w") as f:
         f.write("print('hello shallow second')\n")
     with (second_deep_src).open("w") as f:
         f.write("print('hello deep second')\n")
 
     # Set the app definition, and install sources
@@ -127,27 +150,33 @@
     assert (app_path / "second" / "submodule").exists()
     assert (app_path / "second" / "submodule" / "deeper.py").exists()
 
     # Metadata has been created
     assert_dist_info(app_path)
 
 
-def test_source_file(create_command, myapp, tmp_path, app_path):
+def test_source_file(
+    create_command,
+    myapp,
+    tmp_path,
+    app_path,
+    app_requirements_path_index,
+):
     """If an app defines single file sources, the files are copied."""
     # Create the mock sources
     # src /
     #   first /
     #     demo.py
     #   other.py
-    first_src = tmp_path / "src" / "first" / "demo.py"
+    first_src = tmp_path / "project" / "src" / "first" / "demo.py"
     first_src.parent.mkdir(parents=True)
     with (first_src).open("w") as f:
         f.write("print('hello first')\n")
 
-    second_src = tmp_path / "src" / "other.py"
+    second_src = tmp_path / "project" / "src" / "other.py"
     with (second_src).open("w") as f:
         f.write("print('hello second')\n")
 
     # Set the app definition, and install sources
     myapp.sources = ["src/first/demo.py", "src/other.py"]
 
     create_command.install_app_code(myapp)
@@ -156,31 +185,39 @@
     assert (app_path / "demo.py").exists()
     assert (app_path / "other.py").exists()
 
     # Metadata has been created
     assert_dist_info(app_path)
 
 
-def test_replace_sources(create_command, myapp, tmp_path, app_path):
+def test_replace_sources(
+    create_command,
+    myapp,
+    tmp_path,
+    app_path,
+    app_requirements_path_index,
+):
     """Stale sources and dist-info are removed on installation."""
     # Create the mock sources
     # src /
     #   first /
     #     demo.py
     #   second /
     #     shallow.py
     #     submodule /
     #       deeper.py
-    first_src = tmp_path / "src" / "first" / "demo.py"
+    first_src = tmp_path / "project" / "src" / "first" / "demo.py"
     first_src.parent.mkdir(parents=True)
     with (first_src).open("w") as f:
         f.write("print('hello first')\n")
 
-    second_shallow_src = tmp_path / "src" / "second" / "shallow.py"
-    second_deep_src = tmp_path / "src" / "second" / "submodule" / "deeper.py"
+    second_shallow_src = tmp_path / "project" / "src" / "second" / "shallow.py"
+    second_deep_src = (
+        tmp_path / "project" / "src" / "second" / "submodule" / "deeper.py"
+    )
     second_deep_src.parent.mkdir(parents=True)
     with (second_shallow_src).open("w") as f:
         f.write("print('hello shallow second')\n")
     with (second_deep_src).open("w") as f:
         f.write("print('hello deep second')\n")
 
     # Also create some existing sources:
@@ -247,15 +284,20 @@
     assert not (app_path / "second" / "broken").exists()
 
     # Metadata has been updated.
     assert not (app_path / "my_app-1.2.2.dist-info").exists()
     assert_dist_info(app_path)
 
 
-def test_non_latin_metadata(create_command, myapp, app_path):
+def test_non_latin_metadata(
+    create_command,
+    myapp,
+    app_path,
+    app_requirements_path_index,
+):
     """If the app metadata contains non-Latin-1 characters, the METADATA file
     is written correctly (Briefcase#767)"""
     myapp.formal_name = "My büggy app"
     myapp.author = "José Weiß-Müller"
     myapp.author_email = "钱华林@中科院.中国"
     myapp.url = "https://xn--7qvx15a.cn"
     myapp.description = "A Møøse once bit my sister..."
```

### Comparing `briefcase-0.3.8/tests/commands/create/test_install_app_resources.py` & `briefcase-0.3.9/tests/commands/create/test_install_app_resources.py`

 * *Files 25% similar despite different names*

```diff
@@ -59,22 +59,34 @@
     install_image.assert_has_calls(
         [
             mock.call(
                 "application icon",
                 source="images/icon",
                 variant=None,
                 size="10",
-                target=tmp_path / "tester/my-app.bundle/path/to/icon-10.png",
+                target=tmp_path
+                / "project"
+                / "tester"
+                / "my-app.bundle"
+                / "path"
+                / "to"
+                / "icon-10.png",
             ),
             mock.call(
                 "application icon",
                 source="images/icon",
                 variant=None,
                 size="20",
-                target=tmp_path / "tester/my-app.bundle/path/to/icon-20.png",
+                target=tmp_path
+                / "project"
+                / "tester"
+                / "my-app.bundle"
+                / "path"
+                / "to"
+                / "icon-20.png",
             ),
         ],
         any_order=True,
     )
 
 
 def test_icon_variant_target(create_command, tmp_path):
@@ -116,29 +128,47 @@
     install_image.assert_has_calls(
         [
             mock.call(
                 "application icon",
                 source={"round": "images/round", "square": "images/square"},
                 variant=None,
                 size="round",  # This is expected for unsized variants
-                target=tmp_path / "tester/my-app.bundle/path/to/round.png",
+                target=tmp_path
+                / "project"
+                / "tester"
+                / "my-app.bundle"
+                / "path"
+                / "to"
+                / "round.png",
             ),
             mock.call(
                 "application icon",
                 source={"round": "images/round", "square": "images/square"},
                 variant="square",
                 size="10",
-                target=tmp_path / "tester/my-app.bundle/path/to/square-10.png",
+                target=tmp_path
+                / "project"
+                / "tester"
+                / "my-app.bundle"
+                / "path"
+                / "to"
+                / "square-10.png",
             ),
             mock.call(
                 "application icon",
                 source={"round": "images/round", "square": "images/square"},
                 variant="square",
                 size="20",
-                target=tmp_path / "tester/my-app.bundle/path/to/square-20.png",
+                target=tmp_path
+                / "project"
+                / "tester"
+                / "my-app.bundle"
+                / "path"
+                / "to"
+                / "square-20.png",
             ),
         ],
         any_order=True,
     )
 
 
 def test_splash_target(create_command, tmp_path):
@@ -173,22 +203,34 @@
     install_image.assert_has_calls(
         [
             mock.call(
                 "splash image",
                 source="images/splash",
                 variant=None,
                 size="10x20",
-                target=tmp_path / "tester/my-app.bundle/path/to/splash-10x20.png",
+                target=tmp_path
+                / "project"
+                / "tester"
+                / "my-app.bundle"
+                / "path"
+                / "to"
+                / "splash-10x20.png",
             ),
             mock.call(
                 "splash image",
                 source="images/splash",
                 variant=None,
                 size="20x30",
-                target=tmp_path / "tester/my-app.bundle/path/to/splash-20x30.png",
+                target=tmp_path
+                / "project"
+                / "tester"
+                / "my-app.bundle"
+                / "path"
+                / "to"
+                / "splash-20x30.png",
             ),
         ],
         any_order=True,
     )
 
 
 def test_splash_variant_target(create_command, tmp_path):
@@ -230,29 +272,47 @@
     install_image.assert_has_calls(
         [
             mock.call(
                 "splash image",
                 source={"portrait": "images/portrait", "landscape": "images/landscape"},
                 variant=None,
                 size="portrait",  # This is expected for unsized variants
-                target=tmp_path / "tester/my-app.bundle/path/to/portrait.png",
+                target=tmp_path
+                / "project"
+                / "tester"
+                / "my-app.bundle"
+                / "path"
+                / "to"
+                / "portrait.png",
             ),
             mock.call(
                 "splash image",
                 source={"portrait": "images/portrait", "landscape": "images/landscape"},
                 variant="landscape",
                 size="10x20",
-                target=tmp_path / "tester/my-app.bundle/path/to/landscape-10x20.png",
+                target=tmp_path
+                / "project"
+                / "tester"
+                / "my-app.bundle"
+                / "path"
+                / "to"
+                / "landscape-10x20.png",
             ),
             mock.call(
                 "splash image",
                 source={"portrait": "images/portrait", "landscape": "images/landscape"},
                 variant="landscape",
                 size="20x30",
-                target=tmp_path / "tester/my-app.bundle/path/to/landscape-20x30.png",
+                target=tmp_path
+                / "project"
+                / "tester"
+                / "my-app.bundle"
+                / "path"
+                / "to"
+                / "landscape-20x30.png",
             ),
         ],
         any_order=True,
     )
 
 
 def test_doctype_icon_target(create_command, tmp_path):
@@ -298,26 +358,44 @@
     install_image.assert_has_calls(
         [
             mock.call(
                 "icon for .mydoc documents",
                 source="images/mydoc-icon",
                 variant=None,
                 size=None,
-                target=tmp_path / "tester/my-app.bundle/path/to/mydoc-icon.png",
+                target=tmp_path
+                / "project"
+                / "tester"
+                / "my-app.bundle"
+                / "path"
+                / "to"
+                / "mydoc-icon.png",
             ),
             mock.call(
                 "icon for .other documents",
                 source="images/other-icon",
                 variant=None,
                 size="10",
-                target=tmp_path / "tester/my-app.bundle/path/to/other-icon-10.png",
+                target=tmp_path
+                / "project"
+                / "tester"
+                / "my-app.bundle"
+                / "path"
+                / "to"
+                / "other-icon-10.png",
             ),
             mock.call(
                 "icon for .other documents",
                 source="images/other-icon",
                 variant=None,
                 size="20",
-                target=tmp_path / "tester/my-app.bundle/path/to/other-icon-20.png",
+                target=tmp_path
+                / "project"
+                / "tester"
+                / "my-app.bundle"
+                / "path"
+                / "to"
+                / "other-icon-20.png",
             ),
         ],
         any_order=True,
     )
```

### Comparing `briefcase-0.3.8/tests/commands/create/test_install_image.py` & `briefcase-0.3.9/tests/commands/create/test_install_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 def test_no_requested_size(create_command, tmp_path, capsys):
     """If the app specifies a no-size image, an un-annotated image is used."""
     create_command.shutil = mock.MagicMock()
 
     # Create the source image
-    source_file = tmp_path / "input" / "original.png"
+    source_file = tmp_path / "project" / "input" / "original.png"
     source_file.parent.mkdir(parents=True, exist_ok=True)
     with source_file.open("w") as f:
         f.write("image")
 
     # Try to install the image
     out_path = tmp_path / "output.png"
     create_command.install_image(
@@ -47,26 +47,26 @@
         source="input/original",
         variant=None,
         size=None,
         target=out_path,
     )
 
     # The right message was written to output
-    expected = "\nInstalling input/original.png as sample image... done\n"
+    expected = "Installing input/original.png as sample image... done\n\n"
     assert capsys.readouterr().out == expected
 
     # The file was copied into position
     create_command.shutil.copy.assert_called_with(
         create_command.base_path / "input" / "original.png",
         out_path,
     )
 
 
 def test_no_requested_size_invalid_path(create_command, tmp_path, capsys):
-    """If the app specifies an no-size image that doesn't exist, an error is
+    """If the app specifies a no-size image that doesn't exist, an error is
     raised."""
     create_command.shutil = mock.MagicMock()
     create_command.shutil.copy.side_effect = FileNotFoundError
 
     # Try to install the image
     out_path = tmp_path / "output.png"
     create_command.install_image(
@@ -87,15 +87,15 @@
 
 def test_requested_size(create_command, tmp_path, capsys):
     """If the app specifies a sized image, an anoated image filename is
     used."""
     create_command.shutil = mock.MagicMock()
 
     # Create the source image
-    source_file = tmp_path / "input" / "original-3742.png"
+    source_file = tmp_path / "project" / "input" / "original-3742.png"
     source_file.parent.mkdir(parents=True, exist_ok=True)
     with source_file.open("w") as f:
         f.write("image")
 
     # Try to install the image
     out_path = tmp_path / "output.png"
     create_command.install_image(
@@ -103,15 +103,15 @@
         source="input/original",
         variant=None,
         size="3742",
         target=out_path,
     )
 
     # The right message was written to output
-    expected = "\nInstalling input/original-3742.png as 3742px sample image... done\n"
+    expected = "Installing input/original-3742.png as 3742px sample image... done\n\n"
     assert capsys.readouterr().out == expected
 
     # The file was copied into position
     create_command.shutil.copy.assert_called_with(
         create_command.base_path / "input" / "original-3742.png",
         out_path,
     )
@@ -143,15 +143,15 @@
 
 def test_variant_with_no_requested_size(create_command, tmp_path, capsys):
     """If the app specifies a variant with no size, the variant is used
     unsized."""
     create_command.shutil = mock.MagicMock()
 
     # Create the source image
-    source_file = tmp_path / "input" / "original.png"
+    source_file = tmp_path / "project" / "input" / "original.png"
     source_file.parent.mkdir(parents=True, exist_ok=True)
     with source_file.open("w") as f:
         f.write("image")
 
     # Try to install the image
     out_path = tmp_path / "output.png"
     create_command.install_image(
@@ -161,15 +161,15 @@
         },
         variant="round",
         size=None,
         target=out_path,
     )
 
     # The right message was written to output
-    expected = "\nInstalling input/original.png as round sample image... done\n"
+    expected = "Installing input/original.png as round sample image... done\n\n"
     assert capsys.readouterr().out == expected
 
     # The file was copied into position
     create_command.shutil.copy.assert_called_with(
         create_command.base_path / "input" / "original.png",
         out_path,
     )
@@ -179,15 +179,15 @@
     create_command, tmp_path, capsys
 ):
     """If the template specifies a variant with no size, but app doesn't have
     variants, a message is reported."""
     create_command.shutil = mock.MagicMock()
 
     # Create the source image
-    source_file = tmp_path / "input" / "original.png"
+    source_file = tmp_path / "project" / "input" / "original.png"
     source_file.parent.mkdir(parents=True, exist_ok=True)
     with source_file.open("w") as f:
         f.write("image")
 
     # Try to install the image
     out_path = tmp_path / "output.png"
     create_command.install_image(
@@ -207,15 +207,15 @@
 
 
 def test_unknown_variant_with_no_requested_size(create_command, tmp_path, capsys):
     """If the app specifies an unknown variant, an message is reported."""
     create_command.shutil = mock.MagicMock()
 
     # Create the source image
-    source_file = tmp_path / "input" / "original.png"
+    source_file = tmp_path / "project" / "input" / "original.png"
     source_file.parent.mkdir(parents=True, exist_ok=True)
     with source_file.open("w") as f:
         f.write("image")
 
     # Try to install the image
     out_path = tmp_path / "output.png"
     create_command.install_image(
@@ -238,15 +238,15 @@
 
 def test_variant_with_size(create_command, tmp_path, capsys):
     """If the app specifies a variant with a size, the sized variant is
     used."""
     create_command.shutil = mock.MagicMock()
 
     # Create the source image
-    source_file = tmp_path / "input" / "original-3742.png"
+    source_file = tmp_path / "project" / "input" / "original-3742.png"
     source_file.parent.mkdir(parents=True, exist_ok=True)
     with source_file.open("w") as f:
         f.write("image")
 
     # Try to install the image
     out_path = tmp_path / "output.png"
     create_command.install_image(
@@ -257,15 +257,15 @@
         variant="round",
         size="3742",
         target=out_path,
     )
 
     # The right message was written to output
     expected = (
-        "\nInstalling input/original-3742.png as 3742px round sample image... done\n"
+        "Installing input/original-3742.png as 3742px round sample image... done\n\n"
     )
     assert capsys.readouterr().out == expected
 
     # The file was copied into position
     create_command.shutil.copy.assert_called_with(
         create_command.base_path / "input" / "original-3742.png",
         out_path,
@@ -274,15 +274,15 @@
 
 def test_variant_with_size_without_variants(create_command, tmp_path, capsys):
     """If the app specifies a variant with a size, but no variants are
     specified, a message is output."""
     create_command.shutil = mock.MagicMock()
 
     # Create the source image
-    source_file = tmp_path / "input" / "original-3742.png"
+    source_file = tmp_path / "project" / "input" / "original-3742.png"
     source_file.parent.mkdir(parents=True, exist_ok=True)
     with source_file.open("w") as f:
         f.write("image")
 
     # Try to install the image
     out_path = tmp_path / "output.png"
     create_command.install_image(
@@ -302,15 +302,15 @@
 
 
 def test_unsized_variant(create_command, tmp_path, capsys):
     """If the app specifies an unsized variant, it is used."""
     create_command.shutil = mock.MagicMock()
 
     # Create the source image
-    source_file = tmp_path / "input" / "original.png"
+    source_file = tmp_path / "project" / "input" / "original.png"
     source_file.parent.mkdir(parents=True, exist_ok=True)
     with source_file.open("w") as f:
         f.write("image")
 
     # Try to install the image
     # Unsized variants are an annoying edge case; they get the *variant*
     # as the *size*.
@@ -322,15 +322,15 @@
         },
         variant=None,
         size="round",
         target=out_path,
     )
 
     # The right message was written to output
-    expected = "\nInstalling input/original.png as round sample image... done\n"
+    expected = "Installing input/original.png as round sample image... done\n\n"
     assert capsys.readouterr().out == expected
 
     # The file was copied into position
     create_command.shutil.copy.assert_called_with(
         create_command.base_path / "input" / "original.png",
         out_path,
     )
```

### Comparing `briefcase-0.3.8/tests/commands/create/test_properties.py` & `briefcase-0.3.9/tests/commands/create/test_properties.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/dev/conftest.py` & `briefcase-0.3.9/tests/commands/dev/conftest.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/dev/test_call.py` & `briefcase-0.3.9/tests/commands/dev/test_call.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/dev/test_get_environment.py` & `briefcase-0.3.9/tests/commands/dev/test_get_environment.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import sys
+from pathlib import Path
 
 import pytest
 
 PYTHONPATH = "PYTHONPATH"
 
 
 def test_pythonpath_with_one_source(dev_command, first_app):
     """Test get environment with one source."""
     env = dev_command.get_environment(first_app)
-    assert env[PYTHONPATH] == "src"
+    assert env[PYTHONPATH] == f"{Path.cwd() / 'src'}"
 
 
 @pytest.mark.skipif(sys.platform != "win32", reason="Relevant only for windows")
 def test_pythonpath_with_two_sources_in_windows(dev_command, third_app):
     """Test get environment with two sources in windows."""
     env = dev_command.get_environment(third_app)
-    assert env[PYTHONPATH] == "src;other"
+    assert env[PYTHONPATH] == f"{Path.cwd() / 'src'};{Path.cwd() / 'other'}"
 
 
 @pytest.mark.skipif(sys.platform == "win32", reason="Relevant only for non-windows")
 def test_pythonpath_with_two_sources_in_linux(dev_command, third_app):
     """Test get environment with two sources in linux."""
     env = dev_command.get_environment(third_app)
-    assert env[PYTHONPATH] == "src:other"
+    assert env[PYTHONPATH] == f"{Path.cwd() / 'src'}:{Path.cwd() / 'other'}"
```

### Comparing `briefcase-0.3.8/tests/commands/dev/test_install_dev_dependencies.py` & `briefcase-0.3.9/tests/commands/dev/test_install_dev_dependencies.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/new/conftest.py` & `briefcase-0.3.9/tests/commands/new/conftest.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/new/test_build_app_context.py` & `briefcase-0.3.9/tests/commands/new/test_build_app_context.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/new/test_call.py` & `briefcase-0.3.9/tests/commands/new/test_call.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/new/test_input_select.py` & `briefcase-0.3.9/tests/commands/new/test_input_select.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/new/test_input_text.py` & `briefcase-0.3.9/tests/commands/new/test_input_text.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/new/test_make_app_name.py` & `briefcase-0.3.9/tests/commands/new/test_make_app_name.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/new/test_make_author_email.py` & `briefcase-0.3.9/tests/commands/new/test_make_author_email.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/new/test_make_class_name.py` & `briefcase-0.3.9/tests/commands/new/test_make_class_name.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/new/test_make_project_url.py` & `briefcase-0.3.9/tests/commands/new/test_make_project_url.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/new/test_new_app.py` & `briefcase-0.3.9/tests/commands/new/test_new_app.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/new/test_titlecase.py` & `briefcase-0.3.9/tests/commands/new/test_titlecase.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/new/test_validate_app_name.py` & `briefcase-0.3.9/tests/commands/new/test_validate_app_name.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/new/test_validate_bundle.py` & `briefcase-0.3.9/tests/commands/new/test_validate_bundle.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/new/test_validate_email.py` & `briefcase-0.3.9/tests/commands/new/test_validate_email.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/package/conftest.py` & `briefcase-0.3.9/tests/commands/package/conftest.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/package/test_call.py` & `briefcase-0.3.9/tests/commands/package/test_call.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/publish/conftest.py` & `briefcase-0.3.9/tests/commands/publish/conftest.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/publish/test_call.py` & `briefcase-0.3.9/tests/commands/publish/test_call.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/run/conftest.py` & `briefcase-0.3.9/tests/commands/build/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,123 +1,78 @@
 import pytest
 
-from briefcase.commands import RunCommand
+from briefcase.commands import BuildCommand
 from briefcase.commands.base import full_options
 from briefcase.config import AppConfig
 
 
-class DummyRunCommand(RunCommand):
-    """A dummy run command that doesn't actually do anything.
+class DummyBuildCommand(BuildCommand):
+    """A dummy build command that doesn't actually do anything.
 
-    It only serves to track which actions would be performed.
+    It only serves to track which actions would be performend.
     """
 
     platform = "tester"
     output_format = "dummy"
-    description = "Dummy run command"
+    description = "Dummy build command"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, apps=[], **kwargs)
 
         self.actions = []
 
     def bundle_path(self, app):
-        return self.platform_path / app.app_name
+        return self.platform_path / f"{app.app_name}.dummy"
 
     def binary_path(self, app):
-        return self.platform_path / app.app_name / f"{app.app_name}.bin"
+        return self.platform_path / f"{app.app_name}.dummy.bin"
 
     def distribution_path(self, app, packaging_format):
         return self.platform_path / f"{app.app_name}.dummy.{packaging_format}"
 
     def verify_tools(self):
         super().verify_tools()
         self.actions.append(("verify",))
 
-    def run_app(self, app, **kwargs):
-        self.actions.append(("run", app.app_name, kwargs))
-        return full_options({"run_state": app.app_name}, kwargs)
+    def build_app(self, app, **kwargs):
+        self.actions.append(("build", app.app_name, kwargs))
+        return full_options({"build_state": app.app_name}, kwargs)
 
     # These commands override the default behavior, simply tracking that
-    # they were invoked, rather than instantiating a Create/Update/Build command.
+    # they were invoked, rather than instantiating a Create/Update command.
     # This is for testing purposes.
     def create_command(self, app, **kwargs):
         self.actions.append(("create", app.app_name, kwargs))
         return full_options({"create_state": app.app_name}, kwargs)
 
     def update_command(self, app, **kwargs):
         self.actions.append(("update", app.app_name, kwargs))
         return full_options({"update_state": app.app_name}, kwargs)
 
-    def build_command(self, app, **kwargs):
-        self.actions.append(("build", app.app_name, kwargs))
-        return full_options({"build_state": app.app_name}, kwargs)
-
-
-@pytest.fixture
-def run_command(tmp_path):
-    return DummyRunCommand(base_path=tmp_path)
-
-
-@pytest.fixture
-def first_app_config():
-    return AppConfig(
-        app_name="first",
-        bundle="com.example",
-        version="0.0.1",
-        description="The first simple app",
-        sources=["src/first"],
-    )
-
 
 @pytest.fixture
-def first_app_uncompiled(first_app_config, tmp_path):
-    # The same fixture as first_app_config,
-    # but ensures that the bundle for the app exists
-    (tmp_path / "tester" / "first").mkdir(parents=True, exist_ok=True)
-    with (tmp_path / "tester" / "first" / "first.dummy").open("w") as f:
-        f.write("first.dummy")
-
-    return first_app_config
-
-
-@pytest.fixture
-def first_app(first_app_uncompiled, tmp_path):
-    # The same fixture as first_app_uncompiled,
-    # but ensures that the binary for the app exists
-    with (tmp_path / "tester" / "first" / "first.bin").open("w") as f:
-        f.write("first.bin")
-
-    return first_app_uncompiled
+def build_command(tmp_path):
+    return DummyBuildCommand(base_path=tmp_path)
 
 
 @pytest.fixture
 def second_app_config():
     return AppConfig(
         app_name="second",
         bundle="com.example",
         version="0.0.2",
         description="The second simple app",
         sources=["src/second"],
     )
 
 
 @pytest.fixture
-def second_app_uncompiled(second_app_config, tmp_path):
+def second_app(second_app_config, tmp_path):
     # The same fixture as second_app_config,
-    # but ensures that the bundle for the app exists
-    (tmp_path / "tester" / "second").mkdir(parents=True, exist_ok=True)
-    with (tmp_path / "tester" / "second" / "second.dummy").open("w") as f:
-        f.write("second.dummy")
-
-    return second_app_config
-
-
-@pytest.fixture
-def second_app(second_app_uncompiled, tmp_path):
-    # The same fixture as second_app_uncompiled,
     # but ensures that the binary for the app exists
     (tmp_path / "tester").mkdir(parents=True, exist_ok=True)
-    with (tmp_path / "tester" / "second" / "second.bin").open("w") as f:
-        f.write("second.bin")
+    with (tmp_path / "tester" / "second.dummy").open("w") as f:
+        f.write("second.bundle")
+    with (tmp_path / "tester" / "second.dummy.bin").open("w") as f:
+        f.write("second.exe")
 
-    return second_app_uncompiled
+    return second_app_config
```

### Comparing `briefcase-0.3.8/tests/commands/run/test_call.py` & `briefcase-0.3.9/tests/commands/run/test_call.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/update/conftest.py` & `briefcase-0.3.9/tests/commands/update/conftest.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/update/test_call.py` & `briefcase-0.3.9/tests/commands/update/test_call.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/update/test_update_app.py` & `briefcase-0.3.9/tests/commands/update/test_update_app.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/commands/upgrade/test_call.py` & `briefcase-0.3.9/tests/commands/upgrade/test_call.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 import pytest
 
 from briefcase.exceptions import BriefcaseCommandError
 
 
 def test_list_tools(
-    upgrade_command, ManagedSDK1, ManagedSDK2, NonManagedSDK, NonInstalledSDK, capsys
+    upgrade_command,
+    ManagedSDK1,
+    ManagedSDK2,
+    ManagedSDK2Plugin1,
+    ManagedSDK2Plugin2,
+    ManagedSDK2Plugin3,
+    NonManagedSDK,
+    NonInstalledSDK,
+    capsys,
 ):
     """The tools for upgrade can be listed."""
 
     upgrade_command(tool_list=[], list_tools=True)
 
     # The tools are all verified
     ManagedSDK1.verify.assert_called_with(upgrade_command, install=False)
     ManagedSDK2.verify.assert_called_with(upgrade_command, install=False)
+    ManagedSDK2Plugin1.verify.assert_called_with(upgrade_command, install=False)
+    ManagedSDK2Plugin2.verify.assert_called_with(upgrade_command, install=False)
+    ManagedSDK2Plugin3.verify.assert_called_with(upgrade_command, install=False)
     NonManagedSDK.verify.assert_called_with(upgrade_command, install=False)
     NonInstalledSDK.verify.assert_called_with(upgrade_command, install=False)
 
     # The console contains the lines we expect, but not the non-managed and
     # non-installed tools.
     out = capsys.readouterr().out
     assert " - managed-1" in out
     assert " - managed-2" in out
+    assert " - managed-2-plugin-1" in out
+    assert " - managed-2-plugin-2" in out
+    assert " - managed-2-plugin-3" not in out
     assert " - non-managed" not in out
     assert " - non-installed" not in out
 
 
 def test_list_specific_tools(
     upgrade_command, ManagedSDK1, ManagedSDK2, NonManagedSDK, NonInstalledSDK, capsys
 ):
```

### Comparing `briefcase-0.3.8/tests/config/test_AppConfig.py` & `briefcase-0.3.9/tests/config/test_AppConfig.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/config/test_GlobalConfig.py` & `briefcase-0.3.9/tests/config/test_GlobalConfig.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/config/test_is_pep440_version.py` & `briefcase-0.3.9/tests/config/test_is_pep440_version.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/config/test_is_reserved_keyword.py` & `briefcase-0.3.9/tests/config/test_is_reserved_keyword.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/config/test_is_valid_app_name.py` & `briefcase-0.3.9/tests/config/test_is_valid_app_name.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/config/test_is_valid_bundle_identifier.py` & `briefcase-0.3.9/tests/config/test_is_valid_bundle_identifier.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/config/test_merge_config.py` & `briefcase-0.3.9/tests/config/test_merge_config.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/config/test_parse_config.py` & `briefcase-0.3.9/tests/config/test_parse_config.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/console/Console/test_boolean_input.py` & `briefcase-0.3.9/tests/console/Console/test_boolean_input.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/console/Console/test_call.py` & `briefcase-0.3.9/tests/console/Console/test_call.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/console/Console/test_properties.py` & `briefcase-0.3.9/tests/console/Console/test_properties.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/console/Console/test_selection_input.py` & `briefcase-0.3.9/tests/console/Console/test_selection_input.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/console/Console/test_text_input.py` & `briefcase-0.3.9/tests/console/Console/test_text_input.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/console/test_Log.py` & `briefcase-0.3.9/tests/console/test_Log.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/console/test_Printer.py` & `briefcase-0.3.9/tests/console/test_Printer.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/console/test_select_option.py` & `briefcase-0.3.9/tests/console/test_select_option.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/ADB/test_avd_name.py` & `briefcase-0.3.9/tests/integrations/android_sdk/ADB/test_avd_name.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/ADB/test_command.py` & `briefcase-0.3.9/tests/integrations/android_sdk/ADB/test_command.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/ADB/test_force_stop_app.py` & `briefcase-0.3.9/tests/integrations/android_sdk/ADB/test_force_stop_app.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/ADB/test_has_booted.py` & `briefcase-0.3.9/tests/integrations/android_sdk/ADB/test_has_booted.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/ADB/test_install_apk.py` & `briefcase-0.3.9/tests/integrations/android_sdk/ADB/test_install_apk.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/ADB/test_logcat.py` & `briefcase-0.3.9/tests/integrations/android_sdk/ADB/test_logcat.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,27 +10,26 @@
 
 def test_logcat(mock_sdk):
     """Invoking `logcat()` calls `run()` with the appropriate parameters."""
     # Mock out the run command on an adb instance
     adb = ADB(mock_sdk, "exampleDevice")
 
     # Invoke logcat
-    adb.logcat()
+    adb.logcat("1234")
 
     # Validate call parameters.
     mock_sdk.command.subprocess.run.assert_called_once_with(
         [
             os.fsdecode(mock_sdk.adb_path),
             "-s",
             "exampleDevice",
             "logcat",
-            "-s",
-            "MainActivity:*",
-            "stdio:*",
-            "Python:*",
+            "--pid",
+            "1234",
+            "EGL_emulation:S",
         ],
         env=mock_sdk.env,
         check=True,
         stream_output=True,
     )
 
 
@@ -39,15 +38,15 @@
     # Mock out the run command on an adb instance
     adb = ADB(mock_sdk, "exampleDevice")
     mock_sdk.command.subprocess.run = MagicMock(
         side_effect=subprocess.CalledProcessError(returncode=1, cmd="adb logcat")
     )
 
     with pytest.raises(BriefcaseCommandError):
-        adb.logcat()
+        adb.logcat("1234")
 
 
 @pytest.mark.parametrize(
     "return_code",
     (
         0xC000013A,  # Windows: STATUS_CONTROL_C_EXIT in hex
         3221225786,  # Windows: STATUS_CONTROL_C_EXIT in dec
@@ -61,8 +60,8 @@
     mock_sdk.command.subprocess.run = MagicMock(
         side_effect=subprocess.CalledProcessError(
             returncode=return_code, cmd="adb logcat"
         )
     )
 
     # does not raise BriefcaseCommandError
-    adb.logcat()
+    adb.logcat("1234")
```

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/ADB/test_start_app.py` & `briefcase-0.3.9/tests/integrations/android_sdk/ADB/test_start_app.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_avd_config.py` & `briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_avd_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 def test_avd_config(mock_sdk, tmp_path):
     """An AVD configuration can be read."""
-    config_file = tmp_path / ".android" / "avd" / "testDevice.avd" / "config.ini"
+    config_file = (
+        tmp_path / "home" / ".android" / "avd" / "testDevice.avd" / "config.ini"
+    )
     config_file.parent.mkdir(parents=True)
 
     # Write a default config. It contains:
     # * blank lines
     # * a key whose value explicitly contains an equals sign.
     with config_file.open("w") as f:
         f.write(
@@ -31,15 +33,17 @@
         "disk.cachePartition": "yes",
         "disk.cachePartition.size": "37MB",
     }
 
 
 def test_avd_config_with_space(mock_sdk, tmp_path):
     """An AVD configuration that contains spaces can be read."""
-    config_file = tmp_path / ".android" / "avd" / "testDevice.avd" / "config.ini"
+    config_file = (
+        tmp_path / "home" / ".android" / "avd" / "testDevice.avd" / "config.ini"
+    )
     config_file.parent.mkdir(parents=True)
 
     # Write a default config. It contains:
     # * blank lines
     # * a key whose value explicitly contains an equals sign.
     # * spaces either side of the key/value separator
     with config_file.open("w") as f:
```

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_create_emulator.py` & `briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_create_emulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from briefcase.integrations.android_sdk import AndroidSDK
 from tests.utils import FsPathMock
 
 
 @pytest.fixture
 def mock_sdk(tmp_path):
     command = MagicMock()
-    command.home_path = tmp_path
+    command.home_path = tmp_path / "home"
+    command.data_path = tmp_path / "data"
 
     # For default test purposes, assume we're on macOS x86_64
     command.host_os = "Darwin"
     command.host_arch = "x86_64"
 
     sdk = AndroidSDK(command, jdk=MagicMock(), root_path=tmp_path)
 
@@ -59,15 +60,17 @@
     ]
 
     # Mock system image and skin verification
     mock_sdk.verify_system_image = MagicMock()
     mock_sdk.verify_emulator_skin = MagicMock()
 
     # Mock the initial output of an AVD config file.
-    avd_config_path = tmp_path / ".android" / "avd" / "new-emulator.avd" / "config.ini"
+    avd_config_path = (
+        tmp_path / "home" / ".android" / "avd" / "new-emulator.avd" / "config.ini"
+    )
     avd_config_path.parent.mkdir(parents=True)
     with avd_config_path.open("w") as f:
         f.write("hw.device.name=pixel\n")
 
     # Create the emulator
     avd = mock_sdk.create_emulator()
 
@@ -159,15 +162,17 @@
     # This test doesn't validate most of the test process;
     # it only checks that the emulator is created with the default name.
 
     # User provides no input; default name will be used
     mock_sdk.command.input.return_value = ""
 
     # Mock the initial output of an AVD config file.
-    avd_config_path = tmp_path / ".android" / "avd" / "beePhone.avd" / "config.ini"
+    avd_config_path = (
+        tmp_path / "home" / ".android" / "avd" / "beePhone.avd" / "config.ini"
+    )
     avd_config_path.parent.mkdir(parents=True)
     with avd_config_path.open("w") as f:
         f.write("hw.device.name=pixel\n")
 
     # Consider to remove if block when we drop py3.7 support.
     # MagicMock below py3.8 doesn't has __fspath__ attribute.
     if sys.version_info < (3, 8):
@@ -194,15 +199,17 @@
             "beePhone",
         ]
     )
     # User provides no input; default name will be used
     mock_sdk.command.input.return_value = ""
 
     # Mock the initial output of an AVD config file.
-    avd_config_path = tmp_path / ".android" / "avd" / "beePhone3.avd" / "config.ini"
+    avd_config_path = (
+        tmp_path / "home" / ".android" / "avd" / "beePhone3.avd" / "config.ini"
+    )
     avd_config_path.parent.mkdir(parents=True)
     with avd_config_path.open("w") as f:
         f.write("hw.device.name=pixel\n")
 
     # Consider to remove if block when we drop py3.7 support.
     # MagicMock below py3.8 doesn't has __fspath__ attribute.
     if sys.version_info < (3, 8):
```

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_devices.py` & `briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_devices.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_emulators.py` & `briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_emulators.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_list_packages.py` & `briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_list_packages.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_properties.py` & `briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     # Mock out `host_os` so we can test Windows when not on Windows.
     mock_sdk.command.host_os = host_os
 
     assert mock_sdk.emulator_path == (mock_sdk.root_path / "emulator" / emulator_name)
 
 
 def test_avd_path(mock_sdk, tmp_path):
-    assert mock_sdk.avd_path == tmp_path / ".android" / "avd"
+    assert mock_sdk.avd_path == tmp_path / "home" / ".android" / "avd"
 
 
 def test_simple_env(mock_sdk, tmp_path):
     """The SDK Environment can be constructed."""
     assert mock_sdk.env == {
         "JAVA_HOME": os.fsdecode(Path("/path/to/jdk")),
         "ANDROID_SDK_ROOT": os.fsdecode(tmp_path / "sdk"),
```

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_select_target_device.py` & `briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_select_target_device.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_start_emulator.py` & `briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_start_emulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,16 @@
             os.fsdecode(mock_sdk.emulator_path),
             "@idleEmulator",
             "-dns-server",
             "8.8.8.8",
         ],
         env=mock_sdk.env,
         stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+        bufsize=1,
         start_new_session=True,
     )
 
     # There were 5 calls to run
     mock_sdk.mock_run.assert_has_calls(
         [
             # Three calls to get avd name
@@ -211,15 +212,16 @@
             os.fsdecode(mock_sdk.emulator_path),
             "@idleEmulator",
             "-dns-server",
             "8.8.8.8",
         ],
         env=mock_sdk.env,
         stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+        bufsize=1,
         start_new_session=True,
     )
 
     # There were 2 calls to run, both to get AVD name
     mock_sdk.mock_run.assert_has_calls(
         [
             call("emu", "avd", "name"),
@@ -310,15 +312,16 @@
             os.fsdecode(mock_sdk.emulator_path),
             "@idleEmulator",
             "-dns-server",
             "8.8.8.8",
         ],
         env=mock_sdk.env,
         stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+        bufsize=1,
         start_new_session=True,
     )
 
     # There were 6 calls to run before failure
     mock_sdk.mock_run.assert_has_calls(
         [
             # 3 calls to get avd name
```

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_update_emulator_config.py` & `briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_update_emulator_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import pytest
 
 
 @pytest.fixture
 def test_device(mock_sdk, tmp_path):
     """Create an AVD configuration file."""
-    config_file = tmp_path / ".android" / "avd" / "testDevice.avd" / "config.ini"
+    config_file = (
+        tmp_path / "home" / ".android" / "avd" / "testDevice.avd" / "config.ini"
+    )
     config_file.parent.mkdir(parents=True)
 
     # Write a default config. It contains:
     # * blank lines
     # * a key whose value explicitly contains an equals sign.
     with config_file.open("w") as f:
         f.write(
```

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_upgrade.py` & `briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_verify.py` & `briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_verify.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,19 @@
 
     command.logger = Log(verbosity=1)
 
     # Mock-out the `sys` module so we can mock out the Python version in some tests.
     command.sys = MagicMock()
     command.tools_path = tmp_path / "tools"
 
-    # Make the `os` module and `host_os` live.
-    command.os = os
+    # Mock the os environment, but copy over other key functions.
+    command.os = MagicMock()
+    command.os.environ = {}
+    command.os.fsdecode = os.fsdecode
+    command.os.access = os.access
 
     # Identify the host platform
     command.host_os = platform.system()
     command._test_download_tag = {
         "Windows": "win",
         "Darwin": "mac",
         "Linux": "linux",
```

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_verify_avd.py` & `briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_verify_avd.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_verify_emulator.py` & `briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_verify_emulator.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_verify_emulator_skin.py` & `briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_verify_emulator_skin.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_verify_license.py` & `briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_verify_license.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/AndroidSDK/test_verify_system_image.py` & `briefcase-0.3.9/tests/integrations/android_sdk/AndroidSDK/test_verify_system_image.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/android_sdk/conftest.py` & `briefcase-0.3.9/tests/integrations/android_sdk/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from briefcase.integrations.android_sdk import AndroidSDK
 from tests.utils import DummyConsole
 
 
 @pytest.fixture
 def mock_sdk(tmp_path):
     command = MagicMock()
-    command.home_path = tmp_path
+    command.home_path = tmp_path / "home"
+    command.data_path = tmp_path / "data"
     command.subprocess = MagicMock()
     command.input = DummyConsole()
     command.logger = Log(verbosity=1)
 
     # For default test purposes, assume we're on macOS x86_64
     command.host_os = "Darwin"
     command.host_arch = "x86_64"
```

### Comparing `briefcase-0.3.8/tests/integrations/docker/conftest.py` & `briefcase-0.3.9/tests/integrations/docker/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,27 +11,32 @@
 def mock_docker(tmp_path):
     command = MagicMock()
     command.logger = Log()
     command.input = Console()
     command.base_path = tmp_path / "base"
     command.platform_path = tmp_path / "platform"
     command.bundle_path.return_value = tmp_path / "bundle"
-    command.dot_briefcase_path = tmp_path / ".briefcase"
+    command.data_path = tmp_path / "briefcase"
+    command.tools_path = command.data_path / "tools"
     command.docker_image_tag.return_value = "briefcase/com.example.myapp:py3.X"
     command.python_version_tag = "3.X"
     command.os.getuid.return_value = "37"
     command.os.getgid.return_value = "42"
 
     command.subprocess = Subprocess(command)
     command.subprocess._subprocess = MagicMock()
 
     proc = MagicMock()
+    # Mock return values for run
     proc.returncode = 3
     command.subprocess._subprocess.run.return_value = proc
 
+    # Mock return values for check_output
+    command.subprocess._subprocess.check_output.return_value = "goodbye\n"
+
     # Short circuit the process streamer
     wait_bar_streamer = MagicMock()
     wait_bar_streamer.stdout.readline.return_value = ""
     wait_bar_streamer.poll.return_value = 0
     command.subprocess._subprocess.Popen.return_value.__enter__.return_value = (
         wait_bar_streamer
     )
```

### Comparing `briefcase-0.3.8/tests/integrations/docker/test_Docker__prepare.py` & `briefcase-0.3.9/tests/integrations/docker/test_Docker__prepare.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
             "HOST_UID=37",
             "--build-arg",
             "HOST_GID=42",
             os.fsdecode(tmp_path / "base" / "path" / "to" / "src"),
         ],
         stdout=-1,
         stderr=-2,
+        bufsize=1,
         text=True,
         encoding=ANY,
     )
 
 
 def test_prepare_failure(mock_docker, tmp_path):
     """If the Docker environment can't be prepared, an error is raised."""
@@ -67,10 +68,11 @@
             "HOST_UID=37",
             "--build-arg",
             "HOST_GID=42",
             os.fsdecode(tmp_path / "base" / "path" / "to" / "src"),
         ],
         stdout=-1,
         stderr=-2,
+        bufsize=1,
         text=True,
         encoding=ANY,
     )
```

### Comparing `briefcase-0.3.8/tests/integrations/docker/test_Docker__run.py` & `briefcase-0.3.9/tests/integrations/docker/test_Docker__run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import sys
+from pathlib import Path
 from unittest.mock import ANY
 
 import pytest
 
 from briefcase.console import Log
 
 
@@ -12,137 +13,136 @@
 
     mock_docker.run(["hello", "world"])
 
     mock_docker._subprocess._subprocess.run.assert_called_with(
         [
             "docker",
             "run",
-            "--tty",
             "--volume",
             f"{tmp_path / 'platform'}:/app:z",
             "--volume",
-            f"{tmp_path / '.briefcase'}:/home/brutus/.briefcase:z",
+            f"{tmp_path / 'briefcase'}:/home/brutus/.cache/briefcase:z",
+            "--rm",
             "briefcase/com.example.myapp:py3.X",
             "hello",
             "world",
         ],
         text=True,
         encoding=ANY,
     )
     assert capsys.readouterr().out == ""
 
 
-def test_simple_call_with_arg(mock_docker, tmp_path, capsys):
-    """Any extra keyword arguments are passed through as-is."""
-
-    mock_docker.run(["hello", "world"], universal_newlines=True)
+def test_call_with_arg_and_env(mock_docker, tmp_path, capsys):
+    """Extra keyword arguments are passed through as-is; env modifications are
+    converted."""
+
+    mock_docker.run(
+        ["hello", "world"],
+        env={
+            "MAGIC": "True",
+            "IMPORTANCE": "super high",
+        },
+        universal_newlines=True,
+    )
 
     mock_docker._subprocess._subprocess.run.assert_called_with(
         [
             "docker",
             "run",
-            "--tty",
             "--volume",
             f"{tmp_path / 'platform'}:/app:z",
             "--volume",
-            f"{tmp_path / '.briefcase'}:/home/brutus/.briefcase:z",
+            f"{tmp_path / 'briefcase'}:/home/brutus/.cache/briefcase:z",
+            "--rm",
+            "--env",
+            "MAGIC=True",
+            "--env",
+            "IMPORTANCE=super high",
             "briefcase/com.example.myapp:py3.X",
             "hello",
             "world",
         ],
         universal_newlines=True,
         encoding=ANY,
     )
     assert capsys.readouterr().out == ""
 
 
-def test_simple_call_with_path_arg(mock_docker, tmp_path, capsys):
-    """Path-based arguments are converted to strings and passed in as-is."""
-
-    mock_docker.run(["hello", tmp_path / "location"], cwd=tmp_path / "cwd")
+@pytest.mark.skipif(
+    sys.platform == "win32", reason="Windows paths aren't converted in Docker context"
+)
+def test_call_with_path_arg_and_env(mock_docker, tmp_path, capsys):
+    """Path-based arguments and environment are converted to strings and passed
+    in as-is."""
+
+    mock_docker.run(
+        ["hello", tmp_path / "location"],
+        env={
+            "MAGIC": "True",
+            "PATH": f"/somewhere/safe:{tmp_path / 'briefcase' / 'tools'}:{tmp_path / 'platform' / 'location'}",
+        },
+        cwd=tmp_path / "cwd",
+    )
 
     mock_docker._subprocess._subprocess.run.assert_called_with(
         [
             "docker",
             "run",
-            "--tty",
             "--volume",
             f"{tmp_path / 'platform'}:/app:z",
             "--volume",
-            f"{tmp_path / '.briefcase'}:/home/brutus/.briefcase:z",
+            f"{tmp_path / 'briefcase'}:/home/brutus/.cache/briefcase:z",
+            "--rm",
+            "--env",
+            "MAGIC=True",
+            "--env",
+            "PATH=/somewhere/safe:/home/brutus/.cache/briefcase/tools:/app/location",
             "briefcase/com.example.myapp:py3.X",
             "hello",
             os.fsdecode(tmp_path / "location"),
         ],
         cwd=os.fsdecode(tmp_path / "cwd"),
         text=True,
         encoding=ANY,
     )
     assert capsys.readouterr().out == ""
 
 
-def test_simple_call_with_sys_executable_arg(
-    mock_docker, tmp_path, capsys, monkeypatch
-):
-    """Filepath arg that are same as sys.executable are replaced with
-    unqualified python[ver]"""
-
-    test_python_path = "/path/to/python"
-    monkeypatch.setattr("sys.executable", "/path/to/python")
-
-    mock_docker.run(["hello", test_python_path])
-
-    mock_docker._subprocess._subprocess.run.assert_called_with(
-        [
-            "docker",
-            "run",
-            "--tty",
-            "--volume",
-            f"{tmp_path / 'platform'}:/app:z",
-            "--volume",
-            f"{tmp_path / '.briefcase'}:/home/brutus/.briefcase:z",
-            "briefcase/com.example.myapp:py3.X",
-            "hello",
-            "python3.X",
-        ],
-        text=True,
-        encoding=ANY,
-    )
-
-    assert capsys.readouterr().out == ""
-
-
 @pytest.mark.skipif(
     sys.platform == "win32", reason="Windows paths aren't converted in Docker context"
 )
 def test_simple_verbose_call(mock_docker, tmp_path, capsys):
     """If verbosity is turned out, there is output."""
     mock_docker.command.logger = Log(verbosity=2)
 
     mock_docker.run(["hello", "world"])
 
     mock_docker._subprocess._subprocess.run.assert_called_with(
         [
             "docker",
             "run",
-            "--tty",
             "--volume",
             f"{tmp_path / 'platform'}:/app:z",
             "--volume",
-            f"{tmp_path / '.briefcase'}:/home/brutus/.briefcase:z",
+            f"{tmp_path / 'briefcase'}:/home/brutus/.cache/briefcase:z",
+            "--rm",
             "briefcase/com.example.myapp:py3.X",
             "hello",
             "world",
         ],
         text=True,
         encoding=ANY,
     )
     assert capsys.readouterr().out == (
         "\n"
         ">>> Running Command:\n"
-        ">>>     docker run --tty "
+        ">>>     docker run "
         f"--volume {tmp_path / 'platform'}:/app:z "
-        f"--volume {tmp_path / '.briefcase'}:/home/brutus/.briefcase:z "
+        f"--volume {tmp_path / 'briefcase'}:/home/brutus/.cache/briefcase:z "
+        "--rm "
         "briefcase/com.example.myapp:py3.X "
         "hello world\n"
+        ">>> Working Directory:\n"
+        f">>>     {Path.cwd()}\n"
         ">>> Return code: 3\n"
     )
```

### Comparing `briefcase-0.3.8/tests/integrations/docker/test_verify_docker.py` & `briefcase-0.3.9/tests/integrations/docker/test_verify_docker.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/java/test_JDK__verify.py` & `briefcase-0.3.9/tests/integrations/java/test_JDK__verify.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/java/test_JDK_upgrade.py` & `briefcase-0.3.9/tests/integrations/java/test_JDK_upgrade.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/linuxdeploy/test_LinuxDeploy__patch_elf_binary.py` & `briefcase-0.3.9/tests/integrations/linuxdeploy/test_LinuxDeployBase__patch_elf_binary.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,87 +1,96 @@
 from unittest.mock import MagicMock
 
 import pytest
 
-from briefcase.exceptions import CorruptToolError, MissingToolError
+from briefcase.exceptions import CorruptToolError
 from briefcase.integrations.linuxdeploy import (
     ELF_PATCH_OFFSET,
     ELF_PATCH_ORIGINAL_BYTES,
     ELF_PATCH_PATCHED_BYTES,
-    LinuxDeploy,
+    LinuxDeployBase,
 )
 from tests.integrations.linuxdeploy.utils import create_mock_appimage
 
 
 @pytest.fixture
 def mock_command(tmp_path):
     command = MagicMock()
     command.host_arch = "wonky"
     command.tools_path = tmp_path / "tools"
     command.tools_path.mkdir()
 
     return command
 
 
-def test_patch_linuxdeploy_elf_header_unpatched(mock_command, tmp_path):
-    """If linuxdeploy is not patched, patch it."""
-    appimage_path = tmp_path / "tools" / "linuxdeploy-wonky.AppImage"
+@pytest.fixture
+def linuxdeploy(mock_command, tmp_path):
+    class LinuxDeployDummy(LinuxDeployBase):
+        name = "dummy-plugin"
+
+        @property
+        def file_name(self):
+            return "linuxdeploy-dummy-wonky.AppImage"
+
+        @property
+        def download_url(self):
+            return "https://example.com/path/to/linuxdeploy-dummy-wonky.AppImage"
+
+        @property
+        def file_path(self):
+            return tmp_path / "plugin"
+
+    return LinuxDeployDummy(mock_command)
+
+
+def test_patch_linuxdeploy_elf_header_unpatched(linuxdeploy, tmp_path):
+    """If the linuxdeploy tool/plugin is not patched, patch it."""
+    appimage_path = tmp_path / "plugin" / "linuxdeploy-dummy-wonky.AppImage"
 
     # Mock an unpatched linuxdeploy AppImage
     pre_patch_header = create_mock_appimage(
         appimage_path=appimage_path, mock_appimage_kind="original"
     )
 
     # Create a linuxdeploy wrapper, then patch the elf header
-    linuxdeploy = LinuxDeploy(mock_command)
     linuxdeploy.patch_elf_header()
 
     # Ensure the patch was applied.
     with open(appimage_path, "rb") as mock_appimage:
         mock_appimage.seek(ELF_PATCH_OFFSET)
         patched_header = mock_appimage.read(len(ELF_PATCH_PATCHED_BYTES))
 
     assert pre_patch_header == ELF_PATCH_ORIGINAL_BYTES
     assert patched_header == ELF_PATCH_PATCHED_BYTES
 
 
-def test_patch_linuxdeploy_elf_header_already_patched(mock_command, tmp_path):
+def test_patch_linuxdeploy_elf_header_already_patched(linuxdeploy, tmp_path):
     """If linuxdeploy is already patched, don't patch it."""
-    appimage_path = tmp_path / "tools" / "linuxdeploy-wonky.AppImage"
+    appimage_path = tmp_path / "plugin" / "linuxdeploy-dummy-wonky.AppImage"
 
     # Mock a patched linuxdeploy AppImage
     pre_patch_header = create_mock_appimage(
         appimage_path=appimage_path, mock_appimage_kind="patched"
     )
 
     # Create a linuxdeploy wrapper, then patch the elf header
-    linuxdeploy = LinuxDeploy(mock_command)
     linuxdeploy.patch_elf_header()
 
     # Ensure the patch was applied.
     with open(appimage_path, "rb") as mock_appimage:
         mock_appimage.seek(ELF_PATCH_OFFSET)
         patched_header = mock_appimage.read(len(ELF_PATCH_PATCHED_BYTES))
 
     assert pre_patch_header == ELF_PATCH_PATCHED_BYTES
     assert patched_header == ELF_PATCH_PATCHED_BYTES
 
 
-def test_patch_linuxdeploy_elf_header_bad_appimage(mock_command, tmp_path):
+def test_patch_linuxdeploy_elf_header_bad_appimage(linuxdeploy, tmp_path):
     """If linuxdeploy does not have a valid header, raise an error."""
-    appimage_path = tmp_path / "tools" / "linuxdeploy-wonky.AppImage"
+    appimage_path = tmp_path / "plugin" / "linuxdeploy-dummy-wonky.AppImage"
 
     # Mock an bad linuxdeploy AppImage
     create_mock_appimage(appimage_path=appimage_path, mock_appimage_kind="corrupt")
 
     # Create a linuxdeploy wrapper, then patch the elf header
-    linuxdeploy = LinuxDeploy(mock_command)
     with pytest.raises(CorruptToolError):
         linuxdeploy = linuxdeploy.patch_elf_header()
-
-
-def test_patch_linuxdeploy_elf_header_no_file(mock_command, tmp_path):
-    """If there is no linuxdeploy AppImage, raise an error."""
-    # Create a linuxdeploy wrapper, then patch the elf header
-    linuxdeploy = LinuxDeploy(mock_command)
-    with pytest.raises(MissingToolError):
-        linuxdeploy = linuxdeploy.patch_elf_header()
```

### Comparing `briefcase-0.3.8/tests/integrations/linuxdeploy/test_LinuxDeploy__upgrade.py` & `briefcase-0.3.9/tests/integrations/linuxdeploy/test_LinuxDeployBase__upgrade.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,101 @@
 from unittest.mock import MagicMock
 
 import pytest
 from requests import exceptions as requests_exceptions
 
 from briefcase.exceptions import MissingToolError, NetworkFailure
-from briefcase.integrations.linuxdeploy import LinuxDeploy
-from tests.integrations.linuxdeploy.utils import create_mock_appimage
+from briefcase.integrations.linuxdeploy import LinuxDeployBase
+from tests.integrations.linuxdeploy.utils import side_effect_create_mock_appimage
 
 
 @pytest.fixture
 def mock_command(tmp_path):
     command = MagicMock()
     command.host_arch = "wonky"
     command.tools_path = tmp_path / "tools"
     command.tools_path.mkdir()
 
     return command
 
 
-def test_upgrade_exists(mock_command, tmp_path):
+@pytest.fixture
+def linuxdeploy(mock_command, tmp_path):
+    class LinuxDeployDummy(LinuxDeployBase):
+        name = "dummy-plugin"
+        full_name = "Dummy plugin"
+
+        @property
+        def file_name(self):
+            return "linuxdeploy-dummy-wonky.AppImage"
+
+        @property
+        def download_url(self):
+            return "https://example.com/path/to/linuxdeploy-dummy-wonky.AppImage"
+
+        @property
+        def file_path(self):
+            return tmp_path / "plugin"
+
+    return LinuxDeployDummy(mock_command)
+
+
+def test_upgrade_exists(linuxdeploy, mock_command, tmp_path):
     """If linuxdeploy already exists, upgrading deletes first."""
-    appimage_path = tmp_path / "tools" / "linuxdeploy-wonky.AppImage"
+    appimage_path = tmp_path / "plugin" / "linuxdeploy-dummy-wonky.AppImage"
 
     # Mock the existence of an install
+    appimage_path.parent.mkdir(parents=True)
     appimage_path.touch()
 
     # Mock a successful download
-    def side_effect_create_mock_appimage(*args, **kwargs):
-        create_mock_appimage(appimage_path=appimage_path)
-        return "new-downloaded-file"
-
-    mock_command.download_url.side_effect = side_effect_create_mock_appimage
+    mock_command.download_url.side_effect = side_effect_create_mock_appimage(
+        appimage_path
+    )
 
     # Create a linuxdeploy wrapper, then upgrade it
-    linuxdeploy = LinuxDeploy(mock_command)
     linuxdeploy.upgrade()
 
     # The mock file should exist as the upgraded version
     assert appimage_path.exists()
 
     # A download is invoked
     mock_command.download_url.assert_called_with(
-        url="https://github.com/linuxdeploy/linuxdeploy/"
-        "releases/download/continuous/linuxdeploy-wonky.AppImage",
-        download_path=tmp_path / "tools",
+        url="https://example.com/path/to/linuxdeploy-dummy-wonky.AppImage",
+        download_path=tmp_path / "plugin",
     )
     # The downloaded file will be made executable
     mock_command.os.chmod.assert_called_with("new-downloaded-file", 0o755)
 
 
-def test_upgrade_does_not_exist(mock_command, tmp_path):
+def test_upgrade_does_not_exist(linuxdeploy, mock_command):
     """If linuxdeploy doesn't already exist, upgrading is an error."""
     # Create a linuxdeploy wrapper, then upgrade it
-    linuxdeploy = LinuxDeploy(mock_command)
     with pytest.raises(MissingToolError):
         linuxdeploy.upgrade()
 
     # The tool wasn't already installed, so an error is raised.
     assert mock_command.download_url.call_count == 0
 
 
-def test_upgrade_linuxdeploy_download_failure(mock_command, tmp_path):
+def test_upgrade_linuxdeploy_download_failure(linuxdeploy, mock_command, tmp_path):
     """If linuxdeploy doesn't exist, but a download failure occurs, an error is
     raised."""
     # Mock the existence of an install
-    appimage_path = tmp_path / "tools" / "linuxdeploy-wonky.AppImage"
+    appimage_path = tmp_path / "plugin" / "linuxdeploy-dummy-wonky.AppImage"
+    appimage_path.parent.mkdir(parents=True)
     appimage_path.touch()
 
     mock_command.download_url.side_effect = requests_exceptions.ConnectionError
 
-    # Create a linuxdeploy wrapper, then upgrade it.
-    # The upgrade will fail
-    linuxdeploy = LinuxDeploy(mock_command)
+    # Updated the linuxdeploy wrapper; the upgrade will fail
     with pytest.raises(NetworkFailure):
         linuxdeploy.upgrade()
 
     # The mock file will be deleted
     assert not appimage_path.exists()
 
     # A download was invoked
     mock_command.download_url.assert_called_with(
-        url="https://github.com/linuxdeploy/linuxdeploy/"
-        "releases/download/continuous/linuxdeploy-wonky.AppImage",
-        download_path=tmp_path / "tools",
+        url="https://example.com/path/to/linuxdeploy-dummy-wonky.AppImage",
+        download_path=tmp_path / "plugin",
     )
```

### Comparing `briefcase-0.3.8/tests/integrations/linuxdeploy/test_LinuxDeploy__verify.py` & `briefcase-0.3.9/tests/integrations/rcedit/test_RCEdit__verify.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,91 @@
 from unittest.mock import MagicMock
 
 import pytest
 from requests import exceptions as requests_exceptions
 
 from briefcase.exceptions import MissingToolError, NetworkFailure
-from briefcase.integrations.linuxdeploy import LinuxDeploy
-from tests.integrations.linuxdeploy.utils import create_mock_appimage
+from briefcase.integrations.rcedit import RCEdit
 
 
 @pytest.fixture
 def mock_command(tmp_path):
     command = MagicMock()
     command.host_arch = "wonky"
     command.tools_path = tmp_path / "tools"
     command.tools_path.mkdir()
 
     return command
 
 
 def test_verify_exists(mock_command, tmp_path):
-    """If linuxdeploy already exists, verification doesn't download."""
-    appimage_path = tmp_path / "tools" / "linuxdeploy-wonky.AppImage"
+    """If RCEdit already exists, verification doesn't download."""
+    rcedit_path = tmp_path / "tools" / "rcedit-x64.exe"
 
     # Mock the existence of an install
-    appimage_path.touch()
+    rcedit_path.touch()
 
-    # Create a linuxdeploy wrapper by verification
-    linuxdeploy = LinuxDeploy.verify(mock_command)
+    # Create a rcedit wrapper by verification
+    rcedit = RCEdit.verify(mock_command)
 
     # No download occured
     assert mock_command.download_url.call_count == 0
     assert mock_command.os.chmod.call_count == 0
 
     # The build command retains the path to the downloaded file.
-    assert linuxdeploy.appimage_path == appimage_path
+    assert rcedit.rcedit_path == rcedit_path
 
 
 def test_verify_does_not_exist_dont_install(mock_command, tmp_path):
-    """If linuxdeploy doesn't exist, and install=False, it is *not*
-    downloaded."""
+    """If RCEdit doesn't exist, and install=False, it is *not* downloaded."""
     # Mock a successful download
     mock_command.download_url.return_value = "new-downloaded-file"
 
-    # True to create a linuxdeploy wrapper by verification.
+    # True to create a rcedit wrapper by verification.
     # This will fail because it doesn't exist, but installation was disabled.
     with pytest.raises(MissingToolError):
-        LinuxDeploy.verify(mock_command, install=False)
+        RCEdit.verify(mock_command, install=False)
 
     # No download occured
     assert mock_command.download_url.call_count == 0
     assert mock_command.os.chmod.call_count == 0
 
 
 def test_verify_does_not_exist(mock_command, tmp_path):
-    """If linuxdeploy doesn't exist, it is downloaded."""
-    appimage_path = tmp_path / "tools" / "linuxdeploy-wonky.AppImage"
+    """If RCEdit doesn't exist, it is downloaded."""
+    rcedit_path = tmp_path / "tools" / "rcedit-x64.exe"
 
     # Mock a successful download
     def side_effect_create_mock_appimage(*args, **kwargs):
-        create_mock_appimage(appimage_path=appimage_path)
+        rcedit_path.touch()
         return "new-downloaded-file"
 
     mock_command.download_url.side_effect = side_effect_create_mock_appimage
 
-    # Create a linuxdeploy wrapper by verification
-    linuxdeploy = LinuxDeploy.verify(mock_command)
+    # Create a rcedit wrapper by verification
+    rcedit = RCEdit.verify(mock_command)
 
     # A download is invoked
     mock_command.download_url.assert_called_with(
-        url="https://github.com/linuxdeploy/linuxdeploy/"
-        "releases/download/continuous/linuxdeploy-wonky.AppImage",
+        url="https://github.com/electron/rcedit/"
+        "releases/download/v1.1.1/rcedit-x64.exe",
         download_path=tmp_path / "tools",
     )
-    # The downloaded file will be made executable
-    mock_command.os.chmod.assert_called_with("new-downloaded-file", 0o755)
 
     # The build command retains the path to the downloaded file.
-    assert linuxdeploy.appimage_path == appimage_path
+    assert rcedit.rcedit_path == rcedit_path
 
 
-def test_verify_linuxdeploy_download_failure(mock_command, tmp_path):
-    """If linuxdeploy doesn't exist, but a download failure occurs, an error is
+def test_verify_rcedit_download_failure(mock_command, tmp_path):
+    """If RCEdit doesn't exist, but a download failure occurs, an error is
     raised."""
     mock_command.download_url.side_effect = requests_exceptions.ConnectionError
 
     with pytest.raises(NetworkFailure):
-        LinuxDeploy.verify(mock_command)
+        RCEdit.verify(mock_command)
 
     # A download was invoked
     mock_command.download_url.assert_called_with(
-        url="https://github.com/linuxdeploy/linuxdeploy/"
-        "releases/download/continuous/linuxdeploy-wonky.AppImage",
+        url="https://github.com/electron/rcedit/"
+        "releases/download/v1.1.1/rcedit-x64.exe",
         download_path=tmp_path / "tools",
     )
```

### Comparing `briefcase-0.3.8/tests/integrations/subprocess/conftest.py` & `briefcase-0.3.9/tests/integrations/subprocess/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 from unittest.mock import MagicMock
 
 import pytest
 
 from briefcase.console import Console, Log
 from briefcase.integrations.subprocess import Subprocess
 
@@ -37,22 +38,24 @@
 
     return sub
 
 
 @pytest.fixture
 def popen_process():
     process = MagicMock()
-    # There are extra empty strings at the end to simulate readline
-    # continuously returning "" once it reaches EOF
-    process.stdout.readline.side_effect = [
-        "output line 1\n",
-        "\n",
-        "output line 3\n",
-        "",
-        "",
-        "",
-        "",
-        "",
-        "",
-    ]
-    process.poll.side_effect = [None, None, None, -3, -3, -3]
+
+    # Mock the readline values of an actual process. The final return value is "",
+    # indicating that the process has exited; however, we insert a short sleep
+    # to ensure that any other threads will have a chance to run before this
+    # thread acutally terminates.
+    def mock_readline():
+        yield from [
+            "output line 1\n",
+            "\n",
+            "output line 3\n",
+        ]
+        time.sleep(0.1)
+        yield ""
+
+    process.stdout.readline.side_effect = mock_readline()
+    process.poll.return_value = -3
     return process
```

### Comparing `briefcase-0.3.8/tests/integrations/subprocess/test_Subprocess__Popen.py` & `briefcase-0.3.9/tests/integrations/subprocess/test_Subprocess__Popen.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from pathlib import Path
 from unittest.mock import ANY
 
 import pytest
 
 from briefcase.console import Log
 
 from .conftest import CREATE_NEW_PROCESS_GROUP, CREATE_NO_WINDOW
@@ -129,39 +130,46 @@
 
     mock_sub._subprocess.Popen.assert_called_with(
         ["hello", "world"],
         text=True,
         encoding=ANY,
     )
     assert capsys.readouterr().out == (
-        "\n" ">>> Running Command:\n" ">>>     hello world\n"
+        "\n"
+        ">>> Running Command:\n"
+        ">>>     hello world\n"
+        ">>> Working Directory:\n"
+        f">>>     {Path.cwd()}\n"
     )
 
 
-def test_debug_call_with_env(mock_sub, capsys):
+def test_debug_call_with_env(mock_sub, capsys, tmp_path):
     """If verbosity is turned up, and injected env vars are included output."""
     mock_sub.command.logger = Log(verbosity=2)
 
     env = {"NewVar": "NewVarValue"}
-    mock_sub.Popen(["hello", "world"], env=env)
+    mock_sub.Popen(["hello", "world"], env=env, cwd=tmp_path / "cwd")
 
     merged_env = mock_sub.command.os.environ.copy()
     merged_env.update(env)
 
     mock_sub._subprocess.Popen.assert_called_with(
         ["hello", "world"],
         env=merged_env,
+        cwd=os.fsdecode(tmp_path / "cwd"),
         text=True,
         encoding=ANY,
     )
 
     expected_output = (
         "\n"
         ">>> Running Command:\n"
         ">>>     hello world\n"
+        ">>> Working Directory:\n"
+        f">>>     {tmp_path / 'cwd'}\n"
         ">>> Environment Overrides:\n"
         ">>>     NewVar=NewVarValue\n"
     )
 
     assert capsys.readouterr().out == expected_output
```

### Comparing `briefcase-0.3.8/tests/integrations/subprocess/test_Subprocess__check_output.py` & `briefcase-0.3.9/tests/integrations/subprocess/test_Subprocess__check_output.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from pathlib import Path
 from subprocess import CalledProcessError
 from unittest.mock import ANY
 
 import pytest
 
 from briefcase.console import Log
 
@@ -134,58 +135,63 @@
         encoding=ANY,
     )
 
     expected_output = (
         "\n"
         ">>> Running Command:\n"
         ">>>     hello world\n"
+        ">>> Working Directory:\n"
+        f">>>     {Path.cwd()}\n"
         ">>> Command Output:\n"
         ">>>     some output line 1\n"
         ">>>     more output line 2\n"
         ">>> Return code: 0\n"
     )
 
     assert capsys.readouterr().out == expected_output
 
 
-def test_debug_call_with_env(mock_sub, capsys):
+def test_debug_call_with_env(mock_sub, capsys, tmp_path):
     """If verbosity is turned up, injected env vars are included in output."""
     mock_sub.command.logger = Log(verbosity=2)
 
     env = {"NewVar": "NewVarValue"}
-    mock_sub.check_output(["hello", "world"], env=env)
+    mock_sub.check_output(["hello", "world"], env=env, cwd=tmp_path / "cwd")
 
     merged_env = mock_sub.command.os.environ.copy()
     merged_env.update(env)
 
     mock_sub._subprocess.check_output.assert_called_with(
         ["hello", "world"],
         env=merged_env,
+        cwd=os.fsdecode(tmp_path / "cwd"),
         text=True,
         encoding=ANY,
     )
 
     expected_output = (
         "\n"
         ">>> Running Command:\n"
         ">>>     hello world\n"
+        ">>> Working Directory:\n"
+        f">>>     {tmp_path / 'cwd'}\n"
         ">>> Environment Overrides:\n"
         ">>>     NewVar=NewVarValue\n"
         ">>> Command Output:\n"
         ">>>     some output line 1\n"
         ">>>     more output line 2\n"
         ">>> Return code: 0\n"
     )
 
     assert capsys.readouterr().out == expected_output
 
 
 def test_calledprocesserror_exception_logging(mock_sub, capsys):
     """If command errors, ensure command output is printed."""
-    mock_sub.command.logger = Log(verbosity=3)
+    mock_sub.command.logger = Log(verbosity=2)
 
     called_process_error = CalledProcessError(
         returncode=-1,
         cmd="hello world",
         output="output line 1\noutput line 2",
         stderr="error line 1\nerror line 2",
     )
@@ -194,14 +200,16 @@
     with pytest.raises(CalledProcessError):
         mock_sub.check_output(["hello", "world"])
 
     expected_output = (
         "\n"
         ">>> Running Command:\n"
         ">>>     hello world\n"
+        ">>> Working Directory:\n"
+        f">>>     {Path.cwd()}\n"
         ">>> Command Output:\n"
         ">>>     output line 1\n"
         ">>>     output line 2\n"
         ">>> Command Error Output (stderr):\n"
         ">>>     error line 1\n"
         ">>>     error line 2\n"
         ">>> Return code: -1\n"
```

### Comparing `briefcase-0.3.8/tests/integrations/subprocess/test_Subprocess__cleanup.py` & `briefcase-0.3.9/tests/integrations/subprocess/test_Subprocess__cleanup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,8 +24,8 @@
     mock_sub.cleanup("testing process", process)
 
     process.terminate.assert_called_once()
     process.wait.assert_called_once_with(timeout=3)
     process.kill.assert_called_once_with()
 
     # Log contains a contextual message.
-    assert capsys.readouterr().out == ("Forcibly killing testing process...\n")
+    assert capsys.readouterr().out == "Forcibly killing testing process...\n"
```

### Comparing `briefcase-0.3.8/tests/integrations/subprocess/test_Subprocess__final_kwargs.py` & `briefcase-0.3.9/tests/integrations/subprocess/test_Subprocess__final_kwargs.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/subprocess/test_Subprocess__parse_output.py` & `briefcase-0.3.9/tests/integrations/subprocess/test_Subprocess__parse_output.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/subprocess/test_Subprocess__run.py` & `briefcase-0.3.9/tests/integrations/subprocess/test_Subprocess__run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from pathlib import Path
 from subprocess import CalledProcessError
 from unittest.mock import ANY
 
 import pytest
 
 from briefcase.console import Log
 
@@ -134,50 +135,55 @@
         encoding=ANY,
     )
     # fmt: off
     expected_output = (
         "\n"
         ">>> Running Command:\n"
         ">>>     hello world\n"
+        ">>> Working Directory:\n"
+        f">>>     {Path.cwd()}\n"
         ">>> Return code: 0\n"
     )
     # fmt: on
 
     assert capsys.readouterr().out == expected_output
 
 
-def test_debug_call_with_env(mock_sub, capsys):
+def test_debug_call_with_env(mock_sub, capsys, tmp_path):
     """If verbosity is turned up, injected env vars are included output."""
     mock_sub.command.logger = Log(verbosity=2)
 
     env = {"NewVar": "NewVarValue"}
-    mock_sub.run(["hello", "world"], env=env)
+    mock_sub.run(["hello", "world"], env=env, cwd=tmp_path / "cwd")
 
     merged_env = mock_sub.command.os.environ.copy()
     merged_env.update(env)
 
     mock_sub._subprocess.run.assert_called_with(
         ["hello", "world"],
         env=merged_env,
+        cwd=os.fsdecode(tmp_path / "cwd"),
         text=True,
         encoding=ANY,
     )
     expected_output = (
         "\n"
         ">>> Running Command:\n"
         ">>>     hello world\n"
+        ">>> Working Directory:\n"
+        f">>>     {tmp_path / 'cwd'}\n"
         ">>> Environment Overrides:\n"
         ">>>     NewVar=NewVarValue\n"
         ">>> Return code: 0\n"
     )
     assert capsys.readouterr().out == expected_output
 
 
 def test_calledprocesserror_exception_logging(mock_sub, capsys):
-    mock_sub.command.logger = Log(verbosity=3)
+    mock_sub.command.logger = Log(verbosity=2)
 
     called_process_error = CalledProcessError(
         returncode=-1,
         cmd="hello world",
         output="output line 1\noutput line 2",
         stderr="error line 1\nerror line 2",
     )
@@ -187,14 +193,16 @@
         mock_sub.run(["hello", "world"])
 
     # fmt: off
     expected_output = (
         "\n"
         ">>> Running Command:\n"
         ">>>     hello world\n"
+        ">>> Working Directory:\n"
+        f">>>     {Path.cwd()}\n"
         ">>> Return code: -1\n"
     )
     # fmt: on
 
     assert capsys.readouterr().out == expected_output
```

### Comparing `briefcase-0.3.8/tests/integrations/subprocess/test_Subprocess__run_in_wait_bar.py` & `briefcase-0.3.9/tests/integrations/subprocess/test_Subprocess__run_in_wait_bar.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import os
 import subprocess
+from pathlib import Path
 from unittest.mock import ANY
 
 import pytest
 
 from briefcase.console import Log
 
 
@@ -19,14 +21,15 @@
     with mock_sub.command.input.wait_bar():
         mock_sub.run(["hello", "world"])
 
     mock_sub._subprocess.Popen.assert_called_with(
         ["hello", "world"],
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
+        bufsize=1,
         text=True,
         encoding=ANY,
     )
     expected_output = "output line 1\n" "\n" "output line 3\n" "\n"
     assert capsys.readouterr().out == expected_output
 
 
@@ -36,14 +39,15 @@
     with mock_sub.command.input.wait_bar():
         mock_sub.run(["hello", "world"], universal_newlines=True)
 
     mock_sub._subprocess.Popen.assert_called_with(
         ["hello", "world"],
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
+        bufsize=1,
         universal_newlines=True,
         encoding=ANY,
     )
     expected_output = "output line 1\n" "\n" "output line 3\n" "\n"
     assert capsys.readouterr().out == expected_output
 
 
@@ -54,73 +58,84 @@
     with mock_sub.command.input.wait_bar():
         mock_sub.run(["hello", "world"])
 
     mock_sub._subprocess.Popen.assert_called_with(
         ["hello", "world"],
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
+        bufsize=1,
         text=True,
         encoding=ANY,
     )
     expected_output = (
         "\n"
         ">>> Running Command:\n"
         ">>>     hello world\n"
+        ">>> Working Directory:\n"
+        f">>>     {Path.cwd()}\n"
         "output line 1\n"
         "\n"
         "output line 3\n"
         ">>> Return code: -3\n"
         "\n"
     )
     assert capsys.readouterr().out == expected_output
 
 
-def test_debug_call_with_env(mock_sub, capsys):
+def test_debug_call_with_env(mock_sub, capsys, tmp_path):
     """If verbosity is turned up, injected env vars are included in debug
     output."""
     mock_sub.command.logger = Log(verbosity=2)
 
     env = {"NewVar": "NewVarValue"}
     with mock_sub.command.input.wait_bar():
-        mock_sub.run(["hello", "world"], env=env)
+        mock_sub.run(["hello", "world"], env=env, cwd=tmp_path / "cwd")
 
     merged_env = mock_sub.command.os.environ.copy()
     merged_env.update(env)
 
     mock_sub._subprocess.Popen.assert_called_with(
         ["hello", "world"],
         env=merged_env,
+        cwd=os.fsdecode(tmp_path / "cwd"),
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
+        bufsize=1,
         text=True,
         encoding=ANY,
     )
     expected_output = (
         "\n"
         ">>> Running Command:\n"
         ">>>     hello world\n"
+        ">>> Working Directory:\n"
+        f">>>     {tmp_path / 'cwd'}\n"
         ">>> Environment Overrides:\n"
         ">>>     NewVar=NewVarValue\n"
         "output line 1\n"
         "\n"
         "output line 3\n"
         ">>> Return code: -3\n"
         "\n"
     )
     assert capsys.readouterr().out == expected_output
 
 
 @pytest.mark.parametrize(
     "in_kwargs, kwargs",
     [
-        ({}, {"text": True, "encoding": ANY}),
-        ({"text": True}, {"text": True, "encoding": ANY}),
-        ({"text": False}, {"text": False}),
-        ({"universal_newlines": False}, {"universal_newlines": False}),
-        ({"universal_newlines": True}, {"universal_newlines": True, "encoding": ANY}),
+        ({}, {"text": True, "encoding": ANY, "bufsize": 1}),
+        ({"text": True}, {"text": True, "encoding": ANY, "bufsize": 1}),
+        ({"text": False}, {"text": False, "bufsize": 1}),
+        ({"text": False, "bufsize": 42}, {"text": False, "bufsize": 42}),
+        ({"universal_newlines": False}, {"universal_newlines": False, "bufsize": 1}),
+        (
+            {"universal_newlines": True},
+            {"universal_newlines": True, "encoding": ANY, "bufsize": 1},
+        ),
     ],
 )
 def test_text_eq_true_default_overriding(mock_sub, in_kwargs, kwargs):
     """if text or universal_newlines is explicitly provided, those should
     override text=true default."""
     with mock_sub.command.input.wait_bar():
         mock_sub.run(["hello", "world"], **in_kwargs)
@@ -140,14 +155,15 @@
     with mock_sub.command.input.wait_bar():
         run_result = mock_sub.run(["hello", "world"], stderr=subprocess.PIPE)
 
     mock_sub._subprocess.Popen.assert_called_with(
         ["hello", "world"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
+        bufsize=1,
         text=True,
         encoding=ANY,
     )
 
     expected_output = "output line 1\n" "\n" "output line 3\n" "\n"
     assert capsys.readouterr().out == expected_output
     assert run_result.stderr == stderr_output
@@ -160,14 +176,15 @@
     with mock_sub.command.input.wait_bar():
         run_result = mock_sub.run(["hello", "world"], stderr=subprocess.DEVNULL)
 
     mock_sub._subprocess.Popen.assert_called_with(
         ["hello", "world"],
         stdout=subprocess.PIPE,
         stderr=subprocess.DEVNULL,
+        bufsize=1,
         text=True,
         encoding=ANY,
     )
 
     expected_output = "output line 1\n" "\n" "output line 3\n" "\n"
     assert capsys.readouterr().out == expected_output
     assert run_result.stderr is None
```

### Comparing `briefcase-0.3.8/tests/integrations/subprocess/test_get_process_id_by_command.py` & `briefcase-0.3.9/tests/integrations/subprocess/test_get_process_id_by_command.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/subprocess/test_json_parser.py` & `briefcase-0.3.9/tests/integrations/subprocess/test_json_parser.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/wix/test_WiX__upgrade.py` & `briefcase-0.3.9/tests/integrations/wix/test_WiX__upgrade.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/wix/test_WiX__verify.py` & `briefcase-0.3.9/tests/integrations/wix/test_WiX__verify.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/xcode/simctl/alternate-format.json` & `briefcase-0.3.9/tests/integrations/xcode/simctl/alternate-format.json`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/xcode/simctl/iOS-13.2-only.json` & `briefcase-0.3.9/tests/integrations/xcode/simctl/iOS-13.2-only.json`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/xcode/simctl/multiple-iOS-versions.json` & `briefcase-0.3.9/tests/integrations/xcode/simctl/multiple-iOS-versions.json`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/xcode/test_confirm_xcode_license_accepted.py` & `briefcase-0.3.9/tests/integrations/xcode/test_confirm_xcode_license_accepted.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/xcode/test_ensure_command_line_tools_are_installed.py` & `briefcase-0.3.9/tests/integrations/xcode/test_ensure_command_line_tools_are_installed.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/xcode/test_ensure_xcode_is_installed.py` & `briefcase-0.3.9/tests/integrations/xcode/test_ensure_xcode_is_installed.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/xcode/test_get_device_state.py` & `briefcase-0.3.9/tests/integrations/xcode/test_get_device_state.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/xcode/test_get_identities.py` & `briefcase-0.3.9/tests/integrations/xcode/test_get_identities.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/integrations/xcode/test_get_simulators.py` & `briefcase-0.3.9/tests/integrations/xcode/test_get_simulators.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/platforms/android/gradle/test_build.py` & `briefcase-0.3.9/tests/platforms/android/gradle/test_build.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from briefcase.exceptions import BriefcaseCommandError
 from briefcase.platforms.android.gradle import GradleBuildCommand
 
 
 @pytest.fixture
 def build_command(tmp_path, first_app_config):
     command = GradleBuildCommand(base_path=tmp_path / "base_path")
-    command.dot_briefcase_path = tmp_path / ".briefcase"
+    command.data_path = tmp_path / "briefcase"
     command.android_sdk = MagicMock()
     command.os = MagicMock()
     command.os.environ = {}
     command.sys = MagicMock()
     command.requests = MagicMock()
     command.subprocess = MagicMock()
     return command
```

### Comparing `briefcase-0.3.8/tests/platforms/android/gradle/test_create.py` & `briefcase-0.3.9/tests/platforms/android/gradle/test_create.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/platforms/android/gradle/test_package.py` & `briefcase-0.3.9/tests/platforms/android/gradle/test_package.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from briefcase.exceptions import BriefcaseCommandError
 from briefcase.platforms.android.gradle import GradlePackageCommand
 
 
 @pytest.fixture
 def package_command(tmp_path, first_app_config):
     command = GradlePackageCommand(base_path=tmp_path / "base_path")
-    command.dot_briefcase_path = tmp_path / ".briefcase"
+    command.data_path = tmp_path / "briefcase"
     command.android_sdk = MagicMock()
     command.os = MagicMock()
     command.os.environ = {}
     command.sys = MagicMock()
     command.requests = MagicMock()
     command.subprocess = MagicMock()
     return command
```

### Comparing `briefcase-0.3.8/tests/platforms/android/gradle/test_run.py` & `briefcase-0.3.9/tests/platforms/android/gradle/test_run.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from unittest.mock import MagicMock
+import time
+from unittest.mock import MagicMock, call
 
 import pytest
 
 from briefcase.integrations.android_sdk import AndroidSDK
 from briefcase.platforms.android.gradle import GradleRunCommand
 
 
 @pytest.fixture
 def run_command(tmp_path, first_app_config):
     command = GradleRunCommand(base_path=tmp_path / "base_path")
-    command.dot_briefcase_path = tmp_path / ".briefcase"
+    command.data_path = tmp_path / "briefcase"
     command.java_home_path = tmp_path / "java"
 
     command.mock_adb = MagicMock()
+    command.mock_adb.pidof = MagicMock(return_value="777")
     command.android_sdk = AndroidSDK(command, jdk=MagicMock(), root_path=tmp_path)
     command.android_sdk.adb = MagicMock(return_value=command.mock_adb)
 
     command.os = MagicMock()
     command.os.environ = {}
     command.requests = MagicMock()
     command.subprocess = MagicMock()
@@ -49,22 +51,37 @@
     run_command.mock_adb.install_apk.assert_called_once_with(
         run_command.binary_path(first_app_config)
     )
     run_command.mock_adb.force_stop_app.assert_called_once_with(
         f"{first_app_config.package_name}.{first_app_config.module_name}",
     )
 
-    run_command.mock_adb.clear_log.assert_called_once()
-
     run_command.mock_adb.start_app.assert_called_once_with(
         f"{first_app_config.package_name}.{first_app_config.module_name}",
         "org.beeware.android.MainActivity",
     )
 
-    run_command.mock_adb.logcat.assert_called_once()
+    run_command.mock_adb.pidof.assert_called_once_with(
+        f"{first_app_config.package_name}.{first_app_config.module_name}"
+    )
+    run_command.mock_adb.logcat.assert_called_once_with("777")
+
+
+def test_run_slow_start(run_command, first_app_config, monkeypatch):
+    run_command.android_sdk.select_target_device = MagicMock(
+        return_value=("exampleDevice", "ExampleDevice", None)
+    )
+    run_command.mock_adb.pidof.side_effect = [None, None, "888"]
+    monkeypatch.setattr(time, "sleep", MagicMock())
+
+    run_command.run_app(first_app_config, device_or_avd="exampleDevice")
+
+    assert run_command.mock_adb.pidof.mock_calls == [call("com.example.first_app")] * 3
+    assert time.sleep.mock_calls == [call(0.5)] * 2
+    run_command.mock_adb.logcat.assert_called_once_with("888")
 
 
 def test_run_created_emulator(run_command, first_app_config):
     """The user can choose to run on a newly created emulator."""
     # Set up device selection to return a completely new emulator
     run_command.android_sdk.select_target_device = MagicMock(
         return_value=(None, None, None)
@@ -95,22 +112,20 @@
     run_command.mock_adb.install_apk.assert_called_once_with(
         run_command.binary_path(first_app_config)
     )
     run_command.mock_adb.force_stop_app.assert_called_once_with(
         f"{first_app_config.package_name}.{first_app_config.module_name}",
     )
 
-    run_command.mock_adb.clear_log.assert_called_once()
-
     run_command.mock_adb.start_app.assert_called_once_with(
         f"{first_app_config.package_name}.{first_app_config.module_name}",
         "org.beeware.android.MainActivity",
     )
 
-    run_command.mock_adb.logcat.assert_called_once()
+    run_command.mock_adb.logcat.assert_called_once_with("777")
 
 
 def test_run_idle_device(run_command, first_app_config):
     """The user can choose to run on an idle device."""
     # Set up device selection to return a new device that has an AVD,
     # but not a device ID.
     run_command.android_sdk.select_target_device = MagicMock(
@@ -142,15 +157,13 @@
     run_command.mock_adb.install_apk.assert_called_once_with(
         run_command.binary_path(first_app_config)
     )
     run_command.mock_adb.force_stop_app.assert_called_once_with(
         f"{first_app_config.package_name}.{first_app_config.module_name}",
     )
 
-    run_command.mock_adb.clear_log.assert_called_once()
-
     run_command.mock_adb.start_app.assert_called_once_with(
         f"{first_app_config.package_name}.{first_app_config.module_name}",
         "org.beeware.android.MainActivity",
     )
 
-    run_command.mock_adb.logcat.assert_called_once()
+    run_command.mock_adb.logcat.assert_called_once_with("777")
```

### Comparing `briefcase-0.3.8/tests/platforms/android/gradle/test_safe_formal_name.py` & `briefcase-0.3.9/tests/platforms/android/gradle/test_safe_formal_name.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/platforms/android/gradle/test_verify_tools.py` & `briefcase-0.3.9/tests/platforms/android/gradle/test_verify_tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,17 +12,17 @@
         base_path=tmp_path / "base_path",
         apps={"first": first_app_config},
     )
 
     # Mock-out the `sys` module so we can mock out the Python version in some tests.
     command.sys = mock.MagicMock()
 
-    # Use the `tmp_path` in `dot_briefcase_path` to ensure tests don't interfere
+    # Use the `tmp_path` in `data_path` to ensure tests don't interfere
     # with each other.
-    command.dot_briefcase_path = tmp_path / ".briefcase"
+    command.data_path = tmp_path / "briefcase"
 
     # Use a dummy JAVA HOME
     command.java_home_path = tmp_path / "java"
 
     # Override the `os` module so the app has an environment with JAVA_HOME
     command.os = mock.MagicMock(
         environ={"JAVA_HOME": os.fsdecode(command.java_home_path)}
```

### Comparing `briefcase-0.3.8/tests/platforms/conftest.py` & `briefcase-0.3.9/tests/platforms/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 
 @pytest.fixture
 def first_app_config():
     return AppConfig(
         app_name="first-app",
         project_name="First Project",
         formal_name="First App",
+        author="Megacorp",
         bundle="com.example",
         version="0.0.1",
         description="The first simple app",
         sources=["src/first_app"],
     )
 
 
 @pytest.fixture
 def uppercase_app_config():
     return AppConfig(
         app_name="First-App",
         project_name="First Project",
         formal_name="First App",
+        author="Megacorp",
         bundle="com.example",
         version="0.0.1",
         description="The first simple app",
         sources=["src/First_App"],
     )
```

### Comparing `briefcase-0.3.8/tests/platforms/iOS/xcode/mixin/test_select_target_device.py` & `briefcase-0.3.9/tests/platforms/iOS/xcode/mixin/test_select_target_device.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/platforms/iOS/xcode/test_build.py` & `briefcase-0.3.9/tests/platforms/iOS/xcode/test_build.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/platforms/iOS/xcode/test_mixin.py` & `briefcase-0.3.9/tests/platforms/iOS/xcode/test_mixin.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/platforms/iOS/xcode/test_run.py` & `briefcase-0.3.9/tests/platforms/iOS/xcode/test_run.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/platforms/linux/appimage/test_create.py` & `briefcase-0.3.9/tests/platforms/linux/appimage/test_create.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,16 +51,14 @@
         [
             sys.executable,
             "-m",
             "pip",
             "install",
             "--upgrade",
             "--no-user",
-            "--progress-bar",
-            "off",
             f"--target={tmp_path}/linux/appimage/First App/path/to/app_packages",
             "foo==1.2.3",
             "bar>=4.5",
         ],
         check=True,
     )
 
@@ -97,15 +95,13 @@
         [
             sys.executable,
             "-m",
             "pip",
             "install",
             "--upgrade",
             "--no-user",
-            "--progress-bar",
-            "off",
             f"--target={tmp_path}/linux/appimage/First App/path/to/app_packages",
             "foo==1.2.3",
             "bar>=4.5",
         ],
         check=True,
     )
```

### Comparing `briefcase-0.3.8/tests/platforms/linux/appimage/test_mixin.py` & `briefcase-0.3.9/tests/platforms/linux/appimage/test_mixin.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/platforms/macOS/app/conftest.py` & `briefcase-0.3.9/tests/platforms/macOS/app/conftest.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/platforms/macOS/app/test_build.py` & `briefcase-0.3.9/tests/platforms/macOS/app/test_build.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/platforms/macOS/app/test_create.py` & `briefcase-0.3.9/tests/platforms/macOS/app/test_create.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/platforms/macOS/app/test_mixin.py` & `briefcase-0.3.9/tests/platforms/macOS/app/test_mixin.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/platforms/macOS/app/test_package.py` & `briefcase-0.3.9/tests/platforms/macOS/app/test_package.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/platforms/macOS/app/test_package__notarize.py` & `briefcase-0.3.9/tests/platforms/macOS/app/test_package__notarize.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/platforms/macOS/app/test_package__team_id_from_identity.py` & `briefcase-0.3.9/tests/platforms/macOS/app/test_package__team_id_from_identity.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/platforms/macOS/app/test_run.py` & `briefcase-0.3.9/tests/platforms/macOS/app/test_run.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 
 from briefcase.exceptions import BriefcaseCommandError
 from briefcase.platforms.macOS.app import macOSAppRunCommand
 
 
 def test_run_app(first_app_config, tmp_path, monkeypatch):
     """A macOS app can be started."""
-    command = macOSAppRunCommand(base_path=tmp_path)
+    command = macOSAppRunCommand(
+        base_path=tmp_path / "base",
+        home_path=tmp_path / "home",
+    )
     command.subprocess = mock.MagicMock()
     log_stream_process = mock.MagicMock()
     command.subprocess.Popen.return_value = log_stream_process
 
     monkeypatch.setattr(
         "briefcase.platforms.macOS.get_process_id_by_command", lambda *a, **kw: 100
     )
@@ -38,25 +41,30 @@
             ' AND senderImagePath=="/usr/lib/libffi.dylib")',
         ],
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
         bufsize=1,
     )
     command.subprocess.run.assert_called_with(
-        ["open", "-n", os.fsdecode(bin_path)], check=True
+        ["open", "-n", os.fsdecode(bin_path)],
+        cwd=tmp_path / "home",
+        check=True,
     )
     command.subprocess.stream_output.assert_called_with(
         "log stream", log_stream_process, stop_func=mock.ANY
     )
     command.subprocess.cleanup.assert_called_with("log stream", log_stream_process)
 
 
 def test_run_app_failed(first_app_config, tmp_path):
     """If there's a problem started the app, an exception is raised."""
-    command = macOSAppRunCommand(base_path=tmp_path)
+    command = macOSAppRunCommand(
+        base_path=tmp_path / "base",
+        home_path=tmp_path / "home",
+    )
     command.subprocess = mock.MagicMock()
     log_stream_process = mock.MagicMock()
     command.subprocess.Popen.return_value = log_stream_process
     command.subprocess.run.side_effect = subprocess.CalledProcessError(
         cmd=["open", "-n", os.fsdecode(command.binary_path(first_app_config))],
         returncode=1,
     )
@@ -79,25 +87,30 @@
             ' AND senderImagePath=="/usr/lib/libffi.dylib")',
         ],
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
         bufsize=1,
     )
     command.subprocess.run.assert_called_with(
-        ["open", "-n", os.fsdecode(bin_path)], check=True
+        ["open", "-n", os.fsdecode(bin_path)],
+        cwd=tmp_path / "home",
+        check=True,
     )
 
     # No attempt was made to stream the log; but there was a cleanup
     command.subprocess.stream_output.assert_not_called()
     command.subprocess.cleanup.assert_called_with("log stream", log_stream_process)
 
 
 def test_run_app_find_pid_failed(first_app_config, tmp_path, monkeypatch, capsys):
     """If after app is started, its pid is not found, do not stream output."""
-    command = macOSAppRunCommand(base_path=tmp_path)
+    command = macOSAppRunCommand(
+        base_path=tmp_path / "base",
+        home_path=tmp_path / "home",
+    )
     command.subprocess = mock.MagicMock()
     log_stream_process = mock.MagicMock()
     command.subprocess.Popen.return_value = log_stream_process
 
     monkeypatch.setattr(
         "briefcase.platforms.macOS.get_process_id_by_command", lambda *a, **kw: None
     )
@@ -118,15 +131,17 @@
             ' AND senderImagePath=="/usr/lib/libffi.dylib")',
         ],
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
         bufsize=1,
     )
     command.subprocess.run.assert_called_with(
-        ["open", "-n", os.fsdecode(bin_path)], check=True
+        ["open", "-n", os.fsdecode(bin_path)],
+        cwd=tmp_path / "home",
+        check=True,
     )
     assert capsys.readouterr().out == (
         "\n"
         "[first-app] Starting app...\n"
         "\n"
         "Unable to find process for app first-app to start log streaming.\n"
     )
```

### Comparing `briefcase-0.3.8/tests/platforms/macOS/app/test_signing.py` & `briefcase-0.3.9/tests/platforms/macOS/app/test_signing.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/platforms/macOS/xcode/test_build.py` & `briefcase-0.3.9/tests/platforms/macOS/xcode/test_build.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/platforms/macOS/xcode/test_mixin.py` & `briefcase-0.3.9/tests/platforms/macOS/xcode/test_mixin.py`

 * *Files identical despite different names*

### Comparing `briefcase-0.3.8/tests/platforms/macOS/xcode/test_run.py` & `briefcase-0.3.9/tests/platforms/macOS/xcode/test_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 from unittest import mock
 
 from briefcase.platforms.macOS.xcode import macOSXcodeRunCommand
 
 
 def test_run_app(first_app_config, tmp_path):
     """A macOS Xcode app can be started."""
-    command = macOSXcodeRunCommand(base_path=tmp_path)
+    command = macOSXcodeRunCommand(
+        base_path=tmp_path / "base",
+        home_path=tmp_path / "home",
+    )
     command.subprocess = mock.MagicMock()
-
     command.run_app(first_app_config)
 
     # Calls were made to start the app and to start a log stream.
     bin_path = command.binary_path(first_app_config)
     sender = bin_path / "Contents" / "MacOS" / "First App"
     command.subprocess.Popen.assert_called_with(
         [
@@ -30,9 +32,11 @@
             ' AND senderImagePath=="/usr/lib/libffi.dylib")',
         ],
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
         bufsize=1,
     )
     command.subprocess.run.assert_called_with(
-        ["open", "-n", os.fsdecode(bin_path)], check=True
+        ["open", "-n", os.fsdecode(bin_path)],
+        cwd=tmp_path / "home",
+        check=True,
     )
```

### Comparing `briefcase-0.3.8/tests/platforms/windows/msi/test_create.py` & `briefcase-0.3.9/tests/platforms/windows/app/test_create.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 import pytest
 
-from briefcase.platforms.windows.msi import WindowsMSICreateCommand
+from briefcase.platforms.windows.app import WindowsAppCreateCommand
 
 
 @pytest.mark.parametrize(
     "version, version_triple",
     [
         ("1", "1.0.0"),
         ("1.2", "1.2.0"),
@@ -16,56 +16,56 @@
         ("1.2.3b5", "1.2.3"),
         ("1.2.3rc6", "1.2.3"),
         ("1.2.3.dev7", "1.2.3"),
         ("1.2.3.post8", "1.2.3"),
     ],
 )
 def test_version_triple(first_app_config, tmp_path, version, version_triple):
-    command = WindowsMSICreateCommand(base_path=tmp_path)
+    command = WindowsAppCreateCommand(base_path=tmp_path)
 
     first_app_config.version = version
     context = command.output_format_template_context(first_app_config)
 
     assert context["version_triple"] == version_triple
 
 
 def test_explicit_version_triple(first_app_config, tmp_path):
-    command = WindowsMSICreateCommand(base_path=tmp_path)
+    command = WindowsAppCreateCommand(base_path=tmp_path)
 
     first_app_config.version = "1.2.3a1"
     first_app_config.version_triple = "2.3.4"
 
     context = command.output_format_template_context(first_app_config)
 
     # Explicit version triple is used.
     assert context["version_triple"] == "2.3.4"
 
 
 def test_guid(first_app_config, tmp_path):
     """A preictable GUID will be generated from the bundle."""
-    command = WindowsMSICreateCommand(base_path=tmp_path)
+    command = WindowsAppCreateCommand(base_path=tmp_path)
 
     context = command.output_format_template_context(first_app_config)
 
     assert context["guid"] == "d666a4f1-c7b7-52cc-888a-3a35a7cc97e5"
 
 
 def test_explicit_guid(first_app_config, tmp_path):
     """If a GUID is explicitly provided, it is used."""
-    command = WindowsMSICreateCommand(base_path=tmp_path)
+    command = WindowsAppCreateCommand(base_path=tmp_path)
 
     first_app_config.guid = "e822176f-b755-589f-849c-6c6600f7efb1"
     context = command.output_format_template_context(first_app_config)
 
     # Explicitly provided GUID is used.
     assert context["guid"] == "e822176f-b755-589f-849c-6c6600f7efb1"
 
 
 def test_support_package_url(first_app_config, tmp_path):
-    command = WindowsMSICreateCommand(base_path=tmp_path)
+    command = WindowsAppCreateCommand(base_path=tmp_path)
 
     # Set some properties of the host system for test purposes.
     command.host_arch = "wonky"
     command.platform = "tester"
 
     # This test result is dependent on whether we're using a 32-bit (win32)
     # or 64-bit (amd64) machine.
@@ -75,32 +75,44 @@
         ("version", f"3.{sys.version_info.minor}"),
         ("arch", arch),
     ]
 
 
 def test_default_install_scope(first_app_config, tmp_path):
     """By default, app should be installed per user."""
-    command = WindowsMSICreateCommand(base_path=tmp_path)
+    command = WindowsAppCreateCommand(base_path=tmp_path)
 
     context = command.output_format_template_context(first_app_config)
 
-    assert context["install_scope"] == "perUser"
+    assert context == {
+        "guid": "d666a4f1-c7b7-52cc-888a-3a35a7cc97e5",
+        "version_triple": "0.0.1",
+        "install_scope": None,
+    }
 
 
 def test_per_machine_install_scope(first_app_config, tmp_path):
     """By default, app should be installed per user."""
-    command = WindowsMSICreateCommand(base_path=tmp_path)
+    command = WindowsAppCreateCommand(base_path=tmp_path)
     first_app_config.system_installer = True
 
     context = command.output_format_template_context(first_app_config)
 
-    assert context["install_scope"] == "perMachine"
+    assert context == {
+        "guid": "d666a4f1-c7b7-52cc-888a-3a35a7cc97e5",
+        "version_triple": "0.0.1",
+        "install_scope": "perMachine",
+    }
 
 
 def test_per_user_install_scope(first_app_config, tmp_path):
-    """App can be set to have explocit per-user scope."""
-    command = WindowsMSICreateCommand(base_path=tmp_path)
+    """App can be set to have explicit per-user scope."""
+    command = WindowsAppCreateCommand(base_path=tmp_path)
     first_app_config.system_installer = False
 
     context = command.output_format_template_context(first_app_config)
 
-    assert context["install_scope"] == "perUser"
+    assert context == {
+        "guid": "d666a4f1-c7b7-52cc-888a-3a35a7cc97e5",
+        "version_triple": "0.0.1",
+        "install_scope": "perUser",
+    }
```

### Comparing `briefcase-0.3.8/tests/platforms/windows/msi/test_mixin.py` & `briefcase-0.3.9/tests/platforms/windows/visualstudio/test_mixin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,24 @@
-from briefcase.platforms.windows.msi import WindowsMSICreateCommand
+from briefcase.platforms.windows.visualstudio import WindowsVisualStudioCreateCommand
 
 
 def test_binary_path(first_app_config, tmp_path):
-    command = WindowsMSICreateCommand(base_path=tmp_path)
+    command = WindowsVisualStudioCreateCommand(base_path=tmp_path)
     binary_path = command.binary_path(first_app_config)
 
-    assert binary_path == tmp_path / "windows" / "msi" / "First App"
+    assert (
+        binary_path
+        == tmp_path
+        / "windows"
+        / "VisualStudio"
+        / "First App"
+        / "x64"
+        / "Release"
+        / "First App.exe"
+    )
 
 
 def test_distribution_path(first_app_config, tmp_path):
-    command = WindowsMSICreateCommand(base_path=tmp_path)
-    distribution_path = command.distribution_path(first_app_config, "msi")
+    command = WindowsVisualStudioCreateCommand(base_path=tmp_path)
+    distribution_path = command.distribution_path(first_app_config, "app")
 
     assert distribution_path == tmp_path / "windows" / "First App-0.0.1.msi"
```

### Comparing `briefcase-0.3.8/tests/platforms/windows/msi/test_package.py` & `briefcase-0.3.9/tests/platforms/windows/app/test_package.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from unittest import mock
 
 import pytest
 
 from briefcase.integrations.wix import WiX
-from briefcase.platforms.windows.msi import WindowsMSIPackageCommand
+from briefcase.platforms.windows.app import WindowsAppPackageCommand
 
 
 @pytest.fixture
 def package_command(tmp_path):
-    command = WindowsMSIPackageCommand(base_path=tmp_path)
+    command = WindowsAppPackageCommand(base_path=tmp_path)
     command.subprocess = mock.MagicMock()
     command.wix = WiX(command=command, wix_home=tmp_path / "wix")
     return command
 
 
 def test_package_msi(package_command, first_app_config, tmp_path):
     """A Wwindows app can be packaged as an MSI."""
@@ -39,31 +39,33 @@
                     "first_app_COMPONENTS",
                     "-var",
                     "var.SourceDir",
                     "-out",
                     "first-app-manifest.wxs",
                 ],
                 check=True,
-                cwd=tmp_path / "windows" / "msi" / "First App",
+                cwd=tmp_path / "windows" / "app" / "First App",
             ),
             # Compile MSI
             mock.call(
                 [
                     tmp_path / "wix" / "bin" / "candle.exe",
                     "-nologo",
                     "-ext",
                     "WixUtilExtension",
                     "-ext",
                     "WixUIExtension",
+                    "-arch",
+                    "x64",
                     "-dSourceDir=src",
                     "first-app.wxs",
                     "first-app-manifest.wxs",
                 ],
                 check=True,
-                cwd=tmp_path / "windows" / "msi" / "First App",
+                cwd=tmp_path / "windows" / "app" / "First App",
             ),
             # Link MSI
             mock.call(
                 [
                     tmp_path / "wix" / "bin" / "light.exe",
                     "-nologo",
                     "-ext",
@@ -74,11 +76,11 @@
                     "unicode.wxl",
                     "-o",
                     tmp_path / "windows" / "First App-0.0.1.msi",
                     "first-app.wixobj",
                     "first-app-manifest.wixobj",
                 ],
                 check=True,
-                cwd=tmp_path / "windows" / "msi" / "First App",
+                cwd=tmp_path / "windows" / "app" / "First App",
             ),
         ]
     )
```

### Comparing `briefcase-0.3.8/tests/platforms/windows/msi/test_run.py` & `briefcase-0.3.9/tests/platforms/windows/app/test_run.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 import os
 from unittest import mock
 
 import pytest
 
 from briefcase.exceptions import BriefcaseCommandError
-from briefcase.platforms.windows.msi import WindowsMSIRunCommand
+from briefcase.platforms.windows.app import WindowsAppRunCommand
 
 
 def test_run_app(first_app_config, tmp_path):
-    """A windows MSI can be started."""
-    command = WindowsMSIRunCommand(base_path=tmp_path)
+    """A windows app can be started."""
+    command = WindowsAppRunCommand(
+        base_path=tmp_path / "base",
+        home_path=tmp_path / "home",
+    )
     command.subprocess = mock.MagicMock()
 
     command.run_app(first_app_config)
 
     command.subprocess.run.assert_called_with(
         [
             os.fsdecode(
                 tmp_path
+                / "base"
                 / "windows"
-                / "msi"
+                / "app"
                 / "First App"
                 / "src"
-                / "python"
-                / "pythonw.exe"
+                / "First App.exe"
             ),
-            "-m",
-            "first_app",
         ],
+        cwd=tmp_path / "home",
         check=True,
     )
 
 
 def test_run_app_failed(first_app_config, tmp_path):
     """If there's a problem started the app, an exception is raised."""
-    command = WindowsMSIRunCommand(base_path=tmp_path)
+    command = WindowsAppRunCommand(
+        base_path=tmp_path / "base",
+        home_path=tmp_path / "home",
+    )
     command.subprocess = mock.MagicMock()
     command.subprocess.run.side_effect = BriefcaseCommandError("problem")
 
     with pytest.raises(BriefcaseCommandError):
         command.run_app(first_app_config)
 
     # The run command was still invoked, though
     command.subprocess.run.assert_called_with(
         [
             os.fsdecode(
                 tmp_path
+                / "base"
                 / "windows"
-                / "msi"
+                / "app"
                 / "First App"
                 / "src"
-                / "python"
-                / "pythonw.exe"
+                / "First App.exe"
             ),
-            "-m",
-            "first_app",
         ],
+        cwd=tmp_path / "home",
         check=True,
     )
```

### Comparing `briefcase-0.3.8/tests/test_cmdline.py` & `briefcase-0.3.9/tests/test_cmdline.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     InvalidFormatError,
     NoCommandError,
     ShowOutputFormats,
     UnsupportedCommandError,
 )
 from briefcase.platforms.linux.appimage import LinuxAppImageCreateCommand
 from briefcase.platforms.macOS.app import macOSAppCreateCommand, macOSAppPublishCommand
-from briefcase.platforms.windows.msi import WindowsMSICreateCommand
+from briefcase.platforms.windows.app import WindowsAppCreateCommand
 
 
 def test_empty():
     """``briefcase`` returns basic usage."""
     with pytest.raises(NoCommandError) as excinfo:
         parse_cmdline("".split())
 
@@ -170,22 +170,22 @@
     assert cmd.input.enabled
     assert cmd.logger.verbosity == 1
     assert options == {}
 
 
 @pytest.mark.skipif(sys.platform != "win32", reason="requires Windows")
 def test_windows_default():
-    """``briefcase create`` returns the Windows create msi command on
+    """``briefcase create`` returns the Windows create app command on
     Windows."""
 
     cmd, options = parse_cmdline("create".split())
 
-    assert isinstance(cmd, WindowsMSICreateCommand)
+    assert isinstance(cmd, WindowsAppCreateCommand)
     assert cmd.platform == "windows"
-    assert cmd.output_format == "msi"
+    assert cmd.output_format == "app"
     assert cmd.input.enabled
     assert cmd.logger.verbosity == 1
     assert options == {}
 
 
 def test_bare_command_help(monkeypatch, capsys):
     """``briefcase create -h`` returns the macOS create app command help."""
```

### Comparing `briefcase-0.3.8/tox.ini` & `briefcase-0.3.9/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -62,10 +62,10 @@
 deps =
 allowlist_externals =
     sh
     rm
 commands =
     rm -rf {envname}
     sh -c 'cat {envname}.config | briefcase new'
-    sh -c 'cd {envname} && briefcase create'
-    sh -c 'cd {envname} && briefcase build'
-    sh -c 'cd {envname} && briefcase package --adhoc-sign'
+    sh -c 'cd {envname} && briefcase create {posargs}'
+    sh -c 'cd {envname} && briefcase build {posargs}'
+    sh -c 'cd {envname} && briefcase package --adhoc-sign {posargs}'
```

