# Comparing `tmp/CoverGPT-1.2.0.tar.gz` & `tmp/CoverGPT-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoverGPT-1.2.0.tar", last modified: Sat Mar 11 20:15:23 2023, max compression
+gzip compressed data, was "CoverGPT-1.3.0.tar", last modified: Wed Apr 12 20:30:59 2023, max compression
```

## Comparing `CoverGPT-1.2.0.tar` & `CoverGPT-1.3.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-03-11 20:15:23.345682 CoverGPT-1.2.0/
-drwxrwxrwx   0        0        0        0 2023-03-11 20:15:23.227330 CoverGPT-1.2.0/CoverGPT/
-drwxrwxrwx   0        0        0        0 2023-03-11 20:15:23.246534 CoverGPT-1.2.0/CoverGPT/OpenFonts/
--rw-rw-rw-   0        0        0     7970 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/OpenFonts/deedy_resume-openfont.xtx
-drwxrwxrwx   0        0        0        0 2023-03-11 20:15:23.194821 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/
-drwxrwxrwx   0        0        0        0 2023-03-11 20:15:23.296295 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/
--rw-rw-rw-   0        0        0   114588 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/Lato-Bla.ttf
--rw-rw-rw-   0        0        0   111616 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/Lato-BlaIta.ttf
--rw-rw-rw-   0        0        0   121788 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/Lato-Bol.ttf
--rw-rw-rw-   0        0        0   120312 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/Lato-BolIta.ttf
--rw-rw-rw-   0        0        0   115316 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/Lato-Hai.ttf
--rw-rw-rw-   0        0        0    91460 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/Lato-HaiIta.ttf
--rw-rw-rw-   0        0        0   122524 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/Lato-Lig.ttf
--rw-rw-rw-   0        0        0    91600 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/Lato-LigIta.ttf
--rw-rw-rw-   0        0        0   120196 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/Lato-Reg.ttf
--rw-rw-rw-   0        0        0   118352 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/Lato-RegIta.ttf
-drwxrwxrwx   0        0        0        0 2023-03-11 20:15:23.345682 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/raleway/
--rw-rw-rw-   0        0        0    66088 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Bold.otf
--rw-rw-rw-   0        0        0    66336 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-ExtraBold.otf
--rw-rw-rw-   0        0        0    63364 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-ExtraLight.otf
--rw-rw-rw-   0        0        0    70484 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Heavy.otf
--rw-rw-rw-   0        0        0    64488 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Light.otf
--rw-rw-rw-   0        0        0    64776 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Medium.otf
--rw-rw-rw-   0        0        0    64368 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Regular.otf
--rw-rw-rw-   0        0        0    65696 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-SemiBold.otf
--rw-rw-rw-   0        0        0    64256 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Thin.otf
--rw-rw-rw-   0        0        0        0 2023-02-19 07:21:21.000000 CoverGPT-1.2.0/CoverGPT/__init_.py
--rw-rw-rw-   0        0        0      138 2023-02-04 20:20:55.000000 CoverGPT-1.2.0/CoverGPT/__main__.py
--rw-rw-rw-   0        0        0     4197 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/CoverGPT/cover.cls
--rw-rw-rw-   0        0        0     3185 2023-02-17 02:48:54.000000 CoverGPT-1.2.0/CoverGPT/gptex.py
--rw-rw-rw-   0        0        0    13419 2023-02-16 01:27:58.000000 CoverGPT-1.2.0/CoverGPT/gui.py
--rw-rw-rw-   0        0        0      778 2023-02-04 22:42:37.000000 CoverGPT-1.2.0/CoverGPT/template.tex
-drwxrwxrwx   0        0        0        0 2023-03-11 20:15:23.241021 CoverGPT-1.2.0/CoverGPT.egg-info/
--rw-rw-rw-   0        0        0      759 2023-03-11 20:15:22.000000 CoverGPT-1.2.0/CoverGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1273 2023-03-11 20:15:22.000000 CoverGPT-1.2.0/CoverGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-11 20:15:22.000000 CoverGPT-1.2.0/CoverGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-03-11 20:15:22.000000 CoverGPT-1.2.0/CoverGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-11 20:15:22.000000 CoverGPT-1.2.0/CoverGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-02-04 19:38:59.000000 CoverGPT-1.2.0/LICENSE
--rw-rw-rw-   0        0        0      759 2023-03-11 20:15:23.345682 CoverGPT-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1860 2023-02-04 19:31:36.000000 CoverGPT-1.2.0/README.md
--rw-rw-rw-   0        0        0       86 2023-03-11 20:15:23.347193 CoverGPT-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1153 2023-03-11 20:14:29.000000 CoverGPT-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:30:59.764684 CoverGPT-1.3.0/
+drwxrwxrwx   0        0        0        0 2023-04-12 20:30:59.652495 CoverGPT-1.3.0/CoverGPT/
+drwxrwxrwx   0        0        0        0 2023-04-12 20:30:59.674527 CoverGPT-1.3.0/CoverGPT/OpenFonts/
+-rw-rw-rw-   0        0        0     7970 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/OpenFonts/deedy_resume-openfont.xtx
+drwxrwxrwx   0        0        0        0 2023-04-12 20:30:59.630468 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/
+drwxrwxrwx   0        0        0        0 2023-04-12 20:30:59.722815 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/
+-rw-rw-rw-   0        0        0   114588 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/Lato-Bla.ttf
+-rw-rw-rw-   0        0        0   111616 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/Lato-BlaIta.ttf
+-rw-rw-rw-   0        0        0   121788 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/Lato-Bol.ttf
+-rw-rw-rw-   0        0        0   120312 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/Lato-BolIta.ttf
+-rw-rw-rw-   0        0        0   115316 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/Lato-Hai.ttf
+-rw-rw-rw-   0        0        0    91460 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/Lato-HaiIta.ttf
+-rw-rw-rw-   0        0        0   122524 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/Lato-Lig.ttf
+-rw-rw-rw-   0        0        0    91600 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/Lato-LigIta.ttf
+-rw-rw-rw-   0        0        0   120196 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/Lato-Reg.ttf
+-rw-rw-rw-   0        0        0   118352 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/Lato-RegIta.ttf
+drwxrwxrwx   0        0        0        0 2023-04-12 20:30:59.763680 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/raleway/
+-rw-rw-rw-   0        0        0    66088 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Bold.otf
+-rw-rw-rw-   0        0        0    66336 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-ExtraBold.otf
+-rw-rw-rw-   0        0        0    63364 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-ExtraLight.otf
+-rw-rw-rw-   0        0        0    70484 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Heavy.otf
+-rw-rw-rw-   0        0        0    64488 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Light.otf
+-rw-rw-rw-   0        0        0    64776 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Medium.otf
+-rw-rw-rw-   0        0        0    64368 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Regular.otf
+-rw-rw-rw-   0        0        0    65696 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-SemiBold.otf
+-rw-rw-rw-   0        0        0    64256 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Thin.otf
+-rw-rw-rw-   0        0        0        0 2023-02-19 07:21:21.000000 CoverGPT-1.3.0/CoverGPT/__init_.py
+-rw-rw-rw-   0        0        0      138 2023-02-04 20:20:55.000000 CoverGPT-1.3.0/CoverGPT/__main__.py
+-rw-rw-rw-   0        0        0     4197 2023-02-04 19:31:36.000000 CoverGPT-1.3.0/CoverGPT/cover.cls
+-rw-rw-rw-   0        0        0     3194 2023-04-12 20:13:15.000000 CoverGPT-1.3.0/CoverGPT/gptex.py
+-rw-rw-rw-   0        0        0    13440 2023-04-12 20:15:25.000000 CoverGPT-1.3.0/CoverGPT/gui.py
+-rw-rw-rw-   0        0        0      778 2023-02-04 22:42:37.000000 CoverGPT-1.3.0/CoverGPT/template.tex
+drwxrwxrwx   0        0        0        0 2023-04-12 20:30:59.669528 CoverGPT-1.3.0/CoverGPT.egg-info/
+-rw-rw-rw-   0        0        0      759 2023-04-12 20:30:59.000000 CoverGPT-1.3.0/CoverGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1273 2023-04-12 20:30:59.000000 CoverGPT-1.3.0/CoverGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 20:30:59.000000 CoverGPT-1.3.0/CoverGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-04-12 20:30:59.000000 CoverGPT-1.3.0/CoverGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 20:30:59.000000 CoverGPT-1.3.0/CoverGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-02-04 19:38:59.000000 CoverGPT-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0      759 2023-04-12 20:30:59.764684 CoverGPT-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2253 2023-04-12 20:27:02.000000 CoverGPT-1.3.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-12 20:30:59.766195 CoverGPT-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1153 2023-04-12 20:30:04.000000 CoverGPT-1.3.0/setup.py
```

### Comparing `CoverGPT-1.2.0/CoverGPT/OpenFonts/deedy_resume-openfont.xtx` & `CoverGPT-1.3.0/CoverGPT/OpenFonts/deedy_resume-openfont.xtx`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/Lato-Bla.ttf` & `CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/Lato-Bla.ttf`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/Lato-BlaIta.ttf` & `CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/Lato-BlaIta.ttf`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/Lato-Bol.ttf` & `CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/Lato-Bol.ttf`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/Lato-BolIta.ttf` & `CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/Lato-BolIta.ttf`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/Lato-Hai.ttf` & `CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/Lato-Hai.ttf`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/Lato-HaiIta.ttf` & `CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/Lato-HaiIta.ttf`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/Lato-Lig.ttf` & `CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/Lato-Lig.ttf`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/Lato-LigIta.ttf` & `CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/Lato-LigIta.ttf`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/Lato-Reg.ttf` & `CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/Lato-Reg.ttf`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/lato/Lato-RegIta.ttf` & `CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/lato/Lato-RegIta.ttf`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Bold.otf` & `CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Bold.otf`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-ExtraBold.otf` & `CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-ExtraBold.otf`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-ExtraLight.otf` & `CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-ExtraLight.otf`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Heavy.otf` & `CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Heavy.otf`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Light.otf` & `CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Light.otf`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Medium.otf` & `CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Medium.otf`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Regular.otf` & `CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Regular.otf`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-SemiBold.otf` & `CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-SemiBold.otf`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Thin.otf` & `CoverGPT-1.3.0/CoverGPT/OpenFonts/fonts/raleway/Raleway-Thin.otf`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/cover.cls` & `CoverGPT-1.3.0/CoverGPT/cover.cls`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT/gptex.py` & `CoverGPT-1.3.0/CoverGPT/gptex.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def generateCoverLetter(job_listing, company_name, address1, address2):
     script_dir = os.path.dirname(os.path.realpath(__file__))
 
     # read user credentials from file
     api_key_file = os.path.join(script_dir, "login")
     with open(api_key_file, "r") as f:
         user_email = f.readline().strip()
-        user_password = f.readline().strip()
+        #user_password = f.readline().strip()
 
     # read settings from file
     settings_file = os.path.join(script_dir, "settings")
     with open(settings_file, "r") as f:
         first_name = f.readline().strip()
         last_name = f.readline().strip()
         website_url = f.readline().strip()
@@ -34,16 +34,16 @@
         message = "Write a cover letter without a letter closing for this job position: " + company_name + " " + job_listing + "\n This is my resume: \n" + resume
         message = "".join(c for c in message if c <= "\uFFFF")
     else:
         message = "Write a cover letter without a letter closing for this job position: " + company_name + " " + job_listing
 
     print(message)
     chatbot = Chatbot(config={
-        "email": user_email,
-        "password": user_password
+        "access_token": user_email,
+        #"password": user_password
     })
     for data in chatbot.ask(
     message
     ):
         content = data["message"]
 
     print(content)
```

### Comparing `CoverGPT-1.2.0/CoverGPT/gui.py` & `CoverGPT-1.3.0/CoverGPT/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         self.main_button_1 = customtkinter.CTkButton(master=self, text="Upload Resume", fg_color="transparent", border_width=2, text_color=("gray10", "#DCE4EE"), command=self.upload_resume)
         self.main_button_1.grid(row=2, column=3, padx=(20, 20), pady=(20, 20), sticky="nsew")
 
         # set default values
         self.appearance_mode_optionemenu.set("Dark")
         self.scaling_optionemenu.set("120%")
         self.progressbar_1.configure(mode="indeterminnate")
-        self.textbox.insert("0.0", "CoverGPT, a cover letter generator powered by GPT-3.\n\n")
+        self.textbox.insert("0.0", "CoverGPT, a cover letter generator powered by ChatGPT.\n\n")
         self.textbox.insert("end", "Please login and set your user info before generating (see github page).\n\n\n")
 
 
     def send_job_listing(self):
         if self.company_entry.get() and self.entry.get() == "":
             self.textbox.insert("end", "Please enter a job listing and company name.\n")
             return
@@ -151,25 +151,26 @@
         resume.close()
         rawResume.close()
 
 
     def sign_in_event(self):
         self.window = customtkinter.CTkToplevel(self)
         self.window.title("Sign In")
-        self.window.geometry("320x200")
+        self.window.geometry("340x145")
 
-        self.userEmail_label = customtkinter.CTkLabel(self.window, text="Email:", anchor="w")
+        self.userEmail_label = customtkinter.CTkLabel(self.window, text="Access Token:", anchor="w")
         self.userEmail_label.grid(row=0, column=0, padx=(20, 0), pady=(20, 0), sticky="nsew")
         self.userEmail_entry = customtkinter.CTkEntry(self.window)
         self.userEmail_entry.grid(row=0, column=1, padx=(20, 20), pady=(20, 0), sticky="nsew")
 
-        self.userPass_label = customtkinter.CTkLabel(self.window, text="Password:", anchor="w")
-        self.userPass_label.grid(row=1, column=0, padx=(20, 0), pady=(20, 0), sticky="nsew")
-        self.userPass_entry = customtkinter.CTkEntry(self.window, show="*")
-        self.userPass_entry.grid(row=1, column=1, padx=(20, 20), pady=(20, 0), sticky="nsew")
+        ## email/pass auth broken, replaced with access token auth
+        #self.userPass_label = customtkinter.CTkLabel(self.window, text="Password:", anchor="w")
+        #self.userPass_label.grid(row=1, column=0, padx=(20, 0), pady=(20, 0), sticky="nsew")
+        #self.userPass_entry = customtkinter.CTkEntry(self.window, show="*")
+        #self.userPass_entry.grid(row=1, column=1, padx=(20, 20), pady=(20, 0), sticky="nsew")
 
         self.save_button = customtkinter.CTkButton(self.window, text="Save", command=self.save_login_button_event)
         self.save_button.grid(row=5, column=0, columnspan=2, padx=(20, 20), pady=(20, 20), sticky="nsew")
 
         file_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "login")
         if os.path.exists(file_path):
             with open(file_path, "r") as f:
@@ -221,17 +222,16 @@
                 self.phoneNumber_entry.insert(0, f.readline().rstrip())
 
 
     def save_login_button_event(self):
         file_dir = os.path.dirname(os.path.abspath(__file__))
         file_path = os.path.join(file_dir, "login")
         with open(file_path, "w") as f:
-            f.write(self.userEmail_entry.get() + "\n")
-            f.write(self.userPass_entry.get() + "\n")
-        self.textbox.insert("end", "Login info saved.\n")
+            f.write(self.userEmail_entry.get())
+        self.textbox.insert("end", "Access token saved.\n")
         self.window.destroy()
 
 
     def save_user_button_event(self):
         file_dir = os.path.dirname(os.path.abspath(__file__))
         file_path = os.path.join(file_dir, "settings")
         with open(file_path, "w") as f:
```

### Comparing `CoverGPT-1.2.0/CoverGPT/template.tex` & `CoverGPT-1.3.0/CoverGPT/template.tex`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/CoverGPT.egg-info/PKG-INFO` & `CoverGPT-1.3.0/CoverGPT.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: CoverGPT
-Version: 1.2.0
+Version: 1.3.0
 Summary: Generate a personalized and formatted cover letter for a given job position, using your resume to add personalized details. Utilizes ChatGPT.
 Home-page: https://github.com/mahfoozm/CoverGPT
-Download-URL: https://github.com/mahfoozm/CoverGPT/archive/refs/tags/v1.2.0.tar.gz
+Download-URL: https://github.com/mahfoozm/CoverGPT/archive/refs/tags/v1.3.0.tar.gz
 Author: Mohammad Mahfooz
 Author-email: mohammadmahfoozpersonal@gmail.com
 License: gpl-3.0
 Keywords: ChatGPT,AI,Cover Letter
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Utilities
```

### Comparing `CoverGPT-1.2.0/CoverGPT.egg-info/SOURCES.txt` & `CoverGPT-1.3.0/CoverGPT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/LICENSE` & `CoverGPT-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CoverGPT-1.2.0/PKG-INFO` & `CoverGPT-1.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: CoverGPT
-Version: 1.2.0
+Version: 1.3.0
 Summary: Generate a personalized and formatted cover letter for a given job position, using your resume to add personalized details. Utilizes ChatGPT.
 Home-page: https://github.com/mahfoozm/CoverGPT
-Download-URL: https://github.com/mahfoozm/CoverGPT/archive/refs/tags/v1.2.0.tar.gz
+Download-URL: https://github.com/mahfoozm/CoverGPT/archive/refs/tags/v1.3.0.tar.gz
 Author: Mohammad Mahfooz
 Author-email: mohammadmahfoozpersonal@gmail.com
 License: gpl-3.0
 Keywords: ChatGPT,AI,Cover Letter
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Utilities
```

### Comparing `CoverGPT-1.2.0/README.md` & `CoverGPT-1.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,56 @@
 # CoverGPT
-Generate a personalized & formatted cover letter for a job position, using your resume to add personalized details.
 
-![image](https://user-images.githubusercontent.com/95328615/216740257-41b94c3d-3f1c-491d-ab5c-904d40a2033e.png)
+[![PyPi](https://img.shields.io/pypi/v/CoverGPT.svg)](https://pypi.python.org/pypi/CoverGPT)
+[![Downloads](https://static.pepy.tech/badge/CoverGPT)](https://pypi.python.org/pypi/CoverGPT)
 
-## API Key
-To use CoverGPT, you need a ChatGPT API key. To get one, make a ChatGPT account and go to [this link](https://platform.openai.com/account/api-keys). Generate an API key and set it in CoverGPT.
+Generate a personalized & formatted cover letter for a given job position utilizing your resume.
 
-## Usage
-Clone the repository. Before generating your first cover letter, ensure that you have set your API key and filled out your user information. If you want a more personalized cover letter, upload your resume. You can still generate a cover letter without uploading your resume; but it will be of much lower quality.
+![CoverGPT](https://user-images.githubusercontent.com/95328615/218336746-7d12fbac-70a2-4125-b2a5-b93919d66169.png)
 
-## Requirements
-Requires the following python packages:
-tk, customtkinter, PyPDF2, revChatGPT
+## Installation
 
-You also need XeTeX installed on your system.
+> You will need [Python 3.9+](https://www.python.org/downloads/) (with Tcl/Tk) and a [TeX](https://www.tug.org/texlive/) distribution installed on your system.
+
+Install with this command (enter in command prompt/terminal):
+
+```
+pip install CoverGPT
+```
+
+Run with this command:
+
+```
+python3 -m CoverGPT
+```
+
+Before generating your first cover letter, ensure that you have logged in and filled out your user information. If you want a more personalized cover letter, upload your resume. You can still generate a cover letter without uploading your resume; but it will be of much lower quality.
+
+### Login
+
+To use CoverGPT, you need a ChatGPT account. To make an account, head to [this link](https://chat.openai.com/chat) and click sign up. Then, login to CoverGPT using your access token (which can be found [here](https://chat.openai.com/api/auth/session), make sure you are logged into ChatGPT before heading to that link).
 
 ## Example
-Example of a cover letter generated using CoverGPT (using the included cover letter template)
 
-![example](https://user-images.githubusercontent.com/95328615/216749052-9fab03dc-f02a-4523-967f-e07f382618b4.png)
+Example of a cover letter generated using CoverGPT (using the included template)
 
+![example](https://user-images.githubusercontent.com/95328615/216749052-9fab03dc-f02a-4523-967f-e07f382618b4.png)
 
 ## Using your own cover letter template
+
 A LaTeX template is provided, but you can use your own if you wish. If you choose to use your own template, make the following replacements in your .tex file:
+
 - First Name: #firstName
 - Last Name: #lastName
 - Website Link: #websiteUrl
 - Email: #email
 - Phone Number: #phoneNumber
 - Full Name: #fullName
 - Company Name: #companyName
 - Company Address: #address1
 - City, State/Province, Zip/Postal Code: #address2
 
 Insert a \vspace{0.5cm} at the bottom of your template (this is where the paragraph body will be inserted).
 
 ### TO-DO:
 
-- add requirements to a txt file, to simplify installation
-- considering a CoverGPT web app, to simplify usage
+- considering a CoverGPT web app, for simplified usage
```

### Comparing `CoverGPT-1.2.0/setup.py` & `CoverGPT-1.3.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from distutils.core import setup
 setup(
   name = 'CoverGPT',    
   packages = ['CoverGPT'], 
-  version = '1.2.0',
+  version = '1.3.0',
   license='gpl-3.0',
   description = 'Generate a personalized and formatted cover letter for a given job position, using your resume to add personalized details. Utilizes ChatGPT.',   # Give a short description about your library
   author = 'Mohammad Mahfooz',  
   author_email = 'mohammadmahfoozpersonal@gmail.com', 
   url = 'https://github.com/mahfoozm/CoverGPT',
-  download_url = 'https://github.com/mahfoozm/CoverGPT/archive/refs/tags/v1.2.0.tar.gz',
+  download_url = 'https://github.com/mahfoozm/CoverGPT/archive/refs/tags/v1.3.0.tar.gz',
   keywords = ['ChatGPT', 'AI', 'Cover Letter'],
   install_requires=[
           'customtkinter==5.0.3',
           'PyPDF2==3.0.1',
-          'revChatGPT==3.3.4'
+          'revChatGPT==4.2.0'
       ],
   classifiers=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: End Users/Desktop',
     'Topic :: Utilities',
     'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
     'Programming Language :: Python :: 3',
```

