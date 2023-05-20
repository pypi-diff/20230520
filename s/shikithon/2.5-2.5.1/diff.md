# Comparing `tmp/shikithon-2.5.tar.gz` & `tmp/shikithon-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shikithon-2.5.tar", max compression
+gzip compressed data, was "shikithon-2.5.1.tar", max compression
```

## Comparing `shikithon-2.5.tar` & `shikithon-2.5.1.tar`

### file list

```diff
@@ -1,135 +1,135 @@
--rw-r--r--   0        0        0     1075 2023-05-03 12:49:40.722659 shikithon-2.5/LICENSE
--rw-r--r--   0        0        0    12299 2023-05-03 12:49:40.722659 shikithon-2.5/README.md
--rw-r--r--   0        0        0     1220 2023-05-03 12:49:40.722659 shikithon-2.5/pyproject.toml
--rw-r--r--   0        0        0      260 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/__init__.py
--rw-r--r--   0        0        0     3958 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/api.py
--rw-r--r--   0        0        0    22018 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/base_client.py
--rw-r--r--   0        0        0      189 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/decorators/__init__.py
--rw-r--r--   0        0        0     2074 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/decorators/exceptions_handler.py
--rw-r--r--   0        0        0     1617 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/decorators/method_endpoint.py
--rw-r--r--   0        0        0    35815 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/endpoints.py
--rw-r--r--   0        0        0     1699 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/__init__.py
--rw-r--r--   0        0        0     2707 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/anime.py
--rw-r--r--   0        0        0      897 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/club.py
--rw-r--r--   0        0        0      634 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/comment.py
--rw-r--r--   0        0        0      312 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/enhanced_enum.py
--rw-r--r--   0        0        0      291 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/favorite.py
--rw-r--r--   0        0        0      225 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/history.py
--rw-r--r--   0        0        0     1963 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/manga.py
--rw-r--r--   0        0        0      289 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/message.py
--rw-r--r--   0        0        0      470 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/person.py
--rw-r--r--   0        0        0     1524 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/ranobe.py
--rw-r--r--   0        0        0      240 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/enums/request.py
--rw-r--r--   0        0        0      218 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/enums/response.py
--rw-r--r--   0        0        0      247 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/enums/review.py
--rw-r--r--   0        0        0      200 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/enums/style.py
--rw-r--r--   0        0        0     2001 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/enums/topic.py
--rw-r--r--   0        0        0      712 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/enums/user_rate.py
--rw-r--r--   0        0        0      382 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/enums/video.py
--rw-r--r--   0        0        0      657 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/exceptions/__init__.py
--rw-r--r--   0        0        0      276 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/exceptions/already_running_client.py
--rw-r--r--   0        0        0      329 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/exceptions/invalid_content_type.py
--rw-r--r--   0        0        0      732 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/exceptions/missing_app_variable.py
--rw-r--r--   0        0        0      231 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/exceptions/retry_later.py
--rw-r--r--   0        0        0      358 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/exceptions/shikimori_api_response_error.py
--rw-r--r--   0        0        0      240 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/exceptions/shikithon_exception.py
--rw-r--r--   0        0        0      235 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/exceptions/store_exception.py
--rw-r--r--   0        0        0     2167 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/__init__.py
--rw-r--r--   0        0        0      233 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/abuse_response.py
--rw-r--r--   0        0        0      306 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/achievement.py
--rw-r--r--   0        0        0      193 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/activity.py
--rw-r--r--   0        0        0     1676 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/anime.py
--rw-r--r--   0        0        0      433 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/ban.py
--rw-r--r--   0        0        0      342 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/calendar_event.py
--rw-r--r--   0        0        0      855 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/character.py
--rw-r--r--   0        0        0      803 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/club.py
--rw-r--r--   0        0        0      293 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/club_image.py
--rw-r--r--   0        0        0      590 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/comment.py
--rw-r--r--   0        0        0     1579 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/constants.py
--rw-r--r--   0        0        0      210 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/created_user_image.py
--rw-r--r--   0        0        0      727 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/critique.py
--rw-r--r--   0        0        0      276 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/date.py
--rw-r--r--   0        0        0      238 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/dialog.py
--rw-r--r--   0        0        0      246 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/favourite.py
--rw-r--r--   0        0        0      455 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/favourites.py
--rw-r--r--   0        0        0      199 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/forum.py
--rw-r--r--   0        0        0      330 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/franchise_tree.py
--rw-r--r--   0        0        0      228 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/genre.py
--rw-r--r--   0        0        0      428 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/history.py
--rw-r--r--   0        0        0      196 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/image.py
--rw-r--r--   0        0        0      417 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/link.py
--rw-r--r--   0        0        0      613 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/linked_topic.py
--rw-r--r--   0        0        0      202 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/logo.py
--rw-r--r--   0        0        0     1751 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/manga.py
--rw-r--r--   0        0        0      647 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/message.py
--rw-r--r--   0        0        0     1008 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/person.py
--rw-r--r--   0        0        0      161 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/publisher.py
--rw-r--r--   0        0        0     1663 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/ranobe.py
--rw-r--r--   0        0        0      164 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/rating.py
--rw-r--r--   0        0        0      280 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/rating_list.py
--rw-r--r--   0        0        0      406 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/relation.py
--rw-r--r--   0        0        0      578 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/review.py
--rw-r--r--   0        0        0      376 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/role.py
--rw-r--r--   0        0        0      290 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/roles.py
--rw-r--r--   0        0        0      161 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/score.py
--rw-r--r--   0        0        0      244 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/score_list.py
--rw-r--r--   0        0        0      174 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/screenshot.py
--rw-r--r--   0        0        0      237 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/seyu.py
--rw-r--r--   0        0        0      860 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/stats.py
--rw-r--r--   0        0        0      209 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/status.py
--rw-r--r--   0        0        0      249 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/status_list.py
--rw-r--r--   0        0        0      252 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/studio.py
--rw-r--r--   0        0        0      500 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/style.py
--rw-r--r--   0        0        0     1600 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/topic.py
--rw-r--r--   0        0        0      255 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/tree_link.py
--rw-r--r--   0        0        0      304 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/tree_node.py
--rw-r--r--   0        0        0      158 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/type.py
--rw-r--r--   0        0        0      238 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/type_list.py
--rw-r--r--   0        0        0      247 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/unread_messages.py
--rw-r--r--   0        0        0      903 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/user.py
--rw-r--r--   0        0        0      232 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/user_image.py
--rw-r--r--   0        0        0      726 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/user_list.py
--rw-r--r--   0        0        0      543 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/user_rate.py
--rw-r--r--   0        0        0      170 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/user_rate_score.py
--rw-r--r--   0        0        0      172 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/user_rate_status.py
--rw-r--r--   0        0        0      290 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/video.py
--rw-r--r--   0        0        0      355 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/works.py
--rw-r--r--   0        0        0        0 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/py.typed
--rw-r--r--   0        0        0     1338 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/__init__.py
--rw-r--r--   0        0        0     4706 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/abuse_requests.py
--rw-r--r--   0        0        0     1176 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/achievements.py
--rw-r--r--   0        0        0    14269 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/animes.py
--rw-r--r--   0        0        0     1160 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/appears.py
--rw-r--r--   0        0        0     1319 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/bans.py
--rw-r--r--   0        0        0      162 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/base_resource.py
--rw-r--r--   0        0        0     1294 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/calendars.py
--rw-r--r--   0        0        0     1839 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/characters.py
--rw-r--r--   0        0        0    13716 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/clubs.py
--rw-r--r--   0        0        0     6302 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/comments.py
--rw-r--r--   0        0        0     3218 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/constants.py
--rw-r--r--   0        0        0     2440 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/dialogs.py
--rw-r--r--   0        0        0     3684 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/favorites.py
--rw-r--r--   0        0        0      912 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/forums.py
--rw-r--r--   0        0        0     1483 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/friends.py
--rw-r--r--   0        0        0      911 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/genres.py
--rw-r--r--   0        0        0     9732 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/mangas.py
--rw-r--r--   0        0        0     6578 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/messages.py
--rw-r--r--   0        0        0     2028 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/people.py
--rw-r--r--   0        0        0      955 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/publishers.py
--rw-r--r--   0        0        0     9542 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/ranobes.py
--rw-r--r--   0        0        0     4380 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/reviews.py
--rw-r--r--   0        0        0      751 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/stats.py
--rw-r--r--   0        0        0      922 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/studios.py
--rw-r--r--   0        0        0     4153 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/styles.py
--rw-r--r--   0        0        0     9901 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/topics.py
--rw-r--r--   0        0        0     1536 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/user_images.py
--rw-r--r--   0        0        0    10959 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/user_rates.py
--rw-r--r--   0        0        0    15848 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/users.py
--rw-r--r--   0        0        0      217 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/store/__init__.py
--rw-r--r--   0        0        0     4116 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/store/base.py
--rw-r--r--   0        0        0     3142 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/store/json.py
--rw-r--r--   0        0        0     4427 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/store/memory.py
--rw-r--r--   0        0        0     1189 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/store/null.py
--rw-r--r--   0        0        0       82 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/utils/__init__.py
--rw-r--r--   0        0        0    13234 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/utils/utils.py
--rw-r--r--   0        0        0    13437 1970-01-01 00:00:00.000000 shikithon-2.5/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-20 15:28:00.718376 shikithon-2.5.1/LICENSE
+-rw-r--r--   0        0        0    12346 2023-05-20 15:28:00.718376 shikithon-2.5.1/README.md
+-rw-r--r--   0        0        0     1222 2023-05-20 15:28:00.722376 shikithon-2.5.1/pyproject.toml
+-rw-r--r--   0        0        0      262 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/__init__.py
+-rw-r--r--   0        0        0     3958 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/api.py
+-rw-r--r--   0        0        0    22038 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/base_client.py
+-rw-r--r--   0        0        0      189 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/decorators/__init__.py
+-rw-r--r--   0        0        0     2074 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/decorators/exceptions_handler.py
+-rw-r--r--   0        0        0     1617 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/decorators/method_endpoint.py
+-rw-r--r--   0        0        0    35815 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/endpoints.py
+-rw-r--r--   0        0        0     1699 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/enums/__init__.py
+-rw-r--r--   0        0        0     2707 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/enums/anime.py
+-rw-r--r--   0        0        0      897 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/enums/club.py
+-rw-r--r--   0        0        0      634 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/enums/comment.py
+-rw-r--r--   0        0        0      312 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/enums/enhanced_enum.py
+-rw-r--r--   0        0        0      291 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/enums/favorite.py
+-rw-r--r--   0        0        0      225 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/enums/history.py
+-rw-r--r--   0        0        0     1963 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/enums/manga.py
+-rw-r--r--   0        0        0      289 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/enums/message.py
+-rw-r--r--   0        0        0      470 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/enums/person.py
+-rw-r--r--   0        0        0     1524 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/enums/ranobe.py
+-rw-r--r--   0        0        0      240 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/enums/request.py
+-rw-r--r--   0        0        0      218 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/enums/response.py
+-rw-r--r--   0        0        0      247 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/enums/review.py
+-rw-r--r--   0        0        0      200 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/enums/style.py
+-rw-r--r--   0        0        0     2001 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/enums/topic.py
+-rw-r--r--   0        0        0      712 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/enums/user_rate.py
+-rw-r--r--   0        0        0      382 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/enums/video.py
+-rw-r--r--   0        0        0      657 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/exceptions/__init__.py
+-rw-r--r--   0        0        0      276 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/exceptions/already_running_client.py
+-rw-r--r--   0        0        0      329 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/exceptions/invalid_content_type.py
+-rw-r--r--   0        0        0      732 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/exceptions/missing_app_variable.py
+-rw-r--r--   0        0        0      231 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/exceptions/retry_later.py
+-rw-r--r--   0        0        0      358 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/exceptions/shikimori_api_response_error.py
+-rw-r--r--   0        0        0      240 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/exceptions/shikithon_exception.py
+-rw-r--r--   0        0        0      235 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/exceptions/store_exception.py
+-rw-r--r--   0        0        0     2167 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/__init__.py
+-rw-r--r--   0        0        0      233 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/abuse_response.py
+-rw-r--r--   0        0        0      306 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/achievement.py
+-rw-r--r--   0        0        0      193 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/activity.py
+-rw-r--r--   0        0        0     1676 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/anime.py
+-rw-r--r--   0        0        0      433 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/ban.py
+-rw-r--r--   0        0        0      342 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/calendar_event.py
+-rw-r--r--   0        0        0      855 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/character.py
+-rw-r--r--   0        0        0      803 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/club.py
+-rw-r--r--   0        0        0      293 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/club_image.py
+-rw-r--r--   0        0        0      590 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/comment.py
+-rw-r--r--   0        0        0     1579 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/constants.py
+-rw-r--r--   0        0        0      210 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/created_user_image.py
+-rw-r--r--   0        0        0      727 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/critique.py
+-rw-r--r--   0        0        0      276 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/date.py
+-rw-r--r--   0        0        0      238 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/dialog.py
+-rw-r--r--   0        0        0      246 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/favourite.py
+-rw-r--r--   0        0        0      455 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/favourites.py
+-rw-r--r--   0        0        0      199 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/forum.py
+-rw-r--r--   0        0        0      330 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/franchise_tree.py
+-rw-r--r--   0        0        0      228 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/genre.py
+-rw-r--r--   0        0        0      428 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/history.py
+-rw-r--r--   0        0        0      197 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/image.py
+-rw-r--r--   0        0        0      417 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/link.py
+-rw-r--r--   0        0        0      613 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/linked_topic.py
+-rw-r--r--   0        0        0      202 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/logo.py
+-rw-r--r--   0        0        0     1751 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/manga.py
+-rw-r--r--   0        0        0      647 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/message.py
+-rw-r--r--   0        0        0     1008 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/person.py
+-rw-r--r--   0        0        0      161 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/publisher.py
+-rw-r--r--   0        0        0     1663 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/ranobe.py
+-rw-r--r--   0        0        0      164 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/rating.py
+-rw-r--r--   0        0        0      280 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/rating_list.py
+-rw-r--r--   0        0        0      406 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/relation.py
+-rw-r--r--   0        0        0      578 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/review.py
+-rw-r--r--   0        0        0      376 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/role.py
+-rw-r--r--   0        0        0      290 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/roles.py
+-rw-r--r--   0        0        0      161 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/score.py
+-rw-r--r--   0        0        0      244 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/score_list.py
+-rw-r--r--   0        0        0      174 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/screenshot.py
+-rw-r--r--   0        0        0      237 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/seyu.py
+-rw-r--r--   0        0        0      860 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/stats.py
+-rw-r--r--   0        0        0      209 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/status.py
+-rw-r--r--   0        0        0      249 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/status_list.py
+-rw-r--r--   0        0        0      252 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/studio.py
+-rw-r--r--   0        0        0      500 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/style.py
+-rw-r--r--   0        0        0     1600 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/topic.py
+-rw-r--r--   0        0        0      255 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/tree_link.py
+-rw-r--r--   0        0        0      304 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/tree_node.py
+-rw-r--r--   0        0        0      158 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/type.py
+-rw-r--r--   0        0        0      238 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/type_list.py
+-rw-r--r--   0        0        0      247 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/unread_messages.py
+-rw-r--r--   0        0        0      903 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/user.py
+-rw-r--r--   0        0        0      232 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/user_image.py
+-rw-r--r--   0        0        0      726 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/user_list.py
+-rw-r--r--   0        0        0      543 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/user_rate.py
+-rw-r--r--   0        0        0      170 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/user_rate_score.py
+-rw-r--r--   0        0        0      172 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/user_rate_status.py
+-rw-r--r--   0        0        0      290 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/video.py
+-rw-r--r--   0        0        0      355 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/models/works.py
+-rw-r--r--   0        0        0        0 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/py.typed
+-rw-r--r--   0        0        0     1338 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/__init__.py
+-rw-r--r--   0        0        0     4706 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/abuse_requests.py
+-rw-r--r--   0        0        0     1176 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/achievements.py
+-rw-r--r--   0        0        0    14269 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/animes.py
+-rw-r--r--   0        0        0     1160 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/appears.py
+-rw-r--r--   0        0        0     1319 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/bans.py
+-rw-r--r--   0        0        0      162 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/base_resource.py
+-rw-r--r--   0        0        0     1294 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/calendars.py
+-rw-r--r--   0        0        0     1839 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/characters.py
+-rw-r--r--   0        0        0    13716 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/clubs.py
+-rw-r--r--   0        0        0     6302 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/comments.py
+-rw-r--r--   0        0        0     3218 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/constants.py
+-rw-r--r--   0        0        0     2440 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/dialogs.py
+-rw-r--r--   0        0        0     3684 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/favorites.py
+-rw-r--r--   0        0        0      912 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/forums.py
+-rw-r--r--   0        0        0     1483 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/friends.py
+-rw-r--r--   0        0        0      911 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/genres.py
+-rw-r--r--   0        0        0     9732 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/mangas.py
+-rw-r--r--   0        0        0     6578 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/messages.py
+-rw-r--r--   0        0        0     2028 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/people.py
+-rw-r--r--   0        0        0      955 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/publishers.py
+-rw-r--r--   0        0        0     9542 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/ranobes.py
+-rw-r--r--   0        0        0     4380 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/reviews.py
+-rw-r--r--   0        0        0      751 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/stats.py
+-rw-r--r--   0        0        0      922 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/studios.py
+-rw-r--r--   0        0        0     4153 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/styles.py
+-rw-r--r--   0        0        0     9901 2023-05-20 15:28:00.722376 shikithon-2.5.1/shikithon/resources/topics.py
+-rw-r--r--   0        0        0     1536 2023-05-20 15:28:00.726376 shikithon-2.5.1/shikithon/resources/user_images.py
+-rw-r--r--   0        0        0    10959 2023-05-20 15:28:00.726376 shikithon-2.5.1/shikithon/resources/user_rates.py
+-rw-r--r--   0        0        0    15848 2023-05-20 15:28:00.726376 shikithon-2.5.1/shikithon/resources/users.py
+-rw-r--r--   0        0        0      217 2023-05-20 15:28:00.726376 shikithon-2.5.1/shikithon/store/__init__.py
+-rw-r--r--   0        0        0     4116 2023-05-20 15:28:00.726376 shikithon-2.5.1/shikithon/store/base.py
+-rw-r--r--   0        0        0     3142 2023-05-20 15:28:00.726376 shikithon-2.5.1/shikithon/store/json.py
+-rw-r--r--   0        0        0     4427 2023-05-20 15:28:00.726376 shikithon-2.5.1/shikithon/store/memory.py
+-rw-r--r--   0        0        0     1189 2023-05-20 15:28:00.726376 shikithon-2.5.1/shikithon/store/null.py
+-rw-r--r--   0        0        0       82 2023-05-20 15:28:00.726376 shikithon-2.5.1/shikithon/utils/__init__.py
+-rw-r--r--   0        0        0    13856 2023-05-20 15:28:00.726376 shikithon-2.5.1/shikithon/utils/utils.py
+-rw-r--r--   0        0        0    13438 1970-01-01 00:00:00.000000 shikithon-2.5.1/PKG-INFO
```

### Comparing `shikithon-2.5/LICENSE` & `shikithon-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/README.md` & `shikithon-2.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 
 > Данная библиотека начинает свою поддержку с Python 3.8.10.
 
 ## Установка
 
 ```shell
 pip install shikithon
+
+# или используя Poetry
+poetry add shikithon
 ```
 
 ## Пример использования
 
 ```py
 import asyncio
 
@@ -81,15 +84,15 @@
     # Вариант 1
     async with api.auth(
         client_id=config["client_id"],
         client_secret=config["client_secret"],
         auth_code=config["auth_code"],
     ):
         print(await api.users.current())
-        # >> UserBrief(id=723052, nickname='SecondThundeR', ...
+        # >> id=723052, nickname='SecondThundeR', ...
 
     # Вариант 2
 
     # Создаем новый объект API
     # (По умолчанию используется NullStore в качестве хранилища)
     api_2 = ShikimoriAPI(app_name="...")
```

### Comparing `shikithon-2.5/pyproject.toml` & `shikithon-2.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shikithon"
-version = "2.5"
+version = "2.5.1"
 description = "Yet another Python wrapper for Shikimori API"
 authors = [
     "SecondThundeR <awayfromgalaxy@gmail.com>"
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/SecondThundeR/shikithon"
@@ -41,13 +41,13 @@
 validators ="^0.20.0"
 aiohttp = "^3.8.4"
 pyrate-limiter = "^2.10.0"
 backoff = "^2.2.1"
 typing-extensions = "^4.5.0"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^3.3.1"
-mypy = "^1.2.0"
+pre-commit = "^3.3.2"
+mypy = "^1.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shikithon-2.5/shikithon/api.py` & `shikithon-2.5.1/shikithon/api.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/base_client.py` & `shikithon-2.5.1/shikithon/base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -491,15 +491,15 @@
                 response = await self._session.delete(url,
                                                       json=data,
                                                       params=query)
             else:
                 logger.debug('Unknown request type passed. Returning None')
                 return None
 
-        await Utils.log_response_info(response)
+        await Utils.log_response_info(response, not output_logging)
 
         try:
             if response.status == 401 and self._is_protected_request(url):
                 await self._refresh_and_save_tokens()
                 return await self.request(url, data, form_data, query,
                                           request_type, output_logging)
             elif response.status == ResponseCode.RETRY_LATER.value:
```

### Comparing `shikithon-2.5/shikithon/decorators/exceptions_handler.py` & `shikithon-2.5.1/shikithon/decorators/exceptions_handler.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/decorators/method_endpoint.py` & `shikithon-2.5.1/shikithon/decorators/method_endpoint.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/endpoints.py` & `shikithon-2.5.1/shikithon/endpoints.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/enums/__init__.py` & `shikithon-2.5.1/shikithon/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/enums/anime.py` & `shikithon-2.5.1/shikithon/enums/anime.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/enums/club.py` & `shikithon-2.5.1/shikithon/enums/club.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/enums/comment.py` & `shikithon-2.5.1/shikithon/enums/comment.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/enums/manga.py` & `shikithon-2.5.1/shikithon/enums/manga.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/enums/ranobe.py` & `shikithon-2.5.1/shikithon/enums/ranobe.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/enums/topic.py` & `shikithon-2.5.1/shikithon/enums/topic.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/enums/user_rate.py` & `shikithon-2.5.1/shikithon/enums/user_rate.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/exceptions/__init__.py` & `shikithon-2.5.1/shikithon/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/exceptions/missing_app_variable.py` & `shikithon-2.5.1/shikithon/exceptions/missing_app_variable.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/models/__init__.py` & `shikithon-2.5.1/shikithon/models/__init__.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/models/anime.py` & `shikithon-2.5.1/shikithon/models/anime.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/models/character.py` & `shikithon-2.5.1/shikithon/models/character.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/models/club.py` & `shikithon-2.5.1/shikithon/models/club.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/models/comment.py` & `shikithon-2.5.1/shikithon/models/comment.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/models/constants.py` & `shikithon-2.5.1/shikithon/models/constants.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/models/critique.py` & `shikithon-2.5.1/shikithon/models/critique.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/models/linked_topic.py` & `shikithon-2.5.1/shikithon/models/linked_topic.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/models/manga.py` & `shikithon-2.5.1/shikithon/models/manga.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/models/message.py` & `shikithon-2.5.1/shikithon/models/message.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/models/person.py` & `shikithon-2.5.1/shikithon/models/person.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/models/ranobe.py` & `shikithon-2.5.1/shikithon/models/ranobe.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/models/review.py` & `shikithon-2.5.1/shikithon/models/review.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/models/stats.py` & `shikithon-2.5.1/shikithon/models/stats.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/models/topic.py` & `shikithon-2.5.1/shikithon/models/topic.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/models/user.py` & `shikithon-2.5.1/shikithon/models/user.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/models/user_list.py` & `shikithon-2.5.1/shikithon/models/user_list.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/models/user_rate.py` & `shikithon-2.5.1/shikithon/models/user_rate.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/__init__.py` & `shikithon-2.5.1/shikithon/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/abuse_requests.py` & `shikithon-2.5.1/shikithon/resources/abuse_requests.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/achievements.py` & `shikithon-2.5.1/shikithon/resources/achievements.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/animes.py` & `shikithon-2.5.1/shikithon/resources/animes.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/appears.py` & `shikithon-2.5.1/shikithon/resources/appears.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/bans.py` & `shikithon-2.5.1/shikithon/resources/bans.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/calendars.py` & `shikithon-2.5.1/shikithon/resources/calendars.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/characters.py` & `shikithon-2.5.1/shikithon/resources/characters.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/clubs.py` & `shikithon-2.5.1/shikithon/resources/clubs.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/comments.py` & `shikithon-2.5.1/shikithon/resources/comments.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/constants.py` & `shikithon-2.5.1/shikithon/resources/constants.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/dialogs.py` & `shikithon-2.5.1/shikithon/resources/dialogs.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/favorites.py` & `shikithon-2.5.1/shikithon/resources/favorites.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/forums.py` & `shikithon-2.5.1/shikithon/resources/forums.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/friends.py` & `shikithon-2.5.1/shikithon/resources/friends.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/genres.py` & `shikithon-2.5.1/shikithon/resources/genres.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/mangas.py` & `shikithon-2.5.1/shikithon/resources/mangas.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/messages.py` & `shikithon-2.5.1/shikithon/resources/messages.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/people.py` & `shikithon-2.5.1/shikithon/resources/people.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/publishers.py` & `shikithon-2.5.1/shikithon/resources/publishers.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/ranobes.py` & `shikithon-2.5.1/shikithon/resources/ranobes.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/reviews.py` & `shikithon-2.5.1/shikithon/resources/reviews.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/stats.py` & `shikithon-2.5.1/shikithon/resources/stats.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/studios.py` & `shikithon-2.5.1/shikithon/resources/studios.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/styles.py` & `shikithon-2.5.1/shikithon/resources/styles.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/topics.py` & `shikithon-2.5.1/shikithon/resources/topics.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/user_images.py` & `shikithon-2.5.1/shikithon/resources/user_images.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/user_rates.py` & `shikithon-2.5.1/shikithon/resources/user_rates.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/resources/users.py` & `shikithon-2.5.1/shikithon/resources/users.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/store/base.py` & `shikithon-2.5.1/shikithon/store/base.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/store/json.py` & `shikithon-2.5.1/shikithon/store/json.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/store/memory.py` & `shikithon-2.5.1/shikithon/store/memory.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/store/null.py` & `shikithon-2.5.1/shikithon/store/null.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5/shikithon/utils/utils.py` & `shikithon-2.5.1/shikithon/utils/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 from loguru import logger
 from pydantic import BaseModel, parse_obj_as
 from validators import url
 
 from ..enums import ResponseCode
 
 LOWER_LIMIT_NUMBER = 1
+CENSORED_FIELDS = (
+    'access_token',
+    'refresh_token',
+)
 M = TypeVar('M', bound=BaseModel)
 
 R = TypeVar('R')
 T = TypeVar('T')
 
 
 class Utils:
@@ -381,18 +385,31 @@
                     form_data.add_field(f'{key}[]', list_value)
             form_data.add_field(key, value)
 
         logger.debug('Successfully generated FormData object')
         return form_data
 
     @staticmethod
-    async def log_response_info(response: ClientResponse):
+    async def log_response_info(response: ClientResponse,
+                                remove_sensitive_data: Optional[bool] = False):
         """Logs response info.
 
         This method extracts response status, headers and data
 
         :param response: Response object
         :type response: ClientResponse
+
+        :param remove_sensitive_data: Boolean flag for censoring sensitive data
+        :type remove_sensitive_data: Optional[bool]
         """
         logger.debug(f'Response status: {response.status}')
         logger.debug(f'Response headers: {response.headers}')
-        logger.debug(f'Response data: {await response.text()}')
+        if not remove_sensitive_data:
+            logger.debug(f'Response data: {await response.text()}')
+            return
+
+        censored_response_data: Dict[str, Any] = await response.json()
+        for key in censored_response_data.keys():
+            if key in CENSORED_FIELDS:
+                censored_response_data[key] = '[REDACTED]'
+
+        logger.debug(f'Response data: {censored_response_data}')
```

### Comparing `shikithon-2.5/PKG-INFO` & `shikithon-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: shikithon
-Version: 2.5
+Version: 2.5.1
 Summary: Yet another Python wrapper for Shikimori API
 Home-page: https://github.com/SecondThundeR/shikithon
 License: MIT
 Keywords: Python,Shikimori,API
 Author: SecondThundeR
 Author-email: awayfromgalaxy@gmail.com
 Requires-Python: >=3.8.10,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyrate-limiter (>=2.10.0,<3.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
@@ -56,14 +55,17 @@
 
 > Данная библиотека начинает свою поддержку с Python 3.8.10.
 
 ## Установка
 
 ```shell
 pip install shikithon
+
+# или используя Poetry
+poetry add shikithon
 ```
 
 ## Пример использования
 
 ```py
 import asyncio
 
@@ -109,15 +111,15 @@
     # Вариант 1
     async with api.auth(
         client_id=config["client_id"],
         client_secret=config["client_secret"],
         auth_code=config["auth_code"],
     ):
         print(await api.users.current())
-        # >> UserBrief(id=723052, nickname='SecondThundeR', ...
+        # >> id=723052, nickname='SecondThundeR', ...
 
     # Вариант 2
 
     # Создаем новый объект API
     # (По умолчанию используется NullStore в качестве хранилища)
     api_2 = ShikimoriAPI(app_name="...")
```

