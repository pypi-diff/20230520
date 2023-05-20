# Comparing `tmp/lokiunimore-0.6.1.tar.gz` & `tmp/lokiunimore-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lokiunimore-0.6.1.tar", max compression
+gzip compressed data, was "lokiunimore-0.7.0.tar", max compression
```

## Comparing `lokiunimore-0.6.1.tar` & `lokiunimore-0.7.0.tar`

### file list

```diff
@@ -1,45 +1,44 @@
--rw-r--r--   0        0        0    34523 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/LICENSE.txt
--rw-r--r--   0        0        0     3434 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/README.md
--rw-r--r--   0        0        0       22 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/config/__init__.py
--rw-r--r--   0        0        0       41 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/config/__main__.py
--rw-r--r--   0        0        0     6187 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/config/config.py
--rw-r--r--   0        0        0       22 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/matrix/__init__.py
--rw-r--r--   0        0        0      735 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/matrix/__main__.py
--rw-r--r--   0        0        0    22084 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/matrix/client.py
--rw-r--r--   0        0        0     3066 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/matrix/templates/messages.py
--rw-r--r--   0        0        0       22 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/sql/__init__.py
--rw-r--r--   0        0        0      260 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/sql/__main__.py
--rw-r--r--   0        0        0     2431 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/sql/tables.py
--rw-r--r--   0        0        0      348 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/utils/device_names.py
--rw-r--r--   0        0        0      888 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/utils/logs.py
--rw-r--r--   0        0        0       19 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/__init__.py
--rw-r--r--   0        0        0      236 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/__main__.py
--rw-r--r--   0        0        0     5476 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/app.py
--rw-r--r--   0        0        0     1897 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/extensions/matrix_client.py
--rw-r--r--   0        0        0    67646 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/static/favicon.ico
--rw-r--r--   0        0        0     8288 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/static/icon.png
--rw-r--r--   0        0        0     9408 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/static/newcode.png
--rw-r--r--   0        0        0   151500 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/static/opengraph.png
--rw-r--r--   0        0        0    13849 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/static/rooms.png
--rw-r--r--   0        0        0    11414 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/static/s-192.png
--rw-r--r--   0        0        0    12609 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/static/spaces.png
--rw-r--r--   0        0        0     9703 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/static/thor.png
--rw-r--r--   0        0        0     2380 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/static/unimore.css
--rw-r--r--   0        0        0    15136 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/static/verify.png
--rw-r--r--   0        0        0     1941 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/templates/_base.html
--rw-r--r--   0        0        0      593 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/templates/errors/_base.html
--rw-r--r--   0        0        0      521 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/templates/errors/failed-invite.html
--rw-r--r--   0        0        0      470 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/templates/errors/no-link.html
--rw-r--r--   0        0        0      330 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/templates/errors/not-found.html
--rw-r--r--   0        0        0      645 2023-05-16 23:04:18.254748 lokiunimore-0.6.1/lokiunimore/web/templates/errors/not-student.html
--rw-r--r--   0        0        0      599 2023-05-16 23:04:18.258748 lokiunimore-0.6.1/lokiunimore/web/templates/errors/not-verified.html
--rw-r--r--   0        0        0      300 2023-05-16 23:04:18.258748 lokiunimore-0.6.1/lokiunimore/web/templates/errors/oidc.html
--rw-r--r--   0        0        0      418 2023-05-16 23:04:18.258748 lokiunimore-0.6.1/lokiunimore/web/templates/errors/rate-invite.html
--rw-r--r--   0        0        0     2125 2023-05-16 23:04:18.258748 lokiunimore-0.6.1/lokiunimore/web/templates/matrix/complete.html
--rw-r--r--   0        0        0     2481 2023-05-16 23:04:18.258748 lokiunimore-0.6.1/lokiunimore/web/templates/matrix/join.html
--rw-r--r--   0        0        0     1764 2023-05-16 23:04:18.258748 lokiunimore-0.6.1/lokiunimore/web/templates/matrix/verify.html
--rw-r--r--   0        0        0     5933 2023-05-16 23:04:18.258748 lokiunimore-0.6.1/lokiunimore/web/templates/privacy.html
--rw-r--r--   0        0        0     5336 2023-05-16 23:04:18.258748 lokiunimore-0.6.1/lokiunimore/web/templates/root.html
--rw-r--r--   0        0        0     4703 2023-05-16 23:04:18.258748 lokiunimore-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     4923 1970-01-01 00:00:00.000000 lokiunimore-0.6.1/setup.py
--rw-r--r--   0        0        0     4695 1970-01-01 00:00:00.000000 lokiunimore-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2022-09-12 07:14:39.309540 lokiunimore-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     3234 2023-05-20 17:24:22.739375 lokiunimore-0.7.0/README.md
+-rw-r--r--   0        0        0       22 2022-09-09 23:37:05.679098 lokiunimore-0.7.0/lokiunimore/config/__init__.py
+-rw-r--r--   0        0        0       41 2022-09-11 01:13:26.488730 lokiunimore-0.7.0/lokiunimore/config/__main__.py
+-rw-r--r--   0        0        0     6187 2022-09-16 12:02:50.924023 lokiunimore-0.7.0/lokiunimore/config/config.py
+-rw-r--r--   0        0        0       22 2022-09-12 07:14:39.419540 lokiunimore-0.7.0/lokiunimore/matrix/__init__.py
+-rw-r--r--   0        0        0      758 2023-05-20 16:25:25.326851 lokiunimore-0.7.0/lokiunimore/matrix/__main__.py
+-rw-r--r--   0        0        0    21685 2023-05-20 16:52:12.169800 lokiunimore-0.7.0/lokiunimore/matrix/client.py
+-rw-r--r--   0        0        0     3083 2023-05-20 17:15:57.638520 lokiunimore-0.7.0/lokiunimore/matrix/templates/messages.py
+-rw-r--r--   0        0        0       22 2022-09-09 23:45:02.955105 lokiunimore-0.7.0/lokiunimore/sql/__init__.py
+-rw-r--r--   0        0        0      260 2022-09-14 02:12:05.840975 lokiunimore-0.7.0/lokiunimore/sql/__main__.py
+-rw-r--r--   0        0        0     4905 2023-05-20 16:07:43.524933 lokiunimore-0.7.0/lokiunimore/sql/tables.py
+-rw-r--r--   0        0        0      348 2022-09-11 02:48:06.533186 lokiunimore-0.7.0/lokiunimore/utils/device_names.py
+-rw-r--r--   0        0        0      888 2022-09-12 07:14:39.521540 lokiunimore-0.7.0/lokiunimore/utils/logs.py
+-rw-r--r--   0        0        0       19 2022-09-12 07:14:39.708540 lokiunimore-0.7.0/lokiunimore/web/__init__.py
+-rw-r--r--   0        0        0      236 2022-09-16 12:02:50.925022 lokiunimore-0.7.0/lokiunimore/web/__main__.py
+-rw-r--r--   0        0        0     5511 2023-05-20 15:09:54.328778 lokiunimore-0.7.0/lokiunimore/web/app.py
+-rw-r--r--   0        0        0     1907 2023-05-20 14:09:26.998276 lokiunimore-0.7.0/lokiunimore/web/extensions/matrix_client.py
+-rw-r--r--   0        0        0    67646 2022-09-12 07:40:28.587432 lokiunimore-0.7.0/lokiunimore/web/static/favicon.ico
+-rw-r--r--   0        0        0     8288 2022-09-12 07:40:19.534432 lokiunimore-0.7.0/lokiunimore/web/static/icon.png
+-rw-r--r--   0        0        0     9408 2022-12-22 19:17:21.649603 lokiunimore-0.7.0/lokiunimore/web/static/newcode.png
+-rw-r--r--   0        0        0   151500 2022-09-14 02:23:19.041943 lokiunimore-0.7.0/lokiunimore/web/static/opengraph.png
+-rw-r--r--   0        0        0    13849 2022-12-22 17:36:27.101505 lokiunimore-0.7.0/lokiunimore/web/static/rooms.png
+-rw-r--r--   0        0        0    11414 2022-12-22 19:29:55.750615 lokiunimore-0.7.0/lokiunimore/web/static/s-192.png
+-rw-r--r--   0        0        0    12609 2022-12-22 17:35:11.929504 lokiunimore-0.7.0/lokiunimore/web/static/spaces.png
+-rw-r--r--   0        0        0     9703 2022-12-22 18:25:58.877553 lokiunimore-0.7.0/lokiunimore/web/static/thor.png
+-rw-r--r--   0        0        0     2380 2022-12-22 19:27:04.461613 lokiunimore-0.7.0/lokiunimore/web/static/unimore.css
+-rw-r--r--   0        0        0    15136 2022-12-22 17:54:43.661523 lokiunimore-0.7.0/lokiunimore/web/static/verify.png
+-rw-r--r--   0        0        0     1941 2022-12-22 19:27:29.637613 lokiunimore-0.7.0/lokiunimore/web/templates/_base.html
+-rw-r--r--   0        0        0      593 2022-09-12 08:32:11.762215 lokiunimore-0.7.0/lokiunimore/web/templates/errors/_base.html
+-rw-r--r--   0        0        0      521 2022-12-22 19:33:02.285618 lokiunimore-0.7.0/lokiunimore/web/templates/errors/failed-invite.html
+-rw-r--r--   0        0        0      470 2022-12-22 19:33:15.098619 lokiunimore-0.7.0/lokiunimore/web/templates/errors/no-link.html
+-rw-r--r--   0        0        0      330 2022-09-12 08:33:58.481208 lokiunimore-0.7.0/lokiunimore/web/templates/errors/not-found.html
+-rw-r--r--   0        0        0      645 2022-09-12 08:32:21.533214 lokiunimore-0.7.0/lokiunimore/web/templates/errors/not-student.html
+-rw-r--r--   0        0        0      599 2022-09-12 08:32:25.528214 lokiunimore-0.7.0/lokiunimore/web/templates/errors/not-verified.html
+-rw-r--r--   0        0        0      300 2022-09-12 08:32:29.441214 lokiunimore-0.7.0/lokiunimore/web/templates/errors/oidc.html
+-rw-r--r--   0        0        0      418 2022-12-22 19:34:20.990620 lokiunimore-0.7.0/lokiunimore/web/templates/errors/rate-invite.html
+-rw-r--r--   0        0        0     2125 2022-12-22 19:34:44.869620 lokiunimore-0.7.0/lokiunimore/web/templates/matrix/complete.html
+-rw-r--r--   0        0        0     2481 2022-12-22 19:34:59.842620 lokiunimore-0.7.0/lokiunimore/web/templates/matrix/join.html
+-rw-r--r--   0        0        0     1764 2022-12-22 19:35:47.109621 lokiunimore-0.7.0/lokiunimore/web/templates/matrix/verify.html
+-rw-r--r--   0        0        0     5933 2022-12-25 04:58:24.750659 lokiunimore-0.7.0/lokiunimore/web/templates/privacy.html
+-rw-r--r--   0        0        0     5336 2022-12-22 19:19:19.669605 lokiunimore-0.7.0/lokiunimore/web/templates/root.html
+-rw-r--r--   0        0        0     4702 2023-05-20 16:57:00.499419 lokiunimore-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4493 1970-01-01 00:00:00.000000 lokiunimore-0.7.0/PKG-INFO
```

### Comparing `lokiunimore-0.6.1/LICENSE.txt` & `lokiunimore-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/README.md` & `lokiunimore-0.7.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Loki Bot
 
-Gatekeeper bot for the Unimore Informatica unofficial Matrix space
+Gatekeeper bot for the Unimore Informatica unofficial Matrix space.
+
+## Links
+
+
 
 \[ [**Website**](https://loki.steffo.eu) | [PyPI](https://pypi.org/project/lokiunimore/) \]
 
 > TIP: You may be looking for its predecessor, [Thor Bot](https://github.com/Steffo99/thorunimore).
 
 ![](lokiunimore/web/static/opengraph.png)
 
@@ -72,13 +76,7 @@
 Use the [pre-built Docker image](https://github.com/Steffo99/lokiunimore/pkgs/container/lokiunimore), or build it from the [provided Dockerfile](Dockerfile).
 
 Run the image without any command to view and validate the current configuration.
 
 Run the image with the `gunicorn -b 0.0.0.0:80 lokiunimore.web.app:rp_app` command to launch the production web server on local port 80, expecting to be behind a  reverse proxy.
 
 Run the image with the `lokiunimore.matrix` command to launch the Matrix bot.
-
-### Using Docker Compose
-
-Use the [given Docker Compose file](docker-compose.yml).
-
-Either use [Portainer](https://www.portainer.io/), or start it manually using `docker compose up -d && docker compose logs -f`.
```

### Comparing `lokiunimore-0.6.1/lokiunimore/config/config.py` & `lokiunimore-0.7.0/lokiunimore/config/config.py`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/matrix/__main__.py` & `lokiunimore-0.7.0/lokiunimore/matrix/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     user=MATRIX_USER_ID.__wrapped__,
     database_url=SQLALCHEMY_DATABASE_URL.__wrapped__
 )
 
 
 async def main():
     await client.login_with_shared_secret(MATRIX_USER_SECRET.__wrapped__)
-    await client.sync_forever(60_000, full_state=True)
+    await client.sync_forever(60_000, full_state=True, set_presence="online")
 
 
 async def cleanup():
     await client.logout()
 
 
 try:
```

### Comparing `lokiunimore-0.6.1/lokiunimore/matrix/client.py` & `lokiunimore-0.7.0/lokiunimore/matrix/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import logging
 import hashlib
 import hmac
 import typing as t
 import functools
 import sqlalchemy
 import sqlalchemy.orm
-import flask
 
 T = t.TypeVar("T")
 log = logging.getLogger(__name__)
 
 from lokiunimore.sql.tables import MatrixUser, MatrixProcessedEvent
 from lokiunimore.utils.device_names import generate_device_name
 from lokiunimore.config import MATRIX_PUBLIC_SPACE_ID, MATRIX_PRIVATE_SPACE_ID, MATRIX_SKIP_EVENTS
@@ -141,15 +140,15 @@
         """
 
         log.debug(f"Logging in as {self.user} with a shared secret...")
 
         token = hmac.new(key=shared_secret.encode("utf8"), msg=self.user.encode("utf8"), digestmod=hashlib.sha512).hexdigest()
 
         await self.login_raw({
-            "type": "x.shared_secret_auth",
+            "type": "com.devture.shared_secret_auth",
             "identifier": {
                 "type": "m.id.user",
                 "user": self.user,
             },
             "token": token,
             "initial_device_display_name": generate_device_name(__name__),
         })
@@ -195,41 +194,43 @@
             if not current:
                 break
 
         log.debug(f"Successfully retrieved a hierarchy of {len(rooms)} rooms!")
 
         return rooms
 
-    async def find_or_create_pm_room(self, user_id: str) -> str:
+    async def put_management_room(self, user_id: str) -> str:
         """
-        Find the first available private message room with the given user, or create one if none exist.
+        Find the first available management room with the given user, or create one if none exist.
 
         :param user_id: The user to message.
         :returns: The room id of the created room.
         """
 
-        log.debug(f"Sliding into {user_id}'s PMs...")
+        log.debug(f"Creating a management room for %s", user_id)
 
         for room in self.rooms.values():
             is_dm = "m.direct" in room.tags
             is_group = room.is_group
             has_two_users = len(room.users) + len(room.invited_users) == 2
             contains_user_id = user_id in room.users.keys() or user_id in room.invited_users.keys()
 
             if (is_dm or is_group) and has_two_users and contains_user_id:
-                log.debug(f"Found PM room for: {user_id}")
+                log.debug(f"Found existing management room %s for %s", room.room_id, user_id)
                 return room.room_id
+
         else:
-            log.debug(f"Creating new PM room for: {user_id}")
+            log.debug(f"Creating new management room for %s", user_id)
             response = await self.room_create(invite=[user_id], is_direct=True)
-            if isinstance(response, nio.RoomCreateResponse):
-                log.info(f"Created new PM room for: {user_id}")
-                return response.room_id
-            else:
-                raise Exception("Failed to slide into an user's PMs.")
+
+            if not isinstance(response, nio.RoomCreateResponse):
+                raise Exception("Failed to create a management room.")
+
+            log.info(f"Created new managememt room %s for %s", response.room_id, user_id)
+            return response.room_id
 
     async def room_send_message_html(self, room_id: str, text: str, html: str):
         """
         Send an HTML message with a text fallback.
 
         :param room_id: The ID of the room to send the message in.
         :param text: The plain text fallback of the message.
@@ -333,19 +334,14 @@
         with self._sqla_session() as session:
             session: sqlalchemy.orm.Session
             mpe: MatrixProcessedEvent = MatrixProcessedEvent(id=event.event_id)
             session.add(mpe)
             session.commit()
             return mpe
 
-    @staticmethod
-    def _loki_web_profile(token: str):
-        with app.app_context():
-            return flask.url_for("page_matrix_profile", token=token)
-
     @filter_processed_events
     async def __handle_membership_change(self, room: nio.MatrixRoom, event: nio.Event) -> None:
         # Filters allow us to determine the event type in a better way
         event: nio.InviteMemberEvent | nio.RoomMemberEvent
 
         if event.prev_membership == event.membership:
             # If the event is a name change, or something like that, don't do anything
@@ -385,56 +381,60 @@
         log.debug(f"Received invite to: {room.room_id}")
         await self.join(room.room_id)
         log.info(f"Accepted invite to: {room.room_id}")
 
     async def __handle_public_space_joiner(self, user_id: str):
         log.debug(f"User joined public space: {user_id}")
 
-        log.debug(f"Creating MatrixUser for: {user_id}")
         with self._sqla_session() as session:
             session: sqlalchemy.orm.Session
-            matrix_user = MatrixUser(id=user_id)
-            matrix_user = session.merge(matrix_user)
+            matrix_user: MatrixUser = MatrixUser.create(session=session, id=user_id)
             session.commit()
-            log.debug(f"Created MatrixUser for: {user_id}")
-            token = matrix_user.token
+
+            with app.app_context():
+                formatting = dict(
+                    username_text=self.user_id,
+                    username_html=await self.mention_html(self.user_id),
+                    profile_url=matrix_user.profile_url(),
+                )
 
         log.debug(f"Notifying user of the account creation: {user_id}")
-        formatting = dict(
-            username_text=self.user_id,
-            username_html=await self.mention_html(self.user_id),
-            profile_url=self._loki_web_profile(token),
-        )
         await self.room_send_message_html(
-            await self.find_or_create_pm_room(user_id),
+            await self.put_management_room(user_id),
             text=WELCOME_MESSAGE_TEXT.format(**formatting),
             html=WELCOME_MESSAGE_HTML.format(**formatting)
         )
         log.debug(f"Notified user of the account creation: {user_id}")
 
         log.info(f"Handled joiner of public space: {user_id}")
 
     async def __handle_private_space_joiner(self, user_id: str):
         log.info(f"User joined private space: {user_id}")
 
         log.debug(f"Setting MatrixUser as joined for: {user_id}")
         with self._sqla_session() as session:
             session: sqlalchemy.orm.Session
             matrix_user: MatrixUser = session.query(MatrixUser).get(user_id)
+            if matrix_user is None:
+                log.warning(f"User joined private space without having a pre-existent record in the db: {user_id}")
+                matrix_user = MatrixUser.create(session=session, id=user_id)
+                session.commit()
+
             matrix_user.joined_private_space = True
             session.commit()
             log.debug(f"Set MatrixUser as joined for: {user_id}")
-            token = matrix_user.token
+
+            with app.app_context():
+                formatting = dict(
+                    profile_url=matrix_user.profile_url(),
+                )
 
         log.debug(f"Notifying user of the account link: {user_id}")
-        formatting = dict(
-            profile_url=self._loki_web_profile(token),
-        )
         await self.room_send_message_html(
-            await self.find_or_create_pm_room(user_id),
+            await self.put_management_room(user_id),
             text=SUCCESS_MESSAGE_TEXT.format(**formatting),
             html=SUCCESS_MESSAGE_HTML.format(**formatting)
         )
         log.debug(f"Notified user of the account link: {user_id}")
 
         log.info(f"Handled joiner of private space: {user_id}")
 
@@ -444,23 +444,20 @@
         log.debug(f"Deleting MatrixUser for: {user_id}")
         with self._sqla_session() as session:
             session: sqlalchemy.orm.Session
             matrix_user: MatrixUser = session.query(MatrixUser).get(user_id)
             if matrix_user is None:
                 log.warning(f"User left public space without having a pre-existent record in the db: {user_id}")
             else:
-                if matrix_user.account is not None and len(matrix_user.account.matrix_users) == 1:
-                    session.delete(matrix_user.account)
-                session.delete(matrix_user)
+                matrix_user.destroy(session=session)
                 session.commit()
-                log.debug(f"Deleted MatrixUser for: {user_id}")
 
         log.debug(f"Notifying user of the account deletion: {user_id}")
         await self.room_send_message_html(
-            await self.find_or_create_pm_room(user_id),
+            await self.put_management_room(user_id),
             text=GOODBYE_MESSAGE_TEXT,
             html=GOODBYE_MESSAGE_HTML
         )
         log.debug(f"Notified user of the account deletion: {user_id}")
 
         log.debug(f"Finding room hierarchy of the public space...")
         public_hierarchy = await self.room_hierarchy(MATRIX_PUBLIC_SPACE_ID.__wrapped__, max_depth=9, suggested_only=False)
@@ -492,30 +489,26 @@
             session: sqlalchemy.orm.Session
             matrix_user: MatrixUser = session.query(MatrixUser).get(user_id)
             if matrix_user is None:
                 log.warning(f"User left private space without having a pre-existent record in the db: {user_id}")
                 return
             elif matrix_user.account is None:
                 log.warning(f"User left private space without having a linked account in the db: {user_id}")
-                token = matrix_user.token
             else:
-                if len(matrix_user.account.matrix_users) == 1:
-                    session.delete(matrix_user.account)
-                matrix_user.account = None
-                matrix_user.joined_private_space = False
+                matrix_user.unlink(session=session)
                 session.commit()
-                log.debug(f"Unlinked account for: {user_id}")
-                token = matrix_user.token
+
+            with app.app_context():
+                formatting = dict(
+                    profile_url=matrix_user.profile_url(),
+                )
 
         log.debug(f"Notifying user of the account unlinking: {user_id}")
-        formatting = dict(
-            profile_url=self._loki_web_profile(token),
-        )
         await self.room_send_message_html(
-            await self.find_or_create_pm_room(user_id),
+            await self.put_management_room(user_id),
             text=UNLINK_MESSAGE_TEXT.format(**formatting),
             html=UNLINK_MESSAGE_HTML.format(**formatting)
         )
         log.debug(f"Notified user of the account unlinking: {user_id}")
 
         log.debug(f"Finding room hierarchy of the private space...")
         hierarchy = await self.room_hierarchy(MATRIX_PRIVATE_SPACE_ID.__wrapped__, max_depth=9, suggested_only=False)
```

### Comparing `lokiunimore-0.6.1/lokiunimore/matrix/templates/messages.py` & `lokiunimore-0.7.0/lokiunimore/matrix/templates/messages.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,94 +1,94 @@
 # ==================================== #
 
 WELCOME_MESSAGE_TEXT = """
-Benvenuto allo spazio Matrix dell'Unimore!
+ℹ️ Benvenuto allo spazio Matrix dell'Unimore!
 
-Sono {username_text}, il bot buttafuori che verifica le credenziali degli utenti che entrano e permette loro di accedere alle rispettive aree.
+Sono {username_text}, il bot che verifica le credenziali degli utenti che entrano e permette loro di accedere alle rispettive aree.
 
 Se sei uno studente, puoi ottenere accesso all'Area Studenti verificando la tua identità:
 {profile_url}
 """
 
 # language=html
 WELCOME_MESSAGE_HTML = """
 <p>
-    Benvenuto allo spazio Matrix dell'Unimore!
+    ℹ️ Benvenuto allo spazio Matrix dell'Unimore!
 </p>
 <p>
     Sono {username_html}, il bot buttafuori che verifica le credenziali degli utenti che entrano e permette loro di accedere alle rispettive aree.
 </p>
 <p>
     Se sei uno studente, puoi ottenere accesso all'Area Studenti <a href="{profile_url}">verificando la tua identità</a>!
 </p>
 """
 
 # ==================================== #
 
 SUCCESS_MESSAGE_TEXT = """
-Ti sei unito all'Area Studenti: benvenuto!
+✅ Ti sei unito all'Area Studenti: benvenuto!
 
 Se in qualsiasi momento vuoi modificare o eliminare i tuoi dati salvati sul mio database, puoi accedervi dal tuo profilo privato:
 {profile_url}
 """
 
 # language=html
 SUCCESS_MESSAGE_HTML = """
 <p>
-    Ti sei unito all'Area Studenti: benvenuto!
+    ✅ Ti sei unito all'Area Studenti: benvenuto!
 </p>
 <p>
     Se in qualsiasi momento vuoi modificare o eliminare i tuoi dati salvati sul mio database, puoi <a href="{profile_url}">accedervi dal tuo profilo privato</a>!
 </p>
 """
 
 # ==================================== #
 
 GOODBYE_MESSAGE_TEXT = """
-Hai abbandonato lo spazio Matrix dell'Unimore, quindi ho cancellato i tuoi dati dal mio database; a breve verrai inoltre rimosso da tutte le stanze dello spazio.
+❎ Hai abbandonato lo spazio Matrix dell'Unimore, quindi ho cancellato i tuoi dati dal mio database; a breve verrai inoltre rimosso da tutte le stanze dello spazio.
 
 Se cambierai idea in futuro, potrai sempre rientrare allo stesso indirizzo!
 
-Abbi un buon proseguimento di giornata! :)
+Abbi un buon proseguimento di giornata!
 """
 
 # language=html
 GOODBYE_MESSAGE_HTML = """
 <p>
-    Hai abbandonato lo spazio Matrix dell'Unimore, quindi ho cancellato i tuoi dati dal mio database; a breve verrai inoltre rimosso da tutte le stanze dello spazio.
+    ❎ Hai abbandonato lo spazio Matrix dell'Unimore, quindi ho cancellato i tuoi dati dal mio database; a breve verrai inoltre rimosso da tutte le stanze dello spazio.
 </p>
 <p>
     Se cambierai idea in futuro, potrai sempre rientrare allo stesso indirizzo!
 </p>
 <p>
-    Abbi un buon proseguimento di giornata! :)
+    Abbi un buon proseguimento di giornata!
 </p>
 """
 
 # ==================================== #
 
 UNLINK_MESSAGE_TEXT = """
-Hai abbandonato l'Area Studenti dello spazio Unimore, quindi ho scollegato il tuo account Studenti@Unimore dal tuo account Matrix.
+📴 Hai abbandonato l'Area Studenti dello spazio Unimore, quindi ho scollegato il tuo account Studenti@Unimore dal tuo account Matrix.
 
 Se cambierai idea in futuro, potrai sempre essere riaggiunto all'Area Studenti ricollegando il tuo account:
 {profile_url}
 
-Abbi un buon proseguimento di giornata! :)
+Abbi un buon proseguimento di giornata!
 """
 
 # language=html
 UNLINK_MESSAGE_HTML = """
 <p>
-    Hai abbandonato l'Area Studenti dello spazio Unimore, quindi ho scollegato il tuo account Studenti@Unimore dal tuo account Matrix.
+    📴 Hai abbandonato l'Area Studenti dello spazio Unimore, quindi ho scollegato il tuo account Studenti@Unimore dal tuo account Matrix.
 </p>
 <p>
     Se cambierai idea in futuro, potrai sempre essere riaggiunto all'Area Studenti <a href="{profile_url}">ricollegando il tuo account</a>!
 </p>
 <p>
-    Abbi un buon proseguimento di giornata! :)
+    Abbi un buon proseguimento di giornata!
 </p>
 """
 
 # ==================================== #
 
 __all__ = (
     "WELCOME_MESSAGE_TEXT",
```

#### html2text {}

```diff
@@ -1,44 +1,44 @@
-# ==================================== # WELCOME_MESSAGE_TEXT = """ Benvenuto
-allo spazio Matrix dell'Unimore! Sono {username_text}, il bot buttafuori che
+# ==================================== # WELCOME_MESSAGE_TEXT = """ â¹ï¸
+Benvenuto allo spazio Matrix dell'Unimore! Sono {username_text}, il bot che
 verifica le credenziali degli utenti che entrano e permette loro di accedere
 alle rispettive aree. Se sei uno studente, puoi ottenere accesso all'Area
 Studenti verificando la tua identitÃ : {profile_url} """ # language=html
 WELCOME_MESSAGE_HTML = """
-Benvenuto allo spazio Matrix dell'Unimore!
+â¹ï¸ Benvenuto allo spazio Matrix dell'Unimore!
 Sono {username_html}, il bot buttafuori che verifica le credenziali degli
 utenti che entrano e permette loro di accedere alle rispettive aree.
 Se sei uno studente, puoi ottenere accesso all'Area Studenti verificando_la_tua
 identitÃ !
-""" # ==================================== # SUCCESS_MESSAGE_TEXT = """ Ti sei
-unito all'Area Studenti: benvenuto! Se in qualsiasi momento vuoi modificare o
-eliminare i tuoi dati salvati sul mio database, puoi accedervi dal tuo profilo
-privato: {profile_url} """ # language=html SUCCESS_MESSAGE_HTML = """
-Ti sei unito all'Area Studenti: benvenuto!
+""" # ==================================== # SUCCESS_MESSAGE_TEXT = """ â Ti
+sei unito all'Area Studenti: benvenuto! Se in qualsiasi momento vuoi modificare
+o eliminare i tuoi dati salvati sul mio database, puoi accedervi dal tuo
+profilo privato: {profile_url} """ # language=html SUCCESS_MESSAGE_HTML = """
+â Ti sei unito all'Area Studenti: benvenuto!
 Se in qualsiasi momento vuoi modificare o eliminare i tuoi dati salvati sul mio
 database, puoi accedervi_dal_tuo_profilo_privato!
-""" # ==================================== # GOODBYE_MESSAGE_TEXT = """ Hai
+""" # ==================================== # GOODBYE_MESSAGE_TEXT = """ â Hai
 abbandonato lo spazio Matrix dell'Unimore, quindi ho cancellato i tuoi dati dal
 mio database; a breve verrai inoltre rimosso da tutte le stanze dello spazio.
 Se cambierai idea in futuro, potrai sempre rientrare allo stesso indirizzo!
-Abbi un buon proseguimento di giornata! :) """ # language=html
+Abbi un buon proseguimento di giornata! """ # language=html
 GOODBYE_MESSAGE_HTML = """
-Hai abbandonato lo spazio Matrix dell'Unimore, quindi ho cancellato i tuoi dati
-dal mio database; a breve verrai inoltre rimosso da tutte le stanze dello
+â Hai abbandonato lo spazio Matrix dell'Unimore, quindi ho cancellato i tuoi
+dati dal mio database; a breve verrai inoltre rimosso da tutte le stanze dello
 spazio.
 Se cambierai idea in futuro, potrai sempre rientrare allo stesso indirizzo!
-Abbi un buon proseguimento di giornata! :)
-""" # ==================================== # UNLINK_MESSAGE_TEXT = """ Hai
+Abbi un buon proseguimento di giornata!
+""" # ==================================== # UNLINK_MESSAGE_TEXT = """ ð´ Hai
 abbandonato l'Area Studenti dello spazio Unimore, quindi ho scollegato il tuo
 account Studenti@Unimore dal tuo account Matrix. Se cambierai idea in futuro,
 potrai sempre essere riaggiunto all'Area Studenti ricollegando il tuo account:
-{profile_url} Abbi un buon proseguimento di giornata! :) """ # language=html
+{profile_url} Abbi un buon proseguimento di giornata! """ # language=html
 UNLINK_MESSAGE_HTML = """
-Hai abbandonato l'Area Studenti dello spazio Unimore, quindi ho scollegato il
-tuo account Studenti@Unimore dal tuo account Matrix.
+ð´ Hai abbandonato l'Area Studenti dello spazio Unimore, quindi ho scollegato
+il tuo account Studenti@Unimore dal tuo account Matrix.
 Se cambierai idea in futuro, potrai sempre essere riaggiunto all'Area Studenti
 ricollegando_il_tuo_account!
-Abbi un buon proseguimento di giornata! :)
+Abbi un buon proseguimento di giornata!
 """ # ==================================== # __all__ =
 ( "WELCOME_MESSAGE_TEXT", "WELCOME_MESSAGE_HTML", "SUCCESS_MESSAGE_TEXT",
 "SUCCESS_MESSAGE_HTML", "GOODBYE_MESSAGE_TEXT", "GOODBYE_MESSAGE_HTML",
 "UNLINK_MESSAGE_TEXT", "UNLINK_MESSAGE_HTML", )
```

### Comparing `lokiunimore-0.6.1/lokiunimore/utils/logs.py` & `lokiunimore-0.7.0/lokiunimore/utils/logs.py`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/web/app.py` & `lokiunimore-0.7.0/lokiunimore/web/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,16 +131,15 @@
         email=account.email,
         first_name=account.given_name,
         last_name=account.family_name,
     ))
 
     if matrix_token := flask.session.pop("matrix_token", None):
         matrix_user = sqla_extension.session.query(MatrixUser).filter_by(token=matrix_token).first_or_404()
-        matrix_user.account = local_account
-
+        matrix_user.link(session=sqla_extension.session, account=local_account)
         sqla_extension.session.commit()
 
         return flask.redirect(flask.url_for("page_matrix_invite", token=matrix_token))
 
     else:
         return flask.render_template("errors/no-link.html"), 403
```

### Comparing `lokiunimore-0.6.1/lokiunimore/web/extensions/matrix_client.py` & `lokiunimore-0.7.0/lokiunimore/web/extensions/matrix_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         token = hmac.new(
             key=app.config["MATRIX_USER_SECRET"].encode("utf8"),
             msg=app.config["MATRIX_USER_ID"].encode("utf8"),
             digestmod=hashlib.sha512
         ).hexdigest()
 
         response = requests.post(f"{app.config['MATRIX_HOMESERVER']}/_matrix/client/v3/login", json={
-            "type": "x.shared_secret_auth",
+            "type": "com.devture.shared_secret_auth",
             "identifier": {
                 "type": "m.id.user",
                 "user": app.config["MATRIX_USER_ID"],
             },
             "token": token,
             "initial_device_display_name": generate_device_name(__name__),
         })
```

### Comparing `lokiunimore-0.6.1/lokiunimore/web/static/favicon.ico` & `lokiunimore-0.7.0/lokiunimore/web/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/web/static/icon.png` & `lokiunimore-0.7.0/lokiunimore/web/static/icon.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/web/static/newcode.png` & `lokiunimore-0.7.0/lokiunimore/web/static/newcode.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/web/static/opengraph.png` & `lokiunimore-0.7.0/lokiunimore/web/static/opengraph.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/web/static/rooms.png` & `lokiunimore-0.7.0/lokiunimore/web/static/rooms.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/web/static/s-192.png` & `lokiunimore-0.7.0/lokiunimore/web/static/s-192.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/web/static/spaces.png` & `lokiunimore-0.7.0/lokiunimore/web/static/spaces.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/web/static/thor.png` & `lokiunimore-0.7.0/lokiunimore/web/static/thor.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/web/static/unimore.css` & `lokiunimore-0.7.0/lokiunimore/web/static/unimore.css`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/web/static/verify.png` & `lokiunimore-0.7.0/lokiunimore/web/static/verify.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/web/templates/_base.html` & `lokiunimore-0.7.0/lokiunimore/web/templates/_base.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/web/templates/errors/_base.html` & `lokiunimore-0.7.0/lokiunimore/web/templates/errors/_base.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/web/templates/errors/failed-invite.html` & `lokiunimore-0.7.0/lokiunimore/web/templates/errors/failed-invite.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/web/templates/errors/not-student.html` & `lokiunimore-0.7.0/lokiunimore/web/templates/errors/not-student.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/web/templates/errors/not-verified.html` & `lokiunimore-0.7.0/lokiunimore/web/templates/errors/not-verified.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/web/templates/matrix/complete.html` & `lokiunimore-0.7.0/lokiunimore/web/templates/matrix/complete.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/web/templates/matrix/join.html` & `lokiunimore-0.7.0/lokiunimore/web/templates/matrix/join.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/web/templates/matrix/verify.html` & `lokiunimore-0.7.0/lokiunimore/web/templates/matrix/verify.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/web/templates/privacy.html` & `lokiunimore-0.7.0/lokiunimore/web/templates/privacy.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/lokiunimore/web/templates/root.html` & `lokiunimore-0.7.0/lokiunimore/web/templates/root.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.6.1/pyproject.toml` & `lokiunimore-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # See https://python-poetry.org/docs/pyproject/ for more details!
 
 # The name of your project.
 # Ensure that it is available on PyPI: https://pypi.org/
 name = "lokiunimore"
 
 # The version of the package.
-version = "0.6.1"
+version = "0.7.0"
 
 # A brief, one-sentence description about your project.
 description = "Matrix room gatekeeper bot for the unofficial Unimore space"
 
 # A list of the authors of the project.
 authors = [
     "Stefano Pigozzi <me@steffo.eu>",
@@ -129,23 +129,23 @@
 # ~X.X.X means "newer releases with this minor version"
 #         ~3.10.1  →  == 3.10   && >= 3.10.1
 # nothing means "this specific release"
 #          3.10.1  →  == 3.10.1
 
 python = "^3.10"
 Flask = "^2.2.2"
-Flask-SQLAlchemy = "^2.5.1"
+Flask-SQLAlchemy = "^3.0.0"
 gunicorn = "^20.1.0"
 Authlib = "^1.0.1"
 requests = "^2.28.1"
 coloredlogs = "^15.0.1"
 psycopg2 = "^2.9.3"
 matrix-nio = "^0.20.1"
 cfig = {extras = ["cli"], version = "^0.3.0"}
-python-dotenv = "^0.21.0"
+python-dotenv = "^1.0.0"
 
 
 
 [tool.poetry.dev-dependencies]
 ##############################
 # Development dependencies   #
 ##############################
```

### Comparing `lokiunimore-0.6.1/PKG-INFO` & `lokiunimore-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lokiunimore
-Version: 0.6.1
+Version: 0.7.0
 Summary: Matrix room gatekeeper bot for the unofficial Unimore space
 Home-page: https://loki.steffo.eu/
 License: AGPL-3.0-or-later
 Keywords: bot,matrix,authentication,unimore,oauth2
 Author: Stefano Pigozzi
 Author-email: me@steffo.eu
 Maintainer: Stefano Pigozzi
@@ -14,28 +14,32 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Authlib (>=1.0.1,<2.0.0)
 Requires-Dist: Flask (>=2.2.2,<3.0.0)
-Requires-Dist: Flask-SQLAlchemy (>=2.5.1,<3.0.0)
+Requires-Dist: Flask-SQLAlchemy (>=3.0.0,<4.0.0)
 Requires-Dist: cfig[cli] (>=0.3.0,<0.4.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: matrix-nio (>=0.20.1,<0.21.0)
 Requires-Dist: psycopg2 (>=2.9.3,<3.0.0)
-Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Repository, https://github.com/Steffo99/lokiunimore
 Description-Content-Type: text/markdown
 
 # Loki Bot
 
-Gatekeeper bot for the Unimore Informatica unofficial Matrix space
+Gatekeeper bot for the Unimore Informatica unofficial Matrix space.
+
+## Links
+
+
 
 \[ [**Website**](https://loki.steffo.eu) | [PyPI](https://pypi.org/project/lokiunimore/) \]
 
 > TIP: You may be looking for its predecessor, [Thor Bot](https://github.com/Steffo99/thorunimore).
 
 ![](lokiunimore/web/static/opengraph.png)
 
@@ -104,13 +108,7 @@
 
 Run the image without any command to view and validate the current configuration.
 
 Run the image with the `gunicorn -b 0.0.0.0:80 lokiunimore.web.app:rp_app` command to launch the production web server on local port 80, expecting to be behind a  reverse proxy.
 
 Run the image with the `lokiunimore.matrix` command to launch the Matrix bot.
 
-### Using Docker Compose
-
-Use the [given Docker Compose file](docker-compose.yml).
-
-Either use [Portainer](https://www.portainer.io/), or start it manually using `docker compose up -d && docker compose logs -f`.
-
```

