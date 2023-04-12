# Comparing `tmp/pyttsx4-3.0.5-py3-none-any.whl.zip` & `tmp/pyttsx4-3.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 33285 bytes, number of entries: 16
+Zip file size: 33344 bytes, number of entries: 16
 -rw-r--r--  2.0 unx      814 b- defN 23-Apr-07 13:37 pyttsx4/__init__.py
 -rw-r--r--  2.0 unx     7429 b- defN 23-Apr-07 17:19 pyttsx4/driver.py
 -rw-r--r--  2.0 unx     7224 b- defN 23-Apr-07 13:37 pyttsx4/engine.py
 -rw-r--r--  2.0 unx    29524 b- defN 23-Apr-11 03:46 pyttsx4/six.py
 -rw-r--r--  2.0 unx      431 b- defN 23-Apr-07 13:37 pyttsx4/voice.py
 -rw-r--r--  2.0 unx      853 b- defN 23-Apr-11 03:47 pyttsx4/drivers/__init__.py
 -rw-r--r--  2.0 unx    19495 b- defN 23-Apr-07 13:37 pyttsx4/drivers/_espeak.py
 -rw-r--r--  2.0 unx     6182 b- defN 23-Apr-07 13:37 pyttsx4/drivers/dummy.py
 -rw-r--r--  2.0 unx     7448 b- defN 23-Apr-11 03:43 pyttsx4/drivers/espeak.py
--rw-r--r--  2.0 unx     3729 b- defN 23-Apr-07 14:49 pyttsx4/drivers/nsss.py
+-rw-r--r--  2.0 unx     3895 b- defN 23-Apr-12 08:25 pyttsx4/drivers/nsss.py
 -rw-r--r--  2.0 unx     6552 b- defN 23-Apr-11 03:47 pyttsx4/drivers/sapi5.py
--rw-r--r--  2.0 unx    17098 b- defN 23-Apr-11 10:00 pyttsx4-3.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     1821 b- defN 23-Apr-11 10:00 pyttsx4-3.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 10:00 pyttsx4-3.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-11 10:00 pyttsx4-3.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1244 b- defN 23-Apr-11 10:00 pyttsx4-3.0.5.dist-info/RECORD
-16 files, 109944 bytes uncompressed, 31265 bytes compressed:  71.6%
+-rw-r--r--  2.0 unx    17098 b- defN 23-Apr-12 08:28 pyttsx4-3.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1821 b- defN 23-Apr-12 08:28 pyttsx4-3.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 08:28 pyttsx4-3.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-12 08:28 pyttsx4-3.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1244 b- defN 23-Apr-12 08:28 pyttsx4-3.0.6.dist-info/RECORD
+16 files, 110110 bytes uncompressed, 31324 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: pyttsx4/drivers/nsss.py
 Comment: 
 
 Filename: pyttsx4/drivers/sapi5.py
 Comment: 
 
-Filename: pyttsx4-3.0.5.dist-info/LICENSE
+Filename: pyttsx4-3.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: pyttsx4-3.0.5.dist-info/METADATA
+Filename: pyttsx4-3.0.6.dist-info/METADATA
 Comment: 
 
-Filename: pyttsx4-3.0.5.dist-info/WHEEL
+Filename: pyttsx4-3.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: pyttsx4-3.0.5.dist-info/top_level.txt
+Filename: pyttsx4-3.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: pyttsx4-3.0.5.dist-info/RECORD
+Filename: pyttsx4-3.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyttsx4/drivers/nsss.py

```diff
@@ -94,14 +94,19 @@
         else:
             raise KeyError('unknown property %s' % name)
 
     @objc.python_method
     def save_to_file(self, text, filename):
         url = Foundation.NSURL.fileURLWithPath_(filename)
         self._tts.startSpeakingString_toURL_(text, url)
+        import time
+        time.sleep(0.1)
+        # needed so script doesn't end w/o talking
+        while self._tts.isSpeaking():
+            time.sleep(0.1)
 
     def speechSynthesizer_didFinishSpeaking_(self, tts, success):
         if not self._completed:
             success = False
         else:
             success = True
         self._proxy.notify('finished-utterance', completed=success)
```

## Comparing `pyttsx4-3.0.5.dist-info/LICENSE` & `pyttsx4-3.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyttsx4-3.0.5.dist-info/METADATA` & `pyttsx4-3.0.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyttsx4
-Version: 3.0.5
+Version: 3.0.6
 Summary: Text to Speech (TTS) library for Python 3. Works without internet connection or delay. Supports multiple TTS engines, including Sapi5, nsss, and espeak.
 Home-page: https://github.com/Jiangshan00001/pyttsx4
 Author: Natesh M Bhat
 Author-email: 710806594@qq.com
 License: UNKNOWN
 Keywords: pyttsx,ivona,pyttsx for python3,TTS for python3,pyttsx3,text to speech for python,tts,text to speech,speech,speech synthesis,offline text to speech,offline tts,gtts
 Platform: UNKNOWN
```

## Comparing `pyttsx4-3.0.5.dist-info/RECORD` & `pyttsx4-3.0.6.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 pyttsx4/engine.py,sha256=UJBrPIcN3KXmBCABrb2uY4F_AeAaFlC5h6n_L3V0euA,7224
 pyttsx4/six.py,sha256=yVeu0rLX2Qv1P1UaJtvamDmMrjnxNsJkSuztEvVyGG8,29524
 pyttsx4/voice.py,sha256=GYZLgGtnmjLrg93Wh7_lqDcs6zMaTS_QRr3KZM7RZnY,431
 pyttsx4/drivers/__init__.py,sha256=EFf83iBpSVF4joEh4gQmq5Rl22tngVNuR1zBeWfCdjQ,853
 pyttsx4/drivers/_espeak.py,sha256=Gj0N4aFf3YGZO9fq8K5BFbiwkIExqDu1nBXUn7EZVzY,19495
 pyttsx4/drivers/dummy.py,sha256=d7K46sijjOxwmAJHbgEALwbYwGcktLfW1FcX1iG5I8E,6182
 pyttsx4/drivers/espeak.py,sha256=5QcaVaCyb3xLKXs6_fjnGv0-mioUXINzendba95mpgs,7448
-pyttsx4/drivers/nsss.py,sha256=n849K4ugK87S4ejtc_7xYp5W__maB6vfRX_sxIWlGIU,3729
+pyttsx4/drivers/nsss.py,sha256=n0_ysxWeZhqQuiaxpzZo5RYOIl2Ef0yvX7Kj4du30yo,3895
 pyttsx4/drivers/sapi5.py,sha256=EiEEwvammMCS4YI7aWG0fmtQZm_0-bPJqC9nndUUpp4,6552
-pyttsx4-3.0.5.dist-info/LICENSE,sha256=JoTeFzAOCkNGhvHsf4r2BFIHpLRXo_4EsrnOZV58XVA,17098
-pyttsx4-3.0.5.dist-info/METADATA,sha256=8bpbU-vrPfj6H6ZHwQx0sBwAxo9D-37DDFZKIR1tb8Y,1821
-pyttsx4-3.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyttsx4-3.0.5.dist-info/top_level.txt,sha256=RZW_EXmaQg7go8T0q583RzqdJUlYm0NeSHGpyq92tiY,8
-pyttsx4-3.0.5.dist-info/RECORD,,
+pyttsx4-3.0.6.dist-info/LICENSE,sha256=JoTeFzAOCkNGhvHsf4r2BFIHpLRXo_4EsrnOZV58XVA,17098
+pyttsx4-3.0.6.dist-info/METADATA,sha256=GIyd80nO4G1JqUOWIR4p8t5WAWdqNh5Y6TK7kINJD6w,1821
+pyttsx4-3.0.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pyttsx4-3.0.6.dist-info/top_level.txt,sha256=RZW_EXmaQg7go8T0q583RzqdJUlYm0NeSHGpyq92tiY,8
+pyttsx4-3.0.6.dist-info/RECORD,,
```

