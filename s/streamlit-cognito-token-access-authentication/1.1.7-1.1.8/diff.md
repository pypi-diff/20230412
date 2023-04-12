# Comparing `tmp/streamlit_cognito_token_access_authentication-1.1.7-py3-none-any.whl.zip` & `tmp/streamlit_cognito_token_access_authentication-1.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 17298 bytes, number of entries: 13
+Zip file size: 17281 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       66 b- defN 22-Dec-30 19:25 cognito-authentication-streamlit-test/__init__.py
 -rw-r--r--  2.0 unx    11673 b- defN 22-Dec-30 19:33 cognito-authentication-streamlit-test/authentication.py
 -rw-r--r--  2.0 unx     2880 b- defN 22-Dec-28 15:58 cognito-authentication-streamlit-test/decode_verify_jwt.py
 -rw-r--r--  2.0 unx       66 b- defN 22-Dec-30 19:25 cognito_authentication_streamlit/__init__.py
 -rw-r--r--  2.0 unx    15805 b- defN 23-Mar-13 14:07 cognito_authentication_streamlit/authentication.py
 -rw-r--r--  2.0 unx     3450 b- defN 23-Jan-01 18:18 cognito_authentication_streamlit/decode_verify_jwt.py
 -rw-r--r--  2.0 unx       66 b- defN 22-Dec-30 19:25 streamlit_cognito_token_access_authentication/__init__.py
--rw-r--r--  2.0 unx    12040 b- defN 23-Apr-12 12:37 streamlit_cognito_token_access_authentication/authentication.py
+-rw-r--r--  2.0 unx    11985 b- defN 23-Apr-12 12:49 streamlit_cognito_token_access_authentication/authentication.py
 -rw-r--r--  2.0 unx     3361 b- defN 23-Apr-12 12:37 streamlit_cognito_token_access_authentication/decode_verify_jwt.py
--rw-r--r--  2.0 unx      894 b- defN 23-Apr-12 12:38 streamlit_cognito_token_access_authentication-1.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 12:38 streamlit_cognito_token_access_authentication-1.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Apr-12 12:38 streamlit_cognito_token_access_authentication-1.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1454 b- defN 23-Apr-12 12:38 streamlit_cognito_token_access_authentication-1.1.7.dist-info/RECORD
-13 files, 51893 bytes uncompressed, 14738 bytes compressed:  71.6%
+-rw-r--r--  2.0 unx      894 b- defN 23-Apr-12 12:49 streamlit_cognito_token_access_authentication-1.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 12:49 streamlit_cognito_token_access_authentication-1.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Apr-12 12:49 streamlit_cognito_token_access_authentication-1.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1454 b- defN 23-Apr-12 12:49 streamlit_cognito_token_access_authentication-1.1.8.dist-info/RECORD
+13 files, 51838 bytes uncompressed, 14721 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: streamlit_cognito_token_access_authentication/authentication.py
 Comment: 
 
 Filename: streamlit_cognito_token_access_authentication/decode_verify_jwt.py
 Comment: 
 
-Filename: streamlit_cognito_token_access_authentication-1.1.7.dist-info/METADATA
+Filename: streamlit_cognito_token_access_authentication-1.1.8.dist-info/METADATA
 Comment: 
 
-Filename: streamlit_cognito_token_access_authentication-1.1.7.dist-info/WHEEL
+Filename: streamlit_cognito_token_access_authentication-1.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: streamlit_cognito_token_access_authentication-1.1.7.dist-info/top_level.txt
+Filename: streamlit_cognito_token_access_authentication-1.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: streamlit_cognito_token_access_authentication-1.1.7.dist-info/RECORD
+Filename: streamlit_cognito_token_access_authentication-1.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamlit_cognito_token_access_authentication/authentication.py

```diff
@@ -23,16 +23,14 @@
     
     #CLIENT_IDs = {'dev': "ex1", 'qa': "ex2", 'prod': "ex3"}
     # pass env as query param, then use as dict key
     self.CLIENT_ID = self.CLIENT_IDs[env]
     """
 
     def __init__(self, config):
-        print(f'__init__ {config}')
-        print(f'__init__ {config["APP_ID"]}')
         self.COGNITO_DOMAIN = config["COGNITO_DOMAIN"]
         self.CLIENT_IDs = config["CLIENT_IDs"]
         self.CLIENT_ID = ""
         self.USERPOOL_ID = config["USERPOOL_ID"]
         self.REGION = config["REGION"]
         self.HTTP_PROXY = config["HTTP_PROXY"]
         self.APP_ID = config["APP_ID"] # used to authenticate a user in a cognito group.
@@ -208,14 +206,15 @@
         if location not in ['main', 'sidebar']:
             raise ValueError("Location must be one of 'main' or 'sidebar'")
         
         else:
             try:
                 token = None
                 user = ""
+                env = None
                 params = st.experimental_get_query_params()
                 env = params['env'][0]
                 user = params['user'][0]
                 token = params['token'][0]
                 #print(f'token from params: {token}')
             except Exception as e:
                 print(f'{e}')
```

## Comparing `streamlit_cognito_token_access_authentication-1.1.7.dist-info/METADATA` & `streamlit_cognito_token_access_authentication-1.1.8.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-cognito-token-access-authentication
-Version: 1.1.7
+Version: 1.1.8
 Summary: Cognito token access authentication with streamlit
 Author: Sean Tasaki
 Keywords: cognito,streamlit,access token
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `streamlit_cognito_token_access_authentication-1.1.7.dist-info/RECORD` & `streamlit_cognito_token_access_authentication-1.1.8.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 cognito-authentication-streamlit-test/__init__.py,sha256=5_uvvgsgur8oyU9hddFDmAJbIhXYDdXVgR9xYW9YrBM,66
 cognito-authentication-streamlit-test/authentication.py,sha256=OjxS46hOZzZbVsZtuyx-T1qTOrXRx0FsQnVE3NhOjdQ,11673
 cognito-authentication-streamlit-test/decode_verify_jwt.py,sha256=O7YQBzuNWZ6AEHeJI8XlkX4e1dF_CLoj2VdeO80kp2g,2880
 cognito_authentication_streamlit/__init__.py,sha256=5_uvvgsgur8oyU9hddFDmAJbIhXYDdXVgR9xYW9YrBM,66
 cognito_authentication_streamlit/authentication.py,sha256=3RpOPxS3YyjmGJu-r8Aw8uK0lcHzFttYo98wA0Bn0Ek,15805
 cognito_authentication_streamlit/decode_verify_jwt.py,sha256=4qws6yOnlVi8tFzffwFbxNcV87JEnYBQdKoSHAzrgT4,3450
 streamlit_cognito_token_access_authentication/__init__.py,sha256=5_uvvgsgur8oyU9hddFDmAJbIhXYDdXVgR9xYW9YrBM,66
-streamlit_cognito_token_access_authentication/authentication.py,sha256=RtIAjc4kwqm0HwsT6iEf8ow-woInTiEDHfvO9tbTNl0,12040
+streamlit_cognito_token_access_authentication/authentication.py,sha256=YbDAtOyn1_ZsqsXpVICIqhTSLLyVAW4-Jwfs2wqGTFs,11985
 streamlit_cognito_token_access_authentication/decode_verify_jwt.py,sha256=FLejWtwV01HQcbH5demY9GkEe26ZokKlPs9FPT4jn-4,3361
-streamlit_cognito_token_access_authentication-1.1.7.dist-info/METADATA,sha256=22kglC5tz5mGScDNN9s13eZYjqfe9UOAUBEsgpVZJs4,894
-streamlit_cognito_token_access_authentication-1.1.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-streamlit_cognito_token_access_authentication-1.1.7.dist-info/top_level.txt,sha256=GAa8tNUySCFwPC0VuD3Ulp2SSNm6sriYlQ70oQV1SCk,46
-streamlit_cognito_token_access_authentication-1.1.7.dist-info/RECORD,,
+streamlit_cognito_token_access_authentication-1.1.8.dist-info/METADATA,sha256=qMwkomhs2eRbALTwykflJ-WNAY9ZutU9CV2quYbVkl4,894
+streamlit_cognito_token_access_authentication-1.1.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+streamlit_cognito_token_access_authentication-1.1.8.dist-info/top_level.txt,sha256=GAa8tNUySCFwPC0VuD3Ulp2SSNm6sriYlQ70oQV1SCk,46
+streamlit_cognito_token_access_authentication-1.1.8.dist-info/RECORD,,
```

