# Comparing `tmp/audioace-0.0.0.tar.gz` & `tmp/audioace-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioace-0.0.0.tar", last modified: Wed Apr 12 10:48:21 2023, max compression
+gzip compressed data, was "audioace-0.0.4.tar", last modified: Wed Apr 12 17:54:35 2023, max compression
```

## Comparing `audioace-0.0.0.tar` & `audioace-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 10:48:21.242639 audioace-0.0.0/
--rw-rw-rw-   0        0        0     1088 2023-04-12 10:47:13.000000 audioace-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      466 2023-04-12 10:48:21.241648 audioace-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-12 10:47:26.000000 audioace-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 10:48:21.215831 audioace-0.0.0/audioace/
--rw-rw-rw-   0        0        0     5078 2023-04-12 10:45:51.000000 audioace-0.0.0/audioace/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:48:21.238400 audioace-0.0.0/audioace.egg-info/
--rw-rw-rw-   0        0        0      466 2023-04-12 10:48:21.000000 audioace-0.0.0/audioace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-04-12 10:48:21.000000 audioace-0.0.0/audioace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 10:48:21.000000 audioace-0.0.0/audioace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 10:48:21.000000 audioace-0.0.0/audioace.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 10:48:21.000000 audioace-0.0.0/audioace.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 10:48:21.242639 audioace-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      818 2023-04-12 10:47:53.000000 audioace-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:54:35.776406 audioace-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2023-04-12 10:47:13.000000 audioace-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2554 2023-04-12 17:54:35.774412 audioace-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2017 2023-04-12 16:26:03.000000 audioace-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 17:54:35.755510 audioace-0.0.4/audioace/
+-rw-rw-rw-   0        0        0     5037 2023-04-12 13:44:21.000000 audioace-0.0.4/audioace/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:54:35.772419 audioace-0.0.4/audioace.egg-info/
+-rw-rw-rw-   0        0        0     2554 2023-04-12 17:54:35.000000 audioace-0.0.4/audioace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-04-12 17:54:35.000000 audioace-0.0.4/audioace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 17:54:35.000000 audioace-0.0.4/audioace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 17:54:35.000000 audioace-0.0.4/audioace.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 17:54:35.000000 audioace-0.0.4/audioace.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 17:54:35.776406 audioace-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-04-12 17:54:31.000000 audioace-0.0.4/setup.py
```

### Comparing `audioace-0.0.0/LICENSE` & `audioace-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `audioace-0.0.0/audioace/__init__.py` & `audioace-0.0.4/audioace/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,24 +8,21 @@
 import time
 from spotipy.oauth2 import SpotifyOAuth
 from requests.auth import HTTPBasicAuth
 import urllib.parse as parse
 import webbrowser
         
 class Download():
-    def __init__(self, path, client_id, client_secret, redirect_uri, file="songs_name.txt"):
+    def __init__(self, file="songs_name.txt", path = "Songs"):
         self.path = path
         self.vid_ext = "mp4"
         self.aud_ext = "mp3"
         self.command = ('ffmpeg -i "{from_video_path}" '
                         '-f {audio_ext} -ab 192000 '
                         '-vn "{to_audio_path}"')
-        self.client_id = client_id
-        self.client_secret = client_secret
-        self.redirect_uri = redirect_uri
         self.auth_url = "https://accounts.spotify.com/authorize"
         self.token_url = "https://accounts.spotify.com/api/token"
         self.file = file
 
         isExist = os.path.exists(self.path)
         if not isExist:
             os.mkdir(self.path)
@@ -55,16 +52,16 @@
                     from_video_path=f, audio_ext=self.aud_ext, to_audio_path=audio_file_name,
                 )
                 os.system(command)
             os.remove(new_file)
 
             print(yt.title + " has been successfully downloaded.")
 
-    def get_songs_from_playlist(self, playlist_link):
-        client_cred = SpotifyClientCredentials(client_id=self.client_id, client_secret=self.client_secret)
+    def get_songs_from_playlist(self, client_id, client_secret, playlist_link):
+        client_cred = SpotifyClientCredentials(client_id=client_id, client_secret=client_secret)
         sp = spotipy.Spotify(client_credentials_manager=client_cred)
 
         playlist_URI = playlist_link.split("/")[-1].split("?")[0]
 
         offset = 0
         t_end = time.time() + 3
 
@@ -73,40 +70,40 @@
                 #Track name
                 track_name = track["track"]["name"]
                 with open(self.file, "a", encoding="utf-8") as f:
                     f.write(track_name + "\n")
                     f.close()
             offset +=100
 
-    def authenticate(self,scope=None):
+    def authenticate(self,client_id, client_secret, redirect_uri, scope=None):
         '''Implement OAuth 2 Spotify authentication'''
         # Application: Request authorization to access data
-        payload = {'client_id': self.client_id,
+        payload = {'client_id': client_id,
                 'response_type': 'code',
-                'redirect_uri': self.redirect_uri,
+                'redirect_uri': redirect_uri,
                 'show_dialog': 'true'} # allow second account to login
         if scope:
             payload['scope'] = scope
         auth_url = '{}?{}'.format(self.auth_url, parse.urlencode(payload))
         # Spotify: Displays scopes & prompts user to login (if required)
         # User: Logs in, authorizes access
         webbrowser.open(auth_url)
 
         response = input('Enter the URL you were redirected to: ')
         code = parse.parse_qs(parse.urlparse(response).query)['code'][0]
 
-        payload = {'redirect_uri': self.redirect_uri,
+        payload = {'redirect_uri': redirect_uri,
                 'code': code,
                 'grant_type': 'authorization_code'}
         if scope:
             payload['scope'] = scope
 
         # Application: Request access and refresh tokens
         # Spotify: Returns access and refresh tokens
-        auth = HTTPBasicAuth(self.client_id, self.client_secret)
+        auth = HTTPBasicAuth(client_id, client_secret)
         response = requests.post(self.token_url, data=payload, auth=auth)
         if response.status_code != 200:
             response.raise_for_status()
         token_info = response.json()
         token_info['expires_at'] = int(time.time()) + token_info['expires_in']
         token_info['scope'] = scope
         return token_info
@@ -114,16 +111,16 @@
     def show_tracks(self, results):
         for item in results['items']:
             track = item['track']
             name = (track['artists'][0]['name'], track['name'])
             with open(self.file,"a", encoding="utf-8") as f:
                 f.write(str(name) + "\n")
 
-    def get_songs_from_liked_songs(self):
-        user = Download.authenticate(self,scope='user-library-read')
+    def get_songs_from_liked_songs(self, client_id, client_secret, redirect_uri):
+        user = Download.authenticate(self,client_id, client_secret, redirect_uri, scope='user-library-read')
         sp = spotipy.Spotify(auth= user['access_token'])
         results = sp.current_user_saved_tracks(limit=1, offset=0)
         while results['next']:
             results = sp.next(results)
             Download.show_tracks(self,results)
```

