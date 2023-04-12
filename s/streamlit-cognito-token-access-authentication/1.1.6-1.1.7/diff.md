# Comparing `tmp/streamlit_cognito_token_access_authentication-1.1.6-py3-none-any.whl.zip` & `tmp/streamlit_cognito_token_access_authentication-1.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 17297 bytes, number of entries: 13
+Zip file size: 17298 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       66 b- defN 22-Dec-30 19:25 cognito-authentication-streamlit-test/__init__.py
 -rw-r--r--  2.0 unx    11673 b- defN 22-Dec-30 19:33 cognito-authentication-streamlit-test/authentication.py
 -rw-r--r--  2.0 unx     2880 b- defN 22-Dec-28 15:58 cognito-authentication-streamlit-test/decode_verify_jwt.py
 -rw-r--r--  2.0 unx       66 b- defN 22-Dec-30 19:25 cognito_authentication_streamlit/__init__.py
 -rw-r--r--  2.0 unx    15805 b- defN 23-Mar-13 14:07 cognito_authentication_streamlit/authentication.py
 -rw-r--r--  2.0 unx     3450 b- defN 23-Jan-01 18:18 cognito_authentication_streamlit/decode_verify_jwt.py
 -rw-r--r--  2.0 unx       66 b- defN 22-Dec-30 19:25 streamlit_cognito_token_access_authentication/__init__.py
--rw-r--r--  2.0 unx    11975 b- defN 23-Apr-12 12:13 streamlit_cognito_token_access_authentication/authentication.py
--rw-r--r--  2.0 unx     3441 b- defN 23-Mar-16 17:51 streamlit_cognito_token_access_authentication/decode_verify_jwt.py
--rw-r--r--  2.0 unx      894 b- defN 23-Apr-12 12:14 streamlit_cognito_token_access_authentication-1.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 12:14 streamlit_cognito_token_access_authentication-1.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Apr-12 12:14 streamlit_cognito_token_access_authentication-1.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1454 b- defN 23-Apr-12 12:14 streamlit_cognito_token_access_authentication-1.1.6.dist-info/RECORD
-13 files, 51908 bytes uncompressed, 14737 bytes compressed:  71.6%
+-rw-r--r--  2.0 unx    12040 b- defN 23-Apr-12 12:37 streamlit_cognito_token_access_authentication/authentication.py
+-rw-r--r--  2.0 unx     3361 b- defN 23-Apr-12 12:37 streamlit_cognito_token_access_authentication/decode_verify_jwt.py
+-rw-r--r--  2.0 unx      894 b- defN 23-Apr-12 12:38 streamlit_cognito_token_access_authentication-1.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 12:38 streamlit_cognito_token_access_authentication-1.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Apr-12 12:38 streamlit_cognito_token_access_authentication-1.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1454 b- defN 23-Apr-12 12:38 streamlit_cognito_token_access_authentication-1.1.7.dist-info/RECORD
+13 files, 51893 bytes uncompressed, 14738 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: streamlit_cognito_token_access_authentication/authentication.py
 Comment: 
 
 Filename: streamlit_cognito_token_access_authentication/decode_verify_jwt.py
 Comment: 
 
-Filename: streamlit_cognito_token_access_authentication-1.1.6.dist-info/METADATA
+Filename: streamlit_cognito_token_access_authentication-1.1.7.dist-info/METADATA
 Comment: 
 
-Filename: streamlit_cognito_token_access_authentication-1.1.6.dist-info/WHEEL
+Filename: streamlit_cognito_token_access_authentication-1.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: streamlit_cognito_token_access_authentication-1.1.6.dist-info/top_level.txt
+Filename: streamlit_cognito_token_access_authentication-1.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: streamlit_cognito_token_access_authentication-1.1.6.dist-info/RECORD
+Filename: streamlit_cognito_token_access_authentication-1.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamlit_cognito_token_access_authentication/authentication.py

```diff
@@ -227,17 +227,19 @@
             elif location == 'sidebar':
                 login_form = st.sidebar.form('Login', clear_on_submit=True)
             login_form.subheader(f'User Authentication {user}')
             #access_token = login_form.text_input("Access Token", value="", help="copy and paste" ,key="my_input")
             submitted = login_form.form_submit_button("Login", type="primary")
 
             if submitted:
-                print(f'query params: {params}')
                 print(f'env from params: {env}')
+                if not env:
+                    env = 'dev'
                 self.CLIENT_ID = self.CLIENT_IDs[env]
+                print(f'client_id: {self.CLIENT_ID}')
                 self.cognito_authenticate(access_token=token) 
         return st.session_state.authenticated, st.session_state.username
 
     def logout(self, button_name ='Logout', location ='main'):
         """
         Creates a logout button.
         Parameters
```

## streamlit_cognito_token_access_authentication/decode_verify_jwt.py

```diff
@@ -20,20 +20,18 @@
 # https://aws.amazon.com/blogs/compute/container-reuse-in-lambda/
 # with urllib.request.urlopen(keys_url) as f:
 #   response = f.read()
 # keys = json.loads(response.decode('utf-8'))['keys']
 
 def verify_jwt(event, proxies):
     #print(f'os.environ proxy {os.environ["HTTP_PROXY"]}')
-    print(f'proxies {proxies}')
     keys_url = 'https://cognito-idp.{}.amazonaws.com/{}/.well-known/jwks.json'.format(event['REGION'], event['USERPOOL_ID'])
 
     try:
         proxy_support = urllib.request.ProxyHandler(proxies)
-        print(f'proxy_support {proxy_support}')
         opener = urllib.request.build_opener(proxy_support)
         urllib.request.install_opener(opener)
         with urllib.request.urlopen(keys_url) as f:
             response = f.read()
         keys = json.loads(response.decode('utf-8'))['keys']
         token = event['token']
         # get the kid from the headers prior to verification
```

## Comparing `streamlit_cognito_token_access_authentication-1.1.6.dist-info/METADATA` & `streamlit_cognito_token_access_authentication-1.1.7.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-cognito-token-access-authentication
-Version: 1.1.6
+Version: 1.1.7
 Summary: Cognito token access authentication with streamlit
 Author: Sean Tasaki
 Keywords: cognito,streamlit,access token
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `streamlit_cognito_token_access_authentication-1.1.6.dist-info/RECORD` & `streamlit_cognito_token_access_authentication-1.1.7.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 cognito-authentication-streamlit-test/__init__.py,sha256=5_uvvgsgur8oyU9hddFDmAJbIhXYDdXVgR9xYW9YrBM,66
 cognito-authentication-streamlit-test/authentication.py,sha256=OjxS46hOZzZbVsZtuyx-T1qTOrXRx0FsQnVE3NhOjdQ,11673
 cognito-authentication-streamlit-test/decode_verify_jwt.py,sha256=O7YQBzuNWZ6AEHeJI8XlkX4e1dF_CLoj2VdeO80kp2g,2880
 cognito_authentication_streamlit/__init__.py,sha256=5_uvvgsgur8oyU9hddFDmAJbIhXYDdXVgR9xYW9YrBM,66
 cognito_authentication_streamlit/authentication.py,sha256=3RpOPxS3YyjmGJu-r8Aw8uK0lcHzFttYo98wA0Bn0Ek,15805
 cognito_authentication_streamlit/decode_verify_jwt.py,sha256=4qws6yOnlVi8tFzffwFbxNcV87JEnYBQdKoSHAzrgT4,3450
 streamlit_cognito_token_access_authentication/__init__.py,sha256=5_uvvgsgur8oyU9hddFDmAJbIhXYDdXVgR9xYW9YrBM,66
-streamlit_cognito_token_access_authentication/authentication.py,sha256=7G2CdO5sELXtU-eQL79qjaAky4vVoWJTrS1sNgmzKeg,11975
-streamlit_cognito_token_access_authentication/decode_verify_jwt.py,sha256=WhdZlCnjTmjXaTR7KTl117ATim5pgAsl62GKkbzDkWI,3441
-streamlit_cognito_token_access_authentication-1.1.6.dist-info/METADATA,sha256=p542-QES77BFIICImDtVrCLgDRDN_-mvC4DDp5Km9H4,894
-streamlit_cognito_token_access_authentication-1.1.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-streamlit_cognito_token_access_authentication-1.1.6.dist-info/top_level.txt,sha256=GAa8tNUySCFwPC0VuD3Ulp2SSNm6sriYlQ70oQV1SCk,46
-streamlit_cognito_token_access_authentication-1.1.6.dist-info/RECORD,,
+streamlit_cognito_token_access_authentication/authentication.py,sha256=RtIAjc4kwqm0HwsT6iEf8ow-woInTiEDHfvO9tbTNl0,12040
+streamlit_cognito_token_access_authentication/decode_verify_jwt.py,sha256=FLejWtwV01HQcbH5demY9GkEe26ZokKlPs9FPT4jn-4,3361
+streamlit_cognito_token_access_authentication-1.1.7.dist-info/METADATA,sha256=22kglC5tz5mGScDNN9s13eZYjqfe9UOAUBEsgpVZJs4,894
+streamlit_cognito_token_access_authentication-1.1.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+streamlit_cognito_token_access_authentication-1.1.7.dist-info/top_level.txt,sha256=GAa8tNUySCFwPC0VuD3Ulp2SSNm6sriYlQ70oQV1SCk,46
+streamlit_cognito_token_access_authentication-1.1.7.dist-info/RECORD,,
```

