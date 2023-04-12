# Comparing `tmp/django-user-notification-0.7.9.tar.gz` & `tmp/django_user_notification-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-user-notification-0.7.9.tar", max compression
+gzip compressed data, was "django_user_notification-0.8.0.tar", max compression
```

## Comparing `django-user-notification-0.7.9.tar` & `django_user_notification-0.8.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0    11347 2022-08-01 06:35:17.000000 django-user-notification-0.7.9/LICENSE
--rw-r--r--   0        0        0     4517 2022-08-04 11:20:59.880368 django-user-notification-0.7.9/README.md
--rw-r--r--   0        0        0       22 2022-08-08 08:46:34.939027 django-user-notification-0.7.9/notification/__init__.py
--rw-r--r--   0        0        0     4127 2022-08-01 03:08:17.000000 django-user-notification-0.7.9/notification/admin.py
--rw-r--r--   0        0        0       99 2022-08-01 03:08:17.000000 django-user-notification-0.7.9/notification/apps.py
--rw-r--r--   0        0        0     1301 2022-08-01 03:08:17.000000 django-user-notification-0.7.9/notification/backends/__init__.py
--rw-r--r--   0        0        0     4088 2022-08-01 03:08:17.000000 django-user-notification-0.7.9/notification/backends/aliyunsms.py
--rw-r--r--   0        0        0     3972 2022-08-01 03:08:17.000000 django-user-notification-0.7.9/notification/backends/dingchatbot.py
--rw-r--r--   0        0        0     4170 2022-08-08 06:38:56.158235 django-user-notification-0.7.9/notification/backends/dingtodotask.py
--rw-r--r--   0        0        0     4596 2022-08-01 03:08:17.000000 django-user-notification-0.7.9/notification/backends/dingworkmessage.py
--rw-r--r--   0        0        0     1193 2022-08-08 08:42:41.480190 django-user-notification-0.7.9/notification/backends/dummy.py
--rw-r--r--   0        0        0     2422 2022-08-01 03:08:17.000000 django-user-notification-0.7.9/notification/backends/email.py
--rw-r--r--   0        0        0     2216 2022-08-01 03:08:17.000000 django-user-notification-0.7.9/notification/backends/websocket.py
--rw-r--r--   0        0        0     6804 2022-08-08 08:43:35.213511 django-user-notification-0.7.9/notification/base.py
--rw-r--r--   0        0        0     1208 2022-08-01 03:08:17.000000 django-user-notification-0.7.9/notification/consumers.py
--rw-r--r--   0        0        0     4030 2022-08-01 03:08:17.000000 django-user-notification-0.7.9/notification/migrations/0001_initial.py
--rw-r--r--   0        0        0      630 2022-08-08 07:36:05.355986 django-user-notification-0.7.9/notification/migrations/0002_auto_20220808_0736.py
--rw-r--r--   0        0        0        0 2022-08-01 03:08:17.000000 django-user-notification-0.7.9/notification/migrations/__init__.py
--rw-r--r--   0        0        0     5639 2022-08-08 06:57:57.165420 django-user-notification-0.7.9/notification/models.py
--rw-r--r--   0        0        0      109 2022-08-01 03:08:17.000000 django-user-notification-0.7.9/notification/static/css/hide_admin_original.css
--rw-r--r--   0        0        0      174 2022-08-01 03:08:17.000000 django-user-notification-0.7.9/notification/urls.py
--rw-r--r--   0        0        0      785 2022-08-04 10:27:11.874598 django-user-notification-0.7.9/notification/utils.py
--rw-r--r--   0        0        0     1911 2022-08-08 08:46:34.944406 django-user-notification-0.7.9/pyproject.toml
--rw-r--r--   0        0        0     5672 2022-08-08 08:46:39.064463 django-user-notification-0.7.9/setup.py
--rw-r--r--   0        0        0     5699 2022-08-08 08:46:39.064859 django-user-notification-0.7.9/PKG-INFO
+-rw-r--r--   0        0        0    11347 2022-08-01 06:35:17.000000 django_user_notification-0.8.0/LICENSE
+-rw-r--r--   0        0        0     4502 2023-04-12 10:50:30.392725 django_user_notification-0.8.0/README.md
+-rw-r--r--   0        0        0       22 2023-04-12 11:14:59.782011 django_user_notification-0.8.0/notification/__init__.py
+-rw-r--r--   0        0        0     3805 2023-04-12 10:58:28.320016 django_user_notification-0.8.0/notification/admin.py
+-rw-r--r--   0        0        0      156 2023-03-06 01:45:02.889012 django_user_notification-0.8.0/notification/apps.py
+-rw-r--r--   0        0        0     1301 2022-08-01 03:08:17.000000 django_user_notification-0.8.0/notification/backends/__init__.py
+-rw-r--r--   0        0        0     4088 2022-08-01 03:08:17.000000 django_user_notification-0.8.0/notification/backends/aliyunsms.py
+-rw-r--r--   0        0        0     3967 2023-04-12 11:07:43.899930 django_user_notification-0.8.0/notification/backends/dingchatbot.py
+-rw-r--r--   0        0        0     4170 2022-08-08 06:38:56.158235 django_user_notification-0.8.0/notification/backends/dingtodotask.py
+-rw-r--r--   0        0        0     4591 2023-04-12 11:07:59.491019 django_user_notification-0.8.0/notification/backends/dingworkmessage.py
+-rw-r--r--   0        0        0     1193 2022-08-08 08:42:41.480190 django_user_notification-0.8.0/notification/backends/dummy.py
+-rw-r--r--   0        0        0     2417 2023-04-12 11:08:12.028162 django_user_notification-0.8.0/notification/backends/email.py
+-rw-r--r--   0        0        0     2216 2023-04-12 11:08:29.622794 django_user_notification-0.8.0/notification/backends/websocket.py
+-rw-r--r--   0        0        0     6710 2023-04-12 11:12:05.725862 django_user_notification-0.8.0/notification/base.py
+-rw-r--r--   0        0        0     1208 2022-08-01 03:08:17.000000 django_user_notification-0.8.0/notification/consumers.py
+-rw-r--r--   0        0        0     3989 2023-04-12 11:09:49.072702 django_user_notification-0.8.0/notification/migrations/0001_initial.py
+-rw-r--r--   0        0        0      630 2022-08-08 07:36:05.355986 django_user_notification-0.8.0/notification/migrations/0002_auto_20220808_0736.py
+-rw-r--r--   0        0        0      885 2022-08-10 09:10:18.668000 django_user_notification-0.8.0/notification/migrations/0003_auto_20220810_1710.py
+-rw-r--r--   0        0        0     1093 2022-08-12 07:05:54.107684 django_user_notification-0.8.0/notification/migrations/0004_auto_20220812_0705.py
+-rw-r--r--   0        0        0      884 2023-01-29 05:37:49.837884 django_user_notification-0.8.0/notification/migrations/0005_alter_message_id_alter_messagetemplate_id_and_more.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:08:17.000000 django_user_notification-0.8.0/notification/migrations/__init__.py
+-rw-r--r--   0        0        0     5188 2023-04-12 11:05:18.719018 django_user_notification-0.8.0/notification/models.py
+-rw-r--r--   0        0        0      109 2022-08-01 03:08:17.000000 django_user_notification-0.8.0/notification/static/css/hide_admin_original.css
+-rw-r--r--   0        0        0      174 2023-04-12 10:53:45.477657 django_user_notification-0.8.0/notification/urls.py
+-rw-r--r--   0        0        0      785 2022-08-04 10:27:11.874598 django_user_notification-0.8.0/notification/utils.py
+-rw-r--r--   0        0        0     1701 2023-04-12 11:14:59.787743 django_user_notification-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     5738 1970-01-01 00:00:00.000000 django_user_notification-0.8.0/PKG-INFO
```

### Comparing `django-user-notification-0.7.9/LICENSE` & `django_user_notification-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-user-notification-0.7.9/README.md` & `django_user_notification-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,20 +25,20 @@
 Installation
 -----
 
 Install using `pip`...
 
     pip install django-user-notification
 
-Add `'django_quill'` and `'notification'` to your `INSTALLED_APPS` setting.
+Add `'tinymce'` and `'notification'` to your `INSTALLED_APPS` setting.
 ```python
 INSTALLED_APPS = [
     'django.contrib.admin',
     ...
-    'django_quill',
+    'tinymce',
     'notification',
 ]
 ```
 
 Quick Start
 -----
 
@@ -50,15 +50,15 @@
 
 
 Add the following to your `settings.py` module:
 
 ```python
 INSTALLED_APPS = [
     ...  # Make sure to include the default installed apps here.
-    'django_quill',
+    'tinymce',
     'notification',
 ]
 
 DJANGO_USER_NOTIFICATION = {
     "aliyunsms": {
         "access_key_id": "Your Access Key ID",
         "access_key_secret": "Your Access Key Secret",
```

### Comparing `django-user-notification-0.7.9/notification/admin.py` & `django_user_notification-0.8.0/notification/admin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from django.contrib import admin, messages
 from django.contrib.admin import display
 from django.db import models
+from tinymce.widgets import TinyMCE
 from django.forms import Textarea
 from django.utils import timezone
 from django.utils.translation import gettext_lazy as _
 
 from .models import Message, MessageTemplate, Notification
 
 # Register your models here.
@@ -24,15 +25,15 @@
         "backend_kwargs",
         "message_kwargs",
         "content",
     ]
     ordering = ("-id",)
 
     formfield_overrides = {
-        models.TextField: {"widget": Textarea(attrs={"rows": 3, "cols": 38})},
+        models.TextField: {"widget": TinyMCE(attrs={"rows": 10, "cols": 38})},
         models.JSONField: {"widget": Textarea(attrs={"rows": 2, "cols": 38})},
     }
 
 
 @admin.register(Notification)
 class NotificationAdmin(admin.ModelAdmin):
     list_per_page = 15
@@ -43,44 +44,37 @@
         "is_ignored",
         "is_sent",
         "updated_at",
     ]
     list_select_related = ["to", "message"]
     list_filter = ["to", "is_sent", "message__msg_type"]
     search_fields = ["message__mark"]
-    autocomplete_fields = ["to", "message"]
+    autocomplete_fields = ["message"]
+    raw_id_fields = ["to"]
     actions = ["send", "read", "ignore"]
     ordering = ("-id",)
 
     def has_change_permission(self, request, obj=None):
         return False
 
     def send(self, request, queryset):
-        return NotImplemented
+        raise NotImplementedError
 
     def read(self, request, queryset):
         if queryset.count() > 0:
             queryset.update(has_read=True, updated_at=timezone.now())
 
         self.message_user(request, "Notification read", level=messages.SUCCESS)
 
     def ignore(self, request, queryset):
         if queryset.count() > 0:
             queryset.update(is_ignored=True, updated_at=timezone.now())
 
         self.message_user(request, "Notification ignored", level=messages.SUCCESS)
 
-    @display(description=_("Template"))
-    def get_message_template(self, obj):
-        return obj.message.template
-
-    @display(description=_("Render kwargs"))
-    def get_message_render_kwargs(self, obj):
-        return obj.message.render_kwargs
-
     @display(description=_("Title"))
     def get_message_title(self, obj):
         return obj.message.title
 
     @display(description=_("Message Mark"))
     def get_message_mark(self, obj):
         return obj.message.mark
@@ -102,16 +96,14 @@
                 "Message",
                 {
                     "fields": [
                         "get_message_title",
                         "get_message_type",
                         "get_message_mark",
                         "get_message_content",
-                        "get_message_template",
-                        "get_message_render_kwargs",
                     ]
                 },
             ),
             (
                 "Notification",
                 {
                     "fields": [
@@ -130,17 +122,16 @@
 
 @admin.register(Message)
 class MessageAdmin(admin.ModelAdmin):
     list_per_page = 15
     list_display = [
         "title",
         "msg_type",
-        "template",
         "mark",
         "created_at",
     ]
-    list_filter = ("msg_type", "template")
+    list_filter = ("msg_type",)
     search_fields = ["mark", "title"]
     ordering = ("-id",)
 
     def has_change_permission(self, request, obj=None):
         return False
```

### Comparing `django-user-notification-0.7.9/notification/backends/__init__.py` & `django_user_notification-0.8.0/notification/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `django-user-notification-0.7.9/notification/backends/aliyunsms.py` & `django_user_notification-0.8.0/notification/backends/aliyunsms.py`

 * *Files identical despite different names*

### Comparing `django-user-notification-0.7.9/notification/backends/dingchatbot.py` & `django_user_notification-0.8.0/notification/backends/dingchatbot.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
         self.webhook = webhook or self.notification_settting.get("webhook")
 
         super().__init__(*args, **kwargs)
 
     def render_template(self, template: MessageTemplate, context: dict) -> str:
         try:
-            html_content = Template(template.content.html).render(Context(context))
+            html_content = Template(template.content).render(Context(context))
             return markdownify(html_content)
         except Exception as e:
             raise ValueError("Render message failed: %s" % e)
 
     def make_content(
         self, title, content, recipients, recipient_field, **kwargs
     ) -> dict:
```

### Comparing `django-user-notification-0.7.9/notification/backends/dingtodotask.py` & `django_user_notification-0.8.0/notification/backends/dingtodotask.py`

 * *Files identical despite different names*

### Comparing `django-user-notification-0.7.9/notification/backends/dingworkmessage.py` & `django_user_notification-0.8.0/notification/backends/dingworkmessage.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                 "settings.DJANGO_USER_NOTIFICATION[{}]".format(self.id)
             )
 
         super().__init__(*args, **kwargs)
 
     def render_template(self, template: MessageTemplate, context: dict) -> str:
         try:
-            html_content = Template(template.content.html).render(Context(context))
+            html_content = Template(template.content).render(Context(context))
             return markdownify(html_content)
         except Exception as e:
             raise ValueError("Render message failed: %s" % e)
 
     def make_content(
         self, title, content, recipients, recipient_field, **kwargs
     ) -> dict:
```

### Comparing `django-user-notification-0.7.9/notification/backends/dummy.py` & `django_user_notification-0.8.0/notification/backends/dummy.py`

 * *Files identical despite different names*

### Comparing `django-user-notification-0.7.9/notification/backends/email.py` & `django_user_notification-0.8.0/notification/backends/email.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """
 
     id = "email"
     message_subtype = "html"
 
     def render_template(self, template: MessageTemplate, context: dict) -> str:
         try:
-            return Template(template.content.html).render(Context(context))
+            return Template(template.content).render(Context(context))
         except Exception as e:
             raise ValueError("Render message failed: %s" % e)
 
     def make_content(self, title, content, recipients, recipient_field, **kwargs):
         return {
             "subject": title,
             "body": content,
```

### Comparing `django-user-notification-0.7.9/notification/backends/websocket.py` & `django_user_notification-0.8.0/notification/backends/websocket.py`

 * *Files identical despite different names*

### Comparing `django-user-notification-0.7.9/notification/base.py` & `django_user_notification-0.8.0/notification/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import typing
 
 from django.contrib.auth.models import User
 from django.core.exceptions import ObjectDoesNotExist
 from django.template import Context, Template
+from markdownify import markdownify
 from django.utils.module_loading import import_string
 
 from notification.models import Message, MessageTemplate, Notification
 
 logger = logging.getLogger(__name__)
 
 
@@ -40,15 +41,15 @@
                 to=recipient,
                 message=message,
                 notify_kwargs=notify_kwargs or {},
                 is_sent=False,
             )
 
     def on_success(self, message, recipient, save=False, notify_kwargs=None):
-        logger.info("Successfully send message to recipient: %s", recipient)
+        logger.debug("Successfully send message to recipient: %s", recipient)
         if save:
             if message.pk is None:
                 message.save()
 
             if recipient is None:
                 return
 
@@ -57,15 +58,16 @@
                 message=message,
                 notify_kwargs=notify_kwargs or {},
                 is_sent=True,
             )
 
     def render_template(self, template: MessageTemplate, context: dict) -> str:
         try:
-            return Template(template.content.plain).render(Context(context))
+            html_content = Template(template.content).render(Context(context))
+            return markdownify(html_content).strip()
         except Exception as e:
             raise ValueError("Render message failed: %s" % e)
 
     def make_content(
         self, title, content, recipients, recipient_field, **kwargs
     ) -> dict:
         raise NotImplementedError
@@ -102,31 +104,29 @@
         message_kwargs: dict = None,
         **kwargs,
     ) -> None:
         """
         Send notification to receivers with template
         """
         rendered_content = self.render_template(template, context)
+        title = title or template.title
         message_kwargs = message_kwargs or {}
         if template.message_kwargs:
             message_kwargs = template.message_kwargs.update(message_kwargs)
 
-        title = title or template.title
-        message_content = self.make_content(
-            title, rendered_content, recipients, recipient_field, **message_kwargs
-        )
-        message = self.message_class(
-            title=title,
-            content=message_content,
-            template=template,
-            render_kwargs=context,
+        return self.send(
+            title,
+            recipients,
+            rendered_content,
             mark=mark,
-            msg_type=self.id,
+            save=save,
+            recipient_field=recipient_field,
+            message_kwargs=message_kwargs,
+            **kwargs,
         )
-        self.perform_send(message, recipients, recipient_field, save=save, **kwargs)
 
     def send(
         self,
         title: str,
         recipients: list[User],
         content: str,
         mark: str = None,
@@ -202,9 +202,9 @@
             backend.send(
                 title,
                 recipients,
                 message,
                 save=save,
                 recipient_field=recipient_field,
                 message_kwargs=message_kwargs,
-                mark=mark
+                mark=mark,
             )
```

### Comparing `django-user-notification-0.7.9/notification/consumers.py` & `django_user_notification-0.8.0/notification/consumers.py`

 * *Files identical despite different names*

### Comparing `django-user-notification-0.7.9/notification/migrations/0001_initial.py` & `django_user_notification-0.8.0/notification/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Generated by Django 3.2.12 on 2022-07-29 07:54
 
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
-import django_quill.fields
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
@@ -35,15 +34,15 @@
             name='MessageTemplate',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('name', models.CharField(max_length=64, verbose_name='Template Name')),
                 ('description', models.TextField(blank=True, null=True, verbose_name='Description')),
                 ('code', models.CharField(max_length=4, unique=True, verbose_name='Template Code')),
                 ('title', models.CharField(blank=True, max_length=64, null=True, verbose_name='Message Title')),
-                ('content', django_quill.fields.QuillField(verbose_name='Template Content')),
+                ('content', models.TextField(verbose_name='Template Content')),
                 ('backend_kwargs', models.JSONField(blank=True, default=dict, verbose_name='Backend Kwargs')),
                 ('message_kwargs', models.JSONField(blank=True, default=dict, verbose_name='Message Kwargs')),
             ],
             options={
                 'verbose_name': 'Message Template',
                 'db_table': 'message_template',
             },
```

### Comparing `django-user-notification-0.7.9/notification/migrations/0002_auto_20220808_0736.py` & `django_user_notification-0.8.0/notification/migrations/0002_auto_20220808_0736.py`

 * *Files identical despite different names*

### Comparing `django-user-notification-0.7.9/notification/models.py` & `django_user_notification-0.8.0/notification/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.conf import settings
 from django.contrib.postgres.indexes import GinIndex
 from django.db import models
 from django.utils.translation import gettext_lazy as _
-from django_quill.fields import QuillField
+from tinymce.models import HTMLField
 
 
 class NotificationQuerySet(models.QuerySet):
     def read(self):
         """
         return read notification messages
         """
@@ -105,15 +105,15 @@
 
     name = models.CharField(max_length=64, verbose_name=_("Template Name"))
     description = models.TextField(verbose_name=_("Description"), null=True, blank=True)
     code = models.CharField(max_length=4, verbose_name=_("Template Code"), unique=True)
     title = models.CharField(
         max_length=64, verbose_name=_("Message Title"), null=True, blank=True
     )
-    content = QuillField(verbose_name=_("Template Content"))
+    content = models.TextField(verbose_name=_("Template Content"))
     backend_kwargs = models.JSONField(
         verbose_name=_("Backend Kwargs"), blank=True, default=dict
     )
     message_kwargs = models.JSONField(
         verbose_name=_("Message Kwargs"), blank=True, default=dict
     )
 
@@ -160,27 +160,14 @@
         null=True,
         blank=True,
     )
     msg_type = models.CharField(
         max_length=64, verbose_name=_("Message Type"), db_index=True
     )
     content = models.TextField(verbose_name=_("Content"), null=True, blank=True)
-    template = models.ForeignKey(
-        MessageTemplate,
-        verbose_name=_("Template"),
-        db_constraint=False,
-        null=True,
-        blank=True,
-        on_delete=models.CASCADE,
-    )
-    render_kwargs = models.JSONField(
-        verbose_name=_("Render Kwargs"),
-        blank=True,
-        default=dict,
-    )
     created_at = models.DateTimeField(auto_now_add=True, verbose_name=_("Created At"))
 
     objects = models.Manager()
 
     class Meta:
         verbose_name = _("Message")
         db_table = "message"
@@ -190,13 +177,7 @@
                 name="mark_gin_index",
             ),
         ]
 
     def __str__(self):
         return str(self.title)
 
-    def save(self, **kwargs):
-        if self.template:
-            self.content = None
-
-        super().save(**kwargs)
-
```

### Comparing `django-user-notification-0.7.9/notification/utils.py` & `django_user_notification-0.8.0/notification/utils.py`

 * *Files identical despite different names*

### Comparing `django-user-notification-0.7.9/pyproject.toml` & `django_user_notification-0.8.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,19 @@
-[tool.black]
-line-length = 89
-target-version = ['py38', 'py39']
-include = '\.pyi?$'
-exclude = '''
-/(
-    \.eggs
-  | \.git
-  | \.hg
-  | \.mypy_cache
-  | \.tox
-  | \.venv
-  | _build
-  | buck-out
-  | build
-  | dist
-
-  # The following are specific to Black, you probably don't want those.
-  | blib2to3
-  | tests/data
-  | profiling
-  | migrations
-)/
-'''
-
-[tool.isort]
-profile = "black"
-known_first_party = ["notification"]
-default_section = "THIRDPARTY"
-skip = ["venv/", ".venv/"]
-skip_glob = ["**/migrations/*.py"]
-include_trailing_comma = true
-force_grid_wrap = 0
-use_parentheses = true
-
 [tool.commitizen]
-version = "0.7.9"
+version = "0.8.0"
 changelog_start_rev = "0.7.0"
 tag_format = "v$major.$minor.$patch$prerelease"
 version_files = [
     "pyproject.toml:version",
     "notification/__init__.py"
 ]
 
 [tool.poetry]
 name = "django-user-notification"
-version = "0.7.9"
+version = "0.8.0"
 description = "Django message notification package"
 authors = ["Aiden Lu <allaher@icloud.com>"]
 readme = "README.md"
 keywords = ["notification", "django"]
 packages = [
     { include = "notification" },
 ]
@@ -67,20 +32,48 @@
 [tool.poetry.dependencies]
 python = ">=3.8"
 django = ">=3.1"
 requests = "^2.27.1"
 channels = { version=">=3.0.4", optional=true }
 alibabacloud-dysmsapi20170525 = { version=">=2.0.16", optional=true }
 markdownify = ">=0.11.2"
-django-quill-editor = ">=0.1.40"
+django-tinymce = "^3.6.1"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^4.0.1"
 pytest = "^6.2.5"
 
 [tool.poetry.extras]
 channels = ["channels"]
 aliyunsms = ["alibabacloud-dysmsapi20170525"]
 
+[tool.black]
+line-length = 89
+target-version = ['py38', 'py39']
+include = '\.pyi?$'
+exclude = '''
+/(
+    \.eggs
+  | \.git
+  | \.hg
+  | \.mypy_cache
+  | \.tox
+  | \.venv
+  | _build
+  | buck-out
+  | build
+  | dist
+
+  # The following are specific to Black, you probably don't want those.
+  | blib2to3
+  | tests/data
+  | profiling
+  | migrations
+)/
+'''
+
+[tool.isort]
+profile = "black"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django-user-notification-0.7.9/setup.py` & `django_user_notification-0.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,182 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-user-notification
+Version: 0.8.0
+Summary: Django message notification package
+Home-page: https://github.com/aiden520/django-user-notification
+License: Apache-2.0
+Keywords: notification,django
+Author: Aiden Lu
+Author-email: allaher@icloud.com
+Requires-Python: >=3.8
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: aliyunsms
+Provides-Extra: channels
+Requires-Dist: alibabacloud-dysmsapi20170525 (>=2.0.16) ; extra == "aliyunsms"
+Requires-Dist: channels (>=3.0.4) ; extra == "channels"
+Requires-Dist: django (>=3.1)
+Requires-Dist: django-tinymce (>=3.6.1,<4.0.0)
+Requires-Dist: markdownify (>=0.11.2)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Project-URL: Repository, https://github.com/aiden520/django-user-notification
+Description-Content-Type: text/markdown
+
+# Django user notification
+
+[![Build Status](https://img.shields.io/github/workflow/status/anyidea/django-user-notification/CI/master)](https://github.com/anyidea/django-user-notification/actions?query=workflow%3ACI)
+[![GitHub license](https://img.shields.io/github/license/anyidea/django-user-notification)](https://github.com/anyidea/django-user-notification/blob/master/LICENSE)
+[![Documentation Status](https://readthedocs.org/projects/django-user-notification/badge/?version=latest)](https://django-user-notification.readthedocs.io/en/latest/?badge=latest)
+[![pypi-version](https://img.shields.io/pypi/v/django-user-notification.svg)](https://pypi.python.org/pypi/django-user-notification)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-user-notification)
+[![PyPI - Django Version](https://img.shields.io/badge/django-%3E%3D3.1-44B78B)](https://www.djangoproject.com/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+Overview
+-----
+Django user notification is intended to provide a way to send multiple types of notification messages to django users out of box.
+
+Documentation
+-----
+on the way...
+
+Requirements
+-----
+
+* Python 3.8, 3.9, 3.10
+* Django 3.1, 3.2, 4.0, 4.1
+
+Installation
+-----
+
+Install using `pip`...
+
+    pip install django-user-notification
+
+Add `'tinymce'` and `'notification'` to your `INSTALLED_APPS` setting.
+```python
+INSTALLED_APPS = [
+    'django.contrib.admin',
+    ...
+    'tinymce',
+    'notification',
+]
+```
+
+Quick Start
+-----
+
+Let's take a look at a quick start of using Django user notification to send notification messages to users.
+
+Run the `notification` migrations using:
+
+    python manage.py migrate notification
+
+
+Add the following to your `settings.py` module:
+
+```python
+INSTALLED_APPS = [
+    ...  # Make sure to include the default installed apps here.
+    'tinymce',
+    'notification',
+]
+
+DJANGO_USER_NOTIFICATION = {
+    "aliyunsms": {
+        "access_key_id": "Your Access Key ID",
+        "access_key_secret": "Your Access Key Secret",
+        "sign_name": "Your Sign Name",
+    },
+    "dingtalkchatbot": {
+        "webhook": "Your Webhook URL",
+    },
+    "dingtalkworkmessage": {
+        "agent_id": "Your App Agent ID",
+        "app_key": "Your App Key",
+        "app_secret": "Your App Secret",
+    },
+    "dingtalktodotask": {
+        "app_key": "Your App Key",
+        "app_secret": "Your App Secret",
+    },
+}
+```
 
-packages = \
-['notification', 'notification.backends', 'notification.migrations']
+Let's send a notification
 
-package_data = \
-{'': ['*'], 'notification': ['static/css/*']}
+``` {.python}
+from django.contrib.auth import get_user_model
+from notification.backends import notify_by_email, notify_by_dingtalk_workmessage
 
-install_requires = \
-['django-quill-editor>=0.1.40',
- 'django>=3.1',
- 'markdownify>=0.11.2',
- 'requests>=2.27.1,<3.0.0']
-
-extras_require = \
-{'aliyunsms': ['alibabacloud-dysmsapi20170525>=2.0.16'],
- 'channels': ['channels>=3.0.4']}
-
-setup_kwargs = {
-    'name': 'django-user-notification',
-    'version': '0.7.9',
-    'description': 'Django message notification package',
-    'long_description': '# Django user notification\n\n[![Build Status](https://img.shields.io/github/workflow/status/anyidea/django-user-notification/CI/master)](https://github.com/anyidea/django-user-notification/actions?query=workflow%3ACI)\n[![GitHub license](https://img.shields.io/github/license/anyidea/django-user-notification)](https://github.com/anyidea/django-user-notification/blob/master/LICENSE)\n[![Documentation Status](https://readthedocs.org/projects/django-user-notification/badge/?version=latest)](https://django-user-notification.readthedocs.io/en/latest/?badge=latest)\n[![pypi-version](https://img.shields.io/pypi/v/django-user-notification.svg)](https://pypi.python.org/pypi/django-user-notification)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-user-notification)\n[![PyPI - Django Version](https://img.shields.io/badge/django-%3E%3D3.1-44B78B)](https://www.djangoproject.com/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\nOverview\n-----\nDjango user notification is intended to provide a way to send multiple types of notification messages to django users out of box.\n\nDocumentation\n-----\non the way...\n\nRequirements\n-----\n\n* Python 3.8, 3.9, 3.10\n* Django 3.1, 3.2, 4.0, 4.1\n\nInstallation\n-----\n\nInstall using `pip`...\n\n    pip install django-user-notification\n\nAdd `\'django_quill\'` and `\'notification\'` to your `INSTALLED_APPS` setting.\n```python\nINSTALLED_APPS = [\n    \'django.contrib.admin\',\n    ...\n    \'django_quill\',\n    \'notification\',\n]\n```\n\nQuick Start\n-----\n\nLet\'s take a look at a quick start of using Django user notification to send notification messages to users.\n\nRun the `notification` migrations using:\n\n    python manage.py migrate notification\n\n\nAdd the following to your `settings.py` module:\n\n```python\nINSTALLED_APPS = [\n    ...  # Make sure to include the default installed apps here.\n    \'django_quill\',\n    \'notification\',\n]\n\nDJANGO_USER_NOTIFICATION = {\n    "aliyunsms": {\n        "access_key_id": "Your Access Key ID",\n        "access_key_secret": "Your Access Key Secret",\n        "sign_name": "Your Sign Name",\n    },\n    "dingtalkchatbot": {\n        "webhook": "Your Webhook URL",\n    },\n    "dingtalkworkmessage": {\n        "agent_id": "Your App Agent ID",\n        "app_key": "Your App Key",\n        "app_secret": "Your App Secret",\n    },\n    "dingtalktodotask": {\n        "app_key": "Your App Key",\n        "app_secret": "Your App Secret",\n    },\n}\n```\n\nLet\'s send a notification\n\n``` {.python}\nfrom django.contrib.auth import get_user_model\nfrom notification.backends import notify_by_email, notify_by_dingtalk_workmessage\n\nUser = get_user_model()\n\nrecipient = User.objects.first()\n\n# send a dingtalk work message notification\nnotify_by_dingtalk_workmessage([recipient], phone_field="phone", title="This is a title", message="A test message")\n\n\n# send a email notiofication\nnotify_by_email([recipient], title="This is a title", message="A test message")\n```\n\n\nSend Message With Template\n--------------\n\n`django-user-notification` support send notifications with custom template, To\nspecify a custom message template you can provide the `template_code`\nand `context` parameters.\n\n1)  Create a template message with code named `TMP01` on django admin\n\n2)  Provide the `template_code` and `context` to `send` method:\n``` {.python}\n...\n\nnotify_by_email([recipient], template_code="TMP01", context={"content": "Hello"})\n```\n\nSupported backends\n-----------------------------\n\n- `DummyNotificationBackend`: send dummy message\n- `EmailNotificationBackend`: send email notification.\n- `WebsocketNotificationBackend`: send webdocket notification, need install extension: `channels`.\n- `AliyunSMSNotificationBackend`: send aliyun sms notification, need install extension: `aliyunsms`.\n- `DingTalkChatbotNotificationBackend`: send dingtalk chatbot notification.\n- `DingTalkToDoTaskNotificationBackend`: send dingtalk todo tasks notification\n- `DingTalkWorkMessageNotificationBackend`: send dingtalk work message notification.\n- `WechatNotificationBackend`: planning...\n\nRunning the tests\n-----------------\n\nTo run the tests against the current environment:\n\n``` {.bash}\n$ pytest tests/\n```\n\nChangelog\n---------\n\n### 0.7.0\n\n-   Initial release\n\nContributing\n------------\nAs an open source project, we welcome contributions. The code lives on [GitHub](https://github.com/anyidea/django-user-notification/)\n\n## Thanks\n\n[![PyCharm](docs/pycharm.svg)](https://www.jetbrains.com/?from=django-user-notification)\n',
-    'author': 'Aiden Lu',
-    'author_email': 'allaher@icloud.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/aiden520/django-user-notification',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8',
-}
+User = get_user_model()
+
+recipient = User.objects.first()
+
+# send a dingtalk work message notification
+notify_by_dingtalk_workmessage([recipient], phone_field="phone", title="This is a title", message="A test message")
+
+
+# send a email notiofication
+notify_by_email([recipient], title="This is a title", message="A test message")
+```
+
+
+Send Message With Template
+--------------
+
+`django-user-notification` support send notifications with custom template, To
+specify a custom message template you can provide the `template_code`
+and `context` parameters.
+
+1)  Create a template message with code named `TMP01` on django admin
+
+2)  Provide the `template_code` and `context` to `send` method:
+``` {.python}
+...
+
+notify_by_email([recipient], template_code="TMP01", context={"content": "Hello"})
+```
+
+Supported backends
+-----------------------------
+
+- `DummyNotificationBackend`: send dummy message
+- `EmailNotificationBackend`: send email notification.
+- `WebsocketNotificationBackend`: send webdocket notification, need install extension: `channels`.
+- `AliyunSMSNotificationBackend`: send aliyun sms notification, need install extension: `aliyunsms`.
+- `DingTalkChatbotNotificationBackend`: send dingtalk chatbot notification.
+- `DingTalkToDoTaskNotificationBackend`: send dingtalk todo tasks notification
+- `DingTalkWorkMessageNotificationBackend`: send dingtalk work message notification.
+- `WechatNotificationBackend`: planning...
+
+Running the tests
+-----------------
+
+To run the tests against the current environment:
+
+``` {.bash}
+$ pytest tests/
+```
+
+Changelog
+---------
+
+### 0.7.0
+
+-   Initial release
+
+Contributing
+------------
+As an open source project, we welcome contributions. The code lives on [GitHub](https://github.com/anyidea/django-user-notification/)
+
+## Thanks
 
+[![PyCharm](docs/pycharm.svg)](https://www.jetbrains.com/?from=django-user-notification)
 
-setup(**setup_kwargs)
```

