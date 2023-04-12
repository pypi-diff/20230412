# Comparing `tmp/ravendev-0.0.53.tar.gz` & `tmp/ravendev-0.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ravendev-0.0.53.tar", max compression
+gzip compressed data, was "ravendev-0.0.54.tar", max compression
```

## Comparing `ravendev-0.0.53.tar` & `ravendev-0.0.54.tar`

### file list

```diff
@@ -1,59 +1,58 @@
--rw-r--r--   0        0        0      411 2023-04-03 16:12:26.003949 ravendev-0.0.53/pyproject.toml
--rw-r--r--   0        0        0     1615 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/__init__.py
--rw-r--r--   0        0        0     1587 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/__init__.py
--rw-r--r--   0        0        0     6607 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/client.py
--rw-r--r--   0        0        0      348 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/core/__init__.py
--rw-r--r--   0        0        0      326 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/core/datetime_utils.py
--rw-r--r--   0        0        0     3507 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      153 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/errors/__init__.py
--rw-r--r--   0        0        0      318 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/errors/event_not_found_error.py
--rw-r--r--   0        0        0      634 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/__init__.py
--rw-r--r--   0        0        0      135 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/device/__init__.py
--rw-r--r--   0        0        0     7421 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/device/client.py
--rw-r--r--   0        0        0      157 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/device/types/__init__.py
--rw-r--r--   0        0        0     1516 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/device/types/device.py
--rw-r--r--   0        0        0      587 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/device/types/platform.py
--rw-r--r--   0        0        0      175 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/ids/__init__.py
--rw-r--r--   0        0        0      241 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/ids/types/__init__.py
--rw-r--r--   0        0        0       77 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/ids/types/app_id.py
--rw-r--r--   0        0        0       80 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/ids/types/device_id.py
--rw-r--r--   0        0        0       81 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/ids/types/request_id.py
--rw-r--r--   0        0        0       78 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/ids/types/user_id.py
--rw-r--r--   0        0        0      387 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/user/__init__.py
--rw-r--r--   0        0        0     4453 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/user/client.py
--rw-r--r--   0        0        0      526 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/user/types/__init__.py
--rw-r--r--   0        0        0     1385 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/user/types/channel.py
--rw-r--r--   0        0        0      758 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/user/types/channel_preference.py
--rw-r--r--   0        0        0     1112 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/user/types/channel_preferences.py
--rw-r--r--   0        0        0     1720 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/user/types/raven_user.py
--rw-r--r--   0        0        0      825 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/user/types/slack_profile.py
--rw-r--r--   0        0        0      754 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/user/types/telegram_profile.py
--rw-r--r--   0        0        0      927 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/resources/user/types/user_preferences.py
--rw-r--r--   0        0        0     1456 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/types/__init__.py
--rw-r--r--   0        0        0      779 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/types/attachment.py
--rw-r--r--   0        0        0     1052 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/types/batch_event.py
--rw-r--r--   0        0        0      756 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/types/channel_override.py
--rw-r--r--   0        0        0      782 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/types/email_message.py
--rw-r--r--   0        0        0     1138 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/types/email_override.py
--rw-r--r--   0        0        0      765 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/types/email_recipient.py
--rw-r--r--   0        0        0      775 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/types/event_not_found_error_body.py
--rw-r--r--   0        0        0     1609 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/types/event_override.py
--rw-r--r--   0        0        0      758 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/types/in_app_override.py
--rw-r--r--   0        0        0      754 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/types/param.py
--rw-r--r--   0        0        0      944 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/types/provider_override.py
--rw-r--r--   0        0        0      757 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/types/push_override.py
--rw-r--r--   0        0        0      828 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/types/send_event_response.py
--rw-r--r--   0        0        0      769 2023-04-03 16:12:26.003949 ravendev-0.0.53/src/raven/api/types/slack_message.py
--rw-r--r--   0        0        0      825 2023-04-03 16:12:26.007949 ravendev-0.0.53/src/raven/api/types/slack_override.py
--rw-r--r--   0        0        0      744 2023-04-03 16:12:26.007949 ravendev-0.0.53/src/raven/api/types/sms_message.py
--rw-r--r--   0        0        0      833 2023-04-03 16:12:26.007949 ravendev-0.0.53/src/raven/api/types/sms_override.py
--rw-r--r--   0        0        0      761 2023-04-03 16:12:26.007949 ravendev-0.0.53/src/raven/api/types/telegram_override.py
--rw-r--r--   0        0        0     2145 2023-04-03 16:12:26.007949 ravendev-0.0.53/src/raven/api/types/user.py
--rw-r--r--   0        0        0      758 2023-04-03 16:12:26.007949 ravendev-0.0.53/src/raven/api/types/voice_override.py
--rw-r--r--   0        0        0      760 2023-04-03 16:12:26.007949 ravendev-0.0.53/src/raven/api/types/webhook_override.py
--rw-r--r--   0        0        0      822 2023-04-03 16:12:26.007949 ravendev-0.0.53/src/raven/api/types/whatsapp_override.py
--rw-r--r--   0        0        0      155 2023-04-03 16:12:26.007949 ravendev-0.0.53/src/raven/environment.py
--rw-r--r--   0        0        0        0 2023-04-03 16:12:26.007949 ravendev-0.0.53/src/raven/py.typed
--rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 ravendev-0.0.53/PKG-INFO
+-rw-r--r--   0        0        0      411 2023-04-12 21:35:13.412618 ravendev-0.0.54/pyproject.toml
+-rw-r--r--   0        0        0     1659 2023-04-12 21:35:13.412618 ravendev-0.0.54/src/raven/__init__.py
+-rw-r--r--   0        0        0     6606 2023-04-12 21:35:13.412618 ravendev-0.0.54/src/raven/client.py
+-rw-r--r--   0        0        0      348 2023-04-12 21:35:13.412618 ravendev-0.0.54/src/raven/core/__init__.py
+-rw-r--r--   0        0        0      326 2023-04-12 21:35:13.412618 ravendev-0.0.54/src/raven/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-04-12 21:35:13.412618 ravendev-0.0.54/src/raven/core/datetime_utils.py
+-rw-r--r--   0        0        0     3507 2023-04-12 21:35:13.412618 ravendev-0.0.54/src/raven/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-04-12 21:35:13.412618 ravendev-0.0.54/src/raven/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      155 2023-04-12 21:35:13.412618 ravendev-0.0.54/src/raven/environment.py
+-rw-r--r--   0        0        0      153 2023-04-12 21:35:13.412618 ravendev-0.0.54/src/raven/errors/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-12 21:35:13.412618 ravendev-0.0.54/src/raven/errors/event_not_found_error.py
+-rw-r--r--   0        0        0        0 2023-04-12 21:35:13.412618 ravendev-0.0.54/src/raven/py.typed
+-rw-r--r--   0        0        0      634 2023-04-12 21:35:13.412618 ravendev-0.0.54/src/raven/resources/__init__.py
+-rw-r--r--   0        0        0      135 2023-04-12 21:35:13.412618 ravendev-0.0.54/src/raven/resources/device/__init__.py
+-rw-r--r--   0        0        0     7420 2023-04-12 21:35:13.412618 ravendev-0.0.54/src/raven/resources/device/client.py
+-rw-r--r--   0        0        0      157 2023-04-12 21:35:13.412618 ravendev-0.0.54/src/raven/resources/device/types/__init__.py
+-rw-r--r--   0        0        0     1516 2023-04-12 21:35:13.412618 ravendev-0.0.54/src/raven/resources/device/types/device.py
+-rw-r--r--   0        0        0      587 2023-04-12 21:35:13.412618 ravendev-0.0.54/src/raven/resources/device/types/platform.py
+-rw-r--r--   0        0        0      175 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/resources/ids/__init__.py
+-rw-r--r--   0        0        0      241 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/resources/ids/types/__init__.py
+-rw-r--r--   0        0        0       77 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/resources/ids/types/app_id.py
+-rw-r--r--   0        0        0       80 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/resources/ids/types/device_id.py
+-rw-r--r--   0        0        0       81 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/resources/ids/types/request_id.py
+-rw-r--r--   0        0        0       78 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/resources/ids/types/user_id.py
+-rw-r--r--   0        0        0      387 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/resources/user/__init__.py
+-rw-r--r--   0        0        0     4452 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/resources/user/client.py
+-rw-r--r--   0        0        0      526 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/resources/user/types/__init__.py
+-rw-r--r--   0        0        0     1385 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/resources/user/types/channel.py
+-rw-r--r--   0        0        0      758 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/resources/user/types/channel_preference.py
+-rw-r--r--   0        0        0     1112 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/resources/user/types/channel_preferences.py
+-rw-r--r--   0        0        0     1720 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/resources/user/types/raven_user.py
+-rw-r--r--   0        0        0      825 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/resources/user/types/slack_profile.py
+-rw-r--r--   0        0        0      754 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/resources/user/types/telegram_profile.py
+-rw-r--r--   0        0        0      927 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/resources/user/types/user_preferences.py
+-rw-r--r--   0        0        0     1456 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/__init__.py
+-rw-r--r--   0        0        0      779 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/attachment.py
+-rw-r--r--   0        0        0     1052 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/batch_event.py
+-rw-r--r--   0        0        0      756 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/channel_override.py
+-rw-r--r--   0        0        0      782 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/email_message.py
+-rw-r--r--   0        0        0     1138 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/email_override.py
+-rw-r--r--   0        0        0      765 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/email_recipient.py
+-rw-r--r--   0        0        0      775 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/event_not_found_error_body.py
+-rw-r--r--   0        0        0     1609 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/event_override.py
+-rw-r--r--   0        0        0      758 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/in_app_override.py
+-rw-r--r--   0        0        0      754 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/param.py
+-rw-r--r--   0        0        0      944 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/provider_override.py
+-rw-r--r--   0        0        0      757 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/push_override.py
+-rw-r--r--   0        0        0      828 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/send_event_response.py
+-rw-r--r--   0        0        0      769 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/slack_message.py
+-rw-r--r--   0        0        0      825 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/slack_override.py
+-rw-r--r--   0        0        0      744 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/sms_message.py
+-rw-r--r--   0        0        0      833 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/sms_override.py
+-rw-r--r--   0        0        0      761 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/telegram_override.py
+-rw-r--r--   0        0        0     2145 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/user.py
+-rw-r--r--   0        0        0      758 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/voice_override.py
+-rw-r--r--   0        0        0      760 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/webhook_override.py
+-rw-r--r--   0        0        0      822 2023-04-12 21:35:13.416618 ravendev-0.0.54/src/raven/types/whatsapp_override.py
+-rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 ravendev-0.0.54/PKG-INFO
```

### Comparing `ravendev-0.0.53/src/raven/__init__.py` & `ravendev-0.0.54/src/raven/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from .api import (
+from .environment import RavenApiEnvironment
+from .errors import EventNotFoundError
+from .resources import (
     AppId,
-    Attachment,
-    BatchEvent,
     Channel,
-    ChannelOverride,
     ChannelPreference,
     ChannelPreferences,
     Device,
     DeviceId,
+    Platform,
+    RavenUser,
+    RequestId,
+    SlackProfile,
+    TelegramProfile,
+    UserId,
+    UserPreferences,
+    device,
+    ids,
+    user,
+)
+from .types import (
+    Attachment,
+    BatchEvent,
+    ChannelOverride,
     EmailMessage,
     EmailOverride,
     EmailRecipient,
-    EventNotFoundError,
     EventNotFoundErrorBody,
     EventOverride,
     InAppOverride,
     Param,
-    Platform,
     ProviderOverride,
     PushOverride,
-    RavenUser,
-    RequestId,
     SendEventResponse,
     SlackMessage,
     SlackOverride,
-    SlackProfile,
     SmsMessage,
     SmsOverride,
     TelegramOverride,
-    TelegramProfile,
     User,
-    UserId,
-    UserPreferences,
     VoiceOverride,
     WebhookOverride,
     WhatsappOverride,
-    device,
-    ids,
-    user,
 )
-from .environment import RavenApiEnvironment
 
 __all__ = [
     "AppId",
     "Attachment",
     "BatchEvent",
     "Channel",
     "ChannelOverride",
```

### Comparing `ravendev-0.0.53/src/raven/api/client.py` & `ravendev-0.0.54/src/raven/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 from backports.cached_property import cached_property
 
-from ..environment import RavenApiEnvironment
 from .core.api_error import ApiError
 from .core.jsonable_encoder import jsonable_encoder
 from .core.remove_none_from_headers import remove_none_from_headers
+from .environment import RavenApiEnvironment
 from .errors.event_not_found_error import EventNotFoundError
 from .resources.device.client import AsyncDeviceClient, DeviceClient
 from .resources.ids.types.app_id import AppId
 from .resources.user.client import AsyncUserClient, UserClient
 from .types.batch_event import BatchEvent
 from .types.event_not_found_error_body import EventNotFoundErrorBody
 from .types.event_override import EventOverride
```

### Comparing `ravendev-0.0.53/src/raven/api/core/datetime_utils.py` & `ravendev-0.0.54/src/raven/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/core/jsonable_encoder.py` & `ravendev-0.0.54/src/raven/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/resources/__init__.py` & `ravendev-0.0.54/src/raven/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/resources/device/client.py` & `ravendev-0.0.54/src/raven/resources/device/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
-from ....environment import RavenApiEnvironment
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import RavenApiEnvironment
 from ..ids.types.app_id import AppId
 from ..ids.types.device_id import DeviceId
 from ..ids.types.user_id import UserId
 from .types.device import Device
 
 
 class DeviceClient:
```

### Comparing `ravendev-0.0.53/src/raven/api/resources/device/types/device.py` & `ravendev-0.0.54/src/raven/resources/device/types/device.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/resources/device/types/platform.py` & `ravendev-0.0.54/src/raven/resources/device/types/platform.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/resources/user/client.py` & `ravendev-0.0.54/src/raven/resources/user/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
-from ....environment import RavenApiEnvironment
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import RavenApiEnvironment
 from ..ids.types.app_id import AppId
 from ..ids.types.user_id import UserId
 from .types.raven_user import RavenUser
 
 
 class UserClient:
     def __init__(self, *, environment: RavenApiEnvironment = RavenApiEnvironment.PROD, auth_key: str):
```

### Comparing `ravendev-0.0.53/src/raven/api/resources/user/types/__init__.py` & `ravendev-0.0.54/src/raven/resources/user/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/resources/user/types/channel.py` & `ravendev-0.0.54/src/raven/resources/user/types/channel.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/resources/user/types/channel_preference.py` & `ravendev-0.0.54/src/raven/resources/user/types/channel_preference.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/resources/user/types/channel_preferences.py` & `ravendev-0.0.54/src/raven/resources/user/types/channel_preferences.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/resources/user/types/raven_user.py` & `ravendev-0.0.54/src/raven/resources/user/types/raven_user.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/resources/user/types/slack_profile.py` & `ravendev-0.0.54/src/raven/resources/user/types/slack_profile.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/resources/user/types/telegram_profile.py` & `ravendev-0.0.54/src/raven/resources/user/types/telegram_profile.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/resources/user/types/user_preferences.py` & `ravendev-0.0.54/src/raven/resources/user/types/user_preferences.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/__init__.py` & `ravendev-0.0.54/src/raven/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/attachment.py` & `ravendev-0.0.54/src/raven/types/attachment.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/batch_event.py` & `ravendev-0.0.54/src/raven/types/batch_event.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/channel_override.py` & `ravendev-0.0.54/src/raven/types/channel_override.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/email_message.py` & `ravendev-0.0.54/src/raven/types/email_message.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/email_override.py` & `ravendev-0.0.54/src/raven/types/email_override.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/email_recipient.py` & `ravendev-0.0.54/src/raven/types/email_recipient.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/event_not_found_error_body.py` & `ravendev-0.0.54/src/raven/types/event_not_found_error_body.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/event_override.py` & `ravendev-0.0.54/src/raven/types/event_override.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/in_app_override.py` & `ravendev-0.0.54/src/raven/types/in_app_override.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/param.py` & `ravendev-0.0.54/src/raven/types/param.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/provider_override.py` & `ravendev-0.0.54/src/raven/types/provider_override.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/push_override.py` & `ravendev-0.0.54/src/raven/types/push_override.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/send_event_response.py` & `ravendev-0.0.54/src/raven/types/send_event_response.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/slack_message.py` & `ravendev-0.0.54/src/raven/types/slack_message.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/slack_override.py` & `ravendev-0.0.54/src/raven/types/slack_override.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/sms_message.py` & `ravendev-0.0.54/src/raven/types/sms_message.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/sms_override.py` & `ravendev-0.0.54/src/raven/types/sms_override.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/telegram_override.py` & `ravendev-0.0.54/src/raven/types/telegram_override.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/user.py` & `ravendev-0.0.54/src/raven/types/user.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/voice_override.py` & `ravendev-0.0.54/src/raven/types/voice_override.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/webhook_override.py` & `ravendev-0.0.54/src/raven/types/webhook_override.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/src/raven/api/types/whatsapp_override.py` & `ravendev-0.0.54/src/raven/types/whatsapp_override.py`

 * *Files identical despite different names*

### Comparing `ravendev-0.0.53/PKG-INFO` & `ravendev-0.0.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ravendev
-Version: 0.0.53
+Version: 0.0.54
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

