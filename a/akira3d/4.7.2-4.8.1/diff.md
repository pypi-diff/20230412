# Comparing `tmp/akira3d-4.7.2.tar.gz` & `tmp/akira3d-4.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akira3d-4.7.2.tar", last modified: Sun Apr  9 19:25:28 2023, max compression
+gzip compressed data, was "akira3d-4.8.1.tar", last modified: Wed Apr 12 17:50:27 2023, max compression
```

## Comparing `akira3d-4.7.2.tar` & `akira3d-4.8.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 19:25:28.607980 akira3d-4.7.2/
--rw-rw-rw-   0        0        0      144 2023-04-09 19:25:28.607980 akira3d-4.7.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-09 19:25:28.603979 akira3d-4.7.2/akira3d/
--rw-rw-rw-   0        0        0      489 2023-03-27 07:34:49.000000 akira3d-4.7.2/akira3d/__init__.py
--rw-rw-rw-   0        0        0     2073 2023-04-09 18:03:38.000000 akira3d-4.7.2/akira3d/camera.py
--rw-rw-rw-   0        0        0     4879 2023-03-27 07:34:49.000000 akira3d-4.7.2/akira3d/colliders.py
--rw-rw-rw-   0        0        0      366 2023-03-27 07:34:49.000000 akira3d-4.7.2/akira3d/gameEngine.py
--rw-rw-rw-   0        0        0      505 2023-03-27 07:34:49.000000 akira3d-4.7.2/akira3d/light.py
--rw-rw-rw-   0        0        0      277 2023-03-27 07:34:49.000000 akira3d-4.7.2/akira3d/mesh.py
--rw-rw-rw-   0        0        0     1329 2023-03-27 07:34:49.000000 akira3d-4.7.2/akira3d/mobs.py
--rw-rw-rw-   0        0        0     7713 2023-04-09 19:23:39.000000 akira3d-4.7.2/akira3d/model.py
--rw-rw-rw-   0        0        0     1248 2023-03-27 07:34:49.000000 akira3d-4.7.2/akira3d/phisics.py
--rw-rw-rw-   0        0        0     6942 2023-03-27 07:34:49.000000 akira3d-4.7.2/akira3d/render.py
--rw-rw-rw-   0        0        0      882 2023-04-09 17:24:56.000000 akira3d-4.7.2/akira3d/shader_program.py
--rw-rw-rw-   0        0        0     2785 2023-04-09 17:24:56.000000 akira3d-4.7.2/akira3d/texture.py
--rw-rw-rw-   0        0        0     1413 2023-03-27 07:34:49.000000 akira3d-4.7.2/akira3d/vao.py
--rw-rw-rw-   0        0        0     5094 2023-04-09 17:25:55.000000 akira3d-4.7.2/akira3d/vbo.py
--rw-rw-rw-   0        0        0     2097 2023-04-09 17:24:56.000000 akira3d-4.7.2/akira3d/vidSys.py
-drwxrwxrwx   0        0        0        0 2023-04-09 19:25:28.606981 akira3d-4.7.2/akira3d.egg-info/
--rw-rw-rw-   0        0        0      144 2023-04-09 19:25:28.000000 akira3d-4.7.2/akira3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-04-09 19:25:28.000000 akira3d-4.7.2/akira3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 19:25:28.000000 akira3d-4.7.2/akira3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-09 19:25:28.000000 akira3d-4.7.2/akira3d.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-04-09 19:25:28.000000 akira3d-4.7.2/akira3d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 19:25:28.607980 akira3d-4.7.2/setup.cfg
--rw-rw-rw-   0        0        0      241 2023-04-09 19:25:23.000000 akira3d-4.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:50:27.204452 akira3d-4.8.1/
+-rw-rw-rw-   0        0        0      144 2023-04-12 17:50:27.204452 akira3d-4.8.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-12 17:50:27.200451 akira3d-4.8.1/akira3d/
+-rw-rw-rw-   0        0        0      518 2023-04-12 17:31:21.000000 akira3d-4.8.1/akira3d/__init__.py
+-rw-rw-rw-   0        0        0     2045 2023-04-12 17:20:27.000000 akira3d-4.8.1/akira3d/camera.py
+-rw-rw-rw-   0        0        0     4879 2023-03-27 07:34:49.000000 akira3d-4.8.1/akira3d/colliders.py
+-rw-rw-rw-   0        0        0      170 2023-04-12 17:46:39.000000 akira3d-4.8.1/akira3d/createNewGame.py
+-rw-rw-rw-   0        0        0      366 2023-03-27 07:34:49.000000 akira3d-4.8.1/akira3d/gameEngine.py
+-rw-rw-rw-   0        0        0      522 2023-04-12 17:17:16.000000 akira3d-4.8.1/akira3d/light.py
+-rw-rw-rw-   0        0        0      277 2023-03-27 07:34:49.000000 akira3d-4.8.1/akira3d/mesh.py
+-rw-rw-rw-   0        0        0     1329 2023-03-27 07:34:49.000000 akira3d-4.8.1/akira3d/mobs.py
+-rw-rw-rw-   0        0        0     7810 2023-04-11 08:26:43.000000 akira3d-4.8.1/akira3d/model.py
+-rw-rw-rw-   0        0        0     1248 2023-03-27 07:34:49.000000 akira3d-4.8.1/akira3d/phisics.py
+-rw-rw-rw-   0        0        0     6942 2023-04-11 08:32:00.000000 akira3d-4.8.1/akira3d/render.py
+-rw-rw-rw-   0        0        0      882 2023-04-09 17:24:56.000000 akira3d-4.8.1/akira3d/shader_program.py
+-rw-rw-rw-   0        0        0     2785 2023-04-09 17:24:56.000000 akira3d-4.8.1/akira3d/texture.py
+-rw-rw-rw-   0        0        0     1413 2023-03-27 07:34:49.000000 akira3d-4.8.1/akira3d/vao.py
+-rw-rw-rw-   0        0        0     5094 2023-04-09 17:25:55.000000 akira3d-4.8.1/akira3d/vbo.py
+-rw-rw-rw-   0        0        0     2097 2023-04-09 17:24:56.000000 akira3d-4.8.1/akira3d/vidSys.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:50:27.203451 akira3d-4.8.1/akira3d.egg-info/
+-rw-rw-rw-   0        0        0      144 2023-04-12 17:50:27.000000 akira3d-4.8.1/akira3d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-04-12 17:50:27.000000 akira3d-4.8.1/akira3d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 17:50:27.000000 akira3d-4.8.1/akira3d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-12 17:50:27.000000 akira3d-4.8.1/akira3d.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-04-12 17:50:27.000000 akira3d-4.8.1/akira3d.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 17:50:27.204452 akira3d-4.8.1/setup.cfg
+-rw-rw-rw-   0        0        0      241 2023-04-12 17:50:23.000000 akira3d-4.8.1/setup.py
```

### Comparing `akira3d-4.7.2/akira3d/camera.py` & `akira3d-4.8.1/akira3d/camera.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,27 +6,25 @@
     def __init__(self, app, position=(0,0,4), yaw=-90, pitch=0):
         self.app = app
         self.rotMouse = [0, 0]
         self.visible = True
         self.cinematog = False
         self.pcm = {True:[0.02, 0.94], False:[0.15, 0.5]}
         self.aspect_ratio = app.size[0] / app.size[1]
+        self.FOV = 60
+        self.NEAR = 0.1
+        self.FAR = 1000
         self.position = glm.vec3(position)
         self.up = glm.vec3(0, 1, 0)
         self.right = glm.vec3(1, 0, 0)
         self.forward = glm.vec3(0, 0, -1)
         self.yaw = yaw
         self.pitch = pitch
-        self.ini(80, 0.1, 10000)
         self.px, self.pn = 90, -90
-
-    def ini(self, fov, near, far):
-        self.FOV = fov
-        self.NEAR = near
-        self.FAR = far
+        self.view = 300
         self.gvm()
         self.gpm()
 
     def rot(self, rel):
         self.rotMouse[0] += rel[0] * self.pcm[self.cinematog][0]
         self.rotMouse[1] += rel[1] * self.pcm[self.cinematog][0]
 
@@ -38,14 +36,15 @@
         self.forward = glm.normalize(self.forward)
         self.right = glm.normalize(glm.cross(self.forward, glm.vec3(0,1,0)))
         self.up = glm.normalize(glm.cross(self.right, self.forward))
 
     def update(self):
         self.ucv()
         self.gvm()
+        self.gpm()
         self.yaw += self.rotMouse[0]
         self.pitch -= self.rotMouse[1]
         self.pitch = max(self.pn, min(self.px, self.pitch))
         self.rotMouse = [i * self.pcm[self.cinematog][1] for i in self.rotMouse]
 
     def vis(self): self.visible = not self.visible; pg.mouse.set_visible(self.visible); pg.event.set_grab(not(self.visible));
     def cin(self): self.cinematog = not self.cinematog
```

### Comparing `akira3d-4.7.2/akira3d/colliders.py` & `akira3d-4.8.1/akira3d/colliders.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.7.2/akira3d/mobs.py` & `akira3d-4.8.1/akira3d/mobs.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.7.2/akira3d/model.py` & `akira3d-4.8.1/akira3d/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     def __init__(self, app, vao_name, tex_id, pos, rot, scale, hitbox):
         super().__init__(app, vao_name, tex_id, pos, rot, scale, hitbox)
         self.on_init()
 
     def update(self):
         self.texture.use(location=0)
         [vao[0].program['camPos'].write(self.app.camera.position) for vao in self.vao.vaos]
+        [vao[0].program['view'].write(glm.int8(self.app.camera.view)) for vao in self.vao.vaos]
         [vao[0].program['m_view'].write(self.app.camera.m_view) for vao in self.vao.vaos]
         [vao[0].program['m_model'].write(self.m_model) for vao in self.vao.vaos]
 
         [vao[1].program['m_proj'].write(self.camera.m_proj) for vao in self.vao.vaos]
         [vao[1].program['m_view_light'].write(self.app.light.m_view_light) for vao in self.vao.vaos]
 
         [vao[0].program['m_proj'].write(self.app.camera.m_proj) for vao in self.vao.vaos]
```

### Comparing `akira3d-4.7.2/akira3d/phisics.py` & `akira3d-4.8.1/akira3d/phisics.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.7.2/akira3d/render.py` & `akira3d-4.8.1/akira3d/render.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,16 +137,16 @@
 
         pg.display.gl_set_attribute(pg.GL_CONTEXT_MAJOR_VERSION, 3)
         pg.display.gl_set_attribute(pg.GL_CONTEXT_MINOR_VERSION, 3)
         pg.display.gl_set_attribute(pg.GL_CONTEXT_PROFILE_MASK, pg.GL_CONTEXT_PROFILE_CORE)
 
         pg.display.set_mode(self.size, flags=pg.OPENGL | pg.DOUBLEBUF) if self.full else pg.display.set_mode(self.size, flags=pg.OPENGL | pg.DOUBLEBUF | pg.FULLSCREEN)
         self.ctx = mgl.create_context()
-        #self.ctx.front_face = 'cw' | mgl.CULL_FACE
-        self.ctx.enable(flags=mgl.DEPTH_TEST)
+        #self.ctx.front_face = 'cw'
+        self.ctx.enable(flags=mgl.DEPTH_TEST | mgl.CULL_FACE)
 
         self.clock = pg.time.Clock()
         self.camera = Camera(self)
 
         self.surf = pg.Surface(self.size, flags=pg.SRCALPHA)
         self.pg_texture = self.ctx.texture(self.size, 4)
         self.pg_texture.filter = mgl.NEAREST, mgl.NEAREST
```

### Comparing `akira3d-4.7.2/akira3d/shader_program.py` & `akira3d-4.8.1/akira3d/shader_program.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.7.2/akira3d/texture.py` & `akira3d-4.8.1/akira3d/texture.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.7.2/akira3d/vao.py` & `akira3d-4.8.1/akira3d/vao.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.7.2/akira3d/vbo.py` & `akira3d-4.8.1/akira3d/vbo.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.7.2/akira3d/vidSys.py` & `akira3d-4.8.1/akira3d/vidSys.py`

 * *Files identical despite different names*

